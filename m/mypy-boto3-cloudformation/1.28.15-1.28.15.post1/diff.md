# Comparing `tmp/mypy-boto3-cloudformation-1.28.15.tar.gz` & `tmp/mypy-boto3-cloudformation-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cloudformation-1.28.15.tar", last modified: Fri Jul 28 19:47:31 2023, max compression
+gzip compressed data, was "mypy-boto3-cloudformation-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:41 2023, max compression
```

## Comparing `mypy-boto3-cloudformation-1.28.15.tar` & `mypy-boto3-cloudformation-1.28.15.post1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:47:31.692180 mypy-boto3-cloudformation-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 19:46:50.000000 mypy-boto3-cloudformation-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    30041 2023-07-28 19:47:31.692180 mypy-boto3-cloudformation-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    28526 2023-07-28 19:46:50.000000 mypy-boto3-cloudformation-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:47:31.692180 mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation/
--rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-07-28 19:46:50.000000 mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-07-28 19:46:50.000000 mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-28 19:46:50.000000 mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    66347 2023-07-28 19:46:51.000000 mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    66248 2023-07-28 19:46:50.000000 mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18517 2023-07-28 19:46:51.000000 mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    18515 2023-07-28 19:46:51.000000 mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17280 2023-07-28 19:46:51.000000 mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17264 2023-07-28 19:46:51.000000 mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 19:46:50.000000 mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    22955 2023-07-28 19:46:51.000000 mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    22911 2023-07-28 19:46:51.000000 mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    93669 2023-07-28 19:46:53.000000 mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    93552 2023-07-28 19:46:53.000000 mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 19:46:50.000000 mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     8787 2023-07-28 19:46:51.000000 mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8779 2023-07-28 19:46:51.000000 mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:47:31.692180 mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    30041 2023-07-28 19:47:31.000000 mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-28 19:47:31.000000 mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 19:47:31.000000 mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 19:47:31.000000 mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 19:47:31.000000 mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-28 19:47:31.000000 mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 19:47:31.692180 mypy-boto3-cloudformation-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-28 19:46:49.000000 mypy-boto3-cloudformation-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:41.481050 mypy-boto3-cloudformation-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:39:51.000000 mypy-boto3-cloudformation-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    30047 2023-07-29 10:02:41.477050 mypy-boto3-cloudformation-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    28526 2023-07-29 09:39:51.000000 mypy-boto3-cloudformation-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:41.469050 mypy-boto3-cloudformation-1.28.15.post1/mypy_boto3_cloudformation/
+-rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-07-29 09:39:51.000000 mypy-boto3-cloudformation-1.28.15.post1/mypy_boto3_cloudformation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-07-29 09:39:51.000000 mypy-boto3-cloudformation-1.28.15.post1/mypy_boto3_cloudformation/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-29 09:39:51.000000 mypy-boto3-cloudformation-1.28.15.post1/mypy_boto3_cloudformation/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67260 2023-07-29 09:39:52.000000 mypy-boto3-cloudformation-1.28.15.post1/mypy_boto3_cloudformation/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67161 2023-07-29 09:39:51.000000 mypy-boto3-cloudformation-1.28.15.post1/mypy_boto3_cloudformation/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18517 2023-07-29 09:39:54.000000 mypy-boto3-cloudformation-1.28.15.post1/mypy_boto3_cloudformation/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18515 2023-07-29 09:39:53.000000 mypy-boto3-cloudformation-1.28.15.post1/mypy_boto3_cloudformation/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17280 2023-07-29 09:39:52.000000 mypy-boto3-cloudformation-1.28.15.post1/mypy_boto3_cloudformation/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17264 2023-07-29 09:39:52.000000 mypy-boto3-cloudformation-1.28.15.post1/mypy_boto3_cloudformation/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:39:51.000000 mypy-boto3-cloudformation-1.28.15.post1/mypy_boto3_cloudformation/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    23067 2023-07-29 09:39:52.000000 mypy-boto3-cloudformation-1.28.15.post1/mypy_boto3_cloudformation/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23023 2023-07-29 09:39:52.000000 mypy-boto3-cloudformation-1.28.15.post1/mypy_boto3_cloudformation/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    93701 2023-07-29 09:39:56.000000 mypy-boto3-cloudformation-1.28.15.post1/mypy_boto3_cloudformation/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93584 2023-07-29 09:39:55.000000 mypy-boto3-cloudformation-1.28.15.post1/mypy_boto3_cloudformation/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:39:51.000000 mypy-boto3-cloudformation-1.28.15.post1/mypy_boto3_cloudformation/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8787 2023-07-29 09:39:52.000000 mypy-boto3-cloudformation-1.28.15.post1/mypy_boto3_cloudformation/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8779 2023-07-29 09:39:52.000000 mypy-boto3-cloudformation-1.28.15.post1/mypy_boto3_cloudformation/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:41.477050 mypy-boto3-cloudformation-1.28.15.post1/mypy_boto3_cloudformation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    30047 2023-07-29 10:02:41.000000 mypy-boto3-cloudformation-1.28.15.post1/mypy_boto3_cloudformation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-29 10:02:41.000000 mypy-boto3-cloudformation-1.28.15.post1/mypy_boto3_cloudformation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:41.000000 mypy-boto3-cloudformation-1.28.15.post1/mypy_boto3_cloudformation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:41.000000 mypy-boto3-cloudformation-1.28.15.post1/mypy_boto3_cloudformation.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:41.000000 mypy-boto3-cloudformation-1.28.15.post1/mypy_boto3_cloudformation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-29 10:02:41.000000 mypy-boto3-cloudformation-1.28.15.post1/mypy_boto3_cloudformation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:41.481050 mypy-boto3-cloudformation-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-29 09:39:51.000000 mypy-boto3-cloudformation-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-cloudformation-1.28.15/LICENSE` & `mypy-boto3-cloudformation-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudformation-1.28.15/PKG-INFO` & `mypy-boto3-cloudformation-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudformation
-Version: 1.28.15
-Summary: Type annotations for boto3.CloudFormation 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.CloudFormation 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -47,15 +47,15 @@
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.16.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.16.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-cloudformation docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-cloudformation-1.28.15/README.md` & `mypy-boto3-cloudformation-1.28.15.post1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.16.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.16.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-cloudformation docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation/__init__.py` & `mypy-boto3-cloudformation-1.28.15.post1/mypy_boto3_cloudformation/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation/__init__.pyi` & `mypy-boto3-cloudformation-1.28.15.post1/mypy_boto3_cloudformation/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation/__main__.py` & `mypy-boto3-cloudformation-1.28.15.post1/mypy_boto3_cloudformation/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CloudFormation 1.28.15\nVersion:         1.28.15\nBuilder"
-        " version: 7.16.1\nDocs:           "
+        "Type annotations for boto3.CloudFormation 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.15")
+    print("1.28.15.post1")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation/client.py` & `mypy-boto3-cloudformation-1.28.15.post1/mypy_boto3_cloudformation/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_cloudformation.client import CloudFormationClient
 
     session = Session()
     client: CloudFormationClient = session.client("cloudformation")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     CallAsType,
     CapabilityType,
     ChangeSetTypeType,
@@ -61,14 +61,15 @@
     AutoDeploymentTypeDef,
     BatchDescribeTypeConfigurationsOutputTypeDef,
     CreateChangeSetOutputTypeDef,
     CreateStackInstancesOutputTypeDef,
     CreateStackOutputTypeDef,
     CreateStackSetOutputTypeDef,
     DeleteStackInstancesOutputTypeDef,
+    DeploymentTargetsOutputTypeDef,
     DeploymentTargetsTypeDef,
     DescribeAccountLimitsOutputTypeDef,
     DescribeChangeSetHooksOutputTypeDef,
     DescribeChangeSetOutputTypeDef,
     DescribeOrganizationsAccessOutputTypeDef,
     DescribePublisherOutputTypeDef,
     DescribeStackDriftDetectionStatusOutputTypeDef,
@@ -108,18 +109,20 @@
     ManagedExecutionTypeDef,
     OperationResultFilterTypeDef,
     ParameterTypeDef,
     PublishTypeOutputTypeDef,
     RegisterPublisherOutputTypeDef,
     RegisterTypeOutputTypeDef,
     ResourceToImportTypeDef,
+    RollbackConfigurationOutputTypeDef,
     RollbackConfigurationTypeDef,
     RollbackStackOutputTypeDef,
     SetTypeConfigurationOutputTypeDef,
     StackInstanceFilterTypeDef,
+    StackSetOperationPreferencesOutputTypeDef,
     StackSetOperationPreferencesTypeDef,
     TagTypeDef,
     TemplateSummaryConfigTypeDef,
     TestTypeOutputTypeDef,
     TypeConfigurationIdentifierTypeDef,
     TypeFiltersTypeDef,
     UpdateStackInstancesOutputTypeDef,
@@ -290,15 +293,17 @@
         TemplateBody: str = ...,
         TemplateURL: str = ...,
         UsePreviousTemplate: bool = ...,
         Parameters: Sequence[ParameterTypeDef] = ...,
         Capabilities: Sequence[CapabilityType] = ...,
         ResourceTypes: Sequence[str] = ...,
         RoleARN: str = ...,
-        RollbackConfiguration: RollbackConfigurationTypeDef = ...,
+        RollbackConfiguration: Union[
+            RollbackConfigurationTypeDef, RollbackConfigurationOutputTypeDef
+        ] = ...,
         NotificationARNs: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ClientToken: str = ...,
         Description: str = ...,
         ChangeSetType: ChangeSetTypeType = ...,
         ResourcesToImport: Sequence[ResourceToImportTypeDef] = ...,
         IncludeNestedStacks: bool = ...,
@@ -316,15 +321,17 @@
         self,
         *,
         StackName: str,
         TemplateBody: str = ...,
         TemplateURL: str = ...,
         Parameters: Sequence[ParameterTypeDef] = ...,
         DisableRollback: bool = ...,
-        RollbackConfiguration: RollbackConfigurationTypeDef = ...,
+        RollbackConfiguration: Union[
+            RollbackConfigurationTypeDef, RollbackConfigurationOutputTypeDef
+        ] = ...,
         TimeoutInMinutes: int = ...,
         NotificationARNs: Sequence[str] = ...,
         Capabilities: Sequence[CapabilityType] = ...,
         ResourceTypes: Sequence[str] = ...,
         RoleARN: str = ...,
         OnFailure: OnFailureType = ...,
         StackPolicyBody: str = ...,
@@ -343,17 +350,19 @@
 
     def create_stack_instances(
         self,
         *,
         StackSetName: str,
         Regions: Sequence[str],
         Accounts: Sequence[str] = ...,
-        DeploymentTargets: DeploymentTargetsTypeDef = ...,
+        DeploymentTargets: Union[DeploymentTargetsTypeDef, DeploymentTargetsOutputTypeDef] = ...,
         ParameterOverrides: Sequence[ParameterTypeDef] = ...,
-        OperationPreferences: StackSetOperationPreferencesTypeDef = ...,
+        OperationPreferences: Union[
+            StackSetOperationPreferencesTypeDef, StackSetOperationPreferencesOutputTypeDef
+        ] = ...,
         OperationId: str = ...,
         CallAs: CallAsType = ...
     ) -> CreateStackInstancesOutputTypeDef:
         """
         Creates stack instances for the specified accounts, within the specified Amazon
         Web Services Regions.
 
@@ -432,16 +441,18 @@
     def delete_stack_instances(
         self,
         *,
         StackSetName: str,
         Regions: Sequence[str],
         RetainStacks: bool,
         Accounts: Sequence[str] = ...,
-        DeploymentTargets: DeploymentTargetsTypeDef = ...,
-        OperationPreferences: StackSetOperationPreferencesTypeDef = ...,
+        DeploymentTargets: Union[DeploymentTargetsTypeDef, DeploymentTargetsOutputTypeDef] = ...,
+        OperationPreferences: Union[
+            StackSetOperationPreferencesTypeDef, StackSetOperationPreferencesOutputTypeDef
+        ] = ...,
         OperationId: str = ...,
         CallAs: CallAsType = ...
     ) -> DeleteStackInstancesOutputTypeDef:
         """
         Deletes stack instances for the specified accounts, in the specified Amazon Web
         Services Regions.
 
@@ -686,15 +697,17 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/client/#detect_stack_resource_drift)
         """
 
     def detect_stack_set_drift(
         self,
         *,
         StackSetName: str,
-        OperationPreferences: StackSetOperationPreferencesTypeDef = ...,
+        OperationPreferences: Union[
+            StackSetOperationPreferencesTypeDef, StackSetOperationPreferencesOutputTypeDef
+        ] = ...,
         OperationId: str = ...,
         CallAs: CallAsType = ...
     ) -> DetectStackSetDriftOutputTypeDef:
         """
         Detect drift on a stack set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.detect_stack_set_drift)
@@ -788,15 +801,17 @@
     def import_stacks_to_stack_set(
         self,
         *,
         StackSetName: str,
         StackIds: Sequence[str] = ...,
         StackIdsUrl: str = ...,
         OrganizationalUnitIds: Sequence[str] = ...,
-        OperationPreferences: StackSetOperationPreferencesTypeDef = ...,
+        OperationPreferences: Union[
+            StackSetOperationPreferencesTypeDef, StackSetOperationPreferencesOutputTypeDef
+        ] = ...,
         OperationId: str = ...,
         CallAs: CallAsType = ...
     ) -> ImportStacksToStackSetOutputTypeDef:
         """
         Import existing stacks into a new stack sets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.import_stacks_to_stack_set)
@@ -1162,15 +1177,17 @@
         UsePreviousTemplate: bool = ...,
         StackPolicyDuringUpdateBody: str = ...,
         StackPolicyDuringUpdateURL: str = ...,
         Parameters: Sequence[ParameterTypeDef] = ...,
         Capabilities: Sequence[CapabilityType] = ...,
         ResourceTypes: Sequence[str] = ...,
         RoleARN: str = ...,
-        RollbackConfiguration: RollbackConfigurationTypeDef = ...,
+        RollbackConfiguration: Union[
+            RollbackConfigurationTypeDef, RollbackConfigurationOutputTypeDef
+        ] = ...,
         StackPolicyBody: str = ...,
         StackPolicyURL: str = ...,
         NotificationARNs: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         DisableRollback: bool = ...,
         ClientRequestToken: str = ...,
         RetainExceptOnCreate: bool = ...
@@ -1184,17 +1201,19 @@
 
     def update_stack_instances(
         self,
         *,
         StackSetName: str,
         Regions: Sequence[str],
         Accounts: Sequence[str] = ...,
-        DeploymentTargets: DeploymentTargetsTypeDef = ...,
+        DeploymentTargets: Union[DeploymentTargetsTypeDef, DeploymentTargetsOutputTypeDef] = ...,
         ParameterOverrides: Sequence[ParameterTypeDef] = ...,
-        OperationPreferences: StackSetOperationPreferencesTypeDef = ...,
+        OperationPreferences: Union[
+            StackSetOperationPreferencesTypeDef, StackSetOperationPreferencesOutputTypeDef
+        ] = ...,
         OperationId: str = ...,
         CallAs: CallAsType = ...
     ) -> UpdateStackInstancesOutputTypeDef:
         """
         Updates the parameter values for stack instances for the specified accounts,
         within the specified Amazon Web Services Regions.
 
@@ -1209,18 +1228,20 @@
         Description: str = ...,
         TemplateBody: str = ...,
         TemplateURL: str = ...,
         UsePreviousTemplate: bool = ...,
         Parameters: Sequence[ParameterTypeDef] = ...,
         Capabilities: Sequence[CapabilityType] = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        OperationPreferences: StackSetOperationPreferencesTypeDef = ...,
+        OperationPreferences: Union[
+            StackSetOperationPreferencesTypeDef, StackSetOperationPreferencesOutputTypeDef
+        ] = ...,
         AdministrationRoleARN: str = ...,
         ExecutionRoleName: str = ...,
-        DeploymentTargets: DeploymentTargetsTypeDef = ...,
+        DeploymentTargets: Union[DeploymentTargetsTypeDef, DeploymentTargetsOutputTypeDef] = ...,
         PermissionModel: PermissionModelsType = ...,
         AutoDeployment: AutoDeploymentTypeDef = ...,
         OperationId: str = ...,
         Accounts: Sequence[str] = ...,
         Regions: Sequence[str] = ...,
         CallAs: CallAsType = ...,
         ManagedExecution: ManagedExecutionTypeDef = ...
```

### Comparing `mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation/client.pyi` & `mypy-boto3-cloudformation-1.28.15.post1/mypy_boto3_cloudformation/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_cloudformation.client import CloudFormationClient
 
     session = Session()
     client: CloudFormationClient = session.client("cloudformation")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     CallAsType,
     CapabilityType,
     ChangeSetTypeType,
@@ -61,14 +61,15 @@
     AutoDeploymentTypeDef,
     BatchDescribeTypeConfigurationsOutputTypeDef,
     CreateChangeSetOutputTypeDef,
     CreateStackInstancesOutputTypeDef,
     CreateStackOutputTypeDef,
     CreateStackSetOutputTypeDef,
     DeleteStackInstancesOutputTypeDef,
+    DeploymentTargetsOutputTypeDef,
     DeploymentTargetsTypeDef,
     DescribeAccountLimitsOutputTypeDef,
     DescribeChangeSetHooksOutputTypeDef,
     DescribeChangeSetOutputTypeDef,
     DescribeOrganizationsAccessOutputTypeDef,
     DescribePublisherOutputTypeDef,
     DescribeStackDriftDetectionStatusOutputTypeDef,
@@ -108,18 +109,20 @@
     ManagedExecutionTypeDef,
     OperationResultFilterTypeDef,
     ParameterTypeDef,
     PublishTypeOutputTypeDef,
     RegisterPublisherOutputTypeDef,
     RegisterTypeOutputTypeDef,
     ResourceToImportTypeDef,
+    RollbackConfigurationOutputTypeDef,
     RollbackConfigurationTypeDef,
     RollbackStackOutputTypeDef,
     SetTypeConfigurationOutputTypeDef,
     StackInstanceFilterTypeDef,
+    StackSetOperationPreferencesOutputTypeDef,
     StackSetOperationPreferencesTypeDef,
     TagTypeDef,
     TemplateSummaryConfigTypeDef,
     TestTypeOutputTypeDef,
     TypeConfigurationIdentifierTypeDef,
     TypeFiltersTypeDef,
     UpdateStackInstancesOutputTypeDef,
@@ -278,15 +281,17 @@
         TemplateBody: str = ...,
         TemplateURL: str = ...,
         UsePreviousTemplate: bool = ...,
         Parameters: Sequence[ParameterTypeDef] = ...,
         Capabilities: Sequence[CapabilityType] = ...,
         ResourceTypes: Sequence[str] = ...,
         RoleARN: str = ...,
-        RollbackConfiguration: RollbackConfigurationTypeDef = ...,
+        RollbackConfiguration: Union[
+            RollbackConfigurationTypeDef, RollbackConfigurationOutputTypeDef
+        ] = ...,
         NotificationARNs: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ClientToken: str = ...,
         Description: str = ...,
         ChangeSetType: ChangeSetTypeType = ...,
         ResourcesToImport: Sequence[ResourceToImportTypeDef] = ...,
         IncludeNestedStacks: bool = ...,
@@ -303,15 +308,17 @@
         self,
         *,
         StackName: str,
         TemplateBody: str = ...,
         TemplateURL: str = ...,
         Parameters: Sequence[ParameterTypeDef] = ...,
         DisableRollback: bool = ...,
-        RollbackConfiguration: RollbackConfigurationTypeDef = ...,
+        RollbackConfiguration: Union[
+            RollbackConfigurationTypeDef, RollbackConfigurationOutputTypeDef
+        ] = ...,
         TimeoutInMinutes: int = ...,
         NotificationARNs: Sequence[str] = ...,
         Capabilities: Sequence[CapabilityType] = ...,
         ResourceTypes: Sequence[str] = ...,
         RoleARN: str = ...,
         OnFailure: OnFailureType = ...,
         StackPolicyBody: str = ...,
@@ -329,17 +336,19 @@
         """
     def create_stack_instances(
         self,
         *,
         StackSetName: str,
         Regions: Sequence[str],
         Accounts: Sequence[str] = ...,
-        DeploymentTargets: DeploymentTargetsTypeDef = ...,
+        DeploymentTargets: Union[DeploymentTargetsTypeDef, DeploymentTargetsOutputTypeDef] = ...,
         ParameterOverrides: Sequence[ParameterTypeDef] = ...,
-        OperationPreferences: StackSetOperationPreferencesTypeDef = ...,
+        OperationPreferences: Union[
+            StackSetOperationPreferencesTypeDef, StackSetOperationPreferencesOutputTypeDef
+        ] = ...,
         OperationId: str = ...,
         CallAs: CallAsType = ...
     ) -> CreateStackInstancesOutputTypeDef:
         """
         Creates stack instances for the specified accounts, within the specified Amazon
         Web Services Regions.
 
@@ -412,16 +421,18 @@
     def delete_stack_instances(
         self,
         *,
         StackSetName: str,
         Regions: Sequence[str],
         RetainStacks: bool,
         Accounts: Sequence[str] = ...,
-        DeploymentTargets: DeploymentTargetsTypeDef = ...,
-        OperationPreferences: StackSetOperationPreferencesTypeDef = ...,
+        DeploymentTargets: Union[DeploymentTargetsTypeDef, DeploymentTargetsOutputTypeDef] = ...,
+        OperationPreferences: Union[
+            StackSetOperationPreferencesTypeDef, StackSetOperationPreferencesOutputTypeDef
+        ] = ...,
         OperationId: str = ...,
         CallAs: CallAsType = ...
     ) -> DeleteStackInstancesOutputTypeDef:
         """
         Deletes stack instances for the specified accounts, in the specified Amazon Web
         Services Regions.
 
@@ -645,15 +656,17 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.detect_stack_resource_drift)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/client/#detect_stack_resource_drift)
         """
     def detect_stack_set_drift(
         self,
         *,
         StackSetName: str,
-        OperationPreferences: StackSetOperationPreferencesTypeDef = ...,
+        OperationPreferences: Union[
+            StackSetOperationPreferencesTypeDef, StackSetOperationPreferencesOutputTypeDef
+        ] = ...,
         OperationId: str = ...,
         CallAs: CallAsType = ...
     ) -> DetectStackSetDriftOutputTypeDef:
         """
         Detect drift on a stack set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.detect_stack_set_drift)
@@ -740,15 +753,17 @@
     def import_stacks_to_stack_set(
         self,
         *,
         StackSetName: str,
         StackIds: Sequence[str] = ...,
         StackIdsUrl: str = ...,
         OrganizationalUnitIds: Sequence[str] = ...,
-        OperationPreferences: StackSetOperationPreferencesTypeDef = ...,
+        OperationPreferences: Union[
+            StackSetOperationPreferencesTypeDef, StackSetOperationPreferencesOutputTypeDef
+        ] = ...,
         OperationId: str = ...,
         CallAs: CallAsType = ...
     ) -> ImportStacksToStackSetOutputTypeDef:
         """
         Import existing stacks into a new stack sets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.import_stacks_to_stack_set)
@@ -1089,15 +1104,17 @@
         UsePreviousTemplate: bool = ...,
         StackPolicyDuringUpdateBody: str = ...,
         StackPolicyDuringUpdateURL: str = ...,
         Parameters: Sequence[ParameterTypeDef] = ...,
         Capabilities: Sequence[CapabilityType] = ...,
         ResourceTypes: Sequence[str] = ...,
         RoleARN: str = ...,
-        RollbackConfiguration: RollbackConfigurationTypeDef = ...,
+        RollbackConfiguration: Union[
+            RollbackConfigurationTypeDef, RollbackConfigurationOutputTypeDef
+        ] = ...,
         StackPolicyBody: str = ...,
         StackPolicyURL: str = ...,
         NotificationARNs: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         DisableRollback: bool = ...,
         ClientRequestToken: str = ...,
         RetainExceptOnCreate: bool = ...
@@ -1110,17 +1127,19 @@
         """
     def update_stack_instances(
         self,
         *,
         StackSetName: str,
         Regions: Sequence[str],
         Accounts: Sequence[str] = ...,
-        DeploymentTargets: DeploymentTargetsTypeDef = ...,
+        DeploymentTargets: Union[DeploymentTargetsTypeDef, DeploymentTargetsOutputTypeDef] = ...,
         ParameterOverrides: Sequence[ParameterTypeDef] = ...,
-        OperationPreferences: StackSetOperationPreferencesTypeDef = ...,
+        OperationPreferences: Union[
+            StackSetOperationPreferencesTypeDef, StackSetOperationPreferencesOutputTypeDef
+        ] = ...,
         OperationId: str = ...,
         CallAs: CallAsType = ...
     ) -> UpdateStackInstancesOutputTypeDef:
         """
         Updates the parameter values for stack instances for the specified accounts,
         within the specified Amazon Web Services Regions.
 
@@ -1134,18 +1153,20 @@
         Description: str = ...,
         TemplateBody: str = ...,
         TemplateURL: str = ...,
         UsePreviousTemplate: bool = ...,
         Parameters: Sequence[ParameterTypeDef] = ...,
         Capabilities: Sequence[CapabilityType] = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        OperationPreferences: StackSetOperationPreferencesTypeDef = ...,
+        OperationPreferences: Union[
+            StackSetOperationPreferencesTypeDef, StackSetOperationPreferencesOutputTypeDef
+        ] = ...,
         AdministrationRoleARN: str = ...,
         ExecutionRoleName: str = ...,
-        DeploymentTargets: DeploymentTargetsTypeDef = ...,
+        DeploymentTargets: Union[DeploymentTargetsTypeDef, DeploymentTargetsOutputTypeDef] = ...,
         PermissionModel: PermissionModelsType = ...,
         AutoDeployment: AutoDeploymentTypeDef = ...,
         OperationId: str = ...,
         Accounts: Sequence[str] = ...,
         Regions: Sequence[str] = ...,
         CallAs: CallAsType = ...,
         ManagedExecution: ManagedExecutionTypeDef = ...
```

### Comparing `mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation/literals.py` & `mypy-boto3-cloudformation-1.28.15.post1/mypy_boto3_cloudformation/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation/literals.pyi` & `mypy-boto3-cloudformation-1.28.15.post1/mypy_boto3_cloudformation/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation/paginator.py` & `mypy-boto3-cloudformation-1.28.15.post1/mypy_boto3_cloudformation/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation/paginator.pyi` & `mypy-boto3-cloudformation-1.28.15.post1/mypy_boto3_cloudformation/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation/service_resource.py` & `mypy-boto3-cloudformation-1.28.15.post1/mypy_boto3_cloudformation/service_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     my_stack: cloudformation_resources.Stack = resource.Stack(...)
     my_stack_resource: cloudformation_resources.StackResource = resource.StackResource(...)
     my_stack_resource_summary: cloudformation_resources.StackResourceSummary = resource.StackResourceSummary(...)
 ```
 """
 import sys
 from datetime import datetime
-from typing import Iterator, List, Sequence
+from typing import Iterator, List, Sequence, Union
 
 from boto3.resources.base import ResourceMeta, ServiceResource
 from boto3.resources.collection import ResourceCollection
 
 from .client import CloudFormationClient
 from .literals import (
     CapabilityType,
@@ -36,14 +36,15 @@
     ResourceStatusType,
     StackStatusType,
 )
 from .type_defs import (
     ModuleInfoResponseTypeDef,
     OutputTypeDef,
     ParameterTypeDef,
+    RollbackConfigurationOutputTypeDef,
     RollbackConfigurationTypeDef,
     StackDriftInformationResponseTypeDef,
     StackResourceDriftInformationResponseTypeDef,
     StackResourceDriftInformationSummaryResponseTypeDef,
     TagTypeDef,
     UpdateStackOutputTypeDef,
 )
@@ -490,15 +491,17 @@
         self,
         *,
         StackName: str,
         TemplateBody: str = ...,
         TemplateURL: str = ...,
         Parameters: Sequence[ParameterTypeDef] = ...,
         DisableRollback: bool = ...,
-        RollbackConfiguration: RollbackConfigurationTypeDef = ...,
+        RollbackConfiguration: Union[
+            RollbackConfigurationTypeDef, RollbackConfigurationOutputTypeDef
+        ] = ...,
         TimeoutInMinutes: int = ...,
         NotificationARNs: Sequence[str] = ...,
         Capabilities: Sequence[CapabilityType] = ...,
         ResourceTypes: Sequence[str] = ...,
         RoleARN: str = ...,
         OnFailure: OnFailureType = ...,
         StackPolicyBody: str = ...,
```

### Comparing `mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation/service_resource.pyi` & `mypy-boto3-cloudformation-1.28.15.post1/mypy_boto3_cloudformation/service_resource.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     my_stack: cloudformation_resources.Stack = resource.Stack(...)
     my_stack_resource: cloudformation_resources.StackResource = resource.StackResource(...)
     my_stack_resource_summary: cloudformation_resources.StackResourceSummary = resource.StackResourceSummary(...)
 ```
 """
 import sys
 from datetime import datetime
-from typing import Iterator, List, Sequence
+from typing import Iterator, List, Sequence, Union
 
 from boto3.resources.base import ResourceMeta, ServiceResource
 from boto3.resources.collection import ResourceCollection
 
 from .client import CloudFormationClient
 from .literals import (
     CapabilityType,
@@ -36,14 +36,15 @@
     ResourceStatusType,
     StackStatusType,
 )
 from .type_defs import (
     ModuleInfoResponseTypeDef,
     OutputTypeDef,
     ParameterTypeDef,
+    RollbackConfigurationOutputTypeDef,
     RollbackConfigurationTypeDef,
     StackDriftInformationResponseTypeDef,
     StackResourceDriftInformationResponseTypeDef,
     StackResourceDriftInformationSummaryResponseTypeDef,
     TagTypeDef,
     UpdateStackOutputTypeDef,
 )
@@ -447,15 +448,17 @@
         self,
         *,
         StackName: str,
         TemplateBody: str = ...,
         TemplateURL: str = ...,
         Parameters: Sequence[ParameterTypeDef] = ...,
         DisableRollback: bool = ...,
-        RollbackConfiguration: RollbackConfigurationTypeDef = ...,
+        RollbackConfiguration: Union[
+            RollbackConfigurationTypeDef, RollbackConfigurationOutputTypeDef
+        ] = ...,
         TimeoutInMinutes: int = ...,
         NotificationARNs: Sequence[str] = ...,
         Capabilities: Sequence[CapabilityType] = ...,
         ResourceTypes: Sequence[str] = ...,
         RoleARN: str = ...,
         OnFailure: OnFailureType = ...,
         StackPolicyBody: str = ...,
```

### Comparing `mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation/type_defs.py` & `mypy-boto3-cloudformation-1.28.15.post1/mypy_boto3_cloudformation/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -2834,18 +2834,18 @@
     },
     total=False,
 )
 
 RollbackConfigurationTypeDef = TypedDict(
     "RollbackConfigurationTypeDef",
     {
-        "RollbackTriggers": Sequence[RollbackTriggerTypeDef],
+        "RollbackTriggers": List[RollbackTriggerTypeDef],
         "MonitoringTimeInMinutes": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 _RequiredStackSummaryTypeDef = TypedDict(
     "_RequiredStackSummaryTypeDef",
     {
         "StackName": str,
         "CreationTime": datetime,
```

### Comparing `mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation/type_defs.pyi` & `mypy-boto3-cloudformation-1.28.15.post1/mypy_boto3_cloudformation/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -2735,18 +2735,18 @@
     },
     total=False,
 )
 
 RollbackConfigurationTypeDef = TypedDict(
     "RollbackConfigurationTypeDef",
     {
-        "RollbackTriggers": Sequence[RollbackTriggerTypeDef],
+        "RollbackTriggers": List[RollbackTriggerTypeDef],
         "MonitoringTimeInMinutes": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 _RequiredStackSummaryTypeDef = TypedDict(
     "_RequiredStackSummaryTypeDef",
     {
         "StackName": str,
         "CreationTime": datetime,
```

### Comparing `mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation/waiter.py` & `mypy-boto3-cloudformation-1.28.15.post1/mypy_boto3_cloudformation/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation/waiter.pyi` & `mypy-boto3-cloudformation-1.28.15.post1/mypy_boto3_cloudformation/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation.egg-info/PKG-INFO` & `mypy-boto3-cloudformation-1.28.15.post1/mypy_boto3_cloudformation.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudformation
-Version: 1.28.15
-Summary: Type annotations for boto3.CloudFormation 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.CloudFormation 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -47,15 +47,15 @@
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.16.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.16.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-cloudformation docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation.egg-info/SOURCES.txt` & `mypy-boto3-cloudformation-1.28.15.post1/mypy_boto3_cloudformation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudformation-1.28.15/setup.py` & `mypy-boto3-cloudformation-1.28.15.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-cloudformation",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_cloudformation"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.CloudFormation 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.1"
+        " mypy-boto3-builder 7.16.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

