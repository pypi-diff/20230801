# Comparing `tmp/mypy-boto3-workspaces-web-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-workspaces-web-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-workspaces-web-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:27 2023, max compression
+gzip compressed data, was "mypy-boto3-workspaces-web-1.28.16.tar", last modified: Tue Aug  1 11:38:06 2023, max compression
```

## Comparing `mypy-boto3-workspaces-web-1.28.15.post1.tar` & `mypy-boto3-workspaces-web-1.28.16.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:27.397463 mypy-boto3-workspaces-web-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 10:01:56.000000 mypy-boto3-workspaces-web-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17445 2023-07-29 10:04:27.385463 mypy-boto3-workspaces-web-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15925 2023-07-29 10:01:56.000000 mypy-boto3-workspaces-web-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:27.385463 mypy-boto3-workspaces-web-1.28.15.post1/mypy_boto3_workspaces_web/
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-29 10:01:56.000000 mypy-boto3-workspaces-web-1.28.15.post1/mypy_boto3_workspaces_web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-29 10:01:56.000000 mypy-boto3-workspaces-web-1.28.15.post1/mypy_boto3_workspaces_web/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-29 10:01:56.000000 mypy-boto3-workspaces-web-1.28.15.post1/mypy_boto3_workspaces_web/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37970 2023-07-29 10:01:56.000000 mypy-boto3-workspaces-web-1.28.15.post1/mypy_boto3_workspaces_web/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    37906 2023-07-29 10:01:56.000000 mypy-boto3-workspaces-web-1.28.15.post1/mypy_boto3_workspaces_web/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8417 2023-07-29 10:01:57.000000 mypy-boto3-workspaces-web-1.28.15.post1/mypy_boto3_workspaces_web/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8415 2023-07-29 10:01:56.000000 mypy-boto3-workspaces-web-1.28.15.post1/mypy_boto3_workspaces_web/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 10:01:56.000000 mypy-boto3-workspaces-web-1.28.15.post1/mypy_boto3_workspaces_web/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    41306 2023-07-29 10:01:58.000000 mypy-boto3-workspaces-web-1.28.15.post1/mypy_boto3_workspaces_web/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    41255 2023-07-29 10:01:57.000000 mypy-boto3-workspaces-web-1.28.15.post1/mypy_boto3_workspaces_web/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 10:01:56.000000 mypy-boto3-workspaces-web-1.28.15.post1/mypy_boto3_workspaces_web/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:27.385463 mypy-boto3-workspaces-web-1.28.15.post1/mypy_boto3_workspaces_web.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17445 2023-07-29 10:04:27.000000 mypy-boto3-workspaces-web-1.28.15.post1/mypy_boto3_workspaces_web.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-29 10:04:27.000000 mypy-boto3-workspaces-web-1.28.15.post1/mypy_boto3_workspaces_web.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:27.000000 mypy-boto3-workspaces-web-1.28.15.post1/mypy_boto3_workspaces_web.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:27.000000 mypy-boto3-workspaces-web-1.28.15.post1/mypy_boto3_workspaces_web.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:27.000000 mypy-boto3-workspaces-web-1.28.15.post1/mypy_boto3_workspaces_web.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-29 10:04:27.000000 mypy-boto3-workspaces-web-1.28.15.post1/mypy_boto3_workspaces_web.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:27.397463 mypy-boto3-workspaces-web-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-29 10:01:56.000000 mypy-boto3-workspaces-web-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:38:06.696653 mypy-boto3-workspaces-web-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:35:37.000000 mypy-boto3-workspaces-web-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17452 2023-08-01 11:38:06.696653 mypy-boto3-workspaces-web-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15941 2023-08-01 11:35:37.000000 mypy-boto3-workspaces-web-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:38:06.696653 mypy-boto3-workspaces-web-1.28.16/mypy_boto3_workspaces_web/
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-08-01 11:35:37.000000 mypy-boto3-workspaces-web-1.28.16/mypy_boto3_workspaces_web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-08-01 11:35:37.000000 mypy-boto3-workspaces-web-1.28.16/mypy_boto3_workspaces_web/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-08-01 11:35:37.000000 mypy-boto3-workspaces-web-1.28.16/mypy_boto3_workspaces_web/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37872 2023-08-01 11:35:37.000000 mypy-boto3-workspaces-web-1.28.16/mypy_boto3_workspaces_web/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37808 2023-08-01 11:35:37.000000 mypy-boto3-workspaces-web-1.28.16/mypy_boto3_workspaces_web/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8417 2023-08-01 11:35:37.000000 mypy-boto3-workspaces-web-1.28.16/mypy_boto3_workspaces_web/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8415 2023-08-01 11:35:37.000000 mypy-boto3-workspaces-web-1.28.16/mypy_boto3_workspaces_web/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:35:37.000000 mypy-boto3-workspaces-web-1.28.16/mypy_boto3_workspaces_web/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    41319 2023-08-01 11:35:38.000000 mypy-boto3-workspaces-web-1.28.16/mypy_boto3_workspaces_web/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41268 2023-08-01 11:35:38.000000 mypy-boto3-workspaces-web-1.28.16/mypy_boto3_workspaces_web/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:35:37.000000 mypy-boto3-workspaces-web-1.28.16/mypy_boto3_workspaces_web/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:38:06.696653 mypy-boto3-workspaces-web-1.28.16/mypy_boto3_workspaces_web.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17452 2023-08-01 11:38:06.000000 mypy-boto3-workspaces-web-1.28.16/mypy_boto3_workspaces_web.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-08-01 11:38:06.000000 mypy-boto3-workspaces-web-1.28.16/mypy_boto3_workspaces_web.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:38:06.000000 mypy-boto3-workspaces-web-1.28.16/mypy_boto3_workspaces_web.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:38:06.000000 mypy-boto3-workspaces-web-1.28.16/mypy_boto3_workspaces_web.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:38:06.000000 mypy-boto3-workspaces-web-1.28.16/mypy_boto3_workspaces_web.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-01 11:38:06.000000 mypy-boto3-workspaces-web-1.28.16/mypy_boto3_workspaces_web.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:38:06.696653 mypy-boto3-workspaces-web-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-08-01 11:35:37.000000 mypy-boto3-workspaces-web-1.28.16/setup.py
```

### Comparing `mypy-boto3-workspaces-web-1.28.15.post1/LICENSE` & `mypy-boto3-workspaces-web-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workspaces-web-1.28.15.post1/PKG-INFO` & `mypy-boto3-workspaces-web-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-workspaces-web
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.WorkSpacesWeb 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.WorkSpacesWeb 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 workspaces-web type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 workspaces-web type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-workspaces-web.svg?color=blue)](https://pypi.org/project/mypy-boto3-workspaces-web)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-workspaces-web)](https://pepy.tech/project/mypy-boto3-workspaces-web)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WorkSpacesWeb 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb)
+[boto3.WorkSpacesWeb 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb)
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
 [mypy-boto3-workspaces-web docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/).
 
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
@@ -294,30 +294,31 @@
 )
 
 
 def check_value(value: AuthenticationTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_workspaces_web.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_workspaces_web.type_defs import (
     AssociateBrowserSettingsRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     AssociateIpAccessSettingsRequestRequestTypeDef,
     AssociateNetworkSettingsRequestRequestTypeDef,
     AssociateTrustStoreRequestRequestTypeDef,
     AssociateUserAccessLoggingSettingsRequestRequestTypeDef,
     AssociateUserSettingsRequestRequestTypeDef,
+    BlobTypeDef,
     BrowserSettingsSummaryTypeDef,
     BrowserSettingsTypeDef,
     CertificateSummaryTypeDef,
     CertificateTypeDef,
     TagTypeDef,
     CreateIdentityProviderRequestRequestTypeDef,
     IpRuleTypeDef,
@@ -369,15 +370,14 @@
     ListUserSettingsRequestRequestTypeDef,
     UserSettingsSummaryTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateBrowserSettingsRequestRequestTypeDef,
     UpdateIdentityProviderRequestRequestTypeDef,
     UpdateNetworkSettingsRequestRequestTypeDef,
     UpdatePortalRequestRequestTypeDef,
-    UpdateTrustStoreRequestRequestTypeDef,
     UpdateUserAccessLoggingSettingsRequestRequestTypeDef,
     UpdateUserSettingsRequestRequestTypeDef,
     AssociateBrowserSettingsResponseTypeDef,
     AssociateIpAccessSettingsResponseTypeDef,
     AssociateNetworkSettingsResponseTypeDef,
     AssociateTrustStoreResponseTypeDef,
     AssociateUserAccessLoggingSettingsResponseTypeDef,
@@ -388,14 +388,15 @@
     CreateNetworkSettingsResponseTypeDef,
     CreatePortalResponseTypeDef,
     CreateTrustStoreResponseTypeDef,
     CreateUserAccessLoggingSettingsResponseTypeDef,
     CreateUserSettingsResponseTypeDef,
     GetPortalServiceProviderMetadataResponseTypeDef,
     UpdateTrustStoreResponseTypeDef,
+    UpdateTrustStoreRequestRequestTypeDef,
     ListBrowserSettingsResponseTypeDef,
     GetBrowserSettingsResponseTypeDef,
     UpdateBrowserSettingsResponseTypeDef,
     ListTrustStoreCertificatesResponseTypeDef,
     GetTrustStoreCertificateResponseTypeDef,
     CreateBrowserSettingsRequestRequestTypeDef,
     CreateNetworkSettingsRequestRequestTypeDef,
@@ -427,15 +428,15 @@
     ListUserAccessLoggingSettingsResponseTypeDef,
     ListUserSettingsResponseTypeDef,
     GetIpAccessSettingsResponseTypeDef,
     UpdateIpAccessSettingsResponseTypeDef,
 )
 
 
-def get_structure() -> AssociateBrowserSettingsRequestRequestTypeDef:
+def get_value() -> AssociateBrowserSettingsRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-workspaces-web-1.28.15.post1/README.md` & `mypy-boto3-workspaces-web-1.28.16/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-workspaces-web.svg?color=blue)](https://pypi.org/project/mypy-boto3-workspaces-web)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-workspaces-web)](https://pepy.tech/project/mypy-boto3-workspaces-web)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WorkSpacesWeb 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb)
+[boto3.WorkSpacesWeb 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb)
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
 [mypy-boto3-workspaces-web docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/).
 
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
@@ -262,30 +262,31 @@
 )
 
 
 def check_value(value: AuthenticationTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_workspaces_web.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_workspaces_web.type_defs import (
     AssociateBrowserSettingsRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     AssociateIpAccessSettingsRequestRequestTypeDef,
     AssociateNetworkSettingsRequestRequestTypeDef,
     AssociateTrustStoreRequestRequestTypeDef,
     AssociateUserAccessLoggingSettingsRequestRequestTypeDef,
     AssociateUserSettingsRequestRequestTypeDef,
+    BlobTypeDef,
     BrowserSettingsSummaryTypeDef,
     BrowserSettingsTypeDef,
     CertificateSummaryTypeDef,
     CertificateTypeDef,
     TagTypeDef,
     CreateIdentityProviderRequestRequestTypeDef,
     IpRuleTypeDef,
@@ -337,15 +338,14 @@
     ListUserSettingsRequestRequestTypeDef,
     UserSettingsSummaryTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateBrowserSettingsRequestRequestTypeDef,
     UpdateIdentityProviderRequestRequestTypeDef,
     UpdateNetworkSettingsRequestRequestTypeDef,
     UpdatePortalRequestRequestTypeDef,
-    UpdateTrustStoreRequestRequestTypeDef,
     UpdateUserAccessLoggingSettingsRequestRequestTypeDef,
     UpdateUserSettingsRequestRequestTypeDef,
     AssociateBrowserSettingsResponseTypeDef,
     AssociateIpAccessSettingsResponseTypeDef,
     AssociateNetworkSettingsResponseTypeDef,
     AssociateTrustStoreResponseTypeDef,
     AssociateUserAccessLoggingSettingsResponseTypeDef,
@@ -356,14 +356,15 @@
     CreateNetworkSettingsResponseTypeDef,
     CreatePortalResponseTypeDef,
     CreateTrustStoreResponseTypeDef,
     CreateUserAccessLoggingSettingsResponseTypeDef,
     CreateUserSettingsResponseTypeDef,
     GetPortalServiceProviderMetadataResponseTypeDef,
     UpdateTrustStoreResponseTypeDef,
+    UpdateTrustStoreRequestRequestTypeDef,
     ListBrowserSettingsResponseTypeDef,
     GetBrowserSettingsResponseTypeDef,
     UpdateBrowserSettingsResponseTypeDef,
     ListTrustStoreCertificatesResponseTypeDef,
     GetTrustStoreCertificateResponseTypeDef,
     CreateBrowserSettingsRequestRequestTypeDef,
     CreateNetworkSettingsRequestRequestTypeDef,
@@ -395,15 +396,15 @@
     ListUserAccessLoggingSettingsResponseTypeDef,
     ListUserSettingsResponseTypeDef,
     GetIpAccessSettingsResponseTypeDef,
     UpdateIpAccessSettingsResponseTypeDef,
 )
 
 
-def get_structure() -> AssociateBrowserSettingsRequestRequestTypeDef:
+def get_value() -> AssociateBrowserSettingsRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-workspaces-web-1.28.15.post1/mypy_boto3_workspaces_web/__main__.py` & `mypy-boto3-workspaces-web-1.28.16/mypy_boto3_workspaces_web/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.WorkSpacesWeb 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.WorkSpacesWeb 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb\nOther"
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

### Comparing `mypy-boto3-workspaces-web-1.28.15.post1/mypy_boto3_workspaces_web/client.py` & `mypy-boto3-workspaces-web-1.28.16/mypy_boto3_workspaces_web/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,27 +9,27 @@
     from boto3.session import Session
     from mypy_boto3_workspaces_web.client import WorkSpacesWebClient
 
     session = Session()
     client: WorkSpacesWebClient = session.client("workspaces-web")
     ```
 """
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
 from .literals import AuthenticationTypeType, EnabledTypeType, IdentityProviderTypeType
 from .type_defs import (
     AssociateBrowserSettingsResponseTypeDef,
     AssociateIpAccessSettingsResponseTypeDef,
     AssociateNetworkSettingsResponseTypeDef,
     AssociateTrustStoreResponseTypeDef,
     AssociateUserAccessLoggingSettingsResponseTypeDef,
     AssociateUserSettingsResponseTypeDef,
+    BlobTypeDef,
     CreateBrowserSettingsResponseTypeDef,
     CreateIdentityProviderResponseTypeDef,
     CreateIpAccessSettingsResponseTypeDef,
     CreateNetworkSettingsResponseTypeDef,
     CreatePortalResponseTypeDef,
     CreateTrustStoreResponseTypeDef,
     CreateUserAccessLoggingSettingsResponseTypeDef,
@@ -264,15 +264,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.create_portal)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/client/#create_portal)
         """
 
     def create_trust_store(
         self,
         *,
-        certificateList: Sequence[Union[str, bytes, IO[Any], StreamingBody]],
+        certificateList: Sequence[BlobTypeDef],
         clientToken: str = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateTrustStoreResponseTypeDef:
         """
         Creates a trust store that can be associated with a web portal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.create_trust_store)
@@ -716,15 +716,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/client/#update_portal)
         """
 
     def update_trust_store(
         self,
         *,
         trustStoreArn: str,
-        certificatesToAdd: Sequence[Union[str, bytes, IO[Any], StreamingBody]] = ...,
+        certificatesToAdd: Sequence[BlobTypeDef] = ...,
         certificatesToDelete: Sequence[str] = ...,
         clientToken: str = ...
     ) -> UpdateTrustStoreResponseTypeDef:
         """
         Updates the trust store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.update_trust_store)
```

### Comparing `mypy-boto3-workspaces-web-1.28.15.post1/mypy_boto3_workspaces_web/client.pyi` & `mypy-boto3-workspaces-web-1.28.16/mypy_boto3_workspaces_web/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -9,27 +9,27 @@
     from boto3.session import Session
     from mypy_boto3_workspaces_web.client import WorkSpacesWebClient
 
     session = Session()
     client: WorkSpacesWebClient = session.client("workspaces-web")
     ```
 """
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
 from .literals import AuthenticationTypeType, EnabledTypeType, IdentityProviderTypeType
 from .type_defs import (
     AssociateBrowserSettingsResponseTypeDef,
     AssociateIpAccessSettingsResponseTypeDef,
     AssociateNetworkSettingsResponseTypeDef,
     AssociateTrustStoreResponseTypeDef,
     AssociateUserAccessLoggingSettingsResponseTypeDef,
     AssociateUserSettingsResponseTypeDef,
+    BlobTypeDef,
     CreateBrowserSettingsResponseTypeDef,
     CreateIdentityProviderResponseTypeDef,
     CreateIpAccessSettingsResponseTypeDef,
     CreateNetworkSettingsResponseTypeDef,
     CreatePortalResponseTypeDef,
     CreateTrustStoreResponseTypeDef,
     CreateUserAccessLoggingSettingsResponseTypeDef,
@@ -247,15 +247,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.create_portal)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/client/#create_portal)
         """
     def create_trust_store(
         self,
         *,
-        certificateList: Sequence[Union[str, bytes, IO[Any], StreamingBody]],
+        certificateList: Sequence[BlobTypeDef],
         clientToken: str = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateTrustStoreResponseTypeDef:
         """
         Creates a trust store that can be associated with a web portal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.create_trust_store)
@@ -654,15 +654,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.update_portal)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/client/#update_portal)
         """
     def update_trust_store(
         self,
         *,
         trustStoreArn: str,
-        certificatesToAdd: Sequence[Union[str, bytes, IO[Any], StreamingBody]] = ...,
+        certificatesToAdd: Sequence[BlobTypeDef] = ...,
         certificatesToDelete: Sequence[str] = ...,
         clientToken: str = ...
     ) -> UpdateTrustStoreResponseTypeDef:
         """
         Updates the trust store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.update_trust_store)
```

### Comparing `mypy-boto3-workspaces-web-1.28.15.post1/mypy_boto3_workspaces_web/literals.py` & `mypy-boto3-workspaces-web-1.28.16/mypy_boto3_workspaces_web/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workspaces-web-1.28.15.post1/mypy_boto3_workspaces_web/literals.pyi` & `mypy-boto3-workspaces-web-1.28.16/mypy_boto3_workspaces_web/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workspaces-web-1.28.15.post1/mypy_boto3_workspaces_web/type_defs.py` & `mypy-boto3-workspaces-web-1.28.16/mypy_boto3_workspaces_web/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_workspaces_web.type_defs import AssociateBrowserSettingsRequestRequestTypeDef
 
-    data: AssociateBrowserSettingsRequestRequestTypeDef = {...}
+    data: AssociateBrowserSettingsRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -38,14 +38,15 @@
     "AssociateBrowserSettingsRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AssociateIpAccessSettingsRequestRequestTypeDef",
     "AssociateNetworkSettingsRequestRequestTypeDef",
     "AssociateTrustStoreRequestRequestTypeDef",
     "AssociateUserAccessLoggingSettingsRequestRequestTypeDef",
     "AssociateUserSettingsRequestRequestTypeDef",
+    "BlobTypeDef",
     "BrowserSettingsSummaryTypeDef",
     "BrowserSettingsTypeDef",
     "CertificateSummaryTypeDef",
     "CertificateTypeDef",
     "TagTypeDef",
     "CreateIdentityProviderRequestRequestTypeDef",
     "IpRuleTypeDef",
@@ -97,15 +98,14 @@
     "ListUserSettingsRequestRequestTypeDef",
     "UserSettingsSummaryTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateBrowserSettingsRequestRequestTypeDef",
     "UpdateIdentityProviderRequestRequestTypeDef",
     "UpdateNetworkSettingsRequestRequestTypeDef",
     "UpdatePortalRequestRequestTypeDef",
-    "UpdateTrustStoreRequestRequestTypeDef",
     "UpdateUserAccessLoggingSettingsRequestRequestTypeDef",
     "UpdateUserSettingsRequestRequestTypeDef",
     "AssociateBrowserSettingsResponseTypeDef",
     "AssociateIpAccessSettingsResponseTypeDef",
     "AssociateNetworkSettingsResponseTypeDef",
     "AssociateTrustStoreResponseTypeDef",
     "AssociateUserAccessLoggingSettingsResponseTypeDef",
@@ -116,14 +116,15 @@
     "CreateNetworkSettingsResponseTypeDef",
     "CreatePortalResponseTypeDef",
     "CreateTrustStoreResponseTypeDef",
     "CreateUserAccessLoggingSettingsResponseTypeDef",
     "CreateUserSettingsResponseTypeDef",
     "GetPortalServiceProviderMetadataResponseTypeDef",
     "UpdateTrustStoreResponseTypeDef",
+    "UpdateTrustStoreRequestRequestTypeDef",
     "ListBrowserSettingsResponseTypeDef",
     "GetBrowserSettingsResponseTypeDef",
     "UpdateBrowserSettingsResponseTypeDef",
     "ListTrustStoreCertificatesResponseTypeDef",
     "GetTrustStoreCertificateResponseTypeDef",
     "CreateBrowserSettingsRequestRequestTypeDef",
     "CreateNetworkSettingsRequestRequestTypeDef",
@@ -213,14 +214,15 @@
     "AssociateUserSettingsRequestRequestTypeDef",
     {
         "portalArn": str,
         "userSettingsArn": str,
     },
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 BrowserSettingsSummaryTypeDef = TypedDict(
     "BrowserSettingsSummaryTypeDef",
     {
         "browserSettingsArn": str,
     },
     total=False,
 )
@@ -911,37 +913,14 @@
 
 class UpdatePortalRequestRequestTypeDef(
     _RequiredUpdatePortalRequestRequestTypeDef, _OptionalUpdatePortalRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredUpdateTrustStoreRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateTrustStoreRequestRequestTypeDef",
-    {
-        "trustStoreArn": str,
-    },
-)
-_OptionalUpdateTrustStoreRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateTrustStoreRequestRequestTypeDef",
-    {
-        "certificatesToAdd": Sequence[Union[str, bytes, IO[Any], StreamingBody]],
-        "certificatesToDelete": Sequence[str],
-        "clientToken": str,
-    },
-    total=False,
-)
-
-
-class UpdateTrustStoreRequestRequestTypeDef(
-    _RequiredUpdateTrustStoreRequestRequestTypeDef, _OptionalUpdateTrustStoreRequestRequestTypeDef
-):
-    pass
-
-
 _RequiredUpdateUserAccessLoggingSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateUserAccessLoggingSettingsRequestRequestTypeDef",
     {
         "userAccessLoggingSettingsArn": str,
     },
 )
 _OptionalUpdateUserAccessLoggingSettingsRequestRequestTypeDef = TypedDict(
@@ -1122,14 +1101,37 @@
     "UpdateTrustStoreResponseTypeDef",
     {
         "trustStoreArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredUpdateTrustStoreRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateTrustStoreRequestRequestTypeDef",
+    {
+        "trustStoreArn": str,
+    },
+)
+_OptionalUpdateTrustStoreRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateTrustStoreRequestRequestTypeDef",
+    {
+        "certificatesToAdd": Sequence[BlobTypeDef],
+        "certificatesToDelete": Sequence[str],
+        "clientToken": str,
+    },
+    total=False,
+)
+
+
+class UpdateTrustStoreRequestRequestTypeDef(
+    _RequiredUpdateTrustStoreRequestRequestTypeDef, _OptionalUpdateTrustStoreRequestRequestTypeDef
+):
+    pass
+
+
 ListBrowserSettingsResponseTypeDef = TypedDict(
     "ListBrowserSettingsResponseTypeDef",
     {
         "browserSettings": List[BrowserSettingsSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1232,15 +1234,15 @@
     },
     total=False,
 )
 
 _RequiredCreateTrustStoreRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTrustStoreRequestRequestTypeDef",
     {
-        "certificateList": Sequence[Union[str, bytes, IO[Any], StreamingBody]],
+        "certificateList": Sequence[BlobTypeDef],
     },
 )
 _OptionalCreateTrustStoreRequestRequestTypeDef = TypedDict(
     "_OptionalCreateTrustStoreRequestRequestTypeDef",
     {
         "clientToken": str,
         "tags": Sequence[TagTypeDef],
```

### Comparing `mypy-boto3-workspaces-web-1.28.15.post1/mypy_boto3_workspaces_web/type_defs.pyi` & `mypy-boto3-workspaces-web-1.28.16/mypy_boto3_workspaces_web/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_workspaces_web.type_defs import AssociateBrowserSettingsRequestRequestTypeDef
 
-    data: AssociateBrowserSettingsRequestRequestTypeDef = {...}
+    data: AssociateBrowserSettingsRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -37,14 +37,15 @@
     "AssociateBrowserSettingsRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AssociateIpAccessSettingsRequestRequestTypeDef",
     "AssociateNetworkSettingsRequestRequestTypeDef",
     "AssociateTrustStoreRequestRequestTypeDef",
     "AssociateUserAccessLoggingSettingsRequestRequestTypeDef",
     "AssociateUserSettingsRequestRequestTypeDef",
+    "BlobTypeDef",
     "BrowserSettingsSummaryTypeDef",
     "BrowserSettingsTypeDef",
     "CertificateSummaryTypeDef",
     "CertificateTypeDef",
     "TagTypeDef",
     "CreateIdentityProviderRequestRequestTypeDef",
     "IpRuleTypeDef",
@@ -96,15 +97,14 @@
     "ListUserSettingsRequestRequestTypeDef",
     "UserSettingsSummaryTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateBrowserSettingsRequestRequestTypeDef",
     "UpdateIdentityProviderRequestRequestTypeDef",
     "UpdateNetworkSettingsRequestRequestTypeDef",
     "UpdatePortalRequestRequestTypeDef",
-    "UpdateTrustStoreRequestRequestTypeDef",
     "UpdateUserAccessLoggingSettingsRequestRequestTypeDef",
     "UpdateUserSettingsRequestRequestTypeDef",
     "AssociateBrowserSettingsResponseTypeDef",
     "AssociateIpAccessSettingsResponseTypeDef",
     "AssociateNetworkSettingsResponseTypeDef",
     "AssociateTrustStoreResponseTypeDef",
     "AssociateUserAccessLoggingSettingsResponseTypeDef",
@@ -115,14 +115,15 @@
     "CreateNetworkSettingsResponseTypeDef",
     "CreatePortalResponseTypeDef",
     "CreateTrustStoreResponseTypeDef",
     "CreateUserAccessLoggingSettingsResponseTypeDef",
     "CreateUserSettingsResponseTypeDef",
     "GetPortalServiceProviderMetadataResponseTypeDef",
     "UpdateTrustStoreResponseTypeDef",
+    "UpdateTrustStoreRequestRequestTypeDef",
     "ListBrowserSettingsResponseTypeDef",
     "GetBrowserSettingsResponseTypeDef",
     "UpdateBrowserSettingsResponseTypeDef",
     "ListTrustStoreCertificatesResponseTypeDef",
     "GetTrustStoreCertificateResponseTypeDef",
     "CreateBrowserSettingsRequestRequestTypeDef",
     "CreateNetworkSettingsRequestRequestTypeDef",
@@ -212,14 +213,15 @@
     "AssociateUserSettingsRequestRequestTypeDef",
     {
         "portalArn": str,
         "userSettingsArn": str,
     },
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 BrowserSettingsSummaryTypeDef = TypedDict(
     "BrowserSettingsSummaryTypeDef",
     {
         "browserSettingsArn": str,
     },
     total=False,
 )
@@ -884,35 +886,14 @@
 )
 
 class UpdatePortalRequestRequestTypeDef(
     _RequiredUpdatePortalRequestRequestTypeDef, _OptionalUpdatePortalRequestRequestTypeDef
 ):
     pass
 
-_RequiredUpdateTrustStoreRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateTrustStoreRequestRequestTypeDef",
-    {
-        "trustStoreArn": str,
-    },
-)
-_OptionalUpdateTrustStoreRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateTrustStoreRequestRequestTypeDef",
-    {
-        "certificatesToAdd": Sequence[Union[str, bytes, IO[Any], StreamingBody]],
-        "certificatesToDelete": Sequence[str],
-        "clientToken": str,
-    },
-    total=False,
-)
-
-class UpdateTrustStoreRequestRequestTypeDef(
-    _RequiredUpdateTrustStoreRequestRequestTypeDef, _OptionalUpdateTrustStoreRequestRequestTypeDef
-):
-    pass
-
 _RequiredUpdateUserAccessLoggingSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateUserAccessLoggingSettingsRequestRequestTypeDef",
     {
         "userAccessLoggingSettingsArn": str,
     },
 )
 _OptionalUpdateUserAccessLoggingSettingsRequestRequestTypeDef = TypedDict(
@@ -1089,14 +1070,35 @@
     "UpdateTrustStoreResponseTypeDef",
     {
         "trustStoreArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredUpdateTrustStoreRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateTrustStoreRequestRequestTypeDef",
+    {
+        "trustStoreArn": str,
+    },
+)
+_OptionalUpdateTrustStoreRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateTrustStoreRequestRequestTypeDef",
+    {
+        "certificatesToAdd": Sequence[BlobTypeDef],
+        "certificatesToDelete": Sequence[str],
+        "clientToken": str,
+    },
+    total=False,
+)
+
+class UpdateTrustStoreRequestRequestTypeDef(
+    _RequiredUpdateTrustStoreRequestRequestTypeDef, _OptionalUpdateTrustStoreRequestRequestTypeDef
+):
+    pass
+
 ListBrowserSettingsResponseTypeDef = TypedDict(
     "ListBrowserSettingsResponseTypeDef",
     {
         "browserSettings": List[BrowserSettingsSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1195,15 +1197,15 @@
     },
     total=False,
 )
 
 _RequiredCreateTrustStoreRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTrustStoreRequestRequestTypeDef",
     {
-        "certificateList": Sequence[Union[str, bytes, IO[Any], StreamingBody]],
+        "certificateList": Sequence[BlobTypeDef],
     },
 )
 _OptionalCreateTrustStoreRequestRequestTypeDef = TypedDict(
     "_OptionalCreateTrustStoreRequestRequestTypeDef",
     {
         "clientToken": str,
         "tags": Sequence[TagTypeDef],
```

### Comparing `mypy-boto3-workspaces-web-1.28.15.post1/mypy_boto3_workspaces_web.egg-info/PKG-INFO` & `mypy-boto3-workspaces-web-1.28.16/mypy_boto3_workspaces_web.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-workspaces-web
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.WorkSpacesWeb 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.WorkSpacesWeb 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 workspaces-web type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 workspaces-web type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-workspaces-web.svg?color=blue)](https://pypi.org/project/mypy-boto3-workspaces-web)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-workspaces-web)](https://pepy.tech/project/mypy-boto3-workspaces-web)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WorkSpacesWeb 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb)
+[boto3.WorkSpacesWeb 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb)
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
 [mypy-boto3-workspaces-web docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/).
 
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
@@ -294,30 +294,31 @@
 )
 
 
 def check_value(value: AuthenticationTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_workspaces_web.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_workspaces_web.type_defs import (
     AssociateBrowserSettingsRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     AssociateIpAccessSettingsRequestRequestTypeDef,
     AssociateNetworkSettingsRequestRequestTypeDef,
     AssociateTrustStoreRequestRequestTypeDef,
     AssociateUserAccessLoggingSettingsRequestRequestTypeDef,
     AssociateUserSettingsRequestRequestTypeDef,
+    BlobTypeDef,
     BrowserSettingsSummaryTypeDef,
     BrowserSettingsTypeDef,
     CertificateSummaryTypeDef,
     CertificateTypeDef,
     TagTypeDef,
     CreateIdentityProviderRequestRequestTypeDef,
     IpRuleTypeDef,
@@ -369,15 +370,14 @@
     ListUserSettingsRequestRequestTypeDef,
     UserSettingsSummaryTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateBrowserSettingsRequestRequestTypeDef,
     UpdateIdentityProviderRequestRequestTypeDef,
     UpdateNetworkSettingsRequestRequestTypeDef,
     UpdatePortalRequestRequestTypeDef,
-    UpdateTrustStoreRequestRequestTypeDef,
     UpdateUserAccessLoggingSettingsRequestRequestTypeDef,
     UpdateUserSettingsRequestRequestTypeDef,
     AssociateBrowserSettingsResponseTypeDef,
     AssociateIpAccessSettingsResponseTypeDef,
     AssociateNetworkSettingsResponseTypeDef,
     AssociateTrustStoreResponseTypeDef,
     AssociateUserAccessLoggingSettingsResponseTypeDef,
@@ -388,14 +388,15 @@
     CreateNetworkSettingsResponseTypeDef,
     CreatePortalResponseTypeDef,
     CreateTrustStoreResponseTypeDef,
     CreateUserAccessLoggingSettingsResponseTypeDef,
     CreateUserSettingsResponseTypeDef,
     GetPortalServiceProviderMetadataResponseTypeDef,
     UpdateTrustStoreResponseTypeDef,
+    UpdateTrustStoreRequestRequestTypeDef,
     ListBrowserSettingsResponseTypeDef,
     GetBrowserSettingsResponseTypeDef,
     UpdateBrowserSettingsResponseTypeDef,
     ListTrustStoreCertificatesResponseTypeDef,
     GetTrustStoreCertificateResponseTypeDef,
     CreateBrowserSettingsRequestRequestTypeDef,
     CreateNetworkSettingsRequestRequestTypeDef,
@@ -427,15 +428,15 @@
     ListUserAccessLoggingSettingsResponseTypeDef,
     ListUserSettingsResponseTypeDef,
     GetIpAccessSettingsResponseTypeDef,
     UpdateIpAccessSettingsResponseTypeDef,
 )
 
 
-def get_structure() -> AssociateBrowserSettingsRequestRequestTypeDef:
+def get_value() -> AssociateBrowserSettingsRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-workspaces-web-1.28.15.post1/mypy_boto3_workspaces_web.egg-info/SOURCES.txt` & `mypy-boto3-workspaces-web-1.28.16/mypy_boto3_workspaces_web.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workspaces-web-1.28.15.post1/setup.py` & `mypy-boto3-workspaces-web-1.28.16/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-workspaces-web",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_workspaces_web"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.WorkSpacesWeb 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.WorkSpacesWeb 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 workspaces-web type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 workspaces-web type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_workspaces_web": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

