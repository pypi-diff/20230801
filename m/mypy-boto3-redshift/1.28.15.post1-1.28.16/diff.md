# Comparing `tmp/mypy-boto3-redshift-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-redshift-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-redshift-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:58 2023, max compression
+gzip compressed data, was "mypy-boto3-redshift-1.28.16.tar", last modified: Tue Aug  1 11:37:38 2023, max compression
```

## Comparing `mypy-boto3-redshift-1.28.15.post1.tar` & `mypy-boto3-redshift-1.28.16.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:58.529356 mypy-boto3-redshift-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:56:37.000000 mypy-boto3-redshift-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    36924 2023-07-29 10:03:58.521356 mypy-boto3-redshift-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    35427 2023-07-29 09:56:37.000000 mypy-boto3-redshift-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:58.521356 mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift/
--rw-r--r--   0 runner    (1001) docker     (123)     9933 2023-07-29 09:56:37.000000 mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9932 2023-07-29 09:56:37.000000 mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-29 09:56:37.000000 mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   115226 2023-07-29 09:56:39.000000 mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   115059 2023-07-29 09:56:38.000000 mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17351 2023-07-29 09:56:40.000000 mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    17349 2023-07-29 09:56:39.000000 mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    43550 2023-07-29 09:56:39.000000 mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    43515 2023-07-29 09:56:39.000000 mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:56:37.000000 mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   134047 2023-07-29 09:56:47.000000 mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   133928 2023-07-29 09:56:41.000000 mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:56:37.000000 mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-07-29 09:56:39.000000 mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-07-29 09:56:39.000000 mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:58.521356 mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    36924 2023-07-29 10:03:58.000000 mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-29 10:03:58.000000 mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:58.000000 mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:58.000000 mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:58.000000 mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-29 10:03:58.000000 mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:58.529356 mypy-boto3-redshift-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-29 09:56:37.000000 mypy-boto3-redshift-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:38.240776 mypy-boto3-redshift-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:29:58.000000 mypy-boto3-redshift-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    36936 2023-08-01 11:37:38.232776 mypy-boto3-redshift-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    35448 2023-08-01 11:29:58.000000 mypy-boto3-redshift-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:38.232776 mypy-boto3-redshift-1.28.16/mypy_boto3_redshift/
+-rw-r--r--   0 runner    (1001) docker     (123)     9933 2023-08-01 11:29:58.000000 mypy-boto3-redshift-1.28.16/mypy_boto3_redshift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9932 2023-08-01 11:29:58.000000 mypy-boto3-redshift-1.28.16/mypy_boto3_redshift/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-08-01 11:29:58.000000 mypy-boto3-redshift-1.28.16/mypy_boto3_redshift/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   115163 2023-08-01 11:29:59.000000 mypy-boto3-redshift-1.28.16/mypy_boto3_redshift/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   114996 2023-08-01 11:29:59.000000 mypy-boto3-redshift-1.28.16/mypy_boto3_redshift/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17351 2023-08-01 11:30:00.000000 mypy-boto3-redshift-1.28.16/mypy_boto3_redshift/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17349 2023-08-01 11:30:00.000000 mypy-boto3-redshift-1.28.16/mypy_boto3_redshift/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    43511 2023-08-01 11:30:00.000000 mypy-boto3-redshift-1.28.16/mypy_boto3_redshift/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43476 2023-08-01 11:30:00.000000 mypy-boto3-redshift-1.28.16/mypy_boto3_redshift/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:29:58.000000 mypy-boto3-redshift-1.28.16/mypy_boto3_redshift/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   134029 2023-08-01 11:30:08.000000 mypy-boto3-redshift-1.28.16/mypy_boto3_redshift/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   133910 2023-08-01 11:30:06.000000 mypy-boto3-redshift-1.28.16/mypy_boto3_redshift/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:29:58.000000 mypy-boto3-redshift-1.28.16/mypy_boto3_redshift/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-08-01 11:30:00.000000 mypy-boto3-redshift-1.28.16/mypy_boto3_redshift/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5293 2023-08-01 11:30:00.000000 mypy-boto3-redshift-1.28.16/mypy_boto3_redshift/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:38.232776 mypy-boto3-redshift-1.28.16/mypy_boto3_redshift.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    36936 2023-08-01 11:37:37.000000 mypy-boto3-redshift-1.28.16/mypy_boto3_redshift.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-08-01 11:37:38.000000 mypy-boto3-redshift-1.28.16/mypy_boto3_redshift.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:37.000000 mypy-boto3-redshift-1.28.16/mypy_boto3_redshift.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:37.000000 mypy-boto3-redshift-1.28.16/mypy_boto3_redshift.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:37.000000 mypy-boto3-redshift-1.28.16/mypy_boto3_redshift.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-01 11:37:37.000000 mypy-boto3-redshift-1.28.16/mypy_boto3_redshift.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:38.240776 mypy-boto3-redshift-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-08-01 11:29:58.000000 mypy-boto3-redshift-1.28.16/setup.py
```

### Comparing `mypy-boto3-redshift-1.28.15.post1/LICENSE` & `mypy-boto3-redshift-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-1.28.15.post1/PKG-INFO` & `mypy-boto3-redshift-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-redshift
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Redshift 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.Redshift 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 redshift type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 redshift type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-redshift.svg?color=blue)](https://pypi.org/project/mypy-boto3-redshift)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-redshift)](https://pepy.tech/project/mypy-boto3-redshift)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Redshift 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift)
+[boto3.Redshift 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift)
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
 [mypy-boto3-redshift docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/).
 
 See how it helps to find and fix potential bugs:
 
@@ -75,15 +75,15 @@
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
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
@@ -528,20 +528,20 @@
 )
 
 
 def check_value(value: ActionTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_redshift.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_redshift.type_defs import (
     AcceptReservedNodeExchangeInputMessageRequestTypeDef,
     ResponseMetadataTypeDef,
     AttributeValueTargetTypeDef,
     AccountWithRestoreAccessTypeDef,
@@ -577,14 +577,15 @@
     RestoreStatusTypeDef,
     VpcSecurityGroupMembershipTypeDef,
     ClusterVersionTypeDef,
     CopyClusterSnapshotMessageRequestTypeDef,
     CreateAuthenticationProfileMessageRequestTypeDef,
     CreateCustomDomainAssociationMessageRequestTypeDef,
     CreateEndpointAccessMessageRequestTypeDef,
+    TimestampTypeDef,
     DataShareAssociationTypeDef,
     DeauthorizeDataShareMessageRequestTypeDef,
     DeleteAuthenticationProfileMessageRequestTypeDef,
     DeleteClusterMessageRequestTypeDef,
     DeleteClusterParameterGroupMessageRequestTypeDef,
     DeleteClusterSecurityGroupMessageRequestTypeDef,
     DeleteClusterSnapshotMessageRequestTypeDef,
@@ -617,15 +618,14 @@
     DescribeDataSharesForProducerMessageRequestTypeDef,
     DescribeDataSharesMessageRequestTypeDef,
     DescribeDefaultClusterParametersMessageRequestTypeDef,
     DescribeEndpointAccessMessageRequestTypeDef,
     DescribeEndpointAuthorizationMessageRequestTypeDef,
     DescribeEventCategoriesMessageRequestTypeDef,
     DescribeEventSubscriptionsMessageRequestTypeDef,
-    DescribeEventsMessageRequestTypeDef,
     DescribeHsmClientCertificatesMessageRequestTypeDef,
     DescribeHsmConfigurationsMessageRequestTypeDef,
     DescribeLoggingStatusMessageRequestTypeDef,
     NodeConfigurationOptionsFilterTypeDef,
     DescribeOrderableClusterOptionsMessageRequestTypeDef,
     DescribePartnersInputMessageRequestTypeDef,
     PartnerIntegrationInfoTypeDef,
@@ -651,15 +651,14 @@
     GetClusterCredentialsWithIAMMessageRequestTypeDef,
     GetReservedNodeExchangeConfigurationOptionsInputMessageRequestTypeDef,
     GetReservedNodeExchangeOfferingsInputMessageRequestTypeDef,
     ModifyAquaInputMessageRequestTypeDef,
     ModifyAuthenticationProfileMessageRequestTypeDef,
     ModifyClusterDbRevisionMessageRequestTypeDef,
     ModifyClusterIamRolesMessageRequestTypeDef,
-    ModifyClusterMaintenanceMessageRequestTypeDef,
     ModifyClusterMessageRequestTypeDef,
     ModifyClusterSnapshotMessageRequestTypeDef,
     ModifyClusterSnapshotScheduleMessageRequestTypeDef,
     ModifyClusterSubnetGroupMessageRequestTypeDef,
     ModifyCustomDomainAssociationMessageRequestTypeDef,
     ModifyEndpointAccessMessageRequestTypeDef,
     ModifyEventSubscriptionMessageRequestTypeDef,
@@ -739,14 +738,16 @@
     SnapshotScheduleTypeDef,
     SnapshotTypeDef,
     TaggedResourceTypeDef,
     UsageLimitResponseTypeDef,
     UsageLimitTypeDef,
     DescribeReservedNodeExchangeStatusOutputMessageTypeDef,
     ClusterVersionsMessageTypeDef,
+    DescribeEventsMessageRequestTypeDef,
+    ModifyClusterMaintenanceMessageRequestTypeDef,
     DataShareResponseTypeDef,
     DataShareTypeDef,
     DescribeClusterDbRevisionsMessageDescribeClusterDbRevisionsPaginateTypeDef,
     DescribeClusterParameterGroupsMessageDescribeClusterParameterGroupsPaginateTypeDef,
     DescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef,
     DescribeClusterSecurityGroupsMessageDescribeClusterSecurityGroupsPaginateTypeDef,
     DescribeClusterSubnetGroupsMessageDescribeClusterSubnetGroupsPaginateTypeDef,
@@ -872,15 +873,15 @@
     ResizeClusterResultTypeDef,
     RestoreFromClusterSnapshotResultTypeDef,
     ResumeClusterResultTypeDef,
     RotateEncryptionKeyResultTypeDef,
 )
 
 
-def get_structure() -> AcceptReservedNodeExchangeInputMessageRequestTypeDef:
+def get_value() -> AcceptReservedNodeExchangeInputMessageRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-redshift-1.28.15.post1/README.md` & `mypy-boto3-redshift-1.28.16/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-redshift.svg?color=blue)](https://pypi.org/project/mypy-boto3-redshift)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-redshift)](https://pepy.tech/project/mypy-boto3-redshift)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Redshift 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift)
+[boto3.Redshift 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift)
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
 [mypy-boto3-redshift docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/).
 
 See how it helps to find and fix potential bugs:
 
@@ -43,15 +43,15 @@
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
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
@@ -496,20 +496,20 @@
 )
 
 
 def check_value(value: ActionTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_redshift.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_redshift.type_defs import (
     AcceptReservedNodeExchangeInputMessageRequestTypeDef,
     ResponseMetadataTypeDef,
     AttributeValueTargetTypeDef,
     AccountWithRestoreAccessTypeDef,
@@ -545,14 +545,15 @@
     RestoreStatusTypeDef,
     VpcSecurityGroupMembershipTypeDef,
     ClusterVersionTypeDef,
     CopyClusterSnapshotMessageRequestTypeDef,
     CreateAuthenticationProfileMessageRequestTypeDef,
     CreateCustomDomainAssociationMessageRequestTypeDef,
     CreateEndpointAccessMessageRequestTypeDef,
+    TimestampTypeDef,
     DataShareAssociationTypeDef,
     DeauthorizeDataShareMessageRequestTypeDef,
     DeleteAuthenticationProfileMessageRequestTypeDef,
     DeleteClusterMessageRequestTypeDef,
     DeleteClusterParameterGroupMessageRequestTypeDef,
     DeleteClusterSecurityGroupMessageRequestTypeDef,
     DeleteClusterSnapshotMessageRequestTypeDef,
@@ -585,15 +586,14 @@
     DescribeDataSharesForProducerMessageRequestTypeDef,
     DescribeDataSharesMessageRequestTypeDef,
     DescribeDefaultClusterParametersMessageRequestTypeDef,
     DescribeEndpointAccessMessageRequestTypeDef,
     DescribeEndpointAuthorizationMessageRequestTypeDef,
     DescribeEventCategoriesMessageRequestTypeDef,
     DescribeEventSubscriptionsMessageRequestTypeDef,
-    DescribeEventsMessageRequestTypeDef,
     DescribeHsmClientCertificatesMessageRequestTypeDef,
     DescribeHsmConfigurationsMessageRequestTypeDef,
     DescribeLoggingStatusMessageRequestTypeDef,
     NodeConfigurationOptionsFilterTypeDef,
     DescribeOrderableClusterOptionsMessageRequestTypeDef,
     DescribePartnersInputMessageRequestTypeDef,
     PartnerIntegrationInfoTypeDef,
@@ -619,15 +619,14 @@
     GetClusterCredentialsWithIAMMessageRequestTypeDef,
     GetReservedNodeExchangeConfigurationOptionsInputMessageRequestTypeDef,
     GetReservedNodeExchangeOfferingsInputMessageRequestTypeDef,
     ModifyAquaInputMessageRequestTypeDef,
     ModifyAuthenticationProfileMessageRequestTypeDef,
     ModifyClusterDbRevisionMessageRequestTypeDef,
     ModifyClusterIamRolesMessageRequestTypeDef,
-    ModifyClusterMaintenanceMessageRequestTypeDef,
     ModifyClusterMessageRequestTypeDef,
     ModifyClusterSnapshotMessageRequestTypeDef,
     ModifyClusterSnapshotScheduleMessageRequestTypeDef,
     ModifyClusterSubnetGroupMessageRequestTypeDef,
     ModifyCustomDomainAssociationMessageRequestTypeDef,
     ModifyEndpointAccessMessageRequestTypeDef,
     ModifyEventSubscriptionMessageRequestTypeDef,
@@ -707,14 +706,16 @@
     SnapshotScheduleTypeDef,
     SnapshotTypeDef,
     TaggedResourceTypeDef,
     UsageLimitResponseTypeDef,
     UsageLimitTypeDef,
     DescribeReservedNodeExchangeStatusOutputMessageTypeDef,
     ClusterVersionsMessageTypeDef,
+    DescribeEventsMessageRequestTypeDef,
+    ModifyClusterMaintenanceMessageRequestTypeDef,
     DataShareResponseTypeDef,
     DataShareTypeDef,
     DescribeClusterDbRevisionsMessageDescribeClusterDbRevisionsPaginateTypeDef,
     DescribeClusterParameterGroupsMessageDescribeClusterParameterGroupsPaginateTypeDef,
     DescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef,
     DescribeClusterSecurityGroupsMessageDescribeClusterSecurityGroupsPaginateTypeDef,
     DescribeClusterSubnetGroupsMessageDescribeClusterSubnetGroupsPaginateTypeDef,
@@ -840,15 +841,15 @@
     ResizeClusterResultTypeDef,
     RestoreFromClusterSnapshotResultTypeDef,
     ResumeClusterResultTypeDef,
     RotateEncryptionKeyResultTypeDef,
 )
 
 
-def get_structure() -> AcceptReservedNodeExchangeInputMessageRequestTypeDef:
+def get_value() -> AcceptReservedNodeExchangeInputMessageRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift/__init__.py` & `mypy-boto3-redshift-1.28.16/mypy_boto3_redshift/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift/__init__.pyi` & `mypy-boto3-redshift-1.28.16/mypy_boto3_redshift/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift/__main__.py` & `mypy-boto3-redshift-1.28.16/mypy_boto3_redshift/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Redshift 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.Redshift 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift\nOther"
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

### Comparing `mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift/client.py` & `mypy-boto3-redshift-1.28.16/mypy_boto3_redshift/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_redshift.client import RedshiftClient
 
     session = Session()
     client: RedshiftClient = session.client("redshift")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     ActionTypeType,
     AquaConfigurationStatusType,
     DataShareStatusForConsumerType,
@@ -164,14 +163,15 @@
     SnapshotCopyGrantMessageTypeDef,
     SnapshotMessageTypeDef,
     SnapshotScheduleResponseTypeDef,
     SnapshotSortingEntityTypeDef,
     TableRestoreStatusMessageTypeDef,
     TaggedResourceListMessageTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
     TrackListMessageTypeDef,
     UsageLimitListTypeDef,
     UsageLimitResponseTypeDef,
 )
 from .waiter import (
     ClusterAvailableWaiter,
     ClusterDeletedWaiter,
@@ -689,16 +689,16 @@
         self,
         *,
         ScheduledActionName: str,
         TargetAction: ScheduledActionTypeTypeDef,
         Schedule: str,
         IamRole: str,
         ScheduledActionDescription: str = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         Enable: bool = ...
     ) -> ScheduledActionResponseTypeDef:
         """
         Creates a scheduled action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.create_scheduled_action)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#create_scheduled_action)
@@ -1022,16 +1022,16 @@
     def describe_cluster_snapshots(
         self,
         *,
         ClusterIdentifier: str = ...,
         SnapshotIdentifier: str = ...,
         SnapshotArn: str = ...,
         SnapshotType: str = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         OwnerAccount: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
         ClusterExists: bool = ...,
         SortingEntities: Sequence[SnapshotSortingEntityTypeDef] = ...
@@ -1232,16 +1232,16 @@
         """
 
     def describe_events(
         self,
         *,
         SourceIdentifier: str = ...,
         SourceType: SourceTypeType = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         Duration: int = ...,
         MaxRecords: int = ...,
         Marker: str = ...
     ) -> EventsMessageTypeDef:
         """
         Returns events related to clusters, security groups, snapshots, and parameter
         groups for the past 14 days.
@@ -1388,16 +1388,16 @@
         """
 
     def describe_scheduled_actions(
         self,
         *,
         ScheduledActionName: str = ...,
         TargetActionType: ScheduledActionTypeValuesType = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         Active: bool = ...,
         Filters: Sequence[ScheduledActionFilterTypeDef] = ...,
         Marker: str = ...,
         MaxRecords: int = ...
     ) -> ScheduledActionsMessageTypeDef:
         """
         Describes properties of scheduled actions.
@@ -1727,16 +1727,16 @@
 
     def modify_cluster_maintenance(
         self,
         *,
         ClusterIdentifier: str,
         DeferMaintenance: bool = ...,
         DeferMaintenanceIdentifier: str = ...,
-        DeferMaintenanceStartTime: Union[datetime, str] = ...,
-        DeferMaintenanceEndTime: Union[datetime, str] = ...,
+        DeferMaintenanceStartTime: TimestampTypeDef = ...,
+        DeferMaintenanceEndTime: TimestampTypeDef = ...,
         DeferMaintenanceDuration: int = ...
     ) -> ModifyClusterMaintenanceResultTypeDef:
         """
         Modifies the maintenance settings of a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_cluster_maintenance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#modify_cluster_maintenance)
@@ -1836,16 +1836,16 @@
         self,
         *,
         ScheduledActionName: str,
         TargetAction: ScheduledActionTypeTypeDef = ...,
         Schedule: str = ...,
         IamRole: str = ...,
         ScheduledActionDescription: str = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         Enable: bool = ...
     ) -> ScheduledActionResponseTypeDef:
         """
         Modifies a scheduled action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_scheduled_action)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#modify_scheduled_action)
```

### Comparing `mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift/client.pyi` & `mypy-boto3-redshift-1.28.16/mypy_boto3_redshift/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_redshift.client import RedshiftClient
 
     session = Session()
     client: RedshiftClient = session.client("redshift")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     ActionTypeType,
     AquaConfigurationStatusType,
     DataShareStatusForConsumerType,
@@ -164,14 +163,15 @@
     SnapshotCopyGrantMessageTypeDef,
     SnapshotMessageTypeDef,
     SnapshotScheduleResponseTypeDef,
     SnapshotSortingEntityTypeDef,
     TableRestoreStatusMessageTypeDef,
     TaggedResourceListMessageTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
     TrackListMessageTypeDef,
     UsageLimitListTypeDef,
     UsageLimitResponseTypeDef,
 )
 from .waiter import (
     ClusterAvailableWaiter,
     ClusterDeletedWaiter,
@@ -660,16 +660,16 @@
         self,
         *,
         ScheduledActionName: str,
         TargetAction: ScheduledActionTypeTypeDef,
         Schedule: str,
         IamRole: str,
         ScheduledActionDescription: str = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         Enable: bool = ...
     ) -> ScheduledActionResponseTypeDef:
         """
         Creates a scheduled action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.create_scheduled_action)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#create_scheduled_action)
@@ -964,16 +964,16 @@
     def describe_cluster_snapshots(
         self,
         *,
         ClusterIdentifier: str = ...,
         SnapshotIdentifier: str = ...,
         SnapshotArn: str = ...,
         SnapshotType: str = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         OwnerAccount: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
         ClusterExists: bool = ...,
         SortingEntities: Sequence[SnapshotSortingEntityTypeDef] = ...
@@ -1160,16 +1160,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#describe_event_subscriptions)
         """
     def describe_events(
         self,
         *,
         SourceIdentifier: str = ...,
         SourceType: SourceTypeType = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         Duration: int = ...,
         MaxRecords: int = ...,
         Marker: str = ...
     ) -> EventsMessageTypeDef:
         """
         Returns events related to clusters, security groups, snapshots, and parameter
         groups for the past 14 days.
@@ -1305,16 +1305,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#describe_resize)
         """
     def describe_scheduled_actions(
         self,
         *,
         ScheduledActionName: str = ...,
         TargetActionType: ScheduledActionTypeValuesType = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         Active: bool = ...,
         Filters: Sequence[ScheduledActionFilterTypeDef] = ...,
         Marker: str = ...,
         MaxRecords: int = ...
     ) -> ScheduledActionsMessageTypeDef:
         """
         Describes properties of scheduled actions.
@@ -1622,16 +1622,16 @@
         """
     def modify_cluster_maintenance(
         self,
         *,
         ClusterIdentifier: str,
         DeferMaintenance: bool = ...,
         DeferMaintenanceIdentifier: str = ...,
-        DeferMaintenanceStartTime: Union[datetime, str] = ...,
-        DeferMaintenanceEndTime: Union[datetime, str] = ...,
+        DeferMaintenanceStartTime: TimestampTypeDef = ...,
+        DeferMaintenanceEndTime: TimestampTypeDef = ...,
         DeferMaintenanceDuration: int = ...
     ) -> ModifyClusterMaintenanceResultTypeDef:
         """
         Modifies the maintenance settings of a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_cluster_maintenance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#modify_cluster_maintenance)
@@ -1723,16 +1723,16 @@
         self,
         *,
         ScheduledActionName: str,
         TargetAction: ScheduledActionTypeTypeDef = ...,
         Schedule: str = ...,
         IamRole: str = ...,
         ScheduledActionDescription: str = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         Enable: bool = ...
     ) -> ScheduledActionResponseTypeDef:
         """
         Modifies a scheduled action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_scheduled_action)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#modify_scheduled_action)
```

### Comparing `mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift/literals.py` & `mypy-boto3-redshift-1.28.16/mypy_boto3_redshift/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift/literals.pyi` & `mypy-boto3-redshift-1.28.16/mypy_boto3_redshift/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift/paginator.py` & `mypy-boto3-redshift-1.28.16/mypy_boto3_redshift/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,16 +79,15 @@
     describe_table_restore_status_paginator: DescribeTableRestoreStatusPaginator = client.get_paginator("describe_table_restore_status")
     describe_tags_paginator: DescribeTagsPaginator = client.get_paginator("describe_tags")
     describe_usage_limits_paginator: DescribeUsageLimitsPaginator = client.get_paginator("describe_usage_limits")
     get_reserved_node_exchange_configuration_options_paginator: GetReservedNodeExchangeConfigurationOptionsPaginator = client.get_paginator("get_reserved_node_exchange_configuration_options")
     get_reserved_node_exchange_offerings_paginator: GetReservedNodeExchangeOfferingsPaginator = client.get_paginator("get_reserved_node_exchange_offerings")
     ```
 """
-from datetime import datetime
-from typing import Generic, Iterator, Sequence, TypeVar, Union
+from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import (
     ActionTypeType,
     DataShareStatusForConsumerType,
     DataShareStatusForProducerType,
@@ -129,14 +128,15 @@
     ScheduledActionFilterTypeDef,
     ScheduledActionsMessageTypeDef,
     SnapshotCopyGrantMessageTypeDef,
     SnapshotMessageTypeDef,
     SnapshotSortingEntityTypeDef,
     TableRestoreStatusMessageTypeDef,
     TaggedResourceListMessageTypeDef,
+    TimestampTypeDef,
     TrackListMessageTypeDef,
     UsageLimitListTypeDef,
 )
 
 __all__ = (
     "DescribeClusterDbRevisionsPaginator",
     "DescribeClusterParameterGroupsPaginator",
@@ -267,16 +267,16 @@
     def paginate(
         self,
         *,
         ClusterIdentifier: str = ...,
         SnapshotIdentifier: str = ...,
         SnapshotArn: str = ...,
         SnapshotType: str = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         OwnerAccount: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
         ClusterExists: bool = ...,
         SortingEntities: Sequence[SnapshotSortingEntityTypeDef] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SnapshotMessageTypeDef]:
@@ -515,16 +515,16 @@
     """
 
     def paginate(
         self,
         *,
         SourceIdentifier: str = ...,
         SourceType: SourceTypeType = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         Duration: int = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[EventsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describeeventspaginator)
         """
@@ -668,16 +668,16 @@
     """
 
     def paginate(
         self,
         *,
         ScheduledActionName: str = ...,
         TargetActionType: ScheduledActionTypeValuesType = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         Active: bool = ...,
         Filters: Sequence[ScheduledActionFilterTypeDef] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ScheduledActionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeScheduledActions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describescheduledactionspaginator)
```

### Comparing `mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift/paginator.pyi` & `mypy-boto3-redshift-1.28.16/mypy_boto3_redshift/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -79,16 +79,15 @@
     describe_table_restore_status_paginator: DescribeTableRestoreStatusPaginator = client.get_paginator("describe_table_restore_status")
     describe_tags_paginator: DescribeTagsPaginator = client.get_paginator("describe_tags")
     describe_usage_limits_paginator: DescribeUsageLimitsPaginator = client.get_paginator("describe_usage_limits")
     get_reserved_node_exchange_configuration_options_paginator: GetReservedNodeExchangeConfigurationOptionsPaginator = client.get_paginator("get_reserved_node_exchange_configuration_options")
     get_reserved_node_exchange_offerings_paginator: GetReservedNodeExchangeOfferingsPaginator = client.get_paginator("get_reserved_node_exchange_offerings")
     ```
 """
-from datetime import datetime
-from typing import Generic, Iterator, Sequence, TypeVar, Union
+from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import (
     ActionTypeType,
     DataShareStatusForConsumerType,
     DataShareStatusForProducerType,
@@ -129,14 +128,15 @@
     ScheduledActionFilterTypeDef,
     ScheduledActionsMessageTypeDef,
     SnapshotCopyGrantMessageTypeDef,
     SnapshotMessageTypeDef,
     SnapshotSortingEntityTypeDef,
     TableRestoreStatusMessageTypeDef,
     TaggedResourceListMessageTypeDef,
+    TimestampTypeDef,
     TrackListMessageTypeDef,
     UsageLimitListTypeDef,
 )
 
 __all__ = (
     "DescribeClusterDbRevisionsPaginator",
     "DescribeClusterParameterGroupsPaginator",
@@ -260,16 +260,16 @@
     def paginate(
         self,
         *,
         ClusterIdentifier: str = ...,
         SnapshotIdentifier: str = ...,
         SnapshotArn: str = ...,
         SnapshotType: str = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         OwnerAccount: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
         ClusterExists: bool = ...,
         SortingEntities: Sequence[SnapshotSortingEntityTypeDef] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SnapshotMessageTypeDef]:
@@ -495,16 +495,16 @@
     """
 
     def paginate(
         self,
         *,
         SourceIdentifier: str = ...,
         SourceType: SourceTypeType = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         Duration: int = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[EventsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describeeventspaginator)
         """
@@ -640,16 +640,16 @@
     """
 
     def paginate(
         self,
         *,
         ScheduledActionName: str = ...,
         TargetActionType: ScheduledActionTypeValuesType = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         Active: bool = ...,
         Filters: Sequence[ScheduledActionFilterTypeDef] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ScheduledActionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeScheduledActions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describescheduledactionspaginator)
```

### Comparing `mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift/type_defs.py` & `mypy-boto3-redshift-1.28.16/mypy_boto3_redshift/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_redshift.type_defs import AcceptReservedNodeExchangeInputMessageRequestTypeDef
 
-    data: AcceptReservedNodeExchangeInputMessageRequestTypeDef = {...}
+    data: AcceptReservedNodeExchangeInputMessageRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -89,14 +89,15 @@
     "RestoreStatusTypeDef",
     "VpcSecurityGroupMembershipTypeDef",
     "ClusterVersionTypeDef",
     "CopyClusterSnapshotMessageRequestTypeDef",
     "CreateAuthenticationProfileMessageRequestTypeDef",
     "CreateCustomDomainAssociationMessageRequestTypeDef",
     "CreateEndpointAccessMessageRequestTypeDef",
+    "TimestampTypeDef",
     "DataShareAssociationTypeDef",
     "DeauthorizeDataShareMessageRequestTypeDef",
     "DeleteAuthenticationProfileMessageRequestTypeDef",
     "DeleteClusterMessageRequestTypeDef",
     "DeleteClusterParameterGroupMessageRequestTypeDef",
     "DeleteClusterSecurityGroupMessageRequestTypeDef",
     "DeleteClusterSnapshotMessageRequestTypeDef",
@@ -129,15 +130,14 @@
     "DescribeDataSharesForProducerMessageRequestTypeDef",
     "DescribeDataSharesMessageRequestTypeDef",
     "DescribeDefaultClusterParametersMessageRequestTypeDef",
     "DescribeEndpointAccessMessageRequestTypeDef",
     "DescribeEndpointAuthorizationMessageRequestTypeDef",
     "DescribeEventCategoriesMessageRequestTypeDef",
     "DescribeEventSubscriptionsMessageRequestTypeDef",
-    "DescribeEventsMessageRequestTypeDef",
     "DescribeHsmClientCertificatesMessageRequestTypeDef",
     "DescribeHsmConfigurationsMessageRequestTypeDef",
     "DescribeLoggingStatusMessageRequestTypeDef",
     "NodeConfigurationOptionsFilterTypeDef",
     "DescribeOrderableClusterOptionsMessageRequestTypeDef",
     "DescribePartnersInputMessageRequestTypeDef",
     "PartnerIntegrationInfoTypeDef",
@@ -163,15 +163,14 @@
     "GetClusterCredentialsWithIAMMessageRequestTypeDef",
     "GetReservedNodeExchangeConfigurationOptionsInputMessageRequestTypeDef",
     "GetReservedNodeExchangeOfferingsInputMessageRequestTypeDef",
     "ModifyAquaInputMessageRequestTypeDef",
     "ModifyAuthenticationProfileMessageRequestTypeDef",
     "ModifyClusterDbRevisionMessageRequestTypeDef",
     "ModifyClusterIamRolesMessageRequestTypeDef",
-    "ModifyClusterMaintenanceMessageRequestTypeDef",
     "ModifyClusterMessageRequestTypeDef",
     "ModifyClusterSnapshotMessageRequestTypeDef",
     "ModifyClusterSnapshotScheduleMessageRequestTypeDef",
     "ModifyClusterSubnetGroupMessageRequestTypeDef",
     "ModifyCustomDomainAssociationMessageRequestTypeDef",
     "ModifyEndpointAccessMessageRequestTypeDef",
     "ModifyEventSubscriptionMessageRequestTypeDef",
@@ -251,14 +250,16 @@
     "SnapshotScheduleTypeDef",
     "SnapshotTypeDef",
     "TaggedResourceTypeDef",
     "UsageLimitResponseTypeDef",
     "UsageLimitTypeDef",
     "DescribeReservedNodeExchangeStatusOutputMessageTypeDef",
     "ClusterVersionsMessageTypeDef",
+    "DescribeEventsMessageRequestTypeDef",
+    "ModifyClusterMaintenanceMessageRequestTypeDef",
     "DataShareResponseTypeDef",
     "DataShareTypeDef",
     "DescribeClusterDbRevisionsMessageDescribeClusterDbRevisionsPaginateTypeDef",
     "DescribeClusterParameterGroupsMessageDescribeClusterParameterGroupsPaginateTypeDef",
     "DescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef",
     "DescribeClusterSecurityGroupsMessageDescribeClusterSecurityGroupsPaginateTypeDef",
     "DescribeClusterSubnetGroupsMessageDescribeClusterSubnetGroupsPaginateTypeDef",
@@ -895,14 +896,15 @@
 class CreateEndpointAccessMessageRequestTypeDef(
     _RequiredCreateEndpointAccessMessageRequestTypeDef,
     _OptionalCreateEndpointAccessMessageRequestTypeDef,
 ):
     pass
 
 
+TimestampTypeDef = Union[datetime, str]
 DataShareAssociationTypeDef = TypedDict(
     "DataShareAssociationTypeDef",
     {
         "ConsumerIdentifier": str,
         "Status": DataShareStatusType,
         "ConsumerRegion": str,
         "CreatedDate": datetime,
@@ -1329,28 +1331,14 @@
         "Marker": str,
         "TagKeys": Sequence[str],
         "TagValues": Sequence[str],
     },
     total=False,
 )
 
-DescribeEventsMessageRequestTypeDef = TypedDict(
-    "DescribeEventsMessageRequestTypeDef",
-    {
-        "SourceIdentifier": str,
-        "SourceType": SourceTypeType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "Duration": int,
-        "MaxRecords": int,
-        "Marker": str,
-    },
-    total=False,
-)
-
 DescribeHsmClientCertificatesMessageRequestTypeDef = TypedDict(
     "DescribeHsmClientCertificatesMessageRequestTypeDef",
     {
         "HsmClientCertificateIdentifier": str,
         "MaxRecords": int,
         "Marker": str,
         "TagKeys": Sequence[str],
@@ -1816,40 +1804,14 @@
 class ModifyClusterIamRolesMessageRequestTypeDef(
     _RequiredModifyClusterIamRolesMessageRequestTypeDef,
     _OptionalModifyClusterIamRolesMessageRequestTypeDef,
 ):
     pass
 
 
-_RequiredModifyClusterMaintenanceMessageRequestTypeDef = TypedDict(
-    "_RequiredModifyClusterMaintenanceMessageRequestTypeDef",
-    {
-        "ClusterIdentifier": str,
-    },
-)
-_OptionalModifyClusterMaintenanceMessageRequestTypeDef = TypedDict(
-    "_OptionalModifyClusterMaintenanceMessageRequestTypeDef",
-    {
-        "DeferMaintenance": bool,
-        "DeferMaintenanceIdentifier": str,
-        "DeferMaintenanceStartTime": Union[datetime, str],
-        "DeferMaintenanceEndTime": Union[datetime, str],
-        "DeferMaintenanceDuration": int,
-    },
-    total=False,
-)
-
-
-class ModifyClusterMaintenanceMessageRequestTypeDef(
-    _RequiredModifyClusterMaintenanceMessageRequestTypeDef,
-    _OptionalModifyClusterMaintenanceMessageRequestTypeDef,
-):
-    pass
-
-
 _RequiredModifyClusterMessageRequestTypeDef = TypedDict(
     "_RequiredModifyClusterMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
     },
 )
 _OptionalModifyClusterMessageRequestTypeDef = TypedDict(
@@ -3241,14 +3203,54 @@
     {
         "Marker": str,
         "ClusterVersions": List[ClusterVersionTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeEventsMessageRequestTypeDef = TypedDict(
+    "DescribeEventsMessageRequestTypeDef",
+    {
+        "SourceIdentifier": str,
+        "SourceType": SourceTypeType,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "Duration": int,
+        "MaxRecords": int,
+        "Marker": str,
+    },
+    total=False,
+)
+
+_RequiredModifyClusterMaintenanceMessageRequestTypeDef = TypedDict(
+    "_RequiredModifyClusterMaintenanceMessageRequestTypeDef",
+    {
+        "ClusterIdentifier": str,
+    },
+)
+_OptionalModifyClusterMaintenanceMessageRequestTypeDef = TypedDict(
+    "_OptionalModifyClusterMaintenanceMessageRequestTypeDef",
+    {
+        "DeferMaintenance": bool,
+        "DeferMaintenanceIdentifier": str,
+        "DeferMaintenanceStartTime": TimestampTypeDef,
+        "DeferMaintenanceEndTime": TimestampTypeDef,
+        "DeferMaintenanceDuration": int,
+    },
+    total=False,
+)
+
+
+class ModifyClusterMaintenanceMessageRequestTypeDef(
+    _RequiredModifyClusterMaintenanceMessageRequestTypeDef,
+    _OptionalModifyClusterMaintenanceMessageRequestTypeDef,
+):
+    pass
+
+
 DataShareResponseTypeDef = TypedDict(
     "DataShareResponseTypeDef",
     {
         "DataShareArn": str,
         "ProducerArn": str,
         "AllowPubliclyAccessibleConsumers": bool,
         "DataShareAssociations": List[DataShareAssociationTypeDef],
@@ -3460,16 +3462,16 @@
 )
 
 DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
     "DescribeEventsMessageDescribeEventsPaginateTypeDef",
     {
         "SourceIdentifier": str,
         "SourceType": SourceTypeType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
         "Duration": int,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeHsmClientCertificatesMessageDescribeHsmClientCertificatesPaginateTypeDef = TypedDict(
@@ -3639,16 +3641,16 @@
 DescribeClusterSnapshotsMessageDescribeClusterSnapshotsPaginateTypeDef = TypedDict(
     "DescribeClusterSnapshotsMessageDescribeClusterSnapshotsPaginateTypeDef",
     {
         "ClusterIdentifier": str,
         "SnapshotIdentifier": str,
         "SnapshotArn": str,
         "SnapshotType": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
         "OwnerAccount": str,
         "TagKeys": Sequence[str],
         "TagValues": Sequence[str],
         "ClusterExists": bool,
         "SortingEntities": Sequence[SnapshotSortingEntityTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -3658,16 +3660,16 @@
 DescribeClusterSnapshotsMessageRequestTypeDef = TypedDict(
     "DescribeClusterSnapshotsMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
         "SnapshotIdentifier": str,
         "SnapshotArn": str,
         "SnapshotType": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
         "MaxRecords": int,
         "Marker": str,
         "OwnerAccount": str,
         "TagKeys": Sequence[str],
         "TagValues": Sequence[str],
         "ClusterExists": bool,
         "SortingEntities": Sequence[SnapshotSortingEntityTypeDef],
@@ -3678,16 +3680,16 @@
 DescribeClusterSnapshotsMessageSnapshotAvailableWaitTypeDef = TypedDict(
     "DescribeClusterSnapshotsMessageSnapshotAvailableWaitTypeDef",
     {
         "ClusterIdentifier": str,
         "SnapshotIdentifier": str,
         "SnapshotArn": str,
         "SnapshotType": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
         "MaxRecords": int,
         "Marker": str,
         "OwnerAccount": str,
         "TagKeys": Sequence[str],
         "TagValues": Sequence[str],
         "ClusterExists": bool,
         "SortingEntities": Sequence[SnapshotSortingEntityTypeDef],
@@ -3799,30 +3801,30 @@
 )
 
 DescribeScheduledActionsMessageDescribeScheduledActionsPaginateTypeDef = TypedDict(
     "DescribeScheduledActionsMessageDescribeScheduledActionsPaginateTypeDef",
     {
         "ScheduledActionName": str,
         "TargetActionType": ScheduledActionTypeValuesType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
         "Active": bool,
         "Filters": Sequence[ScheduledActionFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeScheduledActionsMessageRequestTypeDef = TypedDict(
     "DescribeScheduledActionsMessageRequestTypeDef",
     {
         "ScheduledActionName": str,
         "TargetActionType": ScheduledActionTypeValuesType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
         "Active": bool,
         "Filters": Sequence[ScheduledActionFilterTypeDef],
         "Marker": str,
         "MaxRecords": int,
     },
     total=False,
 )
@@ -4331,16 +4333,16 @@
         "IamRole": str,
     },
 )
 _OptionalCreateScheduledActionMessageRequestTypeDef = TypedDict(
     "_OptionalCreateScheduledActionMessageRequestTypeDef",
     {
         "ScheduledActionDescription": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
         "Enable": bool,
     },
     total=False,
 )
 
 
 class CreateScheduledActionMessageRequestTypeDef(
@@ -4359,16 +4361,16 @@
 _OptionalModifyScheduledActionMessageRequestTypeDef = TypedDict(
     "_OptionalModifyScheduledActionMessageRequestTypeDef",
     {
         "TargetAction": ScheduledActionTypeTypeDef,
         "Schedule": str,
         "IamRole": str,
         "ScheduledActionDescription": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
         "Enable": bool,
     },
     total=False,
 )
 
 
 class ModifyScheduledActionMessageRequestTypeDef(
```

### Comparing `mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift/type_defs.pyi` & `mypy-boto3-redshift-1.28.16/mypy_boto3_redshift/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_redshift.type_defs import AcceptReservedNodeExchangeInputMessageRequestTypeDef
 
-    data: AcceptReservedNodeExchangeInputMessageRequestTypeDef = {...}
+    data: AcceptReservedNodeExchangeInputMessageRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -88,14 +88,15 @@
     "RestoreStatusTypeDef",
     "VpcSecurityGroupMembershipTypeDef",
     "ClusterVersionTypeDef",
     "CopyClusterSnapshotMessageRequestTypeDef",
     "CreateAuthenticationProfileMessageRequestTypeDef",
     "CreateCustomDomainAssociationMessageRequestTypeDef",
     "CreateEndpointAccessMessageRequestTypeDef",
+    "TimestampTypeDef",
     "DataShareAssociationTypeDef",
     "DeauthorizeDataShareMessageRequestTypeDef",
     "DeleteAuthenticationProfileMessageRequestTypeDef",
     "DeleteClusterMessageRequestTypeDef",
     "DeleteClusterParameterGroupMessageRequestTypeDef",
     "DeleteClusterSecurityGroupMessageRequestTypeDef",
     "DeleteClusterSnapshotMessageRequestTypeDef",
@@ -128,15 +129,14 @@
     "DescribeDataSharesForProducerMessageRequestTypeDef",
     "DescribeDataSharesMessageRequestTypeDef",
     "DescribeDefaultClusterParametersMessageRequestTypeDef",
     "DescribeEndpointAccessMessageRequestTypeDef",
     "DescribeEndpointAuthorizationMessageRequestTypeDef",
     "DescribeEventCategoriesMessageRequestTypeDef",
     "DescribeEventSubscriptionsMessageRequestTypeDef",
-    "DescribeEventsMessageRequestTypeDef",
     "DescribeHsmClientCertificatesMessageRequestTypeDef",
     "DescribeHsmConfigurationsMessageRequestTypeDef",
     "DescribeLoggingStatusMessageRequestTypeDef",
     "NodeConfigurationOptionsFilterTypeDef",
     "DescribeOrderableClusterOptionsMessageRequestTypeDef",
     "DescribePartnersInputMessageRequestTypeDef",
     "PartnerIntegrationInfoTypeDef",
@@ -162,15 +162,14 @@
     "GetClusterCredentialsWithIAMMessageRequestTypeDef",
     "GetReservedNodeExchangeConfigurationOptionsInputMessageRequestTypeDef",
     "GetReservedNodeExchangeOfferingsInputMessageRequestTypeDef",
     "ModifyAquaInputMessageRequestTypeDef",
     "ModifyAuthenticationProfileMessageRequestTypeDef",
     "ModifyClusterDbRevisionMessageRequestTypeDef",
     "ModifyClusterIamRolesMessageRequestTypeDef",
-    "ModifyClusterMaintenanceMessageRequestTypeDef",
     "ModifyClusterMessageRequestTypeDef",
     "ModifyClusterSnapshotMessageRequestTypeDef",
     "ModifyClusterSnapshotScheduleMessageRequestTypeDef",
     "ModifyClusterSubnetGroupMessageRequestTypeDef",
     "ModifyCustomDomainAssociationMessageRequestTypeDef",
     "ModifyEndpointAccessMessageRequestTypeDef",
     "ModifyEventSubscriptionMessageRequestTypeDef",
@@ -250,14 +249,16 @@
     "SnapshotScheduleTypeDef",
     "SnapshotTypeDef",
     "TaggedResourceTypeDef",
     "UsageLimitResponseTypeDef",
     "UsageLimitTypeDef",
     "DescribeReservedNodeExchangeStatusOutputMessageTypeDef",
     "ClusterVersionsMessageTypeDef",
+    "DescribeEventsMessageRequestTypeDef",
+    "ModifyClusterMaintenanceMessageRequestTypeDef",
     "DataShareResponseTypeDef",
     "DataShareTypeDef",
     "DescribeClusterDbRevisionsMessageDescribeClusterDbRevisionsPaginateTypeDef",
     "DescribeClusterParameterGroupsMessageDescribeClusterParameterGroupsPaginateTypeDef",
     "DescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef",
     "DescribeClusterSecurityGroupsMessageDescribeClusterSecurityGroupsPaginateTypeDef",
     "DescribeClusterSubnetGroupsMessageDescribeClusterSubnetGroupsPaginateTypeDef",
@@ -878,14 +879,15 @@
 
 class CreateEndpointAccessMessageRequestTypeDef(
     _RequiredCreateEndpointAccessMessageRequestTypeDef,
     _OptionalCreateEndpointAccessMessageRequestTypeDef,
 ):
     pass
 
+TimestampTypeDef = Union[datetime, str]
 DataShareAssociationTypeDef = TypedDict(
     "DataShareAssociationTypeDef",
     {
         "ConsumerIdentifier": str,
         "Status": DataShareStatusType,
         "ConsumerRegion": str,
         "CreatedDate": datetime,
@@ -1302,28 +1304,14 @@
         "Marker": str,
         "TagKeys": Sequence[str],
         "TagValues": Sequence[str],
     },
     total=False,
 )
 
-DescribeEventsMessageRequestTypeDef = TypedDict(
-    "DescribeEventsMessageRequestTypeDef",
-    {
-        "SourceIdentifier": str,
-        "SourceType": SourceTypeType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "Duration": int,
-        "MaxRecords": int,
-        "Marker": str,
-    },
-    total=False,
-)
-
 DescribeHsmClientCertificatesMessageRequestTypeDef = TypedDict(
     "DescribeHsmClientCertificatesMessageRequestTypeDef",
     {
         "HsmClientCertificateIdentifier": str,
         "MaxRecords": int,
         "Marker": str,
         "TagKeys": Sequence[str],
@@ -1771,38 +1759,14 @@
 
 class ModifyClusterIamRolesMessageRequestTypeDef(
     _RequiredModifyClusterIamRolesMessageRequestTypeDef,
     _OptionalModifyClusterIamRolesMessageRequestTypeDef,
 ):
     pass
 
-_RequiredModifyClusterMaintenanceMessageRequestTypeDef = TypedDict(
-    "_RequiredModifyClusterMaintenanceMessageRequestTypeDef",
-    {
-        "ClusterIdentifier": str,
-    },
-)
-_OptionalModifyClusterMaintenanceMessageRequestTypeDef = TypedDict(
-    "_OptionalModifyClusterMaintenanceMessageRequestTypeDef",
-    {
-        "DeferMaintenance": bool,
-        "DeferMaintenanceIdentifier": str,
-        "DeferMaintenanceStartTime": Union[datetime, str],
-        "DeferMaintenanceEndTime": Union[datetime, str],
-        "DeferMaintenanceDuration": int,
-    },
-    total=False,
-)
-
-class ModifyClusterMaintenanceMessageRequestTypeDef(
-    _RequiredModifyClusterMaintenanceMessageRequestTypeDef,
-    _OptionalModifyClusterMaintenanceMessageRequestTypeDef,
-):
-    pass
-
 _RequiredModifyClusterMessageRequestTypeDef = TypedDict(
     "_RequiredModifyClusterMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
     },
 )
 _OptionalModifyClusterMessageRequestTypeDef = TypedDict(
@@ -3138,14 +3102,52 @@
     {
         "Marker": str,
         "ClusterVersions": List[ClusterVersionTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeEventsMessageRequestTypeDef = TypedDict(
+    "DescribeEventsMessageRequestTypeDef",
+    {
+        "SourceIdentifier": str,
+        "SourceType": SourceTypeType,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "Duration": int,
+        "MaxRecords": int,
+        "Marker": str,
+    },
+    total=False,
+)
+
+_RequiredModifyClusterMaintenanceMessageRequestTypeDef = TypedDict(
+    "_RequiredModifyClusterMaintenanceMessageRequestTypeDef",
+    {
+        "ClusterIdentifier": str,
+    },
+)
+_OptionalModifyClusterMaintenanceMessageRequestTypeDef = TypedDict(
+    "_OptionalModifyClusterMaintenanceMessageRequestTypeDef",
+    {
+        "DeferMaintenance": bool,
+        "DeferMaintenanceIdentifier": str,
+        "DeferMaintenanceStartTime": TimestampTypeDef,
+        "DeferMaintenanceEndTime": TimestampTypeDef,
+        "DeferMaintenanceDuration": int,
+    },
+    total=False,
+)
+
+class ModifyClusterMaintenanceMessageRequestTypeDef(
+    _RequiredModifyClusterMaintenanceMessageRequestTypeDef,
+    _OptionalModifyClusterMaintenanceMessageRequestTypeDef,
+):
+    pass
+
 DataShareResponseTypeDef = TypedDict(
     "DataShareResponseTypeDef",
     {
         "DataShareArn": str,
         "ProducerArn": str,
         "AllowPubliclyAccessibleConsumers": bool,
         "DataShareAssociations": List[DataShareAssociationTypeDef],
@@ -3353,16 +3355,16 @@
 )
 
 DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
     "DescribeEventsMessageDescribeEventsPaginateTypeDef",
     {
         "SourceIdentifier": str,
         "SourceType": SourceTypeType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
         "Duration": int,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeHsmClientCertificatesMessageDescribeHsmClientCertificatesPaginateTypeDef = TypedDict(
@@ -3528,16 +3530,16 @@
 DescribeClusterSnapshotsMessageDescribeClusterSnapshotsPaginateTypeDef = TypedDict(
     "DescribeClusterSnapshotsMessageDescribeClusterSnapshotsPaginateTypeDef",
     {
         "ClusterIdentifier": str,
         "SnapshotIdentifier": str,
         "SnapshotArn": str,
         "SnapshotType": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
         "OwnerAccount": str,
         "TagKeys": Sequence[str],
         "TagValues": Sequence[str],
         "ClusterExists": bool,
         "SortingEntities": Sequence[SnapshotSortingEntityTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -3547,16 +3549,16 @@
 DescribeClusterSnapshotsMessageRequestTypeDef = TypedDict(
     "DescribeClusterSnapshotsMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
         "SnapshotIdentifier": str,
         "SnapshotArn": str,
         "SnapshotType": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
         "MaxRecords": int,
         "Marker": str,
         "OwnerAccount": str,
         "TagKeys": Sequence[str],
         "TagValues": Sequence[str],
         "ClusterExists": bool,
         "SortingEntities": Sequence[SnapshotSortingEntityTypeDef],
@@ -3567,16 +3569,16 @@
 DescribeClusterSnapshotsMessageSnapshotAvailableWaitTypeDef = TypedDict(
     "DescribeClusterSnapshotsMessageSnapshotAvailableWaitTypeDef",
     {
         "ClusterIdentifier": str,
         "SnapshotIdentifier": str,
         "SnapshotArn": str,
         "SnapshotType": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
         "MaxRecords": int,
         "Marker": str,
         "OwnerAccount": str,
         "TagKeys": Sequence[str],
         "TagValues": Sequence[str],
         "ClusterExists": bool,
         "SortingEntities": Sequence[SnapshotSortingEntityTypeDef],
@@ -3684,30 +3686,30 @@
 )
 
 DescribeScheduledActionsMessageDescribeScheduledActionsPaginateTypeDef = TypedDict(
     "DescribeScheduledActionsMessageDescribeScheduledActionsPaginateTypeDef",
     {
         "ScheduledActionName": str,
         "TargetActionType": ScheduledActionTypeValuesType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
         "Active": bool,
         "Filters": Sequence[ScheduledActionFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeScheduledActionsMessageRequestTypeDef = TypedDict(
     "DescribeScheduledActionsMessageRequestTypeDef",
     {
         "ScheduledActionName": str,
         "TargetActionType": ScheduledActionTypeValuesType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
         "Active": bool,
         "Filters": Sequence[ScheduledActionFilterTypeDef],
         "Marker": str,
         "MaxRecords": int,
     },
     total=False,
 )
@@ -4216,16 +4218,16 @@
         "IamRole": str,
     },
 )
 _OptionalCreateScheduledActionMessageRequestTypeDef = TypedDict(
     "_OptionalCreateScheduledActionMessageRequestTypeDef",
     {
         "ScheduledActionDescription": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
         "Enable": bool,
     },
     total=False,
 )
 
 class CreateScheduledActionMessageRequestTypeDef(
     _RequiredCreateScheduledActionMessageRequestTypeDef,
@@ -4242,16 +4244,16 @@
 _OptionalModifyScheduledActionMessageRequestTypeDef = TypedDict(
     "_OptionalModifyScheduledActionMessageRequestTypeDef",
     {
         "TargetAction": ScheduledActionTypeTypeDef,
         "Schedule": str,
         "IamRole": str,
         "ScheduledActionDescription": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
         "Enable": bool,
     },
     total=False,
 )
 
 class ModifyScheduledActionMessageRequestTypeDef(
     _RequiredModifyScheduledActionMessageRequestTypeDef,
```

### Comparing `mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift/waiter.py` & `mypy-boto3-redshift-1.28.16/mypy_boto3_redshift/waiter.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,20 +21,19 @@
 
     cluster_available_waiter: ClusterAvailableWaiter = client.get_waiter("cluster_available")
     cluster_deleted_waiter: ClusterDeletedWaiter = client.get_waiter("cluster_deleted")
     cluster_restored_waiter: ClusterRestoredWaiter = client.get_waiter("cluster_restored")
     snapshot_available_waiter: SnapshotAvailableWaiter = client.get_waiter("snapshot_available")
     ```
 """
-from datetime import datetime
-from typing import Sequence, Union
+from typing import Sequence
 
 from botocore.waiter import Waiter
 
-from .type_defs import SnapshotSortingEntityTypeDef, WaiterConfigTypeDef
+from .type_defs import SnapshotSortingEntityTypeDef, TimestampTypeDef, WaiterConfigTypeDef
 
 __all__ = (
     "ClusterAvailableWaiter",
     "ClusterDeletedWaiter",
     "ClusterRestoredWaiter",
     "SnapshotAvailableWaiter",
 )
@@ -115,16 +114,16 @@
     def wait(
         self,
         *,
         ClusterIdentifier: str = ...,
         SnapshotIdentifier: str = ...,
         SnapshotArn: str = ...,
         SnapshotType: str = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         OwnerAccount: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
         ClusterExists: bool = ...,
         SortingEntities: Sequence[SnapshotSortingEntityTypeDef] = ...,
```

### Comparing `mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift/waiter.pyi` & `mypy-boto3-redshift-1.28.16/mypy_boto3_redshift/waiter.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -21,20 +21,19 @@
 
     cluster_available_waiter: ClusterAvailableWaiter = client.get_waiter("cluster_available")
     cluster_deleted_waiter: ClusterDeletedWaiter = client.get_waiter("cluster_deleted")
     cluster_restored_waiter: ClusterRestoredWaiter = client.get_waiter("cluster_restored")
     snapshot_available_waiter: SnapshotAvailableWaiter = client.get_waiter("snapshot_available")
     ```
 """
-from datetime import datetime
-from typing import Sequence, Union
+from typing import Sequence
 
 from botocore.waiter import Waiter
 
-from .type_defs import SnapshotSortingEntityTypeDef, WaiterConfigTypeDef
+from .type_defs import SnapshotSortingEntityTypeDef, TimestampTypeDef, WaiterConfigTypeDef
 
 __all__ = (
     "ClusterAvailableWaiter",
     "ClusterDeletedWaiter",
     "ClusterRestoredWaiter",
     "SnapshotAvailableWaiter",
 )
@@ -111,16 +110,16 @@
     def wait(
         self,
         *,
         ClusterIdentifier: str = ...,
         SnapshotIdentifier: str = ...,
         SnapshotArn: str = ...,
         SnapshotType: str = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         OwnerAccount: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
         ClusterExists: bool = ...,
         SortingEntities: Sequence[SnapshotSortingEntityTypeDef] = ...,
```

### Comparing `mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift.egg-info/PKG-INFO` & `mypy-boto3-redshift-1.28.16/mypy_boto3_redshift.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-redshift
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Redshift 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.Redshift 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 redshift type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 redshift type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-redshift.svg?color=blue)](https://pypi.org/project/mypy-boto3-redshift)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-redshift)](https://pepy.tech/project/mypy-boto3-redshift)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Redshift 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift)
+[boto3.Redshift 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift)
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
 [mypy-boto3-redshift docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/).
 
 See how it helps to find and fix potential bugs:
 
@@ -75,15 +75,15 @@
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
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
@@ -528,20 +528,20 @@
 )
 
 
 def check_value(value: ActionTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_redshift.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_redshift.type_defs import (
     AcceptReservedNodeExchangeInputMessageRequestTypeDef,
     ResponseMetadataTypeDef,
     AttributeValueTargetTypeDef,
     AccountWithRestoreAccessTypeDef,
@@ -577,14 +577,15 @@
     RestoreStatusTypeDef,
     VpcSecurityGroupMembershipTypeDef,
     ClusterVersionTypeDef,
     CopyClusterSnapshotMessageRequestTypeDef,
     CreateAuthenticationProfileMessageRequestTypeDef,
     CreateCustomDomainAssociationMessageRequestTypeDef,
     CreateEndpointAccessMessageRequestTypeDef,
+    TimestampTypeDef,
     DataShareAssociationTypeDef,
     DeauthorizeDataShareMessageRequestTypeDef,
     DeleteAuthenticationProfileMessageRequestTypeDef,
     DeleteClusterMessageRequestTypeDef,
     DeleteClusterParameterGroupMessageRequestTypeDef,
     DeleteClusterSecurityGroupMessageRequestTypeDef,
     DeleteClusterSnapshotMessageRequestTypeDef,
@@ -617,15 +618,14 @@
     DescribeDataSharesForProducerMessageRequestTypeDef,
     DescribeDataSharesMessageRequestTypeDef,
     DescribeDefaultClusterParametersMessageRequestTypeDef,
     DescribeEndpointAccessMessageRequestTypeDef,
     DescribeEndpointAuthorizationMessageRequestTypeDef,
     DescribeEventCategoriesMessageRequestTypeDef,
     DescribeEventSubscriptionsMessageRequestTypeDef,
-    DescribeEventsMessageRequestTypeDef,
     DescribeHsmClientCertificatesMessageRequestTypeDef,
     DescribeHsmConfigurationsMessageRequestTypeDef,
     DescribeLoggingStatusMessageRequestTypeDef,
     NodeConfigurationOptionsFilterTypeDef,
     DescribeOrderableClusterOptionsMessageRequestTypeDef,
     DescribePartnersInputMessageRequestTypeDef,
     PartnerIntegrationInfoTypeDef,
@@ -651,15 +651,14 @@
     GetClusterCredentialsWithIAMMessageRequestTypeDef,
     GetReservedNodeExchangeConfigurationOptionsInputMessageRequestTypeDef,
     GetReservedNodeExchangeOfferingsInputMessageRequestTypeDef,
     ModifyAquaInputMessageRequestTypeDef,
     ModifyAuthenticationProfileMessageRequestTypeDef,
     ModifyClusterDbRevisionMessageRequestTypeDef,
     ModifyClusterIamRolesMessageRequestTypeDef,
-    ModifyClusterMaintenanceMessageRequestTypeDef,
     ModifyClusterMessageRequestTypeDef,
     ModifyClusterSnapshotMessageRequestTypeDef,
     ModifyClusterSnapshotScheduleMessageRequestTypeDef,
     ModifyClusterSubnetGroupMessageRequestTypeDef,
     ModifyCustomDomainAssociationMessageRequestTypeDef,
     ModifyEndpointAccessMessageRequestTypeDef,
     ModifyEventSubscriptionMessageRequestTypeDef,
@@ -739,14 +738,16 @@
     SnapshotScheduleTypeDef,
     SnapshotTypeDef,
     TaggedResourceTypeDef,
     UsageLimitResponseTypeDef,
     UsageLimitTypeDef,
     DescribeReservedNodeExchangeStatusOutputMessageTypeDef,
     ClusterVersionsMessageTypeDef,
+    DescribeEventsMessageRequestTypeDef,
+    ModifyClusterMaintenanceMessageRequestTypeDef,
     DataShareResponseTypeDef,
     DataShareTypeDef,
     DescribeClusterDbRevisionsMessageDescribeClusterDbRevisionsPaginateTypeDef,
     DescribeClusterParameterGroupsMessageDescribeClusterParameterGroupsPaginateTypeDef,
     DescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef,
     DescribeClusterSecurityGroupsMessageDescribeClusterSecurityGroupsPaginateTypeDef,
     DescribeClusterSubnetGroupsMessageDescribeClusterSubnetGroupsPaginateTypeDef,
@@ -872,15 +873,15 @@
     ResizeClusterResultTypeDef,
     RestoreFromClusterSnapshotResultTypeDef,
     ResumeClusterResultTypeDef,
     RotateEncryptionKeyResultTypeDef,
 )
 
 
-def get_structure() -> AcceptReservedNodeExchangeInputMessageRequestTypeDef:
+def get_value() -> AcceptReservedNodeExchangeInputMessageRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift.egg-info/SOURCES.txt` & `mypy-boto3-redshift-1.28.16/mypy_boto3_redshift.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-1.28.15.post1/setup.py` & `mypy-boto3-redshift-1.28.16/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-redshift",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_redshift"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Redshift 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.Redshift 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 redshift type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 redshift type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_redshift": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

