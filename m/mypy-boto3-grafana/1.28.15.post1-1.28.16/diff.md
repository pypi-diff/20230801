# Comparing `tmp/mypy-boto3-grafana-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-grafana-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-grafana-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:13 2023, max compression
+gzip compressed data, was "mypy-boto3-grafana-1.28.16.tar", last modified: Tue Aug  1 11:36:52 2023, max compression
```

## Comparing `mypy-boto3-grafana-1.28.15.post1.tar` & `mypy-boto3-grafana-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:13.081167 mypy-boto3-grafana-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:46:31.000000 mypy-boto3-grafana-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15523 2023-07-29 10:03:13.073167 mypy-boto3-grafana-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14023 2023-07-29 09:46:31.000000 mypy-boto3-grafana-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:13.073167 mypy-boto3-grafana-1.28.15.post1/mypy_boto3_grafana/
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-29 09:46:31.000000 mypy-boto3-grafana-1.28.15.post1/mypy_boto3_grafana/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-29 09:46:31.000000 mypy-boto3-grafana-1.28.15.post1/mypy_boto3_grafana/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-29 09:46:31.000000 mypy-boto3-grafana-1.28.15.post1/mypy_boto3_grafana/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18397 2023-07-29 09:46:31.000000 mypy-boto3-grafana-1.28.15.post1/mypy_boto3_grafana/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18368 2023-07-29 09:46:31.000000 mypy-boto3-grafana-1.28.15.post1/mypy_boto3_grafana/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-07-29 09:46:31.000000 mypy-boto3-grafana-1.28.15.post1/mypy_boto3_grafana/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9546 2023-07-29 09:46:31.000000 mypy-boto3-grafana-1.28.15.post1/mypy_boto3_grafana/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-07-29 09:46:31.000000 mypy-boto3-grafana-1.28.15.post1/mypy_boto3_grafana/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-07-29 09:46:31.000000 mypy-boto3-grafana-1.28.15.post1/mypy_boto3_grafana/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:46:31.000000 mypy-boto3-grafana-1.28.15.post1/mypy_boto3_grafana/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    22171 2023-07-29 09:46:32.000000 mypy-boto3-grafana-1.28.15.post1/mypy_boto3_grafana/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    22144 2023-07-29 09:46:31.000000 mypy-boto3-grafana-1.28.15.post1/mypy_boto3_grafana/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:46:31.000000 mypy-boto3-grafana-1.28.15.post1/mypy_boto3_grafana/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:13.073167 mypy-boto3-grafana-1.28.15.post1/mypy_boto3_grafana.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15523 2023-07-29 10:03:12.000000 mypy-boto3-grafana-1.28.15.post1/mypy_boto3_grafana.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-29 10:03:12.000000 mypy-boto3-grafana-1.28.15.post1/mypy_boto3_grafana.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:12.000000 mypy-boto3-grafana-1.28.15.post1/mypy_boto3_grafana.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:12.000000 mypy-boto3-grafana-1.28.15.post1/mypy_boto3_grafana.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:12.000000 mypy-boto3-grafana-1.28.15.post1/mypy_boto3_grafana.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-29 10:03:12.000000 mypy-boto3-grafana-1.28.15.post1/mypy_boto3_grafana.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:13.081167 mypy-boto3-grafana-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-29 09:46:30.000000 mypy-boto3-grafana-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:52.736880 mypy-boto3-grafana-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:19:08.000000 mypy-boto3-grafana-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15661 2023-08-01 11:36:52.736880 mypy-boto3-grafana-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14170 2023-08-01 11:19:08.000000 mypy-boto3-grafana-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:52.732880 mypy-boto3-grafana-1.28.16/mypy_boto3_grafana/
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-08-01 11:19:08.000000 mypy-boto3-grafana-1.28.16/mypy_boto3_grafana/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-08-01 11:19:08.000000 mypy-boto3-grafana-1.28.16/mypy_boto3_grafana/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-08-01 11:19:08.000000 mypy-boto3-grafana-1.28.16/mypy_boto3_grafana/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17948 2023-08-01 11:19:08.000000 mypy-boto3-grafana-1.28.16/mypy_boto3_grafana/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17919 2023-08-01 11:19:08.000000 mypy-boto3-grafana-1.28.16/mypy_boto3_grafana/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-08-01 11:19:08.000000 mypy-boto3-grafana-1.28.16/mypy_boto3_grafana/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9546 2023-08-01 11:19:08.000000 mypy-boto3-grafana-1.28.16/mypy_boto3_grafana/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-08-01 11:19:08.000000 mypy-boto3-grafana-1.28.16/mypy_boto3_grafana/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-08-01 11:19:08.000000 mypy-boto3-grafana-1.28.16/mypy_boto3_grafana/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:19:08.000000 mypy-boto3-grafana-1.28.16/mypy_boto3_grafana/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    22683 2023-08-01 11:19:09.000000 mypy-boto3-grafana-1.28.16/mypy_boto3_grafana/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22656 2023-08-01 11:19:09.000000 mypy-boto3-grafana-1.28.16/mypy_boto3_grafana/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:19:08.000000 mypy-boto3-grafana-1.28.16/mypy_boto3_grafana/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:52.736880 mypy-boto3-grafana-1.28.16/mypy_boto3_grafana.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15661 2023-08-01 11:36:52.000000 mypy-boto3-grafana-1.28.16/mypy_boto3_grafana.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-08-01 11:36:52.000000 mypy-boto3-grafana-1.28.16/mypy_boto3_grafana.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:52.000000 mypy-boto3-grafana-1.28.16/mypy_boto3_grafana.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:52.000000 mypy-boto3-grafana-1.28.16/mypy_boto3_grafana.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:52.000000 mypy-boto3-grafana-1.28.16/mypy_boto3_grafana.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-01 11:36:52.000000 mypy-boto3-grafana-1.28.16/mypy_boto3_grafana.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:52.736880 mypy-boto3-grafana-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-08-01 11:19:08.000000 mypy-boto3-grafana-1.28.16/setup.py
```

### Comparing `mypy-boto3-grafana-1.28.15.post1/LICENSE` & `mypy-boto3-grafana-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-grafana-1.28.15.post1/PKG-INFO` & `mypy-boto3-grafana-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-grafana
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.ManagedGrafana 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.ManagedGrafana 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 grafana type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 grafana type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-grafana.svg?color=blue)](https://pypi.org/project/mypy-boto3-grafana)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-grafana)](https://pepy.tech/project/mypy-boto3-grafana)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ManagedGrafana 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana)
+[boto3.ManagedGrafana 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana)
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
 [mypy-boto3-grafana docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/).
 
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
@@ -328,20 +328,20 @@
 )
 
 
 def check_value(value: AccountAccessTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_grafana.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_grafana.type_defs import (
     AssertionAttributesTypeDef,
     AssociateLicenseRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     AwsSsoAuthenticationTypeDef,
@@ -376,40 +376,44 @@
     ListVersionsResponseTypeDef,
     WorkspaceSummaryTypeDef,
     CreateWorkspaceRequestRequestTypeDef,
     UpdateWorkspaceRequestRequestTypeDef,
     ListPermissionsRequestListPermissionsPaginateTypeDef,
     ListVersionsRequestListVersionsPaginateTypeDef,
     ListWorkspacesRequestListWorkspacesPaginateTypeDef,
+    NetworkAccessConfigurationUnionTypeDef,
     PermissionEntryTypeDef,
     UpdateInstructionOutputTypeDef,
     UpdateInstructionTypeDef,
     SamlConfigurationOutputTypeDef,
     SamlConfigurationTypeDef,
+    VpcConfigurationUnionTypeDef,
     WorkspaceDescriptionTypeDef,
     ListWorkspacesResponseTypeDef,
     ListPermissionsResponseTypeDef,
     UpdateErrorTypeDef,
-    UpdatePermissionsRequestRequestTypeDef,
+    UpdateInstructionUnionTypeDef,
     SamlAuthenticationTypeDef,
+    SamlConfigurationUnionTypeDef,
     UpdateWorkspaceAuthenticationRequestRequestTypeDef,
     AssociateLicenseResponseTypeDef,
     CreateWorkspaceResponseTypeDef,
     DeleteWorkspaceResponseTypeDef,
     DescribeWorkspaceResponseTypeDef,
     DisassociateLicenseResponseTypeDef,
     UpdateWorkspaceResponseTypeDef,
     UpdatePermissionsResponseTypeDef,
+    UpdatePermissionsRequestRequestTypeDef,
     AuthenticationDescriptionTypeDef,
     DescribeWorkspaceAuthenticationResponseTypeDef,
     UpdateWorkspaceAuthenticationResponseTypeDef,
 )
 
 
-def get_structure() -> AssertionAttributesTypeDef:
+def get_value() -> AssertionAttributesTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-grafana-1.28.15.post1/README.md` & `mypy-boto3-grafana-1.28.16/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-grafana.svg?color=blue)](https://pypi.org/project/mypy-boto3-grafana)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-grafana)](https://pepy.tech/project/mypy-boto3-grafana)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ManagedGrafana 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana)
+[boto3.ManagedGrafana 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana)
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
 [mypy-boto3-grafana docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/).
 
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
@@ -296,20 +296,20 @@
 )
 
 
 def check_value(value: AccountAccessTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_grafana.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_grafana.type_defs import (
     AssertionAttributesTypeDef,
     AssociateLicenseRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     AwsSsoAuthenticationTypeDef,
@@ -344,40 +344,44 @@
     ListVersionsResponseTypeDef,
     WorkspaceSummaryTypeDef,
     CreateWorkspaceRequestRequestTypeDef,
     UpdateWorkspaceRequestRequestTypeDef,
     ListPermissionsRequestListPermissionsPaginateTypeDef,
     ListVersionsRequestListVersionsPaginateTypeDef,
     ListWorkspacesRequestListWorkspacesPaginateTypeDef,
+    NetworkAccessConfigurationUnionTypeDef,
     PermissionEntryTypeDef,
     UpdateInstructionOutputTypeDef,
     UpdateInstructionTypeDef,
     SamlConfigurationOutputTypeDef,
     SamlConfigurationTypeDef,
+    VpcConfigurationUnionTypeDef,
     WorkspaceDescriptionTypeDef,
     ListWorkspacesResponseTypeDef,
     ListPermissionsResponseTypeDef,
     UpdateErrorTypeDef,
-    UpdatePermissionsRequestRequestTypeDef,
+    UpdateInstructionUnionTypeDef,
     SamlAuthenticationTypeDef,
+    SamlConfigurationUnionTypeDef,
     UpdateWorkspaceAuthenticationRequestRequestTypeDef,
     AssociateLicenseResponseTypeDef,
     CreateWorkspaceResponseTypeDef,
     DeleteWorkspaceResponseTypeDef,
     DescribeWorkspaceResponseTypeDef,
     DisassociateLicenseResponseTypeDef,
     UpdateWorkspaceResponseTypeDef,
     UpdatePermissionsResponseTypeDef,
+    UpdatePermissionsRequestRequestTypeDef,
     AuthenticationDescriptionTypeDef,
     DescribeWorkspaceAuthenticationResponseTypeDef,
     UpdateWorkspaceAuthenticationResponseTypeDef,
 )
 
 
-def get_structure() -> AssertionAttributesTypeDef:
+def get_value() -> AssertionAttributesTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-grafana-1.28.15.post1/mypy_boto3_grafana/__init__.py` & `mypy-boto3-grafana-1.28.16/mypy_boto3_grafana/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-grafana-1.28.15.post1/mypy_boto3_grafana/__init__.pyi` & `mypy-boto3-grafana-1.28.16/mypy_boto3_grafana/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-grafana-1.28.15.post1/mypy_boto3_grafana/__main__.py` & `mypy-boto3-grafana-1.28.16/mypy_boto3_grafana/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ManagedGrafana 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.ManagedGrafana 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana\nOther"
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

### Comparing `mypy-boto3-grafana-1.28.15.post1/mypy_boto3_grafana/client.py` & `mypy-boto3-grafana-1.28.16/mypy_boto3_grafana/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_grafana.client import ManagedGrafanaClient
 
     session = Session()
     client: ManagedGrafanaClient = session.client("grafana")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AccountAccessTypeType,
     AuthenticationProviderTypesType,
     DataSourceTypeType,
@@ -37,25 +37,21 @@
     DescribeWorkspaceConfigurationResponseTypeDef,
     DescribeWorkspaceResponseTypeDef,
     DisassociateLicenseResponseTypeDef,
     ListPermissionsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListVersionsResponseTypeDef,
     ListWorkspacesResponseTypeDef,
-    NetworkAccessConfigurationOutputTypeDef,
-    NetworkAccessConfigurationTypeDef,
-    SamlConfigurationOutputTypeDef,
-    SamlConfigurationTypeDef,
-    UpdateInstructionOutputTypeDef,
-    UpdateInstructionTypeDef,
+    NetworkAccessConfigurationUnionTypeDef,
+    SamlConfigurationUnionTypeDef,
+    UpdateInstructionUnionTypeDef,
     UpdatePermissionsResponseTypeDef,
     UpdateWorkspaceAuthenticationResponseTypeDef,
     UpdateWorkspaceResponseTypeDef,
-    VpcConfigurationOutputTypeDef,
-    VpcConfigurationTypeDef,
+    VpcConfigurationUnionTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -130,21 +126,19 @@
         *,
         accountAccessType: AccountAccessTypeType,
         authenticationProviders: Sequence[AuthenticationProviderTypesType],
         permissionType: PermissionTypeType,
         clientToken: str = ...,
         configuration: str = ...,
         grafanaVersion: str = ...,
-        networkAccessControl: Union[
-            NetworkAccessConfigurationTypeDef, NetworkAccessConfigurationOutputTypeDef
-        ] = ...,
+        networkAccessControl: NetworkAccessConfigurationUnionTypeDef = ...,
         organizationRoleName: str = ...,
         stackSetName: str = ...,
         tags: Mapping[str, str] = ...,
-        vpcConfiguration: Union[VpcConfigurationTypeDef, VpcConfigurationOutputTypeDef] = ...,
+        vpcConfiguration: VpcConfigurationUnionTypeDef = ...,
         workspaceDataSources: Sequence[DataSourceTypeType] = ...,
         workspaceDescription: str = ...,
         workspaceName: str = ...,
         workspaceNotificationDestinations: Sequence[Literal["SNS"]] = ...,
         workspaceOrganizationalUnits: Sequence[str] = ...,
         workspaceRoleArn: str = ...
     ) -> CreateWorkspaceResponseTypeDef:
@@ -299,42 +293,35 @@
         Managed Grafana resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/client/#untag_resource)
         """
 
     def update_permissions(
-        self,
-        *,
-        updateInstructionBatch: Sequence[
-            Union[UpdateInstructionTypeDef, UpdateInstructionOutputTypeDef]
-        ],
-        workspaceId: str
+        self, *, updateInstructionBatch: Sequence[UpdateInstructionUnionTypeDef], workspaceId: str
     ) -> UpdatePermissionsResponseTypeDef:
         """
         Updates which users in a workspace have the Grafana `Admin` or `Editor` roles.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.update_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/client/#update_permissions)
         """
 
     def update_workspace(
         self,
         *,
         workspaceId: str,
         accountAccessType: AccountAccessTypeType = ...,
-        networkAccessControl: Union[
-            NetworkAccessConfigurationTypeDef, NetworkAccessConfigurationOutputTypeDef
-        ] = ...,
+        networkAccessControl: NetworkAccessConfigurationUnionTypeDef = ...,
         organizationRoleName: str = ...,
         permissionType: PermissionTypeType = ...,
         removeNetworkAccessConfiguration: bool = ...,
         removeVpcConfiguration: bool = ...,
         stackSetName: str = ...,
-        vpcConfiguration: Union[VpcConfigurationTypeDef, VpcConfigurationOutputTypeDef] = ...,
+        vpcConfiguration: VpcConfigurationUnionTypeDef = ...,
         workspaceDataSources: Sequence[DataSourceTypeType] = ...,
         workspaceDescription: str = ...,
         workspaceName: str = ...,
         workspaceNotificationDestinations: Sequence[Literal["SNS"]] = ...,
         workspaceOrganizationalUnits: Sequence[str] = ...,
         workspaceRoleArn: str = ...
     ) -> UpdateWorkspaceResponseTypeDef:
@@ -346,15 +333,15 @@
         """
 
     def update_workspace_authentication(
         self,
         *,
         authenticationProviders: Sequence[AuthenticationProviderTypesType],
         workspaceId: str,
-        samlConfiguration: Union[SamlConfigurationTypeDef, SamlConfigurationOutputTypeDef] = ...
+        samlConfiguration: SamlConfigurationUnionTypeDef = ...
     ) -> UpdateWorkspaceAuthenticationResponseTypeDef:
         """
         Use this operation to define the identity provider (IdP) that this workspace
         authenticates users from, using SAML.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.update_workspace_authentication)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/client/#update_workspace_authentication)
```

### Comparing `mypy-boto3-grafana-1.28.15.post1/mypy_boto3_grafana/client.pyi` & `mypy-boto3-grafana-1.28.16/mypy_boto3_grafana/client.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_grafana.client import ManagedGrafanaClient
 
     session = Session()
     client: ManagedGrafanaClient = session.client("grafana")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AccountAccessTypeType,
     AuthenticationProviderTypesType,
     DataSourceTypeType,
@@ -37,25 +37,21 @@
     DescribeWorkspaceConfigurationResponseTypeDef,
     DescribeWorkspaceResponseTypeDef,
     DisassociateLicenseResponseTypeDef,
     ListPermissionsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListVersionsResponseTypeDef,
     ListWorkspacesResponseTypeDef,
-    NetworkAccessConfigurationOutputTypeDef,
-    NetworkAccessConfigurationTypeDef,
-    SamlConfigurationOutputTypeDef,
-    SamlConfigurationTypeDef,
-    UpdateInstructionOutputTypeDef,
-    UpdateInstructionTypeDef,
+    NetworkAccessConfigurationUnionTypeDef,
+    SamlConfigurationUnionTypeDef,
+    UpdateInstructionUnionTypeDef,
     UpdatePermissionsResponseTypeDef,
     UpdateWorkspaceAuthenticationResponseTypeDef,
     UpdateWorkspaceResponseTypeDef,
-    VpcConfigurationOutputTypeDef,
-    VpcConfigurationTypeDef,
+    VpcConfigurationUnionTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -122,21 +118,19 @@
         *,
         accountAccessType: AccountAccessTypeType,
         authenticationProviders: Sequence[AuthenticationProviderTypesType],
         permissionType: PermissionTypeType,
         clientToken: str = ...,
         configuration: str = ...,
         grafanaVersion: str = ...,
-        networkAccessControl: Union[
-            NetworkAccessConfigurationTypeDef, NetworkAccessConfigurationOutputTypeDef
-        ] = ...,
+        networkAccessControl: NetworkAccessConfigurationUnionTypeDef = ...,
         organizationRoleName: str = ...,
         stackSetName: str = ...,
         tags: Mapping[str, str] = ...,
-        vpcConfiguration: Union[VpcConfigurationTypeDef, VpcConfigurationOutputTypeDef] = ...,
+        vpcConfiguration: VpcConfigurationUnionTypeDef = ...,
         workspaceDataSources: Sequence[DataSourceTypeType] = ...,
         workspaceDescription: str = ...,
         workspaceName: str = ...,
         workspaceNotificationDestinations: Sequence[Literal["SNS"]] = ...,
         workspaceOrganizationalUnits: Sequence[str] = ...,
         workspaceRoleArn: str = ...
     ) -> CreateWorkspaceResponseTypeDef:
@@ -276,41 +270,34 @@
         The `UntagResource` operation removes the association of the tag with the Amazon
         Managed Grafana resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/client/#untag_resource)
         """
     def update_permissions(
-        self,
-        *,
-        updateInstructionBatch: Sequence[
-            Union[UpdateInstructionTypeDef, UpdateInstructionOutputTypeDef]
-        ],
-        workspaceId: str
+        self, *, updateInstructionBatch: Sequence[UpdateInstructionUnionTypeDef], workspaceId: str
     ) -> UpdatePermissionsResponseTypeDef:
         """
         Updates which users in a workspace have the Grafana `Admin` or `Editor` roles.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.update_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/client/#update_permissions)
         """
     def update_workspace(
         self,
         *,
         workspaceId: str,
         accountAccessType: AccountAccessTypeType = ...,
-        networkAccessControl: Union[
-            NetworkAccessConfigurationTypeDef, NetworkAccessConfigurationOutputTypeDef
-        ] = ...,
+        networkAccessControl: NetworkAccessConfigurationUnionTypeDef = ...,
         organizationRoleName: str = ...,
         permissionType: PermissionTypeType = ...,
         removeNetworkAccessConfiguration: bool = ...,
         removeVpcConfiguration: bool = ...,
         stackSetName: str = ...,
-        vpcConfiguration: Union[VpcConfigurationTypeDef, VpcConfigurationOutputTypeDef] = ...,
+        vpcConfiguration: VpcConfigurationUnionTypeDef = ...,
         workspaceDataSources: Sequence[DataSourceTypeType] = ...,
         workspaceDescription: str = ...,
         workspaceName: str = ...,
         workspaceNotificationDestinations: Sequence[Literal["SNS"]] = ...,
         workspaceOrganizationalUnits: Sequence[str] = ...,
         workspaceRoleArn: str = ...
     ) -> UpdateWorkspaceResponseTypeDef:
@@ -321,15 +308,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/client/#update_workspace)
         """
     def update_workspace_authentication(
         self,
         *,
         authenticationProviders: Sequence[AuthenticationProviderTypesType],
         workspaceId: str,
-        samlConfiguration: Union[SamlConfigurationTypeDef, SamlConfigurationOutputTypeDef] = ...
+        samlConfiguration: SamlConfigurationUnionTypeDef = ...
     ) -> UpdateWorkspaceAuthenticationResponseTypeDef:
         """
         Use this operation to define the identity provider (IdP) that this workspace
         authenticates users from, using SAML.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.update_workspace_authentication)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/client/#update_workspace_authentication)
```

### Comparing `mypy-boto3-grafana-1.28.15.post1/mypy_boto3_grafana/literals.py` & `mypy-boto3-grafana-1.28.16/mypy_boto3_grafana/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-grafana-1.28.15.post1/mypy_boto3_grafana/literals.pyi` & `mypy-boto3-grafana-1.28.16/mypy_boto3_grafana/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-grafana-1.28.15.post1/mypy_boto3_grafana/paginator.py` & `mypy-boto3-grafana-1.28.16/mypy_boto3_grafana/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-grafana-1.28.15.post1/mypy_boto3_grafana/paginator.pyi` & `mypy-boto3-grafana-1.28.16/mypy_boto3_grafana/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-grafana-1.28.15.post1/mypy_boto3_grafana/type_defs.py` & `mypy-boto3-grafana-1.28.16/mypy_boto3_grafana/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_grafana.type_defs import AssertionAttributesTypeDef
 
-    data: AssertionAttributesTypeDef = {...}
+    data: AssertionAttributesTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -33,15 +33,14 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AssertionAttributesTypeDef",
     "AssociateLicenseRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AwsSsoAuthenticationTypeDef",
     "AuthenticationSummaryTypeDef",
     "CreateWorkspaceApiKeyRequestRequestTypeDef",
@@ -74,33 +73,37 @@
     "ListVersionsResponseTypeDef",
     "WorkspaceSummaryTypeDef",
     "CreateWorkspaceRequestRequestTypeDef",
     "UpdateWorkspaceRequestRequestTypeDef",
     "ListPermissionsRequestListPermissionsPaginateTypeDef",
     "ListVersionsRequestListVersionsPaginateTypeDef",
     "ListWorkspacesRequestListWorkspacesPaginateTypeDef",
+    "NetworkAccessConfigurationUnionTypeDef",
     "PermissionEntryTypeDef",
     "UpdateInstructionOutputTypeDef",
     "UpdateInstructionTypeDef",
     "SamlConfigurationOutputTypeDef",
     "SamlConfigurationTypeDef",
+    "VpcConfigurationUnionTypeDef",
     "WorkspaceDescriptionTypeDef",
     "ListWorkspacesResponseTypeDef",
     "ListPermissionsResponseTypeDef",
     "UpdateErrorTypeDef",
-    "UpdatePermissionsRequestRequestTypeDef",
+    "UpdateInstructionUnionTypeDef",
     "SamlAuthenticationTypeDef",
+    "SamlConfigurationUnionTypeDef",
     "UpdateWorkspaceAuthenticationRequestRequestTypeDef",
     "AssociateLicenseResponseTypeDef",
     "CreateWorkspaceResponseTypeDef",
     "DeleteWorkspaceResponseTypeDef",
     "DescribeWorkspaceResponseTypeDef",
     "DisassociateLicenseResponseTypeDef",
     "UpdateWorkspaceResponseTypeDef",
     "UpdatePermissionsResponseTypeDef",
+    "UpdatePermissionsRequestRequestTypeDef",
     "AuthenticationDescriptionTypeDef",
     "DescribeWorkspaceAuthenticationResponseTypeDef",
     "UpdateWorkspaceAuthenticationResponseTypeDef",
 )
 
 AssertionAttributesTypeDef = TypedDict(
     "AssertionAttributesTypeDef",
@@ -152,21 +155,19 @@
     "_OptionalAuthenticationSummaryTypeDef",
     {
         "samlConfigurationStatus": SamlConfigurationStatusType,
     },
     total=False,
 )
 
-
 class AuthenticationSummaryTypeDef(
     _RequiredAuthenticationSummaryTypeDef, _OptionalAuthenticationSummaryTypeDef
 ):
     pass
 
-
 CreateWorkspaceApiKeyRequestRequestTypeDef = TypedDict(
     "CreateWorkspaceApiKeyRequestRequestTypeDef",
     {
         "keyName": str,
         "keyRole": str,
         "secondsToLive": int,
         "workspaceId": str,
@@ -266,21 +267,19 @@
         "nextToken": str,
         "userId": str,
         "userType": UserTypeType,
     },
     total=False,
 )
 
-
 class ListPermissionsRequestRequestTypeDef(
     _RequiredListPermissionsRequestRequestTypeDef, _OptionalListPermissionsRequestRequestTypeDef
 ):
     pass
 
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
@@ -364,22 +363,20 @@
     "_OptionalUpdateWorkspaceConfigurationRequestRequestTypeDef",
     {
         "grafanaVersion": str,
     },
     total=False,
 )
 
-
 class UpdateWorkspaceConfigurationRequestRequestTypeDef(
     _RequiredUpdateWorkspaceConfigurationRequestRequestTypeDef,
     _OptionalUpdateWorkspaceConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 VpcConfigurationOutputTypeDef = TypedDict(
     "VpcConfigurationOutputTypeDef",
     {
         "securityGroupIds": List[str],
         "subnetIds": List[str],
     },
 )
@@ -448,19 +445,17 @@
         "name": str,
         "notificationDestinations": List[Literal["SNS"]],
         "tags": Dict[str, str],
     },
     total=False,
 )
 
-
 class WorkspaceSummaryTypeDef(_RequiredWorkspaceSummaryTypeDef, _OptionalWorkspaceSummaryTypeDef):
     pass
 
-
 _RequiredCreateWorkspaceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorkspaceRequestRequestTypeDef",
     {
         "accountAccessType": AccountAccessTypeType,
         "authenticationProviders": Sequence[AuthenticationProviderTypesType],
         "permissionType": PermissionTypeType,
     },
@@ -482,21 +477,19 @@
         "workspaceNotificationDestinations": Sequence[Literal["SNS"]],
         "workspaceOrganizationalUnits": Sequence[str],
         "workspaceRoleArn": str,
     },
     total=False,
 )
 
-
 class CreateWorkspaceRequestRequestTypeDef(
     _RequiredCreateWorkspaceRequestRequestTypeDef, _OptionalCreateWorkspaceRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateWorkspaceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateWorkspaceRequestRequestTypeDef",
     {
         "workspaceId": str,
     },
 )
 _OptionalUpdateWorkspaceRequestRequestTypeDef = TypedDict(
@@ -516,21 +509,19 @@
         "workspaceNotificationDestinations": Sequence[Literal["SNS"]],
         "workspaceOrganizationalUnits": Sequence[str],
         "workspaceRoleArn": str,
     },
     total=False,
 )
 
-
 class UpdateWorkspaceRequestRequestTypeDef(
     _RequiredUpdateWorkspaceRequestRequestTypeDef, _OptionalUpdateWorkspaceRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredListPermissionsRequestListPermissionsPaginateTypeDef = TypedDict(
     "_RequiredListPermissionsRequestListPermissionsPaginateTypeDef",
     {
         "workspaceId": str,
     },
 )
 _OptionalListPermissionsRequestListPermissionsPaginateTypeDef = TypedDict(
@@ -540,22 +531,20 @@
         "userId": str,
         "userType": UserTypeType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListPermissionsRequestListPermissionsPaginateTypeDef(
     _RequiredListPermissionsRequestListPermissionsPaginateTypeDef,
     _OptionalListPermissionsRequestListPermissionsPaginateTypeDef,
 ):
     pass
 
-
 ListVersionsRequestListVersionsPaginateTypeDef = TypedDict(
     "ListVersionsRequestListVersionsPaginateTypeDef",
     {
         "workspaceId": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -565,14 +554,17 @@
     "ListWorkspacesRequestListWorkspacesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+NetworkAccessConfigurationUnionTypeDef = Union[
+    NetworkAccessConfigurationTypeDef, NetworkAccessConfigurationOutputTypeDef
+]
 PermissionEntryTypeDef = TypedDict(
     "PermissionEntryTypeDef",
     {
         "role": RoleType,
         "user": UserTypeDef,
     },
 )
@@ -608,21 +600,19 @@
         "assertionAttributes": AssertionAttributesTypeDef,
         "loginValidityDuration": int,
         "roleValues": RoleValuesOutputTypeDef,
     },
     total=False,
 )
 
-
 class SamlConfigurationOutputTypeDef(
     _RequiredSamlConfigurationOutputTypeDef, _OptionalSamlConfigurationOutputTypeDef
 ):
     pass
 
-
 _RequiredSamlConfigurationTypeDef = TypedDict(
     "_RequiredSamlConfigurationTypeDef",
     {
         "idpMetadata": IdpMetadataTypeDef,
     },
 )
 _OptionalSamlConfigurationTypeDef = TypedDict(
@@ -632,21 +622,20 @@
         "assertionAttributes": AssertionAttributesTypeDef,
         "loginValidityDuration": int,
         "roleValues": RoleValuesTypeDef,
     },
     total=False,
 )
 
-
 class SamlConfigurationTypeDef(
     _RequiredSamlConfigurationTypeDef, _OptionalSamlConfigurationTypeDef
 ):
     pass
 
-
+VpcConfigurationUnionTypeDef = Union[VpcConfigurationTypeDef, VpcConfigurationOutputTypeDef]
 _RequiredWorkspaceDescriptionTypeDef = TypedDict(
     "_RequiredWorkspaceDescriptionTypeDef",
     {
         "authentication": AuthenticationSummaryTypeDef,
         "created": datetime,
         "dataSources": List[DataSourceTypeType],
         "endpoint": str,
@@ -675,21 +664,19 @@
         "tags": Dict[str, str],
         "vpcConfiguration": VpcConfigurationOutputTypeDef,
         "workspaceRoleArn": str,
     },
     total=False,
 )
 
-
 class WorkspaceDescriptionTypeDef(
     _RequiredWorkspaceDescriptionTypeDef, _OptionalWorkspaceDescriptionTypeDef
 ):
     pass
 
-
 ListWorkspacesResponseTypeDef = TypedDict(
     "ListWorkspacesResponseTypeDef",
     {
         "nextToken": str,
         "workspaces": List[WorkspaceSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -709,45 +696,35 @@
     {
         "causedBy": UpdateInstructionOutputTypeDef,
         "code": int,
         "message": str,
     },
 )
 
-UpdatePermissionsRequestRequestTypeDef = TypedDict(
-    "UpdatePermissionsRequestRequestTypeDef",
-    {
-        "updateInstructionBatch": Sequence[
-            Union[UpdateInstructionTypeDef, UpdateInstructionOutputTypeDef]
-        ],
-        "workspaceId": str,
-    },
-)
-
+UpdateInstructionUnionTypeDef = Union[UpdateInstructionTypeDef, UpdateInstructionOutputTypeDef]
 _RequiredSamlAuthenticationTypeDef = TypedDict(
     "_RequiredSamlAuthenticationTypeDef",
     {
         "status": SamlConfigurationStatusType,
     },
 )
 _OptionalSamlAuthenticationTypeDef = TypedDict(
     "_OptionalSamlAuthenticationTypeDef",
     {
         "configuration": SamlConfigurationOutputTypeDef,
     },
     total=False,
 )
 
-
 class SamlAuthenticationTypeDef(
     _RequiredSamlAuthenticationTypeDef, _OptionalSamlAuthenticationTypeDef
 ):
     pass
 
-
+SamlConfigurationUnionTypeDef = Union[SamlConfigurationTypeDef, SamlConfigurationOutputTypeDef]
 _RequiredUpdateWorkspaceAuthenticationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateWorkspaceAuthenticationRequestRequestTypeDef",
     {
         "authenticationProviders": Sequence[AuthenticationProviderTypesType],
         "workspaceId": str,
     },
 )
@@ -755,22 +732,20 @@
     "_OptionalUpdateWorkspaceAuthenticationRequestRequestTypeDef",
     {
         "samlConfiguration": SamlConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class UpdateWorkspaceAuthenticationRequestRequestTypeDef(
     _RequiredUpdateWorkspaceAuthenticationRequestRequestTypeDef,
     _OptionalUpdateWorkspaceAuthenticationRequestRequestTypeDef,
 ):
     pass
 
-
 AssociateLicenseResponseTypeDef = TypedDict(
     "AssociateLicenseResponseTypeDef",
     {
         "workspace": WorkspaceDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -819,14 +794,22 @@
     "UpdatePermissionsResponseTypeDef",
     {
         "errors": List[UpdateErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+UpdatePermissionsRequestRequestTypeDef = TypedDict(
+    "UpdatePermissionsRequestRequestTypeDef",
+    {
+        "updateInstructionBatch": Sequence[UpdateInstructionUnionTypeDef],
+        "workspaceId": str,
+    },
+)
+
 _RequiredAuthenticationDescriptionTypeDef = TypedDict(
     "_RequiredAuthenticationDescriptionTypeDef",
     {
         "providers": List[AuthenticationProviderTypesType],
     },
 )
 _OptionalAuthenticationDescriptionTypeDef = TypedDict(
@@ -834,21 +817,19 @@
     {
         "awsSso": AwsSsoAuthenticationTypeDef,
         "saml": SamlAuthenticationTypeDef,
     },
     total=False,
 )
 
-
 class AuthenticationDescriptionTypeDef(
     _RequiredAuthenticationDescriptionTypeDef, _OptionalAuthenticationDescriptionTypeDef
 ):
     pass
 
-
 DescribeWorkspaceAuthenticationResponseTypeDef = TypedDict(
     "DescribeWorkspaceAuthenticationResponseTypeDef",
     {
         "authentication": AuthenticationDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-grafana-1.28.15.post1/mypy_boto3_grafana/type_defs.pyi` & `mypy-boto3-grafana-1.28.16/mypy_boto3_grafana/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_grafana.type_defs import AssertionAttributesTypeDef
 
-    data: AssertionAttributesTypeDef = {...}
+    data: AssertionAttributesTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -33,14 +33,15 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AssertionAttributesTypeDef",
     "AssociateLicenseRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AwsSsoAuthenticationTypeDef",
     "AuthenticationSummaryTypeDef",
     "CreateWorkspaceApiKeyRequestRequestTypeDef",
@@ -73,33 +74,37 @@
     "ListVersionsResponseTypeDef",
     "WorkspaceSummaryTypeDef",
     "CreateWorkspaceRequestRequestTypeDef",
     "UpdateWorkspaceRequestRequestTypeDef",
     "ListPermissionsRequestListPermissionsPaginateTypeDef",
     "ListVersionsRequestListVersionsPaginateTypeDef",
     "ListWorkspacesRequestListWorkspacesPaginateTypeDef",
+    "NetworkAccessConfigurationUnionTypeDef",
     "PermissionEntryTypeDef",
     "UpdateInstructionOutputTypeDef",
     "UpdateInstructionTypeDef",
     "SamlConfigurationOutputTypeDef",
     "SamlConfigurationTypeDef",
+    "VpcConfigurationUnionTypeDef",
     "WorkspaceDescriptionTypeDef",
     "ListWorkspacesResponseTypeDef",
     "ListPermissionsResponseTypeDef",
     "UpdateErrorTypeDef",
-    "UpdatePermissionsRequestRequestTypeDef",
+    "UpdateInstructionUnionTypeDef",
     "SamlAuthenticationTypeDef",
+    "SamlConfigurationUnionTypeDef",
     "UpdateWorkspaceAuthenticationRequestRequestTypeDef",
     "AssociateLicenseResponseTypeDef",
     "CreateWorkspaceResponseTypeDef",
     "DeleteWorkspaceResponseTypeDef",
     "DescribeWorkspaceResponseTypeDef",
     "DisassociateLicenseResponseTypeDef",
     "UpdateWorkspaceResponseTypeDef",
     "UpdatePermissionsResponseTypeDef",
+    "UpdatePermissionsRequestRequestTypeDef",
     "AuthenticationDescriptionTypeDef",
     "DescribeWorkspaceAuthenticationResponseTypeDef",
     "UpdateWorkspaceAuthenticationResponseTypeDef",
 )
 
 AssertionAttributesTypeDef = TypedDict(
     "AssertionAttributesTypeDef",
@@ -151,19 +156,21 @@
     "_OptionalAuthenticationSummaryTypeDef",
     {
         "samlConfigurationStatus": SamlConfigurationStatusType,
     },
     total=False,
 )
 
+
 class AuthenticationSummaryTypeDef(
     _RequiredAuthenticationSummaryTypeDef, _OptionalAuthenticationSummaryTypeDef
 ):
     pass
 
+
 CreateWorkspaceApiKeyRequestRequestTypeDef = TypedDict(
     "CreateWorkspaceApiKeyRequestRequestTypeDef",
     {
         "keyName": str,
         "keyRole": str,
         "secondsToLive": int,
         "workspaceId": str,
@@ -263,19 +270,21 @@
         "nextToken": str,
         "userId": str,
         "userType": UserTypeType,
     },
     total=False,
 )
 
+
 class ListPermissionsRequestRequestTypeDef(
     _RequiredListPermissionsRequestRequestTypeDef, _OptionalListPermissionsRequestRequestTypeDef
 ):
     pass
 
+
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
@@ -359,20 +368,22 @@
     "_OptionalUpdateWorkspaceConfigurationRequestRequestTypeDef",
     {
         "grafanaVersion": str,
     },
     total=False,
 )
 
+
 class UpdateWorkspaceConfigurationRequestRequestTypeDef(
     _RequiredUpdateWorkspaceConfigurationRequestRequestTypeDef,
     _OptionalUpdateWorkspaceConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 VpcConfigurationOutputTypeDef = TypedDict(
     "VpcConfigurationOutputTypeDef",
     {
         "securityGroupIds": List[str],
         "subnetIds": List[str],
     },
 )
@@ -441,17 +452,19 @@
         "name": str,
         "notificationDestinations": List[Literal["SNS"]],
         "tags": Dict[str, str],
     },
     total=False,
 )
 
+
 class WorkspaceSummaryTypeDef(_RequiredWorkspaceSummaryTypeDef, _OptionalWorkspaceSummaryTypeDef):
     pass
 
+
 _RequiredCreateWorkspaceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorkspaceRequestRequestTypeDef",
     {
         "accountAccessType": AccountAccessTypeType,
         "authenticationProviders": Sequence[AuthenticationProviderTypesType],
         "permissionType": PermissionTypeType,
     },
@@ -473,19 +486,21 @@
         "workspaceNotificationDestinations": Sequence[Literal["SNS"]],
         "workspaceOrganizationalUnits": Sequence[str],
         "workspaceRoleArn": str,
     },
     total=False,
 )
 
+
 class CreateWorkspaceRequestRequestTypeDef(
     _RequiredCreateWorkspaceRequestRequestTypeDef, _OptionalCreateWorkspaceRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateWorkspaceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateWorkspaceRequestRequestTypeDef",
     {
         "workspaceId": str,
     },
 )
 _OptionalUpdateWorkspaceRequestRequestTypeDef = TypedDict(
@@ -505,19 +520,21 @@
         "workspaceNotificationDestinations": Sequence[Literal["SNS"]],
         "workspaceOrganizationalUnits": Sequence[str],
         "workspaceRoleArn": str,
     },
     total=False,
 )
 
+
 class UpdateWorkspaceRequestRequestTypeDef(
     _RequiredUpdateWorkspaceRequestRequestTypeDef, _OptionalUpdateWorkspaceRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredListPermissionsRequestListPermissionsPaginateTypeDef = TypedDict(
     "_RequiredListPermissionsRequestListPermissionsPaginateTypeDef",
     {
         "workspaceId": str,
     },
 )
 _OptionalListPermissionsRequestListPermissionsPaginateTypeDef = TypedDict(
@@ -527,20 +544,22 @@
         "userId": str,
         "userType": UserTypeType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListPermissionsRequestListPermissionsPaginateTypeDef(
     _RequiredListPermissionsRequestListPermissionsPaginateTypeDef,
     _OptionalListPermissionsRequestListPermissionsPaginateTypeDef,
 ):
     pass
 
+
 ListVersionsRequestListVersionsPaginateTypeDef = TypedDict(
     "ListVersionsRequestListVersionsPaginateTypeDef",
     {
         "workspaceId": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -550,14 +569,17 @@
     "ListWorkspacesRequestListWorkspacesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+NetworkAccessConfigurationUnionTypeDef = Union[
+    NetworkAccessConfigurationTypeDef, NetworkAccessConfigurationOutputTypeDef
+]
 PermissionEntryTypeDef = TypedDict(
     "PermissionEntryTypeDef",
     {
         "role": RoleType,
         "user": UserTypeDef,
     },
 )
@@ -593,19 +615,21 @@
         "assertionAttributes": AssertionAttributesTypeDef,
         "loginValidityDuration": int,
         "roleValues": RoleValuesOutputTypeDef,
     },
     total=False,
 )
 
+
 class SamlConfigurationOutputTypeDef(
     _RequiredSamlConfigurationOutputTypeDef, _OptionalSamlConfigurationOutputTypeDef
 ):
     pass
 
+
 _RequiredSamlConfigurationTypeDef = TypedDict(
     "_RequiredSamlConfigurationTypeDef",
     {
         "idpMetadata": IdpMetadataTypeDef,
     },
 )
 _OptionalSamlConfigurationTypeDef = TypedDict(
@@ -615,19 +639,22 @@
         "assertionAttributes": AssertionAttributesTypeDef,
         "loginValidityDuration": int,
         "roleValues": RoleValuesTypeDef,
     },
     total=False,
 )
 
+
 class SamlConfigurationTypeDef(
     _RequiredSamlConfigurationTypeDef, _OptionalSamlConfigurationTypeDef
 ):
     pass
 
+
+VpcConfigurationUnionTypeDef = Union[VpcConfigurationTypeDef, VpcConfigurationOutputTypeDef]
 _RequiredWorkspaceDescriptionTypeDef = TypedDict(
     "_RequiredWorkspaceDescriptionTypeDef",
     {
         "authentication": AuthenticationSummaryTypeDef,
         "created": datetime,
         "dataSources": List[DataSourceTypeType],
         "endpoint": str,
@@ -656,19 +683,21 @@
         "tags": Dict[str, str],
         "vpcConfiguration": VpcConfigurationOutputTypeDef,
         "workspaceRoleArn": str,
     },
     total=False,
 )
 
+
 class WorkspaceDescriptionTypeDef(
     _RequiredWorkspaceDescriptionTypeDef, _OptionalWorkspaceDescriptionTypeDef
 ):
     pass
 
+
 ListWorkspacesResponseTypeDef = TypedDict(
     "ListWorkspacesResponseTypeDef",
     {
         "nextToken": str,
         "workspaces": List[WorkspaceSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -688,43 +717,37 @@
     {
         "causedBy": UpdateInstructionOutputTypeDef,
         "code": int,
         "message": str,
     },
 )
 
-UpdatePermissionsRequestRequestTypeDef = TypedDict(
-    "UpdatePermissionsRequestRequestTypeDef",
-    {
-        "updateInstructionBatch": Sequence[
-            Union[UpdateInstructionTypeDef, UpdateInstructionOutputTypeDef]
-        ],
-        "workspaceId": str,
-    },
-)
-
+UpdateInstructionUnionTypeDef = Union[UpdateInstructionTypeDef, UpdateInstructionOutputTypeDef]
 _RequiredSamlAuthenticationTypeDef = TypedDict(
     "_RequiredSamlAuthenticationTypeDef",
     {
         "status": SamlConfigurationStatusType,
     },
 )
 _OptionalSamlAuthenticationTypeDef = TypedDict(
     "_OptionalSamlAuthenticationTypeDef",
     {
         "configuration": SamlConfigurationOutputTypeDef,
     },
     total=False,
 )
 
+
 class SamlAuthenticationTypeDef(
     _RequiredSamlAuthenticationTypeDef, _OptionalSamlAuthenticationTypeDef
 ):
     pass
 
+
+SamlConfigurationUnionTypeDef = Union[SamlConfigurationTypeDef, SamlConfigurationOutputTypeDef]
 _RequiredUpdateWorkspaceAuthenticationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateWorkspaceAuthenticationRequestRequestTypeDef",
     {
         "authenticationProviders": Sequence[AuthenticationProviderTypesType],
         "workspaceId": str,
     },
 )
@@ -732,20 +755,22 @@
     "_OptionalUpdateWorkspaceAuthenticationRequestRequestTypeDef",
     {
         "samlConfiguration": SamlConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class UpdateWorkspaceAuthenticationRequestRequestTypeDef(
     _RequiredUpdateWorkspaceAuthenticationRequestRequestTypeDef,
     _OptionalUpdateWorkspaceAuthenticationRequestRequestTypeDef,
 ):
     pass
 
+
 AssociateLicenseResponseTypeDef = TypedDict(
     "AssociateLicenseResponseTypeDef",
     {
         "workspace": WorkspaceDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -794,14 +819,22 @@
     "UpdatePermissionsResponseTypeDef",
     {
         "errors": List[UpdateErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+UpdatePermissionsRequestRequestTypeDef = TypedDict(
+    "UpdatePermissionsRequestRequestTypeDef",
+    {
+        "updateInstructionBatch": Sequence[UpdateInstructionUnionTypeDef],
+        "workspaceId": str,
+    },
+)
+
 _RequiredAuthenticationDescriptionTypeDef = TypedDict(
     "_RequiredAuthenticationDescriptionTypeDef",
     {
         "providers": List[AuthenticationProviderTypesType],
     },
 )
 _OptionalAuthenticationDescriptionTypeDef = TypedDict(
@@ -809,19 +842,21 @@
     {
         "awsSso": AwsSsoAuthenticationTypeDef,
         "saml": SamlAuthenticationTypeDef,
     },
     total=False,
 )
 
+
 class AuthenticationDescriptionTypeDef(
     _RequiredAuthenticationDescriptionTypeDef, _OptionalAuthenticationDescriptionTypeDef
 ):
     pass
 
+
 DescribeWorkspaceAuthenticationResponseTypeDef = TypedDict(
     "DescribeWorkspaceAuthenticationResponseTypeDef",
     {
         "authentication": AuthenticationDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-grafana-1.28.15.post1/mypy_boto3_grafana.egg-info/PKG-INFO` & `mypy-boto3-grafana-1.28.16/mypy_boto3_grafana.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-grafana
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.ManagedGrafana 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.ManagedGrafana 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 grafana type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 grafana type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-grafana.svg?color=blue)](https://pypi.org/project/mypy-boto3-grafana)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-grafana)](https://pepy.tech/project/mypy-boto3-grafana)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ManagedGrafana 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana)
+[boto3.ManagedGrafana 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana)
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
 [mypy-boto3-grafana docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/).
 
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
@@ -328,20 +328,20 @@
 )
 
 
 def check_value(value: AccountAccessTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_grafana.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_grafana.type_defs import (
     AssertionAttributesTypeDef,
     AssociateLicenseRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     AwsSsoAuthenticationTypeDef,
@@ -376,40 +376,44 @@
     ListVersionsResponseTypeDef,
     WorkspaceSummaryTypeDef,
     CreateWorkspaceRequestRequestTypeDef,
     UpdateWorkspaceRequestRequestTypeDef,
     ListPermissionsRequestListPermissionsPaginateTypeDef,
     ListVersionsRequestListVersionsPaginateTypeDef,
     ListWorkspacesRequestListWorkspacesPaginateTypeDef,
+    NetworkAccessConfigurationUnionTypeDef,
     PermissionEntryTypeDef,
     UpdateInstructionOutputTypeDef,
     UpdateInstructionTypeDef,
     SamlConfigurationOutputTypeDef,
     SamlConfigurationTypeDef,
+    VpcConfigurationUnionTypeDef,
     WorkspaceDescriptionTypeDef,
     ListWorkspacesResponseTypeDef,
     ListPermissionsResponseTypeDef,
     UpdateErrorTypeDef,
-    UpdatePermissionsRequestRequestTypeDef,
+    UpdateInstructionUnionTypeDef,
     SamlAuthenticationTypeDef,
+    SamlConfigurationUnionTypeDef,
     UpdateWorkspaceAuthenticationRequestRequestTypeDef,
     AssociateLicenseResponseTypeDef,
     CreateWorkspaceResponseTypeDef,
     DeleteWorkspaceResponseTypeDef,
     DescribeWorkspaceResponseTypeDef,
     DisassociateLicenseResponseTypeDef,
     UpdateWorkspaceResponseTypeDef,
     UpdatePermissionsResponseTypeDef,
+    UpdatePermissionsRequestRequestTypeDef,
     AuthenticationDescriptionTypeDef,
     DescribeWorkspaceAuthenticationResponseTypeDef,
     UpdateWorkspaceAuthenticationResponseTypeDef,
 )
 
 
-def get_structure() -> AssertionAttributesTypeDef:
+def get_value() -> AssertionAttributesTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-grafana-1.28.15.post1/mypy_boto3_grafana.egg-info/SOURCES.txt` & `mypy-boto3-grafana-1.28.16/mypy_boto3_grafana.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-grafana-1.28.15.post1/setup.py` & `mypy-boto3-grafana-1.28.16/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-grafana",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_grafana"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ManagedGrafana 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.ManagedGrafana 1.28.16 service generated with"
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
-    keywords="boto3 grafana type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 grafana type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_grafana": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

