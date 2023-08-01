# Comparing `tmp/mypy-boto3-fms-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-fms-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-fms-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:09 2023, max compression
+gzip compressed data, was "mypy-boto3-fms-1.28.16.tar", last modified: Tue Aug  1 11:36:49 2023, max compression
```

## Comparing `mypy-boto3-fms-1.28.15.post1.tar` & `mypy-boto3-fms-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:09.605155 mypy-boto3-fms-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:45:29.000000 mypy-boto3-fms-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21126 2023-07-29 10:03:09.605155 mypy-boto3-fms-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19649 2023-07-29 09:45:29.000000 mypy-boto3-fms-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:09.593155 mypy-boto3-fms-1.28.15.post1/mypy_boto3_fms/
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-07-29 09:45:29.000000 mypy-boto3-fms-1.28.15.post1/mypy_boto3_fms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-29 09:45:29.000000 mypy-boto3-fms-1.28.15.post1/mypy_boto3_fms/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-29 09:45:29.000000 mypy-boto3-fms-1.28.15.post1/mypy_boto3_fms/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31257 2023-07-29 09:45:30.000000 mypy-boto3-fms-1.28.15.post1/mypy_boto3_fms/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    31200 2023-07-29 09:45:30.000000 mypy-boto3-fms-1.28.15.post1/mypy_boto3_fms/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13074 2023-07-29 09:45:30.000000 mypy-boto3-fms-1.28.15.post1/mypy_boto3_fms/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13072 2023-07-29 09:45:30.000000 mypy-boto3-fms-1.28.15.post1/mypy_boto3_fms/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9678 2023-07-29 09:45:30.000000 mypy-boto3-fms-1.28.15.post1/mypy_boto3_fms/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9668 2023-07-29 09:45:30.000000 mypy-boto3-fms-1.28.15.post1/mypy_boto3_fms/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:45:29.000000 mypy-boto3-fms-1.28.15.post1/mypy_boto3_fms/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    63794 2023-07-29 09:45:32.000000 mypy-boto3-fms-1.28.15.post1/mypy_boto3_fms/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    63719 2023-07-29 09:45:31.000000 mypy-boto3-fms-1.28.15.post1/mypy_boto3_fms/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:45:29.000000 mypy-boto3-fms-1.28.15.post1/mypy_boto3_fms/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:09.605155 mypy-boto3-fms-1.28.15.post1/mypy_boto3_fms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21126 2023-07-29 10:03:09.000000 mypy-boto3-fms-1.28.15.post1/mypy_boto3_fms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-29 10:03:09.000000 mypy-boto3-fms-1.28.15.post1/mypy_boto3_fms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:09.000000 mypy-boto3-fms-1.28.15.post1/mypy_boto3_fms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:09.000000 mypy-boto3-fms-1.28.15.post1/mypy_boto3_fms.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:09.000000 mypy-boto3-fms-1.28.15.post1/mypy_boto3_fms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-29 10:03:09.000000 mypy-boto3-fms-1.28.15.post1/mypy_boto3_fms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:09.605155 mypy-boto3-fms-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-29 09:45:29.000000 mypy-boto3-fms-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:49.208888 mypy-boto3-fms-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:18:06.000000 mypy-boto3-fms-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21284 2023-08-01 11:36:49.208888 mypy-boto3-fms-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19816 2023-08-01 11:18:06.000000 mypy-boto3-fms-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:49.208888 mypy-boto3-fms-1.28.16/mypy_boto3_fms/
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-08-01 11:18:06.000000 mypy-boto3-fms-1.28.16/mypy_boto3_fms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-08-01 11:18:06.000000 mypy-boto3-fms-1.28.16/mypy_boto3_fms/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-08-01 11:18:06.000000 mypy-boto3-fms-1.28.16/mypy_boto3_fms/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30847 2023-08-01 11:18:06.000000 mypy-boto3-fms-1.28.16/mypy_boto3_fms/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30790 2023-08-01 11:18:06.000000 mypy-boto3-fms-1.28.16/mypy_boto3_fms/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13074 2023-08-01 11:18:07.000000 mypy-boto3-fms-1.28.16/mypy_boto3_fms/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13072 2023-08-01 11:18:07.000000 mypy-boto3-fms-1.28.16/mypy_boto3_fms/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9678 2023-08-01 11:18:06.000000 mypy-boto3-fms-1.28.16/mypy_boto3_fms/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9668 2023-08-01 11:18:06.000000 mypy-boto3-fms-1.28.16/mypy_boto3_fms/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:18:06.000000 mypy-boto3-fms-1.28.16/mypy_boto3_fms/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    64377 2023-08-01 11:18:10.000000 mypy-boto3-fms-1.28.16/mypy_boto3_fms/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64302 2023-08-01 11:18:08.000000 mypy-boto3-fms-1.28.16/mypy_boto3_fms/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:18:06.000000 mypy-boto3-fms-1.28.16/mypy_boto3_fms/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:49.208888 mypy-boto3-fms-1.28.16/mypy_boto3_fms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21284 2023-08-01 11:36:48.000000 mypy-boto3-fms-1.28.16/mypy_boto3_fms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-08-01 11:36:48.000000 mypy-boto3-fms-1.28.16/mypy_boto3_fms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:48.000000 mypy-boto3-fms-1.28.16/mypy_boto3_fms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:48.000000 mypy-boto3-fms-1.28.16/mypy_boto3_fms.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:48.000000 mypy-boto3-fms-1.28.16/mypy_boto3_fms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-01 11:36:48.000000 mypy-boto3-fms-1.28.16/mypy_boto3_fms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:49.208888 mypy-boto3-fms-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-08-01 11:18:06.000000 mypy-boto3-fms-1.28.16/setup.py
```

### Comparing `mypy-boto3-fms-1.28.15.post1/LICENSE` & `mypy-boto3-fms-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fms-1.28.15.post1/PKG-INFO` & `mypy-boto3-fms-1.28.16/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-fms
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.FMS 1.28.15 service generated with mypy-boto3-builder 7.16.2
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 fms type-annotations boto3-stubs mypy typeshed autocomplete
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a id="mypy-boto3-fms"></a>
 
 # mypy-boto3-fms
 
 [![PyPI - mypy-boto3-fms](https://img.shields.io/pypi/v/mypy-boto3-fms.svg?color=blue)](https://pypi.org/project/mypy-boto3-fms)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-fms.svg?color=blue)](https://pypi.org/project/mypy-boto3-fms)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-fms)](https://pepy.tech/project/mypy-boto3-fms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.FMS 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS)
+[boto3.FMS 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS)
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
 [mypy-boto3-fms docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/).
 
 See how it helps to find and fix potential bugs:
 
@@ -74,15 +42,15 @@
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
@@ -362,34 +330,35 @@
 )
 
 
 def check_value(value: AccountRoleStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_fms.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_fms.type_defs import (
     AccountScopeOutputTypeDef,
     AccountScopeTypeDef,
     ActionTargetTypeDef,
     AdminAccountSummaryTypeDef,
     OrganizationalUnitScopeOutputTypeDef,
     PolicyTypeScopeOutputTypeDef,
     RegionScopeOutputTypeDef,
     OrganizationalUnitScopeTypeDef,
     PolicyTypeScopeTypeDef,
     RegionScopeTypeDef,
     AppTypeDef,
+    TimestampTypeDef,
     AssociateAdminAccountRequestRequestTypeDef,
     AssociateThirdPartyFirewallRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     AwsEc2NetworkInterfaceViolationTypeDef,
     PartialMatchTypeDef,
     BatchAssociateResourceRequestRequestTypeDef,
     FailedItemTypeDef,
@@ -409,15 +378,14 @@
     FMSPolicyUpdateFirewallCreationConfigActionTypeDef,
     FirewallSubnetIsOutOfScopeViolationTypeDef,
     FirewallSubnetMissingVPCEndpointViolationTypeDef,
     GetAdminScopeRequestRequestTypeDef,
     GetAppsListRequestRequestTypeDef,
     GetComplianceDetailRequestRequestTypeDef,
     GetPolicyRequestRequestTypeDef,
-    GetProtectionStatusRequestRequestTypeDef,
     GetProtocolsListRequestRequestTypeDef,
     ProtocolsListDataOutputTypeDef,
     GetResourceSetRequestRequestTypeDef,
     ResourceSetOutputTypeDef,
     GetThirdPartyFirewallAssociationStatusRequestRequestTypeDef,
     GetViolationDetailsRequestRequestTypeDef,
     PaginatorConfigTypeDef,
@@ -445,17 +413,15 @@
     NetworkFirewallMissingSubnetViolationTypeDef,
     StatefulEngineOptionsTypeDef,
     StatelessRuleGroupTypeDef,
     NetworkFirewallPolicyTypeDef,
     NetworkFirewallStatefulRuleGroupOverrideTypeDef,
     ThirdPartyFirewallPolicyTypeDef,
     ResourceTagTypeDef,
-    ProtocolsListDataTypeDef,
     PutNotificationChannelRequestRequestTypeDef,
-    ResourceSetTypeDef,
     ThirdPartyFirewallMissingExpectedRouteTableViolationTypeDef,
     ThirdPartyFirewallMissingFirewallViolationTypeDef,
     ThirdPartyFirewallMissingSubnetViolationTypeDef,
     SecurityGroupRuleDescriptionTypeDef,
     UntagResourceRequestRequestTypeDef,
     EC2AssociateRouteTableActionTypeDef,
     EC2CopyRouteTableActionTypeDef,
@@ -465,14 +431,17 @@
     EC2ReplaceRouteActionTypeDef,
     EC2ReplaceRouteTableAssociationActionTypeDef,
     AdminScopeOutputTypeDef,
     AdminScopeTypeDef,
     AppsListDataOutputTypeDef,
     AppsListDataSummaryTypeDef,
     AppsListDataTypeDef,
+    GetProtectionStatusRequestRequestTypeDef,
+    ProtocolsListDataTypeDef,
+    ResourceSetTypeDef,
     AssociateThirdPartyFirewallResponseTypeDef,
     DisassociateThirdPartyFirewallResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetAdminAccountResponseTypeDef,
     GetNotificationChannelResponseTypeDef,
     GetProtectionStatusResponseTypeDef,
     GetThirdPartyFirewallAssociationStatusResponseTypeDef,
@@ -509,45 +478,50 @@
     NetworkFirewallInternetTrafficNotInspectedViolationTypeDef,
     NetworkFirewallInvalidRouteConfigurationViolationTypeDef,
     NetworkFirewallUnexpectedFirewallRoutesViolationTypeDef,
     NetworkFirewallUnexpectedGatewayRoutesViolationTypeDef,
     RouteHasOutOfScopeEndpointViolationTypeDef,
     StatefulRuleGroupTypeDef,
     PolicyOptionTypeDef,
-    PutProtocolsListRequestRequestTypeDef,
-    PutResourceSetRequestRequestTypeDef,
     SecurityGroupRemediationActionTypeDef,
     RemediationActionTypeDef,
     GetAdminScopeResponseTypeDef,
+    AdminScopeUnionTypeDef,
     PutAdminAccountRequestRequestTypeDef,
     GetAppsListResponseTypeDef,
     PutAppsListResponseTypeDef,
     ListAppsListsResponseTypeDef,
+    AppsListDataUnionTypeDef,
     PutAppsListRequestRequestTypeDef,
+    ProtocolsListDataUnionTypeDef,
+    PutProtocolsListRequestRequestTypeDef,
+    PutResourceSetRequestRequestTypeDef,
+    ResourceSetUnionTypeDef,
     GetComplianceDetailResponseTypeDef,
     ListComplianceStatusResponseTypeDef,
     NetworkFirewallPolicyDescriptionTypeDef,
     SecurityServicePolicyDataTypeDef,
     AwsVPCSecurityGroupViolationTypeDef,
     RemediationActionWithOrderTypeDef,
     NetworkFirewallPolicyModifiedViolationTypeDef,
     PolicyOutputTypeDef,
     PolicyTypeDef,
     PossibleRemediationActionTypeDef,
     GetPolicyResponseTypeDef,
     PutPolicyResponseTypeDef,
+    PolicyUnionTypeDef,
     PutPolicyRequestRequestTypeDef,
     PossibleRemediationActionsTypeDef,
     ResourceViolationTypeDef,
     ViolationDetailTypeDef,
     GetViolationDetailsResponseTypeDef,
 )
 
 
-def get_structure() -> AccountScopeOutputTypeDef:
+def get_value() -> AccountScopeOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-fms-1.28.15.post1/README.md` & `mypy-boto3-fms-1.28.16/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-fms
+Version: 1.28.16
+Summary: Type annotations for boto3.FMS 1.28.16 service generated with mypy-boto3-builder 7.17.1
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 fms type-annotations botocore mypy typeshed autocomplete
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <a id="mypy-boto3-fms"></a>
 
 # mypy-boto3-fms
 
 [![PyPI - mypy-boto3-fms](https://img.shields.io/pypi/v/mypy-boto3-fms.svg?color=blue)](https://pypi.org/project/mypy-boto3-fms)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-fms.svg?color=blue)](https://pypi.org/project/mypy-boto3-fms)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-fms)](https://pepy.tech/project/mypy-boto3-fms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.FMS 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS)
+[boto3.FMS 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS)
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
 [mypy-boto3-fms docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/).
 
 See how it helps to find and fix potential bugs:
 
@@ -42,15 +74,15 @@
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
@@ -330,34 +362,35 @@
 )
 
 
 def check_value(value: AccountRoleStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_fms.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_fms.type_defs import (
     AccountScopeOutputTypeDef,
     AccountScopeTypeDef,
     ActionTargetTypeDef,
     AdminAccountSummaryTypeDef,
     OrganizationalUnitScopeOutputTypeDef,
     PolicyTypeScopeOutputTypeDef,
     RegionScopeOutputTypeDef,
     OrganizationalUnitScopeTypeDef,
     PolicyTypeScopeTypeDef,
     RegionScopeTypeDef,
     AppTypeDef,
+    TimestampTypeDef,
     AssociateAdminAccountRequestRequestTypeDef,
     AssociateThirdPartyFirewallRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     AwsEc2NetworkInterfaceViolationTypeDef,
     PartialMatchTypeDef,
     BatchAssociateResourceRequestRequestTypeDef,
     FailedItemTypeDef,
@@ -377,15 +410,14 @@
     FMSPolicyUpdateFirewallCreationConfigActionTypeDef,
     FirewallSubnetIsOutOfScopeViolationTypeDef,
     FirewallSubnetMissingVPCEndpointViolationTypeDef,
     GetAdminScopeRequestRequestTypeDef,
     GetAppsListRequestRequestTypeDef,
     GetComplianceDetailRequestRequestTypeDef,
     GetPolicyRequestRequestTypeDef,
-    GetProtectionStatusRequestRequestTypeDef,
     GetProtocolsListRequestRequestTypeDef,
     ProtocolsListDataOutputTypeDef,
     GetResourceSetRequestRequestTypeDef,
     ResourceSetOutputTypeDef,
     GetThirdPartyFirewallAssociationStatusRequestRequestTypeDef,
     GetViolationDetailsRequestRequestTypeDef,
     PaginatorConfigTypeDef,
@@ -413,17 +445,15 @@
     NetworkFirewallMissingSubnetViolationTypeDef,
     StatefulEngineOptionsTypeDef,
     StatelessRuleGroupTypeDef,
     NetworkFirewallPolicyTypeDef,
     NetworkFirewallStatefulRuleGroupOverrideTypeDef,
     ThirdPartyFirewallPolicyTypeDef,
     ResourceTagTypeDef,
-    ProtocolsListDataTypeDef,
     PutNotificationChannelRequestRequestTypeDef,
-    ResourceSetTypeDef,
     ThirdPartyFirewallMissingExpectedRouteTableViolationTypeDef,
     ThirdPartyFirewallMissingFirewallViolationTypeDef,
     ThirdPartyFirewallMissingSubnetViolationTypeDef,
     SecurityGroupRuleDescriptionTypeDef,
     UntagResourceRequestRequestTypeDef,
     EC2AssociateRouteTableActionTypeDef,
     EC2CopyRouteTableActionTypeDef,
@@ -433,14 +463,17 @@
     EC2ReplaceRouteActionTypeDef,
     EC2ReplaceRouteTableAssociationActionTypeDef,
     AdminScopeOutputTypeDef,
     AdminScopeTypeDef,
     AppsListDataOutputTypeDef,
     AppsListDataSummaryTypeDef,
     AppsListDataTypeDef,
+    GetProtectionStatusRequestRequestTypeDef,
+    ProtocolsListDataTypeDef,
+    ResourceSetTypeDef,
     AssociateThirdPartyFirewallResponseTypeDef,
     DisassociateThirdPartyFirewallResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetAdminAccountResponseTypeDef,
     GetNotificationChannelResponseTypeDef,
     GetProtectionStatusResponseTypeDef,
     GetThirdPartyFirewallAssociationStatusResponseTypeDef,
@@ -477,45 +510,50 @@
     NetworkFirewallInternetTrafficNotInspectedViolationTypeDef,
     NetworkFirewallInvalidRouteConfigurationViolationTypeDef,
     NetworkFirewallUnexpectedFirewallRoutesViolationTypeDef,
     NetworkFirewallUnexpectedGatewayRoutesViolationTypeDef,
     RouteHasOutOfScopeEndpointViolationTypeDef,
     StatefulRuleGroupTypeDef,
     PolicyOptionTypeDef,
-    PutProtocolsListRequestRequestTypeDef,
-    PutResourceSetRequestRequestTypeDef,
     SecurityGroupRemediationActionTypeDef,
     RemediationActionTypeDef,
     GetAdminScopeResponseTypeDef,
+    AdminScopeUnionTypeDef,
     PutAdminAccountRequestRequestTypeDef,
     GetAppsListResponseTypeDef,
     PutAppsListResponseTypeDef,
     ListAppsListsResponseTypeDef,
+    AppsListDataUnionTypeDef,
     PutAppsListRequestRequestTypeDef,
+    ProtocolsListDataUnionTypeDef,
+    PutProtocolsListRequestRequestTypeDef,
+    PutResourceSetRequestRequestTypeDef,
+    ResourceSetUnionTypeDef,
     GetComplianceDetailResponseTypeDef,
     ListComplianceStatusResponseTypeDef,
     NetworkFirewallPolicyDescriptionTypeDef,
     SecurityServicePolicyDataTypeDef,
     AwsVPCSecurityGroupViolationTypeDef,
     RemediationActionWithOrderTypeDef,
     NetworkFirewallPolicyModifiedViolationTypeDef,
     PolicyOutputTypeDef,
     PolicyTypeDef,
     PossibleRemediationActionTypeDef,
     GetPolicyResponseTypeDef,
     PutPolicyResponseTypeDef,
+    PolicyUnionTypeDef,
     PutPolicyRequestRequestTypeDef,
     PossibleRemediationActionsTypeDef,
     ResourceViolationTypeDef,
     ViolationDetailTypeDef,
     GetViolationDetailsResponseTypeDef,
 )
 
 
-def get_structure() -> AccountScopeOutputTypeDef:
+def get_value() -> AccountScopeOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-fms-1.28.15.post1/mypy_boto3_fms/__init__.py` & `mypy-boto3-fms-1.28.16/mypy_boto3_fms/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fms-1.28.15.post1/mypy_boto3_fms/__init__.pyi` & `mypy-boto3-fms-1.28.16/mypy_boto3_fms/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fms-1.28.15.post1/mypy_boto3_fms/__main__.py` & `mypy-boto3-fms-1.28.16/mypy_boto3_fms/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.FMS 1.28.15\nVersion:         1.28.15.post1\nBuilder version:"
-        " 7.16.2\nDocs:           "
+        "Type annotations for boto3.FMS 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS\nOther"
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

### Comparing `mypy-boto3-fms-1.28.15.post1/mypy_boto3_fms/client.py` & `mypy-boto3-fms-1.28.16/mypy_boto3_fms/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_fms.client import FMSClient
 
     session = Session()
     client: FMSClient = session.client("fms")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ThirdPartyFirewallType
 from .paginator import (
     ListAdminAccountsForOrganizationPaginator,
     ListAdminsManagingAccountPaginator,
@@ -27,18 +26,16 @@
     ListComplianceStatusPaginator,
     ListMemberAccountsPaginator,
     ListPoliciesPaginator,
     ListProtocolsListsPaginator,
     ListThirdPartyFirewallFirewallPoliciesPaginator,
 )
 from .type_defs import (
-    AdminScopeOutputTypeDef,
-    AdminScopeTypeDef,
-    AppsListDataOutputTypeDef,
-    AppsListDataTypeDef,
+    AdminScopeUnionTypeDef,
+    AppsListDataUnionTypeDef,
     AssociateThirdPartyFirewallResponseTypeDef,
     BatchAssociateResourceResponseTypeDef,
     BatchDisassociateResourceResponseTypeDef,
     DisassociateThirdPartyFirewallResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetAdminAccountResponseTypeDef,
     GetAdminScopeResponseTypeDef,
@@ -59,25 +56,23 @@
     ListMemberAccountsResponseTypeDef,
     ListPoliciesResponseTypeDef,
     ListProtocolsListsResponseTypeDef,
     ListResourceSetResourcesResponseTypeDef,
     ListResourceSetsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListThirdPartyFirewallFirewallPoliciesResponseTypeDef,
-    PolicyOutputTypeDef,
-    PolicyTypeDef,
-    ProtocolsListDataOutputTypeDef,
-    ProtocolsListDataTypeDef,
+    PolicyUnionTypeDef,
+    ProtocolsListDataUnionTypeDef,
     PutAppsListResponseTypeDef,
     PutPolicyResponseTypeDef,
     PutProtocolsListResponseTypeDef,
     PutResourceSetResponseTypeDef,
-    ResourceSetOutputTypeDef,
-    ResourceSetTypeDef,
+    ResourceSetUnionTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -305,16 +300,16 @@
         """
 
     def get_protection_status(
         self,
         *,
         PolicyId: str,
         MemberAccountId: str = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> GetProtectionStatusResponseTypeDef:
         """
         If you created a Shield Advanced policy, returns policy-level attack summary
         information in the event of a potential DDoS attack.
 
@@ -487,31 +482,25 @@
         with the third-party firewall administrator's account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.list_third_party_firewall_firewall_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#list_third_party_firewall_firewall_policies)
         """
 
     def put_admin_account(
-        self,
-        *,
-        AdminAccount: str,
-        AdminScope: Union[AdminScopeTypeDef, AdminScopeOutputTypeDef] = ...
+        self, *, AdminAccount: str, AdminScope: AdminScopeUnionTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates or updates an Firewall Manager administrator account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.put_admin_account)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#put_admin_account)
         """
 
     def put_apps_list(
-        self,
-        *,
-        AppsList: Union[AppsListDataTypeDef, AppsListDataOutputTypeDef],
-        TagList: Sequence[TagTypeDef] = ...
+        self, *, AppsList: AppsListDataUnionTypeDef, TagList: Sequence[TagTypeDef] = ...
     ) -> PutAppsListResponseTypeDef:
         """
         Creates an Firewall Manager applications list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.put_apps_list)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#put_apps_list)
         """
@@ -524,44 +513,35 @@
         Firewall Manager uses to record SNS logs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.put_notification_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#put_notification_channel)
         """
 
     def put_policy(
-        self,
-        *,
-        Policy: Union[PolicyTypeDef, PolicyOutputTypeDef],
-        TagList: Sequence[TagTypeDef] = ...
+        self, *, Policy: PolicyUnionTypeDef, TagList: Sequence[TagTypeDef] = ...
     ) -> PutPolicyResponseTypeDef:
         """
         Creates an Firewall Manager policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.put_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#put_policy)
         """
 
     def put_protocols_list(
-        self,
-        *,
-        ProtocolsList: Union[ProtocolsListDataTypeDef, ProtocolsListDataOutputTypeDef],
-        TagList: Sequence[TagTypeDef] = ...
+        self, *, ProtocolsList: ProtocolsListDataUnionTypeDef, TagList: Sequence[TagTypeDef] = ...
     ) -> PutProtocolsListResponseTypeDef:
         """
         Creates an Firewall Manager protocols list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.put_protocols_list)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#put_protocols_list)
         """
 
     def put_resource_set(
-        self,
-        *,
-        ResourceSet: Union[ResourceSetTypeDef, ResourceSetOutputTypeDef],
-        TagList: Sequence[TagTypeDef] = ...
+        self, *, ResourceSet: ResourceSetUnionTypeDef, TagList: Sequence[TagTypeDef] = ...
     ) -> PutResourceSetResponseTypeDef:
         """
         Creates the resource set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.put_resource_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#put_resource_set)
         """
```

### Comparing `mypy-boto3-fms-1.28.15.post1/mypy_boto3_fms/client.pyi` & `mypy-boto3-fms-1.28.16/mypy_boto3_fms/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_fms.client import FMSClient
 
     session = Session()
     client: FMSClient = session.client("fms")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ThirdPartyFirewallType
 from .paginator import (
     ListAdminAccountsForOrganizationPaginator,
     ListAdminsManagingAccountPaginator,
@@ -27,18 +26,16 @@
     ListComplianceStatusPaginator,
     ListMemberAccountsPaginator,
     ListPoliciesPaginator,
     ListProtocolsListsPaginator,
     ListThirdPartyFirewallFirewallPoliciesPaginator,
 )
 from .type_defs import (
-    AdminScopeOutputTypeDef,
-    AdminScopeTypeDef,
-    AppsListDataOutputTypeDef,
-    AppsListDataTypeDef,
+    AdminScopeUnionTypeDef,
+    AppsListDataUnionTypeDef,
     AssociateThirdPartyFirewallResponseTypeDef,
     BatchAssociateResourceResponseTypeDef,
     BatchDisassociateResourceResponseTypeDef,
     DisassociateThirdPartyFirewallResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetAdminAccountResponseTypeDef,
     GetAdminScopeResponseTypeDef,
@@ -59,25 +56,23 @@
     ListMemberAccountsResponseTypeDef,
     ListPoliciesResponseTypeDef,
     ListProtocolsListsResponseTypeDef,
     ListResourceSetResourcesResponseTypeDef,
     ListResourceSetsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListThirdPartyFirewallFirewallPoliciesResponseTypeDef,
-    PolicyOutputTypeDef,
-    PolicyTypeDef,
-    ProtocolsListDataOutputTypeDef,
-    ProtocolsListDataTypeDef,
+    PolicyUnionTypeDef,
+    ProtocolsListDataUnionTypeDef,
     PutAppsListResponseTypeDef,
     PutPolicyResponseTypeDef,
     PutProtocolsListResponseTypeDef,
     PutResourceSetResponseTypeDef,
-    ResourceSetOutputTypeDef,
-    ResourceSetTypeDef,
+    ResourceSetUnionTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -280,16 +275,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#get_policy)
         """
     def get_protection_status(
         self,
         *,
         PolicyId: str,
         MemberAccountId: str = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> GetProtectionStatusResponseTypeDef:
         """
         If you created a Shield Advanced policy, returns policy-level attack summary
         information in the event of a potential DDoS attack.
 
@@ -445,30 +440,24 @@
         Retrieves a list of all of the third-party firewall policies that are associated
         with the third-party firewall administrator's account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.list_third_party_firewall_firewall_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#list_third_party_firewall_firewall_policies)
         """
     def put_admin_account(
-        self,
-        *,
-        AdminAccount: str,
-        AdminScope: Union[AdminScopeTypeDef, AdminScopeOutputTypeDef] = ...
+        self, *, AdminAccount: str, AdminScope: AdminScopeUnionTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates or updates an Firewall Manager administrator account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.put_admin_account)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#put_admin_account)
         """
     def put_apps_list(
-        self,
-        *,
-        AppsList: Union[AppsListDataTypeDef, AppsListDataOutputTypeDef],
-        TagList: Sequence[TagTypeDef] = ...
+        self, *, AppsList: AppsListDataUnionTypeDef, TagList: Sequence[TagTypeDef] = ...
     ) -> PutAppsListResponseTypeDef:
         """
         Creates an Firewall Manager applications list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.put_apps_list)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#put_apps_list)
         """
@@ -479,42 +468,33 @@
         Designates the IAM role and Amazon Simple Notification Service (SNS) topic that
         Firewall Manager uses to record SNS logs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.put_notification_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#put_notification_channel)
         """
     def put_policy(
-        self,
-        *,
-        Policy: Union[PolicyTypeDef, PolicyOutputTypeDef],
-        TagList: Sequence[TagTypeDef] = ...
+        self, *, Policy: PolicyUnionTypeDef, TagList: Sequence[TagTypeDef] = ...
     ) -> PutPolicyResponseTypeDef:
         """
         Creates an Firewall Manager policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.put_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#put_policy)
         """
     def put_protocols_list(
-        self,
-        *,
-        ProtocolsList: Union[ProtocolsListDataTypeDef, ProtocolsListDataOutputTypeDef],
-        TagList: Sequence[TagTypeDef] = ...
+        self, *, ProtocolsList: ProtocolsListDataUnionTypeDef, TagList: Sequence[TagTypeDef] = ...
     ) -> PutProtocolsListResponseTypeDef:
         """
         Creates an Firewall Manager protocols list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.put_protocols_list)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#put_protocols_list)
         """
     def put_resource_set(
-        self,
-        *,
-        ResourceSet: Union[ResourceSetTypeDef, ResourceSetOutputTypeDef],
-        TagList: Sequence[TagTypeDef] = ...
+        self, *, ResourceSet: ResourceSetUnionTypeDef, TagList: Sequence[TagTypeDef] = ...
     ) -> PutResourceSetResponseTypeDef:
         """
         Creates the resource set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.put_resource_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#put_resource_set)
         """
```

### Comparing `mypy-boto3-fms-1.28.15.post1/mypy_boto3_fms/literals.py` & `mypy-boto3-fms-1.28.16/mypy_boto3_fms/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fms-1.28.15.post1/mypy_boto3_fms/literals.pyi` & `mypy-boto3-fms-1.28.16/mypy_boto3_fms/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fms-1.28.15.post1/mypy_boto3_fms/paginator.py` & `mypy-boto3-fms-1.28.16/mypy_boto3_fms/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fms-1.28.15.post1/mypy_boto3_fms/paginator.pyi` & `mypy-boto3-fms-1.28.16/mypy_boto3_fms/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fms-1.28.15.post1/mypy_boto3_fms/type_defs.py` & `mypy-boto3-fms-1.28.16/mypy_boto3_fms/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_fms.type_defs import AccountScopeOutputTypeDef
 
-    data: AccountScopeOutputTypeDef = {...}
+    data: AccountScopeOutputTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -54,14 +54,15 @@
     "OrganizationalUnitScopeOutputTypeDef",
     "PolicyTypeScopeOutputTypeDef",
     "RegionScopeOutputTypeDef",
     "OrganizationalUnitScopeTypeDef",
     "PolicyTypeScopeTypeDef",
     "RegionScopeTypeDef",
     "AppTypeDef",
+    "TimestampTypeDef",
     "AssociateAdminAccountRequestRequestTypeDef",
     "AssociateThirdPartyFirewallRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AwsEc2NetworkInterfaceViolationTypeDef",
     "PartialMatchTypeDef",
     "BatchAssociateResourceRequestRequestTypeDef",
     "FailedItemTypeDef",
@@ -81,15 +82,14 @@
     "FMSPolicyUpdateFirewallCreationConfigActionTypeDef",
     "FirewallSubnetIsOutOfScopeViolationTypeDef",
     "FirewallSubnetMissingVPCEndpointViolationTypeDef",
     "GetAdminScopeRequestRequestTypeDef",
     "GetAppsListRequestRequestTypeDef",
     "GetComplianceDetailRequestRequestTypeDef",
     "GetPolicyRequestRequestTypeDef",
-    "GetProtectionStatusRequestRequestTypeDef",
     "GetProtocolsListRequestRequestTypeDef",
     "ProtocolsListDataOutputTypeDef",
     "GetResourceSetRequestRequestTypeDef",
     "ResourceSetOutputTypeDef",
     "GetThirdPartyFirewallAssociationStatusRequestRequestTypeDef",
     "GetViolationDetailsRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
@@ -117,17 +117,15 @@
     "NetworkFirewallMissingSubnetViolationTypeDef",
     "StatefulEngineOptionsTypeDef",
     "StatelessRuleGroupTypeDef",
     "NetworkFirewallPolicyTypeDef",
     "NetworkFirewallStatefulRuleGroupOverrideTypeDef",
     "ThirdPartyFirewallPolicyTypeDef",
     "ResourceTagTypeDef",
-    "ProtocolsListDataTypeDef",
     "PutNotificationChannelRequestRequestTypeDef",
-    "ResourceSetTypeDef",
     "ThirdPartyFirewallMissingExpectedRouteTableViolationTypeDef",
     "ThirdPartyFirewallMissingFirewallViolationTypeDef",
     "ThirdPartyFirewallMissingSubnetViolationTypeDef",
     "SecurityGroupRuleDescriptionTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "EC2AssociateRouteTableActionTypeDef",
     "EC2CopyRouteTableActionTypeDef",
@@ -137,14 +135,17 @@
     "EC2ReplaceRouteActionTypeDef",
     "EC2ReplaceRouteTableAssociationActionTypeDef",
     "AdminScopeOutputTypeDef",
     "AdminScopeTypeDef",
     "AppsListDataOutputTypeDef",
     "AppsListDataSummaryTypeDef",
     "AppsListDataTypeDef",
+    "GetProtectionStatusRequestRequestTypeDef",
+    "ProtocolsListDataTypeDef",
+    "ResourceSetTypeDef",
     "AssociateThirdPartyFirewallResponseTypeDef",
     "DisassociateThirdPartyFirewallResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetAdminAccountResponseTypeDef",
     "GetNotificationChannelResponseTypeDef",
     "GetProtectionStatusResponseTypeDef",
     "GetThirdPartyFirewallAssociationStatusResponseTypeDef",
@@ -181,36 +182,41 @@
     "NetworkFirewallInternetTrafficNotInspectedViolationTypeDef",
     "NetworkFirewallInvalidRouteConfigurationViolationTypeDef",
     "NetworkFirewallUnexpectedFirewallRoutesViolationTypeDef",
     "NetworkFirewallUnexpectedGatewayRoutesViolationTypeDef",
     "RouteHasOutOfScopeEndpointViolationTypeDef",
     "StatefulRuleGroupTypeDef",
     "PolicyOptionTypeDef",
-    "PutProtocolsListRequestRequestTypeDef",
-    "PutResourceSetRequestRequestTypeDef",
     "SecurityGroupRemediationActionTypeDef",
     "RemediationActionTypeDef",
     "GetAdminScopeResponseTypeDef",
+    "AdminScopeUnionTypeDef",
     "PutAdminAccountRequestRequestTypeDef",
     "GetAppsListResponseTypeDef",
     "PutAppsListResponseTypeDef",
     "ListAppsListsResponseTypeDef",
+    "AppsListDataUnionTypeDef",
     "PutAppsListRequestRequestTypeDef",
+    "ProtocolsListDataUnionTypeDef",
+    "PutProtocolsListRequestRequestTypeDef",
+    "PutResourceSetRequestRequestTypeDef",
+    "ResourceSetUnionTypeDef",
     "GetComplianceDetailResponseTypeDef",
     "ListComplianceStatusResponseTypeDef",
     "NetworkFirewallPolicyDescriptionTypeDef",
     "SecurityServicePolicyDataTypeDef",
     "AwsVPCSecurityGroupViolationTypeDef",
     "RemediationActionWithOrderTypeDef",
     "NetworkFirewallPolicyModifiedViolationTypeDef",
     "PolicyOutputTypeDef",
     "PolicyTypeDef",
     "PossibleRemediationActionTypeDef",
     "GetPolicyResponseTypeDef",
     "PutPolicyResponseTypeDef",
+    "PolicyUnionTypeDef",
     "PutPolicyRequestRequestTypeDef",
     "PossibleRemediationActionsTypeDef",
     "ResourceViolationTypeDef",
     "ViolationDetailTypeDef",
     "GetViolationDetailsResponseTypeDef",
 )
 
@@ -314,14 +320,15 @@
     {
         "AppName": str,
         "Protocol": str,
         "Port": int,
     },
 )
 
+TimestampTypeDef = Union[datetime, str]
 AssociateAdminAccountRequestRequestTypeDef = TypedDict(
     "AssociateAdminAccountRequestRequestTypeDef",
     {
         "AdminAccount": str,
     },
 )
 
@@ -582,40 +589,14 @@
 GetPolicyRequestRequestTypeDef = TypedDict(
     "GetPolicyRequestRequestTypeDef",
     {
         "PolicyId": str,
     },
 )
 
-_RequiredGetProtectionStatusRequestRequestTypeDef = TypedDict(
-    "_RequiredGetProtectionStatusRequestRequestTypeDef",
-    {
-        "PolicyId": str,
-    },
-)
-_OptionalGetProtectionStatusRequestRequestTypeDef = TypedDict(
-    "_OptionalGetProtectionStatusRequestRequestTypeDef",
-    {
-        "MemberAccountId": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-
-class GetProtectionStatusRequestRequestTypeDef(
-    _RequiredGetProtectionStatusRequestRequestTypeDef,
-    _OptionalGetProtectionStatusRequestRequestTypeDef,
-):
-    pass
-
-
 _RequiredGetProtocolsListRequestRequestTypeDef = TypedDict(
     "_RequiredGetProtocolsListRequestRequestTypeDef",
     {
         "ListId": str,
     },
 )
 _OptionalGetProtocolsListRequestRequestTypeDef = TypedDict(
@@ -1085,72 +1066,22 @@
 )
 
 
 class ResourceTagTypeDef(_RequiredResourceTagTypeDef, _OptionalResourceTagTypeDef):
     pass
 
 
-_RequiredProtocolsListDataTypeDef = TypedDict(
-    "_RequiredProtocolsListDataTypeDef",
-    {
-        "ListName": str,
-        "ProtocolsList": Sequence[str],
-    },
-)
-_OptionalProtocolsListDataTypeDef = TypedDict(
-    "_OptionalProtocolsListDataTypeDef",
-    {
-        "ListId": str,
-        "ListUpdateToken": str,
-        "CreateTime": Union[datetime, str],
-        "LastUpdateTime": Union[datetime, str],
-        "PreviousProtocolsList": Mapping[str, Sequence[str]],
-    },
-    total=False,
-)
-
-
-class ProtocolsListDataTypeDef(
-    _RequiredProtocolsListDataTypeDef, _OptionalProtocolsListDataTypeDef
-):
-    pass
-
-
 PutNotificationChannelRequestRequestTypeDef = TypedDict(
     "PutNotificationChannelRequestRequestTypeDef",
     {
         "SnsTopicArn": str,
         "SnsRoleName": str,
     },
 )
 
-_RequiredResourceSetTypeDef = TypedDict(
-    "_RequiredResourceSetTypeDef",
-    {
-        "Name": str,
-        "ResourceTypeList": Sequence[str],
-    },
-)
-_OptionalResourceSetTypeDef = TypedDict(
-    "_OptionalResourceSetTypeDef",
-    {
-        "Id": str,
-        "Description": str,
-        "UpdateToken": str,
-        "LastUpdateTime": Union[datetime, str],
-        "ResourceSetStatus": ResourceSetStatusType,
-    },
-    total=False,
-)
-
-
-class ResourceSetTypeDef(_RequiredResourceSetTypeDef, _OptionalResourceSetTypeDef):
-    pass
-
-
 ThirdPartyFirewallMissingExpectedRouteTableViolationTypeDef = TypedDict(
     "ThirdPartyFirewallMissingExpectedRouteTableViolationTypeDef",
     {
         "ViolationTarget": str,
         "VPC": str,
         "AvailabilityZone": str,
         "CurrentRouteTable": str,
@@ -1433,26 +1364,102 @@
     },
 )
 _OptionalAppsListDataTypeDef = TypedDict(
     "_OptionalAppsListDataTypeDef",
     {
         "ListId": str,
         "ListUpdateToken": str,
-        "CreateTime": Union[datetime, str],
-        "LastUpdateTime": Union[datetime, str],
+        "CreateTime": TimestampTypeDef,
+        "LastUpdateTime": TimestampTypeDef,
         "PreviousAppsList": Mapping[str, Sequence[AppTypeDef]],
     },
     total=False,
 )
 
 
 class AppsListDataTypeDef(_RequiredAppsListDataTypeDef, _OptionalAppsListDataTypeDef):
     pass
 
 
+_RequiredGetProtectionStatusRequestRequestTypeDef = TypedDict(
+    "_RequiredGetProtectionStatusRequestRequestTypeDef",
+    {
+        "PolicyId": str,
+    },
+)
+_OptionalGetProtectionStatusRequestRequestTypeDef = TypedDict(
+    "_OptionalGetProtectionStatusRequestRequestTypeDef",
+    {
+        "MemberAccountId": str,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+
+class GetProtectionStatusRequestRequestTypeDef(
+    _RequiredGetProtectionStatusRequestRequestTypeDef,
+    _OptionalGetProtectionStatusRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredProtocolsListDataTypeDef = TypedDict(
+    "_RequiredProtocolsListDataTypeDef",
+    {
+        "ListName": str,
+        "ProtocolsList": Sequence[str],
+    },
+)
+_OptionalProtocolsListDataTypeDef = TypedDict(
+    "_OptionalProtocolsListDataTypeDef",
+    {
+        "ListId": str,
+        "ListUpdateToken": str,
+        "CreateTime": TimestampTypeDef,
+        "LastUpdateTime": TimestampTypeDef,
+        "PreviousProtocolsList": Mapping[str, Sequence[str]],
+    },
+    total=False,
+)
+
+
+class ProtocolsListDataTypeDef(
+    _RequiredProtocolsListDataTypeDef, _OptionalProtocolsListDataTypeDef
+):
+    pass
+
+
+_RequiredResourceSetTypeDef = TypedDict(
+    "_RequiredResourceSetTypeDef",
+    {
+        "Name": str,
+        "ResourceTypeList": Sequence[str],
+    },
+)
+_OptionalResourceSetTypeDef = TypedDict(
+    "_OptionalResourceSetTypeDef",
+    {
+        "Id": str,
+        "Description": str,
+        "UpdateToken": str,
+        "LastUpdateTime": TimestampTypeDef,
+        "ResourceSetStatus": ResourceSetStatusType,
+    },
+    total=False,
+)
+
+
+class ResourceSetTypeDef(_RequiredResourceSetTypeDef, _OptionalResourceSetTypeDef):
+    pass
+
+
 AssociateThirdPartyFirewallResponseTypeDef = TypedDict(
     "AssociateThirdPartyFirewallResponseTypeDef",
     {
         "ThirdPartyFirewallStatus": ThirdPartyFirewallAssociationStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1916,56 +1923,14 @@
     {
         "NetworkFirewallPolicy": NetworkFirewallPolicyTypeDef,
         "ThirdPartyFirewallPolicy": ThirdPartyFirewallPolicyTypeDef,
     },
     total=False,
 )
 
-_RequiredPutProtocolsListRequestRequestTypeDef = TypedDict(
-    "_RequiredPutProtocolsListRequestRequestTypeDef",
-    {
-        "ProtocolsList": ProtocolsListDataTypeDef,
-    },
-)
-_OptionalPutProtocolsListRequestRequestTypeDef = TypedDict(
-    "_OptionalPutProtocolsListRequestRequestTypeDef",
-    {
-        "TagList": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-
-class PutProtocolsListRequestRequestTypeDef(
-    _RequiredPutProtocolsListRequestRequestTypeDef, _OptionalPutProtocolsListRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredPutResourceSetRequestRequestTypeDef = TypedDict(
-    "_RequiredPutResourceSetRequestRequestTypeDef",
-    {
-        "ResourceSet": ResourceSetTypeDef,
-    },
-)
-_OptionalPutResourceSetRequestRequestTypeDef = TypedDict(
-    "_OptionalPutResourceSetRequestRequestTypeDef",
-    {
-        "TagList": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-
-class PutResourceSetRequestRequestTypeDef(
-    _RequiredPutResourceSetRequestRequestTypeDef, _OptionalPutResourceSetRequestRequestTypeDef
-):
-    pass
-
-
 SecurityGroupRemediationActionTypeDef = TypedDict(
     "SecurityGroupRemediationActionTypeDef",
     {
         "RemediationActionType": RemediationActionTypeType,
         "Description": str,
         "RemediationResult": SecurityGroupRuleDescriptionTypeDef,
         "IsDefaultAction": bool,
@@ -1996,14 +1961,15 @@
     {
         "AdminScope": AdminScopeOutputTypeDef,
         "Status": OrganizationStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+AdminScopeUnionTypeDef = Union[AdminScopeTypeDef, AdminScopeOutputTypeDef]
 _RequiredPutAdminAccountRequestRequestTypeDef = TypedDict(
     "_RequiredPutAdminAccountRequestRequestTypeDef",
     {
         "AdminAccount": str,
     },
 )
 _OptionalPutAdminAccountRequestRequestTypeDef = TypedDict(
@@ -2044,14 +2010,15 @@
     {
         "AppsLists": List[AppsListDataSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+AppsListDataUnionTypeDef = Union[AppsListDataTypeDef, AppsListDataOutputTypeDef]
 _RequiredPutAppsListRequestRequestTypeDef = TypedDict(
     "_RequiredPutAppsListRequestRequestTypeDef",
     {
         "AppsList": AppsListDataTypeDef,
     },
 )
 _OptionalPutAppsListRequestRequestTypeDef = TypedDict(
@@ -2065,14 +2032,58 @@
 
 class PutAppsListRequestRequestTypeDef(
     _RequiredPutAppsListRequestRequestTypeDef, _OptionalPutAppsListRequestRequestTypeDef
 ):
     pass
 
 
+ProtocolsListDataUnionTypeDef = Union[ProtocolsListDataTypeDef, ProtocolsListDataOutputTypeDef]
+_RequiredPutProtocolsListRequestRequestTypeDef = TypedDict(
+    "_RequiredPutProtocolsListRequestRequestTypeDef",
+    {
+        "ProtocolsList": ProtocolsListDataTypeDef,
+    },
+)
+_OptionalPutProtocolsListRequestRequestTypeDef = TypedDict(
+    "_OptionalPutProtocolsListRequestRequestTypeDef",
+    {
+        "TagList": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class PutProtocolsListRequestRequestTypeDef(
+    _RequiredPutProtocolsListRequestRequestTypeDef, _OptionalPutProtocolsListRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredPutResourceSetRequestRequestTypeDef = TypedDict(
+    "_RequiredPutResourceSetRequestRequestTypeDef",
+    {
+        "ResourceSet": ResourceSetTypeDef,
+    },
+)
+_OptionalPutResourceSetRequestRequestTypeDef = TypedDict(
+    "_OptionalPutResourceSetRequestRequestTypeDef",
+    {
+        "TagList": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class PutResourceSetRequestRequestTypeDef(
+    _RequiredPutResourceSetRequestRequestTypeDef, _OptionalPutResourceSetRequestRequestTypeDef
+):
+    pass
+
+
+ResourceSetUnionTypeDef = Union[ResourceSetTypeDef, ResourceSetOutputTypeDef]
 GetComplianceDetailResponseTypeDef = TypedDict(
     "GetComplianceDetailResponseTypeDef",
     {
         "PolicyComplianceDetail": PolicyComplianceDetailTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2252,14 +2263,15 @@
     {
         "Policy": PolicyOutputTypeDef,
         "PolicyArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+PolicyUnionTypeDef = Union[PolicyTypeDef, PolicyOutputTypeDef]
 _RequiredPutPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutPolicyRequestRequestTypeDef",
     {
         "Policy": PolicyTypeDef,
     },
 )
 _OptionalPutPolicyRequestRequestTypeDef = TypedDict(
```

### Comparing `mypy-boto3-fms-1.28.15.post1/mypy_boto3_fms/type_defs.pyi` & `mypy-boto3-fms-1.28.16/mypy_boto3_fms/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_fms.type_defs import AccountScopeOutputTypeDef
 
-    data: AccountScopeOutputTypeDef = {...}
+    data: AccountScopeOutputTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -53,14 +53,15 @@
     "OrganizationalUnitScopeOutputTypeDef",
     "PolicyTypeScopeOutputTypeDef",
     "RegionScopeOutputTypeDef",
     "OrganizationalUnitScopeTypeDef",
     "PolicyTypeScopeTypeDef",
     "RegionScopeTypeDef",
     "AppTypeDef",
+    "TimestampTypeDef",
     "AssociateAdminAccountRequestRequestTypeDef",
     "AssociateThirdPartyFirewallRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AwsEc2NetworkInterfaceViolationTypeDef",
     "PartialMatchTypeDef",
     "BatchAssociateResourceRequestRequestTypeDef",
     "FailedItemTypeDef",
@@ -80,15 +81,14 @@
     "FMSPolicyUpdateFirewallCreationConfigActionTypeDef",
     "FirewallSubnetIsOutOfScopeViolationTypeDef",
     "FirewallSubnetMissingVPCEndpointViolationTypeDef",
     "GetAdminScopeRequestRequestTypeDef",
     "GetAppsListRequestRequestTypeDef",
     "GetComplianceDetailRequestRequestTypeDef",
     "GetPolicyRequestRequestTypeDef",
-    "GetProtectionStatusRequestRequestTypeDef",
     "GetProtocolsListRequestRequestTypeDef",
     "ProtocolsListDataOutputTypeDef",
     "GetResourceSetRequestRequestTypeDef",
     "ResourceSetOutputTypeDef",
     "GetThirdPartyFirewallAssociationStatusRequestRequestTypeDef",
     "GetViolationDetailsRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
@@ -116,17 +116,15 @@
     "NetworkFirewallMissingSubnetViolationTypeDef",
     "StatefulEngineOptionsTypeDef",
     "StatelessRuleGroupTypeDef",
     "NetworkFirewallPolicyTypeDef",
     "NetworkFirewallStatefulRuleGroupOverrideTypeDef",
     "ThirdPartyFirewallPolicyTypeDef",
     "ResourceTagTypeDef",
-    "ProtocolsListDataTypeDef",
     "PutNotificationChannelRequestRequestTypeDef",
-    "ResourceSetTypeDef",
     "ThirdPartyFirewallMissingExpectedRouteTableViolationTypeDef",
     "ThirdPartyFirewallMissingFirewallViolationTypeDef",
     "ThirdPartyFirewallMissingSubnetViolationTypeDef",
     "SecurityGroupRuleDescriptionTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "EC2AssociateRouteTableActionTypeDef",
     "EC2CopyRouteTableActionTypeDef",
@@ -136,14 +134,17 @@
     "EC2ReplaceRouteActionTypeDef",
     "EC2ReplaceRouteTableAssociationActionTypeDef",
     "AdminScopeOutputTypeDef",
     "AdminScopeTypeDef",
     "AppsListDataOutputTypeDef",
     "AppsListDataSummaryTypeDef",
     "AppsListDataTypeDef",
+    "GetProtectionStatusRequestRequestTypeDef",
+    "ProtocolsListDataTypeDef",
+    "ResourceSetTypeDef",
     "AssociateThirdPartyFirewallResponseTypeDef",
     "DisassociateThirdPartyFirewallResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetAdminAccountResponseTypeDef",
     "GetNotificationChannelResponseTypeDef",
     "GetProtectionStatusResponseTypeDef",
     "GetThirdPartyFirewallAssociationStatusResponseTypeDef",
@@ -180,36 +181,41 @@
     "NetworkFirewallInternetTrafficNotInspectedViolationTypeDef",
     "NetworkFirewallInvalidRouteConfigurationViolationTypeDef",
     "NetworkFirewallUnexpectedFirewallRoutesViolationTypeDef",
     "NetworkFirewallUnexpectedGatewayRoutesViolationTypeDef",
     "RouteHasOutOfScopeEndpointViolationTypeDef",
     "StatefulRuleGroupTypeDef",
     "PolicyOptionTypeDef",
-    "PutProtocolsListRequestRequestTypeDef",
-    "PutResourceSetRequestRequestTypeDef",
     "SecurityGroupRemediationActionTypeDef",
     "RemediationActionTypeDef",
     "GetAdminScopeResponseTypeDef",
+    "AdminScopeUnionTypeDef",
     "PutAdminAccountRequestRequestTypeDef",
     "GetAppsListResponseTypeDef",
     "PutAppsListResponseTypeDef",
     "ListAppsListsResponseTypeDef",
+    "AppsListDataUnionTypeDef",
     "PutAppsListRequestRequestTypeDef",
+    "ProtocolsListDataUnionTypeDef",
+    "PutProtocolsListRequestRequestTypeDef",
+    "PutResourceSetRequestRequestTypeDef",
+    "ResourceSetUnionTypeDef",
     "GetComplianceDetailResponseTypeDef",
     "ListComplianceStatusResponseTypeDef",
     "NetworkFirewallPolicyDescriptionTypeDef",
     "SecurityServicePolicyDataTypeDef",
     "AwsVPCSecurityGroupViolationTypeDef",
     "RemediationActionWithOrderTypeDef",
     "NetworkFirewallPolicyModifiedViolationTypeDef",
     "PolicyOutputTypeDef",
     "PolicyTypeDef",
     "PossibleRemediationActionTypeDef",
     "GetPolicyResponseTypeDef",
     "PutPolicyResponseTypeDef",
+    "PolicyUnionTypeDef",
     "PutPolicyRequestRequestTypeDef",
     "PossibleRemediationActionsTypeDef",
     "ResourceViolationTypeDef",
     "ViolationDetailTypeDef",
     "GetViolationDetailsResponseTypeDef",
 )
 
@@ -313,14 +319,15 @@
     {
         "AppName": str,
         "Protocol": str,
         "Port": int,
     },
 )
 
+TimestampTypeDef = Union[datetime, str]
 AssociateAdminAccountRequestRequestTypeDef = TypedDict(
     "AssociateAdminAccountRequestRequestTypeDef",
     {
         "AdminAccount": str,
     },
 )
 
@@ -577,38 +584,14 @@
 GetPolicyRequestRequestTypeDef = TypedDict(
     "GetPolicyRequestRequestTypeDef",
     {
         "PolicyId": str,
     },
 )
 
-_RequiredGetProtectionStatusRequestRequestTypeDef = TypedDict(
-    "_RequiredGetProtectionStatusRequestRequestTypeDef",
-    {
-        "PolicyId": str,
-    },
-)
-_OptionalGetProtectionStatusRequestRequestTypeDef = TypedDict(
-    "_OptionalGetProtectionStatusRequestRequestTypeDef",
-    {
-        "MemberAccountId": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-class GetProtectionStatusRequestRequestTypeDef(
-    _RequiredGetProtectionStatusRequestRequestTypeDef,
-    _OptionalGetProtectionStatusRequestRequestTypeDef,
-):
-    pass
-
 _RequiredGetProtocolsListRequestRequestTypeDef = TypedDict(
     "_RequiredGetProtocolsListRequestRequestTypeDef",
     {
         "ListId": str,
     },
 )
 _OptionalGetProtocolsListRequestRequestTypeDef = TypedDict(
@@ -1056,68 +1039,22 @@
     },
     total=False,
 )
 
 class ResourceTagTypeDef(_RequiredResourceTagTypeDef, _OptionalResourceTagTypeDef):
     pass
 
-_RequiredProtocolsListDataTypeDef = TypedDict(
-    "_RequiredProtocolsListDataTypeDef",
-    {
-        "ListName": str,
-        "ProtocolsList": Sequence[str],
-    },
-)
-_OptionalProtocolsListDataTypeDef = TypedDict(
-    "_OptionalProtocolsListDataTypeDef",
-    {
-        "ListId": str,
-        "ListUpdateToken": str,
-        "CreateTime": Union[datetime, str],
-        "LastUpdateTime": Union[datetime, str],
-        "PreviousProtocolsList": Mapping[str, Sequence[str]],
-    },
-    total=False,
-)
-
-class ProtocolsListDataTypeDef(
-    _RequiredProtocolsListDataTypeDef, _OptionalProtocolsListDataTypeDef
-):
-    pass
-
 PutNotificationChannelRequestRequestTypeDef = TypedDict(
     "PutNotificationChannelRequestRequestTypeDef",
     {
         "SnsTopicArn": str,
         "SnsRoleName": str,
     },
 )
 
-_RequiredResourceSetTypeDef = TypedDict(
-    "_RequiredResourceSetTypeDef",
-    {
-        "Name": str,
-        "ResourceTypeList": Sequence[str],
-    },
-)
-_OptionalResourceSetTypeDef = TypedDict(
-    "_OptionalResourceSetTypeDef",
-    {
-        "Id": str,
-        "Description": str,
-        "UpdateToken": str,
-        "LastUpdateTime": Union[datetime, str],
-        "ResourceSetStatus": ResourceSetStatusType,
-    },
-    total=False,
-)
-
-class ResourceSetTypeDef(_RequiredResourceSetTypeDef, _OptionalResourceSetTypeDef):
-    pass
-
 ThirdPartyFirewallMissingExpectedRouteTableViolationTypeDef = TypedDict(
     "ThirdPartyFirewallMissingExpectedRouteTableViolationTypeDef",
     {
         "ViolationTarget": str,
         "VPC": str,
         "AvailabilityZone": str,
         "CurrentRouteTable": str,
@@ -1384,24 +1321,94 @@
     },
 )
 _OptionalAppsListDataTypeDef = TypedDict(
     "_OptionalAppsListDataTypeDef",
     {
         "ListId": str,
         "ListUpdateToken": str,
-        "CreateTime": Union[datetime, str],
-        "LastUpdateTime": Union[datetime, str],
+        "CreateTime": TimestampTypeDef,
+        "LastUpdateTime": TimestampTypeDef,
         "PreviousAppsList": Mapping[str, Sequence[AppTypeDef]],
     },
     total=False,
 )
 
 class AppsListDataTypeDef(_RequiredAppsListDataTypeDef, _OptionalAppsListDataTypeDef):
     pass
 
+_RequiredGetProtectionStatusRequestRequestTypeDef = TypedDict(
+    "_RequiredGetProtectionStatusRequestRequestTypeDef",
+    {
+        "PolicyId": str,
+    },
+)
+_OptionalGetProtectionStatusRequestRequestTypeDef = TypedDict(
+    "_OptionalGetProtectionStatusRequestRequestTypeDef",
+    {
+        "MemberAccountId": str,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+class GetProtectionStatusRequestRequestTypeDef(
+    _RequiredGetProtectionStatusRequestRequestTypeDef,
+    _OptionalGetProtectionStatusRequestRequestTypeDef,
+):
+    pass
+
+_RequiredProtocolsListDataTypeDef = TypedDict(
+    "_RequiredProtocolsListDataTypeDef",
+    {
+        "ListName": str,
+        "ProtocolsList": Sequence[str],
+    },
+)
+_OptionalProtocolsListDataTypeDef = TypedDict(
+    "_OptionalProtocolsListDataTypeDef",
+    {
+        "ListId": str,
+        "ListUpdateToken": str,
+        "CreateTime": TimestampTypeDef,
+        "LastUpdateTime": TimestampTypeDef,
+        "PreviousProtocolsList": Mapping[str, Sequence[str]],
+    },
+    total=False,
+)
+
+class ProtocolsListDataTypeDef(
+    _RequiredProtocolsListDataTypeDef, _OptionalProtocolsListDataTypeDef
+):
+    pass
+
+_RequiredResourceSetTypeDef = TypedDict(
+    "_RequiredResourceSetTypeDef",
+    {
+        "Name": str,
+        "ResourceTypeList": Sequence[str],
+    },
+)
+_OptionalResourceSetTypeDef = TypedDict(
+    "_OptionalResourceSetTypeDef",
+    {
+        "Id": str,
+        "Description": str,
+        "UpdateToken": str,
+        "LastUpdateTime": TimestampTypeDef,
+        "ResourceSetStatus": ResourceSetStatusType,
+    },
+    total=False,
+)
+
+class ResourceSetTypeDef(_RequiredResourceSetTypeDef, _OptionalResourceSetTypeDef):
+    pass
+
 AssociateThirdPartyFirewallResponseTypeDef = TypedDict(
     "AssociateThirdPartyFirewallResponseTypeDef",
     {
         "ThirdPartyFirewallStatus": ThirdPartyFirewallAssociationStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1861,52 +1868,14 @@
     {
         "NetworkFirewallPolicy": NetworkFirewallPolicyTypeDef,
         "ThirdPartyFirewallPolicy": ThirdPartyFirewallPolicyTypeDef,
     },
     total=False,
 )
 
-_RequiredPutProtocolsListRequestRequestTypeDef = TypedDict(
-    "_RequiredPutProtocolsListRequestRequestTypeDef",
-    {
-        "ProtocolsList": ProtocolsListDataTypeDef,
-    },
-)
-_OptionalPutProtocolsListRequestRequestTypeDef = TypedDict(
-    "_OptionalPutProtocolsListRequestRequestTypeDef",
-    {
-        "TagList": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-class PutProtocolsListRequestRequestTypeDef(
-    _RequiredPutProtocolsListRequestRequestTypeDef, _OptionalPutProtocolsListRequestRequestTypeDef
-):
-    pass
-
-_RequiredPutResourceSetRequestRequestTypeDef = TypedDict(
-    "_RequiredPutResourceSetRequestRequestTypeDef",
-    {
-        "ResourceSet": ResourceSetTypeDef,
-    },
-)
-_OptionalPutResourceSetRequestRequestTypeDef = TypedDict(
-    "_OptionalPutResourceSetRequestRequestTypeDef",
-    {
-        "TagList": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-class PutResourceSetRequestRequestTypeDef(
-    _RequiredPutResourceSetRequestRequestTypeDef, _OptionalPutResourceSetRequestRequestTypeDef
-):
-    pass
-
 SecurityGroupRemediationActionTypeDef = TypedDict(
     "SecurityGroupRemediationActionTypeDef",
     {
         "RemediationActionType": RemediationActionTypeType,
         "Description": str,
         "RemediationResult": SecurityGroupRuleDescriptionTypeDef,
         "IsDefaultAction": bool,
@@ -1937,14 +1906,15 @@
     {
         "AdminScope": AdminScopeOutputTypeDef,
         "Status": OrganizationStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+AdminScopeUnionTypeDef = Union[AdminScopeTypeDef, AdminScopeOutputTypeDef]
 _RequiredPutAdminAccountRequestRequestTypeDef = TypedDict(
     "_RequiredPutAdminAccountRequestRequestTypeDef",
     {
         "AdminAccount": str,
     },
 )
 _OptionalPutAdminAccountRequestRequestTypeDef = TypedDict(
@@ -1983,14 +1953,15 @@
     {
         "AppsLists": List[AppsListDataSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+AppsListDataUnionTypeDef = Union[AppsListDataTypeDef, AppsListDataOutputTypeDef]
 _RequiredPutAppsListRequestRequestTypeDef = TypedDict(
     "_RequiredPutAppsListRequestRequestTypeDef",
     {
         "AppsList": AppsListDataTypeDef,
     },
 )
 _OptionalPutAppsListRequestRequestTypeDef = TypedDict(
@@ -2002,14 +1973,54 @@
 )
 
 class PutAppsListRequestRequestTypeDef(
     _RequiredPutAppsListRequestRequestTypeDef, _OptionalPutAppsListRequestRequestTypeDef
 ):
     pass
 
+ProtocolsListDataUnionTypeDef = Union[ProtocolsListDataTypeDef, ProtocolsListDataOutputTypeDef]
+_RequiredPutProtocolsListRequestRequestTypeDef = TypedDict(
+    "_RequiredPutProtocolsListRequestRequestTypeDef",
+    {
+        "ProtocolsList": ProtocolsListDataTypeDef,
+    },
+)
+_OptionalPutProtocolsListRequestRequestTypeDef = TypedDict(
+    "_OptionalPutProtocolsListRequestRequestTypeDef",
+    {
+        "TagList": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class PutProtocolsListRequestRequestTypeDef(
+    _RequiredPutProtocolsListRequestRequestTypeDef, _OptionalPutProtocolsListRequestRequestTypeDef
+):
+    pass
+
+_RequiredPutResourceSetRequestRequestTypeDef = TypedDict(
+    "_RequiredPutResourceSetRequestRequestTypeDef",
+    {
+        "ResourceSet": ResourceSetTypeDef,
+    },
+)
+_OptionalPutResourceSetRequestRequestTypeDef = TypedDict(
+    "_OptionalPutResourceSetRequestRequestTypeDef",
+    {
+        "TagList": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class PutResourceSetRequestRequestTypeDef(
+    _RequiredPutResourceSetRequestRequestTypeDef, _OptionalPutResourceSetRequestRequestTypeDef
+):
+    pass
+
+ResourceSetUnionTypeDef = Union[ResourceSetTypeDef, ResourceSetOutputTypeDef]
 GetComplianceDetailResponseTypeDef = TypedDict(
     "GetComplianceDetailResponseTypeDef",
     {
         "PolicyComplianceDetail": PolicyComplianceDetailTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2181,14 +2192,15 @@
     {
         "Policy": PolicyOutputTypeDef,
         "PolicyArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+PolicyUnionTypeDef = Union[PolicyTypeDef, PolicyOutputTypeDef]
 _RequiredPutPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutPolicyRequestRequestTypeDef",
     {
         "Policy": PolicyTypeDef,
     },
 )
 _OptionalPutPolicyRequestRequestTypeDef = TypedDict(
```

### Comparing `mypy-boto3-fms-1.28.15.post1/mypy_boto3_fms.egg-info/PKG-INFO` & `mypy-boto3-fms-1.28.16/mypy_boto3_fms.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-fms
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.FMS 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.FMS 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 fms type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 fms type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-fms.svg?color=blue)](https://pypi.org/project/mypy-boto3-fms)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-fms)](https://pepy.tech/project/mypy-boto3-fms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.FMS 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS)
+[boto3.FMS 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS)
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
 [mypy-boto3-fms docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/).
 
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
@@ -362,34 +362,35 @@
 )
 
 
 def check_value(value: AccountRoleStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_fms.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_fms.type_defs import (
     AccountScopeOutputTypeDef,
     AccountScopeTypeDef,
     ActionTargetTypeDef,
     AdminAccountSummaryTypeDef,
     OrganizationalUnitScopeOutputTypeDef,
     PolicyTypeScopeOutputTypeDef,
     RegionScopeOutputTypeDef,
     OrganizationalUnitScopeTypeDef,
     PolicyTypeScopeTypeDef,
     RegionScopeTypeDef,
     AppTypeDef,
+    TimestampTypeDef,
     AssociateAdminAccountRequestRequestTypeDef,
     AssociateThirdPartyFirewallRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     AwsEc2NetworkInterfaceViolationTypeDef,
     PartialMatchTypeDef,
     BatchAssociateResourceRequestRequestTypeDef,
     FailedItemTypeDef,
@@ -409,15 +410,14 @@
     FMSPolicyUpdateFirewallCreationConfigActionTypeDef,
     FirewallSubnetIsOutOfScopeViolationTypeDef,
     FirewallSubnetMissingVPCEndpointViolationTypeDef,
     GetAdminScopeRequestRequestTypeDef,
     GetAppsListRequestRequestTypeDef,
     GetComplianceDetailRequestRequestTypeDef,
     GetPolicyRequestRequestTypeDef,
-    GetProtectionStatusRequestRequestTypeDef,
     GetProtocolsListRequestRequestTypeDef,
     ProtocolsListDataOutputTypeDef,
     GetResourceSetRequestRequestTypeDef,
     ResourceSetOutputTypeDef,
     GetThirdPartyFirewallAssociationStatusRequestRequestTypeDef,
     GetViolationDetailsRequestRequestTypeDef,
     PaginatorConfigTypeDef,
@@ -445,17 +445,15 @@
     NetworkFirewallMissingSubnetViolationTypeDef,
     StatefulEngineOptionsTypeDef,
     StatelessRuleGroupTypeDef,
     NetworkFirewallPolicyTypeDef,
     NetworkFirewallStatefulRuleGroupOverrideTypeDef,
     ThirdPartyFirewallPolicyTypeDef,
     ResourceTagTypeDef,
-    ProtocolsListDataTypeDef,
     PutNotificationChannelRequestRequestTypeDef,
-    ResourceSetTypeDef,
     ThirdPartyFirewallMissingExpectedRouteTableViolationTypeDef,
     ThirdPartyFirewallMissingFirewallViolationTypeDef,
     ThirdPartyFirewallMissingSubnetViolationTypeDef,
     SecurityGroupRuleDescriptionTypeDef,
     UntagResourceRequestRequestTypeDef,
     EC2AssociateRouteTableActionTypeDef,
     EC2CopyRouteTableActionTypeDef,
@@ -465,14 +463,17 @@
     EC2ReplaceRouteActionTypeDef,
     EC2ReplaceRouteTableAssociationActionTypeDef,
     AdminScopeOutputTypeDef,
     AdminScopeTypeDef,
     AppsListDataOutputTypeDef,
     AppsListDataSummaryTypeDef,
     AppsListDataTypeDef,
+    GetProtectionStatusRequestRequestTypeDef,
+    ProtocolsListDataTypeDef,
+    ResourceSetTypeDef,
     AssociateThirdPartyFirewallResponseTypeDef,
     DisassociateThirdPartyFirewallResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetAdminAccountResponseTypeDef,
     GetNotificationChannelResponseTypeDef,
     GetProtectionStatusResponseTypeDef,
     GetThirdPartyFirewallAssociationStatusResponseTypeDef,
@@ -509,45 +510,50 @@
     NetworkFirewallInternetTrafficNotInspectedViolationTypeDef,
     NetworkFirewallInvalidRouteConfigurationViolationTypeDef,
     NetworkFirewallUnexpectedFirewallRoutesViolationTypeDef,
     NetworkFirewallUnexpectedGatewayRoutesViolationTypeDef,
     RouteHasOutOfScopeEndpointViolationTypeDef,
     StatefulRuleGroupTypeDef,
     PolicyOptionTypeDef,
-    PutProtocolsListRequestRequestTypeDef,
-    PutResourceSetRequestRequestTypeDef,
     SecurityGroupRemediationActionTypeDef,
     RemediationActionTypeDef,
     GetAdminScopeResponseTypeDef,
+    AdminScopeUnionTypeDef,
     PutAdminAccountRequestRequestTypeDef,
     GetAppsListResponseTypeDef,
     PutAppsListResponseTypeDef,
     ListAppsListsResponseTypeDef,
+    AppsListDataUnionTypeDef,
     PutAppsListRequestRequestTypeDef,
+    ProtocolsListDataUnionTypeDef,
+    PutProtocolsListRequestRequestTypeDef,
+    PutResourceSetRequestRequestTypeDef,
+    ResourceSetUnionTypeDef,
     GetComplianceDetailResponseTypeDef,
     ListComplianceStatusResponseTypeDef,
     NetworkFirewallPolicyDescriptionTypeDef,
     SecurityServicePolicyDataTypeDef,
     AwsVPCSecurityGroupViolationTypeDef,
     RemediationActionWithOrderTypeDef,
     NetworkFirewallPolicyModifiedViolationTypeDef,
     PolicyOutputTypeDef,
     PolicyTypeDef,
     PossibleRemediationActionTypeDef,
     GetPolicyResponseTypeDef,
     PutPolicyResponseTypeDef,
+    PolicyUnionTypeDef,
     PutPolicyRequestRequestTypeDef,
     PossibleRemediationActionsTypeDef,
     ResourceViolationTypeDef,
     ViolationDetailTypeDef,
     GetViolationDetailsResponseTypeDef,
 )
 
 
-def get_structure() -> AccountScopeOutputTypeDef:
+def get_value() -> AccountScopeOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-fms-1.28.15.post1/mypy_boto3_fms.egg-info/SOURCES.txt` & `mypy-boto3-fms-1.28.16/mypy_boto3_fms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fms-1.28.15.post1/setup.py` & `mypy-boto3-fms-1.28.16/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-fms",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_fms"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.FMS 1.28.15 service generated with mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.FMS 1.28.16 service generated with mypy-boto3-builder 7.17.1"
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
-    keywords="boto3 fms type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 fms type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_fms": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

