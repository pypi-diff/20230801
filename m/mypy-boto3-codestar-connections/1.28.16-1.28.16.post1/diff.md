# Comparing `tmp/mypy-boto3-codestar-connections-1.28.16.tar.gz` & `tmp/mypy-boto3-codestar-connections-1.28.16.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-codestar-connections-1.28.16.tar", last modified: Mon Jul 31 19:32:46 2023, max compression
+gzip compressed data, was "mypy-boto3-codestar-connections-1.28.16.post1.tar", last modified: Tue Aug  1 11:36:28 2023, max compression
```

## Comparing `mypy-boto3-codestar-connections-1.28.16.tar` & `mypy-boto3-codestar-connections-1.28.16.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:32:46.250207 mypy-boto3-codestar-connections-1.28.16/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-31 19:32:10.000000 mypy-boto3-codestar-connections-1.28.16/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13300 2023-07-31 19:32:46.250207 mypy-boto3-codestar-connections-1.28.16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11762 2023-07-31 19:32:10.000000 mypy-boto3-codestar-connections-1.28.16/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:32:46.242207 mypy-boto3-codestar-connections-1.28.16/mypy_boto3_codestar_connections/
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-31 19:32:10.000000 mypy-boto3-codestar-connections-1.28.16/mypy_boto3_codestar_connections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-31 19:32:10.000000 mypy-boto3-codestar-connections-1.28.16/mypy_boto3_codestar_connections/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-31 19:32:10.000000 mypy-boto3-codestar-connections-1.28.16/mypy_boto3_codestar_connections/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10563 2023-07-31 19:32:11.000000 mypy-boto3-codestar-connections-1.28.16/mypy_boto3_codestar_connections/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10545 2023-07-31 19:32:10.000000 mypy-boto3-codestar-connections-1.28.16/mypy_boto3_codestar_connections/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8239 2023-07-31 19:32:11.000000 mypy-boto3-codestar-connections-1.28.16/mypy_boto3_codestar_connections/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8237 2023-07-31 19:32:11.000000 mypy-boto3-codestar-connections-1.28.16/mypy_boto3_codestar_connections/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:32:10.000000 mypy-boto3-codestar-connections-1.28.16/mypy_boto3_codestar_connections/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     7860 2023-07-31 19:32:11.000000 mypy-boto3-codestar-connections-1.28.16/mypy_boto3_codestar_connections/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7849 2023-07-31 19:32:11.000000 mypy-boto3-codestar-connections-1.28.16/mypy_boto3_codestar_connections/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-31 19:32:10.000000 mypy-boto3-codestar-connections-1.28.16/mypy_boto3_codestar_connections/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:32:46.246207 mypy-boto3-codestar-connections-1.28.16/mypy_boto3_codestar_connections.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13300 2023-07-31 19:32:46.000000 mypy-boto3-codestar-connections-1.28.16/mypy_boto3_codestar_connections.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-31 19:32:46.000000 mypy-boto3-codestar-connections-1.28.16/mypy_boto3_codestar_connections.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 19:32:46.000000 mypy-boto3-codestar-connections-1.28.16/mypy_boto3_codestar_connections.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 19:32:46.000000 mypy-boto3-codestar-connections-1.28.16/mypy_boto3_codestar_connections.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-31 19:32:46.000000 mypy-boto3-codestar-connections-1.28.16/mypy_boto3_codestar_connections.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-31 19:32:46.000000 mypy-boto3-codestar-connections-1.28.16/mypy_boto3_codestar_connections.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 19:32:46.250207 mypy-boto3-codestar-connections-1.28.16/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-07-31 19:32:10.000000 mypy-boto3-codestar-connections-1.28.16/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:28.844923 mypy-boto3-codestar-connections-1.28.16.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:13:27.000000 mypy-boto3-codestar-connections-1.28.16.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13336 2023-08-01 11:36:28.832923 mypy-boto3-codestar-connections-1.28.16.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11795 2023-08-01 11:13:27.000000 mypy-boto3-codestar-connections-1.28.16.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:28.832923 mypy-boto3-codestar-connections-1.28.16.post1/mypy_boto3_codestar_connections/
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-08-01 11:13:27.000000 mypy-boto3-codestar-connections-1.28.16.post1/mypy_boto3_codestar_connections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-08-01 11:13:27.000000 mypy-boto3-codestar-connections-1.28.16.post1/mypy_boto3_codestar_connections/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-08-01 11:13:27.000000 mypy-boto3-codestar-connections-1.28.16.post1/mypy_boto3_codestar_connections/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10460 2023-08-01 11:13:28.000000 mypy-boto3-codestar-connections-1.28.16.post1/mypy_boto3_codestar_connections/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10442 2023-08-01 11:13:28.000000 mypy-boto3-codestar-connections-1.28.16.post1/mypy_boto3_codestar_connections/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8239 2023-08-01 11:13:28.000000 mypy-boto3-codestar-connections-1.28.16.post1/mypy_boto3_codestar_connections/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8237 2023-08-01 11:13:28.000000 mypy-boto3-codestar-connections-1.28.16.post1/mypy_boto3_codestar_connections/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:13:27.000000 mypy-boto3-codestar-connections-1.28.16.post1/mypy_boto3_codestar_connections/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     7994 2023-08-01 11:13:28.000000 mypy-boto3-codestar-connections-1.28.16.post1/mypy_boto3_codestar_connections/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7983 2023-08-01 11:13:28.000000 mypy-boto3-codestar-connections-1.28.16.post1/mypy_boto3_codestar_connections/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-01 11:13:27.000000 mypy-boto3-codestar-connections-1.28.16.post1/mypy_boto3_codestar_connections/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:28.832923 mypy-boto3-codestar-connections-1.28.16.post1/mypy_boto3_codestar_connections.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13336 2023-08-01 11:36:28.000000 mypy-boto3-codestar-connections-1.28.16.post1/mypy_boto3_codestar_connections.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-08-01 11:36:28.000000 mypy-boto3-codestar-connections-1.28.16.post1/mypy_boto3_codestar_connections.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:28.000000 mypy-boto3-codestar-connections-1.28.16.post1/mypy_boto3_codestar_connections.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:28.000000 mypy-boto3-codestar-connections-1.28.16.post1/mypy_boto3_codestar_connections.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:28.000000 mypy-boto3-codestar-connections-1.28.16.post1/mypy_boto3_codestar_connections.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-01 11:36:28.000000 mypy-boto3-codestar-connections-1.28.16.post1/mypy_boto3_codestar_connections.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:28.844923 mypy-boto3-codestar-connections-1.28.16.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-08-01 11:13:27.000000 mypy-boto3-codestar-connections-1.28.16.post1/setup.py
```

### Comparing `mypy-boto3-codestar-connections-1.28.16/LICENSE` & `mypy-boto3-codestar-connections-1.28.16.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codestar-connections-1.28.16/PKG-INFO` & `mypy-boto3-codestar-connections-1.28.16.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codestar-connections
-Version: 1.28.16
-Summary: Type annotations for boto3.CodeStarconnections 1.28.16 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16.post1
+Summary: Type annotations for boto3.CodeStarconnections 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_connections/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 codestar-connections type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 codestar-connections type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -47,15 +47,15 @@
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
 [mypy-boto3-codestar-connections docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_connections/).
 
 See how it helps to find and fix potential bugs:
 
@@ -73,15 +73,15 @@
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
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
@@ -290,20 +290,20 @@
 )
 
 
 def check_value(value: ConnectionStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_codestar_connections.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_codestar_connections.type_defs import (
     ConnectionTypeDef,
     TagTypeDef,
     ResponseMetadataTypeDef,
     VpcConfigurationTypeDef,
@@ -323,19 +323,20 @@
     GetConnectionOutputTypeDef,
     ListConnectionsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     CreateHostInputRequestTypeDef,
     UpdateHostInputRequestTypeDef,
     GetHostOutputTypeDef,
     HostTypeDef,
+    VpcConfigurationUnionTypeDef,
     ListHostsOutputTypeDef,
 )
 
 
-def get_structure() -> ConnectionTypeDef:
+def get_value() -> ConnectionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-codestar-connections-1.28.16/README.md` & `mypy-boto3-codestar-connections-1.28.16.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
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
 [mypy-boto3-codestar-connections docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_connections/).
 
 See how it helps to find and fix potential bugs:
 
@@ -41,15 +41,15 @@
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
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
@@ -258,20 +258,20 @@
 )
 
 
 def check_value(value: ConnectionStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_codestar_connections.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_codestar_connections.type_defs import (
     ConnectionTypeDef,
     TagTypeDef,
     ResponseMetadataTypeDef,
     VpcConfigurationTypeDef,
@@ -291,19 +291,20 @@
     GetConnectionOutputTypeDef,
     ListConnectionsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     CreateHostInputRequestTypeDef,
     UpdateHostInputRequestTypeDef,
     GetHostOutputTypeDef,
     HostTypeDef,
+    VpcConfigurationUnionTypeDef,
     ListHostsOutputTypeDef,
 )
 
 
-def get_structure() -> ConnectionTypeDef:
+def get_value() -> ConnectionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-codestar-connections-1.28.16/mypy_boto3_codestar_connections/__main__.py` & `mypy-boto3-codestar-connections-1.28.16.post1/mypy_boto3_codestar_connections/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CodeStarconnections 1.28.16\nVersion:         1.28.16\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.CodeStarconnections 1.28.16\nVersion:        "
+        " 1.28.16.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_connections//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.16")
+    print("1.28.16.post1")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-codestar-connections-1.28.16/mypy_boto3_codestar_connections/client.py` & `mypy-boto3-codestar-connections-1.28.16.post1/mypy_boto3_codestar_connections/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,30 +9,29 @@
     from boto3.session import Session
     from mypy_boto3_codestar_connections.client import CodeStarconnectionsClient
 
     session = Session()
     client: CodeStarconnectionsClient = session.client("codestar-connections")
     ```
 """
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ProviderTypeType
 from .type_defs import (
     CreateConnectionOutputTypeDef,
     CreateHostOutputTypeDef,
     GetConnectionOutputTypeDef,
     GetHostOutputTypeDef,
     ListConnectionsOutputTypeDef,
     ListHostsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     TagTypeDef,
-    VpcConfigurationOutputTypeDef,
-    VpcConfigurationTypeDef,
+    VpcConfigurationUnionTypeDef,
 )
 
 __all__ = ("CodeStarconnectionsClient",)
 
 
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
@@ -102,15 +101,15 @@
 
     def create_host(
         self,
         *,
         Name: str,
         ProviderType: ProviderTypeType,
         ProviderEndpoint: str,
-        VpcConfiguration: Union[VpcConfigurationTypeDef, VpcConfigurationOutputTypeDef] = ...,
+        VpcConfiguration: VpcConfigurationUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateHostOutputTypeDef:
         """
         Creates a resource that represents the infrastructure where a third-party
         provider is installed.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client.create_host)
@@ -212,15 +211,15 @@
         """
 
     def update_host(
         self,
         *,
         HostArn: str,
         ProviderEndpoint: str = ...,
-        VpcConfiguration: Union[VpcConfigurationTypeDef, VpcConfigurationOutputTypeDef] = ...
+        VpcConfiguration: VpcConfigurationUnionTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Updates a specified host with the provided configurations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client.update_host)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_connections/client/#update_host)
         """
```

### Comparing `mypy-boto3-codestar-connections-1.28.16/mypy_boto3_codestar_connections/client.pyi` & `mypy-boto3-codestar-connections-1.28.16.post1/mypy_boto3_codestar_connections/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -9,30 +9,29 @@
     from boto3.session import Session
     from mypy_boto3_codestar_connections.client import CodeStarconnectionsClient
 
     session = Session()
     client: CodeStarconnectionsClient = session.client("codestar-connections")
     ```
 """
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ProviderTypeType
 from .type_defs import (
     CreateConnectionOutputTypeDef,
     CreateHostOutputTypeDef,
     GetConnectionOutputTypeDef,
     GetHostOutputTypeDef,
     ListConnectionsOutputTypeDef,
     ListHostsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     TagTypeDef,
-    VpcConfigurationOutputTypeDef,
-    VpcConfigurationTypeDef,
+    VpcConfigurationUnionTypeDef,
 )
 
 __all__ = ("CodeStarconnectionsClient",)
 
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
@@ -95,15 +94,15 @@
         """
     def create_host(
         self,
         *,
         Name: str,
         ProviderType: ProviderTypeType,
         ProviderEndpoint: str,
-        VpcConfiguration: Union[VpcConfigurationTypeDef, VpcConfigurationOutputTypeDef] = ...,
+        VpcConfiguration: VpcConfigurationUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateHostOutputTypeDef:
         """
         Creates a resource that represents the infrastructure where a third-party
         provider is installed.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client.create_host)
@@ -194,15 +193,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_connections/client/#untag_resource)
         """
     def update_host(
         self,
         *,
         HostArn: str,
         ProviderEndpoint: str = ...,
-        VpcConfiguration: Union[VpcConfigurationTypeDef, VpcConfigurationOutputTypeDef] = ...
+        VpcConfiguration: VpcConfigurationUnionTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Updates a specified host with the provided configurations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client.update_host)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_connections/client/#update_host)
         """
```

### Comparing `mypy-boto3-codestar-connections-1.28.16/mypy_boto3_codestar_connections/literals.py` & `mypy-boto3-codestar-connections-1.28.16.post1/mypy_boto3_codestar_connections/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codestar-connections-1.28.16/mypy_boto3_codestar_connections/literals.pyi` & `mypy-boto3-codestar-connections-1.28.16.post1/mypy_boto3_codestar_connections/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codestar-connections-1.28.16/mypy_boto3_codestar_connections/type_defs.py` & `mypy-boto3-codestar-connections-1.28.16.post1/mypy_boto3_codestar_connections/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_connections/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_codestar_connections.type_defs import ConnectionTypeDef
 
-    data: ConnectionTypeDef = {...}
+    data: ConnectionTypeDef = ...
     ```
 """
 import sys
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import ConnectionStatusType, ProviderTypeType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
@@ -43,14 +43,15 @@
     "GetConnectionOutputTypeDef",
     "ListConnectionsOutputTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "CreateHostInputRequestTypeDef",
     "UpdateHostInputRequestTypeDef",
     "GetHostOutputTypeDef",
     "HostTypeDef",
+    "VpcConfigurationUnionTypeDef",
     "ListHostsOutputTypeDef",
 )
 
 ConnectionTypeDef = TypedDict(
     "ConnectionTypeDef",
     {
         "ConnectionName": str,
@@ -331,14 +332,15 @@
         "VpcConfiguration": VpcConfigurationOutputTypeDef,
         "Status": str,
         "StatusMessage": str,
     },
     total=False,
 )
 
+VpcConfigurationUnionTypeDef = Union[VpcConfigurationTypeDef, VpcConfigurationOutputTypeDef]
 ListHostsOutputTypeDef = TypedDict(
     "ListHostsOutputTypeDef",
     {
         "Hosts": List[HostTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-codestar-connections-1.28.16/mypy_boto3_codestar_connections/type_defs.pyi` & `mypy-boto3-codestar-connections-1.28.16.post1/mypy_boto3_codestar_connections/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_connections/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_codestar_connections.type_defs import ConnectionTypeDef
 
-    data: ConnectionTypeDef = {...}
+    data: ConnectionTypeDef = ...
     ```
 """
 import sys
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import ConnectionStatusType, ProviderTypeType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
@@ -42,14 +42,15 @@
     "GetConnectionOutputTypeDef",
     "ListConnectionsOutputTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "CreateHostInputRequestTypeDef",
     "UpdateHostInputRequestTypeDef",
     "GetHostOutputTypeDef",
     "HostTypeDef",
+    "VpcConfigurationUnionTypeDef",
     "ListHostsOutputTypeDef",
 )
 
 ConnectionTypeDef = TypedDict(
     "ConnectionTypeDef",
     {
         "ConnectionName": str,
@@ -320,14 +321,15 @@
         "VpcConfiguration": VpcConfigurationOutputTypeDef,
         "Status": str,
         "StatusMessage": str,
     },
     total=False,
 )
 
+VpcConfigurationUnionTypeDef = Union[VpcConfigurationTypeDef, VpcConfigurationOutputTypeDef]
 ListHostsOutputTypeDef = TypedDict(
     "ListHostsOutputTypeDef",
     {
         "Hosts": List[HostTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-codestar-connections-1.28.16/mypy_boto3_codestar_connections.egg-info/PKG-INFO` & `mypy-boto3-codestar-connections-1.28.16.post1/mypy_boto3_codestar_connections.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codestar-connections
-Version: 1.28.16
-Summary: Type annotations for boto3.CodeStarconnections 1.28.16 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16.post1
+Summary: Type annotations for boto3.CodeStarconnections 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_connections/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 codestar-connections type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 codestar-connections type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -47,15 +47,15 @@
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
 [mypy-boto3-codestar-connections docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_connections/).
 
 See how it helps to find and fix potential bugs:
 
@@ -73,15 +73,15 @@
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
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
@@ -290,20 +290,20 @@
 )
 
 
 def check_value(value: ConnectionStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_codestar_connections.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_codestar_connections.type_defs import (
     ConnectionTypeDef,
     TagTypeDef,
     ResponseMetadataTypeDef,
     VpcConfigurationTypeDef,
@@ -323,19 +323,20 @@
     GetConnectionOutputTypeDef,
     ListConnectionsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     CreateHostInputRequestTypeDef,
     UpdateHostInputRequestTypeDef,
     GetHostOutputTypeDef,
     HostTypeDef,
+    VpcConfigurationUnionTypeDef,
     ListHostsOutputTypeDef,
 )
 
 
-def get_structure() -> ConnectionTypeDef:
+def get_value() -> ConnectionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-codestar-connections-1.28.16/mypy_boto3_codestar_connections.egg-info/SOURCES.txt` & `mypy-boto3-codestar-connections-1.28.16.post1/mypy_boto3_codestar_connections.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codestar-connections-1.28.16/setup.py` & `mypy-boto3-codestar-connections-1.28.16.post1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-codestar-connections",
-    version="1.28.16",
+    version="1.28.16.post1",
     packages=["mypy_boto3_codestar_connections"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.CodeStarconnections 1.28.16 service generated with"
-        " mypy-boto3-builder 7.16.2"
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
-    keywords="boto3 codestar-connections type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 codestar-connections type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_codestar_connections": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_connections/"
```

