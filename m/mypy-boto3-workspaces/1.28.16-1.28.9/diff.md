# Comparing `tmp/mypy-boto3-workspaces-1.28.16.tar.gz` & `tmp/mypy-boto3-workspaces-1.28.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-workspaces-1.28.16.tar", last modified: Tue Aug  1 11:38:06 2023, max compression
+gzip compressed data, was "mypy-boto3-workspaces-1.28.9.tar", last modified: Fri Jul 21 20:32:58 2023, max compression
```

## Comparing `mypy-boto3-workspaces-1.28.16.tar` & `mypy-boto3-workspaces-1.28.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:38:06.276654 mypy-boto3-workspaces-1.28.16/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:35:34.000000 mypy-boto3-workspaces-1.28.16/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22211 2023-08-01 11:38:06.272654 mypy-boto3-workspaces-1.28.16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20715 2023-08-01 11:35:34.000000 mypy-boto3-workspaces-1.28.16/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:38:06.272654 mypy-boto3-workspaces-1.28.16/mypy_boto3_workspaces/
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-08-01 11:35:34.000000 mypy-boto3-workspaces-1.28.16/mypy_boto3_workspaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-08-01 11:35:34.000000 mypy-boto3-workspaces-1.28.16/mypy_boto3_workspaces/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-08-01 11:35:34.000000 mypy-boto3-workspaces-1.28.16/mypy_boto3_workspaces/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48085 2023-08-01 11:35:34.000000 mypy-boto3-workspaces-1.28.16/mypy_boto3_workspaces/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    48005 2023-08-01 11:35:34.000000 mypy-boto3-workspaces-1.28.16/mypy_boto3_workspaces/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13354 2023-08-01 11:35:35.000000 mypy-boto3-workspaces-1.28.16/mypy_boto3_workspaces/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13352 2023-08-01 11:35:35.000000 mypy-boto3-workspaces-1.28.16/mypy_boto3_workspaces/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10740 2023-08-01 11:35:35.000000 mypy-boto3-workspaces-1.28.16/mypy_boto3_workspaces/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10730 2023-08-01 11:35:34.000000 mypy-boto3-workspaces-1.28.16/mypy_boto3_workspaces/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:35:34.000000 mypy-boto3-workspaces-1.28.16/mypy_boto3_workspaces/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    55958 2023-08-01 11:35:36.000000 mypy-boto3-workspaces-1.28.16/mypy_boto3_workspaces/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    55913 2023-08-01 11:35:36.000000 mypy-boto3-workspaces-1.28.16/mypy_boto3_workspaces/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:35:34.000000 mypy-boto3-workspaces-1.28.16/mypy_boto3_workspaces/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:38:06.272654 mypy-boto3-workspaces-1.28.16/mypy_boto3_workspaces.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22211 2023-08-01 11:38:06.000000 mypy-boto3-workspaces-1.28.16/mypy_boto3_workspaces.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-01 11:38:06.000000 mypy-boto3-workspaces-1.28.16/mypy_boto3_workspaces.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:38:06.000000 mypy-boto3-workspaces-1.28.16/mypy_boto3_workspaces.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:38:06.000000 mypy-boto3-workspaces-1.28.16/mypy_boto3_workspaces.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:38:06.000000 mypy-boto3-workspaces-1.28.16/mypy_boto3_workspaces.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-01 11:38:06.000000 mypy-boto3-workspaces-1.28.16/mypy_boto3_workspaces.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:38:06.276654 mypy-boto3-workspaces-1.28.16/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-08-01 11:35:34.000000 mypy-boto3-workspaces-1.28.16/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:32:58.251903 mypy-boto3-workspaces-1.28.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-21 20:32:46.000000 mypy-boto3-workspaces-1.28.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22493 2023-07-21 20:32:58.243903 mypy-boto3-workspaces-1.28.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20996 2023-07-21 20:32:46.000000 mypy-boto3-workspaces-1.28.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:32:58.243903 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-07-21 20:32:46.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-07-21 20:32:46.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-21 20:32:46.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48055 2023-07-21 20:32:47.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47975 2023-07-21 20:32:46.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13299 2023-07-21 20:32:47.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13297 2023-07-21 20:32:47.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10740 2023-07-21 20:32:47.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10730 2023-07-21 20:32:47.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 20:32:46.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    57338 2023-07-21 20:32:48.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57297 2023-07-21 20:32:47.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-21 20:32:46.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:32:58.243903 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22493 2023-07-21 20:32:58.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-21 20:32:58.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 20:32:58.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 20:32:58.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-21 20:32:58.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-21 20:32:58.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 20:32:58.251903 mypy-boto3-workspaces-1.28.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-21 20:32:46.000000 mypy-boto3-workspaces-1.28.9/setup.py
```

### Comparing `mypy-boto3-workspaces-1.28.16/LICENSE` & `mypy-boto3-workspaces-1.28.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workspaces-1.28.16/PKG-INFO` & `mypy-boto3-workspaces-1.28.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-workspaces
-Version: 1.28.16
-Summary: Type annotations for boto3.WorkSpaces 1.28.16 service generated with mypy-boto3-builder 7.17.1
+Version: 1.28.9
+Summary: Type annotations for boto3.WorkSpaces 1.28.9 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 workspaces type-annotations botocore mypy typeshed autocomplete
+Keywords: boto3 workspaces type-annotations boto3-stubs mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-workspaces"></a>
 
 # mypy-boto3-workspaces
 
 [![PyPI - mypy-boto3-workspaces](https://img.shields.io/pypi/v/mypy-boto3-workspaces.svg?color=blue)](https://pypi.org/project/mypy-boto3-workspaces)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-workspaces.svg?color=blue)](https://pypi.org/project/mypy-boto3-workspaces)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-workspaces)](https://pepy.tech/project/mypy-boto3-workspaces)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-workspaces?color=blue)](https://pypistats.org/packages/mypy-boto3-workspaces)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WorkSpaces 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces)
+[boto3.WorkSpaces 1.28.9](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.17.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-workspaces docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/).
 
 See how it helps to find and fix potential bugs:
 
@@ -74,15 +74,15 @@
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Literals](#literals)
-    - [Type definitions](#type-definitions)
+    - [Typed dictionaries](#typed-dictionaries)
   - [How it works](#how-it-works)
   - [What's new](#what's-new)
     - [Implemented features](#implemented-features)
     - [Latest changes](#latest-changes)
   - [Versioning](#versioning)
   - [Thank you](#thank-you)
   - [Documentation](#documentation)
@@ -379,42 +379,46 @@
 )
 
 
 def check_value(value: AccessPropertyValueType) -> bool:
     ...
 ```
 
-<a id="type-definitions"></a>
+<a id="typed-dictionaries"></a>
 
-### Type definitions
+### Typed dictionaries
 
 `mypy_boto3_workspaces.type_defs` module contains structures and shapes
-assembled to typed dictionaries and unions for additional type checking.
+assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_workspaces.type_defs import (
     AccountModificationTypeDef,
     AssociateConnectionAliasRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     AssociateIpGroupsRequestRequestTypeDef,
     IpRuleItemTypeDef,
-    BlobTypeDef,
+    CertificateBasedAuthPropertiesOutputTypeDef,
     CertificateBasedAuthPropertiesTypeDef,
+    ClientPropertiesOutputTypeDef,
     ClientPropertiesTypeDef,
+    ComputeTypeOutputTypeDef,
     ComputeTypeTypeDef,
     ConnectClientAddInTypeDef,
     ConnectionAliasAssociationTypeDef,
+    ConnectionAliasPermissionOutputTypeDef,
     ConnectionAliasPermissionTypeDef,
     TagTypeDef,
     CreateConnectClientAddInRequestRequestTypeDef,
     PendingCreateStandbyWorkspacesRequestTypeDef,
     RootStorageTypeDef,
     UserStorageTypeDef,
     OperatingSystemTypeDef,
     DefaultClientBrandingAttributesTypeDef,
+    DefaultImportClientBrandingAttributesTypeDef,
     DefaultWorkspaceCreationPropertiesTypeDef,
     DeleteClientBrandingRequestRequestTypeDef,
     DeleteConnectClientAddInRequestRequestTypeDef,
     DeleteConnectionAliasRequestRequestTypeDef,
     DeleteIpGroupRequestRequestTypeDef,
     DeleteTagsRequestRequestTypeDef,
     DeleteWorkspaceBundleRequestRequestTypeDef,
@@ -426,27 +430,30 @@
     IosClientBrandingAttributesTypeDef,
     DescribeClientPropertiesRequestRequestTypeDef,
     DescribeConnectClientAddInsRequestRequestTypeDef,
     DescribeConnectionAliasPermissionsRequestRequestTypeDef,
     DescribeConnectionAliasesRequestRequestTypeDef,
     DescribeIpGroupsRequestRequestTypeDef,
     DescribeTagsRequestRequestTypeDef,
+    TagOutputTypeDef,
     DescribeWorkspaceBundlesRequestRequestTypeDef,
     DescribeWorkspaceDirectoriesRequestRequestTypeDef,
     DescribeWorkspaceImagePermissionsRequestRequestTypeDef,
     ImagePermissionTypeDef,
     DescribeWorkspaceImagesRequestRequestTypeDef,
     DescribeWorkspaceSnapshotsRequestRequestTypeDef,
     SnapshotTypeDef,
     DescribeWorkspacesConnectionStatusRequestRequestTypeDef,
     WorkspaceConnectionStatusTypeDef,
     DescribeWorkspacesRequestRequestTypeDef,
     DisassociateConnectionAliasRequestRequestTypeDef,
     DisassociateIpGroupsRequestRequestTypeDef,
     FailedWorkspaceChangeRequestTypeDef,
+    IosImportClientBrandingAttributesTypeDef,
+    IpRuleItemOutputTypeDef,
     ListAvailableManagementCidrRangesRequestRequestTypeDef,
     MigrateWorkspaceRequestRequestTypeDef,
     ModificationStateTypeDef,
     ModifyAccountRequestRequestTypeDef,
     SamlPropertiesTypeDef,
     SelfservicePermissionsTypeDef,
     WorkspaceAccessPropertiesTypeDef,
@@ -454,114 +461,114 @@
     WorkspacePropertiesTypeDef,
     ModifyWorkspaceStateRequestRequestTypeDef,
     RebootRequestTypeDef,
     RebuildRequestTypeDef,
     RelatedWorkspacePropertiesTypeDef,
     RestoreWorkspaceRequestRequestTypeDef,
     RevokeIpRulesRequestRequestTypeDef,
+    RootStorageOutputTypeDef,
+    SamlPropertiesOutputTypeDef,
+    SelfservicePermissionsOutputTypeDef,
     StartRequestTypeDef,
     StopRequestTypeDef,
     TerminateRequestTypeDef,
     UpdateConnectClientAddInRequestRequestTypeDef,
     UpdateResultTypeDef,
     UpdateWorkspaceBundleRequestRequestTypeDef,
     UpdateWorkspaceImagePermissionRequestRequestTypeDef,
+    UserStorageOutputTypeDef,
+    WorkspaceAccessPropertiesOutputTypeDef,
     WorkspacePropertiesOutputTypeDef,
     AssociateConnectionAliasResultTypeDef,
     CopyWorkspaceImageResultTypeDef,
     CreateConnectClientAddInResultTypeDef,
     CreateConnectionAliasResultTypeDef,
     CreateIpGroupResultTypeDef,
     CreateUpdatedWorkspaceImageResultTypeDef,
     DescribeAccountModificationsResultTypeDef,
     DescribeAccountResultTypeDef,
     ImportWorkspaceImageResultTypeDef,
     ListAvailableManagementCidrRangesResultTypeDef,
     MigrateWorkspaceResultTypeDef,
     AuthorizeIpRulesRequestRequestTypeDef,
     UpdateRulesOfIpGroupRequestRequestTypeDef,
-    WorkspacesIpGroupTypeDef,
-    DefaultImportClientBrandingAttributesTypeDef,
-    IosImportClientBrandingAttributesTypeDef,
     ModifyCertificateBasedAuthPropertiesRequestRequestTypeDef,
     ClientPropertiesResultTypeDef,
     ModifyClientPropertiesRequestRequestTypeDef,
     DescribeConnectClientAddInsResultTypeDef,
     ConnectionAliasTypeDef,
     DescribeConnectionAliasPermissionsResultTypeDef,
     UpdateConnectionAliasPermissionRequestRequestTypeDef,
     CopyWorkspaceImageRequestRequestTypeDef,
     CreateConnectionAliasRequestRequestTypeDef,
     CreateIpGroupRequestRequestTypeDef,
     CreateTagsRequestRequestTypeDef,
     CreateUpdatedWorkspaceImageRequestRequestTypeDef,
     CreateWorkspaceImageRequestRequestTypeDef,
-    DescribeTagsResultTypeDef,
     ImportWorkspaceImageRequestRequestTypeDef,
     RegisterWorkspaceDirectoryRequestRequestTypeDef,
-    StandbyWorkspaceOutputTypeDef,
     StandbyWorkspaceTypeDef,
     CreateWorkspaceBundleRequestRequestTypeDef,
-    WorkspaceBundleTypeDef,
     CreateWorkspaceImageResultTypeDef,
     DescribeAccountModificationsRequestDescribeAccountModificationsPaginateTypeDef,
     DescribeIpGroupsRequestDescribeIpGroupsPaginateTypeDef,
     DescribeWorkspaceBundlesRequestDescribeWorkspaceBundlesPaginateTypeDef,
     DescribeWorkspaceDirectoriesRequestDescribeWorkspaceDirectoriesPaginateTypeDef,
     DescribeWorkspaceImagesRequestDescribeWorkspaceImagesPaginateTypeDef,
     DescribeWorkspacesConnectionStatusRequestDescribeWorkspacesConnectionStatusPaginateTypeDef,
     DescribeWorkspacesRequestDescribeWorkspacesPaginateTypeDef,
     ListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef,
     DescribeClientBrandingResultTypeDef,
     ImportClientBrandingResultTypeDef,
+    DescribeTagsResultTypeDef,
+    StandbyWorkspaceOutputTypeDef,
     DescribeWorkspaceImagePermissionsResultTypeDef,
     DescribeWorkspaceSnapshotsResultTypeDef,
     DescribeWorkspacesConnectionStatusResultTypeDef,
     RebootWorkspacesResultTypeDef,
     RebuildWorkspacesResultTypeDef,
     StartWorkspacesResultTypeDef,
     StopWorkspacesResultTypeDef,
     TerminateWorkspacesResultTypeDef,
+    ImportClientBrandingRequestRequestTypeDef,
+    WorkspacesIpGroupTypeDef,
     ModifySamlPropertiesRequestRequestTypeDef,
     ModifySelfservicePermissionsRequestRequestTypeDef,
     ModifyWorkspaceAccessPropertiesRequestRequestTypeDef,
-    WorkspaceDirectoryTypeDef,
     ModifyWorkspaceCreationPropertiesRequestRequestTypeDef,
     ModifyWorkspacePropertiesRequestRequestTypeDef,
     WorkspaceRequestTypeDef,
     RebootWorkspacesRequestRequestTypeDef,
     RebuildWorkspacesRequestRequestTypeDef,
     StartWorkspacesRequestRequestTypeDef,
     StopWorkspacesRequestRequestTypeDef,
     TerminateWorkspacesRequestRequestTypeDef,
     WorkspaceImageTypeDef,
-    WorkspacePropertiesUnionTypeDef,
+    WorkspaceBundleTypeDef,
+    WorkspaceDirectoryTypeDef,
     WorkspaceRequestOutputTypeDef,
     WorkspaceTypeDef,
-    DescribeIpGroupsResultTypeDef,
-    ImportClientBrandingRequestRequestTypeDef,
     DescribeClientPropertiesResultTypeDef,
     DescribeConnectionAliasesResultTypeDef,
+    CreateStandbyWorkspacesRequestRequestTypeDef,
     FailedCreateStandbyWorkspacesRequestTypeDef,
-    StandbyWorkspaceUnionTypeDef,
+    DescribeIpGroupsResultTypeDef,
+    CreateWorkspacesRequestRequestTypeDef,
+    DescribeWorkspaceImagesResultTypeDef,
     CreateWorkspaceBundleResultTypeDef,
     DescribeWorkspaceBundlesResultTypeDef,
     DescribeWorkspaceDirectoriesResultTypeDef,
-    DescribeWorkspaceImagesResultTypeDef,
     FailedCreateWorkspaceRequestTypeDef,
-    WorkspaceRequestUnionTypeDef,
     DescribeWorkspacesResultTypeDef,
     CreateStandbyWorkspacesResultTypeDef,
-    CreateStandbyWorkspacesRequestRequestTypeDef,
     CreateWorkspacesResultTypeDef,
-    CreateWorkspacesRequestRequestTypeDef,
 )
 
 
-def get_value() -> AccountModificationTypeDef:
+def get_structure() -> AccountModificationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-workspaces-1.28.16/README.md` & `mypy-boto3-workspaces-1.28.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-workspaces"></a>
 
 # mypy-boto3-workspaces
 
 [![PyPI - mypy-boto3-workspaces](https://img.shields.io/pypi/v/mypy-boto3-workspaces.svg?color=blue)](https://pypi.org/project/mypy-boto3-workspaces)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-workspaces.svg?color=blue)](https://pypi.org/project/mypy-boto3-workspaces)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-workspaces)](https://pepy.tech/project/mypy-boto3-workspaces)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-workspaces?color=blue)](https://pypistats.org/packages/mypy-boto3-workspaces)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WorkSpaces 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces)
+[boto3.WorkSpaces 1.28.9](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.17.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-workspaces docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/).
 
 See how it helps to find and fix potential bugs:
 
@@ -42,15 +42,15 @@
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Literals](#literals)
-    - [Type definitions](#type-definitions)
+    - [Typed dictionaries](#typed-dictionaries)
   - [How it works](#how-it-works)
   - [What's new](#what's-new)
     - [Implemented features](#implemented-features)
     - [Latest changes](#latest-changes)
   - [Versioning](#versioning)
   - [Thank you](#thank-you)
   - [Documentation](#documentation)
@@ -347,42 +347,46 @@
 )
 
 
 def check_value(value: AccessPropertyValueType) -> bool:
     ...
 ```
 
-<a id="type-definitions"></a>
+<a id="typed-dictionaries"></a>
 
-### Type definitions
+### Typed dictionaries
 
 `mypy_boto3_workspaces.type_defs` module contains structures and shapes
-assembled to typed dictionaries and unions for additional type checking.
+assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_workspaces.type_defs import (
     AccountModificationTypeDef,
     AssociateConnectionAliasRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     AssociateIpGroupsRequestRequestTypeDef,
     IpRuleItemTypeDef,
-    BlobTypeDef,
+    CertificateBasedAuthPropertiesOutputTypeDef,
     CertificateBasedAuthPropertiesTypeDef,
+    ClientPropertiesOutputTypeDef,
     ClientPropertiesTypeDef,
+    ComputeTypeOutputTypeDef,
     ComputeTypeTypeDef,
     ConnectClientAddInTypeDef,
     ConnectionAliasAssociationTypeDef,
+    ConnectionAliasPermissionOutputTypeDef,
     ConnectionAliasPermissionTypeDef,
     TagTypeDef,
     CreateConnectClientAddInRequestRequestTypeDef,
     PendingCreateStandbyWorkspacesRequestTypeDef,
     RootStorageTypeDef,
     UserStorageTypeDef,
     OperatingSystemTypeDef,
     DefaultClientBrandingAttributesTypeDef,
+    DefaultImportClientBrandingAttributesTypeDef,
     DefaultWorkspaceCreationPropertiesTypeDef,
     DeleteClientBrandingRequestRequestTypeDef,
     DeleteConnectClientAddInRequestRequestTypeDef,
     DeleteConnectionAliasRequestRequestTypeDef,
     DeleteIpGroupRequestRequestTypeDef,
     DeleteTagsRequestRequestTypeDef,
     DeleteWorkspaceBundleRequestRequestTypeDef,
@@ -394,27 +398,30 @@
     IosClientBrandingAttributesTypeDef,
     DescribeClientPropertiesRequestRequestTypeDef,
     DescribeConnectClientAddInsRequestRequestTypeDef,
     DescribeConnectionAliasPermissionsRequestRequestTypeDef,
     DescribeConnectionAliasesRequestRequestTypeDef,
     DescribeIpGroupsRequestRequestTypeDef,
     DescribeTagsRequestRequestTypeDef,
+    TagOutputTypeDef,
     DescribeWorkspaceBundlesRequestRequestTypeDef,
     DescribeWorkspaceDirectoriesRequestRequestTypeDef,
     DescribeWorkspaceImagePermissionsRequestRequestTypeDef,
     ImagePermissionTypeDef,
     DescribeWorkspaceImagesRequestRequestTypeDef,
     DescribeWorkspaceSnapshotsRequestRequestTypeDef,
     SnapshotTypeDef,
     DescribeWorkspacesConnectionStatusRequestRequestTypeDef,
     WorkspaceConnectionStatusTypeDef,
     DescribeWorkspacesRequestRequestTypeDef,
     DisassociateConnectionAliasRequestRequestTypeDef,
     DisassociateIpGroupsRequestRequestTypeDef,
     FailedWorkspaceChangeRequestTypeDef,
+    IosImportClientBrandingAttributesTypeDef,
+    IpRuleItemOutputTypeDef,
     ListAvailableManagementCidrRangesRequestRequestTypeDef,
     MigrateWorkspaceRequestRequestTypeDef,
     ModificationStateTypeDef,
     ModifyAccountRequestRequestTypeDef,
     SamlPropertiesTypeDef,
     SelfservicePermissionsTypeDef,
     WorkspaceAccessPropertiesTypeDef,
@@ -422,114 +429,114 @@
     WorkspacePropertiesTypeDef,
     ModifyWorkspaceStateRequestRequestTypeDef,
     RebootRequestTypeDef,
     RebuildRequestTypeDef,
     RelatedWorkspacePropertiesTypeDef,
     RestoreWorkspaceRequestRequestTypeDef,
     RevokeIpRulesRequestRequestTypeDef,
+    RootStorageOutputTypeDef,
+    SamlPropertiesOutputTypeDef,
+    SelfservicePermissionsOutputTypeDef,
     StartRequestTypeDef,
     StopRequestTypeDef,
     TerminateRequestTypeDef,
     UpdateConnectClientAddInRequestRequestTypeDef,
     UpdateResultTypeDef,
     UpdateWorkspaceBundleRequestRequestTypeDef,
     UpdateWorkspaceImagePermissionRequestRequestTypeDef,
+    UserStorageOutputTypeDef,
+    WorkspaceAccessPropertiesOutputTypeDef,
     WorkspacePropertiesOutputTypeDef,
     AssociateConnectionAliasResultTypeDef,
     CopyWorkspaceImageResultTypeDef,
     CreateConnectClientAddInResultTypeDef,
     CreateConnectionAliasResultTypeDef,
     CreateIpGroupResultTypeDef,
     CreateUpdatedWorkspaceImageResultTypeDef,
     DescribeAccountModificationsResultTypeDef,
     DescribeAccountResultTypeDef,
     ImportWorkspaceImageResultTypeDef,
     ListAvailableManagementCidrRangesResultTypeDef,
     MigrateWorkspaceResultTypeDef,
     AuthorizeIpRulesRequestRequestTypeDef,
     UpdateRulesOfIpGroupRequestRequestTypeDef,
-    WorkspacesIpGroupTypeDef,
-    DefaultImportClientBrandingAttributesTypeDef,
-    IosImportClientBrandingAttributesTypeDef,
     ModifyCertificateBasedAuthPropertiesRequestRequestTypeDef,
     ClientPropertiesResultTypeDef,
     ModifyClientPropertiesRequestRequestTypeDef,
     DescribeConnectClientAddInsResultTypeDef,
     ConnectionAliasTypeDef,
     DescribeConnectionAliasPermissionsResultTypeDef,
     UpdateConnectionAliasPermissionRequestRequestTypeDef,
     CopyWorkspaceImageRequestRequestTypeDef,
     CreateConnectionAliasRequestRequestTypeDef,
     CreateIpGroupRequestRequestTypeDef,
     CreateTagsRequestRequestTypeDef,
     CreateUpdatedWorkspaceImageRequestRequestTypeDef,
     CreateWorkspaceImageRequestRequestTypeDef,
-    DescribeTagsResultTypeDef,
     ImportWorkspaceImageRequestRequestTypeDef,
     RegisterWorkspaceDirectoryRequestRequestTypeDef,
-    StandbyWorkspaceOutputTypeDef,
     StandbyWorkspaceTypeDef,
     CreateWorkspaceBundleRequestRequestTypeDef,
-    WorkspaceBundleTypeDef,
     CreateWorkspaceImageResultTypeDef,
     DescribeAccountModificationsRequestDescribeAccountModificationsPaginateTypeDef,
     DescribeIpGroupsRequestDescribeIpGroupsPaginateTypeDef,
     DescribeWorkspaceBundlesRequestDescribeWorkspaceBundlesPaginateTypeDef,
     DescribeWorkspaceDirectoriesRequestDescribeWorkspaceDirectoriesPaginateTypeDef,
     DescribeWorkspaceImagesRequestDescribeWorkspaceImagesPaginateTypeDef,
     DescribeWorkspacesConnectionStatusRequestDescribeWorkspacesConnectionStatusPaginateTypeDef,
     DescribeWorkspacesRequestDescribeWorkspacesPaginateTypeDef,
     ListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef,
     DescribeClientBrandingResultTypeDef,
     ImportClientBrandingResultTypeDef,
+    DescribeTagsResultTypeDef,
+    StandbyWorkspaceOutputTypeDef,
     DescribeWorkspaceImagePermissionsResultTypeDef,
     DescribeWorkspaceSnapshotsResultTypeDef,
     DescribeWorkspacesConnectionStatusResultTypeDef,
     RebootWorkspacesResultTypeDef,
     RebuildWorkspacesResultTypeDef,
     StartWorkspacesResultTypeDef,
     StopWorkspacesResultTypeDef,
     TerminateWorkspacesResultTypeDef,
+    ImportClientBrandingRequestRequestTypeDef,
+    WorkspacesIpGroupTypeDef,
     ModifySamlPropertiesRequestRequestTypeDef,
     ModifySelfservicePermissionsRequestRequestTypeDef,
     ModifyWorkspaceAccessPropertiesRequestRequestTypeDef,
-    WorkspaceDirectoryTypeDef,
     ModifyWorkspaceCreationPropertiesRequestRequestTypeDef,
     ModifyWorkspacePropertiesRequestRequestTypeDef,
     WorkspaceRequestTypeDef,
     RebootWorkspacesRequestRequestTypeDef,
     RebuildWorkspacesRequestRequestTypeDef,
     StartWorkspacesRequestRequestTypeDef,
     StopWorkspacesRequestRequestTypeDef,
     TerminateWorkspacesRequestRequestTypeDef,
     WorkspaceImageTypeDef,
-    WorkspacePropertiesUnionTypeDef,
+    WorkspaceBundleTypeDef,
+    WorkspaceDirectoryTypeDef,
     WorkspaceRequestOutputTypeDef,
     WorkspaceTypeDef,
-    DescribeIpGroupsResultTypeDef,
-    ImportClientBrandingRequestRequestTypeDef,
     DescribeClientPropertiesResultTypeDef,
     DescribeConnectionAliasesResultTypeDef,
+    CreateStandbyWorkspacesRequestRequestTypeDef,
     FailedCreateStandbyWorkspacesRequestTypeDef,
-    StandbyWorkspaceUnionTypeDef,
+    DescribeIpGroupsResultTypeDef,
+    CreateWorkspacesRequestRequestTypeDef,
+    DescribeWorkspaceImagesResultTypeDef,
     CreateWorkspaceBundleResultTypeDef,
     DescribeWorkspaceBundlesResultTypeDef,
     DescribeWorkspaceDirectoriesResultTypeDef,
-    DescribeWorkspaceImagesResultTypeDef,
     FailedCreateWorkspaceRequestTypeDef,
-    WorkspaceRequestUnionTypeDef,
     DescribeWorkspacesResultTypeDef,
     CreateStandbyWorkspacesResultTypeDef,
-    CreateStandbyWorkspacesRequestRequestTypeDef,
     CreateWorkspacesResultTypeDef,
-    CreateWorkspacesRequestRequestTypeDef,
 )
 
 
-def get_value() -> AccountModificationTypeDef:
+def get_structure() -> AccountModificationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-workspaces-1.28.16/mypy_boto3_workspaces/__init__.py` & `mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workspaces-1.28.16/mypy_boto3_workspaces/__init__.pyi` & `mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workspaces-1.28.16/mypy_boto3_workspaces/__main__.py` & `mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.WorkSpaces 1.28.16\nVersion:         1.28.16\nBuilder version:"
-        " 7.17.1\nDocs:           "
+        "Type annotations for boto3.WorkSpaces 1.28.9\nVersion:         1.28.9\nBuilder version:"
+        " 7.15.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.16")
+    print("1.28.9")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-workspaces-1.28.16/mypy_boto3_workspaces/client.py` & `mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,27 +78,27 @@
     RebootRequestTypeDef,
     RebootWorkspacesResultTypeDef,
     RebuildRequestTypeDef,
     RebuildWorkspacesResultTypeDef,
     RootStorageTypeDef,
     SamlPropertiesTypeDef,
     SelfservicePermissionsTypeDef,
-    StandbyWorkspaceUnionTypeDef,
+    StandbyWorkspaceTypeDef,
     StartRequestTypeDef,
     StartWorkspacesResultTypeDef,
     StopRequestTypeDef,
     StopWorkspacesResultTypeDef,
     TagTypeDef,
     TerminateRequestTypeDef,
     TerminateWorkspacesResultTypeDef,
     UserStorageTypeDef,
     WorkspaceAccessPropertiesTypeDef,
     WorkspaceCreationPropertiesTypeDef,
-    WorkspacePropertiesUnionTypeDef,
-    WorkspaceRequestUnionTypeDef,
+    WorkspacePropertiesTypeDef,
+    WorkspaceRequestTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -242,15 +242,15 @@
         Creates an IP access control group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.create_ip_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/client/#create_ip_group)
         """
 
     def create_standby_workspaces(
-        self, *, PrimaryRegion: str, StandbyWorkspaces: Sequence[StandbyWorkspaceUnionTypeDef]
+        self, *, PrimaryRegion: str, StandbyWorkspaces: Sequence[StandbyWorkspaceTypeDef]
     ) -> CreateStandbyWorkspacesResultTypeDef:
         """
         Creates a standby WorkSpace in a secondary Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.create_standby_workspaces)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/client/#create_standby_workspaces)
         """
@@ -298,15 +298,15 @@
         Creates a new WorkSpace image from an existing WorkSpace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.create_workspace_image)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/client/#create_workspace_image)
         """
 
     def create_workspaces(
-        self, *, Workspaces: Sequence[WorkspaceRequestUnionTypeDef]
+        self, *, Workspaces: Sequence[WorkspaceRequestTypeDef]
     ) -> CreateWorkspacesResultTypeDef:
         """
         Creates one or more WorkSpaces.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.create_workspaces)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/client/#create_workspaces)
         """
@@ -732,15 +732,15 @@
         Modify the default properties used to create WorkSpaces.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.modify_workspace_creation_properties)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/client/#modify_workspace_creation_properties)
         """
 
     def modify_workspace_properties(
-        self, *, WorkspaceId: str, WorkspaceProperties: WorkspacePropertiesUnionTypeDef
+        self, *, WorkspaceId: str, WorkspaceProperties: WorkspacePropertiesTypeDef
     ) -> Dict[str, Any]:
         """
         Modifies the specified WorkSpace properties.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.modify_workspace_properties)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/client/#modify_workspace_properties)
         """
```

### Comparing `mypy-boto3-workspaces-1.28.16/mypy_boto3_workspaces/client.pyi` & `mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -78,27 +78,27 @@
     RebootRequestTypeDef,
     RebootWorkspacesResultTypeDef,
     RebuildRequestTypeDef,
     RebuildWorkspacesResultTypeDef,
     RootStorageTypeDef,
     SamlPropertiesTypeDef,
     SelfservicePermissionsTypeDef,
-    StandbyWorkspaceUnionTypeDef,
+    StandbyWorkspaceTypeDef,
     StartRequestTypeDef,
     StartWorkspacesResultTypeDef,
     StopRequestTypeDef,
     StopWorkspacesResultTypeDef,
     TagTypeDef,
     TerminateRequestTypeDef,
     TerminateWorkspacesResultTypeDef,
     UserStorageTypeDef,
     WorkspaceAccessPropertiesTypeDef,
     WorkspaceCreationPropertiesTypeDef,
-    WorkspacePropertiesUnionTypeDef,
-    WorkspaceRequestUnionTypeDef,
+    WorkspacePropertiesTypeDef,
+    WorkspaceRequestTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -228,15 +228,15 @@
         """
         Creates an IP access control group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.create_ip_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/client/#create_ip_group)
         """
     def create_standby_workspaces(
-        self, *, PrimaryRegion: str, StandbyWorkspaces: Sequence[StandbyWorkspaceUnionTypeDef]
+        self, *, PrimaryRegion: str, StandbyWorkspaces: Sequence[StandbyWorkspaceTypeDef]
     ) -> CreateStandbyWorkspacesResultTypeDef:
         """
         Creates a standby WorkSpace in a secondary Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.create_standby_workspaces)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/client/#create_standby_workspaces)
         """
@@ -279,15 +279,15 @@
         """
         Creates a new WorkSpace image from an existing WorkSpace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.create_workspace_image)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/client/#create_workspace_image)
         """
     def create_workspaces(
-        self, *, Workspaces: Sequence[WorkspaceRequestUnionTypeDef]
+        self, *, Workspaces: Sequence[WorkspaceRequestTypeDef]
     ) -> CreateWorkspacesResultTypeDef:
         """
         Creates one or more WorkSpaces.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.create_workspaces)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/client/#create_workspaces)
         """
@@ -674,15 +674,15 @@
         """
         Modify the default properties used to create WorkSpaces.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.modify_workspace_creation_properties)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/client/#modify_workspace_creation_properties)
         """
     def modify_workspace_properties(
-        self, *, WorkspaceId: str, WorkspaceProperties: WorkspacePropertiesUnionTypeDef
+        self, *, WorkspaceId: str, WorkspaceProperties: WorkspacePropertiesTypeDef
     ) -> Dict[str, Any]:
         """
         Modifies the specified WorkSpace properties.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.modify_workspace_properties)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/client/#modify_workspace_properties)
         """
```

### Comparing `mypy-boto3-workspaces-1.28.16/mypy_boto3_workspaces/literals.py` & `mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -281,15 +281,14 @@
     "elasticbeanstalk",
     "elastictranscoder",
     "elb",
     "elbv2",
     "emr",
     "emr-containers",
     "emr-serverless",
-    "entityresolution",
     "es",
     "events",
     "evidently",
     "finspace",
     "finspace-data",
     "firehose",
     "fis",
@@ -368,15 +367,14 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie",
     "macie2",
     "managedblockchain",
-    "managedblockchain-query",
     "marketplace-catalog",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
```

### Comparing `mypy-boto3-workspaces-1.28.16/mypy_boto3_workspaces/literals.pyi` & `mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -279,15 +279,14 @@
     "elasticbeanstalk",
     "elastictranscoder",
     "elb",
     "elbv2",
     "emr",
     "emr-containers",
     "emr-serverless",
-    "entityresolution",
     "es",
     "events",
     "evidently",
     "finspace",
     "finspace-data",
     "firehose",
     "fis",
@@ -366,15 +365,14 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie",
     "macie2",
     "managedblockchain",
-    "managedblockchain-query",
     "marketplace-catalog",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
```

### Comparing `mypy-boto3-workspaces-1.28.16/mypy_boto3_workspaces/paginator.py` & `mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workspaces-1.28.16/mypy_boto3_workspaces/paginator.pyi` & `mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workspaces-1.28.16/mypy_boto3_workspaces/type_defs.py` & `mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_workspaces.type_defs import AccountModificationTypeDef
 
-    data: AccountModificationTypeDef = ...
+    data: AccountModificationTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -63,28 +63,32 @@
 
 __all__ = (
     "AccountModificationTypeDef",
     "AssociateConnectionAliasRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AssociateIpGroupsRequestRequestTypeDef",
     "IpRuleItemTypeDef",
-    "BlobTypeDef",
+    "CertificateBasedAuthPropertiesOutputTypeDef",
     "CertificateBasedAuthPropertiesTypeDef",
+    "ClientPropertiesOutputTypeDef",
     "ClientPropertiesTypeDef",
+    "ComputeTypeOutputTypeDef",
     "ComputeTypeTypeDef",
     "ConnectClientAddInTypeDef",
     "ConnectionAliasAssociationTypeDef",
+    "ConnectionAliasPermissionOutputTypeDef",
     "ConnectionAliasPermissionTypeDef",
     "TagTypeDef",
     "CreateConnectClientAddInRequestRequestTypeDef",
     "PendingCreateStandbyWorkspacesRequestTypeDef",
     "RootStorageTypeDef",
     "UserStorageTypeDef",
     "OperatingSystemTypeDef",
     "DefaultClientBrandingAttributesTypeDef",
+    "DefaultImportClientBrandingAttributesTypeDef",
     "DefaultWorkspaceCreationPropertiesTypeDef",
     "DeleteClientBrandingRequestRequestTypeDef",
     "DeleteConnectClientAddInRequestRequestTypeDef",
     "DeleteConnectionAliasRequestRequestTypeDef",
     "DeleteIpGroupRequestRequestTypeDef",
     "DeleteTagsRequestRequestTypeDef",
     "DeleteWorkspaceBundleRequestRequestTypeDef",
@@ -96,27 +100,30 @@
     "IosClientBrandingAttributesTypeDef",
     "DescribeClientPropertiesRequestRequestTypeDef",
     "DescribeConnectClientAddInsRequestRequestTypeDef",
     "DescribeConnectionAliasPermissionsRequestRequestTypeDef",
     "DescribeConnectionAliasesRequestRequestTypeDef",
     "DescribeIpGroupsRequestRequestTypeDef",
     "DescribeTagsRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "DescribeWorkspaceBundlesRequestRequestTypeDef",
     "DescribeWorkspaceDirectoriesRequestRequestTypeDef",
     "DescribeWorkspaceImagePermissionsRequestRequestTypeDef",
     "ImagePermissionTypeDef",
     "DescribeWorkspaceImagesRequestRequestTypeDef",
     "DescribeWorkspaceSnapshotsRequestRequestTypeDef",
     "SnapshotTypeDef",
     "DescribeWorkspacesConnectionStatusRequestRequestTypeDef",
     "WorkspaceConnectionStatusTypeDef",
     "DescribeWorkspacesRequestRequestTypeDef",
     "DisassociateConnectionAliasRequestRequestTypeDef",
     "DisassociateIpGroupsRequestRequestTypeDef",
     "FailedWorkspaceChangeRequestTypeDef",
+    "IosImportClientBrandingAttributesTypeDef",
+    "IpRuleItemOutputTypeDef",
     "ListAvailableManagementCidrRangesRequestRequestTypeDef",
     "MigrateWorkspaceRequestRequestTypeDef",
     "ModificationStateTypeDef",
     "ModifyAccountRequestRequestTypeDef",
     "SamlPropertiesTypeDef",
     "SelfservicePermissionsTypeDef",
     "WorkspaceAccessPropertiesTypeDef",
@@ -124,123 +131,122 @@
     "WorkspacePropertiesTypeDef",
     "ModifyWorkspaceStateRequestRequestTypeDef",
     "RebootRequestTypeDef",
     "RebuildRequestTypeDef",
     "RelatedWorkspacePropertiesTypeDef",
     "RestoreWorkspaceRequestRequestTypeDef",
     "RevokeIpRulesRequestRequestTypeDef",
+    "RootStorageOutputTypeDef",
+    "SamlPropertiesOutputTypeDef",
+    "SelfservicePermissionsOutputTypeDef",
     "StartRequestTypeDef",
     "StopRequestTypeDef",
     "TerminateRequestTypeDef",
     "UpdateConnectClientAddInRequestRequestTypeDef",
     "UpdateResultTypeDef",
     "UpdateWorkspaceBundleRequestRequestTypeDef",
     "UpdateWorkspaceImagePermissionRequestRequestTypeDef",
+    "UserStorageOutputTypeDef",
+    "WorkspaceAccessPropertiesOutputTypeDef",
     "WorkspacePropertiesOutputTypeDef",
     "AssociateConnectionAliasResultTypeDef",
     "CopyWorkspaceImageResultTypeDef",
     "CreateConnectClientAddInResultTypeDef",
     "CreateConnectionAliasResultTypeDef",
     "CreateIpGroupResultTypeDef",
     "CreateUpdatedWorkspaceImageResultTypeDef",
     "DescribeAccountModificationsResultTypeDef",
     "DescribeAccountResultTypeDef",
     "ImportWorkspaceImageResultTypeDef",
     "ListAvailableManagementCidrRangesResultTypeDef",
     "MigrateWorkspaceResultTypeDef",
     "AuthorizeIpRulesRequestRequestTypeDef",
     "UpdateRulesOfIpGroupRequestRequestTypeDef",
-    "WorkspacesIpGroupTypeDef",
-    "DefaultImportClientBrandingAttributesTypeDef",
-    "IosImportClientBrandingAttributesTypeDef",
     "ModifyCertificateBasedAuthPropertiesRequestRequestTypeDef",
     "ClientPropertiesResultTypeDef",
     "ModifyClientPropertiesRequestRequestTypeDef",
     "DescribeConnectClientAddInsResultTypeDef",
     "ConnectionAliasTypeDef",
     "DescribeConnectionAliasPermissionsResultTypeDef",
     "UpdateConnectionAliasPermissionRequestRequestTypeDef",
     "CopyWorkspaceImageRequestRequestTypeDef",
     "CreateConnectionAliasRequestRequestTypeDef",
     "CreateIpGroupRequestRequestTypeDef",
     "CreateTagsRequestRequestTypeDef",
     "CreateUpdatedWorkspaceImageRequestRequestTypeDef",
     "CreateWorkspaceImageRequestRequestTypeDef",
-    "DescribeTagsResultTypeDef",
     "ImportWorkspaceImageRequestRequestTypeDef",
     "RegisterWorkspaceDirectoryRequestRequestTypeDef",
-    "StandbyWorkspaceOutputTypeDef",
     "StandbyWorkspaceTypeDef",
     "CreateWorkspaceBundleRequestRequestTypeDef",
-    "WorkspaceBundleTypeDef",
     "CreateWorkspaceImageResultTypeDef",
     "DescribeAccountModificationsRequestDescribeAccountModificationsPaginateTypeDef",
     "DescribeIpGroupsRequestDescribeIpGroupsPaginateTypeDef",
     "DescribeWorkspaceBundlesRequestDescribeWorkspaceBundlesPaginateTypeDef",
     "DescribeWorkspaceDirectoriesRequestDescribeWorkspaceDirectoriesPaginateTypeDef",
     "DescribeWorkspaceImagesRequestDescribeWorkspaceImagesPaginateTypeDef",
     "DescribeWorkspacesConnectionStatusRequestDescribeWorkspacesConnectionStatusPaginateTypeDef",
     "DescribeWorkspacesRequestDescribeWorkspacesPaginateTypeDef",
     "ListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef",
     "DescribeClientBrandingResultTypeDef",
     "ImportClientBrandingResultTypeDef",
+    "DescribeTagsResultTypeDef",
+    "StandbyWorkspaceOutputTypeDef",
     "DescribeWorkspaceImagePermissionsResultTypeDef",
     "DescribeWorkspaceSnapshotsResultTypeDef",
     "DescribeWorkspacesConnectionStatusResultTypeDef",
     "RebootWorkspacesResultTypeDef",
     "RebuildWorkspacesResultTypeDef",
     "StartWorkspacesResultTypeDef",
     "StopWorkspacesResultTypeDef",
     "TerminateWorkspacesResultTypeDef",
+    "ImportClientBrandingRequestRequestTypeDef",
+    "WorkspacesIpGroupTypeDef",
     "ModifySamlPropertiesRequestRequestTypeDef",
     "ModifySelfservicePermissionsRequestRequestTypeDef",
     "ModifyWorkspaceAccessPropertiesRequestRequestTypeDef",
-    "WorkspaceDirectoryTypeDef",
     "ModifyWorkspaceCreationPropertiesRequestRequestTypeDef",
     "ModifyWorkspacePropertiesRequestRequestTypeDef",
     "WorkspaceRequestTypeDef",
     "RebootWorkspacesRequestRequestTypeDef",
     "RebuildWorkspacesRequestRequestTypeDef",
     "StartWorkspacesRequestRequestTypeDef",
     "StopWorkspacesRequestRequestTypeDef",
     "TerminateWorkspacesRequestRequestTypeDef",
     "WorkspaceImageTypeDef",
-    "WorkspacePropertiesUnionTypeDef",
+    "WorkspaceBundleTypeDef",
+    "WorkspaceDirectoryTypeDef",
     "WorkspaceRequestOutputTypeDef",
     "WorkspaceTypeDef",
-    "DescribeIpGroupsResultTypeDef",
-    "ImportClientBrandingRequestRequestTypeDef",
     "DescribeClientPropertiesResultTypeDef",
     "DescribeConnectionAliasesResultTypeDef",
+    "CreateStandbyWorkspacesRequestRequestTypeDef",
     "FailedCreateStandbyWorkspacesRequestTypeDef",
-    "StandbyWorkspaceUnionTypeDef",
+    "DescribeIpGroupsResultTypeDef",
+    "CreateWorkspacesRequestRequestTypeDef",
+    "DescribeWorkspaceImagesResultTypeDef",
     "CreateWorkspaceBundleResultTypeDef",
     "DescribeWorkspaceBundlesResultTypeDef",
     "DescribeWorkspaceDirectoriesResultTypeDef",
-    "DescribeWorkspaceImagesResultTypeDef",
     "FailedCreateWorkspaceRequestTypeDef",
-    "WorkspaceRequestUnionTypeDef",
     "DescribeWorkspacesResultTypeDef",
     "CreateStandbyWorkspacesResultTypeDef",
-    "CreateStandbyWorkspacesRequestRequestTypeDef",
     "CreateWorkspacesResultTypeDef",
-    "CreateWorkspacesRequestRequestTypeDef",
 )
 
 AccountModificationTypeDef = TypedDict(
     "AccountModificationTypeDef",
     {
         "ModificationState": DedicatedTenancyModificationStateEnumType,
         "DedicatedTenancySupport": DedicatedTenancySupportResultEnumType,
         "DedicatedTenancyManagementCidrRange": str,
         "StartTime": datetime,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
-    total=False,
 )
 
 AssociateConnectionAliasRequestRequestTypeDef = TypedDict(
     "AssociateConnectionAliasRequestRequestTypeDef",
     {
         "AliasId": str,
         "ResourceId": str,
@@ -271,33 +277,55 @@
     {
         "ipRule": str,
         "ruleDesc": str,
     },
     total=False,
 )
 
-BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
+CertificateBasedAuthPropertiesOutputTypeDef = TypedDict(
+    "CertificateBasedAuthPropertiesOutputTypeDef",
+    {
+        "Status": CertificateBasedAuthStatusEnumType,
+        "CertificateAuthorityArn": str,
+    },
+)
+
 CertificateBasedAuthPropertiesTypeDef = TypedDict(
     "CertificateBasedAuthPropertiesTypeDef",
     {
         "Status": CertificateBasedAuthStatusEnumType,
         "CertificateAuthorityArn": str,
     },
     total=False,
 )
 
+ClientPropertiesOutputTypeDef = TypedDict(
+    "ClientPropertiesOutputTypeDef",
+    {
+        "ReconnectEnabled": ReconnectEnumType,
+        "LogUploadEnabled": LogUploadEnumType,
+    },
+)
+
 ClientPropertiesTypeDef = TypedDict(
     "ClientPropertiesTypeDef",
     {
         "ReconnectEnabled": ReconnectEnumType,
         "LogUploadEnabled": LogUploadEnumType,
     },
     total=False,
 )
 
+ComputeTypeOutputTypeDef = TypedDict(
+    "ComputeTypeOutputTypeDef",
+    {
+        "Name": ComputeType,
+    },
+)
+
 ComputeTypeTypeDef = TypedDict(
     "ComputeTypeTypeDef",
     {
         "Name": ComputeType,
     },
     total=False,
 )
@@ -306,26 +334,32 @@
     "ConnectClientAddInTypeDef",
     {
         "AddInId": str,
         "ResourceId": str,
         "Name": str,
         "URL": str,
     },
-    total=False,
 )
 
 ConnectionAliasAssociationTypeDef = TypedDict(
     "ConnectionAliasAssociationTypeDef",
     {
         "AssociationStatus": AssociationStatusType,
         "AssociatedAccountId": str,
         "ResourceId": str,
         "ConnectionIdentifier": str,
     },
-    total=False,
+)
+
+ConnectionAliasPermissionOutputTypeDef = TypedDict(
+    "ConnectionAliasPermissionOutputTypeDef",
+    {
+        "SharedAccountId": str,
+        "AllowAssociation": bool,
+    },
 )
 
 ConnectionAliasPermissionTypeDef = TypedDict(
     "ConnectionAliasPermissionTypeDef",
     {
         "SharedAccountId": str,
         "AllowAssociation": bool,
@@ -364,15 +398,14 @@
     "PendingCreateStandbyWorkspacesRequestTypeDef",
     {
         "UserName": str,
         "DirectoryId": str,
         "State": WorkspaceStateType,
         "WorkspaceId": str,
     },
-    total=False,
 )
 
 RootStorageTypeDef = TypedDict(
     "RootStorageTypeDef",
     {
         "Capacity": str,
     },
@@ -388,40 +421,49 @@
 )
 
 OperatingSystemTypeDef = TypedDict(
     "OperatingSystemTypeDef",
     {
         "Type": OperatingSystemTypeType,
     },
-    total=False,
 )
 
 DefaultClientBrandingAttributesTypeDef = TypedDict(
     "DefaultClientBrandingAttributesTypeDef",
     {
         "LogoUrl": str,
         "SupportEmail": str,
         "SupportLink": str,
         "ForgotPasswordLink": str,
         "LoginMessage": Dict[str, str],
     },
+)
+
+DefaultImportClientBrandingAttributesTypeDef = TypedDict(
+    "DefaultImportClientBrandingAttributesTypeDef",
+    {
+        "Logo": Union[str, bytes, IO[Any], StreamingBody],
+        "SupportEmail": str,
+        "SupportLink": str,
+        "ForgotPasswordLink": str,
+        "LoginMessage": Mapping[str, str],
+    },
     total=False,
 )
 
 DefaultWorkspaceCreationPropertiesTypeDef = TypedDict(
     "DefaultWorkspaceCreationPropertiesTypeDef",
     {
         "EnableWorkDocs": bool,
         "EnableInternetAccess": bool,
         "DefaultOu": str,
         "CustomSecurityGroupId": str,
         "UserEnabledAsLocalAdministrator": bool,
         "EnableMaintenanceMode": bool,
     },
-    total=False,
 )
 
 DeleteClientBrandingRequestRequestTypeDef = TypedDict(
     "DeleteClientBrandingRequestRequestTypeDef",
     {
         "ResourceId": str,
         "Platforms": Sequence[ClientDeviceTypeType],
@@ -512,15 +554,14 @@
         "Logo2xUrl": str,
         "Logo3xUrl": str,
         "SupportEmail": str,
         "SupportLink": str,
         "ForgotPasswordLink": str,
         "LoginMessage": Dict[str, str],
     },
-    total=False,
 )
 
 DescribeClientPropertiesRequestRequestTypeDef = TypedDict(
     "DescribeClientPropertiesRequestRequestTypeDef",
     {
         "ResourceIds": Sequence[str],
     },
@@ -596,14 +637,22 @@
 DescribeTagsRequestRequestTypeDef = TypedDict(
     "DescribeTagsRequestRequestTypeDef",
     {
         "ResourceId": str,
     },
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
 DescribeWorkspaceBundlesRequestRequestTypeDef = TypedDict(
     "DescribeWorkspaceBundlesRequestRequestTypeDef",
     {
         "BundleIds": Sequence[str],
         "Owner": str,
         "NextToken": str,
     },
@@ -644,15 +693,14 @@
 
 
 ImagePermissionTypeDef = TypedDict(
     "ImagePermissionTypeDef",
     {
         "SharedAccountId": str,
     },
-    total=False,
 )
 
 DescribeWorkspaceImagesRequestRequestTypeDef = TypedDict(
     "DescribeWorkspaceImagesRequestRequestTypeDef",
     {
         "ImageIds": Sequence[str],
         "ImageType": ImageTypeType,
@@ -670,15 +718,14 @@
 )
 
 SnapshotTypeDef = TypedDict(
     "SnapshotTypeDef",
     {
         "SnapshotTime": datetime,
     },
-    total=False,
 )
 
 DescribeWorkspacesConnectionStatusRequestRequestTypeDef = TypedDict(
     "DescribeWorkspacesConnectionStatusRequestRequestTypeDef",
     {
         "WorkspaceIds": Sequence[str],
         "NextToken": str,
@@ -690,15 +737,14 @@
     "WorkspaceConnectionStatusTypeDef",
     {
         "WorkspaceId": str,
         "ConnectionState": ConnectionStateType,
         "ConnectionStateCheckTimestamp": datetime,
         "LastKnownUserConnectionTimestamp": datetime,
     },
-    total=False,
 )
 
 DescribeWorkspacesRequestRequestTypeDef = TypedDict(
     "DescribeWorkspacesRequestRequestTypeDef",
     {
         "WorkspaceIds": Sequence[str],
         "DirectoryId": str,
@@ -728,17 +774,38 @@
 FailedWorkspaceChangeRequestTypeDef = TypedDict(
     "FailedWorkspaceChangeRequestTypeDef",
     {
         "WorkspaceId": str,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
+)
+
+IosImportClientBrandingAttributesTypeDef = TypedDict(
+    "IosImportClientBrandingAttributesTypeDef",
+    {
+        "Logo": Union[str, bytes, IO[Any], StreamingBody],
+        "Logo2x": Union[str, bytes, IO[Any], StreamingBody],
+        "Logo3x": Union[str, bytes, IO[Any], StreamingBody],
+        "SupportEmail": str,
+        "SupportLink": str,
+        "ForgotPasswordLink": str,
+        "LoginMessage": Mapping[str, str],
+    },
     total=False,
 )
 
+IpRuleItemOutputTypeDef = TypedDict(
+    "IpRuleItemOutputTypeDef",
+    {
+        "ipRule": str,
+        "ruleDesc": str,
+    },
+)
+
 _RequiredListAvailableManagementCidrRangesRequestRequestTypeDef = TypedDict(
     "_RequiredListAvailableManagementCidrRangesRequestRequestTypeDef",
     {
         "ManagementCidrRangeConstraint": str,
     },
 )
 _OptionalListAvailableManagementCidrRangesRequestRequestTypeDef = TypedDict(
@@ -768,15 +835,14 @@
 
 ModificationStateTypeDef = TypedDict(
     "ModificationStateTypeDef",
     {
         "Resource": ModificationResourceEnumType,
         "State": ModificationStateEnumType,
     },
-    total=False,
 )
 
 ModifyAccountRequestRequestTypeDef = TypedDict(
     "ModifyAccountRequestRequestTypeDef",
     {
         "DedicatedTenancySupport": Literal["ENABLED"],
         "DedicatedTenancyManagementCidrRange": str,
@@ -873,15 +939,14 @@
     "RelatedWorkspacePropertiesTypeDef",
     {
         "WorkspaceId": str,
         "Region": str,
         "State": WorkspaceStateType,
         "Type": StandbyWorkspaceRelationshipTypeType,
     },
-    total=False,
 )
 
 RestoreWorkspaceRequestRequestTypeDef = TypedDict(
     "RestoreWorkspaceRequestRequestTypeDef",
     {
         "WorkspaceId": str,
     },
@@ -891,14 +956,41 @@
     "RevokeIpRulesRequestRequestTypeDef",
     {
         "GroupId": str,
         "UserRules": Sequence[str],
     },
 )
 
+RootStorageOutputTypeDef = TypedDict(
+    "RootStorageOutputTypeDef",
+    {
+        "Capacity": str,
+    },
+)
+
+SamlPropertiesOutputTypeDef = TypedDict(
+    "SamlPropertiesOutputTypeDef",
+    {
+        "Status": SamlStatusEnumType,
+        "UserAccessUrl": str,
+        "RelayStateParameterName": str,
+    },
+)
+
+SelfservicePermissionsOutputTypeDef = TypedDict(
+    "SelfservicePermissionsOutputTypeDef",
+    {
+        "RestartWorkspace": ReconnectEnumType,
+        "IncreaseVolumeSize": ReconnectEnumType,
+        "ChangeComputeType": ReconnectEnumType,
+        "SwitchRunningMode": ReconnectEnumType,
+        "RebuildWorkspace": ReconnectEnumType,
+    },
+)
+
 StartRequestTypeDef = TypedDict(
     "StartRequestTypeDef",
     {
         "WorkspaceId": str,
     },
     total=False,
 )
@@ -944,15 +1036,14 @@
 
 UpdateResultTypeDef = TypedDict(
     "UpdateResultTypeDef",
     {
         "UpdateAvailable": bool,
         "Description": str,
     },
-    total=False,
 )
 
 UpdateWorkspaceBundleRequestRequestTypeDef = TypedDict(
     "UpdateWorkspaceBundleRequestRequestTypeDef",
     {
         "BundleId": str,
         "ImageId": str,
@@ -965,25 +1056,45 @@
     {
         "ImageId": str,
         "AllowCopyImage": bool,
         "SharedAccountId": str,
     },
 )
 
+UserStorageOutputTypeDef = TypedDict(
+    "UserStorageOutputTypeDef",
+    {
+        "Capacity": str,
+    },
+)
+
+WorkspaceAccessPropertiesOutputTypeDef = TypedDict(
+    "WorkspaceAccessPropertiesOutputTypeDef",
+    {
+        "DeviceTypeWindows": AccessPropertyValueType,
+        "DeviceTypeOsx": AccessPropertyValueType,
+        "DeviceTypeWeb": AccessPropertyValueType,
+        "DeviceTypeIos": AccessPropertyValueType,
+        "DeviceTypeAndroid": AccessPropertyValueType,
+        "DeviceTypeChromeOs": AccessPropertyValueType,
+        "DeviceTypeZeroClient": AccessPropertyValueType,
+        "DeviceTypeLinux": AccessPropertyValueType,
+    },
+)
+
 WorkspacePropertiesOutputTypeDef = TypedDict(
     "WorkspacePropertiesOutputTypeDef",
     {
         "RunningMode": RunningModeType,
         "RunningModeAutoStopTimeoutInMinutes": int,
         "RootVolumeSizeGib": int,
         "UserVolumeSizeGib": int,
         "ComputeTypeName": ComputeType,
         "Protocols": List[ProtocolType],
     },
-    total=False,
 )
 
 AssociateConnectionAliasResultTypeDef = TypedDict(
     "AssociateConnectionAliasResultTypeDef",
     {
         "ConnectionIdentifier": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1086,51 +1197,14 @@
     "UpdateRulesOfIpGroupRequestRequestTypeDef",
     {
         "GroupId": str,
         "UserRules": Sequence[IpRuleItemTypeDef],
     },
 )
 
-WorkspacesIpGroupTypeDef = TypedDict(
-    "WorkspacesIpGroupTypeDef",
-    {
-        "groupId": str,
-        "groupName": str,
-        "groupDesc": str,
-        "userRules": List[IpRuleItemTypeDef],
-    },
-    total=False,
-)
-
-DefaultImportClientBrandingAttributesTypeDef = TypedDict(
-    "DefaultImportClientBrandingAttributesTypeDef",
-    {
-        "Logo": BlobTypeDef,
-        "SupportEmail": str,
-        "SupportLink": str,
-        "ForgotPasswordLink": str,
-        "LoginMessage": Mapping[str, str],
-    },
-    total=False,
-)
-
-IosImportClientBrandingAttributesTypeDef = TypedDict(
-    "IosImportClientBrandingAttributesTypeDef",
-    {
-        "Logo": BlobTypeDef,
-        "Logo2x": BlobTypeDef,
-        "Logo3x": BlobTypeDef,
-        "SupportEmail": str,
-        "SupportLink": str,
-        "ForgotPasswordLink": str,
-        "LoginMessage": Mapping[str, str],
-    },
-    total=False,
-)
-
 _RequiredModifyCertificateBasedAuthPropertiesRequestRequestTypeDef = TypedDict(
     "_RequiredModifyCertificateBasedAuthPropertiesRequestRequestTypeDef",
     {
         "ResourceId": str,
     },
 )
 _OptionalModifyCertificateBasedAuthPropertiesRequestRequestTypeDef = TypedDict(
@@ -1152,17 +1226,16 @@
     pass
 
 
 ClientPropertiesResultTypeDef = TypedDict(
     "ClientPropertiesResultTypeDef",
     {
         "ResourceId": str,
-        "ClientProperties": ClientPropertiesTypeDef,
+        "ClientProperties": ClientPropertiesOutputTypeDef,
     },
-    total=False,
 )
 
 ModifyClientPropertiesRequestRequestTypeDef = TypedDict(
     "ModifyClientPropertiesRequestRequestTypeDef",
     {
         "ResourceId": str,
         "ClientProperties": ClientPropertiesTypeDef,
@@ -1183,22 +1256,21 @@
     {
         "ConnectionString": str,
         "AliasId": str,
         "State": ConnectionAliasStateType,
         "OwnerAccountId": str,
         "Associations": List[ConnectionAliasAssociationTypeDef],
     },
-    total=False,
 )
 
 DescribeConnectionAliasPermissionsResultTypeDef = TypedDict(
     "DescribeConnectionAliasPermissionsResultTypeDef",
     {
         "AliasId": str,
-        "ConnectionAliasPermissions": List[ConnectionAliasPermissionTypeDef],
+        "ConnectionAliasPermissions": List[ConnectionAliasPermissionOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateConnectionAliasPermissionRequestRequestTypeDef = TypedDict(
     "UpdateConnectionAliasPermissionRequestRequestTypeDef",
@@ -1330,22 +1402,14 @@
 class CreateWorkspaceImageRequestRequestTypeDef(
     _RequiredCreateWorkspaceImageRequestRequestTypeDef,
     _OptionalCreateWorkspaceImageRequestRequestTypeDef,
 ):
     pass
 
 
-DescribeTagsResultTypeDef = TypedDict(
-    "DescribeTagsResultTypeDef",
-    {
-        "TagList": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredImportWorkspaceImageRequestRequestTypeDef = TypedDict(
     "_RequiredImportWorkspaceImageRequestRequestTypeDef",
     {
         "Ec2ImageId": str,
         "IngestionProcess": WorkspaceImageIngestionProcessType,
         "ImageName": str,
         "ImageDescription": str,
@@ -1390,37 +1454,14 @@
 class RegisterWorkspaceDirectoryRequestRequestTypeDef(
     _RequiredRegisterWorkspaceDirectoryRequestRequestTypeDef,
     _OptionalRegisterWorkspaceDirectoryRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredStandbyWorkspaceOutputTypeDef = TypedDict(
-    "_RequiredStandbyWorkspaceOutputTypeDef",
-    {
-        "PrimaryWorkspaceId": str,
-        "DirectoryId": str,
-    },
-)
-_OptionalStandbyWorkspaceOutputTypeDef = TypedDict(
-    "_OptionalStandbyWorkspaceOutputTypeDef",
-    {
-        "VolumeEncryptionKey": str,
-        "Tags": List[TagTypeDef],
-    },
-    total=False,
-)
-
-
-class StandbyWorkspaceOutputTypeDef(
-    _RequiredStandbyWorkspaceOutputTypeDef, _OptionalStandbyWorkspaceOutputTypeDef
-):
-    pass
-
-
 _RequiredStandbyWorkspaceTypeDef = TypedDict(
     "_RequiredStandbyWorkspaceTypeDef",
     {
         "PrimaryWorkspaceId": str,
         "DirectoryId": str,
     },
 )
@@ -1461,33 +1502,14 @@
 class CreateWorkspaceBundleRequestRequestTypeDef(
     _RequiredCreateWorkspaceBundleRequestRequestTypeDef,
     _OptionalCreateWorkspaceBundleRequestRequestTypeDef,
 ):
     pass
 
 
-WorkspaceBundleTypeDef = TypedDict(
-    "WorkspaceBundleTypeDef",
-    {
-        "BundleId": str,
-        "Name": str,
-        "Owner": str,
-        "Description": str,
-        "ImageId": str,
-        "RootStorage": RootStorageTypeDef,
-        "UserStorage": UserStorageTypeDef,
-        "ComputeType": ComputeTypeTypeDef,
-        "LastUpdatedTime": datetime,
-        "CreationTime": datetime,
-        "State": WorkspaceBundleStateType,
-        "BundleType": BundleTypeType,
-    },
-    total=False,
-)
-
 CreateWorkspaceImageResultTypeDef = TypedDict(
     "CreateWorkspaceImageResultTypeDef",
     {
         "ImageId": str,
         "Name": str,
         "Description": str,
         "OperatingSystem": OperatingSystemTypeDef,
@@ -1611,14 +1633,32 @@
         "DeviceTypeIos": IosClientBrandingAttributesTypeDef,
         "DeviceTypeLinux": DefaultClientBrandingAttributesTypeDef,
         "DeviceTypeWeb": DefaultClientBrandingAttributesTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeTagsResultTypeDef = TypedDict(
+    "DescribeTagsResultTypeDef",
+    {
+        "TagList": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StandbyWorkspaceOutputTypeDef = TypedDict(
+    "StandbyWorkspaceOutputTypeDef",
+    {
+        "PrimaryWorkspaceId": str,
+        "VolumeEncryptionKey": str,
+        "DirectoryId": str,
+        "Tags": List[TagOutputTypeDef],
+    },
+)
+
 DescribeWorkspaceImagePermissionsResultTypeDef = TypedDict(
     "DescribeWorkspaceImagePermissionsResultTypeDef",
     {
         "ImageId": str,
         "ImagePermissions": List[ImagePermissionTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1679,14 +1719,51 @@
     "TerminateWorkspacesResultTypeDef",
     {
         "FailedRequests": List[FailedWorkspaceChangeRequestTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredImportClientBrandingRequestRequestTypeDef = TypedDict(
+    "_RequiredImportClientBrandingRequestRequestTypeDef",
+    {
+        "ResourceId": str,
+    },
+)
+_OptionalImportClientBrandingRequestRequestTypeDef = TypedDict(
+    "_OptionalImportClientBrandingRequestRequestTypeDef",
+    {
+        "DeviceTypeWindows": DefaultImportClientBrandingAttributesTypeDef,
+        "DeviceTypeOsx": DefaultImportClientBrandingAttributesTypeDef,
+        "DeviceTypeAndroid": DefaultImportClientBrandingAttributesTypeDef,
+        "DeviceTypeIos": IosImportClientBrandingAttributesTypeDef,
+        "DeviceTypeLinux": DefaultImportClientBrandingAttributesTypeDef,
+        "DeviceTypeWeb": DefaultImportClientBrandingAttributesTypeDef,
+    },
+    total=False,
+)
+
+
+class ImportClientBrandingRequestRequestTypeDef(
+    _RequiredImportClientBrandingRequestRequestTypeDef,
+    _OptionalImportClientBrandingRequestRequestTypeDef,
+):
+    pass
+
+
+WorkspacesIpGroupTypeDef = TypedDict(
+    "WorkspacesIpGroupTypeDef",
+    {
+        "groupId": str,
+        "groupName": str,
+        "groupDesc": str,
+        "userRules": List[IpRuleItemOutputTypeDef],
+    },
+)
+
 _RequiredModifySamlPropertiesRequestRequestTypeDef = TypedDict(
     "_RequiredModifySamlPropertiesRequestRequestTypeDef",
     {
         "ResourceId": str,
     },
 )
 _OptionalModifySamlPropertiesRequestRequestTypeDef = TypedDict(
@@ -1718,39 +1795,14 @@
     "ModifyWorkspaceAccessPropertiesRequestRequestTypeDef",
     {
         "ResourceId": str,
         "WorkspaceAccessProperties": WorkspaceAccessPropertiesTypeDef,
     },
 )
 
-WorkspaceDirectoryTypeDef = TypedDict(
-    "WorkspaceDirectoryTypeDef",
-    {
-        "DirectoryId": str,
-        "Alias": str,
-        "DirectoryName": str,
-        "RegistrationCode": str,
-        "SubnetIds": List[str],
-        "DnsIpAddresses": List[str],
-        "CustomerUserName": str,
-        "IamRoleId": str,
-        "DirectoryType": WorkspaceDirectoryTypeType,
-        "WorkspaceSecurityGroupId": str,
-        "State": WorkspaceDirectoryStateType,
-        "WorkspaceCreationProperties": DefaultWorkspaceCreationPropertiesTypeDef,
-        "ipGroupIds": List[str],
-        "WorkspaceAccessProperties": WorkspaceAccessPropertiesTypeDef,
-        "Tenancy": TenancyType,
-        "SelfservicePermissions": SelfservicePermissionsTypeDef,
-        "SamlProperties": SamlPropertiesTypeDef,
-        "CertificateBasedAuthProperties": CertificateBasedAuthPropertiesTypeDef,
-    },
-    total=False,
-)
-
 ModifyWorkspaceCreationPropertiesRequestRequestTypeDef = TypedDict(
     "ModifyWorkspaceCreationPropertiesRequestRequestTypeDef",
     {
         "ResourceId": str,
         "WorkspaceCreationProperties": WorkspaceCreationPropertiesTypeDef,
     },
 )
@@ -1834,47 +1886,72 @@
         "RequiredTenancy": WorkspaceImageRequiredTenancyType,
         "ErrorCode": str,
         "ErrorMessage": str,
         "Created": datetime,
         "OwnerAccountId": str,
         "Updates": UpdateResultTypeDef,
     },
-    total=False,
 )
 
-WorkspacePropertiesUnionTypeDef = Union[
-    WorkspacePropertiesTypeDef, WorkspacePropertiesOutputTypeDef
-]
-_RequiredWorkspaceRequestOutputTypeDef = TypedDict(
-    "_RequiredWorkspaceRequestOutputTypeDef",
+WorkspaceBundleTypeDef = TypedDict(
+    "WorkspaceBundleTypeDef",
     {
-        "DirectoryId": str,
-        "UserName": str,
         "BundleId": str,
+        "Name": str,
+        "Owner": str,
+        "Description": str,
+        "ImageId": str,
+        "RootStorage": RootStorageOutputTypeDef,
+        "UserStorage": UserStorageOutputTypeDef,
+        "ComputeType": ComputeTypeOutputTypeDef,
+        "LastUpdatedTime": datetime,
+        "CreationTime": datetime,
+        "State": WorkspaceBundleStateType,
+        "BundleType": BundleTypeType,
+    },
+)
+
+WorkspaceDirectoryTypeDef = TypedDict(
+    "WorkspaceDirectoryTypeDef",
+    {
+        "DirectoryId": str,
+        "Alias": str,
+        "DirectoryName": str,
+        "RegistrationCode": str,
+        "SubnetIds": List[str],
+        "DnsIpAddresses": List[str],
+        "CustomerUserName": str,
+        "IamRoleId": str,
+        "DirectoryType": WorkspaceDirectoryTypeType,
+        "WorkspaceSecurityGroupId": str,
+        "State": WorkspaceDirectoryStateType,
+        "WorkspaceCreationProperties": DefaultWorkspaceCreationPropertiesTypeDef,
+        "ipGroupIds": List[str],
+        "WorkspaceAccessProperties": WorkspaceAccessPropertiesOutputTypeDef,
+        "Tenancy": TenancyType,
+        "SelfservicePermissions": SelfservicePermissionsOutputTypeDef,
+        "SamlProperties": SamlPropertiesOutputTypeDef,
+        "CertificateBasedAuthProperties": CertificateBasedAuthPropertiesOutputTypeDef,
     },
 )
-_OptionalWorkspaceRequestOutputTypeDef = TypedDict(
-    "_OptionalWorkspaceRequestOutputTypeDef",
+
+WorkspaceRequestOutputTypeDef = TypedDict(
+    "WorkspaceRequestOutputTypeDef",
     {
+        "DirectoryId": str,
+        "UserName": str,
+        "BundleId": str,
         "VolumeEncryptionKey": str,
         "UserVolumeEncryptionEnabled": bool,
         "RootVolumeEncryptionEnabled": bool,
         "WorkspaceProperties": WorkspacePropertiesOutputTypeDef,
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
     },
-    total=False,
 )
 
-
-class WorkspaceRequestOutputTypeDef(
-    _RequiredWorkspaceRequestOutputTypeDef, _OptionalWorkspaceRequestOutputTypeDef
-):
-    pass
-
-
 WorkspaceTypeDef = TypedDict(
     "WorkspaceTypeDef",
     {
         "WorkspaceId": str,
         "DirectoryId": str,
         "UserName": str,
         "IpAddress": str,
@@ -1887,53 +1964,16 @@
         "VolumeEncryptionKey": str,
         "UserVolumeEncryptionEnabled": bool,
         "RootVolumeEncryptionEnabled": bool,
         "WorkspaceProperties": WorkspacePropertiesOutputTypeDef,
         "ModificationStates": List[ModificationStateTypeDef],
         "RelatedWorkspaces": List[RelatedWorkspacePropertiesTypeDef],
     },
-    total=False,
 )
 
-DescribeIpGroupsResultTypeDef = TypedDict(
-    "DescribeIpGroupsResultTypeDef",
-    {
-        "Result": List[WorkspacesIpGroupTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredImportClientBrandingRequestRequestTypeDef = TypedDict(
-    "_RequiredImportClientBrandingRequestRequestTypeDef",
-    {
-        "ResourceId": str,
-    },
-)
-_OptionalImportClientBrandingRequestRequestTypeDef = TypedDict(
-    "_OptionalImportClientBrandingRequestRequestTypeDef",
-    {
-        "DeviceTypeWindows": DefaultImportClientBrandingAttributesTypeDef,
-        "DeviceTypeOsx": DefaultImportClientBrandingAttributesTypeDef,
-        "DeviceTypeAndroid": DefaultImportClientBrandingAttributesTypeDef,
-        "DeviceTypeIos": IosImportClientBrandingAttributesTypeDef,
-        "DeviceTypeLinux": DefaultImportClientBrandingAttributesTypeDef,
-        "DeviceTypeWeb": DefaultImportClientBrandingAttributesTypeDef,
-    },
-    total=False,
-)
-
-
-class ImportClientBrandingRequestRequestTypeDef(
-    _RequiredImportClientBrandingRequestRequestTypeDef,
-    _OptionalImportClientBrandingRequestRequestTypeDef,
-):
-    pass
-
-
 DescribeClientPropertiesResultTypeDef = TypedDict(
     "DescribeClientPropertiesResultTypeDef",
     {
         "ClientPropertiesList": List[ClientPropertiesResultTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1943,25 +1983,56 @@
     {
         "ConnectionAliases": List[ConnectionAliasTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CreateStandbyWorkspacesRequestRequestTypeDef = TypedDict(
+    "CreateStandbyWorkspacesRequestRequestTypeDef",
+    {
+        "PrimaryRegion": str,
+        "StandbyWorkspaces": Sequence[StandbyWorkspaceTypeDef],
+    },
+)
+
 FailedCreateStandbyWorkspacesRequestTypeDef = TypedDict(
     "FailedCreateStandbyWorkspacesRequestTypeDef",
     {
         "StandbyWorkspaceRequest": StandbyWorkspaceOutputTypeDef,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
-    total=False,
 )
 
-StandbyWorkspaceUnionTypeDef = Union[StandbyWorkspaceTypeDef, StandbyWorkspaceOutputTypeDef]
+DescribeIpGroupsResultTypeDef = TypedDict(
+    "DescribeIpGroupsResultTypeDef",
+    {
+        "Result": List[WorkspacesIpGroupTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateWorkspacesRequestRequestTypeDef = TypedDict(
+    "CreateWorkspacesRequestRequestTypeDef",
+    {
+        "Workspaces": Sequence[WorkspaceRequestTypeDef],
+    },
+)
+
+DescribeWorkspaceImagesResultTypeDef = TypedDict(
+    "DescribeWorkspaceImagesResultTypeDef",
+    {
+        "Images": List[WorkspaceImageTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateWorkspaceBundleResultTypeDef = TypedDict(
     "CreateWorkspaceBundleResultTypeDef",
     {
         "WorkspaceBundle": WorkspaceBundleTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1980,34 +2051,23 @@
     {
         "Directories": List[WorkspaceDirectoryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeWorkspaceImagesResultTypeDef = TypedDict(
-    "DescribeWorkspaceImagesResultTypeDef",
-    {
-        "Images": List[WorkspaceImageTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 FailedCreateWorkspaceRequestTypeDef = TypedDict(
     "FailedCreateWorkspaceRequestTypeDef",
     {
         "WorkspaceRequest": WorkspaceRequestOutputTypeDef,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
-    total=False,
 )
 
-WorkspaceRequestUnionTypeDef = Union[WorkspaceRequestTypeDef, WorkspaceRequestOutputTypeDef]
 DescribeWorkspacesResultTypeDef = TypedDict(
     "DescribeWorkspacesResultTypeDef",
     {
         "Workspaces": List[WorkspaceTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2018,30 +2078,15 @@
     {
         "FailedStandbyRequests": List[FailedCreateStandbyWorkspacesRequestTypeDef],
         "PendingStandbyRequests": List[PendingCreateStandbyWorkspacesRequestTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateStandbyWorkspacesRequestRequestTypeDef = TypedDict(
-    "CreateStandbyWorkspacesRequestRequestTypeDef",
-    {
-        "PrimaryRegion": str,
-        "StandbyWorkspaces": Sequence[StandbyWorkspaceUnionTypeDef],
-    },
-)
-
 CreateWorkspacesResultTypeDef = TypedDict(
     "CreateWorkspacesResultTypeDef",
     {
         "FailedRequests": List[FailedCreateWorkspaceRequestTypeDef],
         "PendingRequests": List[WorkspaceTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-
-CreateWorkspacesRequestRequestTypeDef = TypedDict(
-    "CreateWorkspacesRequestRequestTypeDef",
-    {
-        "Workspaces": Sequence[WorkspaceRequestUnionTypeDef],
-    },
-)
```

### Comparing `mypy-boto3-workspaces-1.28.16/mypy_boto3_workspaces/type_defs.pyi` & `mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_workspaces.type_defs import AccountModificationTypeDef
 
-    data: AccountModificationTypeDef = ...
+    data: AccountModificationTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -62,28 +62,32 @@
 
 __all__ = (
     "AccountModificationTypeDef",
     "AssociateConnectionAliasRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AssociateIpGroupsRequestRequestTypeDef",
     "IpRuleItemTypeDef",
-    "BlobTypeDef",
+    "CertificateBasedAuthPropertiesOutputTypeDef",
     "CertificateBasedAuthPropertiesTypeDef",
+    "ClientPropertiesOutputTypeDef",
     "ClientPropertiesTypeDef",
+    "ComputeTypeOutputTypeDef",
     "ComputeTypeTypeDef",
     "ConnectClientAddInTypeDef",
     "ConnectionAliasAssociationTypeDef",
+    "ConnectionAliasPermissionOutputTypeDef",
     "ConnectionAliasPermissionTypeDef",
     "TagTypeDef",
     "CreateConnectClientAddInRequestRequestTypeDef",
     "PendingCreateStandbyWorkspacesRequestTypeDef",
     "RootStorageTypeDef",
     "UserStorageTypeDef",
     "OperatingSystemTypeDef",
     "DefaultClientBrandingAttributesTypeDef",
+    "DefaultImportClientBrandingAttributesTypeDef",
     "DefaultWorkspaceCreationPropertiesTypeDef",
     "DeleteClientBrandingRequestRequestTypeDef",
     "DeleteConnectClientAddInRequestRequestTypeDef",
     "DeleteConnectionAliasRequestRequestTypeDef",
     "DeleteIpGroupRequestRequestTypeDef",
     "DeleteTagsRequestRequestTypeDef",
     "DeleteWorkspaceBundleRequestRequestTypeDef",
@@ -95,27 +99,30 @@
     "IosClientBrandingAttributesTypeDef",
     "DescribeClientPropertiesRequestRequestTypeDef",
     "DescribeConnectClientAddInsRequestRequestTypeDef",
     "DescribeConnectionAliasPermissionsRequestRequestTypeDef",
     "DescribeConnectionAliasesRequestRequestTypeDef",
     "DescribeIpGroupsRequestRequestTypeDef",
     "DescribeTagsRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "DescribeWorkspaceBundlesRequestRequestTypeDef",
     "DescribeWorkspaceDirectoriesRequestRequestTypeDef",
     "DescribeWorkspaceImagePermissionsRequestRequestTypeDef",
     "ImagePermissionTypeDef",
     "DescribeWorkspaceImagesRequestRequestTypeDef",
     "DescribeWorkspaceSnapshotsRequestRequestTypeDef",
     "SnapshotTypeDef",
     "DescribeWorkspacesConnectionStatusRequestRequestTypeDef",
     "WorkspaceConnectionStatusTypeDef",
     "DescribeWorkspacesRequestRequestTypeDef",
     "DisassociateConnectionAliasRequestRequestTypeDef",
     "DisassociateIpGroupsRequestRequestTypeDef",
     "FailedWorkspaceChangeRequestTypeDef",
+    "IosImportClientBrandingAttributesTypeDef",
+    "IpRuleItemOutputTypeDef",
     "ListAvailableManagementCidrRangesRequestRequestTypeDef",
     "MigrateWorkspaceRequestRequestTypeDef",
     "ModificationStateTypeDef",
     "ModifyAccountRequestRequestTypeDef",
     "SamlPropertiesTypeDef",
     "SelfservicePermissionsTypeDef",
     "WorkspaceAccessPropertiesTypeDef",
@@ -123,123 +130,122 @@
     "WorkspacePropertiesTypeDef",
     "ModifyWorkspaceStateRequestRequestTypeDef",
     "RebootRequestTypeDef",
     "RebuildRequestTypeDef",
     "RelatedWorkspacePropertiesTypeDef",
     "RestoreWorkspaceRequestRequestTypeDef",
     "RevokeIpRulesRequestRequestTypeDef",
+    "RootStorageOutputTypeDef",
+    "SamlPropertiesOutputTypeDef",
+    "SelfservicePermissionsOutputTypeDef",
     "StartRequestTypeDef",
     "StopRequestTypeDef",
     "TerminateRequestTypeDef",
     "UpdateConnectClientAddInRequestRequestTypeDef",
     "UpdateResultTypeDef",
     "UpdateWorkspaceBundleRequestRequestTypeDef",
     "UpdateWorkspaceImagePermissionRequestRequestTypeDef",
+    "UserStorageOutputTypeDef",
+    "WorkspaceAccessPropertiesOutputTypeDef",
     "WorkspacePropertiesOutputTypeDef",
     "AssociateConnectionAliasResultTypeDef",
     "CopyWorkspaceImageResultTypeDef",
     "CreateConnectClientAddInResultTypeDef",
     "CreateConnectionAliasResultTypeDef",
     "CreateIpGroupResultTypeDef",
     "CreateUpdatedWorkspaceImageResultTypeDef",
     "DescribeAccountModificationsResultTypeDef",
     "DescribeAccountResultTypeDef",
     "ImportWorkspaceImageResultTypeDef",
     "ListAvailableManagementCidrRangesResultTypeDef",
     "MigrateWorkspaceResultTypeDef",
     "AuthorizeIpRulesRequestRequestTypeDef",
     "UpdateRulesOfIpGroupRequestRequestTypeDef",
-    "WorkspacesIpGroupTypeDef",
-    "DefaultImportClientBrandingAttributesTypeDef",
-    "IosImportClientBrandingAttributesTypeDef",
     "ModifyCertificateBasedAuthPropertiesRequestRequestTypeDef",
     "ClientPropertiesResultTypeDef",
     "ModifyClientPropertiesRequestRequestTypeDef",
     "DescribeConnectClientAddInsResultTypeDef",
     "ConnectionAliasTypeDef",
     "DescribeConnectionAliasPermissionsResultTypeDef",
     "UpdateConnectionAliasPermissionRequestRequestTypeDef",
     "CopyWorkspaceImageRequestRequestTypeDef",
     "CreateConnectionAliasRequestRequestTypeDef",
     "CreateIpGroupRequestRequestTypeDef",
     "CreateTagsRequestRequestTypeDef",
     "CreateUpdatedWorkspaceImageRequestRequestTypeDef",
     "CreateWorkspaceImageRequestRequestTypeDef",
-    "DescribeTagsResultTypeDef",
     "ImportWorkspaceImageRequestRequestTypeDef",
     "RegisterWorkspaceDirectoryRequestRequestTypeDef",
-    "StandbyWorkspaceOutputTypeDef",
     "StandbyWorkspaceTypeDef",
     "CreateWorkspaceBundleRequestRequestTypeDef",
-    "WorkspaceBundleTypeDef",
     "CreateWorkspaceImageResultTypeDef",
     "DescribeAccountModificationsRequestDescribeAccountModificationsPaginateTypeDef",
     "DescribeIpGroupsRequestDescribeIpGroupsPaginateTypeDef",
     "DescribeWorkspaceBundlesRequestDescribeWorkspaceBundlesPaginateTypeDef",
     "DescribeWorkspaceDirectoriesRequestDescribeWorkspaceDirectoriesPaginateTypeDef",
     "DescribeWorkspaceImagesRequestDescribeWorkspaceImagesPaginateTypeDef",
     "DescribeWorkspacesConnectionStatusRequestDescribeWorkspacesConnectionStatusPaginateTypeDef",
     "DescribeWorkspacesRequestDescribeWorkspacesPaginateTypeDef",
     "ListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef",
     "DescribeClientBrandingResultTypeDef",
     "ImportClientBrandingResultTypeDef",
+    "DescribeTagsResultTypeDef",
+    "StandbyWorkspaceOutputTypeDef",
     "DescribeWorkspaceImagePermissionsResultTypeDef",
     "DescribeWorkspaceSnapshotsResultTypeDef",
     "DescribeWorkspacesConnectionStatusResultTypeDef",
     "RebootWorkspacesResultTypeDef",
     "RebuildWorkspacesResultTypeDef",
     "StartWorkspacesResultTypeDef",
     "StopWorkspacesResultTypeDef",
     "TerminateWorkspacesResultTypeDef",
+    "ImportClientBrandingRequestRequestTypeDef",
+    "WorkspacesIpGroupTypeDef",
     "ModifySamlPropertiesRequestRequestTypeDef",
     "ModifySelfservicePermissionsRequestRequestTypeDef",
     "ModifyWorkspaceAccessPropertiesRequestRequestTypeDef",
-    "WorkspaceDirectoryTypeDef",
     "ModifyWorkspaceCreationPropertiesRequestRequestTypeDef",
     "ModifyWorkspacePropertiesRequestRequestTypeDef",
     "WorkspaceRequestTypeDef",
     "RebootWorkspacesRequestRequestTypeDef",
     "RebuildWorkspacesRequestRequestTypeDef",
     "StartWorkspacesRequestRequestTypeDef",
     "StopWorkspacesRequestRequestTypeDef",
     "TerminateWorkspacesRequestRequestTypeDef",
     "WorkspaceImageTypeDef",
-    "WorkspacePropertiesUnionTypeDef",
+    "WorkspaceBundleTypeDef",
+    "WorkspaceDirectoryTypeDef",
     "WorkspaceRequestOutputTypeDef",
     "WorkspaceTypeDef",
-    "DescribeIpGroupsResultTypeDef",
-    "ImportClientBrandingRequestRequestTypeDef",
     "DescribeClientPropertiesResultTypeDef",
     "DescribeConnectionAliasesResultTypeDef",
+    "CreateStandbyWorkspacesRequestRequestTypeDef",
     "FailedCreateStandbyWorkspacesRequestTypeDef",
-    "StandbyWorkspaceUnionTypeDef",
+    "DescribeIpGroupsResultTypeDef",
+    "CreateWorkspacesRequestRequestTypeDef",
+    "DescribeWorkspaceImagesResultTypeDef",
     "CreateWorkspaceBundleResultTypeDef",
     "DescribeWorkspaceBundlesResultTypeDef",
     "DescribeWorkspaceDirectoriesResultTypeDef",
-    "DescribeWorkspaceImagesResultTypeDef",
     "FailedCreateWorkspaceRequestTypeDef",
-    "WorkspaceRequestUnionTypeDef",
     "DescribeWorkspacesResultTypeDef",
     "CreateStandbyWorkspacesResultTypeDef",
-    "CreateStandbyWorkspacesRequestRequestTypeDef",
     "CreateWorkspacesResultTypeDef",
-    "CreateWorkspacesRequestRequestTypeDef",
 )
 
 AccountModificationTypeDef = TypedDict(
     "AccountModificationTypeDef",
     {
         "ModificationState": DedicatedTenancyModificationStateEnumType,
         "DedicatedTenancySupport": DedicatedTenancySupportResultEnumType,
         "DedicatedTenancyManagementCidrRange": str,
         "StartTime": datetime,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
-    total=False,
 )
 
 AssociateConnectionAliasRequestRequestTypeDef = TypedDict(
     "AssociateConnectionAliasRequestRequestTypeDef",
     {
         "AliasId": str,
         "ResourceId": str,
@@ -270,33 +276,55 @@
     {
         "ipRule": str,
         "ruleDesc": str,
     },
     total=False,
 )
 
-BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
+CertificateBasedAuthPropertiesOutputTypeDef = TypedDict(
+    "CertificateBasedAuthPropertiesOutputTypeDef",
+    {
+        "Status": CertificateBasedAuthStatusEnumType,
+        "CertificateAuthorityArn": str,
+    },
+)
+
 CertificateBasedAuthPropertiesTypeDef = TypedDict(
     "CertificateBasedAuthPropertiesTypeDef",
     {
         "Status": CertificateBasedAuthStatusEnumType,
         "CertificateAuthorityArn": str,
     },
     total=False,
 )
 
+ClientPropertiesOutputTypeDef = TypedDict(
+    "ClientPropertiesOutputTypeDef",
+    {
+        "ReconnectEnabled": ReconnectEnumType,
+        "LogUploadEnabled": LogUploadEnumType,
+    },
+)
+
 ClientPropertiesTypeDef = TypedDict(
     "ClientPropertiesTypeDef",
     {
         "ReconnectEnabled": ReconnectEnumType,
         "LogUploadEnabled": LogUploadEnumType,
     },
     total=False,
 )
 
+ComputeTypeOutputTypeDef = TypedDict(
+    "ComputeTypeOutputTypeDef",
+    {
+        "Name": ComputeType,
+    },
+)
+
 ComputeTypeTypeDef = TypedDict(
     "ComputeTypeTypeDef",
     {
         "Name": ComputeType,
     },
     total=False,
 )
@@ -305,26 +333,32 @@
     "ConnectClientAddInTypeDef",
     {
         "AddInId": str,
         "ResourceId": str,
         "Name": str,
         "URL": str,
     },
-    total=False,
 )
 
 ConnectionAliasAssociationTypeDef = TypedDict(
     "ConnectionAliasAssociationTypeDef",
     {
         "AssociationStatus": AssociationStatusType,
         "AssociatedAccountId": str,
         "ResourceId": str,
         "ConnectionIdentifier": str,
     },
-    total=False,
+)
+
+ConnectionAliasPermissionOutputTypeDef = TypedDict(
+    "ConnectionAliasPermissionOutputTypeDef",
+    {
+        "SharedAccountId": str,
+        "AllowAssociation": bool,
+    },
 )
 
 ConnectionAliasPermissionTypeDef = TypedDict(
     "ConnectionAliasPermissionTypeDef",
     {
         "SharedAccountId": str,
         "AllowAssociation": bool,
@@ -361,15 +395,14 @@
     "PendingCreateStandbyWorkspacesRequestTypeDef",
     {
         "UserName": str,
         "DirectoryId": str,
         "State": WorkspaceStateType,
         "WorkspaceId": str,
     },
-    total=False,
 )
 
 RootStorageTypeDef = TypedDict(
     "RootStorageTypeDef",
     {
         "Capacity": str,
     },
@@ -385,40 +418,49 @@
 )
 
 OperatingSystemTypeDef = TypedDict(
     "OperatingSystemTypeDef",
     {
         "Type": OperatingSystemTypeType,
     },
-    total=False,
 )
 
 DefaultClientBrandingAttributesTypeDef = TypedDict(
     "DefaultClientBrandingAttributesTypeDef",
     {
         "LogoUrl": str,
         "SupportEmail": str,
         "SupportLink": str,
         "ForgotPasswordLink": str,
         "LoginMessage": Dict[str, str],
     },
+)
+
+DefaultImportClientBrandingAttributesTypeDef = TypedDict(
+    "DefaultImportClientBrandingAttributesTypeDef",
+    {
+        "Logo": Union[str, bytes, IO[Any], StreamingBody],
+        "SupportEmail": str,
+        "SupportLink": str,
+        "ForgotPasswordLink": str,
+        "LoginMessage": Mapping[str, str],
+    },
     total=False,
 )
 
 DefaultWorkspaceCreationPropertiesTypeDef = TypedDict(
     "DefaultWorkspaceCreationPropertiesTypeDef",
     {
         "EnableWorkDocs": bool,
         "EnableInternetAccess": bool,
         "DefaultOu": str,
         "CustomSecurityGroupId": str,
         "UserEnabledAsLocalAdministrator": bool,
         "EnableMaintenanceMode": bool,
     },
-    total=False,
 )
 
 DeleteClientBrandingRequestRequestTypeDef = TypedDict(
     "DeleteClientBrandingRequestRequestTypeDef",
     {
         "ResourceId": str,
         "Platforms": Sequence[ClientDeviceTypeType],
@@ -509,15 +551,14 @@
         "Logo2xUrl": str,
         "Logo3xUrl": str,
         "SupportEmail": str,
         "SupportLink": str,
         "ForgotPasswordLink": str,
         "LoginMessage": Dict[str, str],
     },
-    total=False,
 )
 
 DescribeClientPropertiesRequestRequestTypeDef = TypedDict(
     "DescribeClientPropertiesRequestRequestTypeDef",
     {
         "ResourceIds": Sequence[str],
     },
@@ -589,14 +630,22 @@
 DescribeTagsRequestRequestTypeDef = TypedDict(
     "DescribeTagsRequestRequestTypeDef",
     {
         "ResourceId": str,
     },
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
 DescribeWorkspaceBundlesRequestRequestTypeDef = TypedDict(
     "DescribeWorkspaceBundlesRequestRequestTypeDef",
     {
         "BundleIds": Sequence[str],
         "Owner": str,
         "NextToken": str,
     },
@@ -635,15 +684,14 @@
     pass
 
 ImagePermissionTypeDef = TypedDict(
     "ImagePermissionTypeDef",
     {
         "SharedAccountId": str,
     },
-    total=False,
 )
 
 DescribeWorkspaceImagesRequestRequestTypeDef = TypedDict(
     "DescribeWorkspaceImagesRequestRequestTypeDef",
     {
         "ImageIds": Sequence[str],
         "ImageType": ImageTypeType,
@@ -661,15 +709,14 @@
 )
 
 SnapshotTypeDef = TypedDict(
     "SnapshotTypeDef",
     {
         "SnapshotTime": datetime,
     },
-    total=False,
 )
 
 DescribeWorkspacesConnectionStatusRequestRequestTypeDef = TypedDict(
     "DescribeWorkspacesConnectionStatusRequestRequestTypeDef",
     {
         "WorkspaceIds": Sequence[str],
         "NextToken": str,
@@ -681,15 +728,14 @@
     "WorkspaceConnectionStatusTypeDef",
     {
         "WorkspaceId": str,
         "ConnectionState": ConnectionStateType,
         "ConnectionStateCheckTimestamp": datetime,
         "LastKnownUserConnectionTimestamp": datetime,
     },
-    total=False,
 )
 
 DescribeWorkspacesRequestRequestTypeDef = TypedDict(
     "DescribeWorkspacesRequestRequestTypeDef",
     {
         "WorkspaceIds": Sequence[str],
         "DirectoryId": str,
@@ -719,17 +765,38 @@
 FailedWorkspaceChangeRequestTypeDef = TypedDict(
     "FailedWorkspaceChangeRequestTypeDef",
     {
         "WorkspaceId": str,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
+)
+
+IosImportClientBrandingAttributesTypeDef = TypedDict(
+    "IosImportClientBrandingAttributesTypeDef",
+    {
+        "Logo": Union[str, bytes, IO[Any], StreamingBody],
+        "Logo2x": Union[str, bytes, IO[Any], StreamingBody],
+        "Logo3x": Union[str, bytes, IO[Any], StreamingBody],
+        "SupportEmail": str,
+        "SupportLink": str,
+        "ForgotPasswordLink": str,
+        "LoginMessage": Mapping[str, str],
+    },
     total=False,
 )
 
+IpRuleItemOutputTypeDef = TypedDict(
+    "IpRuleItemOutputTypeDef",
+    {
+        "ipRule": str,
+        "ruleDesc": str,
+    },
+)
+
 _RequiredListAvailableManagementCidrRangesRequestRequestTypeDef = TypedDict(
     "_RequiredListAvailableManagementCidrRangesRequestRequestTypeDef",
     {
         "ManagementCidrRangeConstraint": str,
     },
 )
 _OptionalListAvailableManagementCidrRangesRequestRequestTypeDef = TypedDict(
@@ -757,15 +824,14 @@
 
 ModificationStateTypeDef = TypedDict(
     "ModificationStateTypeDef",
     {
         "Resource": ModificationResourceEnumType,
         "State": ModificationStateEnumType,
     },
-    total=False,
 )
 
 ModifyAccountRequestRequestTypeDef = TypedDict(
     "ModifyAccountRequestRequestTypeDef",
     {
         "DedicatedTenancySupport": Literal["ENABLED"],
         "DedicatedTenancyManagementCidrRange": str,
@@ -862,15 +928,14 @@
     "RelatedWorkspacePropertiesTypeDef",
     {
         "WorkspaceId": str,
         "Region": str,
         "State": WorkspaceStateType,
         "Type": StandbyWorkspaceRelationshipTypeType,
     },
-    total=False,
 )
 
 RestoreWorkspaceRequestRequestTypeDef = TypedDict(
     "RestoreWorkspaceRequestRequestTypeDef",
     {
         "WorkspaceId": str,
     },
@@ -880,14 +945,41 @@
     "RevokeIpRulesRequestRequestTypeDef",
     {
         "GroupId": str,
         "UserRules": Sequence[str],
     },
 )
 
+RootStorageOutputTypeDef = TypedDict(
+    "RootStorageOutputTypeDef",
+    {
+        "Capacity": str,
+    },
+)
+
+SamlPropertiesOutputTypeDef = TypedDict(
+    "SamlPropertiesOutputTypeDef",
+    {
+        "Status": SamlStatusEnumType,
+        "UserAccessUrl": str,
+        "RelayStateParameterName": str,
+    },
+)
+
+SelfservicePermissionsOutputTypeDef = TypedDict(
+    "SelfservicePermissionsOutputTypeDef",
+    {
+        "RestartWorkspace": ReconnectEnumType,
+        "IncreaseVolumeSize": ReconnectEnumType,
+        "ChangeComputeType": ReconnectEnumType,
+        "SwitchRunningMode": ReconnectEnumType,
+        "RebuildWorkspace": ReconnectEnumType,
+    },
+)
+
 StartRequestTypeDef = TypedDict(
     "StartRequestTypeDef",
     {
         "WorkspaceId": str,
     },
     total=False,
 )
@@ -931,15 +1023,14 @@
 
 UpdateResultTypeDef = TypedDict(
     "UpdateResultTypeDef",
     {
         "UpdateAvailable": bool,
         "Description": str,
     },
-    total=False,
 )
 
 UpdateWorkspaceBundleRequestRequestTypeDef = TypedDict(
     "UpdateWorkspaceBundleRequestRequestTypeDef",
     {
         "BundleId": str,
         "ImageId": str,
@@ -952,25 +1043,45 @@
     {
         "ImageId": str,
         "AllowCopyImage": bool,
         "SharedAccountId": str,
     },
 )
 
+UserStorageOutputTypeDef = TypedDict(
+    "UserStorageOutputTypeDef",
+    {
+        "Capacity": str,
+    },
+)
+
+WorkspaceAccessPropertiesOutputTypeDef = TypedDict(
+    "WorkspaceAccessPropertiesOutputTypeDef",
+    {
+        "DeviceTypeWindows": AccessPropertyValueType,
+        "DeviceTypeOsx": AccessPropertyValueType,
+        "DeviceTypeWeb": AccessPropertyValueType,
+        "DeviceTypeIos": AccessPropertyValueType,
+        "DeviceTypeAndroid": AccessPropertyValueType,
+        "DeviceTypeChromeOs": AccessPropertyValueType,
+        "DeviceTypeZeroClient": AccessPropertyValueType,
+        "DeviceTypeLinux": AccessPropertyValueType,
+    },
+)
+
 WorkspacePropertiesOutputTypeDef = TypedDict(
     "WorkspacePropertiesOutputTypeDef",
     {
         "RunningMode": RunningModeType,
         "RunningModeAutoStopTimeoutInMinutes": int,
         "RootVolumeSizeGib": int,
         "UserVolumeSizeGib": int,
         "ComputeTypeName": ComputeType,
         "Protocols": List[ProtocolType],
     },
-    total=False,
 )
 
 AssociateConnectionAliasResultTypeDef = TypedDict(
     "AssociateConnectionAliasResultTypeDef",
     {
         "ConnectionIdentifier": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1073,51 +1184,14 @@
     "UpdateRulesOfIpGroupRequestRequestTypeDef",
     {
         "GroupId": str,
         "UserRules": Sequence[IpRuleItemTypeDef],
     },
 )
 
-WorkspacesIpGroupTypeDef = TypedDict(
-    "WorkspacesIpGroupTypeDef",
-    {
-        "groupId": str,
-        "groupName": str,
-        "groupDesc": str,
-        "userRules": List[IpRuleItemTypeDef],
-    },
-    total=False,
-)
-
-DefaultImportClientBrandingAttributesTypeDef = TypedDict(
-    "DefaultImportClientBrandingAttributesTypeDef",
-    {
-        "Logo": BlobTypeDef,
-        "SupportEmail": str,
-        "SupportLink": str,
-        "ForgotPasswordLink": str,
-        "LoginMessage": Mapping[str, str],
-    },
-    total=False,
-)
-
-IosImportClientBrandingAttributesTypeDef = TypedDict(
-    "IosImportClientBrandingAttributesTypeDef",
-    {
-        "Logo": BlobTypeDef,
-        "Logo2x": BlobTypeDef,
-        "Logo3x": BlobTypeDef,
-        "SupportEmail": str,
-        "SupportLink": str,
-        "ForgotPasswordLink": str,
-        "LoginMessage": Mapping[str, str],
-    },
-    total=False,
-)
-
 _RequiredModifyCertificateBasedAuthPropertiesRequestRequestTypeDef = TypedDict(
     "_RequiredModifyCertificateBasedAuthPropertiesRequestRequestTypeDef",
     {
         "ResourceId": str,
     },
 )
 _OptionalModifyCertificateBasedAuthPropertiesRequestRequestTypeDef = TypedDict(
@@ -1137,17 +1211,16 @@
 ):
     pass
 
 ClientPropertiesResultTypeDef = TypedDict(
     "ClientPropertiesResultTypeDef",
     {
         "ResourceId": str,
-        "ClientProperties": ClientPropertiesTypeDef,
+        "ClientProperties": ClientPropertiesOutputTypeDef,
     },
-    total=False,
 )
 
 ModifyClientPropertiesRequestRequestTypeDef = TypedDict(
     "ModifyClientPropertiesRequestRequestTypeDef",
     {
         "ResourceId": str,
         "ClientProperties": ClientPropertiesTypeDef,
@@ -1168,22 +1241,21 @@
     {
         "ConnectionString": str,
         "AliasId": str,
         "State": ConnectionAliasStateType,
         "OwnerAccountId": str,
         "Associations": List[ConnectionAliasAssociationTypeDef],
     },
-    total=False,
 )
 
 DescribeConnectionAliasPermissionsResultTypeDef = TypedDict(
     "DescribeConnectionAliasPermissionsResultTypeDef",
     {
         "AliasId": str,
-        "ConnectionAliasPermissions": List[ConnectionAliasPermissionTypeDef],
+        "ConnectionAliasPermissions": List[ConnectionAliasPermissionOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateConnectionAliasPermissionRequestRequestTypeDef = TypedDict(
     "UpdateConnectionAliasPermissionRequestRequestTypeDef",
@@ -1305,22 +1377,14 @@
 
 class CreateWorkspaceImageRequestRequestTypeDef(
     _RequiredCreateWorkspaceImageRequestRequestTypeDef,
     _OptionalCreateWorkspaceImageRequestRequestTypeDef,
 ):
     pass
 
-DescribeTagsResultTypeDef = TypedDict(
-    "DescribeTagsResultTypeDef",
-    {
-        "TagList": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredImportWorkspaceImageRequestRequestTypeDef = TypedDict(
     "_RequiredImportWorkspaceImageRequestRequestTypeDef",
     {
         "Ec2ImageId": str,
         "IngestionProcess": WorkspaceImageIngestionProcessType,
         "ImageName": str,
         "ImageDescription": str,
@@ -1361,35 +1425,14 @@
 
 class RegisterWorkspaceDirectoryRequestRequestTypeDef(
     _RequiredRegisterWorkspaceDirectoryRequestRequestTypeDef,
     _OptionalRegisterWorkspaceDirectoryRequestRequestTypeDef,
 ):
     pass
 
-_RequiredStandbyWorkspaceOutputTypeDef = TypedDict(
-    "_RequiredStandbyWorkspaceOutputTypeDef",
-    {
-        "PrimaryWorkspaceId": str,
-        "DirectoryId": str,
-    },
-)
-_OptionalStandbyWorkspaceOutputTypeDef = TypedDict(
-    "_OptionalStandbyWorkspaceOutputTypeDef",
-    {
-        "VolumeEncryptionKey": str,
-        "Tags": List[TagTypeDef],
-    },
-    total=False,
-)
-
-class StandbyWorkspaceOutputTypeDef(
-    _RequiredStandbyWorkspaceOutputTypeDef, _OptionalStandbyWorkspaceOutputTypeDef
-):
-    pass
-
 _RequiredStandbyWorkspaceTypeDef = TypedDict(
     "_RequiredStandbyWorkspaceTypeDef",
     {
         "PrimaryWorkspaceId": str,
         "DirectoryId": str,
     },
 )
@@ -1426,33 +1469,14 @@
 
 class CreateWorkspaceBundleRequestRequestTypeDef(
     _RequiredCreateWorkspaceBundleRequestRequestTypeDef,
     _OptionalCreateWorkspaceBundleRequestRequestTypeDef,
 ):
     pass
 
-WorkspaceBundleTypeDef = TypedDict(
-    "WorkspaceBundleTypeDef",
-    {
-        "BundleId": str,
-        "Name": str,
-        "Owner": str,
-        "Description": str,
-        "ImageId": str,
-        "RootStorage": RootStorageTypeDef,
-        "UserStorage": UserStorageTypeDef,
-        "ComputeType": ComputeTypeTypeDef,
-        "LastUpdatedTime": datetime,
-        "CreationTime": datetime,
-        "State": WorkspaceBundleStateType,
-        "BundleType": BundleTypeType,
-    },
-    total=False,
-)
-
 CreateWorkspaceImageResultTypeDef = TypedDict(
     "CreateWorkspaceImageResultTypeDef",
     {
         "ImageId": str,
         "Name": str,
         "Description": str,
         "OperatingSystem": OperatingSystemTypeDef,
@@ -1574,14 +1598,32 @@
         "DeviceTypeIos": IosClientBrandingAttributesTypeDef,
         "DeviceTypeLinux": DefaultClientBrandingAttributesTypeDef,
         "DeviceTypeWeb": DefaultClientBrandingAttributesTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeTagsResultTypeDef = TypedDict(
+    "DescribeTagsResultTypeDef",
+    {
+        "TagList": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StandbyWorkspaceOutputTypeDef = TypedDict(
+    "StandbyWorkspaceOutputTypeDef",
+    {
+        "PrimaryWorkspaceId": str,
+        "VolumeEncryptionKey": str,
+        "DirectoryId": str,
+        "Tags": List[TagOutputTypeDef],
+    },
+)
+
 DescribeWorkspaceImagePermissionsResultTypeDef = TypedDict(
     "DescribeWorkspaceImagePermissionsResultTypeDef",
     {
         "ImageId": str,
         "ImagePermissions": List[ImagePermissionTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1642,14 +1684,49 @@
     "TerminateWorkspacesResultTypeDef",
     {
         "FailedRequests": List[FailedWorkspaceChangeRequestTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredImportClientBrandingRequestRequestTypeDef = TypedDict(
+    "_RequiredImportClientBrandingRequestRequestTypeDef",
+    {
+        "ResourceId": str,
+    },
+)
+_OptionalImportClientBrandingRequestRequestTypeDef = TypedDict(
+    "_OptionalImportClientBrandingRequestRequestTypeDef",
+    {
+        "DeviceTypeWindows": DefaultImportClientBrandingAttributesTypeDef,
+        "DeviceTypeOsx": DefaultImportClientBrandingAttributesTypeDef,
+        "DeviceTypeAndroid": DefaultImportClientBrandingAttributesTypeDef,
+        "DeviceTypeIos": IosImportClientBrandingAttributesTypeDef,
+        "DeviceTypeLinux": DefaultImportClientBrandingAttributesTypeDef,
+        "DeviceTypeWeb": DefaultImportClientBrandingAttributesTypeDef,
+    },
+    total=False,
+)
+
+class ImportClientBrandingRequestRequestTypeDef(
+    _RequiredImportClientBrandingRequestRequestTypeDef,
+    _OptionalImportClientBrandingRequestRequestTypeDef,
+):
+    pass
+
+WorkspacesIpGroupTypeDef = TypedDict(
+    "WorkspacesIpGroupTypeDef",
+    {
+        "groupId": str,
+        "groupName": str,
+        "groupDesc": str,
+        "userRules": List[IpRuleItemOutputTypeDef],
+    },
+)
+
 _RequiredModifySamlPropertiesRequestRequestTypeDef = TypedDict(
     "_RequiredModifySamlPropertiesRequestRequestTypeDef",
     {
         "ResourceId": str,
     },
 )
 _OptionalModifySamlPropertiesRequestRequestTypeDef = TypedDict(
@@ -1679,39 +1756,14 @@
     "ModifyWorkspaceAccessPropertiesRequestRequestTypeDef",
     {
         "ResourceId": str,
         "WorkspaceAccessProperties": WorkspaceAccessPropertiesTypeDef,
     },
 )
 
-WorkspaceDirectoryTypeDef = TypedDict(
-    "WorkspaceDirectoryTypeDef",
-    {
-        "DirectoryId": str,
-        "Alias": str,
-        "DirectoryName": str,
-        "RegistrationCode": str,
-        "SubnetIds": List[str],
-        "DnsIpAddresses": List[str],
-        "CustomerUserName": str,
-        "IamRoleId": str,
-        "DirectoryType": WorkspaceDirectoryTypeType,
-        "WorkspaceSecurityGroupId": str,
-        "State": WorkspaceDirectoryStateType,
-        "WorkspaceCreationProperties": DefaultWorkspaceCreationPropertiesTypeDef,
-        "ipGroupIds": List[str],
-        "WorkspaceAccessProperties": WorkspaceAccessPropertiesTypeDef,
-        "Tenancy": TenancyType,
-        "SelfservicePermissions": SelfservicePermissionsTypeDef,
-        "SamlProperties": SamlPropertiesTypeDef,
-        "CertificateBasedAuthProperties": CertificateBasedAuthPropertiesTypeDef,
-    },
-    total=False,
-)
-
 ModifyWorkspaceCreationPropertiesRequestRequestTypeDef = TypedDict(
     "ModifyWorkspaceCreationPropertiesRequestRequestTypeDef",
     {
         "ResourceId": str,
         "WorkspaceCreationProperties": WorkspaceCreationPropertiesTypeDef,
     },
 )
@@ -1793,45 +1845,72 @@
         "RequiredTenancy": WorkspaceImageRequiredTenancyType,
         "ErrorCode": str,
         "ErrorMessage": str,
         "Created": datetime,
         "OwnerAccountId": str,
         "Updates": UpdateResultTypeDef,
     },
-    total=False,
 )
 
-WorkspacePropertiesUnionTypeDef = Union[
-    WorkspacePropertiesTypeDef, WorkspacePropertiesOutputTypeDef
-]
-_RequiredWorkspaceRequestOutputTypeDef = TypedDict(
-    "_RequiredWorkspaceRequestOutputTypeDef",
+WorkspaceBundleTypeDef = TypedDict(
+    "WorkspaceBundleTypeDef",
     {
-        "DirectoryId": str,
-        "UserName": str,
         "BundleId": str,
+        "Name": str,
+        "Owner": str,
+        "Description": str,
+        "ImageId": str,
+        "RootStorage": RootStorageOutputTypeDef,
+        "UserStorage": UserStorageOutputTypeDef,
+        "ComputeType": ComputeTypeOutputTypeDef,
+        "LastUpdatedTime": datetime,
+        "CreationTime": datetime,
+        "State": WorkspaceBundleStateType,
+        "BundleType": BundleTypeType,
+    },
+)
+
+WorkspaceDirectoryTypeDef = TypedDict(
+    "WorkspaceDirectoryTypeDef",
+    {
+        "DirectoryId": str,
+        "Alias": str,
+        "DirectoryName": str,
+        "RegistrationCode": str,
+        "SubnetIds": List[str],
+        "DnsIpAddresses": List[str],
+        "CustomerUserName": str,
+        "IamRoleId": str,
+        "DirectoryType": WorkspaceDirectoryTypeType,
+        "WorkspaceSecurityGroupId": str,
+        "State": WorkspaceDirectoryStateType,
+        "WorkspaceCreationProperties": DefaultWorkspaceCreationPropertiesTypeDef,
+        "ipGroupIds": List[str],
+        "WorkspaceAccessProperties": WorkspaceAccessPropertiesOutputTypeDef,
+        "Tenancy": TenancyType,
+        "SelfservicePermissions": SelfservicePermissionsOutputTypeDef,
+        "SamlProperties": SamlPropertiesOutputTypeDef,
+        "CertificateBasedAuthProperties": CertificateBasedAuthPropertiesOutputTypeDef,
     },
 )
-_OptionalWorkspaceRequestOutputTypeDef = TypedDict(
-    "_OptionalWorkspaceRequestOutputTypeDef",
+
+WorkspaceRequestOutputTypeDef = TypedDict(
+    "WorkspaceRequestOutputTypeDef",
     {
+        "DirectoryId": str,
+        "UserName": str,
+        "BundleId": str,
         "VolumeEncryptionKey": str,
         "UserVolumeEncryptionEnabled": bool,
         "RootVolumeEncryptionEnabled": bool,
         "WorkspaceProperties": WorkspacePropertiesOutputTypeDef,
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
     },
-    total=False,
 )
 
-class WorkspaceRequestOutputTypeDef(
-    _RequiredWorkspaceRequestOutputTypeDef, _OptionalWorkspaceRequestOutputTypeDef
-):
-    pass
-
 WorkspaceTypeDef = TypedDict(
     "WorkspaceTypeDef",
     {
         "WorkspaceId": str,
         "DirectoryId": str,
         "UserName": str,
         "IpAddress": str,
@@ -1844,51 +1923,16 @@
         "VolumeEncryptionKey": str,
         "UserVolumeEncryptionEnabled": bool,
         "RootVolumeEncryptionEnabled": bool,
         "WorkspaceProperties": WorkspacePropertiesOutputTypeDef,
         "ModificationStates": List[ModificationStateTypeDef],
         "RelatedWorkspaces": List[RelatedWorkspacePropertiesTypeDef],
     },
-    total=False,
-)
-
-DescribeIpGroupsResultTypeDef = TypedDict(
-    "DescribeIpGroupsResultTypeDef",
-    {
-        "Result": List[WorkspacesIpGroupTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredImportClientBrandingRequestRequestTypeDef = TypedDict(
-    "_RequiredImportClientBrandingRequestRequestTypeDef",
-    {
-        "ResourceId": str,
-    },
-)
-_OptionalImportClientBrandingRequestRequestTypeDef = TypedDict(
-    "_OptionalImportClientBrandingRequestRequestTypeDef",
-    {
-        "DeviceTypeWindows": DefaultImportClientBrandingAttributesTypeDef,
-        "DeviceTypeOsx": DefaultImportClientBrandingAttributesTypeDef,
-        "DeviceTypeAndroid": DefaultImportClientBrandingAttributesTypeDef,
-        "DeviceTypeIos": IosImportClientBrandingAttributesTypeDef,
-        "DeviceTypeLinux": DefaultImportClientBrandingAttributesTypeDef,
-        "DeviceTypeWeb": DefaultImportClientBrandingAttributesTypeDef,
-    },
-    total=False,
 )
 
-class ImportClientBrandingRequestRequestTypeDef(
-    _RequiredImportClientBrandingRequestRequestTypeDef,
-    _OptionalImportClientBrandingRequestRequestTypeDef,
-):
-    pass
-
 DescribeClientPropertiesResultTypeDef = TypedDict(
     "DescribeClientPropertiesResultTypeDef",
     {
         "ClientPropertiesList": List[ClientPropertiesResultTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1898,25 +1942,56 @@
     {
         "ConnectionAliases": List[ConnectionAliasTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CreateStandbyWorkspacesRequestRequestTypeDef = TypedDict(
+    "CreateStandbyWorkspacesRequestRequestTypeDef",
+    {
+        "PrimaryRegion": str,
+        "StandbyWorkspaces": Sequence[StandbyWorkspaceTypeDef],
+    },
+)
+
 FailedCreateStandbyWorkspacesRequestTypeDef = TypedDict(
     "FailedCreateStandbyWorkspacesRequestTypeDef",
     {
         "StandbyWorkspaceRequest": StandbyWorkspaceOutputTypeDef,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
-    total=False,
 )
 
-StandbyWorkspaceUnionTypeDef = Union[StandbyWorkspaceTypeDef, StandbyWorkspaceOutputTypeDef]
+DescribeIpGroupsResultTypeDef = TypedDict(
+    "DescribeIpGroupsResultTypeDef",
+    {
+        "Result": List[WorkspacesIpGroupTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateWorkspacesRequestRequestTypeDef = TypedDict(
+    "CreateWorkspacesRequestRequestTypeDef",
+    {
+        "Workspaces": Sequence[WorkspaceRequestTypeDef],
+    },
+)
+
+DescribeWorkspaceImagesResultTypeDef = TypedDict(
+    "DescribeWorkspaceImagesResultTypeDef",
+    {
+        "Images": List[WorkspaceImageTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateWorkspaceBundleResultTypeDef = TypedDict(
     "CreateWorkspaceBundleResultTypeDef",
     {
         "WorkspaceBundle": WorkspaceBundleTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1935,34 +2010,23 @@
     {
         "Directories": List[WorkspaceDirectoryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeWorkspaceImagesResultTypeDef = TypedDict(
-    "DescribeWorkspaceImagesResultTypeDef",
-    {
-        "Images": List[WorkspaceImageTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 FailedCreateWorkspaceRequestTypeDef = TypedDict(
     "FailedCreateWorkspaceRequestTypeDef",
     {
         "WorkspaceRequest": WorkspaceRequestOutputTypeDef,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
-    total=False,
 )
 
-WorkspaceRequestUnionTypeDef = Union[WorkspaceRequestTypeDef, WorkspaceRequestOutputTypeDef]
 DescribeWorkspacesResultTypeDef = TypedDict(
     "DescribeWorkspacesResultTypeDef",
     {
         "Workspaces": List[WorkspaceTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1973,30 +2037,15 @@
     {
         "FailedStandbyRequests": List[FailedCreateStandbyWorkspacesRequestTypeDef],
         "PendingStandbyRequests": List[PendingCreateStandbyWorkspacesRequestTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateStandbyWorkspacesRequestRequestTypeDef = TypedDict(
-    "CreateStandbyWorkspacesRequestRequestTypeDef",
-    {
-        "PrimaryRegion": str,
-        "StandbyWorkspaces": Sequence[StandbyWorkspaceUnionTypeDef],
-    },
-)
-
 CreateWorkspacesResultTypeDef = TypedDict(
     "CreateWorkspacesResultTypeDef",
     {
         "FailedRequests": List[FailedCreateWorkspaceRequestTypeDef],
         "PendingRequests": List[WorkspaceTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-
-CreateWorkspacesRequestRequestTypeDef = TypedDict(
-    "CreateWorkspacesRequestRequestTypeDef",
-    {
-        "Workspaces": Sequence[WorkspaceRequestUnionTypeDef],
-    },
-)
```

### Comparing `mypy-boto3-workspaces-1.28.16/mypy_boto3_workspaces.egg-info/PKG-INFO` & `mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-workspaces
-Version: 1.28.16
-Summary: Type annotations for boto3.WorkSpaces 1.28.16 service generated with mypy-boto3-builder 7.17.1
+Version: 1.28.9
+Summary: Type annotations for boto3.WorkSpaces 1.28.9 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 workspaces type-annotations botocore mypy typeshed autocomplete
+Keywords: boto3 workspaces type-annotations boto3-stubs mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-workspaces"></a>
 
 # mypy-boto3-workspaces
 
 [![PyPI - mypy-boto3-workspaces](https://img.shields.io/pypi/v/mypy-boto3-workspaces.svg?color=blue)](https://pypi.org/project/mypy-boto3-workspaces)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-workspaces.svg?color=blue)](https://pypi.org/project/mypy-boto3-workspaces)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-workspaces)](https://pepy.tech/project/mypy-boto3-workspaces)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-workspaces?color=blue)](https://pypistats.org/packages/mypy-boto3-workspaces)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WorkSpaces 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces)
+[boto3.WorkSpaces 1.28.9](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.17.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-workspaces docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/).
 
 See how it helps to find and fix potential bugs:
 
@@ -74,15 +74,15 @@
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Literals](#literals)
-    - [Type definitions](#type-definitions)
+    - [Typed dictionaries](#typed-dictionaries)
   - [How it works](#how-it-works)
   - [What's new](#what's-new)
     - [Implemented features](#implemented-features)
     - [Latest changes](#latest-changes)
   - [Versioning](#versioning)
   - [Thank you](#thank-you)
   - [Documentation](#documentation)
@@ -379,42 +379,46 @@
 )
 
 
 def check_value(value: AccessPropertyValueType) -> bool:
     ...
 ```
 
-<a id="type-definitions"></a>
+<a id="typed-dictionaries"></a>
 
-### Type definitions
+### Typed dictionaries
 
 `mypy_boto3_workspaces.type_defs` module contains structures and shapes
-assembled to typed dictionaries and unions for additional type checking.
+assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_workspaces.type_defs import (
     AccountModificationTypeDef,
     AssociateConnectionAliasRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     AssociateIpGroupsRequestRequestTypeDef,
     IpRuleItemTypeDef,
-    BlobTypeDef,
+    CertificateBasedAuthPropertiesOutputTypeDef,
     CertificateBasedAuthPropertiesTypeDef,
+    ClientPropertiesOutputTypeDef,
     ClientPropertiesTypeDef,
+    ComputeTypeOutputTypeDef,
     ComputeTypeTypeDef,
     ConnectClientAddInTypeDef,
     ConnectionAliasAssociationTypeDef,
+    ConnectionAliasPermissionOutputTypeDef,
     ConnectionAliasPermissionTypeDef,
     TagTypeDef,
     CreateConnectClientAddInRequestRequestTypeDef,
     PendingCreateStandbyWorkspacesRequestTypeDef,
     RootStorageTypeDef,
     UserStorageTypeDef,
     OperatingSystemTypeDef,
     DefaultClientBrandingAttributesTypeDef,
+    DefaultImportClientBrandingAttributesTypeDef,
     DefaultWorkspaceCreationPropertiesTypeDef,
     DeleteClientBrandingRequestRequestTypeDef,
     DeleteConnectClientAddInRequestRequestTypeDef,
     DeleteConnectionAliasRequestRequestTypeDef,
     DeleteIpGroupRequestRequestTypeDef,
     DeleteTagsRequestRequestTypeDef,
     DeleteWorkspaceBundleRequestRequestTypeDef,
@@ -426,27 +430,30 @@
     IosClientBrandingAttributesTypeDef,
     DescribeClientPropertiesRequestRequestTypeDef,
     DescribeConnectClientAddInsRequestRequestTypeDef,
     DescribeConnectionAliasPermissionsRequestRequestTypeDef,
     DescribeConnectionAliasesRequestRequestTypeDef,
     DescribeIpGroupsRequestRequestTypeDef,
     DescribeTagsRequestRequestTypeDef,
+    TagOutputTypeDef,
     DescribeWorkspaceBundlesRequestRequestTypeDef,
     DescribeWorkspaceDirectoriesRequestRequestTypeDef,
     DescribeWorkspaceImagePermissionsRequestRequestTypeDef,
     ImagePermissionTypeDef,
     DescribeWorkspaceImagesRequestRequestTypeDef,
     DescribeWorkspaceSnapshotsRequestRequestTypeDef,
     SnapshotTypeDef,
     DescribeWorkspacesConnectionStatusRequestRequestTypeDef,
     WorkspaceConnectionStatusTypeDef,
     DescribeWorkspacesRequestRequestTypeDef,
     DisassociateConnectionAliasRequestRequestTypeDef,
     DisassociateIpGroupsRequestRequestTypeDef,
     FailedWorkspaceChangeRequestTypeDef,
+    IosImportClientBrandingAttributesTypeDef,
+    IpRuleItemOutputTypeDef,
     ListAvailableManagementCidrRangesRequestRequestTypeDef,
     MigrateWorkspaceRequestRequestTypeDef,
     ModificationStateTypeDef,
     ModifyAccountRequestRequestTypeDef,
     SamlPropertiesTypeDef,
     SelfservicePermissionsTypeDef,
     WorkspaceAccessPropertiesTypeDef,
@@ -454,114 +461,114 @@
     WorkspacePropertiesTypeDef,
     ModifyWorkspaceStateRequestRequestTypeDef,
     RebootRequestTypeDef,
     RebuildRequestTypeDef,
     RelatedWorkspacePropertiesTypeDef,
     RestoreWorkspaceRequestRequestTypeDef,
     RevokeIpRulesRequestRequestTypeDef,
+    RootStorageOutputTypeDef,
+    SamlPropertiesOutputTypeDef,
+    SelfservicePermissionsOutputTypeDef,
     StartRequestTypeDef,
     StopRequestTypeDef,
     TerminateRequestTypeDef,
     UpdateConnectClientAddInRequestRequestTypeDef,
     UpdateResultTypeDef,
     UpdateWorkspaceBundleRequestRequestTypeDef,
     UpdateWorkspaceImagePermissionRequestRequestTypeDef,
+    UserStorageOutputTypeDef,
+    WorkspaceAccessPropertiesOutputTypeDef,
     WorkspacePropertiesOutputTypeDef,
     AssociateConnectionAliasResultTypeDef,
     CopyWorkspaceImageResultTypeDef,
     CreateConnectClientAddInResultTypeDef,
     CreateConnectionAliasResultTypeDef,
     CreateIpGroupResultTypeDef,
     CreateUpdatedWorkspaceImageResultTypeDef,
     DescribeAccountModificationsResultTypeDef,
     DescribeAccountResultTypeDef,
     ImportWorkspaceImageResultTypeDef,
     ListAvailableManagementCidrRangesResultTypeDef,
     MigrateWorkspaceResultTypeDef,
     AuthorizeIpRulesRequestRequestTypeDef,
     UpdateRulesOfIpGroupRequestRequestTypeDef,
-    WorkspacesIpGroupTypeDef,
-    DefaultImportClientBrandingAttributesTypeDef,
-    IosImportClientBrandingAttributesTypeDef,
     ModifyCertificateBasedAuthPropertiesRequestRequestTypeDef,
     ClientPropertiesResultTypeDef,
     ModifyClientPropertiesRequestRequestTypeDef,
     DescribeConnectClientAddInsResultTypeDef,
     ConnectionAliasTypeDef,
     DescribeConnectionAliasPermissionsResultTypeDef,
     UpdateConnectionAliasPermissionRequestRequestTypeDef,
     CopyWorkspaceImageRequestRequestTypeDef,
     CreateConnectionAliasRequestRequestTypeDef,
     CreateIpGroupRequestRequestTypeDef,
     CreateTagsRequestRequestTypeDef,
     CreateUpdatedWorkspaceImageRequestRequestTypeDef,
     CreateWorkspaceImageRequestRequestTypeDef,
-    DescribeTagsResultTypeDef,
     ImportWorkspaceImageRequestRequestTypeDef,
     RegisterWorkspaceDirectoryRequestRequestTypeDef,
-    StandbyWorkspaceOutputTypeDef,
     StandbyWorkspaceTypeDef,
     CreateWorkspaceBundleRequestRequestTypeDef,
-    WorkspaceBundleTypeDef,
     CreateWorkspaceImageResultTypeDef,
     DescribeAccountModificationsRequestDescribeAccountModificationsPaginateTypeDef,
     DescribeIpGroupsRequestDescribeIpGroupsPaginateTypeDef,
     DescribeWorkspaceBundlesRequestDescribeWorkspaceBundlesPaginateTypeDef,
     DescribeWorkspaceDirectoriesRequestDescribeWorkspaceDirectoriesPaginateTypeDef,
     DescribeWorkspaceImagesRequestDescribeWorkspaceImagesPaginateTypeDef,
     DescribeWorkspacesConnectionStatusRequestDescribeWorkspacesConnectionStatusPaginateTypeDef,
     DescribeWorkspacesRequestDescribeWorkspacesPaginateTypeDef,
     ListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef,
     DescribeClientBrandingResultTypeDef,
     ImportClientBrandingResultTypeDef,
+    DescribeTagsResultTypeDef,
+    StandbyWorkspaceOutputTypeDef,
     DescribeWorkspaceImagePermissionsResultTypeDef,
     DescribeWorkspaceSnapshotsResultTypeDef,
     DescribeWorkspacesConnectionStatusResultTypeDef,
     RebootWorkspacesResultTypeDef,
     RebuildWorkspacesResultTypeDef,
     StartWorkspacesResultTypeDef,
     StopWorkspacesResultTypeDef,
     TerminateWorkspacesResultTypeDef,
+    ImportClientBrandingRequestRequestTypeDef,
+    WorkspacesIpGroupTypeDef,
     ModifySamlPropertiesRequestRequestTypeDef,
     ModifySelfservicePermissionsRequestRequestTypeDef,
     ModifyWorkspaceAccessPropertiesRequestRequestTypeDef,
-    WorkspaceDirectoryTypeDef,
     ModifyWorkspaceCreationPropertiesRequestRequestTypeDef,
     ModifyWorkspacePropertiesRequestRequestTypeDef,
     WorkspaceRequestTypeDef,
     RebootWorkspacesRequestRequestTypeDef,
     RebuildWorkspacesRequestRequestTypeDef,
     StartWorkspacesRequestRequestTypeDef,
     StopWorkspacesRequestRequestTypeDef,
     TerminateWorkspacesRequestRequestTypeDef,
     WorkspaceImageTypeDef,
-    WorkspacePropertiesUnionTypeDef,
+    WorkspaceBundleTypeDef,
+    WorkspaceDirectoryTypeDef,
     WorkspaceRequestOutputTypeDef,
     WorkspaceTypeDef,
-    DescribeIpGroupsResultTypeDef,
-    ImportClientBrandingRequestRequestTypeDef,
     DescribeClientPropertiesResultTypeDef,
     DescribeConnectionAliasesResultTypeDef,
+    CreateStandbyWorkspacesRequestRequestTypeDef,
     FailedCreateStandbyWorkspacesRequestTypeDef,
-    StandbyWorkspaceUnionTypeDef,
+    DescribeIpGroupsResultTypeDef,
+    CreateWorkspacesRequestRequestTypeDef,
+    DescribeWorkspaceImagesResultTypeDef,
     CreateWorkspaceBundleResultTypeDef,
     DescribeWorkspaceBundlesResultTypeDef,
     DescribeWorkspaceDirectoriesResultTypeDef,
-    DescribeWorkspaceImagesResultTypeDef,
     FailedCreateWorkspaceRequestTypeDef,
-    WorkspaceRequestUnionTypeDef,
     DescribeWorkspacesResultTypeDef,
     CreateStandbyWorkspacesResultTypeDef,
-    CreateStandbyWorkspacesRequestRequestTypeDef,
     CreateWorkspacesResultTypeDef,
-    CreateWorkspacesRequestRequestTypeDef,
 )
 
 
-def get_value() -> AccountModificationTypeDef:
+def get_structure() -> AccountModificationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-workspaces-1.28.16/mypy_boto3_workspaces.egg-info/SOURCES.txt` & `mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workspaces-1.28.16/setup.py` & `mypy-boto3-workspaces-1.28.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-workspaces",
-    version="1.28.16",
+    version="1.28.9",
     packages=["mypy_boto3_workspaces"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.WorkSpaces 1.28.16 service generated with mypy-boto3-builder"
-        " 7.17.1"
+        "Type annotations for boto3.WorkSpaces 1.28.9 service generated with mypy-boto3-builder"
+        " 7.15.1"
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
-    keywords="boto3 workspaces type-annotations botocore mypy typeshed autocomplete",
+    keywords="boto3 workspaces type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_workspaces": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

