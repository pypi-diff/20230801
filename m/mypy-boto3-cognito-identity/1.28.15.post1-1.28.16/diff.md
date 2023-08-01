# Comparing `tmp/mypy-boto3-cognito-identity-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-cognito-identity-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cognito-identity-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:48 2023, max compression
+gzip compressed data, was "mypy-boto3-cognito-identity-1.28.16.tar", last modified: Tue Aug  1 11:36:29 2023, max compression
```

## Comparing `mypy-boto3-cognito-identity-1.28.15.post1.tar` & `mypy-boto3-cognito-identity-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:48.669077 mypy-boto3-cognito-identity-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:40:58.000000 mypy-boto3-cognito-identity-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15186 2023-07-29 10:02:48.661077 mypy-boto3-cognito-identity-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13658 2023-07-29 09:40:58.000000 mypy-boto3-cognito-identity-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:48.661077 mypy-boto3-cognito-identity-1.28.15.post1/mypy_boto3_cognito_identity/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-29 09:40:58.000000 mypy-boto3-cognito-identity-1.28.15.post1/mypy_boto3_cognito_identity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-29 09:40:58.000000 mypy-boto3-cognito-identity-1.28.15.post1/mypy_boto3_cognito_identity/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-29 09:40:58.000000 mypy-boto3-cognito-identity-1.28.15.post1/mypy_boto3_cognito_identity/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19575 2023-07-29 09:40:58.000000 mypy-boto3-cognito-identity-1.28.15.post1/mypy_boto3_cognito_identity/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    19544 2023-07-29 09:40:58.000000 mypy-boto3-cognito-identity-1.28.15.post1/mypy_boto3_cognito_identity/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8615 2023-07-29 09:40:59.000000 mypy-boto3-cognito-identity-1.28.15.post1/mypy_boto3_cognito_identity/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8613 2023-07-29 09:40:58.000000 mypy-boto3-cognito-identity-1.28.15.post1/mypy_boto3_cognito_identity/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-29 09:40:58.000000 mypy-boto3-cognito-identity-1.28.15.post1/mypy_boto3_cognito_identity/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-07-29 09:40:58.000000 mypy-boto3-cognito-identity-1.28.15.post1/mypy_boto3_cognito_identity/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:40:58.000000 mypy-boto3-cognito-identity-1.28.15.post1/mypy_boto3_cognito_identity/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    19033 2023-07-29 09:40:59.000000 mypy-boto3-cognito-identity-1.28.15.post1/mypy_boto3_cognito_identity/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19007 2023-07-29 09:40:59.000000 mypy-boto3-cognito-identity-1.28.15.post1/mypy_boto3_cognito_identity/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:40:58.000000 mypy-boto3-cognito-identity-1.28.15.post1/mypy_boto3_cognito_identity/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:48.661077 mypy-boto3-cognito-identity-1.28.15.post1/mypy_boto3_cognito_identity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15186 2023-07-29 10:02:48.000000 mypy-boto3-cognito-identity-1.28.15.post1/mypy_boto3_cognito_identity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-29 10:02:48.000000 mypy-boto3-cognito-identity-1.28.15.post1/mypy_boto3_cognito_identity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:48.000000 mypy-boto3-cognito-identity-1.28.15.post1/mypy_boto3_cognito_identity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:48.000000 mypy-boto3-cognito-identity-1.28.15.post1/mypy_boto3_cognito_identity.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:48.000000 mypy-boto3-cognito-identity-1.28.15.post1/mypy_boto3_cognito_identity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-29 10:02:48.000000 mypy-boto3-cognito-identity-1.28.15.post1/mypy_boto3_cognito_identity.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:48.669077 mypy-boto3-cognito-identity-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-29 09:40:58.000000 mypy-boto3-cognito-identity-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:29.096923 mypy-boto3-cognito-identity-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:13:30.000000 mypy-boto3-cognito-identity-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15205 2023-08-01 11:36:29.096923 mypy-boto3-cognito-identity-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13686 2023-08-01 11:13:30.000000 mypy-boto3-cognito-identity-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:29.096923 mypy-boto3-cognito-identity-1.28.16/mypy_boto3_cognito_identity/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-08-01 11:13:30.000000 mypy-boto3-cognito-identity-1.28.16/mypy_boto3_cognito_identity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-08-01 11:13:30.000000 mypy-boto3-cognito-identity-1.28.16/mypy_boto3_cognito_identity/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-08-01 11:13:30.000000 mypy-boto3-cognito-identity-1.28.16/mypy_boto3_cognito_identity/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19515 2023-08-01 11:13:30.000000 mypy-boto3-cognito-identity-1.28.16/mypy_boto3_cognito_identity/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19484 2023-08-01 11:13:30.000000 mypy-boto3-cognito-identity-1.28.16/mypy_boto3_cognito_identity/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8615 2023-08-01 11:13:30.000000 mypy-boto3-cognito-identity-1.28.16/mypy_boto3_cognito_identity/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8613 2023-08-01 11:13:30.000000 mypy-boto3-cognito-identity-1.28.16/mypy_boto3_cognito_identity/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-08-01 11:13:30.000000 mypy-boto3-cognito-identity-1.28.16/mypy_boto3_cognito_identity/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-08-01 11:13:30.000000 mypy-boto3-cognito-identity-1.28.16/mypy_boto3_cognito_identity/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:13:30.000000 mypy-boto3-cognito-identity-1.28.16/mypy_boto3_cognito_identity/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    19112 2023-08-01 11:13:31.000000 mypy-boto3-cognito-identity-1.28.16/mypy_boto3_cognito_identity/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19086 2023-08-01 11:13:30.000000 mypy-boto3-cognito-identity-1.28.16/mypy_boto3_cognito_identity/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:13:30.000000 mypy-boto3-cognito-identity-1.28.16/mypy_boto3_cognito_identity/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:29.096923 mypy-boto3-cognito-identity-1.28.16/mypy_boto3_cognito_identity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15205 2023-08-01 11:36:28.000000 mypy-boto3-cognito-identity-1.28.16/mypy_boto3_cognito_identity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-08-01 11:36:28.000000 mypy-boto3-cognito-identity-1.28.16/mypy_boto3_cognito_identity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:28.000000 mypy-boto3-cognito-identity-1.28.16/mypy_boto3_cognito_identity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:28.000000 mypy-boto3-cognito-identity-1.28.16/mypy_boto3_cognito_identity.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:28.000000 mypy-boto3-cognito-identity-1.28.16/mypy_boto3_cognito_identity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-01 11:36:28.000000 mypy-boto3-cognito-identity-1.28.16/mypy_boto3_cognito_identity.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:29.096923 mypy-boto3-cognito-identity-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-08-01 11:13:30.000000 mypy-boto3-cognito-identity-1.28.16/setup.py
```

### Comparing `mypy-boto3-cognito-identity-1.28.15.post1/LICENSE` & `mypy-boto3-cognito-identity-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-identity-1.28.15.post1/PKG-INFO` & `mypy-boto3-cognito-identity-1.28.16/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cognito-identity
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.CognitoIdentity 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.CognitoIdentity 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_identity/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 cognito-identity type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 cognito-identity type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cognito-identity.svg?color=blue)](https://pypi.org/project/mypy-boto3-cognito-identity)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_identity/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cognito-identity)](https://pepy.tech/project/mypy-boto3-cognito-identity)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CognitoIdentity 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity)
+[boto3.CognitoIdentity 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity)
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
 [mypy-boto3-cognito-identity docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_identity/).
 
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
@@ -317,20 +317,20 @@
 )
 
 
 def check_value(value: AmbiguousRoleResolutionTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_cognito_identity.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_cognito_identity.type_defs import (
     CognitoIdentityProviderTypeDef,
     CredentialsTypeDef,
     DeleteIdentitiesInputRequestTypeDef,
     ResponseMetadataTypeDef,
@@ -377,19 +377,20 @@
     ListIdentityPoolsResponseTypeDef,
     ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef,
     RulesConfigurationTypeOutputTypeDef,
     RulesConfigurationTypeTypeDef,
     RoleMappingOutputTypeDef,
     RoleMappingTypeDef,
     GetIdentityPoolRolesResponseTypeDef,
+    RoleMappingUnionTypeDef,
     SetIdentityPoolRolesInputRequestTypeDef,
 )
 
 
-def get_structure() -> CognitoIdentityProviderTypeDef:
+def get_value() -> CognitoIdentityProviderTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-cognito-identity-1.28.15.post1/README.md` & `mypy-boto3-cognito-identity-1.28.16/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cognito-identity.svg?color=blue)](https://pypi.org/project/mypy-boto3-cognito-identity)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_identity/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cognito-identity)](https://pepy.tech/project/mypy-boto3-cognito-identity)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CognitoIdentity 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity)
+[boto3.CognitoIdentity 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity)
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
 [mypy-boto3-cognito-identity docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_identity/).
 
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
@@ -285,20 +285,20 @@
 )
 
 
 def check_value(value: AmbiguousRoleResolutionTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_cognito_identity.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_cognito_identity.type_defs import (
     CognitoIdentityProviderTypeDef,
     CredentialsTypeDef,
     DeleteIdentitiesInputRequestTypeDef,
     ResponseMetadataTypeDef,
@@ -345,19 +345,20 @@
     ListIdentityPoolsResponseTypeDef,
     ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef,
     RulesConfigurationTypeOutputTypeDef,
     RulesConfigurationTypeTypeDef,
     RoleMappingOutputTypeDef,
     RoleMappingTypeDef,
     GetIdentityPoolRolesResponseTypeDef,
+    RoleMappingUnionTypeDef,
     SetIdentityPoolRolesInputRequestTypeDef,
 )
 
 
-def get_structure() -> CognitoIdentityProviderTypeDef:
+def get_value() -> CognitoIdentityProviderTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-cognito-identity-1.28.15.post1/mypy_boto3_cognito_identity/__init__.py` & `mypy-boto3-cognito-identity-1.28.16/mypy_boto3_cognito_identity/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-identity-1.28.15.post1/mypy_boto3_cognito_identity/__init__.pyi` & `mypy-boto3-cognito-identity-1.28.16/mypy_boto3_cognito_identity/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-identity-1.28.15.post1/mypy_boto3_cognito_identity/__main__.py` & `mypy-boto3-cognito-identity-1.28.16/mypy_boto3_cognito_identity/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CognitoIdentity 1.28.15\nVersion:        "
-        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.CognitoIdentity 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_identity//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity\nOther"
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

### Comparing `mypy-boto3-cognito-identity-1.28.15.post1/mypy_boto3_cognito_identity/client.py` & `mypy-boto3-cognito-identity-1.28.16/mypy_boto3_cognito_identity/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_cognito_identity.client import CognitoIdentityClient
 
     session = Session()
     client: CognitoIdentityClient = session.client("cognito-identity")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .paginator import ListIdentityPoolsPaginator
 from .type_defs import (
     CognitoIdentityProviderTypeDef,
     DeleteIdentitiesResponseTypeDef,
@@ -32,16 +32,15 @@
     IdentityDescriptionResponseTypeDef,
     IdentityPoolTypeDef,
     ListIdentitiesResponseTypeDef,
     ListIdentityPoolsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     LookupDeveloperIdentityResponseTypeDef,
     MergeDeveloperIdentitiesResponseTypeDef,
-    RoleMappingOutputTypeDef,
-    RoleMappingTypeDef,
+    RoleMappingUnionTypeDef,
     SetPrincipalTagAttributeMapResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -312,15 +311,15 @@
         """
 
     def set_identity_pool_roles(
         self,
         *,
         IdentityPoolId: str,
         Roles: Mapping[str, str],
-        RoleMappings: Mapping[str, Union[RoleMappingTypeDef, RoleMappingOutputTypeDef]] = ...
+        RoleMappings: Mapping[str, RoleMappingUnionTypeDef] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Sets the roles for an identity pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client.set_identity_pool_roles)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_identity/client/#set_identity_pool_roles)
         """
```

### Comparing `mypy-boto3-cognito-identity-1.28.15.post1/mypy_boto3_cognito_identity/client.pyi` & `mypy-boto3-cognito-identity-1.28.16/mypy_boto3_cognito_identity/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_cognito_identity.client import CognitoIdentityClient
 
     session = Session()
     client: CognitoIdentityClient = session.client("cognito-identity")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .paginator import ListIdentityPoolsPaginator
 from .type_defs import (
     CognitoIdentityProviderTypeDef,
     DeleteIdentitiesResponseTypeDef,
@@ -32,16 +32,15 @@
     IdentityDescriptionResponseTypeDef,
     IdentityPoolTypeDef,
     ListIdentitiesResponseTypeDef,
     ListIdentityPoolsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     LookupDeveloperIdentityResponseTypeDef,
     MergeDeveloperIdentitiesResponseTypeDef,
-    RoleMappingOutputTypeDef,
-    RoleMappingTypeDef,
+    RoleMappingUnionTypeDef,
     SetPrincipalTagAttributeMapResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -288,15 +287,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_identity/client/#merge_developer_identities)
         """
     def set_identity_pool_roles(
         self,
         *,
         IdentityPoolId: str,
         Roles: Mapping[str, str],
-        RoleMappings: Mapping[str, Union[RoleMappingTypeDef, RoleMappingOutputTypeDef]] = ...
+        RoleMappings: Mapping[str, RoleMappingUnionTypeDef] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Sets the roles for an identity pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client.set_identity_pool_roles)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_identity/client/#set_identity_pool_roles)
         """
```

### Comparing `mypy-boto3-cognito-identity-1.28.15.post1/mypy_boto3_cognito_identity/literals.py` & `mypy-boto3-cognito-identity-1.28.16/mypy_boto3_cognito_identity/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-identity-1.28.15.post1/mypy_boto3_cognito_identity/literals.pyi` & `mypy-boto3-cognito-identity-1.28.16/mypy_boto3_cognito_identity/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-identity-1.28.15.post1/mypy_boto3_cognito_identity/paginator.py` & `mypy-boto3-cognito-identity-1.28.16/mypy_boto3_cognito_identity/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-identity-1.28.15.post1/mypy_boto3_cognito_identity/paginator.pyi` & `mypy-boto3-cognito-identity-1.28.16/mypy_boto3_cognito_identity/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-identity-1.28.15.post1/mypy_boto3_cognito_identity/type_defs.py` & `mypy-boto3-cognito-identity-1.28.16/mypy_boto3_cognito_identity/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_identity/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_cognito_identity.type_defs import CognitoIdentityProviderTypeDef
 
-    data: CognitoIdentityProviderTypeDef = {...}
+    data: CognitoIdentityProviderTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -23,15 +23,14 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "CognitoIdentityProviderTypeDef",
     "CredentialsTypeDef",
     "DeleteIdentitiesInputRequestTypeDef",
     "ResponseMetadataTypeDef",
     "UnprocessedIdentityIdTypeDef",
     "DeleteIdentityPoolInputRequestTypeDef",
@@ -76,14 +75,15 @@
     "ListIdentityPoolsResponseTypeDef",
     "ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef",
     "RulesConfigurationTypeOutputTypeDef",
     "RulesConfigurationTypeTypeDef",
     "RoleMappingOutputTypeDef",
     "RoleMappingTypeDef",
     "GetIdentityPoolRolesResponseTypeDef",
+    "RoleMappingUnionTypeDef",
     "SetIdentityPoolRolesInputRequestTypeDef",
 )
 
 CognitoIdentityProviderTypeDef = TypedDict(
     "CognitoIdentityProviderTypeDef",
     {
         "ProviderName": str,
@@ -163,22 +163,20 @@
     {
         "Logins": Mapping[str, str],
         "CustomRoleArn": str,
     },
     total=False,
 )
 
-
 class GetCredentialsForIdentityInputRequestTypeDef(
     _RequiredGetCredentialsForIdentityInputRequestTypeDef,
     _OptionalGetCredentialsForIdentityInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetIdInputRequestTypeDef = TypedDict(
     "_RequiredGetIdInputRequestTypeDef",
     {
         "IdentityPoolId": str,
     },
 )
 _OptionalGetIdInputRequestTypeDef = TypedDict(
@@ -186,21 +184,19 @@
     {
         "AccountId": str,
         "Logins": Mapping[str, str],
     },
     total=False,
 )
 
-
 class GetIdInputRequestTypeDef(
     _RequiredGetIdInputRequestTypeDef, _OptionalGetIdInputRequestTypeDef
 ):
     pass
 
-
 GetIdentityPoolRolesInputRequestTypeDef = TypedDict(
     "GetIdentityPoolRolesInputRequestTypeDef",
     {
         "IdentityPoolId": str,
     },
 )
 
@@ -217,43 +213,39 @@
         "IdentityId": str,
         "PrincipalTags": Mapping[str, str],
         "TokenDuration": int,
     },
     total=False,
 )
 
-
 class GetOpenIdTokenForDeveloperIdentityInputRequestTypeDef(
     _RequiredGetOpenIdTokenForDeveloperIdentityInputRequestTypeDef,
     _OptionalGetOpenIdTokenForDeveloperIdentityInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetOpenIdTokenInputRequestTypeDef = TypedDict(
     "_RequiredGetOpenIdTokenInputRequestTypeDef",
     {
         "IdentityId": str,
     },
 )
 _OptionalGetOpenIdTokenInputRequestTypeDef = TypedDict(
     "_OptionalGetOpenIdTokenInputRequestTypeDef",
     {
         "Logins": Mapping[str, str],
     },
     total=False,
 )
 
-
 class GetOpenIdTokenInputRequestTypeDef(
     _RequiredGetOpenIdTokenInputRequestTypeDef, _OptionalGetOpenIdTokenInputRequestTypeDef
 ):
     pass
 
-
 GetPrincipalTagAttributeMapInputRequestTypeDef = TypedDict(
     "GetPrincipalTagAttributeMapInputRequestTypeDef",
     {
         "IdentityPoolId": str,
         "IdentityProviderName": str,
     },
 )
@@ -290,21 +282,19 @@
     {
         "NextToken": str,
         "HideDisabled": bool,
     },
     total=False,
 )
 
-
 class ListIdentitiesInputRequestTypeDef(
     _RequiredListIdentitiesInputRequestTypeDef, _OptionalListIdentitiesInputRequestTypeDef
 ):
     pass
 
-
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -321,21 +311,19 @@
     "_OptionalListIdentityPoolsInputRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListIdentityPoolsInputRequestTypeDef(
     _RequiredListIdentityPoolsInputRequestTypeDef, _OptionalListIdentityPoolsInputRequestTypeDef
 ):
     pass
 
-
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
@@ -352,22 +340,20 @@
         "DeveloperUserIdentifier": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class LookupDeveloperIdentityInputRequestTypeDef(
     _RequiredLookupDeveloperIdentityInputRequestTypeDef,
     _OptionalLookupDeveloperIdentityInputRequestTypeDef,
 ):
     pass
 
-
 MappingRuleTypeDef = TypedDict(
     "MappingRuleTypeDef",
     {
         "Claim": str,
         "MatchType": MappingRuleMatchTypeType,
         "Value": str,
         "RoleARN": str,
@@ -396,22 +382,20 @@
     {
         "UseDefaults": bool,
         "PrincipalTags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class SetPrincipalTagAttributeMapInputRequestTypeDef(
     _RequiredSetPrincipalTagAttributeMapInputRequestTypeDef,
     _OptionalSetPrincipalTagAttributeMapInputRequestTypeDef,
 ):
     pass
 
-
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -460,21 +444,19 @@
         "CognitoIdentityProviders": Sequence[CognitoIdentityProviderTypeDef],
         "SamlProviderARNs": Sequence[str],
         "IdentityPoolTags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateIdentityPoolInputRequestTypeDef(
     _RequiredCreateIdentityPoolInputRequestTypeDef, _OptionalCreateIdentityPoolInputRequestTypeDef
 ):
     pass
 
-
 _RequiredIdentityPoolRequestTypeDef = TypedDict(
     "_RequiredIdentityPoolRequestTypeDef",
     {
         "IdentityPoolId": str,
         "IdentityPoolName": str,
         "AllowUnauthenticatedIdentities": bool,
     },
@@ -489,21 +471,19 @@
         "CognitoIdentityProviders": Sequence[CognitoIdentityProviderTypeDef],
         "SamlProviderARNs": Sequence[str],
         "IdentityPoolTags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class IdentityPoolRequestTypeDef(
     _RequiredIdentityPoolRequestTypeDef, _OptionalIdentityPoolRequestTypeDef
 ):
     pass
 
-
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
@@ -678,21 +658,19 @@
     {
         "AmbiguousRoleResolution": AmbiguousRoleResolutionTypeType,
         "RulesConfiguration": RulesConfigurationTypeOutputTypeDef,
     },
     total=False,
 )
 
-
 class RoleMappingOutputTypeDef(
     _RequiredRoleMappingOutputTypeDef, _OptionalRoleMappingOutputTypeDef
 ):
     pass
 
-
 _RequiredRoleMappingTypeDef = TypedDict(
     "_RequiredRoleMappingTypeDef",
     {
         "Type": RoleMappingTypeType,
     },
 )
 _OptionalRoleMappingTypeDef = TypedDict(
@@ -700,43 +678,41 @@
     {
         "AmbiguousRoleResolution": AmbiguousRoleResolutionTypeType,
         "RulesConfiguration": RulesConfigurationTypeTypeDef,
     },
     total=False,
 )
 
-
 class RoleMappingTypeDef(_RequiredRoleMappingTypeDef, _OptionalRoleMappingTypeDef):
     pass
 
-
 GetIdentityPoolRolesResponseTypeDef = TypedDict(
     "GetIdentityPoolRolesResponseTypeDef",
     {
         "IdentityPoolId": str,
         "Roles": Dict[str, str],
         "RoleMappings": Dict[str, RoleMappingOutputTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+RoleMappingUnionTypeDef = Union[RoleMappingTypeDef, RoleMappingOutputTypeDef]
 _RequiredSetIdentityPoolRolesInputRequestTypeDef = TypedDict(
     "_RequiredSetIdentityPoolRolesInputRequestTypeDef",
     {
         "IdentityPoolId": str,
         "Roles": Mapping[str, str],
     },
 )
 _OptionalSetIdentityPoolRolesInputRequestTypeDef = TypedDict(
     "_OptionalSetIdentityPoolRolesInputRequestTypeDef",
     {
-        "RoleMappings": Mapping[str, Union[RoleMappingTypeDef, RoleMappingOutputTypeDef]],
+        "RoleMappings": Mapping[str, RoleMappingUnionTypeDef],
     },
     total=False,
 )
 
-
 class SetIdentityPoolRolesInputRequestTypeDef(
     _RequiredSetIdentityPoolRolesInputRequestTypeDef,
     _OptionalSetIdentityPoolRolesInputRequestTypeDef,
 ):
     pass
```

### Comparing `mypy-boto3-cognito-identity-1.28.15.post1/mypy_boto3_cognito_identity/type_defs.pyi` & `mypy-boto3-cognito-identity-1.28.16/mypy_boto3_cognito_identity/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_identity/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_cognito_identity.type_defs import CognitoIdentityProviderTypeDef
 
-    data: CognitoIdentityProviderTypeDef = {...}
+    data: CognitoIdentityProviderTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -23,14 +23,15 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "CognitoIdentityProviderTypeDef",
     "CredentialsTypeDef",
     "DeleteIdentitiesInputRequestTypeDef",
     "ResponseMetadataTypeDef",
     "UnprocessedIdentityIdTypeDef",
     "DeleteIdentityPoolInputRequestTypeDef",
@@ -75,14 +76,15 @@
     "ListIdentityPoolsResponseTypeDef",
     "ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef",
     "RulesConfigurationTypeOutputTypeDef",
     "RulesConfigurationTypeTypeDef",
     "RoleMappingOutputTypeDef",
     "RoleMappingTypeDef",
     "GetIdentityPoolRolesResponseTypeDef",
+    "RoleMappingUnionTypeDef",
     "SetIdentityPoolRolesInputRequestTypeDef",
 )
 
 CognitoIdentityProviderTypeDef = TypedDict(
     "CognitoIdentityProviderTypeDef",
     {
         "ProviderName": str,
@@ -162,20 +164,22 @@
     {
         "Logins": Mapping[str, str],
         "CustomRoleArn": str,
     },
     total=False,
 )
 
+
 class GetCredentialsForIdentityInputRequestTypeDef(
     _RequiredGetCredentialsForIdentityInputRequestTypeDef,
     _OptionalGetCredentialsForIdentityInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetIdInputRequestTypeDef = TypedDict(
     "_RequiredGetIdInputRequestTypeDef",
     {
         "IdentityPoolId": str,
     },
 )
 _OptionalGetIdInputRequestTypeDef = TypedDict(
@@ -183,19 +187,21 @@
     {
         "AccountId": str,
         "Logins": Mapping[str, str],
     },
     total=False,
 )
 
+
 class GetIdInputRequestTypeDef(
     _RequiredGetIdInputRequestTypeDef, _OptionalGetIdInputRequestTypeDef
 ):
     pass
 
+
 GetIdentityPoolRolesInputRequestTypeDef = TypedDict(
     "GetIdentityPoolRolesInputRequestTypeDef",
     {
         "IdentityPoolId": str,
     },
 )
 
@@ -212,39 +218,43 @@
         "IdentityId": str,
         "PrincipalTags": Mapping[str, str],
         "TokenDuration": int,
     },
     total=False,
 )
 
+
 class GetOpenIdTokenForDeveloperIdentityInputRequestTypeDef(
     _RequiredGetOpenIdTokenForDeveloperIdentityInputRequestTypeDef,
     _OptionalGetOpenIdTokenForDeveloperIdentityInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetOpenIdTokenInputRequestTypeDef = TypedDict(
     "_RequiredGetOpenIdTokenInputRequestTypeDef",
     {
         "IdentityId": str,
     },
 )
 _OptionalGetOpenIdTokenInputRequestTypeDef = TypedDict(
     "_OptionalGetOpenIdTokenInputRequestTypeDef",
     {
         "Logins": Mapping[str, str],
     },
     total=False,
 )
 
+
 class GetOpenIdTokenInputRequestTypeDef(
     _RequiredGetOpenIdTokenInputRequestTypeDef, _OptionalGetOpenIdTokenInputRequestTypeDef
 ):
     pass
 
+
 GetPrincipalTagAttributeMapInputRequestTypeDef = TypedDict(
     "GetPrincipalTagAttributeMapInputRequestTypeDef",
     {
         "IdentityPoolId": str,
         "IdentityProviderName": str,
     },
 )
@@ -281,19 +291,21 @@
     {
         "NextToken": str,
         "HideDisabled": bool,
     },
     total=False,
 )
 
+
 class ListIdentitiesInputRequestTypeDef(
     _RequiredListIdentitiesInputRequestTypeDef, _OptionalListIdentitiesInputRequestTypeDef
 ):
     pass
 
+
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -310,19 +322,21 @@
     "_OptionalListIdentityPoolsInputRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListIdentityPoolsInputRequestTypeDef(
     _RequiredListIdentityPoolsInputRequestTypeDef, _OptionalListIdentityPoolsInputRequestTypeDef
 ):
     pass
 
+
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
@@ -339,20 +353,22 @@
         "DeveloperUserIdentifier": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class LookupDeveloperIdentityInputRequestTypeDef(
     _RequiredLookupDeveloperIdentityInputRequestTypeDef,
     _OptionalLookupDeveloperIdentityInputRequestTypeDef,
 ):
     pass
 
+
 MappingRuleTypeDef = TypedDict(
     "MappingRuleTypeDef",
     {
         "Claim": str,
         "MatchType": MappingRuleMatchTypeType,
         "Value": str,
         "RoleARN": str,
@@ -381,20 +397,22 @@
     {
         "UseDefaults": bool,
         "PrincipalTags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class SetPrincipalTagAttributeMapInputRequestTypeDef(
     _RequiredSetPrincipalTagAttributeMapInputRequestTypeDef,
     _OptionalSetPrincipalTagAttributeMapInputRequestTypeDef,
 ):
     pass
 
+
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -443,19 +461,21 @@
         "CognitoIdentityProviders": Sequence[CognitoIdentityProviderTypeDef],
         "SamlProviderARNs": Sequence[str],
         "IdentityPoolTags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateIdentityPoolInputRequestTypeDef(
     _RequiredCreateIdentityPoolInputRequestTypeDef, _OptionalCreateIdentityPoolInputRequestTypeDef
 ):
     pass
 
+
 _RequiredIdentityPoolRequestTypeDef = TypedDict(
     "_RequiredIdentityPoolRequestTypeDef",
     {
         "IdentityPoolId": str,
         "IdentityPoolName": str,
         "AllowUnauthenticatedIdentities": bool,
     },
@@ -470,19 +490,21 @@
         "CognitoIdentityProviders": Sequence[CognitoIdentityProviderTypeDef],
         "SamlProviderARNs": Sequence[str],
         "IdentityPoolTags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class IdentityPoolRequestTypeDef(
     _RequiredIdentityPoolRequestTypeDef, _OptionalIdentityPoolRequestTypeDef
 ):
     pass
 
+
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
@@ -657,19 +679,21 @@
     {
         "AmbiguousRoleResolution": AmbiguousRoleResolutionTypeType,
         "RulesConfiguration": RulesConfigurationTypeOutputTypeDef,
     },
     total=False,
 )
 
+
 class RoleMappingOutputTypeDef(
     _RequiredRoleMappingOutputTypeDef, _OptionalRoleMappingOutputTypeDef
 ):
     pass
 
+
 _RequiredRoleMappingTypeDef = TypedDict(
     "_RequiredRoleMappingTypeDef",
     {
         "Type": RoleMappingTypeType,
     },
 )
 _OptionalRoleMappingTypeDef = TypedDict(
@@ -677,40 +701,44 @@
     {
         "AmbiguousRoleResolution": AmbiguousRoleResolutionTypeType,
         "RulesConfiguration": RulesConfigurationTypeTypeDef,
     },
     total=False,
 )
 
+
 class RoleMappingTypeDef(_RequiredRoleMappingTypeDef, _OptionalRoleMappingTypeDef):
     pass
 
+
 GetIdentityPoolRolesResponseTypeDef = TypedDict(
     "GetIdentityPoolRolesResponseTypeDef",
     {
         "IdentityPoolId": str,
         "Roles": Dict[str, str],
         "RoleMappings": Dict[str, RoleMappingOutputTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+RoleMappingUnionTypeDef = Union[RoleMappingTypeDef, RoleMappingOutputTypeDef]
 _RequiredSetIdentityPoolRolesInputRequestTypeDef = TypedDict(
     "_RequiredSetIdentityPoolRolesInputRequestTypeDef",
     {
         "IdentityPoolId": str,
         "Roles": Mapping[str, str],
     },
 )
 _OptionalSetIdentityPoolRolesInputRequestTypeDef = TypedDict(
     "_OptionalSetIdentityPoolRolesInputRequestTypeDef",
     {
-        "RoleMappings": Mapping[str, Union[RoleMappingTypeDef, RoleMappingOutputTypeDef]],
+        "RoleMappings": Mapping[str, RoleMappingUnionTypeDef],
     },
     total=False,
 )
 
+
 class SetIdentityPoolRolesInputRequestTypeDef(
     _RequiredSetIdentityPoolRolesInputRequestTypeDef,
     _OptionalSetIdentityPoolRolesInputRequestTypeDef,
 ):
     pass
```

### Comparing `mypy-boto3-cognito-identity-1.28.15.post1/mypy_boto3_cognito_identity.egg-info/PKG-INFO` & `mypy-boto3-cognito-identity-1.28.16/mypy_boto3_cognito_identity.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cognito-identity
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.CognitoIdentity 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.CognitoIdentity 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_identity/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 cognito-identity type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 cognito-identity type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cognito-identity.svg?color=blue)](https://pypi.org/project/mypy-boto3-cognito-identity)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_identity/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cognito-identity)](https://pepy.tech/project/mypy-boto3-cognito-identity)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CognitoIdentity 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity)
+[boto3.CognitoIdentity 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity)
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
 [mypy-boto3-cognito-identity docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_identity/).
 
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
@@ -317,20 +317,20 @@
 )
 
 
 def check_value(value: AmbiguousRoleResolutionTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_cognito_identity.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_cognito_identity.type_defs import (
     CognitoIdentityProviderTypeDef,
     CredentialsTypeDef,
     DeleteIdentitiesInputRequestTypeDef,
     ResponseMetadataTypeDef,
@@ -377,19 +377,20 @@
     ListIdentityPoolsResponseTypeDef,
     ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef,
     RulesConfigurationTypeOutputTypeDef,
     RulesConfigurationTypeTypeDef,
     RoleMappingOutputTypeDef,
     RoleMappingTypeDef,
     GetIdentityPoolRolesResponseTypeDef,
+    RoleMappingUnionTypeDef,
     SetIdentityPoolRolesInputRequestTypeDef,
 )
 
 
-def get_structure() -> CognitoIdentityProviderTypeDef:
+def get_value() -> CognitoIdentityProviderTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-cognito-identity-1.28.15.post1/mypy_boto3_cognito_identity.egg-info/SOURCES.txt` & `mypy-boto3-cognito-identity-1.28.16/mypy_boto3_cognito_identity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-identity-1.28.15.post1/setup.py` & `mypy-boto3-cognito-identity-1.28.16/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-cognito-identity",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_cognito_identity"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CognitoIdentity 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.CognitoIdentity 1.28.16 service generated with"
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
-    keywords="boto3 cognito-identity type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 cognito-identity type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_cognito_identity": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_identity/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

