# Comparing `tmp/mypy-boto3-lightsail-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-lightsail-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-lightsail-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:33 2023, max compression
+gzip compressed data, was "mypy-boto3-lightsail-1.28.16.tar", last modified: Tue Aug  1 11:37:13 2023, max compression
```

## Comparing `mypy-boto3-lightsail-1.28.15.post1.tar` & `mypy-boto3-lightsail-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:33.685251 mypy-boto3-lightsail-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:49:51.000000 mypy-boto3-lightsail-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    36694 2023-07-29 10:03:33.681251 mypy-boto3-lightsail-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    35193 2023-07-29 09:49:51.000000 mypy-boto3-lightsail-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:33.669251 mypy-boto3-lightsail-1.28.15.post1/mypy_boto3_lightsail/
--rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-07-29 09:49:51.000000 mypy-boto3-lightsail-1.28.15.post1/mypy_boto3_lightsail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-07-29 09:49:51.000000 mypy-boto3-lightsail-1.28.15.post1/mypy_boto3_lightsail/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-29 09:49:51.000000 mypy-boto3-lightsail-1.28.15.post1/mypy_boto3_lightsail/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   114230 2023-07-29 09:49:54.000000 mypy-boto3-lightsail-1.28.15.post1/mypy_boto3_lightsail/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   114044 2023-07-29 09:49:54.000000 mypy-boto3-lightsail-1.28.15.post1/mypy_boto3_lightsail/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    25315 2023-07-29 09:49:55.000000 mypy-boto3-lightsail-1.28.15.post1/mypy_boto3_lightsail/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    25313 2023-07-29 09:49:55.000000 mypy-boto3-lightsail-1.28.15.post1/mypy_boto3_lightsail/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    22961 2023-07-29 09:49:54.000000 mypy-boto3-lightsail-1.28.15.post1/mypy_boto3_lightsail/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    22938 2023-07-29 09:49:54.000000 mypy-boto3-lightsail-1.28.15.post1/mypy_boto3_lightsail/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:49:51.000000 mypy-boto3-lightsail-1.28.15.post1/mypy_boto3_lightsail/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   148016 2023-07-29 09:49:59.000000 mypy-boto3-lightsail-1.28.15.post1/mypy_boto3_lightsail/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   147917 2023-07-29 09:49:57.000000 mypy-boto3-lightsail-1.28.15.post1/mypy_boto3_lightsail/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:49:51.000000 mypy-boto3-lightsail-1.28.15.post1/mypy_boto3_lightsail/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:33.681251 mypy-boto3-lightsail-1.28.15.post1/mypy_boto3_lightsail.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    36694 2023-07-29 10:03:33.000000 mypy-boto3-lightsail-1.28.15.post1/mypy_boto3_lightsail.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-29 10:03:33.000000 mypy-boto3-lightsail-1.28.15.post1/mypy_boto3_lightsail.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:33.000000 mypy-boto3-lightsail-1.28.15.post1/mypy_boto3_lightsail.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:33.000000 mypy-boto3-lightsail-1.28.15.post1/mypy_boto3_lightsail.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:33.000000 mypy-boto3-lightsail-1.28.15.post1/mypy_boto3_lightsail.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-29 10:03:33.000000 mypy-boto3-lightsail-1.28.15.post1/mypy_boto3_lightsail.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:33.685251 mypy-boto3-lightsail-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-29 09:49:51.000000 mypy-boto3-lightsail-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:13.576837 mypy-boto3-lightsail-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:22:44.000000 mypy-boto3-lightsail-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    36793 2023-08-01 11:37:13.576837 mypy-boto3-lightsail-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    35301 2023-08-01 11:22:44.000000 mypy-boto3-lightsail-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:13.572837 mypy-boto3-lightsail-1.28.16/mypy_boto3_lightsail/
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-08-01 11:22:44.000000 mypy-boto3-lightsail-1.28.16/mypy_boto3_lightsail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-08-01 11:22:44.000000 mypy-boto3-lightsail-1.28.16/mypy_boto3_lightsail/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-08-01 11:22:44.000000 mypy-boto3-lightsail-1.28.16/mypy_boto3_lightsail/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   113894 2023-08-01 11:22:45.000000 mypy-boto3-lightsail-1.28.16/mypy_boto3_lightsail/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   113708 2023-08-01 11:22:44.000000 mypy-boto3-lightsail-1.28.16/mypy_boto3_lightsail/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    25315 2023-08-01 11:22:45.000000 mypy-boto3-lightsail-1.28.16/mypy_boto3_lightsail/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25313 2023-08-01 11:22:45.000000 mypy-boto3-lightsail-1.28.16/mypy_boto3_lightsail/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    22961 2023-08-01 11:22:45.000000 mypy-boto3-lightsail-1.28.16/mypy_boto3_lightsail/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22938 2023-08-01 11:22:45.000000 mypy-boto3-lightsail-1.28.16/mypy_boto3_lightsail/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:22:44.000000 mypy-boto3-lightsail-1.28.16/mypy_boto3_lightsail/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   148303 2023-08-01 11:22:52.000000 mypy-boto3-lightsail-1.28.16/mypy_boto3_lightsail/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   148204 2023-08-01 11:22:47.000000 mypy-boto3-lightsail-1.28.16/mypy_boto3_lightsail/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:22:44.000000 mypy-boto3-lightsail-1.28.16/mypy_boto3_lightsail/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:13.576837 mypy-boto3-lightsail-1.28.16/mypy_boto3_lightsail.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    36793 2023-08-01 11:37:13.000000 mypy-boto3-lightsail-1.28.16/mypy_boto3_lightsail.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-08-01 11:37:13.000000 mypy-boto3-lightsail-1.28.16/mypy_boto3_lightsail.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:13.000000 mypy-boto3-lightsail-1.28.16/mypy_boto3_lightsail.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:13.000000 mypy-boto3-lightsail-1.28.16/mypy_boto3_lightsail.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:13.000000 mypy-boto3-lightsail-1.28.16/mypy_boto3_lightsail.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-01 11:37:13.000000 mypy-boto3-lightsail-1.28.16/mypy_boto3_lightsail.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:13.576837 mypy-boto3-lightsail-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-08-01 11:22:43.000000 mypy-boto3-lightsail-1.28.16/setup.py
```

### Comparing `mypy-boto3-lightsail-1.28.15.post1/LICENSE` & `mypy-boto3-lightsail-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lightsail-1.28.15.post1/PKG-INFO` & `mypy-boto3-lightsail-1.28.16/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lightsail
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Lightsail 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.Lightsail 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 lightsail type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 lightsail type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lightsail.svg?color=blue)](https://pypi.org/project/mypy-boto3-lightsail)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lightsail)](https://pepy.tech/project/mypy-boto3-lightsail)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Lightsail 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail)
+[boto3.Lightsail 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail)
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
 [mypy-boto3-lightsail docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/).
 
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
@@ -464,20 +464,20 @@
 )
 
 
 def check_value(value: AccessDirectionType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_lightsail.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_lightsail.type_defs import (
     AccessKeyLastUsedTypeDef,
     AccessRulesTypeDef,
     AccountLevelBpaSyncTypeDef,
     AutoSnapshotAddOnRequestTypeDef,
@@ -527,14 +527,15 @@
     InstanceEntryTypeDef,
     CreateContactMethodRequestRequestTypeDef,
     InputOriginTypeDef,
     DomainEntryTypeDef,
     CreateGUISessionAccessDetailsRequestRequestTypeDef,
     SessionTypeDef,
     DiskMapTypeDef,
+    TimestampTypeDef,
     DeleteAlarmRequestRequestTypeDef,
     DeleteAutoSnapshotRequestRequestTypeDef,
     DeleteBucketAccessKeyRequestRequestTypeDef,
     DeleteBucketRequestRequestTypeDef,
     DeleteCertificateRequestRequestTypeDef,
     DeleteContactMethodRequestRequestTypeDef,
     DeleteContainerImageRequestRequestTypeDef,
@@ -567,50 +568,43 @@
     PaginatorConfigTypeDef,
     GetActiveNamesRequestRequestTypeDef,
     GetAlarmsRequestRequestTypeDef,
     GetAutoSnapshotsRequestRequestTypeDef,
     GetBlueprintsRequestRequestTypeDef,
     GetBucketAccessKeysRequestRequestTypeDef,
     GetBucketBundlesRequestRequestTypeDef,
-    GetBucketMetricDataRequestRequestTypeDef,
     MetricDatapointTypeDef,
     GetBucketsRequestRequestTypeDef,
     GetBundlesRequestRequestTypeDef,
     GetCertificatesRequestRequestTypeDef,
     GetCloudFormationStackRecordsRequestRequestTypeDef,
     GetContactMethodsRequestRequestTypeDef,
     GetContainerImagesRequestRequestTypeDef,
-    GetContainerLogRequestRequestTypeDef,
     GetContainerServiceDeploymentsRequestRequestTypeDef,
-    GetContainerServiceMetricDataRequestRequestTypeDef,
     GetContainerServicesRequestRequestTypeDef,
-    GetCostEstimateRequestRequestTypeDef,
     GetDiskRequestRequestTypeDef,
     GetDiskSnapshotRequestRequestTypeDef,
     GetDiskSnapshotsRequestRequestTypeDef,
     GetDisksRequestRequestTypeDef,
     GetDistributionLatestCacheResetRequestRequestTypeDef,
-    GetDistributionMetricDataRequestRequestTypeDef,
     GetDistributionsRequestRequestTypeDef,
     GetDomainRequestRequestTypeDef,
     GetDomainsRequestRequestTypeDef,
     GetExportSnapshotRecordsRequestRequestTypeDef,
     GetInstanceAccessDetailsRequestRequestTypeDef,
-    GetInstanceMetricDataRequestRequestTypeDef,
     GetInstancePortStatesRequestRequestTypeDef,
     InstancePortStateTypeDef,
     GetInstanceRequestRequestTypeDef,
     GetInstanceSnapshotRequestRequestTypeDef,
     GetInstanceSnapshotsRequestRequestTypeDef,
     GetInstanceStateRequestRequestTypeDef,
     InstanceStateTypeDef,
     GetInstancesRequestRequestTypeDef,
     GetKeyPairRequestRequestTypeDef,
     GetKeyPairsRequestRequestTypeDef,
-    GetLoadBalancerMetricDataRequestRequestTypeDef,
     GetLoadBalancerRequestRequestTypeDef,
     GetLoadBalancerTlsCertificatesRequestRequestTypeDef,
     GetLoadBalancerTlsPoliciesRequestRequestTypeDef,
     LoadBalancerTlsPolicyTypeDef,
     GetLoadBalancersRequestRequestTypeDef,
     GetOperationRequestRequestTypeDef,
     GetOperationsForResourceRequestRequestTypeDef,
@@ -618,19 +612,17 @@
     GetRegionsRequestRequestTypeDef,
     GetRelationalDatabaseBlueprintsRequestRequestTypeDef,
     RelationalDatabaseBlueprintTypeDef,
     GetRelationalDatabaseBundlesRequestRequestTypeDef,
     RelationalDatabaseBundleTypeDef,
     GetRelationalDatabaseEventsRequestRequestTypeDef,
     RelationalDatabaseEventTypeDef,
-    GetRelationalDatabaseLogEventsRequestRequestTypeDef,
     LogEventTypeDef,
     GetRelationalDatabaseLogStreamsRequestRequestTypeDef,
     GetRelationalDatabaseMasterUserPasswordRequestRequestTypeDef,
-    GetRelationalDatabaseMetricDataRequestRequestTypeDef,
     GetRelationalDatabaseParametersRequestRequestTypeDef,
     RelationalDatabaseParameterTypeDef,
     GetRelationalDatabaseRequestRequestTypeDef,
     GetRelationalDatabaseSnapshotRequestRequestTypeDef,
     GetRelationalDatabaseSnapshotsRequestRequestTypeDef,
     GetRelationalDatabasesRequestRequestTypeDef,
     GetStaticIpRequestRequestTypeDef,
@@ -697,15 +689,14 @@
     CreateCertificateRequestRequestTypeDef,
     CreateDiskSnapshotRequestRequestTypeDef,
     CreateDomainRequestRequestTypeDef,
     CreateInstanceSnapshotRequestRequestTypeDef,
     CreateKeyPairRequestRequestTypeDef,
     CreateLoadBalancerRequestRequestTypeDef,
     CreateLoadBalancerTlsCertificateRequestRequestTypeDef,
-    CreateRelationalDatabaseFromSnapshotRequestRequestTypeDef,
     CreateRelationalDatabaseRequestRequestTypeDef,
     CreateRelationalDatabaseSnapshotRequestRequestTypeDef,
     DiskSnapshotTypeDef,
     DiskTypeDef,
     KeyPairTypeDef,
     RelationalDatabaseSnapshotTypeDef,
     TagResourceRequestRequestTypeDef,
@@ -714,28 +705,40 @@
     CacheSettingsTypeDef,
     CloseInstancePublicPortsRequestRequestTypeDef,
     OpenInstancePublicPortsRequestRequestTypeDef,
     PutInstancePublicPortsRequestRequestTypeDef,
     CloudFormationStackRecordTypeDef,
     GetContainerImagesResultTypeDef,
     RegisterContainerImageResultTypeDef,
+    ContainerUnionTypeDef,
     PrivateRegistryAccessRequestTypeDef,
     PrivateRegistryAccessTypeDef,
     ContainerServiceEndpointTypeDef,
     EndpointRequestTypeDef,
     GetContainerLogResultTypeDef,
     GetContainerServicePowersResultTypeDef,
     CreateContainerServiceRegistryLoginResultTypeDef,
     CreateCloudFormationStackRequestRequestTypeDef,
     CreateDomainEntryRequestRequestTypeDef,
     DeleteDomainEntryRequestRequestTypeDef,
     UpdateDomainEntryRequestRequestTypeDef,
     CreateGUISessionAccessDetailsResultTypeDef,
+    CreateRelationalDatabaseFromSnapshotRequestRequestTypeDef,
+    GetBucketMetricDataRequestRequestTypeDef,
+    GetContainerLogRequestRequestTypeDef,
+    GetContainerServiceMetricDataRequestRequestTypeDef,
+    GetCostEstimateRequestRequestTypeDef,
+    GetDistributionMetricDataRequestRequestTypeDef,
+    GetInstanceMetricDataRequestRequestTypeDef,
+    GetLoadBalancerMetricDataRequestRequestTypeDef,
+    GetRelationalDatabaseLogEventsRequestRequestTypeDef,
+    GetRelationalDatabaseMetricDataRequestRequestTypeDef,
     InstanceSnapshotInfoTypeDef,
     GetDistributionBundlesResultTypeDef,
+    DomainEntryUnionTypeDef,
     DomainValidationRecordTypeDef,
     EstimateByTimeTypeDef,
     GetActiveNamesRequestGetActiveNamesPaginateTypeDef,
     GetBlueprintsRequestGetBlueprintsPaginateTypeDef,
     GetBundlesRequestGetBundlesPaginateTypeDef,
     GetCloudFormationStackRecordsRequestGetCloudFormationStackRecordsPaginateTypeDef,
     GetDiskSnapshotsRequestGetDiskSnapshotsPaginateTypeDef,
@@ -882,14 +885,15 @@
     InstanceSnapshotTypeDef,
     CreateKeyPairResultTypeDef,
     GetKeyPairResultTypeDef,
     GetKeyPairsResultTypeDef,
     GetRelationalDatabaseSnapshotResultTypeDef,
     GetRelationalDatabaseSnapshotsResultTypeDef,
     LightsailDistributionTypeDef,
+    CacheSettingsUnionTypeDef,
     CreateDistributionRequestRequestTypeDef,
     UpdateDistributionRequestRequestTypeDef,
     GetCloudFormationStackRecordsResultTypeDef,
     UpdateContainerServiceRequestRequestTypeDef,
     ContainerServiceDeploymentTypeDef,
     ContainerServiceDeploymentRequestTypeDef,
     CreateContainerServiceDeploymentRequestRequestTypeDef,
@@ -927,15 +931,15 @@
     CertificateSummaryTypeDef,
     GetCostEstimateResultTypeDef,
     CreateCertificateResultTypeDef,
     GetCertificatesResultTypeDef,
 )
 
 
-def get_structure() -> AccessKeyLastUsedTypeDef:
+def get_value() -> AccessKeyLastUsedTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-lightsail-1.28.15.post1/README.md` & `mypy-boto3-lightsail-1.28.16/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lightsail.svg?color=blue)](https://pypi.org/project/mypy-boto3-lightsail)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lightsail)](https://pepy.tech/project/mypy-boto3-lightsail)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Lightsail 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail)
+[boto3.Lightsail 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail)
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
 [mypy-boto3-lightsail docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/).
 
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
@@ -432,20 +432,20 @@
 )
 
 
 def check_value(value: AccessDirectionType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_lightsail.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_lightsail.type_defs import (
     AccessKeyLastUsedTypeDef,
     AccessRulesTypeDef,
     AccountLevelBpaSyncTypeDef,
     AutoSnapshotAddOnRequestTypeDef,
@@ -495,14 +495,15 @@
     InstanceEntryTypeDef,
     CreateContactMethodRequestRequestTypeDef,
     InputOriginTypeDef,
     DomainEntryTypeDef,
     CreateGUISessionAccessDetailsRequestRequestTypeDef,
     SessionTypeDef,
     DiskMapTypeDef,
+    TimestampTypeDef,
     DeleteAlarmRequestRequestTypeDef,
     DeleteAutoSnapshotRequestRequestTypeDef,
     DeleteBucketAccessKeyRequestRequestTypeDef,
     DeleteBucketRequestRequestTypeDef,
     DeleteCertificateRequestRequestTypeDef,
     DeleteContactMethodRequestRequestTypeDef,
     DeleteContainerImageRequestRequestTypeDef,
@@ -535,50 +536,43 @@
     PaginatorConfigTypeDef,
     GetActiveNamesRequestRequestTypeDef,
     GetAlarmsRequestRequestTypeDef,
     GetAutoSnapshotsRequestRequestTypeDef,
     GetBlueprintsRequestRequestTypeDef,
     GetBucketAccessKeysRequestRequestTypeDef,
     GetBucketBundlesRequestRequestTypeDef,
-    GetBucketMetricDataRequestRequestTypeDef,
     MetricDatapointTypeDef,
     GetBucketsRequestRequestTypeDef,
     GetBundlesRequestRequestTypeDef,
     GetCertificatesRequestRequestTypeDef,
     GetCloudFormationStackRecordsRequestRequestTypeDef,
     GetContactMethodsRequestRequestTypeDef,
     GetContainerImagesRequestRequestTypeDef,
-    GetContainerLogRequestRequestTypeDef,
     GetContainerServiceDeploymentsRequestRequestTypeDef,
-    GetContainerServiceMetricDataRequestRequestTypeDef,
     GetContainerServicesRequestRequestTypeDef,
-    GetCostEstimateRequestRequestTypeDef,
     GetDiskRequestRequestTypeDef,
     GetDiskSnapshotRequestRequestTypeDef,
     GetDiskSnapshotsRequestRequestTypeDef,
     GetDisksRequestRequestTypeDef,
     GetDistributionLatestCacheResetRequestRequestTypeDef,
-    GetDistributionMetricDataRequestRequestTypeDef,
     GetDistributionsRequestRequestTypeDef,
     GetDomainRequestRequestTypeDef,
     GetDomainsRequestRequestTypeDef,
     GetExportSnapshotRecordsRequestRequestTypeDef,
     GetInstanceAccessDetailsRequestRequestTypeDef,
-    GetInstanceMetricDataRequestRequestTypeDef,
     GetInstancePortStatesRequestRequestTypeDef,
     InstancePortStateTypeDef,
     GetInstanceRequestRequestTypeDef,
     GetInstanceSnapshotRequestRequestTypeDef,
     GetInstanceSnapshotsRequestRequestTypeDef,
     GetInstanceStateRequestRequestTypeDef,
     InstanceStateTypeDef,
     GetInstancesRequestRequestTypeDef,
     GetKeyPairRequestRequestTypeDef,
     GetKeyPairsRequestRequestTypeDef,
-    GetLoadBalancerMetricDataRequestRequestTypeDef,
     GetLoadBalancerRequestRequestTypeDef,
     GetLoadBalancerTlsCertificatesRequestRequestTypeDef,
     GetLoadBalancerTlsPoliciesRequestRequestTypeDef,
     LoadBalancerTlsPolicyTypeDef,
     GetLoadBalancersRequestRequestTypeDef,
     GetOperationRequestRequestTypeDef,
     GetOperationsForResourceRequestRequestTypeDef,
@@ -586,19 +580,17 @@
     GetRegionsRequestRequestTypeDef,
     GetRelationalDatabaseBlueprintsRequestRequestTypeDef,
     RelationalDatabaseBlueprintTypeDef,
     GetRelationalDatabaseBundlesRequestRequestTypeDef,
     RelationalDatabaseBundleTypeDef,
     GetRelationalDatabaseEventsRequestRequestTypeDef,
     RelationalDatabaseEventTypeDef,
-    GetRelationalDatabaseLogEventsRequestRequestTypeDef,
     LogEventTypeDef,
     GetRelationalDatabaseLogStreamsRequestRequestTypeDef,
     GetRelationalDatabaseMasterUserPasswordRequestRequestTypeDef,
-    GetRelationalDatabaseMetricDataRequestRequestTypeDef,
     GetRelationalDatabaseParametersRequestRequestTypeDef,
     RelationalDatabaseParameterTypeDef,
     GetRelationalDatabaseRequestRequestTypeDef,
     GetRelationalDatabaseSnapshotRequestRequestTypeDef,
     GetRelationalDatabaseSnapshotsRequestRequestTypeDef,
     GetRelationalDatabasesRequestRequestTypeDef,
     GetStaticIpRequestRequestTypeDef,
@@ -665,15 +657,14 @@
     CreateCertificateRequestRequestTypeDef,
     CreateDiskSnapshotRequestRequestTypeDef,
     CreateDomainRequestRequestTypeDef,
     CreateInstanceSnapshotRequestRequestTypeDef,
     CreateKeyPairRequestRequestTypeDef,
     CreateLoadBalancerRequestRequestTypeDef,
     CreateLoadBalancerTlsCertificateRequestRequestTypeDef,
-    CreateRelationalDatabaseFromSnapshotRequestRequestTypeDef,
     CreateRelationalDatabaseRequestRequestTypeDef,
     CreateRelationalDatabaseSnapshotRequestRequestTypeDef,
     DiskSnapshotTypeDef,
     DiskTypeDef,
     KeyPairTypeDef,
     RelationalDatabaseSnapshotTypeDef,
     TagResourceRequestRequestTypeDef,
@@ -682,28 +673,40 @@
     CacheSettingsTypeDef,
     CloseInstancePublicPortsRequestRequestTypeDef,
     OpenInstancePublicPortsRequestRequestTypeDef,
     PutInstancePublicPortsRequestRequestTypeDef,
     CloudFormationStackRecordTypeDef,
     GetContainerImagesResultTypeDef,
     RegisterContainerImageResultTypeDef,
+    ContainerUnionTypeDef,
     PrivateRegistryAccessRequestTypeDef,
     PrivateRegistryAccessTypeDef,
     ContainerServiceEndpointTypeDef,
     EndpointRequestTypeDef,
     GetContainerLogResultTypeDef,
     GetContainerServicePowersResultTypeDef,
     CreateContainerServiceRegistryLoginResultTypeDef,
     CreateCloudFormationStackRequestRequestTypeDef,
     CreateDomainEntryRequestRequestTypeDef,
     DeleteDomainEntryRequestRequestTypeDef,
     UpdateDomainEntryRequestRequestTypeDef,
     CreateGUISessionAccessDetailsResultTypeDef,
+    CreateRelationalDatabaseFromSnapshotRequestRequestTypeDef,
+    GetBucketMetricDataRequestRequestTypeDef,
+    GetContainerLogRequestRequestTypeDef,
+    GetContainerServiceMetricDataRequestRequestTypeDef,
+    GetCostEstimateRequestRequestTypeDef,
+    GetDistributionMetricDataRequestRequestTypeDef,
+    GetInstanceMetricDataRequestRequestTypeDef,
+    GetLoadBalancerMetricDataRequestRequestTypeDef,
+    GetRelationalDatabaseLogEventsRequestRequestTypeDef,
+    GetRelationalDatabaseMetricDataRequestRequestTypeDef,
     InstanceSnapshotInfoTypeDef,
     GetDistributionBundlesResultTypeDef,
+    DomainEntryUnionTypeDef,
     DomainValidationRecordTypeDef,
     EstimateByTimeTypeDef,
     GetActiveNamesRequestGetActiveNamesPaginateTypeDef,
     GetBlueprintsRequestGetBlueprintsPaginateTypeDef,
     GetBundlesRequestGetBundlesPaginateTypeDef,
     GetCloudFormationStackRecordsRequestGetCloudFormationStackRecordsPaginateTypeDef,
     GetDiskSnapshotsRequestGetDiskSnapshotsPaginateTypeDef,
@@ -850,14 +853,15 @@
     InstanceSnapshotTypeDef,
     CreateKeyPairResultTypeDef,
     GetKeyPairResultTypeDef,
     GetKeyPairsResultTypeDef,
     GetRelationalDatabaseSnapshotResultTypeDef,
     GetRelationalDatabaseSnapshotsResultTypeDef,
     LightsailDistributionTypeDef,
+    CacheSettingsUnionTypeDef,
     CreateDistributionRequestRequestTypeDef,
     UpdateDistributionRequestRequestTypeDef,
     GetCloudFormationStackRecordsResultTypeDef,
     UpdateContainerServiceRequestRequestTypeDef,
     ContainerServiceDeploymentTypeDef,
     ContainerServiceDeploymentRequestTypeDef,
     CreateContainerServiceDeploymentRequestRequestTypeDef,
@@ -895,15 +899,15 @@
     CertificateSummaryTypeDef,
     GetCostEstimateResultTypeDef,
     CreateCertificateResultTypeDef,
     GetCertificatesResultTypeDef,
 )
 
 
-def get_structure() -> AccessKeyLastUsedTypeDef:
+def get_value() -> AccessKeyLastUsedTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-lightsail-1.28.15.post1/mypy_boto3_lightsail/__init__.py` & `mypy-boto3-lightsail-1.28.16/mypy_boto3_lightsail/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lightsail-1.28.15.post1/mypy_boto3_lightsail/__init__.pyi` & `mypy-boto3-lightsail-1.28.16/mypy_boto3_lightsail/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lightsail-1.28.15.post1/mypy_boto3_lightsail/__main__.py` & `mypy-boto3-lightsail-1.28.16/mypy_boto3_lightsail/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Lightsail 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.Lightsail 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail\nOther"
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

### Comparing `mypy-boto3-lightsail-1.28.15.post1/mypy_boto3_lightsail/client.py` & `mypy-boto3-lightsail-1.28.16/mypy_boto3_lightsail/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_lightsail.client import LightsailClient
 
     session = Session()
     client: LightsailClient = session.client("lightsail")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AddOnTypeType,
     AlarmStateType,
     BucketMetricNameType,
@@ -77,21 +76,19 @@
     AttachDiskResultTypeDef,
     AttachInstancesToLoadBalancerResultTypeDef,
     AttachLoadBalancerTlsCertificateResultTypeDef,
     AttachStaticIpResultTypeDef,
     BucketAccessLogConfigTypeDef,
     CacheBehaviorPerPathTypeDef,
     CacheBehaviorTypeDef,
-    CacheSettingsOutputTypeDef,
-    CacheSettingsTypeDef,
+    CacheSettingsUnionTypeDef,
     CloseInstancePublicPortsResultTypeDef,
-    ContainerOutputTypeDef,
     ContainerServiceDeploymentRequestTypeDef,
     ContainerServicesListResultTypeDef,
-    ContainerTypeDef,
+    ContainerUnionTypeDef,
     CopySnapshotResultTypeDef,
     CreateBucketAccessKeyResultTypeDef,
     CreateBucketResultTypeDef,
     CreateCertificateResultTypeDef,
     CreateCloudFormationStackResultTypeDef,
     CreateContactMethodResultTypeDef,
     CreateContainerServiceDeploymentResultTypeDef,
@@ -134,16 +131,15 @@
     DeleteRelationalDatabaseSnapshotResultTypeDef,
     DetachCertificateFromDistributionResultTypeDef,
     DetachDiskResultTypeDef,
     DetachInstancesFromLoadBalancerResultTypeDef,
     DetachStaticIpResultTypeDef,
     DisableAddOnResultTypeDef,
     DiskMapTypeDef,
-    DomainEntryOutputTypeDef,
-    DomainEntryTypeDef,
+    DomainEntryUnionTypeDef,
     DownloadDefaultKeyPairResultTypeDef,
     EnableAddOnResultTypeDef,
     EndpointRequestTypeDef,
     ExportSnapshotResultTypeDef,
     GetActiveNamesResultTypeDef,
     GetAlarmsResultTypeDef,
     GetAutoSnapshotsResultTypeDef,
@@ -231,14 +227,15 @@
     StartRelationalDatabaseResultTypeDef,
     StopGUISessionResultTypeDef,
     StopInstanceResultTypeDef,
     StopRelationalDatabaseResultTypeDef,
     TagResourceResultTypeDef,
     TagTypeDef,
     TestAlarmResultTypeDef,
+    TimestampTypeDef,
     UnpeerVpcResultTypeDef,
     UntagResourceResultTypeDef,
     UpdateBucketBundleResultTypeDef,
     UpdateBucketResultTypeDef,
     UpdateContainerServiceResultTypeDef,
     UpdateDistributionBundleResultTypeDef,
     UpdateDistributionResultTypeDef,
@@ -476,15 +473,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#create_container_service)
         """
 
     def create_container_service_deployment(
         self,
         *,
         serviceName: str,
-        containers: Mapping[str, Union[ContainerTypeDef, ContainerOutputTypeDef]] = ...,
+        containers: Mapping[str, ContainerUnionTypeDef] = ...,
         publicEndpoint: EndpointRequestTypeDef = ...
     ) -> CreateContainerServiceDeploymentResultTypeDef:
         """
         Creates a deployment for your Amazon Lightsail container service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.create_container_service_deployment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#create_container_service_deployment)
@@ -556,15 +553,15 @@
     def create_distribution(
         self,
         *,
         distributionName: str,
         origin: InputOriginTypeDef,
         defaultCacheBehavior: CacheBehaviorTypeDef,
         bundleId: str,
-        cacheBehaviorSettings: Union[CacheSettingsTypeDef, CacheSettingsOutputTypeDef] = ...,
+        cacheBehaviorSettings: CacheSettingsUnionTypeDef = ...,
         cacheBehaviors: Sequence[CacheBehaviorPerPathTypeDef] = ...,
         ipAddressType: IpAddressTypeType = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateDistributionResultTypeDef:
         """
         Creates an Amazon Lightsail content delivery network (CDN) distribution.
 
@@ -579,15 +576,15 @@
         Creates a domain resource for the specified domain (e.g., example.com).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.create_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#create_domain)
         """
 
     def create_domain_entry(
-        self, *, domainName: str, domainEntry: Union[DomainEntryTypeDef, DomainEntryOutputTypeDef]
+        self, *, domainName: str, domainEntry: DomainEntryUnionTypeDef
     ) -> CreateDomainEntryResultTypeDef:
         """
         Creates one of the following domain name system (DNS) records in a domain DNS
         zone: Address (A), canonical name (CNAME), mail exchanger (MX), name server
         (NS), start of authority (SOA), service locator (SRV), or text (TXT).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.create_domain_entry)
@@ -735,15 +732,15 @@
         *,
         relationalDatabaseName: str,
         availabilityZone: str = ...,
         publiclyAccessible: bool = ...,
         relationalDatabaseSnapshotName: str = ...,
         relationalDatabaseBundleId: str = ...,
         sourceRelationalDatabaseName: str = ...,
-        restoreTime: Union[datetime, str] = ...,
+        restoreTime: TimestampTypeDef = ...,
         useLatestRestorableTime: bool = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateRelationalDatabaseFromSnapshotResultTypeDef:
         """
         Creates a new database from an existing database snapshot in Amazon Lightsail.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.create_relational_database_from_snapshot)
@@ -871,15 +868,15 @@
         Deletes the specified domain recordset and all of its domain records.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.delete_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#delete_domain)
         """
 
     def delete_domain_entry(
-        self, *, domainName: str, domainEntry: Union[DomainEntryTypeDef, DomainEntryOutputTypeDef]
+        self, *, domainName: str, domainEntry: DomainEntryUnionTypeDef
     ) -> DeleteDomainEntryResultTypeDef:
         """
         Deletes a specific domain entry.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.delete_domain_entry)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#delete_domain_entry)
         """
@@ -1110,16 +1107,16 @@
         """
 
     def get_bucket_metric_data(
         self,
         *,
         bucketName: str,
         metricName: BucketMetricNameType,
-        startTime: Union[datetime, str],
-        endTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
+        endTime: TimestampTypeDef,
         period: int,
         statistics: Sequence[MetricStatisticType],
         unit: MetricUnitType
     ) -> GetBucketMetricDataResultTypeDef:
         """
         Returns the data points of a specific metric for an Amazon Lightsail bucket.
 
@@ -1207,16 +1204,16 @@
         """
 
     def get_container_log(
         self,
         *,
         serviceName: str,
         containerName: str,
-        startTime: Union[datetime, str] = ...,
-        endTime: Union[datetime, str] = ...,
+        startTime: TimestampTypeDef = ...,
+        endTime: TimestampTypeDef = ...,
         filterPattern: str = ...,
         pageToken: str = ...
     ) -> GetContainerLogResultTypeDef:
         """
         Returns the log events of a container of your Amazon Lightsail container
         service.
 
@@ -1237,16 +1234,16 @@
         """
 
     def get_container_service_metric_data(
         self,
         *,
         serviceName: str,
         metricName: ContainerServiceMetricNameType,
-        startTime: Union[datetime, str],
-        endTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
+        endTime: TimestampTypeDef,
         period: int,
         statistics: Sequence[MetricStatisticType]
     ) -> GetContainerServiceMetricDataResultTypeDef:
         """
         Returns the data points of a specific metric of your Amazon Lightsail container
         service.
 
@@ -1271,15 +1268,15 @@
         services.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.get_container_services)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#get_container_services)
         """
 
     def get_cost_estimate(
-        self, *, resourceName: str, startTime: Union[datetime, str], endTime: Union[datetime, str]
+        self, *, resourceName: str, startTime: TimestampTypeDef, endTime: TimestampTypeDef
     ) -> GetCostEstimateResultTypeDef:
         """
         Retrieves information about the cost estimate for a specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.get_cost_estimate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#get_cost_estimate)
         """
@@ -1339,16 +1336,16 @@
         """
 
     def get_distribution_metric_data(
         self,
         *,
         distributionName: str,
         metricName: DistributionMetricNameType,
-        startTime: Union[datetime, str],
-        endTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
+        endTime: TimestampTypeDef,
         period: int,
         unit: MetricUnitType,
         statistics: Sequence[MetricStatisticType]
     ) -> GetDistributionMetricDataResultTypeDef:
         """
         Returns the data points of a specific metric for an Amazon Lightsail content
         delivery network (CDN) distribution.
@@ -1417,16 +1414,16 @@
 
     def get_instance_metric_data(
         self,
         *,
         instanceName: str,
         metricName: InstanceMetricNameType,
         period: int,
-        startTime: Union[datetime, str],
-        endTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
+        endTime: TimestampTypeDef,
         unit: MetricUnitType,
         statistics: Sequence[MetricStatisticType]
     ) -> GetInstanceMetricDataResultTypeDef:
         """
         Returns the data points for the specified Amazon Lightsail instance metric,
         given an instance name.
 
@@ -1507,16 +1504,16 @@
 
     def get_load_balancer_metric_data(
         self,
         *,
         loadBalancerName: str,
         metricName: LoadBalancerMetricNameType,
         period: int,
-        startTime: Union[datetime, str],
-        endTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
+        endTime: TimestampTypeDef,
         unit: MetricUnitType,
         statistics: Sequence[MetricStatisticType]
     ) -> GetLoadBalancerMetricDataResultTypeDef:
         """
         Returns information about health metrics for your Lightsail load balancer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.get_load_balancer_metric_data)
@@ -1633,16 +1630,16 @@
         """
 
     def get_relational_database_log_events(
         self,
         *,
         relationalDatabaseName: str,
         logStreamName: str,
-        startTime: Union[datetime, str] = ...,
-        endTime: Union[datetime, str] = ...,
+        startTime: TimestampTypeDef = ...,
+        endTime: TimestampTypeDef = ...,
         startFromHead: bool = ...,
         pageToken: str = ...
     ) -> GetRelationalDatabaseLogEventsResultTypeDef:
         """
         Returns a list of log events for a database in Amazon Lightsail.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.get_relational_database_log_events)
@@ -1676,16 +1673,16 @@
 
     def get_relational_database_metric_data(
         self,
         *,
         relationalDatabaseName: str,
         metricName: RelationalDatabaseMetricNameType,
         period: int,
-        startTime: Union[datetime, str],
-        endTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
+        endTime: TimestampTypeDef,
         unit: MetricUnitType,
         statistics: Sequence[MetricStatisticType]
     ) -> GetRelationalDatabaseMetricDataResultTypeDef:
         """
         Returns the data points of the specified metric for a database in Amazon
         Lightsail.
 
@@ -2038,15 +2035,15 @@
 
     def update_distribution(
         self,
         *,
         distributionName: str,
         origin: InputOriginTypeDef = ...,
         defaultCacheBehavior: CacheBehaviorTypeDef = ...,
-        cacheBehaviorSettings: Union[CacheSettingsTypeDef, CacheSettingsOutputTypeDef] = ...,
+        cacheBehaviorSettings: CacheSettingsUnionTypeDef = ...,
         cacheBehaviors: Sequence[CacheBehaviorPerPathTypeDef] = ...,
         isEnabled: bool = ...
     ) -> UpdateDistributionResultTypeDef:
         """
         Updates an existing Amazon Lightsail content delivery network (CDN)
         distribution.
 
@@ -2062,15 +2059,15 @@
         distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.update_distribution_bundle)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#update_distribution_bundle)
         """
 
     def update_domain_entry(
-        self, *, domainName: str, domainEntry: Union[DomainEntryTypeDef, DomainEntryOutputTypeDef]
+        self, *, domainName: str, domainEntry: DomainEntryUnionTypeDef
     ) -> UpdateDomainEntryResultTypeDef:
         """
         Updates a domain recordset after it is created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.update_domain_entry)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#update_domain_entry)
         """
```

### Comparing `mypy-boto3-lightsail-1.28.15.post1/mypy_boto3_lightsail/client.pyi` & `mypy-boto3-lightsail-1.28.16/mypy_boto3_lightsail/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_lightsail.client import LightsailClient
 
     session = Session()
     client: LightsailClient = session.client("lightsail")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AddOnTypeType,
     AlarmStateType,
     BucketMetricNameType,
@@ -77,21 +76,19 @@
     AttachDiskResultTypeDef,
     AttachInstancesToLoadBalancerResultTypeDef,
     AttachLoadBalancerTlsCertificateResultTypeDef,
     AttachStaticIpResultTypeDef,
     BucketAccessLogConfigTypeDef,
     CacheBehaviorPerPathTypeDef,
     CacheBehaviorTypeDef,
-    CacheSettingsOutputTypeDef,
-    CacheSettingsTypeDef,
+    CacheSettingsUnionTypeDef,
     CloseInstancePublicPortsResultTypeDef,
-    ContainerOutputTypeDef,
     ContainerServiceDeploymentRequestTypeDef,
     ContainerServicesListResultTypeDef,
-    ContainerTypeDef,
+    ContainerUnionTypeDef,
     CopySnapshotResultTypeDef,
     CreateBucketAccessKeyResultTypeDef,
     CreateBucketResultTypeDef,
     CreateCertificateResultTypeDef,
     CreateCloudFormationStackResultTypeDef,
     CreateContactMethodResultTypeDef,
     CreateContainerServiceDeploymentResultTypeDef,
@@ -134,16 +131,15 @@
     DeleteRelationalDatabaseSnapshotResultTypeDef,
     DetachCertificateFromDistributionResultTypeDef,
     DetachDiskResultTypeDef,
     DetachInstancesFromLoadBalancerResultTypeDef,
     DetachStaticIpResultTypeDef,
     DisableAddOnResultTypeDef,
     DiskMapTypeDef,
-    DomainEntryOutputTypeDef,
-    DomainEntryTypeDef,
+    DomainEntryUnionTypeDef,
     DownloadDefaultKeyPairResultTypeDef,
     EnableAddOnResultTypeDef,
     EndpointRequestTypeDef,
     ExportSnapshotResultTypeDef,
     GetActiveNamesResultTypeDef,
     GetAlarmsResultTypeDef,
     GetAutoSnapshotsResultTypeDef,
@@ -231,14 +227,15 @@
     StartRelationalDatabaseResultTypeDef,
     StopGUISessionResultTypeDef,
     StopInstanceResultTypeDef,
     StopRelationalDatabaseResultTypeDef,
     TagResourceResultTypeDef,
     TagTypeDef,
     TestAlarmResultTypeDef,
+    TimestampTypeDef,
     UnpeerVpcResultTypeDef,
     UntagResourceResultTypeDef,
     UpdateBucketBundleResultTypeDef,
     UpdateBucketResultTypeDef,
     UpdateContainerServiceResultTypeDef,
     UpdateDistributionBundleResultTypeDef,
     UpdateDistributionResultTypeDef,
@@ -455,15 +452,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.create_container_service)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#create_container_service)
         """
     def create_container_service_deployment(
         self,
         *,
         serviceName: str,
-        containers: Mapping[str, Union[ContainerTypeDef, ContainerOutputTypeDef]] = ...,
+        containers: Mapping[str, ContainerUnionTypeDef] = ...,
         publicEndpoint: EndpointRequestTypeDef = ...
     ) -> CreateContainerServiceDeploymentResultTypeDef:
         """
         Creates a deployment for your Amazon Lightsail container service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.create_container_service_deployment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#create_container_service_deployment)
@@ -530,15 +527,15 @@
     def create_distribution(
         self,
         *,
         distributionName: str,
         origin: InputOriginTypeDef,
         defaultCacheBehavior: CacheBehaviorTypeDef,
         bundleId: str,
-        cacheBehaviorSettings: Union[CacheSettingsTypeDef, CacheSettingsOutputTypeDef] = ...,
+        cacheBehaviorSettings: CacheSettingsUnionTypeDef = ...,
         cacheBehaviors: Sequence[CacheBehaviorPerPathTypeDef] = ...,
         ipAddressType: IpAddressTypeType = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateDistributionResultTypeDef:
         """
         Creates an Amazon Lightsail content delivery network (CDN) distribution.
 
@@ -551,15 +548,15 @@
         """
         Creates a domain resource for the specified domain (e.g., example.com).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.create_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#create_domain)
         """
     def create_domain_entry(
-        self, *, domainName: str, domainEntry: Union[DomainEntryTypeDef, DomainEntryOutputTypeDef]
+        self, *, domainName: str, domainEntry: DomainEntryUnionTypeDef
     ) -> CreateDomainEntryResultTypeDef:
         """
         Creates one of the following domain name system (DNS) records in a domain DNS
         zone: Address (A), canonical name (CNAME), mail exchanger (MX), name server
         (NS), start of authority (SOA), service locator (SRV), or text (TXT).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.create_domain_entry)
@@ -698,15 +695,15 @@
         *,
         relationalDatabaseName: str,
         availabilityZone: str = ...,
         publiclyAccessible: bool = ...,
         relationalDatabaseSnapshotName: str = ...,
         relationalDatabaseBundleId: str = ...,
         sourceRelationalDatabaseName: str = ...,
-        restoreTime: Union[datetime, str] = ...,
+        restoreTime: TimestampTypeDef = ...,
         useLatestRestorableTime: bool = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateRelationalDatabaseFromSnapshotResultTypeDef:
         """
         Creates a new database from an existing database snapshot in Amazon Lightsail.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.create_relational_database_from_snapshot)
@@ -820,15 +817,15 @@
         """
         Deletes the specified domain recordset and all of its domain records.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.delete_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#delete_domain)
         """
     def delete_domain_entry(
-        self, *, domainName: str, domainEntry: Union[DomainEntryTypeDef, DomainEntryOutputTypeDef]
+        self, *, domainName: str, domainEntry: DomainEntryUnionTypeDef
     ) -> DeleteDomainEntryResultTypeDef:
         """
         Deletes a specific domain entry.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.delete_domain_entry)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#delete_domain_entry)
         """
@@ -1035,16 +1032,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#get_bucket_bundles)
         """
     def get_bucket_metric_data(
         self,
         *,
         bucketName: str,
         metricName: BucketMetricNameType,
-        startTime: Union[datetime, str],
-        endTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
+        endTime: TimestampTypeDef,
         period: int,
         statistics: Sequence[MetricStatisticType],
         unit: MetricUnitType
     ) -> GetBucketMetricDataResultTypeDef:
         """
         Returns the data points of a specific metric for an Amazon Lightsail bucket.
 
@@ -1124,16 +1121,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#get_container_images)
         """
     def get_container_log(
         self,
         *,
         serviceName: str,
         containerName: str,
-        startTime: Union[datetime, str] = ...,
-        endTime: Union[datetime, str] = ...,
+        startTime: TimestampTypeDef = ...,
+        endTime: TimestampTypeDef = ...,
         filterPattern: str = ...,
         pageToken: str = ...
     ) -> GetContainerLogResultTypeDef:
         """
         Returns the log events of a container of your Amazon Lightsail container
         service.
 
@@ -1152,16 +1149,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#get_container_service_deployments)
         """
     def get_container_service_metric_data(
         self,
         *,
         serviceName: str,
         metricName: ContainerServiceMetricNameType,
-        startTime: Union[datetime, str],
-        endTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
+        endTime: TimestampTypeDef,
         period: int,
         statistics: Sequence[MetricStatisticType]
     ) -> GetContainerServiceMetricDataResultTypeDef:
         """
         Returns the data points of a specific metric of your Amazon Lightsail container
         service.
 
@@ -1183,15 +1180,15 @@
         Returns information about one or more of your Amazon Lightsail container
         services.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.get_container_services)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#get_container_services)
         """
     def get_cost_estimate(
-        self, *, resourceName: str, startTime: Union[datetime, str], endTime: Union[datetime, str]
+        self, *, resourceName: str, startTime: TimestampTypeDef, endTime: TimestampTypeDef
     ) -> GetCostEstimateResultTypeDef:
         """
         Retrieves information about the cost estimate for a specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.get_cost_estimate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#get_cost_estimate)
         """
@@ -1244,16 +1241,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#get_distribution_latest_cache_reset)
         """
     def get_distribution_metric_data(
         self,
         *,
         distributionName: str,
         metricName: DistributionMetricNameType,
-        startTime: Union[datetime, str],
-        endTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
+        endTime: TimestampTypeDef,
         period: int,
         unit: MetricUnitType,
         statistics: Sequence[MetricStatisticType]
     ) -> GetDistributionMetricDataResultTypeDef:
         """
         Returns the data points of a specific metric for an Amazon Lightsail content
         delivery network (CDN) distribution.
@@ -1315,16 +1312,16 @@
         """
     def get_instance_metric_data(
         self,
         *,
         instanceName: str,
         metricName: InstanceMetricNameType,
         period: int,
-        startTime: Union[datetime, str],
-        endTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
+        endTime: TimestampTypeDef,
         unit: MetricUnitType,
         statistics: Sequence[MetricStatisticType]
     ) -> GetInstanceMetricDataResultTypeDef:
         """
         Returns the data points for the specified Amazon Lightsail instance metric,
         given an instance name.
 
@@ -1396,16 +1393,16 @@
         """
     def get_load_balancer_metric_data(
         self,
         *,
         loadBalancerName: str,
         metricName: LoadBalancerMetricNameType,
         period: int,
-        startTime: Union[datetime, str],
-        endTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
+        endTime: TimestampTypeDef,
         unit: MetricUnitType,
         statistics: Sequence[MetricStatisticType]
     ) -> GetLoadBalancerMetricDataResultTypeDef:
         """
         Returns information about health metrics for your Lightsail load balancer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.get_load_balancer_metric_data)
@@ -1510,16 +1507,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#get_relational_database_events)
         """
     def get_relational_database_log_events(
         self,
         *,
         relationalDatabaseName: str,
         logStreamName: str,
-        startTime: Union[datetime, str] = ...,
-        endTime: Union[datetime, str] = ...,
+        startTime: TimestampTypeDef = ...,
+        endTime: TimestampTypeDef = ...,
         startFromHead: bool = ...,
         pageToken: str = ...
     ) -> GetRelationalDatabaseLogEventsResultTypeDef:
         """
         Returns a list of log events for a database in Amazon Lightsail.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.get_relational_database_log_events)
@@ -1550,16 +1547,16 @@
         """
     def get_relational_database_metric_data(
         self,
         *,
         relationalDatabaseName: str,
         metricName: RelationalDatabaseMetricNameType,
         period: int,
-        startTime: Union[datetime, str],
-        endTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
+        endTime: TimestampTypeDef,
         unit: MetricUnitType,
         statistics: Sequence[MetricStatisticType]
     ) -> GetRelationalDatabaseMetricDataResultTypeDef:
         """
         Returns the data points of the specified metric for a database in Amazon
         Lightsail.
 
@@ -1878,15 +1875,15 @@
         """
     def update_distribution(
         self,
         *,
         distributionName: str,
         origin: InputOriginTypeDef = ...,
         defaultCacheBehavior: CacheBehaviorTypeDef = ...,
-        cacheBehaviorSettings: Union[CacheSettingsTypeDef, CacheSettingsOutputTypeDef] = ...,
+        cacheBehaviorSettings: CacheSettingsUnionTypeDef = ...,
         cacheBehaviors: Sequence[CacheBehaviorPerPathTypeDef] = ...,
         isEnabled: bool = ...
     ) -> UpdateDistributionResultTypeDef:
         """
         Updates an existing Amazon Lightsail content delivery network (CDN)
         distribution.
 
@@ -1900,15 +1897,15 @@
         Updates the bundle of your Amazon Lightsail content delivery network (CDN)
         distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.update_distribution_bundle)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#update_distribution_bundle)
         """
     def update_domain_entry(
-        self, *, domainName: str, domainEntry: Union[DomainEntryTypeDef, DomainEntryOutputTypeDef]
+        self, *, domainName: str, domainEntry: DomainEntryUnionTypeDef
     ) -> UpdateDomainEntryResultTypeDef:
         """
         Updates a domain recordset after it is created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.update_domain_entry)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#update_domain_entry)
         """
```

### Comparing `mypy-boto3-lightsail-1.28.15.post1/mypy_boto3_lightsail/literals.py` & `mypy-boto3-lightsail-1.28.16/mypy_boto3_lightsail/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lightsail-1.28.15.post1/mypy_boto3_lightsail/literals.pyi` & `mypy-boto3-lightsail-1.28.16/mypy_boto3_lightsail/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lightsail-1.28.15.post1/mypy_boto3_lightsail/paginator.py` & `mypy-boto3-lightsail-1.28.16/mypy_boto3_lightsail/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lightsail-1.28.15.post1/mypy_boto3_lightsail/paginator.pyi` & `mypy-boto3-lightsail-1.28.16/mypy_boto3_lightsail/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lightsail-1.28.15.post1/mypy_boto3_lightsail/type_defs.py` & `mypy-boto3-lightsail-1.28.16/mypy_boto3_lightsail/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_lightsail.type_defs import AccessKeyLastUsedTypeDef
 
-    data: AccessKeyLastUsedTypeDef = {...}
+    data: AccessKeyLastUsedTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -152,14 +152,15 @@
     "InstanceEntryTypeDef",
     "CreateContactMethodRequestRequestTypeDef",
     "InputOriginTypeDef",
     "DomainEntryTypeDef",
     "CreateGUISessionAccessDetailsRequestRequestTypeDef",
     "SessionTypeDef",
     "DiskMapTypeDef",
+    "TimestampTypeDef",
     "DeleteAlarmRequestRequestTypeDef",
     "DeleteAutoSnapshotRequestRequestTypeDef",
     "DeleteBucketAccessKeyRequestRequestTypeDef",
     "DeleteBucketRequestRequestTypeDef",
     "DeleteCertificateRequestRequestTypeDef",
     "DeleteContactMethodRequestRequestTypeDef",
     "DeleteContainerImageRequestRequestTypeDef",
@@ -192,50 +193,43 @@
     "PaginatorConfigTypeDef",
     "GetActiveNamesRequestRequestTypeDef",
     "GetAlarmsRequestRequestTypeDef",
     "GetAutoSnapshotsRequestRequestTypeDef",
     "GetBlueprintsRequestRequestTypeDef",
     "GetBucketAccessKeysRequestRequestTypeDef",
     "GetBucketBundlesRequestRequestTypeDef",
-    "GetBucketMetricDataRequestRequestTypeDef",
     "MetricDatapointTypeDef",
     "GetBucketsRequestRequestTypeDef",
     "GetBundlesRequestRequestTypeDef",
     "GetCertificatesRequestRequestTypeDef",
     "GetCloudFormationStackRecordsRequestRequestTypeDef",
     "GetContactMethodsRequestRequestTypeDef",
     "GetContainerImagesRequestRequestTypeDef",
-    "GetContainerLogRequestRequestTypeDef",
     "GetContainerServiceDeploymentsRequestRequestTypeDef",
-    "GetContainerServiceMetricDataRequestRequestTypeDef",
     "GetContainerServicesRequestRequestTypeDef",
-    "GetCostEstimateRequestRequestTypeDef",
     "GetDiskRequestRequestTypeDef",
     "GetDiskSnapshotRequestRequestTypeDef",
     "GetDiskSnapshotsRequestRequestTypeDef",
     "GetDisksRequestRequestTypeDef",
     "GetDistributionLatestCacheResetRequestRequestTypeDef",
-    "GetDistributionMetricDataRequestRequestTypeDef",
     "GetDistributionsRequestRequestTypeDef",
     "GetDomainRequestRequestTypeDef",
     "GetDomainsRequestRequestTypeDef",
     "GetExportSnapshotRecordsRequestRequestTypeDef",
     "GetInstanceAccessDetailsRequestRequestTypeDef",
-    "GetInstanceMetricDataRequestRequestTypeDef",
     "GetInstancePortStatesRequestRequestTypeDef",
     "InstancePortStateTypeDef",
     "GetInstanceRequestRequestTypeDef",
     "GetInstanceSnapshotRequestRequestTypeDef",
     "GetInstanceSnapshotsRequestRequestTypeDef",
     "GetInstanceStateRequestRequestTypeDef",
     "InstanceStateTypeDef",
     "GetInstancesRequestRequestTypeDef",
     "GetKeyPairRequestRequestTypeDef",
     "GetKeyPairsRequestRequestTypeDef",
-    "GetLoadBalancerMetricDataRequestRequestTypeDef",
     "GetLoadBalancerRequestRequestTypeDef",
     "GetLoadBalancerTlsCertificatesRequestRequestTypeDef",
     "GetLoadBalancerTlsPoliciesRequestRequestTypeDef",
     "LoadBalancerTlsPolicyTypeDef",
     "GetLoadBalancersRequestRequestTypeDef",
     "GetOperationRequestRequestTypeDef",
     "GetOperationsForResourceRequestRequestTypeDef",
@@ -243,19 +237,17 @@
     "GetRegionsRequestRequestTypeDef",
     "GetRelationalDatabaseBlueprintsRequestRequestTypeDef",
     "RelationalDatabaseBlueprintTypeDef",
     "GetRelationalDatabaseBundlesRequestRequestTypeDef",
     "RelationalDatabaseBundleTypeDef",
     "GetRelationalDatabaseEventsRequestRequestTypeDef",
     "RelationalDatabaseEventTypeDef",
-    "GetRelationalDatabaseLogEventsRequestRequestTypeDef",
     "LogEventTypeDef",
     "GetRelationalDatabaseLogStreamsRequestRequestTypeDef",
     "GetRelationalDatabaseMasterUserPasswordRequestRequestTypeDef",
-    "GetRelationalDatabaseMetricDataRequestRequestTypeDef",
     "GetRelationalDatabaseParametersRequestRequestTypeDef",
     "RelationalDatabaseParameterTypeDef",
     "GetRelationalDatabaseRequestRequestTypeDef",
     "GetRelationalDatabaseSnapshotRequestRequestTypeDef",
     "GetRelationalDatabaseSnapshotsRequestRequestTypeDef",
     "GetRelationalDatabasesRequestRequestTypeDef",
     "GetStaticIpRequestRequestTypeDef",
@@ -322,15 +314,14 @@
     "CreateCertificateRequestRequestTypeDef",
     "CreateDiskSnapshotRequestRequestTypeDef",
     "CreateDomainRequestRequestTypeDef",
     "CreateInstanceSnapshotRequestRequestTypeDef",
     "CreateKeyPairRequestRequestTypeDef",
     "CreateLoadBalancerRequestRequestTypeDef",
     "CreateLoadBalancerTlsCertificateRequestRequestTypeDef",
-    "CreateRelationalDatabaseFromSnapshotRequestRequestTypeDef",
     "CreateRelationalDatabaseRequestRequestTypeDef",
     "CreateRelationalDatabaseSnapshotRequestRequestTypeDef",
     "DiskSnapshotTypeDef",
     "DiskTypeDef",
     "KeyPairTypeDef",
     "RelationalDatabaseSnapshotTypeDef",
     "TagResourceRequestRequestTypeDef",
@@ -339,28 +330,40 @@
     "CacheSettingsTypeDef",
     "CloseInstancePublicPortsRequestRequestTypeDef",
     "OpenInstancePublicPortsRequestRequestTypeDef",
     "PutInstancePublicPortsRequestRequestTypeDef",
     "CloudFormationStackRecordTypeDef",
     "GetContainerImagesResultTypeDef",
     "RegisterContainerImageResultTypeDef",
+    "ContainerUnionTypeDef",
     "PrivateRegistryAccessRequestTypeDef",
     "PrivateRegistryAccessTypeDef",
     "ContainerServiceEndpointTypeDef",
     "EndpointRequestTypeDef",
     "GetContainerLogResultTypeDef",
     "GetContainerServicePowersResultTypeDef",
     "CreateContainerServiceRegistryLoginResultTypeDef",
     "CreateCloudFormationStackRequestRequestTypeDef",
     "CreateDomainEntryRequestRequestTypeDef",
     "DeleteDomainEntryRequestRequestTypeDef",
     "UpdateDomainEntryRequestRequestTypeDef",
     "CreateGUISessionAccessDetailsResultTypeDef",
+    "CreateRelationalDatabaseFromSnapshotRequestRequestTypeDef",
+    "GetBucketMetricDataRequestRequestTypeDef",
+    "GetContainerLogRequestRequestTypeDef",
+    "GetContainerServiceMetricDataRequestRequestTypeDef",
+    "GetCostEstimateRequestRequestTypeDef",
+    "GetDistributionMetricDataRequestRequestTypeDef",
+    "GetInstanceMetricDataRequestRequestTypeDef",
+    "GetLoadBalancerMetricDataRequestRequestTypeDef",
+    "GetRelationalDatabaseLogEventsRequestRequestTypeDef",
+    "GetRelationalDatabaseMetricDataRequestRequestTypeDef",
     "InstanceSnapshotInfoTypeDef",
     "GetDistributionBundlesResultTypeDef",
+    "DomainEntryUnionTypeDef",
     "DomainValidationRecordTypeDef",
     "EstimateByTimeTypeDef",
     "GetActiveNamesRequestGetActiveNamesPaginateTypeDef",
     "GetBlueprintsRequestGetBlueprintsPaginateTypeDef",
     "GetBundlesRequestGetBundlesPaginateTypeDef",
     "GetCloudFormationStackRecordsRequestGetCloudFormationStackRecordsPaginateTypeDef",
     "GetDiskSnapshotsRequestGetDiskSnapshotsPaginateTypeDef",
@@ -507,14 +510,15 @@
     "InstanceSnapshotTypeDef",
     "CreateKeyPairResultTypeDef",
     "GetKeyPairResultTypeDef",
     "GetKeyPairsResultTypeDef",
     "GetRelationalDatabaseSnapshotResultTypeDef",
     "GetRelationalDatabaseSnapshotsResultTypeDef",
     "LightsailDistributionTypeDef",
+    "CacheSettingsUnionTypeDef",
     "CreateDistributionRequestRequestTypeDef",
     "UpdateDistributionRequestRequestTypeDef",
     "GetCloudFormationStackRecordsResultTypeDef",
     "UpdateContainerServiceRequestRequestTypeDef",
     "ContainerServiceDeploymentTypeDef",
     "ContainerServiceDeploymentRequestTypeDef",
     "CreateContainerServiceDeploymentRequestRequestTypeDef",
@@ -1140,14 +1144,15 @@
     {
         "originalDiskPath": str,
         "newDiskName": str,
     },
     total=False,
 )
 
+TimestampTypeDef = Union[datetime, str]
 DeleteAlarmRequestRequestTypeDef = TypedDict(
     "DeleteAlarmRequestRequestTypeDef",
     {
         "alarmName": str,
     },
 )
 
@@ -1548,27 +1553,14 @@
     "GetBucketBundlesRequestRequestTypeDef",
     {
         "includeInactive": bool,
     },
     total=False,
 )
 
-GetBucketMetricDataRequestRequestTypeDef = TypedDict(
-    "GetBucketMetricDataRequestRequestTypeDef",
-    {
-        "bucketName": str,
-        "metricName": BucketMetricNameType,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-        "period": int,
-        "statistics": Sequence[MetricStatisticType],
-        "unit": MetricUnitType,
-    },
-)
-
 MetricDatapointTypeDef = TypedDict(
     "MetricDatapointTypeDef",
     {
         "average": float,
         "maximum": float,
         "minimum": float,
         "sampleCount": float,
@@ -1629,75 +1621,29 @@
 GetContainerImagesRequestRequestTypeDef = TypedDict(
     "GetContainerImagesRequestRequestTypeDef",
     {
         "serviceName": str,
     },
 )
 
-_RequiredGetContainerLogRequestRequestTypeDef = TypedDict(
-    "_RequiredGetContainerLogRequestRequestTypeDef",
-    {
-        "serviceName": str,
-        "containerName": str,
-    },
-)
-_OptionalGetContainerLogRequestRequestTypeDef = TypedDict(
-    "_OptionalGetContainerLogRequestRequestTypeDef",
-    {
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-        "filterPattern": str,
-        "pageToken": str,
-    },
-    total=False,
-)
-
-
-class GetContainerLogRequestRequestTypeDef(
-    _RequiredGetContainerLogRequestRequestTypeDef, _OptionalGetContainerLogRequestRequestTypeDef
-):
-    pass
-
-
 GetContainerServiceDeploymentsRequestRequestTypeDef = TypedDict(
     "GetContainerServiceDeploymentsRequestRequestTypeDef",
     {
         "serviceName": str,
     },
 )
 
-GetContainerServiceMetricDataRequestRequestTypeDef = TypedDict(
-    "GetContainerServiceMetricDataRequestRequestTypeDef",
-    {
-        "serviceName": str,
-        "metricName": ContainerServiceMetricNameType,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-        "period": int,
-        "statistics": Sequence[MetricStatisticType],
-    },
-)
-
 GetContainerServicesRequestRequestTypeDef = TypedDict(
     "GetContainerServicesRequestRequestTypeDef",
     {
         "serviceName": str,
     },
     total=False,
 )
 
-GetCostEstimateRequestRequestTypeDef = TypedDict(
-    "GetCostEstimateRequestRequestTypeDef",
-    {
-        "resourceName": str,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-    },
-)
-
 GetDiskRequestRequestTypeDef = TypedDict(
     "GetDiskRequestRequestTypeDef",
     {
         "diskName": str,
     },
 )
 
@@ -1728,27 +1674,14 @@
     "GetDistributionLatestCacheResetRequestRequestTypeDef",
     {
         "distributionName": str,
     },
     total=False,
 )
 
-GetDistributionMetricDataRequestRequestTypeDef = TypedDict(
-    "GetDistributionMetricDataRequestRequestTypeDef",
-    {
-        "distributionName": str,
-        "metricName": DistributionMetricNameType,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-        "period": int,
-        "unit": MetricUnitType,
-        "statistics": Sequence[MetricStatisticType],
-    },
-)
-
 GetDistributionsRequestRequestTypeDef = TypedDict(
     "GetDistributionsRequestRequestTypeDef",
     {
         "distributionName": str,
         "pageToken": str,
     },
     total=False,
@@ -1795,27 +1728,14 @@
 class GetInstanceAccessDetailsRequestRequestTypeDef(
     _RequiredGetInstanceAccessDetailsRequestRequestTypeDef,
     _OptionalGetInstanceAccessDetailsRequestRequestTypeDef,
 ):
     pass
 
 
-GetInstanceMetricDataRequestRequestTypeDef = TypedDict(
-    "GetInstanceMetricDataRequestRequestTypeDef",
-    {
-        "instanceName": str,
-        "metricName": InstanceMetricNameType,
-        "period": int,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-        "unit": MetricUnitType,
-        "statistics": Sequence[MetricStatisticType],
-    },
-)
-
 GetInstancePortStatesRequestRequestTypeDef = TypedDict(
     "GetInstancePortStatesRequestRequestTypeDef",
     {
         "instanceName": str,
     },
 )
 
@@ -1891,27 +1811,14 @@
     {
         "pageToken": str,
         "includeDefaultKeyPair": bool,
     },
     total=False,
 )
 
-GetLoadBalancerMetricDataRequestRequestTypeDef = TypedDict(
-    "GetLoadBalancerMetricDataRequestRequestTypeDef",
-    {
-        "loadBalancerName": str,
-        "metricName": LoadBalancerMetricNameType,
-        "period": int,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-        "unit": MetricUnitType,
-        "statistics": Sequence[MetricStatisticType],
-    },
-)
-
 GetLoadBalancerRequestRequestTypeDef = TypedDict(
     "GetLoadBalancerRequestRequestTypeDef",
     {
         "loadBalancerName": str,
     },
 )
 
@@ -2072,40 +1979,14 @@
         "createdAt": datetime,
         "message": str,
         "eventCategories": List[str],
     },
     total=False,
 )
 
-_RequiredGetRelationalDatabaseLogEventsRequestRequestTypeDef = TypedDict(
-    "_RequiredGetRelationalDatabaseLogEventsRequestRequestTypeDef",
-    {
-        "relationalDatabaseName": str,
-        "logStreamName": str,
-    },
-)
-_OptionalGetRelationalDatabaseLogEventsRequestRequestTypeDef = TypedDict(
-    "_OptionalGetRelationalDatabaseLogEventsRequestRequestTypeDef",
-    {
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-        "startFromHead": bool,
-        "pageToken": str,
-    },
-    total=False,
-)
-
-
-class GetRelationalDatabaseLogEventsRequestRequestTypeDef(
-    _RequiredGetRelationalDatabaseLogEventsRequestRequestTypeDef,
-    _OptionalGetRelationalDatabaseLogEventsRequestRequestTypeDef,
-):
-    pass
-
-
 LogEventTypeDef = TypedDict(
     "LogEventTypeDef",
     {
         "createdAt": datetime,
         "message": str,
     },
     total=False,
@@ -2136,27 +2017,14 @@
 class GetRelationalDatabaseMasterUserPasswordRequestRequestTypeDef(
     _RequiredGetRelationalDatabaseMasterUserPasswordRequestRequestTypeDef,
     _OptionalGetRelationalDatabaseMasterUserPasswordRequestRequestTypeDef,
 ):
     pass
 
 
-GetRelationalDatabaseMetricDataRequestRequestTypeDef = TypedDict(
-    "GetRelationalDatabaseMetricDataRequestRequestTypeDef",
-    {
-        "relationalDatabaseName": str,
-        "metricName": RelationalDatabaseMetricNameType,
-        "period": int,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-        "unit": MetricUnitType,
-        "statistics": Sequence[MetricStatisticType],
-    },
-)
-
 _RequiredGetRelationalDatabaseParametersRequestRequestTypeDef = TypedDict(
     "_RequiredGetRelationalDatabaseParametersRequestRequestTypeDef",
     {
         "relationalDatabaseName": str,
     },
 )
 _OptionalGetRelationalDatabaseParametersRequestRequestTypeDef = TypedDict(
@@ -3127,43 +2995,14 @@
 class CreateLoadBalancerTlsCertificateRequestRequestTypeDef(
     _RequiredCreateLoadBalancerTlsCertificateRequestRequestTypeDef,
     _OptionalCreateLoadBalancerTlsCertificateRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredCreateRelationalDatabaseFromSnapshotRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateRelationalDatabaseFromSnapshotRequestRequestTypeDef",
-    {
-        "relationalDatabaseName": str,
-    },
-)
-_OptionalCreateRelationalDatabaseFromSnapshotRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateRelationalDatabaseFromSnapshotRequestRequestTypeDef",
-    {
-        "availabilityZone": str,
-        "publiclyAccessible": bool,
-        "relationalDatabaseSnapshotName": str,
-        "relationalDatabaseBundleId": str,
-        "sourceRelationalDatabaseName": str,
-        "restoreTime": Union[datetime, str],
-        "useLatestRestorableTime": bool,
-        "tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-
-class CreateRelationalDatabaseFromSnapshotRequestRequestTypeDef(
-    _RequiredCreateRelationalDatabaseFromSnapshotRequestRequestTypeDef,
-    _OptionalCreateRelationalDatabaseFromSnapshotRequestRequestTypeDef,
-):
-    pass
-
-
 _RequiredCreateRelationalDatabaseRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRelationalDatabaseRequestRequestTypeDef",
     {
         "relationalDatabaseName": str,
         "relationalDatabaseBlueprintId": str,
         "relationalDatabaseBundleId": str,
         "masterDatabaseName": str,
@@ -3410,14 +3249,15 @@
     "RegisterContainerImageResultTypeDef",
     {
         "containerImage": ContainerImageTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ContainerUnionTypeDef = Union[ContainerTypeDef, ContainerOutputTypeDef]
 PrivateRegistryAccessRequestTypeDef = TypedDict(
     "PrivateRegistryAccessRequestTypeDef",
     {
         "ecrImagePullerRole": ContainerServiceECRImagePullerRoleRequestTypeDef,
     },
     total=False,
 )
@@ -3524,14 +3364,180 @@
         "percentageComplete": int,
         "failureReason": str,
         "sessions": List[SessionTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateRelationalDatabaseFromSnapshotRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateRelationalDatabaseFromSnapshotRequestRequestTypeDef",
+    {
+        "relationalDatabaseName": str,
+    },
+)
+_OptionalCreateRelationalDatabaseFromSnapshotRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateRelationalDatabaseFromSnapshotRequestRequestTypeDef",
+    {
+        "availabilityZone": str,
+        "publiclyAccessible": bool,
+        "relationalDatabaseSnapshotName": str,
+        "relationalDatabaseBundleId": str,
+        "sourceRelationalDatabaseName": str,
+        "restoreTime": TimestampTypeDef,
+        "useLatestRestorableTime": bool,
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateRelationalDatabaseFromSnapshotRequestRequestTypeDef(
+    _RequiredCreateRelationalDatabaseFromSnapshotRequestRequestTypeDef,
+    _OptionalCreateRelationalDatabaseFromSnapshotRequestRequestTypeDef,
+):
+    pass
+
+
+GetBucketMetricDataRequestRequestTypeDef = TypedDict(
+    "GetBucketMetricDataRequestRequestTypeDef",
+    {
+        "bucketName": str,
+        "metricName": BucketMetricNameType,
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+        "period": int,
+        "statistics": Sequence[MetricStatisticType],
+        "unit": MetricUnitType,
+    },
+)
+
+_RequiredGetContainerLogRequestRequestTypeDef = TypedDict(
+    "_RequiredGetContainerLogRequestRequestTypeDef",
+    {
+        "serviceName": str,
+        "containerName": str,
+    },
+)
+_OptionalGetContainerLogRequestRequestTypeDef = TypedDict(
+    "_OptionalGetContainerLogRequestRequestTypeDef",
+    {
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+        "filterPattern": str,
+        "pageToken": str,
+    },
+    total=False,
+)
+
+
+class GetContainerLogRequestRequestTypeDef(
+    _RequiredGetContainerLogRequestRequestTypeDef, _OptionalGetContainerLogRequestRequestTypeDef
+):
+    pass
+
+
+GetContainerServiceMetricDataRequestRequestTypeDef = TypedDict(
+    "GetContainerServiceMetricDataRequestRequestTypeDef",
+    {
+        "serviceName": str,
+        "metricName": ContainerServiceMetricNameType,
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+        "period": int,
+        "statistics": Sequence[MetricStatisticType],
+    },
+)
+
+GetCostEstimateRequestRequestTypeDef = TypedDict(
+    "GetCostEstimateRequestRequestTypeDef",
+    {
+        "resourceName": str,
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+    },
+)
+
+GetDistributionMetricDataRequestRequestTypeDef = TypedDict(
+    "GetDistributionMetricDataRequestRequestTypeDef",
+    {
+        "distributionName": str,
+        "metricName": DistributionMetricNameType,
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+        "period": int,
+        "unit": MetricUnitType,
+        "statistics": Sequence[MetricStatisticType],
+    },
+)
+
+GetInstanceMetricDataRequestRequestTypeDef = TypedDict(
+    "GetInstanceMetricDataRequestRequestTypeDef",
+    {
+        "instanceName": str,
+        "metricName": InstanceMetricNameType,
+        "period": int,
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+        "unit": MetricUnitType,
+        "statistics": Sequence[MetricStatisticType],
+    },
+)
+
+GetLoadBalancerMetricDataRequestRequestTypeDef = TypedDict(
+    "GetLoadBalancerMetricDataRequestRequestTypeDef",
+    {
+        "loadBalancerName": str,
+        "metricName": LoadBalancerMetricNameType,
+        "period": int,
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+        "unit": MetricUnitType,
+        "statistics": Sequence[MetricStatisticType],
+    },
+)
+
+_RequiredGetRelationalDatabaseLogEventsRequestRequestTypeDef = TypedDict(
+    "_RequiredGetRelationalDatabaseLogEventsRequestRequestTypeDef",
+    {
+        "relationalDatabaseName": str,
+        "logStreamName": str,
+    },
+)
+_OptionalGetRelationalDatabaseLogEventsRequestRequestTypeDef = TypedDict(
+    "_OptionalGetRelationalDatabaseLogEventsRequestRequestTypeDef",
+    {
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+        "startFromHead": bool,
+        "pageToken": str,
+    },
+    total=False,
+)
+
+
+class GetRelationalDatabaseLogEventsRequestRequestTypeDef(
+    _RequiredGetRelationalDatabaseLogEventsRequestRequestTypeDef,
+    _OptionalGetRelationalDatabaseLogEventsRequestRequestTypeDef,
+):
+    pass
+
+
+GetRelationalDatabaseMetricDataRequestRequestTypeDef = TypedDict(
+    "GetRelationalDatabaseMetricDataRequestRequestTypeDef",
+    {
+        "relationalDatabaseName": str,
+        "metricName": RelationalDatabaseMetricNameType,
+        "period": int,
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+        "unit": MetricUnitType,
+        "statistics": Sequence[MetricStatisticType],
+    },
+)
+
 InstanceSnapshotInfoTypeDef = TypedDict(
     "InstanceSnapshotInfoTypeDef",
     {
         "fromBundleId": str,
         "fromBlueprintId": str,
         "fromDiskInfo": List[DiskInfoTypeDef],
     },
@@ -3542,14 +3548,15 @@
     "GetDistributionBundlesResultTypeDef",
     {
         "bundles": List[DistributionBundleTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DomainEntryUnionTypeDef = Union[DomainEntryTypeDef, DomainEntryOutputTypeDef]
 DomainValidationRecordTypeDef = TypedDict(
     "DomainValidationRecordTypeDef",
     {
         "domainName": str,
         "resourceRecord": ResourceRecordTypeDef,
         "dnsRecordCreationState": DnsRecordCreationStateTypeDef,
         "validationStatus": CertificateDomainValidationStatusType,
@@ -5029,14 +5036,15 @@
         "ableToUpdateBundle": bool,
         "ipAddressType": IpAddressTypeType,
         "tags": List[TagTypeDef],
     },
     total=False,
 )
 
+CacheSettingsUnionTypeDef = Union[CacheSettingsTypeDef, CacheSettingsOutputTypeDef]
 _RequiredCreateDistributionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDistributionRequestRequestTypeDef",
     {
         "distributionName": str,
         "origin": InputOriginTypeDef,
         "defaultCacheBehavior": CacheBehaviorTypeDef,
         "bundleId": str,
@@ -5148,15 +5156,15 @@
     {
         "serviceName": str,
     },
 )
 _OptionalCreateContainerServiceDeploymentRequestRequestTypeDef = TypedDict(
     "_OptionalCreateContainerServiceDeploymentRequestRequestTypeDef",
     {
-        "containers": Mapping[str, Union[ContainerTypeDef, ContainerOutputTypeDef]],
+        "containers": Mapping[str, ContainerUnionTypeDef],
         "publicEndpoint": EndpointRequestTypeDef,
     },
     total=False,
 )
 
 
 class CreateContainerServiceDeploymentRequestRequestTypeDef(
```

### Comparing `mypy-boto3-lightsail-1.28.15.post1/mypy_boto3_lightsail/type_defs.pyi` & `mypy-boto3-lightsail-1.28.16/mypy_boto3_lightsail/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_lightsail.type_defs import AccessKeyLastUsedTypeDef
 
-    data: AccessKeyLastUsedTypeDef = {...}
+    data: AccessKeyLastUsedTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -151,14 +151,15 @@
     "InstanceEntryTypeDef",
     "CreateContactMethodRequestRequestTypeDef",
     "InputOriginTypeDef",
     "DomainEntryTypeDef",
     "CreateGUISessionAccessDetailsRequestRequestTypeDef",
     "SessionTypeDef",
     "DiskMapTypeDef",
+    "TimestampTypeDef",
     "DeleteAlarmRequestRequestTypeDef",
     "DeleteAutoSnapshotRequestRequestTypeDef",
     "DeleteBucketAccessKeyRequestRequestTypeDef",
     "DeleteBucketRequestRequestTypeDef",
     "DeleteCertificateRequestRequestTypeDef",
     "DeleteContactMethodRequestRequestTypeDef",
     "DeleteContainerImageRequestRequestTypeDef",
@@ -191,50 +192,43 @@
     "PaginatorConfigTypeDef",
     "GetActiveNamesRequestRequestTypeDef",
     "GetAlarmsRequestRequestTypeDef",
     "GetAutoSnapshotsRequestRequestTypeDef",
     "GetBlueprintsRequestRequestTypeDef",
     "GetBucketAccessKeysRequestRequestTypeDef",
     "GetBucketBundlesRequestRequestTypeDef",
-    "GetBucketMetricDataRequestRequestTypeDef",
     "MetricDatapointTypeDef",
     "GetBucketsRequestRequestTypeDef",
     "GetBundlesRequestRequestTypeDef",
     "GetCertificatesRequestRequestTypeDef",
     "GetCloudFormationStackRecordsRequestRequestTypeDef",
     "GetContactMethodsRequestRequestTypeDef",
     "GetContainerImagesRequestRequestTypeDef",
-    "GetContainerLogRequestRequestTypeDef",
     "GetContainerServiceDeploymentsRequestRequestTypeDef",
-    "GetContainerServiceMetricDataRequestRequestTypeDef",
     "GetContainerServicesRequestRequestTypeDef",
-    "GetCostEstimateRequestRequestTypeDef",
     "GetDiskRequestRequestTypeDef",
     "GetDiskSnapshotRequestRequestTypeDef",
     "GetDiskSnapshotsRequestRequestTypeDef",
     "GetDisksRequestRequestTypeDef",
     "GetDistributionLatestCacheResetRequestRequestTypeDef",
-    "GetDistributionMetricDataRequestRequestTypeDef",
     "GetDistributionsRequestRequestTypeDef",
     "GetDomainRequestRequestTypeDef",
     "GetDomainsRequestRequestTypeDef",
     "GetExportSnapshotRecordsRequestRequestTypeDef",
     "GetInstanceAccessDetailsRequestRequestTypeDef",
-    "GetInstanceMetricDataRequestRequestTypeDef",
     "GetInstancePortStatesRequestRequestTypeDef",
     "InstancePortStateTypeDef",
     "GetInstanceRequestRequestTypeDef",
     "GetInstanceSnapshotRequestRequestTypeDef",
     "GetInstanceSnapshotsRequestRequestTypeDef",
     "GetInstanceStateRequestRequestTypeDef",
     "InstanceStateTypeDef",
     "GetInstancesRequestRequestTypeDef",
     "GetKeyPairRequestRequestTypeDef",
     "GetKeyPairsRequestRequestTypeDef",
-    "GetLoadBalancerMetricDataRequestRequestTypeDef",
     "GetLoadBalancerRequestRequestTypeDef",
     "GetLoadBalancerTlsCertificatesRequestRequestTypeDef",
     "GetLoadBalancerTlsPoliciesRequestRequestTypeDef",
     "LoadBalancerTlsPolicyTypeDef",
     "GetLoadBalancersRequestRequestTypeDef",
     "GetOperationRequestRequestTypeDef",
     "GetOperationsForResourceRequestRequestTypeDef",
@@ -242,19 +236,17 @@
     "GetRegionsRequestRequestTypeDef",
     "GetRelationalDatabaseBlueprintsRequestRequestTypeDef",
     "RelationalDatabaseBlueprintTypeDef",
     "GetRelationalDatabaseBundlesRequestRequestTypeDef",
     "RelationalDatabaseBundleTypeDef",
     "GetRelationalDatabaseEventsRequestRequestTypeDef",
     "RelationalDatabaseEventTypeDef",
-    "GetRelationalDatabaseLogEventsRequestRequestTypeDef",
     "LogEventTypeDef",
     "GetRelationalDatabaseLogStreamsRequestRequestTypeDef",
     "GetRelationalDatabaseMasterUserPasswordRequestRequestTypeDef",
-    "GetRelationalDatabaseMetricDataRequestRequestTypeDef",
     "GetRelationalDatabaseParametersRequestRequestTypeDef",
     "RelationalDatabaseParameterTypeDef",
     "GetRelationalDatabaseRequestRequestTypeDef",
     "GetRelationalDatabaseSnapshotRequestRequestTypeDef",
     "GetRelationalDatabaseSnapshotsRequestRequestTypeDef",
     "GetRelationalDatabasesRequestRequestTypeDef",
     "GetStaticIpRequestRequestTypeDef",
@@ -321,15 +313,14 @@
     "CreateCertificateRequestRequestTypeDef",
     "CreateDiskSnapshotRequestRequestTypeDef",
     "CreateDomainRequestRequestTypeDef",
     "CreateInstanceSnapshotRequestRequestTypeDef",
     "CreateKeyPairRequestRequestTypeDef",
     "CreateLoadBalancerRequestRequestTypeDef",
     "CreateLoadBalancerTlsCertificateRequestRequestTypeDef",
-    "CreateRelationalDatabaseFromSnapshotRequestRequestTypeDef",
     "CreateRelationalDatabaseRequestRequestTypeDef",
     "CreateRelationalDatabaseSnapshotRequestRequestTypeDef",
     "DiskSnapshotTypeDef",
     "DiskTypeDef",
     "KeyPairTypeDef",
     "RelationalDatabaseSnapshotTypeDef",
     "TagResourceRequestRequestTypeDef",
@@ -338,28 +329,40 @@
     "CacheSettingsTypeDef",
     "CloseInstancePublicPortsRequestRequestTypeDef",
     "OpenInstancePublicPortsRequestRequestTypeDef",
     "PutInstancePublicPortsRequestRequestTypeDef",
     "CloudFormationStackRecordTypeDef",
     "GetContainerImagesResultTypeDef",
     "RegisterContainerImageResultTypeDef",
+    "ContainerUnionTypeDef",
     "PrivateRegistryAccessRequestTypeDef",
     "PrivateRegistryAccessTypeDef",
     "ContainerServiceEndpointTypeDef",
     "EndpointRequestTypeDef",
     "GetContainerLogResultTypeDef",
     "GetContainerServicePowersResultTypeDef",
     "CreateContainerServiceRegistryLoginResultTypeDef",
     "CreateCloudFormationStackRequestRequestTypeDef",
     "CreateDomainEntryRequestRequestTypeDef",
     "DeleteDomainEntryRequestRequestTypeDef",
     "UpdateDomainEntryRequestRequestTypeDef",
     "CreateGUISessionAccessDetailsResultTypeDef",
+    "CreateRelationalDatabaseFromSnapshotRequestRequestTypeDef",
+    "GetBucketMetricDataRequestRequestTypeDef",
+    "GetContainerLogRequestRequestTypeDef",
+    "GetContainerServiceMetricDataRequestRequestTypeDef",
+    "GetCostEstimateRequestRequestTypeDef",
+    "GetDistributionMetricDataRequestRequestTypeDef",
+    "GetInstanceMetricDataRequestRequestTypeDef",
+    "GetLoadBalancerMetricDataRequestRequestTypeDef",
+    "GetRelationalDatabaseLogEventsRequestRequestTypeDef",
+    "GetRelationalDatabaseMetricDataRequestRequestTypeDef",
     "InstanceSnapshotInfoTypeDef",
     "GetDistributionBundlesResultTypeDef",
+    "DomainEntryUnionTypeDef",
     "DomainValidationRecordTypeDef",
     "EstimateByTimeTypeDef",
     "GetActiveNamesRequestGetActiveNamesPaginateTypeDef",
     "GetBlueprintsRequestGetBlueprintsPaginateTypeDef",
     "GetBundlesRequestGetBundlesPaginateTypeDef",
     "GetCloudFormationStackRecordsRequestGetCloudFormationStackRecordsPaginateTypeDef",
     "GetDiskSnapshotsRequestGetDiskSnapshotsPaginateTypeDef",
@@ -506,14 +509,15 @@
     "InstanceSnapshotTypeDef",
     "CreateKeyPairResultTypeDef",
     "GetKeyPairResultTypeDef",
     "GetKeyPairsResultTypeDef",
     "GetRelationalDatabaseSnapshotResultTypeDef",
     "GetRelationalDatabaseSnapshotsResultTypeDef",
     "LightsailDistributionTypeDef",
+    "CacheSettingsUnionTypeDef",
     "CreateDistributionRequestRequestTypeDef",
     "UpdateDistributionRequestRequestTypeDef",
     "GetCloudFormationStackRecordsResultTypeDef",
     "UpdateContainerServiceRequestRequestTypeDef",
     "ContainerServiceDeploymentTypeDef",
     "ContainerServiceDeploymentRequestTypeDef",
     "CreateContainerServiceDeploymentRequestRequestTypeDef",
@@ -1131,14 +1135,15 @@
     {
         "originalDiskPath": str,
         "newDiskName": str,
     },
     total=False,
 )
 
+TimestampTypeDef = Union[datetime, str]
 DeleteAlarmRequestRequestTypeDef = TypedDict(
     "DeleteAlarmRequestRequestTypeDef",
     {
         "alarmName": str,
     },
 )
 
@@ -1527,27 +1532,14 @@
     "GetBucketBundlesRequestRequestTypeDef",
     {
         "includeInactive": bool,
     },
     total=False,
 )
 
-GetBucketMetricDataRequestRequestTypeDef = TypedDict(
-    "GetBucketMetricDataRequestRequestTypeDef",
-    {
-        "bucketName": str,
-        "metricName": BucketMetricNameType,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-        "period": int,
-        "statistics": Sequence[MetricStatisticType],
-        "unit": MetricUnitType,
-    },
-)
-
 MetricDatapointTypeDef = TypedDict(
     "MetricDatapointTypeDef",
     {
         "average": float,
         "maximum": float,
         "minimum": float,
         "sampleCount": float,
@@ -1608,73 +1600,29 @@
 GetContainerImagesRequestRequestTypeDef = TypedDict(
     "GetContainerImagesRequestRequestTypeDef",
     {
         "serviceName": str,
     },
 )
 
-_RequiredGetContainerLogRequestRequestTypeDef = TypedDict(
-    "_RequiredGetContainerLogRequestRequestTypeDef",
-    {
-        "serviceName": str,
-        "containerName": str,
-    },
-)
-_OptionalGetContainerLogRequestRequestTypeDef = TypedDict(
-    "_OptionalGetContainerLogRequestRequestTypeDef",
-    {
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-        "filterPattern": str,
-        "pageToken": str,
-    },
-    total=False,
-)
-
-class GetContainerLogRequestRequestTypeDef(
-    _RequiredGetContainerLogRequestRequestTypeDef, _OptionalGetContainerLogRequestRequestTypeDef
-):
-    pass
-
 GetContainerServiceDeploymentsRequestRequestTypeDef = TypedDict(
     "GetContainerServiceDeploymentsRequestRequestTypeDef",
     {
         "serviceName": str,
     },
 )
 
-GetContainerServiceMetricDataRequestRequestTypeDef = TypedDict(
-    "GetContainerServiceMetricDataRequestRequestTypeDef",
-    {
-        "serviceName": str,
-        "metricName": ContainerServiceMetricNameType,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-        "period": int,
-        "statistics": Sequence[MetricStatisticType],
-    },
-)
-
 GetContainerServicesRequestRequestTypeDef = TypedDict(
     "GetContainerServicesRequestRequestTypeDef",
     {
         "serviceName": str,
     },
     total=False,
 )
 
-GetCostEstimateRequestRequestTypeDef = TypedDict(
-    "GetCostEstimateRequestRequestTypeDef",
-    {
-        "resourceName": str,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-    },
-)
-
 GetDiskRequestRequestTypeDef = TypedDict(
     "GetDiskRequestRequestTypeDef",
     {
         "diskName": str,
     },
 )
 
@@ -1705,27 +1653,14 @@
     "GetDistributionLatestCacheResetRequestRequestTypeDef",
     {
         "distributionName": str,
     },
     total=False,
 )
 
-GetDistributionMetricDataRequestRequestTypeDef = TypedDict(
-    "GetDistributionMetricDataRequestRequestTypeDef",
-    {
-        "distributionName": str,
-        "metricName": DistributionMetricNameType,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-        "period": int,
-        "unit": MetricUnitType,
-        "statistics": Sequence[MetricStatisticType],
-    },
-)
-
 GetDistributionsRequestRequestTypeDef = TypedDict(
     "GetDistributionsRequestRequestTypeDef",
     {
         "distributionName": str,
         "pageToken": str,
     },
     total=False,
@@ -1770,27 +1705,14 @@
 
 class GetInstanceAccessDetailsRequestRequestTypeDef(
     _RequiredGetInstanceAccessDetailsRequestRequestTypeDef,
     _OptionalGetInstanceAccessDetailsRequestRequestTypeDef,
 ):
     pass
 
-GetInstanceMetricDataRequestRequestTypeDef = TypedDict(
-    "GetInstanceMetricDataRequestRequestTypeDef",
-    {
-        "instanceName": str,
-        "metricName": InstanceMetricNameType,
-        "period": int,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-        "unit": MetricUnitType,
-        "statistics": Sequence[MetricStatisticType],
-    },
-)
-
 GetInstancePortStatesRequestRequestTypeDef = TypedDict(
     "GetInstancePortStatesRequestRequestTypeDef",
     {
         "instanceName": str,
     },
 )
 
@@ -1866,27 +1788,14 @@
     {
         "pageToken": str,
         "includeDefaultKeyPair": bool,
     },
     total=False,
 )
 
-GetLoadBalancerMetricDataRequestRequestTypeDef = TypedDict(
-    "GetLoadBalancerMetricDataRequestRequestTypeDef",
-    {
-        "loadBalancerName": str,
-        "metricName": LoadBalancerMetricNameType,
-        "period": int,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-        "unit": MetricUnitType,
-        "statistics": Sequence[MetricStatisticType],
-    },
-)
-
 GetLoadBalancerRequestRequestTypeDef = TypedDict(
     "GetLoadBalancerRequestRequestTypeDef",
     {
         "loadBalancerName": str,
     },
 )
 
@@ -2043,38 +1952,14 @@
         "createdAt": datetime,
         "message": str,
         "eventCategories": List[str],
     },
     total=False,
 )
 
-_RequiredGetRelationalDatabaseLogEventsRequestRequestTypeDef = TypedDict(
-    "_RequiredGetRelationalDatabaseLogEventsRequestRequestTypeDef",
-    {
-        "relationalDatabaseName": str,
-        "logStreamName": str,
-    },
-)
-_OptionalGetRelationalDatabaseLogEventsRequestRequestTypeDef = TypedDict(
-    "_OptionalGetRelationalDatabaseLogEventsRequestRequestTypeDef",
-    {
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-        "startFromHead": bool,
-        "pageToken": str,
-    },
-    total=False,
-)
-
-class GetRelationalDatabaseLogEventsRequestRequestTypeDef(
-    _RequiredGetRelationalDatabaseLogEventsRequestRequestTypeDef,
-    _OptionalGetRelationalDatabaseLogEventsRequestRequestTypeDef,
-):
-    pass
-
 LogEventTypeDef = TypedDict(
     "LogEventTypeDef",
     {
         "createdAt": datetime,
         "message": str,
     },
     total=False,
@@ -2103,27 +1988,14 @@
 
 class GetRelationalDatabaseMasterUserPasswordRequestRequestTypeDef(
     _RequiredGetRelationalDatabaseMasterUserPasswordRequestRequestTypeDef,
     _OptionalGetRelationalDatabaseMasterUserPasswordRequestRequestTypeDef,
 ):
     pass
 
-GetRelationalDatabaseMetricDataRequestRequestTypeDef = TypedDict(
-    "GetRelationalDatabaseMetricDataRequestRequestTypeDef",
-    {
-        "relationalDatabaseName": str,
-        "metricName": RelationalDatabaseMetricNameType,
-        "period": int,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-        "unit": MetricUnitType,
-        "statistics": Sequence[MetricStatisticType],
-    },
-)
-
 _RequiredGetRelationalDatabaseParametersRequestRequestTypeDef = TypedDict(
     "_RequiredGetRelationalDatabaseParametersRequestRequestTypeDef",
     {
         "relationalDatabaseName": str,
     },
 )
 _OptionalGetRelationalDatabaseParametersRequestRequestTypeDef = TypedDict(
@@ -3060,41 +2932,14 @@
 
 class CreateLoadBalancerTlsCertificateRequestRequestTypeDef(
     _RequiredCreateLoadBalancerTlsCertificateRequestRequestTypeDef,
     _OptionalCreateLoadBalancerTlsCertificateRequestRequestTypeDef,
 ):
     pass
 
-_RequiredCreateRelationalDatabaseFromSnapshotRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateRelationalDatabaseFromSnapshotRequestRequestTypeDef",
-    {
-        "relationalDatabaseName": str,
-    },
-)
-_OptionalCreateRelationalDatabaseFromSnapshotRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateRelationalDatabaseFromSnapshotRequestRequestTypeDef",
-    {
-        "availabilityZone": str,
-        "publiclyAccessible": bool,
-        "relationalDatabaseSnapshotName": str,
-        "relationalDatabaseBundleId": str,
-        "sourceRelationalDatabaseName": str,
-        "restoreTime": Union[datetime, str],
-        "useLatestRestorableTime": bool,
-        "tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-class CreateRelationalDatabaseFromSnapshotRequestRequestTypeDef(
-    _RequiredCreateRelationalDatabaseFromSnapshotRequestRequestTypeDef,
-    _OptionalCreateRelationalDatabaseFromSnapshotRequestRequestTypeDef,
-):
-    pass
-
 _RequiredCreateRelationalDatabaseRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRelationalDatabaseRequestRequestTypeDef",
     {
         "relationalDatabaseName": str,
         "relationalDatabaseBlueprintId": str,
         "relationalDatabaseBundleId": str,
         "masterDatabaseName": str,
@@ -3335,14 +3180,15 @@
     "RegisterContainerImageResultTypeDef",
     {
         "containerImage": ContainerImageTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ContainerUnionTypeDef = Union[ContainerTypeDef, ContainerOutputTypeDef]
 PrivateRegistryAccessRequestTypeDef = TypedDict(
     "PrivateRegistryAccessRequestTypeDef",
     {
         "ecrImagePullerRole": ContainerServiceECRImagePullerRoleRequestTypeDef,
     },
     total=False,
 )
@@ -3447,14 +3293,174 @@
         "percentageComplete": int,
         "failureReason": str,
         "sessions": List[SessionTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateRelationalDatabaseFromSnapshotRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateRelationalDatabaseFromSnapshotRequestRequestTypeDef",
+    {
+        "relationalDatabaseName": str,
+    },
+)
+_OptionalCreateRelationalDatabaseFromSnapshotRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateRelationalDatabaseFromSnapshotRequestRequestTypeDef",
+    {
+        "availabilityZone": str,
+        "publiclyAccessible": bool,
+        "relationalDatabaseSnapshotName": str,
+        "relationalDatabaseBundleId": str,
+        "sourceRelationalDatabaseName": str,
+        "restoreTime": TimestampTypeDef,
+        "useLatestRestorableTime": bool,
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class CreateRelationalDatabaseFromSnapshotRequestRequestTypeDef(
+    _RequiredCreateRelationalDatabaseFromSnapshotRequestRequestTypeDef,
+    _OptionalCreateRelationalDatabaseFromSnapshotRequestRequestTypeDef,
+):
+    pass
+
+GetBucketMetricDataRequestRequestTypeDef = TypedDict(
+    "GetBucketMetricDataRequestRequestTypeDef",
+    {
+        "bucketName": str,
+        "metricName": BucketMetricNameType,
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+        "period": int,
+        "statistics": Sequence[MetricStatisticType],
+        "unit": MetricUnitType,
+    },
+)
+
+_RequiredGetContainerLogRequestRequestTypeDef = TypedDict(
+    "_RequiredGetContainerLogRequestRequestTypeDef",
+    {
+        "serviceName": str,
+        "containerName": str,
+    },
+)
+_OptionalGetContainerLogRequestRequestTypeDef = TypedDict(
+    "_OptionalGetContainerLogRequestRequestTypeDef",
+    {
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+        "filterPattern": str,
+        "pageToken": str,
+    },
+    total=False,
+)
+
+class GetContainerLogRequestRequestTypeDef(
+    _RequiredGetContainerLogRequestRequestTypeDef, _OptionalGetContainerLogRequestRequestTypeDef
+):
+    pass
+
+GetContainerServiceMetricDataRequestRequestTypeDef = TypedDict(
+    "GetContainerServiceMetricDataRequestRequestTypeDef",
+    {
+        "serviceName": str,
+        "metricName": ContainerServiceMetricNameType,
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+        "period": int,
+        "statistics": Sequence[MetricStatisticType],
+    },
+)
+
+GetCostEstimateRequestRequestTypeDef = TypedDict(
+    "GetCostEstimateRequestRequestTypeDef",
+    {
+        "resourceName": str,
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+    },
+)
+
+GetDistributionMetricDataRequestRequestTypeDef = TypedDict(
+    "GetDistributionMetricDataRequestRequestTypeDef",
+    {
+        "distributionName": str,
+        "metricName": DistributionMetricNameType,
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+        "period": int,
+        "unit": MetricUnitType,
+        "statistics": Sequence[MetricStatisticType],
+    },
+)
+
+GetInstanceMetricDataRequestRequestTypeDef = TypedDict(
+    "GetInstanceMetricDataRequestRequestTypeDef",
+    {
+        "instanceName": str,
+        "metricName": InstanceMetricNameType,
+        "period": int,
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+        "unit": MetricUnitType,
+        "statistics": Sequence[MetricStatisticType],
+    },
+)
+
+GetLoadBalancerMetricDataRequestRequestTypeDef = TypedDict(
+    "GetLoadBalancerMetricDataRequestRequestTypeDef",
+    {
+        "loadBalancerName": str,
+        "metricName": LoadBalancerMetricNameType,
+        "period": int,
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+        "unit": MetricUnitType,
+        "statistics": Sequence[MetricStatisticType],
+    },
+)
+
+_RequiredGetRelationalDatabaseLogEventsRequestRequestTypeDef = TypedDict(
+    "_RequiredGetRelationalDatabaseLogEventsRequestRequestTypeDef",
+    {
+        "relationalDatabaseName": str,
+        "logStreamName": str,
+    },
+)
+_OptionalGetRelationalDatabaseLogEventsRequestRequestTypeDef = TypedDict(
+    "_OptionalGetRelationalDatabaseLogEventsRequestRequestTypeDef",
+    {
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+        "startFromHead": bool,
+        "pageToken": str,
+    },
+    total=False,
+)
+
+class GetRelationalDatabaseLogEventsRequestRequestTypeDef(
+    _RequiredGetRelationalDatabaseLogEventsRequestRequestTypeDef,
+    _OptionalGetRelationalDatabaseLogEventsRequestRequestTypeDef,
+):
+    pass
+
+GetRelationalDatabaseMetricDataRequestRequestTypeDef = TypedDict(
+    "GetRelationalDatabaseMetricDataRequestRequestTypeDef",
+    {
+        "relationalDatabaseName": str,
+        "metricName": RelationalDatabaseMetricNameType,
+        "period": int,
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+        "unit": MetricUnitType,
+        "statistics": Sequence[MetricStatisticType],
+    },
+)
+
 InstanceSnapshotInfoTypeDef = TypedDict(
     "InstanceSnapshotInfoTypeDef",
     {
         "fromBundleId": str,
         "fromBlueprintId": str,
         "fromDiskInfo": List[DiskInfoTypeDef],
     },
@@ -3465,14 +3471,15 @@
     "GetDistributionBundlesResultTypeDef",
     {
         "bundles": List[DistributionBundleTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DomainEntryUnionTypeDef = Union[DomainEntryTypeDef, DomainEntryOutputTypeDef]
 DomainValidationRecordTypeDef = TypedDict(
     "DomainValidationRecordTypeDef",
     {
         "domainName": str,
         "resourceRecord": ResourceRecordTypeDef,
         "dnsRecordCreationState": DnsRecordCreationStateTypeDef,
         "validationStatus": CertificateDomainValidationStatusType,
@@ -4940,14 +4947,15 @@
         "ableToUpdateBundle": bool,
         "ipAddressType": IpAddressTypeType,
         "tags": List[TagTypeDef],
     },
     total=False,
 )
 
+CacheSettingsUnionTypeDef = Union[CacheSettingsTypeDef, CacheSettingsOutputTypeDef]
 _RequiredCreateDistributionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDistributionRequestRequestTypeDef",
     {
         "distributionName": str,
         "origin": InputOriginTypeDef,
         "defaultCacheBehavior": CacheBehaviorTypeDef,
         "bundleId": str,
@@ -5053,15 +5061,15 @@
     {
         "serviceName": str,
     },
 )
 _OptionalCreateContainerServiceDeploymentRequestRequestTypeDef = TypedDict(
     "_OptionalCreateContainerServiceDeploymentRequestRequestTypeDef",
     {
-        "containers": Mapping[str, Union[ContainerTypeDef, ContainerOutputTypeDef]],
+        "containers": Mapping[str, ContainerUnionTypeDef],
         "publicEndpoint": EndpointRequestTypeDef,
     },
     total=False,
 )
 
 class CreateContainerServiceDeploymentRequestRequestTypeDef(
     _RequiredCreateContainerServiceDeploymentRequestRequestTypeDef,
```

### Comparing `mypy-boto3-lightsail-1.28.15.post1/mypy_boto3_lightsail.egg-info/PKG-INFO` & `mypy-boto3-lightsail-1.28.16/mypy_boto3_lightsail.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lightsail
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Lightsail 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.Lightsail 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 lightsail type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 lightsail type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lightsail.svg?color=blue)](https://pypi.org/project/mypy-boto3-lightsail)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lightsail)](https://pepy.tech/project/mypy-boto3-lightsail)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Lightsail 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail)
+[boto3.Lightsail 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail)
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
 [mypy-boto3-lightsail docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/).
 
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
@@ -464,20 +464,20 @@
 )
 
 
 def check_value(value: AccessDirectionType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_lightsail.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_lightsail.type_defs import (
     AccessKeyLastUsedTypeDef,
     AccessRulesTypeDef,
     AccountLevelBpaSyncTypeDef,
     AutoSnapshotAddOnRequestTypeDef,
@@ -527,14 +527,15 @@
     InstanceEntryTypeDef,
     CreateContactMethodRequestRequestTypeDef,
     InputOriginTypeDef,
     DomainEntryTypeDef,
     CreateGUISessionAccessDetailsRequestRequestTypeDef,
     SessionTypeDef,
     DiskMapTypeDef,
+    TimestampTypeDef,
     DeleteAlarmRequestRequestTypeDef,
     DeleteAutoSnapshotRequestRequestTypeDef,
     DeleteBucketAccessKeyRequestRequestTypeDef,
     DeleteBucketRequestRequestTypeDef,
     DeleteCertificateRequestRequestTypeDef,
     DeleteContactMethodRequestRequestTypeDef,
     DeleteContainerImageRequestRequestTypeDef,
@@ -567,50 +568,43 @@
     PaginatorConfigTypeDef,
     GetActiveNamesRequestRequestTypeDef,
     GetAlarmsRequestRequestTypeDef,
     GetAutoSnapshotsRequestRequestTypeDef,
     GetBlueprintsRequestRequestTypeDef,
     GetBucketAccessKeysRequestRequestTypeDef,
     GetBucketBundlesRequestRequestTypeDef,
-    GetBucketMetricDataRequestRequestTypeDef,
     MetricDatapointTypeDef,
     GetBucketsRequestRequestTypeDef,
     GetBundlesRequestRequestTypeDef,
     GetCertificatesRequestRequestTypeDef,
     GetCloudFormationStackRecordsRequestRequestTypeDef,
     GetContactMethodsRequestRequestTypeDef,
     GetContainerImagesRequestRequestTypeDef,
-    GetContainerLogRequestRequestTypeDef,
     GetContainerServiceDeploymentsRequestRequestTypeDef,
-    GetContainerServiceMetricDataRequestRequestTypeDef,
     GetContainerServicesRequestRequestTypeDef,
-    GetCostEstimateRequestRequestTypeDef,
     GetDiskRequestRequestTypeDef,
     GetDiskSnapshotRequestRequestTypeDef,
     GetDiskSnapshotsRequestRequestTypeDef,
     GetDisksRequestRequestTypeDef,
     GetDistributionLatestCacheResetRequestRequestTypeDef,
-    GetDistributionMetricDataRequestRequestTypeDef,
     GetDistributionsRequestRequestTypeDef,
     GetDomainRequestRequestTypeDef,
     GetDomainsRequestRequestTypeDef,
     GetExportSnapshotRecordsRequestRequestTypeDef,
     GetInstanceAccessDetailsRequestRequestTypeDef,
-    GetInstanceMetricDataRequestRequestTypeDef,
     GetInstancePortStatesRequestRequestTypeDef,
     InstancePortStateTypeDef,
     GetInstanceRequestRequestTypeDef,
     GetInstanceSnapshotRequestRequestTypeDef,
     GetInstanceSnapshotsRequestRequestTypeDef,
     GetInstanceStateRequestRequestTypeDef,
     InstanceStateTypeDef,
     GetInstancesRequestRequestTypeDef,
     GetKeyPairRequestRequestTypeDef,
     GetKeyPairsRequestRequestTypeDef,
-    GetLoadBalancerMetricDataRequestRequestTypeDef,
     GetLoadBalancerRequestRequestTypeDef,
     GetLoadBalancerTlsCertificatesRequestRequestTypeDef,
     GetLoadBalancerTlsPoliciesRequestRequestTypeDef,
     LoadBalancerTlsPolicyTypeDef,
     GetLoadBalancersRequestRequestTypeDef,
     GetOperationRequestRequestTypeDef,
     GetOperationsForResourceRequestRequestTypeDef,
@@ -618,19 +612,17 @@
     GetRegionsRequestRequestTypeDef,
     GetRelationalDatabaseBlueprintsRequestRequestTypeDef,
     RelationalDatabaseBlueprintTypeDef,
     GetRelationalDatabaseBundlesRequestRequestTypeDef,
     RelationalDatabaseBundleTypeDef,
     GetRelationalDatabaseEventsRequestRequestTypeDef,
     RelationalDatabaseEventTypeDef,
-    GetRelationalDatabaseLogEventsRequestRequestTypeDef,
     LogEventTypeDef,
     GetRelationalDatabaseLogStreamsRequestRequestTypeDef,
     GetRelationalDatabaseMasterUserPasswordRequestRequestTypeDef,
-    GetRelationalDatabaseMetricDataRequestRequestTypeDef,
     GetRelationalDatabaseParametersRequestRequestTypeDef,
     RelationalDatabaseParameterTypeDef,
     GetRelationalDatabaseRequestRequestTypeDef,
     GetRelationalDatabaseSnapshotRequestRequestTypeDef,
     GetRelationalDatabaseSnapshotsRequestRequestTypeDef,
     GetRelationalDatabasesRequestRequestTypeDef,
     GetStaticIpRequestRequestTypeDef,
@@ -697,15 +689,14 @@
     CreateCertificateRequestRequestTypeDef,
     CreateDiskSnapshotRequestRequestTypeDef,
     CreateDomainRequestRequestTypeDef,
     CreateInstanceSnapshotRequestRequestTypeDef,
     CreateKeyPairRequestRequestTypeDef,
     CreateLoadBalancerRequestRequestTypeDef,
     CreateLoadBalancerTlsCertificateRequestRequestTypeDef,
-    CreateRelationalDatabaseFromSnapshotRequestRequestTypeDef,
     CreateRelationalDatabaseRequestRequestTypeDef,
     CreateRelationalDatabaseSnapshotRequestRequestTypeDef,
     DiskSnapshotTypeDef,
     DiskTypeDef,
     KeyPairTypeDef,
     RelationalDatabaseSnapshotTypeDef,
     TagResourceRequestRequestTypeDef,
@@ -714,28 +705,40 @@
     CacheSettingsTypeDef,
     CloseInstancePublicPortsRequestRequestTypeDef,
     OpenInstancePublicPortsRequestRequestTypeDef,
     PutInstancePublicPortsRequestRequestTypeDef,
     CloudFormationStackRecordTypeDef,
     GetContainerImagesResultTypeDef,
     RegisterContainerImageResultTypeDef,
+    ContainerUnionTypeDef,
     PrivateRegistryAccessRequestTypeDef,
     PrivateRegistryAccessTypeDef,
     ContainerServiceEndpointTypeDef,
     EndpointRequestTypeDef,
     GetContainerLogResultTypeDef,
     GetContainerServicePowersResultTypeDef,
     CreateContainerServiceRegistryLoginResultTypeDef,
     CreateCloudFormationStackRequestRequestTypeDef,
     CreateDomainEntryRequestRequestTypeDef,
     DeleteDomainEntryRequestRequestTypeDef,
     UpdateDomainEntryRequestRequestTypeDef,
     CreateGUISessionAccessDetailsResultTypeDef,
+    CreateRelationalDatabaseFromSnapshotRequestRequestTypeDef,
+    GetBucketMetricDataRequestRequestTypeDef,
+    GetContainerLogRequestRequestTypeDef,
+    GetContainerServiceMetricDataRequestRequestTypeDef,
+    GetCostEstimateRequestRequestTypeDef,
+    GetDistributionMetricDataRequestRequestTypeDef,
+    GetInstanceMetricDataRequestRequestTypeDef,
+    GetLoadBalancerMetricDataRequestRequestTypeDef,
+    GetRelationalDatabaseLogEventsRequestRequestTypeDef,
+    GetRelationalDatabaseMetricDataRequestRequestTypeDef,
     InstanceSnapshotInfoTypeDef,
     GetDistributionBundlesResultTypeDef,
+    DomainEntryUnionTypeDef,
     DomainValidationRecordTypeDef,
     EstimateByTimeTypeDef,
     GetActiveNamesRequestGetActiveNamesPaginateTypeDef,
     GetBlueprintsRequestGetBlueprintsPaginateTypeDef,
     GetBundlesRequestGetBundlesPaginateTypeDef,
     GetCloudFormationStackRecordsRequestGetCloudFormationStackRecordsPaginateTypeDef,
     GetDiskSnapshotsRequestGetDiskSnapshotsPaginateTypeDef,
@@ -882,14 +885,15 @@
     InstanceSnapshotTypeDef,
     CreateKeyPairResultTypeDef,
     GetKeyPairResultTypeDef,
     GetKeyPairsResultTypeDef,
     GetRelationalDatabaseSnapshotResultTypeDef,
     GetRelationalDatabaseSnapshotsResultTypeDef,
     LightsailDistributionTypeDef,
+    CacheSettingsUnionTypeDef,
     CreateDistributionRequestRequestTypeDef,
     UpdateDistributionRequestRequestTypeDef,
     GetCloudFormationStackRecordsResultTypeDef,
     UpdateContainerServiceRequestRequestTypeDef,
     ContainerServiceDeploymentTypeDef,
     ContainerServiceDeploymentRequestTypeDef,
     CreateContainerServiceDeploymentRequestRequestTypeDef,
@@ -927,15 +931,15 @@
     CertificateSummaryTypeDef,
     GetCostEstimateResultTypeDef,
     CreateCertificateResultTypeDef,
     GetCertificatesResultTypeDef,
 )
 
 
-def get_structure() -> AccessKeyLastUsedTypeDef:
+def get_value() -> AccessKeyLastUsedTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-lightsail-1.28.15.post1/mypy_boto3_lightsail.egg-info/SOURCES.txt` & `mypy-boto3-lightsail-1.28.16/mypy_boto3_lightsail.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lightsail-1.28.15.post1/setup.py` & `mypy-boto3-lightsail-1.28.16/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-lightsail",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_lightsail"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Lightsail 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.Lightsail 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 lightsail type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 lightsail type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_lightsail": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

