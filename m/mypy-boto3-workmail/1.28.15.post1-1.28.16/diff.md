# Comparing `tmp/mypy-boto3-workmail-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-workmail-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-workmail-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:26 2023, max compression
+gzip compressed data, was "mypy-boto3-workmail-1.28.16.tar", last modified: Tue Aug  1 11:38:05 2023, max compression
```

## Comparing `mypy-boto3-workmail-1.28.15.post1.tar` & `mypy-boto3-workmail-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:26.373459 mypy-boto3-workmail-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 10:01:45.000000 mypy-boto3-workmail-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21195 2023-07-29 10:04:26.373459 mypy-boto3-workmail-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19698 2023-07-29 10:01:45.000000 mypy-boto3-workmail-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:26.369459 mypy-boto3-workmail-1.28.15.post1/mypy_boto3_workmail/
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-07-29 10:01:45.000000 mypy-boto3-workmail-1.28.15.post1/mypy_boto3_workmail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-07-29 10:01:45.000000 mypy-boto3-workmail-1.28.15.post1/mypy_boto3_workmail/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-29 10:01:45.000000 mypy-boto3-workmail-1.28.15.post1/mypy_boto3_workmail/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    57222 2023-07-29 10:01:50.000000 mypy-boto3-workmail-1.28.15.post1/mypy_boto3_workmail/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    57126 2023-07-29 10:01:45.000000 mypy-boto3-workmail-1.28.15.post1/mypy_boto3_workmail/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10159 2023-07-29 10:01:50.000000 mypy-boto3-workmail-1.28.15.post1/mypy_boto3_workmail/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10157 2023-07-29 10:01:50.000000 mypy-boto3-workmail-1.28.15.post1/mypy_boto3_workmail/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10543 2023-07-29 10:01:50.000000 mypy-boto3-workmail-1.28.15.post1/mypy_boto3_workmail/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10532 2023-07-29 10:01:50.000000 mypy-boto3-workmail-1.28.15.post1/mypy_boto3_workmail/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 10:01:45.000000 mypy-boto3-workmail-1.28.15.post1/mypy_boto3_workmail/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    60398 2023-07-29 10:01:52.000000 mypy-boto3-workmail-1.28.15.post1/mypy_boto3_workmail/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    60317 2023-07-29 10:01:51.000000 mypy-boto3-workmail-1.28.15.post1/mypy_boto3_workmail/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 10:01:45.000000 mypy-boto3-workmail-1.28.15.post1/mypy_boto3_workmail/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:26.373459 mypy-boto3-workmail-1.28.15.post1/mypy_boto3_workmail.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21195 2023-07-29 10:04:26.000000 mypy-boto3-workmail-1.28.15.post1/mypy_boto3_workmail.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-29 10:04:26.000000 mypy-boto3-workmail-1.28.15.post1/mypy_boto3_workmail.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:26.000000 mypy-boto3-workmail-1.28.15.post1/mypy_boto3_workmail.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:26.000000 mypy-boto3-workmail-1.28.15.post1/mypy_boto3_workmail.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:26.000000 mypy-boto3-workmail-1.28.15.post1/mypy_boto3_workmail.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-29 10:04:26.000000 mypy-boto3-workmail-1.28.15.post1/mypy_boto3_workmail.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:26.373459 mypy-boto3-workmail-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-29 10:01:45.000000 mypy-boto3-workmail-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:38:05.488656 mypy-boto3-workmail-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:35:30.000000 mypy-boto3-workmail-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21220 2023-08-01 11:38:05.484656 mypy-boto3-workmail-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19732 2023-08-01 11:35:30.000000 mypy-boto3-workmail-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:38:05.476657 mypy-boto3-workmail-1.28.16/mypy_boto3_workmail/
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-08-01 11:35:30.000000 mypy-boto3-workmail-1.28.16/mypy_boto3_workmail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-08-01 11:35:30.000000 mypy-boto3-workmail-1.28.16/mypy_boto3_workmail/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-08-01 11:35:30.000000 mypy-boto3-workmail-1.28.16/mypy_boto3_workmail/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57116 2023-08-01 11:35:31.000000 mypy-boto3-workmail-1.28.16/mypy_boto3_workmail/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57020 2023-08-01 11:35:30.000000 mypy-boto3-workmail-1.28.16/mypy_boto3_workmail/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10159 2023-08-01 11:35:31.000000 mypy-boto3-workmail-1.28.16/mypy_boto3_workmail/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10157 2023-08-01 11:35:31.000000 mypy-boto3-workmail-1.28.16/mypy_boto3_workmail/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10543 2023-08-01 11:35:31.000000 mypy-boto3-workmail-1.28.16/mypy_boto3_workmail/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10532 2023-08-01 11:35:31.000000 mypy-boto3-workmail-1.28.16/mypy_boto3_workmail/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:35:30.000000 mypy-boto3-workmail-1.28.16/mypy_boto3_workmail/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    60460 2023-08-01 11:35:32.000000 mypy-boto3-workmail-1.28.16/mypy_boto3_workmail/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60380 2023-08-01 11:35:32.000000 mypy-boto3-workmail-1.28.16/mypy_boto3_workmail/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:35:30.000000 mypy-boto3-workmail-1.28.16/mypy_boto3_workmail/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:38:05.484656 mypy-boto3-workmail-1.28.16/mypy_boto3_workmail.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21220 2023-08-01 11:38:05.000000 mypy-boto3-workmail-1.28.16/mypy_boto3_workmail.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-08-01 11:38:05.000000 mypy-boto3-workmail-1.28.16/mypy_boto3_workmail.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:38:05.000000 mypy-boto3-workmail-1.28.16/mypy_boto3_workmail.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:38:05.000000 mypy-boto3-workmail-1.28.16/mypy_boto3_workmail.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:38:05.000000 mypy-boto3-workmail-1.28.16/mypy_boto3_workmail.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-01 11:38:05.000000 mypy-boto3-workmail-1.28.16/mypy_boto3_workmail.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:38:05.488656 mypy-boto3-workmail-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-08-01 11:35:30.000000 mypy-boto3-workmail-1.28.16/setup.py
```

### Comparing `mypy-boto3-workmail-1.28.15.post1/LICENSE` & `mypy-boto3-workmail-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workmail-1.28.15.post1/PKG-INFO` & `mypy-boto3-workmail-1.28.16/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-workmail
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.WorkMail 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.WorkMail 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 workmail type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 workmail type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-workmail.svg?color=blue)](https://pypi.org/project/mypy-boto3-workmail)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-workmail)](https://pepy.tech/project/mypy-boto3-workmail)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WorkMail 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail)
+[boto3.WorkMail 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail)
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
 [mypy-boto3-workmail docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail/).
 
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
@@ -357,20 +357,20 @@
 )
 
 
 def check_value(value: AccessControlRuleEffectType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_workmail.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_workmail.type_defs import (
     AccessControlRuleTypeDef,
     AssociateDelegateToResourceRequestRequestTypeDef,
     AssociateMemberToGroupRequestRequestTypeDef,
     AssumeImpersonationRoleRequestRequestTypeDef,
@@ -378,16 +378,14 @@
     LambdaAvailabilityProviderTypeDef,
     RedactedEwsAvailabilityProviderTypeDef,
     BookingOptionsTypeDef,
     CancelMailboxExportJobRequestRequestTypeDef,
     CreateAliasRequestRequestTypeDef,
     EwsAvailabilityProviderTypeDef,
     CreateGroupRequestRequestTypeDef,
-    ImpersonationRuleOutputTypeDef,
-    ImpersonationRuleTypeDef,
     CreateMobileDeviceAccessRuleRequestRequestTypeDef,
     DomainTypeDef,
     CreateResourceRequestRequestTypeDef,
     CreateUserRequestRequestTypeDef,
     DelegateTypeDef,
     DeleteAccessControlRuleRequestRequestTypeDef,
     DeleteAliasRequestRequestTypeDef,
@@ -416,21 +414,23 @@
     DnsRecordTypeDef,
     FolderConfigurationTypeDef,
     GetAccessControlEffectRequestRequestTypeDef,
     GetDefaultRetentionPolicyRequestRequestTypeDef,
     GetImpersonationRoleEffectRequestRequestTypeDef,
     ImpersonationMatchedRuleTypeDef,
     GetImpersonationRoleRequestRequestTypeDef,
+    ImpersonationRuleOutputTypeDef,
     GetMailDomainRequestRequestTypeDef,
     GetMailboxDetailsRequestRequestTypeDef,
     GetMobileDeviceAccessEffectRequestRequestTypeDef,
     MobileDeviceAccessMatchedRuleTypeDef,
     GetMobileDeviceAccessOverrideRequestRequestTypeDef,
     GroupTypeDef,
     ImpersonationRoleTypeDef,
+    ImpersonationRuleTypeDef,
     ListAccessControlRulesRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     ListAliasesRequestRequestTypeDef,
     ListAvailabilityConfigurationsRequestRequestTypeDef,
     ListGroupMembersRequestRequestTypeDef,
     MemberTypeDef,
     ListGroupsRequestRequestTypeDef,
@@ -491,26 +491,25 @@
     TestAvailabilityConfigurationResponseTypeDef,
     AvailabilityConfigurationTypeDef,
     DescribeResourceResponseTypeDef,
     UpdateResourceRequestRequestTypeDef,
     CreateAvailabilityConfigurationRequestRequestTypeDef,
     TestAvailabilityConfigurationRequestRequestTypeDef,
     UpdateAvailabilityConfigurationRequestRequestTypeDef,
-    GetImpersonationRoleResponseTypeDef,
-    CreateImpersonationRoleRequestRequestTypeDef,
-    UpdateImpersonationRoleRequestRequestTypeDef,
     CreateOrganizationRequestRequestTypeDef,
     ListResourceDelegatesResponseTypeDef,
     GetMailDomainResponseTypeDef,
     GetDefaultRetentionPolicyResponseTypeDef,
     PutRetentionPolicyRequestRequestTypeDef,
     GetImpersonationRoleEffectResponseTypeDef,
+    GetImpersonationRoleResponseTypeDef,
     GetMobileDeviceAccessEffectResponseTypeDef,
     ListGroupsResponseTypeDef,
     ListImpersonationRolesResponseTypeDef,
+    ImpersonationRuleUnionTypeDef,
     ListAliasesRequestListAliasesPaginateTypeDef,
     ListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef,
     ListGroupMembersRequestListGroupMembersPaginateTypeDef,
     ListGroupsRequestListGroupsPaginateTypeDef,
     ListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef,
     ListOrganizationsRequestListOrganizationsPaginateTypeDef,
     ListResourceDelegatesRequestListResourceDelegatesPaginateTypeDef,
@@ -524,18 +523,20 @@
     ListMobileDeviceAccessRulesResponseTypeDef,
     ListOrganizationsResponseTypeDef,
     ListResourcesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     ListUsersResponseTypeDef,
     ListAvailabilityConfigurationsResponseTypeDef,
+    CreateImpersonationRoleRequestRequestTypeDef,
+    UpdateImpersonationRoleRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AccessControlRuleTypeDef:
+def get_value() -> AccessControlRuleTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-workmail-1.28.15.post1/README.md` & `mypy-boto3-workmail-1.28.16/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-workmail.svg?color=blue)](https://pypi.org/project/mypy-boto3-workmail)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-workmail)](https://pepy.tech/project/mypy-boto3-workmail)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WorkMail 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail)
+[boto3.WorkMail 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail)
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
 [mypy-boto3-workmail docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail/).
 
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
@@ -325,20 +325,20 @@
 )
 
 
 def check_value(value: AccessControlRuleEffectType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_workmail.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_workmail.type_defs import (
     AccessControlRuleTypeDef,
     AssociateDelegateToResourceRequestRequestTypeDef,
     AssociateMemberToGroupRequestRequestTypeDef,
     AssumeImpersonationRoleRequestRequestTypeDef,
@@ -346,16 +346,14 @@
     LambdaAvailabilityProviderTypeDef,
     RedactedEwsAvailabilityProviderTypeDef,
     BookingOptionsTypeDef,
     CancelMailboxExportJobRequestRequestTypeDef,
     CreateAliasRequestRequestTypeDef,
     EwsAvailabilityProviderTypeDef,
     CreateGroupRequestRequestTypeDef,
-    ImpersonationRuleOutputTypeDef,
-    ImpersonationRuleTypeDef,
     CreateMobileDeviceAccessRuleRequestRequestTypeDef,
     DomainTypeDef,
     CreateResourceRequestRequestTypeDef,
     CreateUserRequestRequestTypeDef,
     DelegateTypeDef,
     DeleteAccessControlRuleRequestRequestTypeDef,
     DeleteAliasRequestRequestTypeDef,
@@ -384,21 +382,23 @@
     DnsRecordTypeDef,
     FolderConfigurationTypeDef,
     GetAccessControlEffectRequestRequestTypeDef,
     GetDefaultRetentionPolicyRequestRequestTypeDef,
     GetImpersonationRoleEffectRequestRequestTypeDef,
     ImpersonationMatchedRuleTypeDef,
     GetImpersonationRoleRequestRequestTypeDef,
+    ImpersonationRuleOutputTypeDef,
     GetMailDomainRequestRequestTypeDef,
     GetMailboxDetailsRequestRequestTypeDef,
     GetMobileDeviceAccessEffectRequestRequestTypeDef,
     MobileDeviceAccessMatchedRuleTypeDef,
     GetMobileDeviceAccessOverrideRequestRequestTypeDef,
     GroupTypeDef,
     ImpersonationRoleTypeDef,
+    ImpersonationRuleTypeDef,
     ListAccessControlRulesRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     ListAliasesRequestRequestTypeDef,
     ListAvailabilityConfigurationsRequestRequestTypeDef,
     ListGroupMembersRequestRequestTypeDef,
     MemberTypeDef,
     ListGroupsRequestRequestTypeDef,
@@ -459,26 +459,25 @@
     TestAvailabilityConfigurationResponseTypeDef,
     AvailabilityConfigurationTypeDef,
     DescribeResourceResponseTypeDef,
     UpdateResourceRequestRequestTypeDef,
     CreateAvailabilityConfigurationRequestRequestTypeDef,
     TestAvailabilityConfigurationRequestRequestTypeDef,
     UpdateAvailabilityConfigurationRequestRequestTypeDef,
-    GetImpersonationRoleResponseTypeDef,
-    CreateImpersonationRoleRequestRequestTypeDef,
-    UpdateImpersonationRoleRequestRequestTypeDef,
     CreateOrganizationRequestRequestTypeDef,
     ListResourceDelegatesResponseTypeDef,
     GetMailDomainResponseTypeDef,
     GetDefaultRetentionPolicyResponseTypeDef,
     PutRetentionPolicyRequestRequestTypeDef,
     GetImpersonationRoleEffectResponseTypeDef,
+    GetImpersonationRoleResponseTypeDef,
     GetMobileDeviceAccessEffectResponseTypeDef,
     ListGroupsResponseTypeDef,
     ListImpersonationRolesResponseTypeDef,
+    ImpersonationRuleUnionTypeDef,
     ListAliasesRequestListAliasesPaginateTypeDef,
     ListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef,
     ListGroupMembersRequestListGroupMembersPaginateTypeDef,
     ListGroupsRequestListGroupsPaginateTypeDef,
     ListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef,
     ListOrganizationsRequestListOrganizationsPaginateTypeDef,
     ListResourceDelegatesRequestListResourceDelegatesPaginateTypeDef,
@@ -492,18 +491,20 @@
     ListMobileDeviceAccessRulesResponseTypeDef,
     ListOrganizationsResponseTypeDef,
     ListResourcesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     ListUsersResponseTypeDef,
     ListAvailabilityConfigurationsResponseTypeDef,
+    CreateImpersonationRoleRequestRequestTypeDef,
+    UpdateImpersonationRoleRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AccessControlRuleTypeDef:
+def get_value() -> AccessControlRuleTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-workmail-1.28.15.post1/mypy_boto3_workmail/__init__.py` & `mypy-boto3-workmail-1.28.16/mypy_boto3_workmail/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workmail-1.28.15.post1/mypy_boto3_workmail/__init__.pyi` & `mypy-boto3-workmail-1.28.16/mypy_boto3_workmail/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workmail-1.28.15.post1/mypy_boto3_workmail/__main__.py` & `mypy-boto3-workmail-1.28.16/mypy_boto3_workmail/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.WorkMail 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.WorkMail 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail\nOther"
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

### Comparing `mypy-boto3-workmail-1.28.15.post1/mypy_boto3_workmail/client.py` & `mypy-boto3-workmail-1.28.16/mypy_boto3_workmail/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_workmail.client import WorkMailClient
 
     session = Session()
     client: WorkMailClient = session.client("workmail")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AccessControlRuleEffectType,
     ImpersonationRoleTypeType,
     MobileDeviceAccessRuleEffectType,
@@ -60,16 +60,15 @@
     GetDefaultRetentionPolicyResponseTypeDef,
     GetImpersonationRoleEffectResponseTypeDef,
     GetImpersonationRoleResponseTypeDef,
     GetMailboxDetailsResponseTypeDef,
     GetMailDomainResponseTypeDef,
     GetMobileDeviceAccessEffectResponseTypeDef,
     GetMobileDeviceAccessOverrideResponseTypeDef,
-    ImpersonationRuleOutputTypeDef,
-    ImpersonationRuleTypeDef,
+    ImpersonationRuleUnionTypeDef,
     LambdaAvailabilityProviderTypeDef,
     ListAccessControlRulesResponseTypeDef,
     ListAliasesResponseTypeDef,
     ListAvailabilityConfigurationsResponseTypeDef,
     ListGroupMembersResponseTypeDef,
     ListGroupsResponseTypeDef,
     ListImpersonationRolesResponseTypeDef,
@@ -240,15 +239,15 @@
 
     def create_impersonation_role(
         self,
         *,
         OrganizationId: str,
         Name: str,
         Type: ImpersonationRoleTypeType,
-        Rules: Sequence[Union[ImpersonationRuleTypeDef, ImpersonationRuleOutputTypeDef]],
+        Rules: Sequence[ImpersonationRuleUnionTypeDef],
         ClientToken: str = ...,
         Description: str = ...
     ) -> CreateImpersonationRoleResponseTypeDef:
         """
         Creates an impersonation role for the given WorkMail organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Client.create_impersonation_role)
@@ -1016,15 +1015,15 @@
     def update_impersonation_role(
         self,
         *,
         OrganizationId: str,
         ImpersonationRoleId: str,
         Name: str,
         Type: ImpersonationRoleTypeType,
-        Rules: Sequence[Union[ImpersonationRuleTypeDef, ImpersonationRuleOutputTypeDef]],
+        Rules: Sequence[ImpersonationRuleUnionTypeDef],
         Description: str = ...
     ) -> Dict[str, Any]:
         """
         Updates an impersonation role for the given WorkMail organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Client.update_impersonation_role)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail/client/#update_impersonation_role)
```

### Comparing `mypy-boto3-workmail-1.28.15.post1/mypy_boto3_workmail/client.pyi` & `mypy-boto3-workmail-1.28.16/mypy_boto3_workmail/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_workmail.client import WorkMailClient
 
     session = Session()
     client: WorkMailClient = session.client("workmail")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AccessControlRuleEffectType,
     ImpersonationRoleTypeType,
     MobileDeviceAccessRuleEffectType,
@@ -60,16 +60,15 @@
     GetDefaultRetentionPolicyResponseTypeDef,
     GetImpersonationRoleEffectResponseTypeDef,
     GetImpersonationRoleResponseTypeDef,
     GetMailboxDetailsResponseTypeDef,
     GetMailDomainResponseTypeDef,
     GetMobileDeviceAccessEffectResponseTypeDef,
     GetMobileDeviceAccessOverrideResponseTypeDef,
-    ImpersonationRuleOutputTypeDef,
-    ImpersonationRuleTypeDef,
+    ImpersonationRuleUnionTypeDef,
     LambdaAvailabilityProviderTypeDef,
     ListAccessControlRulesResponseTypeDef,
     ListAliasesResponseTypeDef,
     ListAvailabilityConfigurationsResponseTypeDef,
     ListGroupMembersResponseTypeDef,
     ListGroupsResponseTypeDef,
     ListImpersonationRolesResponseTypeDef,
@@ -226,15 +225,15 @@
         """
     def create_impersonation_role(
         self,
         *,
         OrganizationId: str,
         Name: str,
         Type: ImpersonationRoleTypeType,
-        Rules: Sequence[Union[ImpersonationRuleTypeDef, ImpersonationRuleOutputTypeDef]],
+        Rules: Sequence[ImpersonationRuleUnionTypeDef],
         ClientToken: str = ...,
         Description: str = ...
     ) -> CreateImpersonationRoleResponseTypeDef:
         """
         Creates an impersonation role for the given WorkMail organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Client.create_impersonation_role)
@@ -933,15 +932,15 @@
     def update_impersonation_role(
         self,
         *,
         OrganizationId: str,
         ImpersonationRoleId: str,
         Name: str,
         Type: ImpersonationRoleTypeType,
-        Rules: Sequence[Union[ImpersonationRuleTypeDef, ImpersonationRuleOutputTypeDef]],
+        Rules: Sequence[ImpersonationRuleUnionTypeDef],
         Description: str = ...
     ) -> Dict[str, Any]:
         """
         Updates an impersonation role for the given WorkMail organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Client.update_impersonation_role)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail/client/#update_impersonation_role)
```

### Comparing `mypy-boto3-workmail-1.28.15.post1/mypy_boto3_workmail/literals.py` & `mypy-boto3-workmail-1.28.16/mypy_boto3_workmail/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workmail-1.28.15.post1/mypy_boto3_workmail/literals.pyi` & `mypy-boto3-workmail-1.28.16/mypy_boto3_workmail/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workmail-1.28.15.post1/mypy_boto3_workmail/paginator.py` & `mypy-boto3-workmail-1.28.16/mypy_boto3_workmail/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workmail-1.28.15.post1/mypy_boto3_workmail/paginator.pyi` & `mypy-boto3-workmail-1.28.16/mypy_boto3_workmail/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workmail-1.28.15.post1/mypy_boto3_workmail/type_defs.py` & `mypy-boto3-workmail-1.28.16/mypy_boto3_workmail/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_workmail.type_defs import AccessControlRuleTypeDef
 
-    data: AccessControlRuleTypeDef = {...}
+    data: AccessControlRuleTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -47,16 +47,14 @@
     "LambdaAvailabilityProviderTypeDef",
     "RedactedEwsAvailabilityProviderTypeDef",
     "BookingOptionsTypeDef",
     "CancelMailboxExportJobRequestRequestTypeDef",
     "CreateAliasRequestRequestTypeDef",
     "EwsAvailabilityProviderTypeDef",
     "CreateGroupRequestRequestTypeDef",
-    "ImpersonationRuleOutputTypeDef",
-    "ImpersonationRuleTypeDef",
     "CreateMobileDeviceAccessRuleRequestRequestTypeDef",
     "DomainTypeDef",
     "CreateResourceRequestRequestTypeDef",
     "CreateUserRequestRequestTypeDef",
     "DelegateTypeDef",
     "DeleteAccessControlRuleRequestRequestTypeDef",
     "DeleteAliasRequestRequestTypeDef",
@@ -85,21 +83,23 @@
     "DnsRecordTypeDef",
     "FolderConfigurationTypeDef",
     "GetAccessControlEffectRequestRequestTypeDef",
     "GetDefaultRetentionPolicyRequestRequestTypeDef",
     "GetImpersonationRoleEffectRequestRequestTypeDef",
     "ImpersonationMatchedRuleTypeDef",
     "GetImpersonationRoleRequestRequestTypeDef",
+    "ImpersonationRuleOutputTypeDef",
     "GetMailDomainRequestRequestTypeDef",
     "GetMailboxDetailsRequestRequestTypeDef",
     "GetMobileDeviceAccessEffectRequestRequestTypeDef",
     "MobileDeviceAccessMatchedRuleTypeDef",
     "GetMobileDeviceAccessOverrideRequestRequestTypeDef",
     "GroupTypeDef",
     "ImpersonationRoleTypeDef",
+    "ImpersonationRuleTypeDef",
     "ListAccessControlRulesRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "ListAliasesRequestRequestTypeDef",
     "ListAvailabilityConfigurationsRequestRequestTypeDef",
     "ListGroupMembersRequestRequestTypeDef",
     "MemberTypeDef",
     "ListGroupsRequestRequestTypeDef",
@@ -160,26 +160,25 @@
     "TestAvailabilityConfigurationResponseTypeDef",
     "AvailabilityConfigurationTypeDef",
     "DescribeResourceResponseTypeDef",
     "UpdateResourceRequestRequestTypeDef",
     "CreateAvailabilityConfigurationRequestRequestTypeDef",
     "TestAvailabilityConfigurationRequestRequestTypeDef",
     "UpdateAvailabilityConfigurationRequestRequestTypeDef",
-    "GetImpersonationRoleResponseTypeDef",
-    "CreateImpersonationRoleRequestRequestTypeDef",
-    "UpdateImpersonationRoleRequestRequestTypeDef",
     "CreateOrganizationRequestRequestTypeDef",
     "ListResourceDelegatesResponseTypeDef",
     "GetMailDomainResponseTypeDef",
     "GetDefaultRetentionPolicyResponseTypeDef",
     "PutRetentionPolicyRequestRequestTypeDef",
     "GetImpersonationRoleEffectResponseTypeDef",
+    "GetImpersonationRoleResponseTypeDef",
     "GetMobileDeviceAccessEffectResponseTypeDef",
     "ListGroupsResponseTypeDef",
     "ListImpersonationRolesResponseTypeDef",
+    "ImpersonationRuleUnionTypeDef",
     "ListAliasesRequestListAliasesPaginateTypeDef",
     "ListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef",
     "ListGroupMembersRequestListGroupMembersPaginateTypeDef",
     "ListGroupsRequestListGroupsPaginateTypeDef",
     "ListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef",
     "ListOrganizationsRequestListOrganizationsPaginateTypeDef",
     "ListResourceDelegatesRequestListResourceDelegatesPaginateTypeDef",
@@ -193,14 +192,16 @@
     "ListMobileDeviceAccessRulesResponseTypeDef",
     "ListOrganizationsResponseTypeDef",
     "ListResourcesResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "ListUsersResponseTypeDef",
     "ListAvailabilityConfigurationsResponseTypeDef",
+    "CreateImpersonationRoleRequestRequestTypeDef",
+    "UpdateImpersonationRoleRequestRequestTypeDef",
 )
 
 AccessControlRuleTypeDef = TypedDict(
     "AccessControlRuleTypeDef",
     {
         "Name": str,
         "Effect": AccessControlRuleEffectType,
@@ -313,64 +314,14 @@
     "CreateGroupRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "Name": str,
     },
 )
 
-_RequiredImpersonationRuleOutputTypeDef = TypedDict(
-    "_RequiredImpersonationRuleOutputTypeDef",
-    {
-        "ImpersonationRuleId": str,
-        "Effect": AccessEffectType,
-    },
-)
-_OptionalImpersonationRuleOutputTypeDef = TypedDict(
-    "_OptionalImpersonationRuleOutputTypeDef",
-    {
-        "Name": str,
-        "Description": str,
-        "TargetUsers": List[str],
-        "NotTargetUsers": List[str],
-    },
-    total=False,
-)
-
-
-class ImpersonationRuleOutputTypeDef(
-    _RequiredImpersonationRuleOutputTypeDef, _OptionalImpersonationRuleOutputTypeDef
-):
-    pass
-
-
-_RequiredImpersonationRuleTypeDef = TypedDict(
-    "_RequiredImpersonationRuleTypeDef",
-    {
-        "ImpersonationRuleId": str,
-        "Effect": AccessEffectType,
-    },
-)
-_OptionalImpersonationRuleTypeDef = TypedDict(
-    "_OptionalImpersonationRuleTypeDef",
-    {
-        "Name": str,
-        "Description": str,
-        "TargetUsers": Sequence[str],
-        "NotTargetUsers": Sequence[str],
-    },
-    total=False,
-)
-
-
-class ImpersonationRuleTypeDef(
-    _RequiredImpersonationRuleTypeDef, _OptionalImpersonationRuleTypeDef
-):
-    pass
-
-
 _RequiredCreateMobileDeviceAccessRuleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMobileDeviceAccessRuleRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "Name": str,
         "Effect": MobileDeviceAccessRuleEffectType,
     },
@@ -730,14 +681,39 @@
     "GetImpersonationRoleRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "ImpersonationRoleId": str,
     },
 )
 
+_RequiredImpersonationRuleOutputTypeDef = TypedDict(
+    "_RequiredImpersonationRuleOutputTypeDef",
+    {
+        "ImpersonationRuleId": str,
+        "Effect": AccessEffectType,
+    },
+)
+_OptionalImpersonationRuleOutputTypeDef = TypedDict(
+    "_OptionalImpersonationRuleOutputTypeDef",
+    {
+        "Name": str,
+        "Description": str,
+        "TargetUsers": List[str],
+        "NotTargetUsers": List[str],
+    },
+    total=False,
+)
+
+
+class ImpersonationRuleOutputTypeDef(
+    _RequiredImpersonationRuleOutputTypeDef, _OptionalImpersonationRuleOutputTypeDef
+):
+    pass
+
+
 GetMailDomainRequestRequestTypeDef = TypedDict(
     "GetMailDomainRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "DomainName": str,
     },
 )
@@ -814,14 +790,39 @@
         "Type": ImpersonationRoleTypeType,
         "DateCreated": datetime,
         "DateModified": datetime,
     },
     total=False,
 )
 
+_RequiredImpersonationRuleTypeDef = TypedDict(
+    "_RequiredImpersonationRuleTypeDef",
+    {
+        "ImpersonationRuleId": str,
+        "Effect": AccessEffectType,
+    },
+)
+_OptionalImpersonationRuleTypeDef = TypedDict(
+    "_OptionalImpersonationRuleTypeDef",
+    {
+        "Name": str,
+        "Description": str,
+        "TargetUsers": Sequence[str],
+        "NotTargetUsers": Sequence[str],
+    },
+    total=False,
+)
+
+
+class ImpersonationRuleTypeDef(
+    _RequiredImpersonationRuleTypeDef, _OptionalImpersonationRuleTypeDef
+):
+    pass
+
+
 ListAccessControlRulesRequestRequestTypeDef = TypedDict(
     "ListAccessControlRulesRequestRequestTypeDef",
     {
         "OrganizationId": str,
     },
 )
 
@@ -1815,80 +1816,14 @@
 class UpdateAvailabilityConfigurationRequestRequestTypeDef(
     _RequiredUpdateAvailabilityConfigurationRequestRequestTypeDef,
     _OptionalUpdateAvailabilityConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
-GetImpersonationRoleResponseTypeDef = TypedDict(
-    "GetImpersonationRoleResponseTypeDef",
-    {
-        "ImpersonationRoleId": str,
-        "Name": str,
-        "Type": ImpersonationRoleTypeType,
-        "Description": str,
-        "Rules": List[ImpersonationRuleOutputTypeDef],
-        "DateCreated": datetime,
-        "DateModified": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredCreateImpersonationRoleRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateImpersonationRoleRequestRequestTypeDef",
-    {
-        "OrganizationId": str,
-        "Name": str,
-        "Type": ImpersonationRoleTypeType,
-        "Rules": Sequence[Union[ImpersonationRuleTypeDef, ImpersonationRuleOutputTypeDef]],
-    },
-)
-_OptionalCreateImpersonationRoleRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateImpersonationRoleRequestRequestTypeDef",
-    {
-        "ClientToken": str,
-        "Description": str,
-    },
-    total=False,
-)
-
-
-class CreateImpersonationRoleRequestRequestTypeDef(
-    _RequiredCreateImpersonationRoleRequestRequestTypeDef,
-    _OptionalCreateImpersonationRoleRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredUpdateImpersonationRoleRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateImpersonationRoleRequestRequestTypeDef",
-    {
-        "OrganizationId": str,
-        "ImpersonationRoleId": str,
-        "Name": str,
-        "Type": ImpersonationRoleTypeType,
-        "Rules": Sequence[Union[ImpersonationRuleTypeDef, ImpersonationRuleOutputTypeDef]],
-    },
-)
-_OptionalUpdateImpersonationRoleRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateImpersonationRoleRequestRequestTypeDef",
-    {
-        "Description": str,
-    },
-    total=False,
-)
-
-
-class UpdateImpersonationRoleRequestRequestTypeDef(
-    _RequiredUpdateImpersonationRoleRequestRequestTypeDef,
-    _OptionalUpdateImpersonationRoleRequestRequestTypeDef,
-):
-    pass
-
-
 _RequiredCreateOrganizationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateOrganizationRequestRequestTypeDef",
     {
         "Alias": str,
     },
 )
 _OptionalCreateOrganizationRequestRequestTypeDef = TypedDict(
@@ -1974,14 +1909,28 @@
         "Type": ImpersonationRoleTypeType,
         "Effect": AccessEffectType,
         "MatchedRules": List[ImpersonationMatchedRuleTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+GetImpersonationRoleResponseTypeDef = TypedDict(
+    "GetImpersonationRoleResponseTypeDef",
+    {
+        "ImpersonationRoleId": str,
+        "Name": str,
+        "Type": ImpersonationRoleTypeType,
+        "Description": str,
+        "Rules": List[ImpersonationRuleOutputTypeDef],
+        "DateCreated": datetime,
+        "DateModified": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetMobileDeviceAccessEffectResponseTypeDef = TypedDict(
     "GetMobileDeviceAccessEffectResponseTypeDef",
     {
         "Effect": MobileDeviceAccessRuleEffectType,
         "MatchedRules": List[MobileDeviceAccessMatchedRuleTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2001,14 +1950,15 @@
     {
         "Roles": List[ImpersonationRoleTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ImpersonationRuleUnionTypeDef = Union[ImpersonationRuleTypeDef, ImpersonationRuleOutputTypeDef]
 _RequiredListAliasesRequestListAliasesPaginateTypeDef = TypedDict(
     "_RequiredListAliasesRequestListAliasesPaginateTypeDef",
     {
         "OrganizationId": str,
         "EntityId": str,
     },
 )
@@ -2293,7 +2243,58 @@
     "ListAvailabilityConfigurationsResponseTypeDef",
     {
         "AvailabilityConfigurations": List[AvailabilityConfigurationTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+
+_RequiredCreateImpersonationRoleRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateImpersonationRoleRequestRequestTypeDef",
+    {
+        "OrganizationId": str,
+        "Name": str,
+        "Type": ImpersonationRoleTypeType,
+        "Rules": Sequence[ImpersonationRuleUnionTypeDef],
+    },
+)
+_OptionalCreateImpersonationRoleRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateImpersonationRoleRequestRequestTypeDef",
+    {
+        "ClientToken": str,
+        "Description": str,
+    },
+    total=False,
+)
+
+
+class CreateImpersonationRoleRequestRequestTypeDef(
+    _RequiredCreateImpersonationRoleRequestRequestTypeDef,
+    _OptionalCreateImpersonationRoleRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredUpdateImpersonationRoleRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateImpersonationRoleRequestRequestTypeDef",
+    {
+        "OrganizationId": str,
+        "ImpersonationRoleId": str,
+        "Name": str,
+        "Type": ImpersonationRoleTypeType,
+        "Rules": Sequence[ImpersonationRuleUnionTypeDef],
+    },
+)
+_OptionalUpdateImpersonationRoleRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateImpersonationRoleRequestRequestTypeDef",
+    {
+        "Description": str,
+    },
+    total=False,
+)
+
+
+class UpdateImpersonationRoleRequestRequestTypeDef(
+    _RequiredUpdateImpersonationRoleRequestRequestTypeDef,
+    _OptionalUpdateImpersonationRoleRequestRequestTypeDef,
+):
+    pass
```

### Comparing `mypy-boto3-workmail-1.28.15.post1/mypy_boto3_workmail/type_defs.pyi` & `mypy-boto3-workmail-1.28.16/mypy_boto3_workmail/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_workmail.type_defs import AccessControlRuleTypeDef
 
-    data: AccessControlRuleTypeDef = {...}
+    data: AccessControlRuleTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -46,16 +46,14 @@
     "LambdaAvailabilityProviderTypeDef",
     "RedactedEwsAvailabilityProviderTypeDef",
     "BookingOptionsTypeDef",
     "CancelMailboxExportJobRequestRequestTypeDef",
     "CreateAliasRequestRequestTypeDef",
     "EwsAvailabilityProviderTypeDef",
     "CreateGroupRequestRequestTypeDef",
-    "ImpersonationRuleOutputTypeDef",
-    "ImpersonationRuleTypeDef",
     "CreateMobileDeviceAccessRuleRequestRequestTypeDef",
     "DomainTypeDef",
     "CreateResourceRequestRequestTypeDef",
     "CreateUserRequestRequestTypeDef",
     "DelegateTypeDef",
     "DeleteAccessControlRuleRequestRequestTypeDef",
     "DeleteAliasRequestRequestTypeDef",
@@ -84,21 +82,23 @@
     "DnsRecordTypeDef",
     "FolderConfigurationTypeDef",
     "GetAccessControlEffectRequestRequestTypeDef",
     "GetDefaultRetentionPolicyRequestRequestTypeDef",
     "GetImpersonationRoleEffectRequestRequestTypeDef",
     "ImpersonationMatchedRuleTypeDef",
     "GetImpersonationRoleRequestRequestTypeDef",
+    "ImpersonationRuleOutputTypeDef",
     "GetMailDomainRequestRequestTypeDef",
     "GetMailboxDetailsRequestRequestTypeDef",
     "GetMobileDeviceAccessEffectRequestRequestTypeDef",
     "MobileDeviceAccessMatchedRuleTypeDef",
     "GetMobileDeviceAccessOverrideRequestRequestTypeDef",
     "GroupTypeDef",
     "ImpersonationRoleTypeDef",
+    "ImpersonationRuleTypeDef",
     "ListAccessControlRulesRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "ListAliasesRequestRequestTypeDef",
     "ListAvailabilityConfigurationsRequestRequestTypeDef",
     "ListGroupMembersRequestRequestTypeDef",
     "MemberTypeDef",
     "ListGroupsRequestRequestTypeDef",
@@ -159,26 +159,25 @@
     "TestAvailabilityConfigurationResponseTypeDef",
     "AvailabilityConfigurationTypeDef",
     "DescribeResourceResponseTypeDef",
     "UpdateResourceRequestRequestTypeDef",
     "CreateAvailabilityConfigurationRequestRequestTypeDef",
     "TestAvailabilityConfigurationRequestRequestTypeDef",
     "UpdateAvailabilityConfigurationRequestRequestTypeDef",
-    "GetImpersonationRoleResponseTypeDef",
-    "CreateImpersonationRoleRequestRequestTypeDef",
-    "UpdateImpersonationRoleRequestRequestTypeDef",
     "CreateOrganizationRequestRequestTypeDef",
     "ListResourceDelegatesResponseTypeDef",
     "GetMailDomainResponseTypeDef",
     "GetDefaultRetentionPolicyResponseTypeDef",
     "PutRetentionPolicyRequestRequestTypeDef",
     "GetImpersonationRoleEffectResponseTypeDef",
+    "GetImpersonationRoleResponseTypeDef",
     "GetMobileDeviceAccessEffectResponseTypeDef",
     "ListGroupsResponseTypeDef",
     "ListImpersonationRolesResponseTypeDef",
+    "ImpersonationRuleUnionTypeDef",
     "ListAliasesRequestListAliasesPaginateTypeDef",
     "ListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef",
     "ListGroupMembersRequestListGroupMembersPaginateTypeDef",
     "ListGroupsRequestListGroupsPaginateTypeDef",
     "ListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef",
     "ListOrganizationsRequestListOrganizationsPaginateTypeDef",
     "ListResourceDelegatesRequestListResourceDelegatesPaginateTypeDef",
@@ -192,14 +191,16 @@
     "ListMobileDeviceAccessRulesResponseTypeDef",
     "ListOrganizationsResponseTypeDef",
     "ListResourcesResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "ListUsersResponseTypeDef",
     "ListAvailabilityConfigurationsResponseTypeDef",
+    "CreateImpersonationRoleRequestRequestTypeDef",
+    "UpdateImpersonationRoleRequestRequestTypeDef",
 )
 
 AccessControlRuleTypeDef = TypedDict(
     "AccessControlRuleTypeDef",
     {
         "Name": str,
         "Effect": AccessControlRuleEffectType,
@@ -312,60 +313,14 @@
     "CreateGroupRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "Name": str,
     },
 )
 
-_RequiredImpersonationRuleOutputTypeDef = TypedDict(
-    "_RequiredImpersonationRuleOutputTypeDef",
-    {
-        "ImpersonationRuleId": str,
-        "Effect": AccessEffectType,
-    },
-)
-_OptionalImpersonationRuleOutputTypeDef = TypedDict(
-    "_OptionalImpersonationRuleOutputTypeDef",
-    {
-        "Name": str,
-        "Description": str,
-        "TargetUsers": List[str],
-        "NotTargetUsers": List[str],
-    },
-    total=False,
-)
-
-class ImpersonationRuleOutputTypeDef(
-    _RequiredImpersonationRuleOutputTypeDef, _OptionalImpersonationRuleOutputTypeDef
-):
-    pass
-
-_RequiredImpersonationRuleTypeDef = TypedDict(
-    "_RequiredImpersonationRuleTypeDef",
-    {
-        "ImpersonationRuleId": str,
-        "Effect": AccessEffectType,
-    },
-)
-_OptionalImpersonationRuleTypeDef = TypedDict(
-    "_OptionalImpersonationRuleTypeDef",
-    {
-        "Name": str,
-        "Description": str,
-        "TargetUsers": Sequence[str],
-        "NotTargetUsers": Sequence[str],
-    },
-    total=False,
-)
-
-class ImpersonationRuleTypeDef(
-    _RequiredImpersonationRuleTypeDef, _OptionalImpersonationRuleTypeDef
-):
-    pass
-
 _RequiredCreateMobileDeviceAccessRuleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMobileDeviceAccessRuleRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "Name": str,
         "Effect": MobileDeviceAccessRuleEffectType,
     },
@@ -717,14 +672,37 @@
     "GetImpersonationRoleRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "ImpersonationRoleId": str,
     },
 )
 
+_RequiredImpersonationRuleOutputTypeDef = TypedDict(
+    "_RequiredImpersonationRuleOutputTypeDef",
+    {
+        "ImpersonationRuleId": str,
+        "Effect": AccessEffectType,
+    },
+)
+_OptionalImpersonationRuleOutputTypeDef = TypedDict(
+    "_OptionalImpersonationRuleOutputTypeDef",
+    {
+        "Name": str,
+        "Description": str,
+        "TargetUsers": List[str],
+        "NotTargetUsers": List[str],
+    },
+    total=False,
+)
+
+class ImpersonationRuleOutputTypeDef(
+    _RequiredImpersonationRuleOutputTypeDef, _OptionalImpersonationRuleOutputTypeDef
+):
+    pass
+
 GetMailDomainRequestRequestTypeDef = TypedDict(
     "GetMailDomainRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "DomainName": str,
     },
 )
@@ -799,14 +777,37 @@
         "Type": ImpersonationRoleTypeType,
         "DateCreated": datetime,
         "DateModified": datetime,
     },
     total=False,
 )
 
+_RequiredImpersonationRuleTypeDef = TypedDict(
+    "_RequiredImpersonationRuleTypeDef",
+    {
+        "ImpersonationRuleId": str,
+        "Effect": AccessEffectType,
+    },
+)
+_OptionalImpersonationRuleTypeDef = TypedDict(
+    "_OptionalImpersonationRuleTypeDef",
+    {
+        "Name": str,
+        "Description": str,
+        "TargetUsers": Sequence[str],
+        "NotTargetUsers": Sequence[str],
+    },
+    total=False,
+)
+
+class ImpersonationRuleTypeDef(
+    _RequiredImpersonationRuleTypeDef, _OptionalImpersonationRuleTypeDef
+):
+    pass
+
 ListAccessControlRulesRequestRequestTypeDef = TypedDict(
     "ListAccessControlRulesRequestRequestTypeDef",
     {
         "OrganizationId": str,
     },
 )
 
@@ -1758,76 +1759,14 @@
 
 class UpdateAvailabilityConfigurationRequestRequestTypeDef(
     _RequiredUpdateAvailabilityConfigurationRequestRequestTypeDef,
     _OptionalUpdateAvailabilityConfigurationRequestRequestTypeDef,
 ):
     pass
 
-GetImpersonationRoleResponseTypeDef = TypedDict(
-    "GetImpersonationRoleResponseTypeDef",
-    {
-        "ImpersonationRoleId": str,
-        "Name": str,
-        "Type": ImpersonationRoleTypeType,
-        "Description": str,
-        "Rules": List[ImpersonationRuleOutputTypeDef],
-        "DateCreated": datetime,
-        "DateModified": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredCreateImpersonationRoleRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateImpersonationRoleRequestRequestTypeDef",
-    {
-        "OrganizationId": str,
-        "Name": str,
-        "Type": ImpersonationRoleTypeType,
-        "Rules": Sequence[Union[ImpersonationRuleTypeDef, ImpersonationRuleOutputTypeDef]],
-    },
-)
-_OptionalCreateImpersonationRoleRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateImpersonationRoleRequestRequestTypeDef",
-    {
-        "ClientToken": str,
-        "Description": str,
-    },
-    total=False,
-)
-
-class CreateImpersonationRoleRequestRequestTypeDef(
-    _RequiredCreateImpersonationRoleRequestRequestTypeDef,
-    _OptionalCreateImpersonationRoleRequestRequestTypeDef,
-):
-    pass
-
-_RequiredUpdateImpersonationRoleRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateImpersonationRoleRequestRequestTypeDef",
-    {
-        "OrganizationId": str,
-        "ImpersonationRoleId": str,
-        "Name": str,
-        "Type": ImpersonationRoleTypeType,
-        "Rules": Sequence[Union[ImpersonationRuleTypeDef, ImpersonationRuleOutputTypeDef]],
-    },
-)
-_OptionalUpdateImpersonationRoleRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateImpersonationRoleRequestRequestTypeDef",
-    {
-        "Description": str,
-    },
-    total=False,
-)
-
-class UpdateImpersonationRoleRequestRequestTypeDef(
-    _RequiredUpdateImpersonationRoleRequestRequestTypeDef,
-    _OptionalUpdateImpersonationRoleRequestRequestTypeDef,
-):
-    pass
-
 _RequiredCreateOrganizationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateOrganizationRequestRequestTypeDef",
     {
         "Alias": str,
     },
 )
 _OptionalCreateOrganizationRequestRequestTypeDef = TypedDict(
@@ -1909,14 +1848,28 @@
         "Type": ImpersonationRoleTypeType,
         "Effect": AccessEffectType,
         "MatchedRules": List[ImpersonationMatchedRuleTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+GetImpersonationRoleResponseTypeDef = TypedDict(
+    "GetImpersonationRoleResponseTypeDef",
+    {
+        "ImpersonationRoleId": str,
+        "Name": str,
+        "Type": ImpersonationRoleTypeType,
+        "Description": str,
+        "Rules": List[ImpersonationRuleOutputTypeDef],
+        "DateCreated": datetime,
+        "DateModified": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetMobileDeviceAccessEffectResponseTypeDef = TypedDict(
     "GetMobileDeviceAccessEffectResponseTypeDef",
     {
         "Effect": MobileDeviceAccessRuleEffectType,
         "MatchedRules": List[MobileDeviceAccessMatchedRuleTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1936,14 +1889,15 @@
     {
         "Roles": List[ImpersonationRoleTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ImpersonationRuleUnionTypeDef = Union[ImpersonationRuleTypeDef, ImpersonationRuleOutputTypeDef]
 _RequiredListAliasesRequestListAliasesPaginateTypeDef = TypedDict(
     "_RequiredListAliasesRequestListAliasesPaginateTypeDef",
     {
         "OrganizationId": str,
         "EntityId": str,
     },
 )
@@ -2212,7 +2166,55 @@
     "ListAvailabilityConfigurationsResponseTypeDef",
     {
         "AvailabilityConfigurations": List[AvailabilityConfigurationTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+
+_RequiredCreateImpersonationRoleRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateImpersonationRoleRequestRequestTypeDef",
+    {
+        "OrganizationId": str,
+        "Name": str,
+        "Type": ImpersonationRoleTypeType,
+        "Rules": Sequence[ImpersonationRuleUnionTypeDef],
+    },
+)
+_OptionalCreateImpersonationRoleRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateImpersonationRoleRequestRequestTypeDef",
+    {
+        "ClientToken": str,
+        "Description": str,
+    },
+    total=False,
+)
+
+class CreateImpersonationRoleRequestRequestTypeDef(
+    _RequiredCreateImpersonationRoleRequestRequestTypeDef,
+    _OptionalCreateImpersonationRoleRequestRequestTypeDef,
+):
+    pass
+
+_RequiredUpdateImpersonationRoleRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateImpersonationRoleRequestRequestTypeDef",
+    {
+        "OrganizationId": str,
+        "ImpersonationRoleId": str,
+        "Name": str,
+        "Type": ImpersonationRoleTypeType,
+        "Rules": Sequence[ImpersonationRuleUnionTypeDef],
+    },
+)
+_OptionalUpdateImpersonationRoleRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateImpersonationRoleRequestRequestTypeDef",
+    {
+        "Description": str,
+    },
+    total=False,
+)
+
+class UpdateImpersonationRoleRequestRequestTypeDef(
+    _RequiredUpdateImpersonationRoleRequestRequestTypeDef,
+    _OptionalUpdateImpersonationRoleRequestRequestTypeDef,
+):
+    pass
```

### Comparing `mypy-boto3-workmail-1.28.15.post1/mypy_boto3_workmail.egg-info/PKG-INFO` & `mypy-boto3-workmail-1.28.16/mypy_boto3_workmail.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-workmail
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.WorkMail 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.WorkMail 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 workmail type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 workmail type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-workmail.svg?color=blue)](https://pypi.org/project/mypy-boto3-workmail)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-workmail)](https://pepy.tech/project/mypy-boto3-workmail)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WorkMail 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail)
+[boto3.WorkMail 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail)
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
 [mypy-boto3-workmail docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail/).
 
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
@@ -357,20 +357,20 @@
 )
 
 
 def check_value(value: AccessControlRuleEffectType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_workmail.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_workmail.type_defs import (
     AccessControlRuleTypeDef,
     AssociateDelegateToResourceRequestRequestTypeDef,
     AssociateMemberToGroupRequestRequestTypeDef,
     AssumeImpersonationRoleRequestRequestTypeDef,
@@ -378,16 +378,14 @@
     LambdaAvailabilityProviderTypeDef,
     RedactedEwsAvailabilityProviderTypeDef,
     BookingOptionsTypeDef,
     CancelMailboxExportJobRequestRequestTypeDef,
     CreateAliasRequestRequestTypeDef,
     EwsAvailabilityProviderTypeDef,
     CreateGroupRequestRequestTypeDef,
-    ImpersonationRuleOutputTypeDef,
-    ImpersonationRuleTypeDef,
     CreateMobileDeviceAccessRuleRequestRequestTypeDef,
     DomainTypeDef,
     CreateResourceRequestRequestTypeDef,
     CreateUserRequestRequestTypeDef,
     DelegateTypeDef,
     DeleteAccessControlRuleRequestRequestTypeDef,
     DeleteAliasRequestRequestTypeDef,
@@ -416,21 +414,23 @@
     DnsRecordTypeDef,
     FolderConfigurationTypeDef,
     GetAccessControlEffectRequestRequestTypeDef,
     GetDefaultRetentionPolicyRequestRequestTypeDef,
     GetImpersonationRoleEffectRequestRequestTypeDef,
     ImpersonationMatchedRuleTypeDef,
     GetImpersonationRoleRequestRequestTypeDef,
+    ImpersonationRuleOutputTypeDef,
     GetMailDomainRequestRequestTypeDef,
     GetMailboxDetailsRequestRequestTypeDef,
     GetMobileDeviceAccessEffectRequestRequestTypeDef,
     MobileDeviceAccessMatchedRuleTypeDef,
     GetMobileDeviceAccessOverrideRequestRequestTypeDef,
     GroupTypeDef,
     ImpersonationRoleTypeDef,
+    ImpersonationRuleTypeDef,
     ListAccessControlRulesRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     ListAliasesRequestRequestTypeDef,
     ListAvailabilityConfigurationsRequestRequestTypeDef,
     ListGroupMembersRequestRequestTypeDef,
     MemberTypeDef,
     ListGroupsRequestRequestTypeDef,
@@ -491,26 +491,25 @@
     TestAvailabilityConfigurationResponseTypeDef,
     AvailabilityConfigurationTypeDef,
     DescribeResourceResponseTypeDef,
     UpdateResourceRequestRequestTypeDef,
     CreateAvailabilityConfigurationRequestRequestTypeDef,
     TestAvailabilityConfigurationRequestRequestTypeDef,
     UpdateAvailabilityConfigurationRequestRequestTypeDef,
-    GetImpersonationRoleResponseTypeDef,
-    CreateImpersonationRoleRequestRequestTypeDef,
-    UpdateImpersonationRoleRequestRequestTypeDef,
     CreateOrganizationRequestRequestTypeDef,
     ListResourceDelegatesResponseTypeDef,
     GetMailDomainResponseTypeDef,
     GetDefaultRetentionPolicyResponseTypeDef,
     PutRetentionPolicyRequestRequestTypeDef,
     GetImpersonationRoleEffectResponseTypeDef,
+    GetImpersonationRoleResponseTypeDef,
     GetMobileDeviceAccessEffectResponseTypeDef,
     ListGroupsResponseTypeDef,
     ListImpersonationRolesResponseTypeDef,
+    ImpersonationRuleUnionTypeDef,
     ListAliasesRequestListAliasesPaginateTypeDef,
     ListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef,
     ListGroupMembersRequestListGroupMembersPaginateTypeDef,
     ListGroupsRequestListGroupsPaginateTypeDef,
     ListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef,
     ListOrganizationsRequestListOrganizationsPaginateTypeDef,
     ListResourceDelegatesRequestListResourceDelegatesPaginateTypeDef,
@@ -524,18 +523,20 @@
     ListMobileDeviceAccessRulesResponseTypeDef,
     ListOrganizationsResponseTypeDef,
     ListResourcesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     ListUsersResponseTypeDef,
     ListAvailabilityConfigurationsResponseTypeDef,
+    CreateImpersonationRoleRequestRequestTypeDef,
+    UpdateImpersonationRoleRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AccessControlRuleTypeDef:
+def get_value() -> AccessControlRuleTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-workmail-1.28.15.post1/mypy_boto3_workmail.egg-info/SOURCES.txt` & `mypy-boto3-workmail-1.28.16/mypy_boto3_workmail.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workmail-1.28.15.post1/setup.py` & `mypy-boto3-workmail-1.28.16/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-workmail",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_workmail"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.WorkMail 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.WorkMail 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 workmail type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 workmail type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_workmail": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

