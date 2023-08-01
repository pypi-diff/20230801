# Comparing `tmp/mypy-boto3-eks-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-eks-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-eks-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:02 2023, max compression
+gzip compressed data, was "mypy-boto3-eks-1.28.16.tar", last modified: Tue Aug  1 11:36:42 2023, max compression
```

## Comparing `mypy-boto3-eks-1.28.15.post1.tar` & `mypy-boto3-eks-1.28.16.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:02.669129 mypy-boto3-eks-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:44:29.000000 mypy-boto3-eks-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20758 2023-07-29 10:03:02.669129 mypy-boto3-eks-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19281 2023-07-29 09:44:29.000000 mypy-boto3-eks-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:02.669129 mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks/
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-07-29 09:44:29.000000 mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-07-29 09:44:29.000000 mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-29 09:44:29.000000 mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33469 2023-07-29 09:44:29.000000 mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    33412 2023-07-29 09:44:29.000000 mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14738 2023-07-29 09:44:29.000000 mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14736 2023-07-29 09:44:29.000000 mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8324 2023-07-29 09:44:29.000000 mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8315 2023-07-29 09:44:29.000000 mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:44:29.000000 mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    51810 2023-07-29 09:44:32.000000 mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    51737 2023-07-29 09:44:32.000000 mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:44:29.000000 mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7686 2023-07-29 09:44:29.000000 mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-07-29 09:44:29.000000 mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:02.669129 mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20758 2023-07-29 10:03:02.000000 mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-29 10:03:02.000000 mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:02.000000 mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:02.000000 mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:02.000000 mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-29 10:03:02.000000 mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:02.669129 mypy-boto3-eks-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-29 09:44:28.000000 mypy-boto3-eks-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:42.596901 mypy-boto3-eks-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:17:05.000000 mypy-boto3-eks-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20883 2023-08-01 11:36:42.596901 mypy-boto3-eks-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19415 2023-08-01 11:17:05.000000 mypy-boto3-eks-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:42.588901 mypy-boto3-eks-1.28.16/mypy_boto3_eks/
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-08-01 11:17:05.000000 mypy-boto3-eks-1.28.16/mypy_boto3_eks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-08-01 11:17:05.000000 mypy-boto3-eks-1.28.16/mypy_boto3_eks/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-08-01 11:17:05.000000 mypy-boto3-eks-1.28.16/mypy_boto3_eks/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33111 2023-08-01 11:17:05.000000 mypy-boto3-eks-1.28.16/mypy_boto3_eks/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33054 2023-08-01 11:17:05.000000 mypy-boto3-eks-1.28.16/mypy_boto3_eks/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14738 2023-08-01 11:17:06.000000 mypy-boto3-eks-1.28.16/mypy_boto3_eks/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14736 2023-08-01 11:17:05.000000 mypy-boto3-eks-1.28.16/mypy_boto3_eks/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8324 2023-08-01 11:17:05.000000 mypy-boto3-eks-1.28.16/mypy_boto3_eks/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8315 2023-08-01 11:17:05.000000 mypy-boto3-eks-1.28.16/mypy_boto3_eks/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:17:05.000000 mypy-boto3-eks-1.28.16/mypy_boto3_eks/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    52199 2023-08-01 11:17:07.000000 mypy-boto3-eks-1.28.16/mypy_boto3_eks/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52126 2023-08-01 11:17:06.000000 mypy-boto3-eks-1.28.16/mypy_boto3_eks/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:17:05.000000 mypy-boto3-eks-1.28.16/mypy_boto3_eks/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7686 2023-08-01 11:17:05.000000 mypy-boto3-eks-1.28.16/mypy_boto3_eks/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-08-01 11:17:05.000000 mypy-boto3-eks-1.28.16/mypy_boto3_eks/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:42.596901 mypy-boto3-eks-1.28.16/mypy_boto3_eks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20883 2023-08-01 11:36:42.000000 mypy-boto3-eks-1.28.16/mypy_boto3_eks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-08-01 11:36:42.000000 mypy-boto3-eks-1.28.16/mypy_boto3_eks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:42.000000 mypy-boto3-eks-1.28.16/mypy_boto3_eks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:42.000000 mypy-boto3-eks-1.28.16/mypy_boto3_eks.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:42.000000 mypy-boto3-eks-1.28.16/mypy_boto3_eks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-01 11:36:42.000000 mypy-boto3-eks-1.28.16/mypy_boto3_eks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:42.596901 mypy-boto3-eks-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-08-01 11:17:05.000000 mypy-boto3-eks-1.28.16/setup.py
```

### Comparing `mypy-boto3-eks-1.28.15.post1/LICENSE` & `mypy-boto3-eks-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-eks-1.28.15.post1/PKG-INFO` & `mypy-boto3-eks-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-eks
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.EKS 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.EKS 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 eks type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 eks type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-eks.svg?color=blue)](https://pypi.org/project/mypy-boto3-eks)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-eks)](https://pepy.tech/project/mypy-boto3-eks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EKS 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS)
+[boto3.EKS 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS)
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
 [mypy-boto3-eks docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/).
 
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
@@ -402,20 +402,20 @@
 )
 
 
 def check_value(value: AMITypesType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_eks.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_eks.type_defs import (
     AddonIssueTypeDef,
     MarketplaceInformationTypeDef,
     CompatibilityTypeDef,
     ResponseMetadataTypeDef,
@@ -428,16 +428,14 @@
     VpcConfigResponseTypeDef,
     ConnectorConfigRequestTypeDef,
     ControlPlanePlacementRequestTypeDef,
     ControlPlanePlacementResponseTypeDef,
     CreateAddonRequestRequestTypeDef,
     KubernetesNetworkConfigRequestTypeDef,
     VpcConfigRequestTypeDef,
-    FargateProfileSelectorOutputTypeDef,
-    FargateProfileSelectorTypeDef,
     LaunchTemplateSpecificationTypeDef,
     NodegroupScalingConfigTypeDef,
     NodegroupUpdateConfigTypeDef,
     RemoteAccessConfigTypeDef,
     TaintTypeDef,
     DeleteAddonRequestRequestTypeDef,
     DeleteClusterRequestRequestTypeDef,
@@ -452,14 +450,16 @@
     DescribeClusterRequestRequestTypeDef,
     DescribeFargateProfileRequestRequestTypeDef,
     IdentityProviderConfigTypeDef,
     DescribeNodegroupRequestRequestTypeDef,
     DescribeUpdateRequestRequestTypeDef,
     ProviderTypeDef,
     ErrorDetailTypeDef,
+    FargateProfileSelectorOutputTypeDef,
+    FargateProfileSelectorTypeDef,
     OidcIdentityProviderConfigTypeDef,
     OIDCTypeDef,
     IssueTypeDef,
     ListAddonsRequestRequestTypeDef,
     ListClustersRequestRequestTypeDef,
     ListFargateProfilesRequestRequestTypeDef,
     ListIdentityProviderConfigsRequestRequestTypeDef,
@@ -486,16 +486,14 @@
     ListUpdatesResponseTypeDef,
     AssociateIdentityProviderConfigRequestRequestTypeDef,
     NodegroupResourcesTypeDef,
     ClusterHealthTypeDef,
     RegisterClusterRequestRequestTypeDef,
     OutpostConfigRequestTypeDef,
     OutpostConfigResponseTypeDef,
-    FargateProfileTypeDef,
-    CreateFargateProfileRequestRequestTypeDef,
     UpdateNodegroupVersionRequestRequestTypeDef,
     CreateNodegroupRequestRequestTypeDef,
     UpdateTaintsPayloadTypeDef,
     DescribeAddonRequestAddonActiveWaitTypeDef,
     DescribeAddonRequestAddonDeletedWaitTypeDef,
     DescribeClusterRequestClusterActiveWaitTypeDef,
     DescribeClusterRequestClusterDeletedWaitTypeDef,
@@ -511,57 +509,63 @@
     ListNodegroupsRequestListNodegroupsPaginateTypeDef,
     ListUpdatesRequestListUpdatesPaginateTypeDef,
     DescribeIdentityProviderConfigRequestRequestTypeDef,
     DisassociateIdentityProviderConfigRequestRequestTypeDef,
     ListIdentityProviderConfigsResponseTypeDef,
     EncryptionConfigOutputTypeDef,
     EncryptionConfigTypeDef,
+    FargateProfileTypeDef,
+    FargateProfileSelectorUnionTypeDef,
     IdentityProviderConfigResponseTypeDef,
     IdentityTypeDef,
     NodegroupHealthTypeDef,
     LoggingOutputTypeDef,
     LoggingTypeDef,
+    RemoteAccessConfigUnionTypeDef,
     UpdateTypeDef,
     AddonTypeDef,
     AddonInfoTypeDef,
+    UpdateNodegroupConfigRequestRequestTypeDef,
+    EncryptionConfigUnionTypeDef,
     CreateFargateProfileResponseTypeDef,
     DeleteFargateProfileResponseTypeDef,
     DescribeFargateProfileResponseTypeDef,
-    UpdateNodegroupConfigRequestRequestTypeDef,
-    AssociateEncryptionConfigRequestRequestTypeDef,
+    CreateFargateProfileRequestRequestTypeDef,
     DescribeIdentityProviderConfigResponseTypeDef,
     NodegroupTypeDef,
     ClusterTypeDef,
-    CreateClusterRequestRequestTypeDef,
+    LoggingUnionTypeDef,
     UpdateClusterConfigRequestRequestTypeDef,
     AssociateEncryptionConfigResponseTypeDef,
     AssociateIdentityProviderConfigResponseTypeDef,
     DescribeUpdateResponseTypeDef,
     DisassociateIdentityProviderConfigResponseTypeDef,
     UpdateAddonResponseTypeDef,
     UpdateClusterConfigResponseTypeDef,
     UpdateClusterVersionResponseTypeDef,
     UpdateNodegroupConfigResponseTypeDef,
     UpdateNodegroupVersionResponseTypeDef,
     CreateAddonResponseTypeDef,
     DeleteAddonResponseTypeDef,
     DescribeAddonResponseTypeDef,
     DescribeAddonVersionsResponseTypeDef,
+    AssociateEncryptionConfigRequestRequestTypeDef,
+    CreateClusterRequestRequestTypeDef,
     CreateNodegroupResponseTypeDef,
     DeleteNodegroupResponseTypeDef,
     DescribeNodegroupResponseTypeDef,
     CreateClusterResponseTypeDef,
     DeleteClusterResponseTypeDef,
     DeregisterClusterResponseTypeDef,
     DescribeClusterResponseTypeDef,
     RegisterClusterResponseTypeDef,
 )
 
 
-def get_structure() -> AddonIssueTypeDef:
+def get_value() -> AddonIssueTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-eks-1.28.15.post1/README.md` & `mypy-boto3-eks-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-eks.svg?color=blue)](https://pypi.org/project/mypy-boto3-eks)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-eks)](https://pepy.tech/project/mypy-boto3-eks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EKS 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS)
+[boto3.EKS 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS)
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
 [mypy-boto3-eks docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/).
 
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
@@ -370,20 +370,20 @@
 )
 
 
 def check_value(value: AMITypesType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_eks.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_eks.type_defs import (
     AddonIssueTypeDef,
     MarketplaceInformationTypeDef,
     CompatibilityTypeDef,
     ResponseMetadataTypeDef,
@@ -396,16 +396,14 @@
     VpcConfigResponseTypeDef,
     ConnectorConfigRequestTypeDef,
     ControlPlanePlacementRequestTypeDef,
     ControlPlanePlacementResponseTypeDef,
     CreateAddonRequestRequestTypeDef,
     KubernetesNetworkConfigRequestTypeDef,
     VpcConfigRequestTypeDef,
-    FargateProfileSelectorOutputTypeDef,
-    FargateProfileSelectorTypeDef,
     LaunchTemplateSpecificationTypeDef,
     NodegroupScalingConfigTypeDef,
     NodegroupUpdateConfigTypeDef,
     RemoteAccessConfigTypeDef,
     TaintTypeDef,
     DeleteAddonRequestRequestTypeDef,
     DeleteClusterRequestRequestTypeDef,
@@ -420,14 +418,16 @@
     DescribeClusterRequestRequestTypeDef,
     DescribeFargateProfileRequestRequestTypeDef,
     IdentityProviderConfigTypeDef,
     DescribeNodegroupRequestRequestTypeDef,
     DescribeUpdateRequestRequestTypeDef,
     ProviderTypeDef,
     ErrorDetailTypeDef,
+    FargateProfileSelectorOutputTypeDef,
+    FargateProfileSelectorTypeDef,
     OidcIdentityProviderConfigTypeDef,
     OIDCTypeDef,
     IssueTypeDef,
     ListAddonsRequestRequestTypeDef,
     ListClustersRequestRequestTypeDef,
     ListFargateProfilesRequestRequestTypeDef,
     ListIdentityProviderConfigsRequestRequestTypeDef,
@@ -454,16 +454,14 @@
     ListUpdatesResponseTypeDef,
     AssociateIdentityProviderConfigRequestRequestTypeDef,
     NodegroupResourcesTypeDef,
     ClusterHealthTypeDef,
     RegisterClusterRequestRequestTypeDef,
     OutpostConfigRequestTypeDef,
     OutpostConfigResponseTypeDef,
-    FargateProfileTypeDef,
-    CreateFargateProfileRequestRequestTypeDef,
     UpdateNodegroupVersionRequestRequestTypeDef,
     CreateNodegroupRequestRequestTypeDef,
     UpdateTaintsPayloadTypeDef,
     DescribeAddonRequestAddonActiveWaitTypeDef,
     DescribeAddonRequestAddonDeletedWaitTypeDef,
     DescribeClusterRequestClusterActiveWaitTypeDef,
     DescribeClusterRequestClusterDeletedWaitTypeDef,
@@ -479,57 +477,63 @@
     ListNodegroupsRequestListNodegroupsPaginateTypeDef,
     ListUpdatesRequestListUpdatesPaginateTypeDef,
     DescribeIdentityProviderConfigRequestRequestTypeDef,
     DisassociateIdentityProviderConfigRequestRequestTypeDef,
     ListIdentityProviderConfigsResponseTypeDef,
     EncryptionConfigOutputTypeDef,
     EncryptionConfigTypeDef,
+    FargateProfileTypeDef,
+    FargateProfileSelectorUnionTypeDef,
     IdentityProviderConfigResponseTypeDef,
     IdentityTypeDef,
     NodegroupHealthTypeDef,
     LoggingOutputTypeDef,
     LoggingTypeDef,
+    RemoteAccessConfigUnionTypeDef,
     UpdateTypeDef,
     AddonTypeDef,
     AddonInfoTypeDef,
+    UpdateNodegroupConfigRequestRequestTypeDef,
+    EncryptionConfigUnionTypeDef,
     CreateFargateProfileResponseTypeDef,
     DeleteFargateProfileResponseTypeDef,
     DescribeFargateProfileResponseTypeDef,
-    UpdateNodegroupConfigRequestRequestTypeDef,
-    AssociateEncryptionConfigRequestRequestTypeDef,
+    CreateFargateProfileRequestRequestTypeDef,
     DescribeIdentityProviderConfigResponseTypeDef,
     NodegroupTypeDef,
     ClusterTypeDef,
-    CreateClusterRequestRequestTypeDef,
+    LoggingUnionTypeDef,
     UpdateClusterConfigRequestRequestTypeDef,
     AssociateEncryptionConfigResponseTypeDef,
     AssociateIdentityProviderConfigResponseTypeDef,
     DescribeUpdateResponseTypeDef,
     DisassociateIdentityProviderConfigResponseTypeDef,
     UpdateAddonResponseTypeDef,
     UpdateClusterConfigResponseTypeDef,
     UpdateClusterVersionResponseTypeDef,
     UpdateNodegroupConfigResponseTypeDef,
     UpdateNodegroupVersionResponseTypeDef,
     CreateAddonResponseTypeDef,
     DeleteAddonResponseTypeDef,
     DescribeAddonResponseTypeDef,
     DescribeAddonVersionsResponseTypeDef,
+    AssociateEncryptionConfigRequestRequestTypeDef,
+    CreateClusterRequestRequestTypeDef,
     CreateNodegroupResponseTypeDef,
     DeleteNodegroupResponseTypeDef,
     DescribeNodegroupResponseTypeDef,
     CreateClusterResponseTypeDef,
     DeleteClusterResponseTypeDef,
     DeregisterClusterResponseTypeDef,
     DescribeClusterResponseTypeDef,
     RegisterClusterResponseTypeDef,
 )
 
 
-def get_structure() -> AddonIssueTypeDef:
+def get_value() -> AddonIssueTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks/__init__.py` & `mypy-boto3-eks-1.28.16/mypy_boto3_eks/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks/__init__.pyi` & `mypy-boto3-eks-1.28.16/mypy_boto3_eks/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks/__main__.py` & `mypy-boto3-eks-1.28.16/mypy_boto3_eks/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.EKS 1.28.15\nVersion:         1.28.15.post1\nBuilder version:"
-        " 7.16.2\nDocs:           "
+        "Type annotations for boto3.EKS 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS\nOther"
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

### Comparing `mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks/client.py` & `mypy-boto3-eks-1.28.16/mypy_boto3_eks/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_eks.client import EKSClient
 
     session = Session()
     client: EKSClient = session.client("eks")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import AMITypesType, CapacityTypesType, ResolveConflictsType
 from .paginator import (
     DescribeAddonVersionsPaginator,
     ListAddonsPaginator,
@@ -46,37 +46,33 @@
     DescribeAddonVersionsResponseTypeDef,
     DescribeClusterResponseTypeDef,
     DescribeFargateProfileResponseTypeDef,
     DescribeIdentityProviderConfigResponseTypeDef,
     DescribeNodegroupResponseTypeDef,
     DescribeUpdateResponseTypeDef,
     DisassociateIdentityProviderConfigResponseTypeDef,
-    EncryptionConfigOutputTypeDef,
-    EncryptionConfigTypeDef,
-    FargateProfileSelectorOutputTypeDef,
-    FargateProfileSelectorTypeDef,
+    EncryptionConfigUnionTypeDef,
+    FargateProfileSelectorUnionTypeDef,
     IdentityProviderConfigTypeDef,
     KubernetesNetworkConfigRequestTypeDef,
     LaunchTemplateSpecificationTypeDef,
     ListAddonsResponseTypeDef,
     ListClustersResponseTypeDef,
     ListFargateProfilesResponseTypeDef,
     ListIdentityProviderConfigsResponseTypeDef,
     ListNodegroupsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListUpdatesResponseTypeDef,
-    LoggingOutputTypeDef,
-    LoggingTypeDef,
+    LoggingUnionTypeDef,
     NodegroupScalingConfigTypeDef,
     NodegroupUpdateConfigTypeDef,
     OidcIdentityProviderConfigRequestTypeDef,
     OutpostConfigRequestTypeDef,
     RegisterClusterResponseTypeDef,
-    RemoteAccessConfigOutputTypeDef,
-    RemoteAccessConfigTypeDef,
+    RemoteAccessConfigUnionTypeDef,
     TaintTypeDef,
     UpdateAddonResponseTypeDef,
     UpdateClusterConfigResponseTypeDef,
     UpdateClusterVersionResponseTypeDef,
     UpdateLabelsPayloadTypeDef,
     UpdateNodegroupConfigResponseTypeDef,
     UpdateNodegroupVersionResponseTypeDef,
@@ -145,15 +141,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/client/#exceptions)
         """
 
     def associate_encryption_config(
         self,
         *,
         clusterName: str,
-        encryptionConfig: Sequence[Union[EncryptionConfigTypeDef, EncryptionConfigOutputTypeDef]],
+        encryptionConfig: Sequence[EncryptionConfigUnionTypeDef],
         clientRequestToken: str = ...
     ) -> AssociateEncryptionConfigResponseTypeDef:
         """
         Associate encryption configuration to an existing cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.associate_encryption_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/client/#associate_encryption_config)
@@ -213,20 +209,18 @@
         self,
         *,
         name: str,
         roleArn: str,
         resourcesVpcConfig: VpcConfigRequestTypeDef,
         version: str = ...,
         kubernetesNetworkConfig: KubernetesNetworkConfigRequestTypeDef = ...,
-        logging: Union[LoggingTypeDef, LoggingOutputTypeDef] = ...,
+        logging: LoggingUnionTypeDef = ...,
         clientRequestToken: str = ...,
         tags: Mapping[str, str] = ...,
-        encryptionConfig: Sequence[
-            Union[EncryptionConfigTypeDef, EncryptionConfigOutputTypeDef]
-        ] = ...,
+        encryptionConfig: Sequence[EncryptionConfigUnionTypeDef] = ...,
         outpostConfig: OutpostConfigRequestTypeDef = ...
     ) -> CreateClusterResponseTypeDef:
         """
         Creates an Amazon EKS control plane.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.create_cluster)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/client/#create_cluster)
@@ -235,17 +229,15 @@
     def create_fargate_profile(
         self,
         *,
         fargateProfileName: str,
         clusterName: str,
         podExecutionRoleArn: str,
         subnets: Sequence[str] = ...,
-        selectors: Sequence[
-            Union[FargateProfileSelectorTypeDef, FargateProfileSelectorOutputTypeDef]
-        ] = ...,
+        selectors: Sequence[FargateProfileSelectorUnionTypeDef] = ...,
         clientRequestToken: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateFargateProfileResponseTypeDef:
         """
         Creates an Fargate profile for your Amazon EKS cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.create_fargate_profile)
@@ -259,15 +251,15 @@
         nodegroupName: str,
         subnets: Sequence[str],
         nodeRole: str,
         scalingConfig: NodegroupScalingConfigTypeDef = ...,
         diskSize: int = ...,
         instanceTypes: Sequence[str] = ...,
         amiType: AMITypesType = ...,
-        remoteAccess: Union[RemoteAccessConfigTypeDef, RemoteAccessConfigOutputTypeDef] = ...,
+        remoteAccess: RemoteAccessConfigUnionTypeDef = ...,
         labels: Mapping[str, str] = ...,
         taints: Sequence[TaintTypeDef] = ...,
         tags: Mapping[str, str] = ...,
         clientRequestToken: str = ...,
         launchTemplate: LaunchTemplateSpecificationTypeDef = ...,
         updateConfig: NodegroupUpdateConfigTypeDef = ...,
         capacityType: CapacityTypesType = ...,
@@ -568,15 +560,15 @@
         """
 
     def update_cluster_config(
         self,
         *,
         name: str,
         resourcesVpcConfig: VpcConfigRequestTypeDef = ...,
-        logging: Union[LoggingTypeDef, LoggingOutputTypeDef] = ...,
+        logging: LoggingUnionTypeDef = ...,
         clientRequestToken: str = ...
     ) -> UpdateClusterConfigResponseTypeDef:
         """
         Updates an Amazon EKS cluster configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.update_cluster_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/client/#update_cluster_config)
```

### Comparing `mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks/client.pyi` & `mypy-boto3-eks-1.28.16/mypy_boto3_eks/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_eks.client import EKSClient
 
     session = Session()
     client: EKSClient = session.client("eks")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import AMITypesType, CapacityTypesType, ResolveConflictsType
 from .paginator import (
     DescribeAddonVersionsPaginator,
     ListAddonsPaginator,
@@ -46,37 +46,33 @@
     DescribeAddonVersionsResponseTypeDef,
     DescribeClusterResponseTypeDef,
     DescribeFargateProfileResponseTypeDef,
     DescribeIdentityProviderConfigResponseTypeDef,
     DescribeNodegroupResponseTypeDef,
     DescribeUpdateResponseTypeDef,
     DisassociateIdentityProviderConfigResponseTypeDef,
-    EncryptionConfigOutputTypeDef,
-    EncryptionConfigTypeDef,
-    FargateProfileSelectorOutputTypeDef,
-    FargateProfileSelectorTypeDef,
+    EncryptionConfigUnionTypeDef,
+    FargateProfileSelectorUnionTypeDef,
     IdentityProviderConfigTypeDef,
     KubernetesNetworkConfigRequestTypeDef,
     LaunchTemplateSpecificationTypeDef,
     ListAddonsResponseTypeDef,
     ListClustersResponseTypeDef,
     ListFargateProfilesResponseTypeDef,
     ListIdentityProviderConfigsResponseTypeDef,
     ListNodegroupsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListUpdatesResponseTypeDef,
-    LoggingOutputTypeDef,
-    LoggingTypeDef,
+    LoggingUnionTypeDef,
     NodegroupScalingConfigTypeDef,
     NodegroupUpdateConfigTypeDef,
     OidcIdentityProviderConfigRequestTypeDef,
     OutpostConfigRequestTypeDef,
     RegisterClusterResponseTypeDef,
-    RemoteAccessConfigOutputTypeDef,
-    RemoteAccessConfigTypeDef,
+    RemoteAccessConfigUnionTypeDef,
     TaintTypeDef,
     UpdateAddonResponseTypeDef,
     UpdateClusterConfigResponseTypeDef,
     UpdateClusterVersionResponseTypeDef,
     UpdateLabelsPayloadTypeDef,
     UpdateNodegroupConfigResponseTypeDef,
     UpdateNodegroupVersionResponseTypeDef,
@@ -140,15 +136,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/client/#exceptions)
         """
     def associate_encryption_config(
         self,
         *,
         clusterName: str,
-        encryptionConfig: Sequence[Union[EncryptionConfigTypeDef, EncryptionConfigOutputTypeDef]],
+        encryptionConfig: Sequence[EncryptionConfigUnionTypeDef],
         clientRequestToken: str = ...
     ) -> AssociateEncryptionConfigResponseTypeDef:
         """
         Associate encryption configuration to an existing cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.associate_encryption_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/client/#associate_encryption_config)
@@ -203,20 +199,18 @@
         self,
         *,
         name: str,
         roleArn: str,
         resourcesVpcConfig: VpcConfigRequestTypeDef,
         version: str = ...,
         kubernetesNetworkConfig: KubernetesNetworkConfigRequestTypeDef = ...,
-        logging: Union[LoggingTypeDef, LoggingOutputTypeDef] = ...,
+        logging: LoggingUnionTypeDef = ...,
         clientRequestToken: str = ...,
         tags: Mapping[str, str] = ...,
-        encryptionConfig: Sequence[
-            Union[EncryptionConfigTypeDef, EncryptionConfigOutputTypeDef]
-        ] = ...,
+        encryptionConfig: Sequence[EncryptionConfigUnionTypeDef] = ...,
         outpostConfig: OutpostConfigRequestTypeDef = ...
     ) -> CreateClusterResponseTypeDef:
         """
         Creates an Amazon EKS control plane.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.create_cluster)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/client/#create_cluster)
@@ -224,17 +218,15 @@
     def create_fargate_profile(
         self,
         *,
         fargateProfileName: str,
         clusterName: str,
         podExecutionRoleArn: str,
         subnets: Sequence[str] = ...,
-        selectors: Sequence[
-            Union[FargateProfileSelectorTypeDef, FargateProfileSelectorOutputTypeDef]
-        ] = ...,
+        selectors: Sequence[FargateProfileSelectorUnionTypeDef] = ...,
         clientRequestToken: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateFargateProfileResponseTypeDef:
         """
         Creates an Fargate profile for your Amazon EKS cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.create_fargate_profile)
@@ -247,15 +239,15 @@
         nodegroupName: str,
         subnets: Sequence[str],
         nodeRole: str,
         scalingConfig: NodegroupScalingConfigTypeDef = ...,
         diskSize: int = ...,
         instanceTypes: Sequence[str] = ...,
         amiType: AMITypesType = ...,
-        remoteAccess: Union[RemoteAccessConfigTypeDef, RemoteAccessConfigOutputTypeDef] = ...,
+        remoteAccess: RemoteAccessConfigUnionTypeDef = ...,
         labels: Mapping[str, str] = ...,
         taints: Sequence[TaintTypeDef] = ...,
         tags: Mapping[str, str] = ...,
         clientRequestToken: str = ...,
         launchTemplate: LaunchTemplateSpecificationTypeDef = ...,
         updateConfig: NodegroupUpdateConfigTypeDef = ...,
         capacityType: CapacityTypesType = ...,
@@ -529,15 +521,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/client/#update_addon)
         """
     def update_cluster_config(
         self,
         *,
         name: str,
         resourcesVpcConfig: VpcConfigRequestTypeDef = ...,
-        logging: Union[LoggingTypeDef, LoggingOutputTypeDef] = ...,
+        logging: LoggingUnionTypeDef = ...,
         clientRequestToken: str = ...
     ) -> UpdateClusterConfigResponseTypeDef:
         """
         Updates an Amazon EKS cluster configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.update_cluster_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/client/#update_cluster_config)
```

### Comparing `mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks/literals.py` & `mypy-boto3-eks-1.28.16/mypy_boto3_eks/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks/literals.pyi` & `mypy-boto3-eks-1.28.16/mypy_boto3_eks/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks/paginator.py` & `mypy-boto3-eks-1.28.16/mypy_boto3_eks/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks/paginator.pyi` & `mypy-boto3-eks-1.28.16/mypy_boto3_eks/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks/type_defs.py` & `mypy-boto3-eks-1.28.16/mypy_boto3_eks/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_eks.type_defs import AddonIssueTypeDef
 
-    data: AddonIssueTypeDef = {...}
+    data: AddonIssueTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -57,16 +57,14 @@
     "VpcConfigResponseTypeDef",
     "ConnectorConfigRequestTypeDef",
     "ControlPlanePlacementRequestTypeDef",
     "ControlPlanePlacementResponseTypeDef",
     "CreateAddonRequestRequestTypeDef",
     "KubernetesNetworkConfigRequestTypeDef",
     "VpcConfigRequestTypeDef",
-    "FargateProfileSelectorOutputTypeDef",
-    "FargateProfileSelectorTypeDef",
     "LaunchTemplateSpecificationTypeDef",
     "NodegroupScalingConfigTypeDef",
     "NodegroupUpdateConfigTypeDef",
     "RemoteAccessConfigTypeDef",
     "TaintTypeDef",
     "DeleteAddonRequestRequestTypeDef",
     "DeleteClusterRequestRequestTypeDef",
@@ -81,14 +79,16 @@
     "DescribeClusterRequestRequestTypeDef",
     "DescribeFargateProfileRequestRequestTypeDef",
     "IdentityProviderConfigTypeDef",
     "DescribeNodegroupRequestRequestTypeDef",
     "DescribeUpdateRequestRequestTypeDef",
     "ProviderTypeDef",
     "ErrorDetailTypeDef",
+    "FargateProfileSelectorOutputTypeDef",
+    "FargateProfileSelectorTypeDef",
     "OidcIdentityProviderConfigTypeDef",
     "OIDCTypeDef",
     "IssueTypeDef",
     "ListAddonsRequestRequestTypeDef",
     "ListClustersRequestRequestTypeDef",
     "ListFargateProfilesRequestRequestTypeDef",
     "ListIdentityProviderConfigsRequestRequestTypeDef",
@@ -115,16 +115,14 @@
     "ListUpdatesResponseTypeDef",
     "AssociateIdentityProviderConfigRequestRequestTypeDef",
     "NodegroupResourcesTypeDef",
     "ClusterHealthTypeDef",
     "RegisterClusterRequestRequestTypeDef",
     "OutpostConfigRequestTypeDef",
     "OutpostConfigResponseTypeDef",
-    "FargateProfileTypeDef",
-    "CreateFargateProfileRequestRequestTypeDef",
     "UpdateNodegroupVersionRequestRequestTypeDef",
     "CreateNodegroupRequestRequestTypeDef",
     "UpdateTaintsPayloadTypeDef",
     "DescribeAddonRequestAddonActiveWaitTypeDef",
     "DescribeAddonRequestAddonDeletedWaitTypeDef",
     "DescribeClusterRequestClusterActiveWaitTypeDef",
     "DescribeClusterRequestClusterDeletedWaitTypeDef",
@@ -140,45 +138,51 @@
     "ListNodegroupsRequestListNodegroupsPaginateTypeDef",
     "ListUpdatesRequestListUpdatesPaginateTypeDef",
     "DescribeIdentityProviderConfigRequestRequestTypeDef",
     "DisassociateIdentityProviderConfigRequestRequestTypeDef",
     "ListIdentityProviderConfigsResponseTypeDef",
     "EncryptionConfigOutputTypeDef",
     "EncryptionConfigTypeDef",
+    "FargateProfileTypeDef",
+    "FargateProfileSelectorUnionTypeDef",
     "IdentityProviderConfigResponseTypeDef",
     "IdentityTypeDef",
     "NodegroupHealthTypeDef",
     "LoggingOutputTypeDef",
     "LoggingTypeDef",
+    "RemoteAccessConfigUnionTypeDef",
     "UpdateTypeDef",
     "AddonTypeDef",
     "AddonInfoTypeDef",
+    "UpdateNodegroupConfigRequestRequestTypeDef",
+    "EncryptionConfigUnionTypeDef",
     "CreateFargateProfileResponseTypeDef",
     "DeleteFargateProfileResponseTypeDef",
     "DescribeFargateProfileResponseTypeDef",
-    "UpdateNodegroupConfigRequestRequestTypeDef",
-    "AssociateEncryptionConfigRequestRequestTypeDef",
+    "CreateFargateProfileRequestRequestTypeDef",
     "DescribeIdentityProviderConfigResponseTypeDef",
     "NodegroupTypeDef",
     "ClusterTypeDef",
-    "CreateClusterRequestRequestTypeDef",
+    "LoggingUnionTypeDef",
     "UpdateClusterConfigRequestRequestTypeDef",
     "AssociateEncryptionConfigResponseTypeDef",
     "AssociateIdentityProviderConfigResponseTypeDef",
     "DescribeUpdateResponseTypeDef",
     "DisassociateIdentityProviderConfigResponseTypeDef",
     "UpdateAddonResponseTypeDef",
     "UpdateClusterConfigResponseTypeDef",
     "UpdateClusterVersionResponseTypeDef",
     "UpdateNodegroupConfigResponseTypeDef",
     "UpdateNodegroupVersionResponseTypeDef",
     "CreateAddonResponseTypeDef",
     "DeleteAddonResponseTypeDef",
     "DescribeAddonResponseTypeDef",
     "DescribeAddonVersionsResponseTypeDef",
+    "AssociateEncryptionConfigRequestRequestTypeDef",
+    "CreateClusterRequestRequestTypeDef",
     "CreateNodegroupResponseTypeDef",
     "DeleteNodegroupResponseTypeDef",
     "DescribeNodegroupResponseTypeDef",
     "CreateClusterResponseTypeDef",
     "DeleteClusterResponseTypeDef",
     "DeregisterClusterResponseTypeDef",
     "DescribeClusterResponseTypeDef",
@@ -383,32 +387,14 @@
         "endpointPublicAccess": bool,
         "endpointPrivateAccess": bool,
         "publicAccessCidrs": Sequence[str],
     },
     total=False,
 )
 
-FargateProfileSelectorOutputTypeDef = TypedDict(
-    "FargateProfileSelectorOutputTypeDef",
-    {
-        "namespace": str,
-        "labels": Dict[str, str],
-    },
-    total=False,
-)
-
-FargateProfileSelectorTypeDef = TypedDict(
-    "FargateProfileSelectorTypeDef",
-    {
-        "namespace": str,
-        "labels": Mapping[str, str],
-    },
-    total=False,
-)
-
 LaunchTemplateSpecificationTypeDef = TypedDict(
     "LaunchTemplateSpecificationTypeDef",
     {
         "name": str,
         "version": str,
         "id": str,
     },
@@ -622,14 +608,32 @@
         "errorCode": ErrorCodeType,
         "errorMessage": str,
         "resourceIds": List[str],
     },
     total=False,
 )
 
+FargateProfileSelectorOutputTypeDef = TypedDict(
+    "FargateProfileSelectorOutputTypeDef",
+    {
+        "namespace": str,
+        "labels": Dict[str, str],
+    },
+    total=False,
+)
+
+FargateProfileSelectorTypeDef = TypedDict(
+    "FargateProfileSelectorTypeDef",
+    {
+        "namespace": str,
+        "labels": Mapping[str, str],
+    },
+    total=False,
+)
+
 OidcIdentityProviderConfigTypeDef = TypedDict(
     "OidcIdentityProviderConfigTypeDef",
     {
         "identityProviderConfigName": str,
         "identityProviderConfigArn": str,
         "clusterName": str,
         "issuerUrl": str,
@@ -1090,59 +1094,14 @@
 
 class OutpostConfigResponseTypeDef(
     _RequiredOutpostConfigResponseTypeDef, _OptionalOutpostConfigResponseTypeDef
 ):
     pass
 
 
-FargateProfileTypeDef = TypedDict(
-    "FargateProfileTypeDef",
-    {
-        "fargateProfileName": str,
-        "fargateProfileArn": str,
-        "clusterName": str,
-        "createdAt": datetime,
-        "podExecutionRoleArn": str,
-        "subnets": List[str],
-        "selectors": List[FargateProfileSelectorOutputTypeDef],
-        "status": FargateProfileStatusType,
-        "tags": Dict[str, str],
-    },
-    total=False,
-)
-
-_RequiredCreateFargateProfileRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateFargateProfileRequestRequestTypeDef",
-    {
-        "fargateProfileName": str,
-        "clusterName": str,
-        "podExecutionRoleArn": str,
-    },
-)
-_OptionalCreateFargateProfileRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateFargateProfileRequestRequestTypeDef",
-    {
-        "subnets": Sequence[str],
-        "selectors": Sequence[
-            Union[FargateProfileSelectorTypeDef, FargateProfileSelectorOutputTypeDef]
-        ],
-        "clientRequestToken": str,
-        "tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class CreateFargateProfileRequestRequestTypeDef(
-    _RequiredCreateFargateProfileRequestRequestTypeDef,
-    _OptionalCreateFargateProfileRequestRequestTypeDef,
-):
-    pass
-
-
 _RequiredUpdateNodegroupVersionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateNodegroupVersionRequestRequestTypeDef",
     {
         "clusterName": str,
         "nodegroupName": str,
     },
 )
@@ -1582,14 +1541,33 @@
     {
         "resources": Sequence[str],
         "provider": ProviderTypeDef,
     },
     total=False,
 )
 
+FargateProfileTypeDef = TypedDict(
+    "FargateProfileTypeDef",
+    {
+        "fargateProfileName": str,
+        "fargateProfileArn": str,
+        "clusterName": str,
+        "createdAt": datetime,
+        "podExecutionRoleArn": str,
+        "subnets": List[str],
+        "selectors": List[FargateProfileSelectorOutputTypeDef],
+        "status": FargateProfileStatusType,
+        "tags": Dict[str, str],
+    },
+    total=False,
+)
+
+FargateProfileSelectorUnionTypeDef = Union[
+    FargateProfileSelectorTypeDef, FargateProfileSelectorOutputTypeDef
+]
 IdentityProviderConfigResponseTypeDef = TypedDict(
     "IdentityProviderConfigResponseTypeDef",
     {
         "oidc": OidcIdentityProviderConfigTypeDef,
     },
     total=False,
 )
@@ -1622,14 +1600,15 @@
     "LoggingTypeDef",
     {
         "clusterLogging": Sequence[LogSetupTypeDef],
     },
     total=False,
 )
 
+RemoteAccessConfigUnionTypeDef = Union[RemoteAccessConfigTypeDef, RemoteAccessConfigOutputTypeDef]
 UpdateTypeDef = TypedDict(
     "UpdateTypeDef",
     {
         "id": str,
         "status": UpdateStatusType,
         "type": UpdateTypeType,
         "params": List[UpdateParamTypeDef],
@@ -1669,38 +1648,14 @@
         "publisher": str,
         "owner": str,
         "marketplaceInformation": MarketplaceInformationTypeDef,
     },
     total=False,
 )
 
-CreateFargateProfileResponseTypeDef = TypedDict(
-    "CreateFargateProfileResponseTypeDef",
-    {
-        "fargateProfile": FargateProfileTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteFargateProfileResponseTypeDef = TypedDict(
-    "DeleteFargateProfileResponseTypeDef",
-    {
-        "fargateProfile": FargateProfileTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeFargateProfileResponseTypeDef = TypedDict(
-    "DescribeFargateProfileResponseTypeDef",
-    {
-        "fargateProfile": FargateProfileTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredUpdateNodegroupConfigRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateNodegroupConfigRequestRequestTypeDef",
     {
         "clusterName": str,
         "nodegroupName": str,
     },
 )
@@ -1720,33 +1675,62 @@
 class UpdateNodegroupConfigRequestRequestTypeDef(
     _RequiredUpdateNodegroupConfigRequestRequestTypeDef,
     _OptionalUpdateNodegroupConfigRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredAssociateEncryptionConfigRequestRequestTypeDef = TypedDict(
-    "_RequiredAssociateEncryptionConfigRequestRequestTypeDef",
+EncryptionConfigUnionTypeDef = Union[EncryptionConfigTypeDef, EncryptionConfigOutputTypeDef]
+CreateFargateProfileResponseTypeDef = TypedDict(
+    "CreateFargateProfileResponseTypeDef",
+    {
+        "fargateProfile": FargateProfileTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteFargateProfileResponseTypeDef = TypedDict(
+    "DeleteFargateProfileResponseTypeDef",
+    {
+        "fargateProfile": FargateProfileTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeFargateProfileResponseTypeDef = TypedDict(
+    "DescribeFargateProfileResponseTypeDef",
     {
+        "fargateProfile": FargateProfileTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredCreateFargateProfileRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateFargateProfileRequestRequestTypeDef",
+    {
+        "fargateProfileName": str,
         "clusterName": str,
-        "encryptionConfig": Sequence[Union[EncryptionConfigTypeDef, EncryptionConfigOutputTypeDef]],
+        "podExecutionRoleArn": str,
     },
 )
-_OptionalAssociateEncryptionConfigRequestRequestTypeDef = TypedDict(
-    "_OptionalAssociateEncryptionConfigRequestRequestTypeDef",
+_OptionalCreateFargateProfileRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateFargateProfileRequestRequestTypeDef",
     {
+        "subnets": Sequence[str],
+        "selectors": Sequence[FargateProfileSelectorUnionTypeDef],
         "clientRequestToken": str,
+        "tags": Mapping[str, str],
     },
     total=False,
 )
 
 
-class AssociateEncryptionConfigRequestRequestTypeDef(
-    _RequiredAssociateEncryptionConfigRequestRequestTypeDef,
-    _OptionalAssociateEncryptionConfigRequestRequestTypeDef,
+class CreateFargateProfileRequestRequestTypeDef(
+    _RequiredCreateFargateProfileRequestRequestTypeDef,
+    _OptionalCreateFargateProfileRequestRequestTypeDef,
 ):
     pass
 
 
 DescribeIdentityProviderConfigResponseTypeDef = TypedDict(
     "DescribeIdentityProviderConfigResponseTypeDef",
     {
@@ -1808,43 +1792,15 @@
         "id": str,
         "health": ClusterHealthTypeDef,
         "outpostConfig": OutpostConfigResponseTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateClusterRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateClusterRequestRequestTypeDef",
-    {
-        "name": str,
-        "roleArn": str,
-        "resourcesVpcConfig": VpcConfigRequestTypeDef,
-    },
-)
-_OptionalCreateClusterRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateClusterRequestRequestTypeDef",
-    {
-        "version": str,
-        "kubernetesNetworkConfig": KubernetesNetworkConfigRequestTypeDef,
-        "logging": LoggingTypeDef,
-        "clientRequestToken": str,
-        "tags": Mapping[str, str],
-        "encryptionConfig": Sequence[Union[EncryptionConfigTypeDef, EncryptionConfigOutputTypeDef]],
-        "outpostConfig": OutpostConfigRequestTypeDef,
-    },
-    total=False,
-)
-
-
-class CreateClusterRequestRequestTypeDef(
-    _RequiredCreateClusterRequestRequestTypeDef, _OptionalCreateClusterRequestRequestTypeDef
-):
-    pass
-
-
+LoggingUnionTypeDef = Union[LoggingTypeDef, LoggingOutputTypeDef]
 _RequiredUpdateClusterConfigRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateClusterConfigRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalUpdateClusterConfigRequestRequestTypeDef = TypedDict(
@@ -1967,14 +1923,66 @@
     {
         "addons": List[AddonInfoTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredAssociateEncryptionConfigRequestRequestTypeDef = TypedDict(
+    "_RequiredAssociateEncryptionConfigRequestRequestTypeDef",
+    {
+        "clusterName": str,
+        "encryptionConfig": Sequence[EncryptionConfigUnionTypeDef],
+    },
+)
+_OptionalAssociateEncryptionConfigRequestRequestTypeDef = TypedDict(
+    "_OptionalAssociateEncryptionConfigRequestRequestTypeDef",
+    {
+        "clientRequestToken": str,
+    },
+    total=False,
+)
+
+
+class AssociateEncryptionConfigRequestRequestTypeDef(
+    _RequiredAssociateEncryptionConfigRequestRequestTypeDef,
+    _OptionalAssociateEncryptionConfigRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredCreateClusterRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateClusterRequestRequestTypeDef",
+    {
+        "name": str,
+        "roleArn": str,
+        "resourcesVpcConfig": VpcConfigRequestTypeDef,
+    },
+)
+_OptionalCreateClusterRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateClusterRequestRequestTypeDef",
+    {
+        "version": str,
+        "kubernetesNetworkConfig": KubernetesNetworkConfigRequestTypeDef,
+        "logging": LoggingTypeDef,
+        "clientRequestToken": str,
+        "tags": Mapping[str, str],
+        "encryptionConfig": Sequence[EncryptionConfigUnionTypeDef],
+        "outpostConfig": OutpostConfigRequestTypeDef,
+    },
+    total=False,
+)
+
+
+class CreateClusterRequestRequestTypeDef(
+    _RequiredCreateClusterRequestRequestTypeDef, _OptionalCreateClusterRequestRequestTypeDef
+):
+    pass
+
+
 CreateNodegroupResponseTypeDef = TypedDict(
     "CreateNodegroupResponseTypeDef",
     {
         "nodegroup": NodegroupTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks/type_defs.pyi` & `mypy-boto3-eks-1.28.16/mypy_boto3_eks/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_eks.type_defs import AddonIssueTypeDef
 
-    data: AddonIssueTypeDef = {...}
+    data: AddonIssueTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -56,16 +56,14 @@
     "VpcConfigResponseTypeDef",
     "ConnectorConfigRequestTypeDef",
     "ControlPlanePlacementRequestTypeDef",
     "ControlPlanePlacementResponseTypeDef",
     "CreateAddonRequestRequestTypeDef",
     "KubernetesNetworkConfigRequestTypeDef",
     "VpcConfigRequestTypeDef",
-    "FargateProfileSelectorOutputTypeDef",
-    "FargateProfileSelectorTypeDef",
     "LaunchTemplateSpecificationTypeDef",
     "NodegroupScalingConfigTypeDef",
     "NodegroupUpdateConfigTypeDef",
     "RemoteAccessConfigTypeDef",
     "TaintTypeDef",
     "DeleteAddonRequestRequestTypeDef",
     "DeleteClusterRequestRequestTypeDef",
@@ -80,14 +78,16 @@
     "DescribeClusterRequestRequestTypeDef",
     "DescribeFargateProfileRequestRequestTypeDef",
     "IdentityProviderConfigTypeDef",
     "DescribeNodegroupRequestRequestTypeDef",
     "DescribeUpdateRequestRequestTypeDef",
     "ProviderTypeDef",
     "ErrorDetailTypeDef",
+    "FargateProfileSelectorOutputTypeDef",
+    "FargateProfileSelectorTypeDef",
     "OidcIdentityProviderConfigTypeDef",
     "OIDCTypeDef",
     "IssueTypeDef",
     "ListAddonsRequestRequestTypeDef",
     "ListClustersRequestRequestTypeDef",
     "ListFargateProfilesRequestRequestTypeDef",
     "ListIdentityProviderConfigsRequestRequestTypeDef",
@@ -114,16 +114,14 @@
     "ListUpdatesResponseTypeDef",
     "AssociateIdentityProviderConfigRequestRequestTypeDef",
     "NodegroupResourcesTypeDef",
     "ClusterHealthTypeDef",
     "RegisterClusterRequestRequestTypeDef",
     "OutpostConfigRequestTypeDef",
     "OutpostConfigResponseTypeDef",
-    "FargateProfileTypeDef",
-    "CreateFargateProfileRequestRequestTypeDef",
     "UpdateNodegroupVersionRequestRequestTypeDef",
     "CreateNodegroupRequestRequestTypeDef",
     "UpdateTaintsPayloadTypeDef",
     "DescribeAddonRequestAddonActiveWaitTypeDef",
     "DescribeAddonRequestAddonDeletedWaitTypeDef",
     "DescribeClusterRequestClusterActiveWaitTypeDef",
     "DescribeClusterRequestClusterDeletedWaitTypeDef",
@@ -139,45 +137,51 @@
     "ListNodegroupsRequestListNodegroupsPaginateTypeDef",
     "ListUpdatesRequestListUpdatesPaginateTypeDef",
     "DescribeIdentityProviderConfigRequestRequestTypeDef",
     "DisassociateIdentityProviderConfigRequestRequestTypeDef",
     "ListIdentityProviderConfigsResponseTypeDef",
     "EncryptionConfigOutputTypeDef",
     "EncryptionConfigTypeDef",
+    "FargateProfileTypeDef",
+    "FargateProfileSelectorUnionTypeDef",
     "IdentityProviderConfigResponseTypeDef",
     "IdentityTypeDef",
     "NodegroupHealthTypeDef",
     "LoggingOutputTypeDef",
     "LoggingTypeDef",
+    "RemoteAccessConfigUnionTypeDef",
     "UpdateTypeDef",
     "AddonTypeDef",
     "AddonInfoTypeDef",
+    "UpdateNodegroupConfigRequestRequestTypeDef",
+    "EncryptionConfigUnionTypeDef",
     "CreateFargateProfileResponseTypeDef",
     "DeleteFargateProfileResponseTypeDef",
     "DescribeFargateProfileResponseTypeDef",
-    "UpdateNodegroupConfigRequestRequestTypeDef",
-    "AssociateEncryptionConfigRequestRequestTypeDef",
+    "CreateFargateProfileRequestRequestTypeDef",
     "DescribeIdentityProviderConfigResponseTypeDef",
     "NodegroupTypeDef",
     "ClusterTypeDef",
-    "CreateClusterRequestRequestTypeDef",
+    "LoggingUnionTypeDef",
     "UpdateClusterConfigRequestRequestTypeDef",
     "AssociateEncryptionConfigResponseTypeDef",
     "AssociateIdentityProviderConfigResponseTypeDef",
     "DescribeUpdateResponseTypeDef",
     "DisassociateIdentityProviderConfigResponseTypeDef",
     "UpdateAddonResponseTypeDef",
     "UpdateClusterConfigResponseTypeDef",
     "UpdateClusterVersionResponseTypeDef",
     "UpdateNodegroupConfigResponseTypeDef",
     "UpdateNodegroupVersionResponseTypeDef",
     "CreateAddonResponseTypeDef",
     "DeleteAddonResponseTypeDef",
     "DescribeAddonResponseTypeDef",
     "DescribeAddonVersionsResponseTypeDef",
+    "AssociateEncryptionConfigRequestRequestTypeDef",
+    "CreateClusterRequestRequestTypeDef",
     "CreateNodegroupResponseTypeDef",
     "DeleteNodegroupResponseTypeDef",
     "DescribeNodegroupResponseTypeDef",
     "CreateClusterResponseTypeDef",
     "DeleteClusterResponseTypeDef",
     "DeregisterClusterResponseTypeDef",
     "DescribeClusterResponseTypeDef",
@@ -378,32 +382,14 @@
         "endpointPublicAccess": bool,
         "endpointPrivateAccess": bool,
         "publicAccessCidrs": Sequence[str],
     },
     total=False,
 )
 
-FargateProfileSelectorOutputTypeDef = TypedDict(
-    "FargateProfileSelectorOutputTypeDef",
-    {
-        "namespace": str,
-        "labels": Dict[str, str],
-    },
-    total=False,
-)
-
-FargateProfileSelectorTypeDef = TypedDict(
-    "FargateProfileSelectorTypeDef",
-    {
-        "namespace": str,
-        "labels": Mapping[str, str],
-    },
-    total=False,
-)
-
 LaunchTemplateSpecificationTypeDef = TypedDict(
     "LaunchTemplateSpecificationTypeDef",
     {
         "name": str,
         "version": str,
         "id": str,
     },
@@ -613,14 +599,32 @@
         "errorCode": ErrorCodeType,
         "errorMessage": str,
         "resourceIds": List[str],
     },
     total=False,
 )
 
+FargateProfileSelectorOutputTypeDef = TypedDict(
+    "FargateProfileSelectorOutputTypeDef",
+    {
+        "namespace": str,
+        "labels": Dict[str, str],
+    },
+    total=False,
+)
+
+FargateProfileSelectorTypeDef = TypedDict(
+    "FargateProfileSelectorTypeDef",
+    {
+        "namespace": str,
+        "labels": Mapping[str, str],
+    },
+    total=False,
+)
+
 OidcIdentityProviderConfigTypeDef = TypedDict(
     "OidcIdentityProviderConfigTypeDef",
     {
         "identityProviderConfigName": str,
         "identityProviderConfigArn": str,
         "clusterName": str,
         "issuerUrl": str,
@@ -1059,57 +1063,14 @@
 )
 
 class OutpostConfigResponseTypeDef(
     _RequiredOutpostConfigResponseTypeDef, _OptionalOutpostConfigResponseTypeDef
 ):
     pass
 
-FargateProfileTypeDef = TypedDict(
-    "FargateProfileTypeDef",
-    {
-        "fargateProfileName": str,
-        "fargateProfileArn": str,
-        "clusterName": str,
-        "createdAt": datetime,
-        "podExecutionRoleArn": str,
-        "subnets": List[str],
-        "selectors": List[FargateProfileSelectorOutputTypeDef],
-        "status": FargateProfileStatusType,
-        "tags": Dict[str, str],
-    },
-    total=False,
-)
-
-_RequiredCreateFargateProfileRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateFargateProfileRequestRequestTypeDef",
-    {
-        "fargateProfileName": str,
-        "clusterName": str,
-        "podExecutionRoleArn": str,
-    },
-)
-_OptionalCreateFargateProfileRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateFargateProfileRequestRequestTypeDef",
-    {
-        "subnets": Sequence[str],
-        "selectors": Sequence[
-            Union[FargateProfileSelectorTypeDef, FargateProfileSelectorOutputTypeDef]
-        ],
-        "clientRequestToken": str,
-        "tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-class CreateFargateProfileRequestRequestTypeDef(
-    _RequiredCreateFargateProfileRequestRequestTypeDef,
-    _OptionalCreateFargateProfileRequestRequestTypeDef,
-):
-    pass
-
 _RequiredUpdateNodegroupVersionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateNodegroupVersionRequestRequestTypeDef",
     {
         "clusterName": str,
         "nodegroupName": str,
     },
 )
@@ -1517,14 +1478,33 @@
     {
         "resources": Sequence[str],
         "provider": ProviderTypeDef,
     },
     total=False,
 )
 
+FargateProfileTypeDef = TypedDict(
+    "FargateProfileTypeDef",
+    {
+        "fargateProfileName": str,
+        "fargateProfileArn": str,
+        "clusterName": str,
+        "createdAt": datetime,
+        "podExecutionRoleArn": str,
+        "subnets": List[str],
+        "selectors": List[FargateProfileSelectorOutputTypeDef],
+        "status": FargateProfileStatusType,
+        "tags": Dict[str, str],
+    },
+    total=False,
+)
+
+FargateProfileSelectorUnionTypeDef = Union[
+    FargateProfileSelectorTypeDef, FargateProfileSelectorOutputTypeDef
+]
 IdentityProviderConfigResponseTypeDef = TypedDict(
     "IdentityProviderConfigResponseTypeDef",
     {
         "oidc": OidcIdentityProviderConfigTypeDef,
     },
     total=False,
 )
@@ -1557,14 +1537,15 @@
     "LoggingTypeDef",
     {
         "clusterLogging": Sequence[LogSetupTypeDef],
     },
     total=False,
 )
 
+RemoteAccessConfigUnionTypeDef = Union[RemoteAccessConfigTypeDef, RemoteAccessConfigOutputTypeDef]
 UpdateTypeDef = TypedDict(
     "UpdateTypeDef",
     {
         "id": str,
         "status": UpdateStatusType,
         "type": UpdateTypeType,
         "params": List[UpdateParamTypeDef],
@@ -1604,38 +1585,14 @@
         "publisher": str,
         "owner": str,
         "marketplaceInformation": MarketplaceInformationTypeDef,
     },
     total=False,
 )
 
-CreateFargateProfileResponseTypeDef = TypedDict(
-    "CreateFargateProfileResponseTypeDef",
-    {
-        "fargateProfile": FargateProfileTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteFargateProfileResponseTypeDef = TypedDict(
-    "DeleteFargateProfileResponseTypeDef",
-    {
-        "fargateProfile": FargateProfileTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeFargateProfileResponseTypeDef = TypedDict(
-    "DescribeFargateProfileResponseTypeDef",
-    {
-        "fargateProfile": FargateProfileTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredUpdateNodegroupConfigRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateNodegroupConfigRequestRequestTypeDef",
     {
         "clusterName": str,
         "nodegroupName": str,
     },
 )
@@ -1653,32 +1610,61 @@
 
 class UpdateNodegroupConfigRequestRequestTypeDef(
     _RequiredUpdateNodegroupConfigRequestRequestTypeDef,
     _OptionalUpdateNodegroupConfigRequestRequestTypeDef,
 ):
     pass
 
-_RequiredAssociateEncryptionConfigRequestRequestTypeDef = TypedDict(
-    "_RequiredAssociateEncryptionConfigRequestRequestTypeDef",
+EncryptionConfigUnionTypeDef = Union[EncryptionConfigTypeDef, EncryptionConfigOutputTypeDef]
+CreateFargateProfileResponseTypeDef = TypedDict(
+    "CreateFargateProfileResponseTypeDef",
     {
+        "fargateProfile": FargateProfileTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteFargateProfileResponseTypeDef = TypedDict(
+    "DeleteFargateProfileResponseTypeDef",
+    {
+        "fargateProfile": FargateProfileTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeFargateProfileResponseTypeDef = TypedDict(
+    "DescribeFargateProfileResponseTypeDef",
+    {
+        "fargateProfile": FargateProfileTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredCreateFargateProfileRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateFargateProfileRequestRequestTypeDef",
+    {
+        "fargateProfileName": str,
         "clusterName": str,
-        "encryptionConfig": Sequence[Union[EncryptionConfigTypeDef, EncryptionConfigOutputTypeDef]],
+        "podExecutionRoleArn": str,
     },
 )
-_OptionalAssociateEncryptionConfigRequestRequestTypeDef = TypedDict(
-    "_OptionalAssociateEncryptionConfigRequestRequestTypeDef",
+_OptionalCreateFargateProfileRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateFargateProfileRequestRequestTypeDef",
     {
+        "subnets": Sequence[str],
+        "selectors": Sequence[FargateProfileSelectorUnionTypeDef],
         "clientRequestToken": str,
+        "tags": Mapping[str, str],
     },
     total=False,
 )
 
-class AssociateEncryptionConfigRequestRequestTypeDef(
-    _RequiredAssociateEncryptionConfigRequestRequestTypeDef,
-    _OptionalAssociateEncryptionConfigRequestRequestTypeDef,
+class CreateFargateProfileRequestRequestTypeDef(
+    _RequiredCreateFargateProfileRequestRequestTypeDef,
+    _OptionalCreateFargateProfileRequestRequestTypeDef,
 ):
     pass
 
 DescribeIdentityProviderConfigResponseTypeDef = TypedDict(
     "DescribeIdentityProviderConfigResponseTypeDef",
     {
         "identityProviderConfig": IdentityProviderConfigResponseTypeDef,
@@ -1739,41 +1725,15 @@
         "id": str,
         "health": ClusterHealthTypeDef,
         "outpostConfig": OutpostConfigResponseTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateClusterRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateClusterRequestRequestTypeDef",
-    {
-        "name": str,
-        "roleArn": str,
-        "resourcesVpcConfig": VpcConfigRequestTypeDef,
-    },
-)
-_OptionalCreateClusterRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateClusterRequestRequestTypeDef",
-    {
-        "version": str,
-        "kubernetesNetworkConfig": KubernetesNetworkConfigRequestTypeDef,
-        "logging": LoggingTypeDef,
-        "clientRequestToken": str,
-        "tags": Mapping[str, str],
-        "encryptionConfig": Sequence[Union[EncryptionConfigTypeDef, EncryptionConfigOutputTypeDef]],
-        "outpostConfig": OutpostConfigRequestTypeDef,
-    },
-    total=False,
-)
-
-class CreateClusterRequestRequestTypeDef(
-    _RequiredCreateClusterRequestRequestTypeDef, _OptionalCreateClusterRequestRequestTypeDef
-):
-    pass
-
+LoggingUnionTypeDef = Union[LoggingTypeDef, LoggingOutputTypeDef]
 _RequiredUpdateClusterConfigRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateClusterConfigRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalUpdateClusterConfigRequestRequestTypeDef = TypedDict(
@@ -1894,14 +1854,62 @@
     {
         "addons": List[AddonInfoTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredAssociateEncryptionConfigRequestRequestTypeDef = TypedDict(
+    "_RequiredAssociateEncryptionConfigRequestRequestTypeDef",
+    {
+        "clusterName": str,
+        "encryptionConfig": Sequence[EncryptionConfigUnionTypeDef],
+    },
+)
+_OptionalAssociateEncryptionConfigRequestRequestTypeDef = TypedDict(
+    "_OptionalAssociateEncryptionConfigRequestRequestTypeDef",
+    {
+        "clientRequestToken": str,
+    },
+    total=False,
+)
+
+class AssociateEncryptionConfigRequestRequestTypeDef(
+    _RequiredAssociateEncryptionConfigRequestRequestTypeDef,
+    _OptionalAssociateEncryptionConfigRequestRequestTypeDef,
+):
+    pass
+
+_RequiredCreateClusterRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateClusterRequestRequestTypeDef",
+    {
+        "name": str,
+        "roleArn": str,
+        "resourcesVpcConfig": VpcConfigRequestTypeDef,
+    },
+)
+_OptionalCreateClusterRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateClusterRequestRequestTypeDef",
+    {
+        "version": str,
+        "kubernetesNetworkConfig": KubernetesNetworkConfigRequestTypeDef,
+        "logging": LoggingTypeDef,
+        "clientRequestToken": str,
+        "tags": Mapping[str, str],
+        "encryptionConfig": Sequence[EncryptionConfigUnionTypeDef],
+        "outpostConfig": OutpostConfigRequestTypeDef,
+    },
+    total=False,
+)
+
+class CreateClusterRequestRequestTypeDef(
+    _RequiredCreateClusterRequestRequestTypeDef, _OptionalCreateClusterRequestRequestTypeDef
+):
+    pass
+
 CreateNodegroupResponseTypeDef = TypedDict(
     "CreateNodegroupResponseTypeDef",
     {
         "nodegroup": NodegroupTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks/waiter.py` & `mypy-boto3-eks-1.28.16/mypy_boto3_eks/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks/waiter.pyi` & `mypy-boto3-eks-1.28.16/mypy_boto3_eks/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks.egg-info/PKG-INFO` & `mypy-boto3-eks-1.28.16/mypy_boto3_eks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-eks
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.EKS 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.EKS 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 eks type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 eks type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-eks.svg?color=blue)](https://pypi.org/project/mypy-boto3-eks)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-eks)](https://pepy.tech/project/mypy-boto3-eks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EKS 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS)
+[boto3.EKS 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS)
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
 [mypy-boto3-eks docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/).
 
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
@@ -402,20 +402,20 @@
 )
 
 
 def check_value(value: AMITypesType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_eks.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_eks.type_defs import (
     AddonIssueTypeDef,
     MarketplaceInformationTypeDef,
     CompatibilityTypeDef,
     ResponseMetadataTypeDef,
@@ -428,16 +428,14 @@
     VpcConfigResponseTypeDef,
     ConnectorConfigRequestTypeDef,
     ControlPlanePlacementRequestTypeDef,
     ControlPlanePlacementResponseTypeDef,
     CreateAddonRequestRequestTypeDef,
     KubernetesNetworkConfigRequestTypeDef,
     VpcConfigRequestTypeDef,
-    FargateProfileSelectorOutputTypeDef,
-    FargateProfileSelectorTypeDef,
     LaunchTemplateSpecificationTypeDef,
     NodegroupScalingConfigTypeDef,
     NodegroupUpdateConfigTypeDef,
     RemoteAccessConfigTypeDef,
     TaintTypeDef,
     DeleteAddonRequestRequestTypeDef,
     DeleteClusterRequestRequestTypeDef,
@@ -452,14 +450,16 @@
     DescribeClusterRequestRequestTypeDef,
     DescribeFargateProfileRequestRequestTypeDef,
     IdentityProviderConfigTypeDef,
     DescribeNodegroupRequestRequestTypeDef,
     DescribeUpdateRequestRequestTypeDef,
     ProviderTypeDef,
     ErrorDetailTypeDef,
+    FargateProfileSelectorOutputTypeDef,
+    FargateProfileSelectorTypeDef,
     OidcIdentityProviderConfigTypeDef,
     OIDCTypeDef,
     IssueTypeDef,
     ListAddonsRequestRequestTypeDef,
     ListClustersRequestRequestTypeDef,
     ListFargateProfilesRequestRequestTypeDef,
     ListIdentityProviderConfigsRequestRequestTypeDef,
@@ -486,16 +486,14 @@
     ListUpdatesResponseTypeDef,
     AssociateIdentityProviderConfigRequestRequestTypeDef,
     NodegroupResourcesTypeDef,
     ClusterHealthTypeDef,
     RegisterClusterRequestRequestTypeDef,
     OutpostConfigRequestTypeDef,
     OutpostConfigResponseTypeDef,
-    FargateProfileTypeDef,
-    CreateFargateProfileRequestRequestTypeDef,
     UpdateNodegroupVersionRequestRequestTypeDef,
     CreateNodegroupRequestRequestTypeDef,
     UpdateTaintsPayloadTypeDef,
     DescribeAddonRequestAddonActiveWaitTypeDef,
     DescribeAddonRequestAddonDeletedWaitTypeDef,
     DescribeClusterRequestClusterActiveWaitTypeDef,
     DescribeClusterRequestClusterDeletedWaitTypeDef,
@@ -511,57 +509,63 @@
     ListNodegroupsRequestListNodegroupsPaginateTypeDef,
     ListUpdatesRequestListUpdatesPaginateTypeDef,
     DescribeIdentityProviderConfigRequestRequestTypeDef,
     DisassociateIdentityProviderConfigRequestRequestTypeDef,
     ListIdentityProviderConfigsResponseTypeDef,
     EncryptionConfigOutputTypeDef,
     EncryptionConfigTypeDef,
+    FargateProfileTypeDef,
+    FargateProfileSelectorUnionTypeDef,
     IdentityProviderConfigResponseTypeDef,
     IdentityTypeDef,
     NodegroupHealthTypeDef,
     LoggingOutputTypeDef,
     LoggingTypeDef,
+    RemoteAccessConfigUnionTypeDef,
     UpdateTypeDef,
     AddonTypeDef,
     AddonInfoTypeDef,
+    UpdateNodegroupConfigRequestRequestTypeDef,
+    EncryptionConfigUnionTypeDef,
     CreateFargateProfileResponseTypeDef,
     DeleteFargateProfileResponseTypeDef,
     DescribeFargateProfileResponseTypeDef,
-    UpdateNodegroupConfigRequestRequestTypeDef,
-    AssociateEncryptionConfigRequestRequestTypeDef,
+    CreateFargateProfileRequestRequestTypeDef,
     DescribeIdentityProviderConfigResponseTypeDef,
     NodegroupTypeDef,
     ClusterTypeDef,
-    CreateClusterRequestRequestTypeDef,
+    LoggingUnionTypeDef,
     UpdateClusterConfigRequestRequestTypeDef,
     AssociateEncryptionConfigResponseTypeDef,
     AssociateIdentityProviderConfigResponseTypeDef,
     DescribeUpdateResponseTypeDef,
     DisassociateIdentityProviderConfigResponseTypeDef,
     UpdateAddonResponseTypeDef,
     UpdateClusterConfigResponseTypeDef,
     UpdateClusterVersionResponseTypeDef,
     UpdateNodegroupConfigResponseTypeDef,
     UpdateNodegroupVersionResponseTypeDef,
     CreateAddonResponseTypeDef,
     DeleteAddonResponseTypeDef,
     DescribeAddonResponseTypeDef,
     DescribeAddonVersionsResponseTypeDef,
+    AssociateEncryptionConfigRequestRequestTypeDef,
+    CreateClusterRequestRequestTypeDef,
     CreateNodegroupResponseTypeDef,
     DeleteNodegroupResponseTypeDef,
     DescribeNodegroupResponseTypeDef,
     CreateClusterResponseTypeDef,
     DeleteClusterResponseTypeDef,
     DeregisterClusterResponseTypeDef,
     DescribeClusterResponseTypeDef,
     RegisterClusterResponseTypeDef,
 )
 
 
-def get_structure() -> AddonIssueTypeDef:
+def get_value() -> AddonIssueTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks.egg-info/SOURCES.txt` & `mypy-boto3-eks-1.28.16/mypy_boto3_eks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-eks-1.28.15.post1/setup.py` & `mypy-boto3-eks-1.28.16/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-eks",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_eks"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.EKS 1.28.15 service generated with mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.EKS 1.28.16 service generated with mypy-boto3-builder 7.17.1"
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
-    keywords="boto3 eks type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 eks type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_eks": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

