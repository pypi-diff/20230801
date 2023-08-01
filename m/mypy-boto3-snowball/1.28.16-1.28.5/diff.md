# Comparing `tmp/mypy-boto3-snowball-1.28.16.tar.gz` & `tmp/mypy-boto3-snowball-1.28.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-snowball-1.28.16.tar", last modified: Tue Aug  1 11:37:54 2023, max compression
+gzip compressed data, was "mypy-boto3-snowball-1.28.5.tar", last modified: Tue Jul 18 19:32:41 2023, max compression
```

## Comparing `mypy-boto3-snowball-1.28.16.tar` & `mypy-boto3-snowball-1.28.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:54.932721 mypy-boto3-snowball-1.28.16/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:33:22.000000 mypy-boto3-snowball-1.28.16/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17189 2023-08-01 11:37:54.932721 mypy-boto3-snowball-1.28.16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15701 2023-08-01 11:33:22.000000 mypy-boto3-snowball-1.28.16/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:54.924721 mypy-boto3-snowball-1.28.16/mypy_boto3_snowball/
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-08-01 11:33:22.000000 mypy-boto3-snowball-1.28.16/mypy_boto3_snowball/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-08-01 11:33:22.000000 mypy-boto3-snowball-1.28.16/mypy_boto3_snowball/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-08-01 11:33:22.000000 mypy-boto3-snowball-1.28.16/mypy_boto3_snowball/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24349 2023-08-01 11:33:23.000000 mypy-boto3-snowball-1.28.16/mypy_boto3_snowball/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    24309 2023-08-01 11:33:23.000000 mypy-boto3-snowball-1.28.16/mypy_boto3_snowball/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10678 2023-08-01 11:33:23.000000 mypy-boto3-snowball-1.28.16/mypy_boto3_snowball/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10676 2023-08-01 11:33:23.000000 mypy-boto3-snowball-1.28.16/mypy_boto3_snowball/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-08-01 11:33:23.000000 mypy-boto3-snowball-1.28.16/mypy_boto3_snowball/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7017 2023-08-01 11:33:23.000000 mypy-boto3-snowball-1.28.16/mypy_boto3_snowball/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:33:22.000000 mypy-boto3-snowball-1.28.16/mypy_boto3_snowball/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    30675 2023-08-01 11:33:24.000000 mypy-boto3-snowball-1.28.16/mypy_boto3_snowball/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    30654 2023-08-01 11:33:23.000000 mypy-boto3-snowball-1.28.16/mypy_boto3_snowball/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:33:22.000000 mypy-boto3-snowball-1.28.16/mypy_boto3_snowball/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:54.932721 mypy-boto3-snowball-1.28.16/mypy_boto3_snowball.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17189 2023-08-01 11:37:54.000000 mypy-boto3-snowball-1.28.16/mypy_boto3_snowball.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-08-01 11:37:54.000000 mypy-boto3-snowball-1.28.16/mypy_boto3_snowball.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:54.000000 mypy-boto3-snowball-1.28.16/mypy_boto3_snowball.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:54.000000 mypy-boto3-snowball-1.28.16/mypy_boto3_snowball.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:54.000000 mypy-boto3-snowball-1.28.16/mypy_boto3_snowball.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-01 11:37:54.000000 mypy-boto3-snowball-1.28.16/mypy_boto3_snowball.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:54.932721 mypy-boto3-snowball-1.28.16/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-08-01 11:33:22.000000 mypy-boto3-snowball-1.28.16/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:32:41.758719 mypy-boto3-snowball-1.28.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-18 19:32:27.000000 mypy-boto3-snowball-1.28.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17767 2023-07-18 19:32:41.754719 mypy-boto3-snowball-1.28.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16278 2023-07-18 19:32:27.000000 mypy-boto3-snowball-1.28.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:32:41.750719 mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-07-18 19:32:27.000000 mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-18 19:32:27.000000 mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-18 19:32:27.000000 mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24284 2023-07-18 19:32:27.000000 mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24244 2023-07-18 19:32:27.000000 mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10600 2023-07-18 19:32:27.000000 mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10598 2023-07-18 19:32:27.000000 mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7037 2023-07-18 19:32:27.000000 mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-07-18 19:32:27.000000 mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 19:32:27.000000 mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    34275 2023-07-18 19:32:29.000000 mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34254 2023-07-18 19:32:28.000000 mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-18 19:32:27.000000 mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:32:41.750719 mypy-boto3-snowball-1.28.5/mypy_boto3_snowball.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17767 2023-07-18 19:32:41.000000 mypy-boto3-snowball-1.28.5/mypy_boto3_snowball.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-18 19:32:41.000000 mypy-boto3-snowball-1.28.5/mypy_boto3_snowball.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 19:32:41.000000 mypy-boto3-snowball-1.28.5/mypy_boto3_snowball.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 19:32:41.000000 mypy-boto3-snowball-1.28.5/mypy_boto3_snowball.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-18 19:32:41.000000 mypy-boto3-snowball-1.28.5/mypy_boto3_snowball.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-18 19:32:41.000000 mypy-boto3-snowball-1.28.5/mypy_boto3_snowball.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 19:32:41.758719 mypy-boto3-snowball-1.28.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-18 19:32:27.000000 mypy-boto3-snowball-1.28.5/setup.py
```

### Comparing `mypy-boto3-snowball-1.28.16/LICENSE` & `mypy-boto3-snowball-1.28.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-snowball-1.28.16/PKG-INFO` & `mypy-boto3-snowball-1.28.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-snowball
-Version: 1.28.16
-Summary: Type annotations for boto3.Snowball 1.28.16 service generated with mypy-boto3-builder 7.17.1
+Version: 1.28.5
+Summary: Type annotations for boto3.Snowball 1.28.5 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 snowball type-annotations botocore mypy typeshed autocomplete
+Keywords: boto3 snowball type-annotations boto3-stubs mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-snowball"></a>
 
 # mypy-boto3-snowball
 
 [![PyPI - mypy-boto3-snowball](https://img.shields.io/pypi/v/mypy-boto3-snowball.svg?color=blue)](https://pypi.org/project/mypy-boto3-snowball)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-snowball.svg?color=blue)](https://pypi.org/project/mypy-boto3-snowball)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-snowball)](https://pepy.tech/project/mypy-boto3-snowball)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-snowball?color=blue)](https://pypistats.org/packages/mypy-boto3-snowball)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Snowball 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball)
+[boto3.Snowball 1.28.5](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball)
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
 [mypy-boto3-snowball docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/).
 
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
@@ -348,123 +348,136 @@
 )
 
 
 def check_value(value: AddressTypeType) -> bool:
     ...
 ```
 
-<a id="type-definitions"></a>
+<a id="typed-dictionaries"></a>
 
-### Type definitions
+### Typed dictionaries
 
 `mypy_boto3_snowball.type_defs` module contains structures and shapes assembled
-to typed dictionaries and unions for additional type checking.
+to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_snowball.type_defs import (
+    AddressOutputTypeDef,
     AddressTypeDef,
     CancelClusterRequestRequestTypeDef,
     CancelJobRequestRequestTypeDef,
     ClusterListEntryTypeDef,
     NotificationOutputTypeDef,
     CompatibleImageTypeDef,
-    ResponseMetadataTypeDef,
+    CreateAddressResultTypeDef,
     NotificationTypeDef,
     JobListEntryTypeDef,
+    PickupDetailsTypeDef,
+    CreateJobResultTypeDef,
     CreateLongTermPricingRequestRequestTypeDef,
+    CreateLongTermPricingResultTypeDef,
     CreateReturnShippingLabelRequestRequestTypeDef,
+    CreateReturnShippingLabelResultTypeDef,
     DataTransferTypeDef,
+    ServiceVersionOutputTypeDef,
     ServiceVersionTypeDef,
     DescribeAddressRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeAddressesRequestDescribeAddressesPaginateTypeDef,
     DescribeAddressesRequestRequestTypeDef,
     DescribeClusterRequestRequestTypeDef,
     DescribeJobRequestRequestTypeDef,
     DescribeReturnShippingLabelRequestRequestTypeDef,
+    DescribeReturnShippingLabelResultTypeDef,
+    EKSOnDeviceServiceConfigurationOutputTypeDef,
     EKSOnDeviceServiceConfigurationTypeDef,
+    Ec2AmiResourceOutputTypeDef,
     Ec2AmiResourceTypeDef,
+    EventTriggerDefinitionOutputTypeDef,
     EventTriggerDefinitionTypeDef,
     GetJobManifestRequestRequestTypeDef,
+    GetJobManifestResultTypeDef,
     GetJobUnlockCodeRequestRequestTypeDef,
+    GetJobUnlockCodeResultTypeDef,
+    GetSnowballUsageResultTypeDef,
     GetSoftwareUpdatesRequestRequestTypeDef,
+    GetSoftwareUpdatesResultTypeDef,
+    INDTaxDocumentsOutputTypeDef,
     INDTaxDocumentsTypeDef,
     JobLogsTypeDef,
     PickupDetailsOutputTypeDef,
+    KeyRangeOutputTypeDef,
     KeyRangeTypeDef,
+    ListClusterJobsRequestListClusterJobsPaginateTypeDef,
     ListClusterJobsRequestRequestTypeDef,
+    ListClustersRequestListClustersPaginateTypeDef,
     ListClustersRequestRequestTypeDef,
+    ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef,
     ListCompatibleImagesRequestRequestTypeDef,
+    ListJobsRequestListJobsPaginateTypeDef,
     ListJobsRequestRequestTypeDef,
+    ListLongTermPricingRequestListLongTermPricingPaginateTypeDef,
     ListLongTermPricingRequestRequestTypeDef,
     LongTermPricingListEntryTypeDef,
     ListPickupLocationsRequestRequestTypeDef,
+    NFSOnDeviceServiceConfigurationOutputTypeDef,
     NFSOnDeviceServiceConfigurationTypeDef,
+    S3OnDeviceServiceConfigurationOutputTypeDef,
+    TGWOnDeviceServiceConfigurationOutputTypeDef,
     S3OnDeviceServiceConfigurationTypeDef,
     TGWOnDeviceServiceConfigurationTypeDef,
-    TimestampTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
+    TargetOnDeviceServiceOutputTypeDef,
     TargetOnDeviceServiceTypeDef,
     ShipmentTypeDef,
+    WirelessConnectionOutputTypeDef,
     WirelessConnectionTypeDef,
     UpdateJobShipmentStateRequestRequestTypeDef,
     UpdateLongTermPricingRequestRequestTypeDef,
-    CreateAddressRequestRequestTypeDef,
-    CreateAddressResultTypeDef,
-    CreateJobResultTypeDef,
-    CreateLongTermPricingResultTypeDef,
-    CreateReturnShippingLabelResultTypeDef,
     DescribeAddressResultTypeDef,
     DescribeAddressesResultTypeDef,
-    DescribeReturnShippingLabelResultTypeDef,
-    GetJobManifestResultTypeDef,
-    GetJobUnlockCodeResultTypeDef,
-    GetSnowballUsageResultTypeDef,
-    GetSoftwareUpdatesResultTypeDef,
+    ListPickupLocationsResultTypeDef,
+    CreateAddressRequestRequestTypeDef,
     ListClustersResultTypeDef,
     ListCompatibleImagesResultTypeDef,
-    ListPickupLocationsResultTypeDef,
-    NotificationUnionTypeDef,
     CreateClusterResultTypeDef,
     ListClusterJobsResultTypeDef,
     ListJobsResultTypeDef,
+    DependentServiceOutputTypeDef,
     DependentServiceTypeDef,
-    DescribeAddressesRequestDescribeAddressesPaginateTypeDef,
-    ListClusterJobsRequestListClusterJobsPaginateTypeDef,
-    ListClustersRequestListClustersPaginateTypeDef,
-    ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef,
-    ListJobsRequestListJobsPaginateTypeDef,
-    ListLongTermPricingRequestListLongTermPricingPaginateTypeDef,
     LambdaResourceOutputTypeDef,
     LambdaResourceTypeDef,
+    TaxDocumentsOutputTypeDef,
     TaxDocumentsTypeDef,
     ListLongTermPricingResultTypeDef,
+    OnDeviceServiceConfigurationOutputTypeDef,
     OnDeviceServiceConfigurationTypeDef,
-    PickupDetailsTypeDef,
     S3ResourceOutputTypeDef,
     S3ResourceTypeDef,
     ShippingDetailsTypeDef,
+    SnowconeDeviceConfigurationOutputTypeDef,
     SnowconeDeviceConfigurationTypeDef,
-    ListServiceVersionsRequestRequestTypeDef,
     ListServiceVersionsResultTypeDef,
-    PickupDetailsUnionTypeDef,
+    ListServiceVersionsRequestRequestTypeDef,
     JobResourceOutputTypeDef,
     JobResourceTypeDef,
+    DeviceConfigurationOutputTypeDef,
     DeviceConfigurationTypeDef,
     ClusterMetadataTypeDef,
     CreateClusterRequestRequestTypeDef,
-    JobResourceUnionTypeDef,
     UpdateClusterRequestRequestTypeDef,
     UpdateJobRequestRequestTypeDef,
-    CreateJobRequestRequestTypeDef,
     JobMetadataTypeDef,
+    CreateJobRequestRequestTypeDef,
     DescribeClusterResultTypeDef,
     DescribeJobResultTypeDef,
 )
 
 
-def get_value() -> AddressTypeDef:
+def get_structure() -> AddressOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-snowball-1.28.16/README.md` & `mypy-boto3-snowball-1.28.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-snowball"></a>
 
 # mypy-boto3-snowball
 
 [![PyPI - mypy-boto3-snowball](https://img.shields.io/pypi/v/mypy-boto3-snowball.svg?color=blue)](https://pypi.org/project/mypy-boto3-snowball)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-snowball.svg?color=blue)](https://pypi.org/project/mypy-boto3-snowball)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-snowball)](https://pepy.tech/project/mypy-boto3-snowball)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-snowball?color=blue)](https://pypistats.org/packages/mypy-boto3-snowball)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Snowball 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball)
+[boto3.Snowball 1.28.5](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball)
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
 [mypy-boto3-snowball docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/).
 
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
@@ -316,123 +316,136 @@
 )
 
 
 def check_value(value: AddressTypeType) -> bool:
     ...
 ```
 
-<a id="type-definitions"></a>
+<a id="typed-dictionaries"></a>
 
-### Type definitions
+### Typed dictionaries
 
 `mypy_boto3_snowball.type_defs` module contains structures and shapes assembled
-to typed dictionaries and unions for additional type checking.
+to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_snowball.type_defs import (
+    AddressOutputTypeDef,
     AddressTypeDef,
     CancelClusterRequestRequestTypeDef,
     CancelJobRequestRequestTypeDef,
     ClusterListEntryTypeDef,
     NotificationOutputTypeDef,
     CompatibleImageTypeDef,
-    ResponseMetadataTypeDef,
+    CreateAddressResultTypeDef,
     NotificationTypeDef,
     JobListEntryTypeDef,
+    PickupDetailsTypeDef,
+    CreateJobResultTypeDef,
     CreateLongTermPricingRequestRequestTypeDef,
+    CreateLongTermPricingResultTypeDef,
     CreateReturnShippingLabelRequestRequestTypeDef,
+    CreateReturnShippingLabelResultTypeDef,
     DataTransferTypeDef,
+    ServiceVersionOutputTypeDef,
     ServiceVersionTypeDef,
     DescribeAddressRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeAddressesRequestDescribeAddressesPaginateTypeDef,
     DescribeAddressesRequestRequestTypeDef,
     DescribeClusterRequestRequestTypeDef,
     DescribeJobRequestRequestTypeDef,
     DescribeReturnShippingLabelRequestRequestTypeDef,
+    DescribeReturnShippingLabelResultTypeDef,
+    EKSOnDeviceServiceConfigurationOutputTypeDef,
     EKSOnDeviceServiceConfigurationTypeDef,
+    Ec2AmiResourceOutputTypeDef,
     Ec2AmiResourceTypeDef,
+    EventTriggerDefinitionOutputTypeDef,
     EventTriggerDefinitionTypeDef,
     GetJobManifestRequestRequestTypeDef,
+    GetJobManifestResultTypeDef,
     GetJobUnlockCodeRequestRequestTypeDef,
+    GetJobUnlockCodeResultTypeDef,
+    GetSnowballUsageResultTypeDef,
     GetSoftwareUpdatesRequestRequestTypeDef,
+    GetSoftwareUpdatesResultTypeDef,
+    INDTaxDocumentsOutputTypeDef,
     INDTaxDocumentsTypeDef,
     JobLogsTypeDef,
     PickupDetailsOutputTypeDef,
+    KeyRangeOutputTypeDef,
     KeyRangeTypeDef,
+    ListClusterJobsRequestListClusterJobsPaginateTypeDef,
     ListClusterJobsRequestRequestTypeDef,
+    ListClustersRequestListClustersPaginateTypeDef,
     ListClustersRequestRequestTypeDef,
+    ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef,
     ListCompatibleImagesRequestRequestTypeDef,
+    ListJobsRequestListJobsPaginateTypeDef,
     ListJobsRequestRequestTypeDef,
+    ListLongTermPricingRequestListLongTermPricingPaginateTypeDef,
     ListLongTermPricingRequestRequestTypeDef,
     LongTermPricingListEntryTypeDef,
     ListPickupLocationsRequestRequestTypeDef,
+    NFSOnDeviceServiceConfigurationOutputTypeDef,
     NFSOnDeviceServiceConfigurationTypeDef,
+    S3OnDeviceServiceConfigurationOutputTypeDef,
+    TGWOnDeviceServiceConfigurationOutputTypeDef,
     S3OnDeviceServiceConfigurationTypeDef,
     TGWOnDeviceServiceConfigurationTypeDef,
-    TimestampTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
+    TargetOnDeviceServiceOutputTypeDef,
     TargetOnDeviceServiceTypeDef,
     ShipmentTypeDef,
+    WirelessConnectionOutputTypeDef,
     WirelessConnectionTypeDef,
     UpdateJobShipmentStateRequestRequestTypeDef,
     UpdateLongTermPricingRequestRequestTypeDef,
-    CreateAddressRequestRequestTypeDef,
-    CreateAddressResultTypeDef,
-    CreateJobResultTypeDef,
-    CreateLongTermPricingResultTypeDef,
-    CreateReturnShippingLabelResultTypeDef,
     DescribeAddressResultTypeDef,
     DescribeAddressesResultTypeDef,
-    DescribeReturnShippingLabelResultTypeDef,
-    GetJobManifestResultTypeDef,
-    GetJobUnlockCodeResultTypeDef,
-    GetSnowballUsageResultTypeDef,
-    GetSoftwareUpdatesResultTypeDef,
+    ListPickupLocationsResultTypeDef,
+    CreateAddressRequestRequestTypeDef,
     ListClustersResultTypeDef,
     ListCompatibleImagesResultTypeDef,
-    ListPickupLocationsResultTypeDef,
-    NotificationUnionTypeDef,
     CreateClusterResultTypeDef,
     ListClusterJobsResultTypeDef,
     ListJobsResultTypeDef,
+    DependentServiceOutputTypeDef,
     DependentServiceTypeDef,
-    DescribeAddressesRequestDescribeAddressesPaginateTypeDef,
-    ListClusterJobsRequestListClusterJobsPaginateTypeDef,
-    ListClustersRequestListClustersPaginateTypeDef,
-    ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef,
-    ListJobsRequestListJobsPaginateTypeDef,
-    ListLongTermPricingRequestListLongTermPricingPaginateTypeDef,
     LambdaResourceOutputTypeDef,
     LambdaResourceTypeDef,
+    TaxDocumentsOutputTypeDef,
     TaxDocumentsTypeDef,
     ListLongTermPricingResultTypeDef,
+    OnDeviceServiceConfigurationOutputTypeDef,
     OnDeviceServiceConfigurationTypeDef,
-    PickupDetailsTypeDef,
     S3ResourceOutputTypeDef,
     S3ResourceTypeDef,
     ShippingDetailsTypeDef,
+    SnowconeDeviceConfigurationOutputTypeDef,
     SnowconeDeviceConfigurationTypeDef,
-    ListServiceVersionsRequestRequestTypeDef,
     ListServiceVersionsResultTypeDef,
-    PickupDetailsUnionTypeDef,
+    ListServiceVersionsRequestRequestTypeDef,
     JobResourceOutputTypeDef,
     JobResourceTypeDef,
+    DeviceConfigurationOutputTypeDef,
     DeviceConfigurationTypeDef,
     ClusterMetadataTypeDef,
     CreateClusterRequestRequestTypeDef,
-    JobResourceUnionTypeDef,
     UpdateClusterRequestRequestTypeDef,
     UpdateJobRequestRequestTypeDef,
-    CreateJobRequestRequestTypeDef,
     JobMetadataTypeDef,
+    CreateJobRequestRequestTypeDef,
     DescribeClusterResultTypeDef,
     DescribeJobResultTypeDef,
 )
 
 
-def get_value() -> AddressTypeDef:
+def get_structure() -> AddressOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-snowball-1.28.16/mypy_boto3_snowball/__init__.py` & `mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-snowball-1.28.16/mypy_boto3_snowball/__init__.pyi` & `mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-snowball-1.28.16/mypy_boto3_snowball/__main__.py` & `mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Snowball 1.28.16\nVersion:         1.28.16\nBuilder version:"
-        " 7.17.1\nDocs:           "
+        "Type annotations for boto3.Snowball 1.28.5\nVersion:         1.28.5\nBuilder version:"
+        " 7.15.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.16")
+    print("1.28.5")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-snowball-1.28.16/mypy_boto3_snowball/client.py` & `mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,25 +51,25 @@
     DescribeJobResultTypeDef,
     DescribeReturnShippingLabelResultTypeDef,
     DeviceConfigurationTypeDef,
     GetJobManifestResultTypeDef,
     GetJobUnlockCodeResultTypeDef,
     GetSnowballUsageResultTypeDef,
     GetSoftwareUpdatesResultTypeDef,
-    JobResourceUnionTypeDef,
+    JobResourceTypeDef,
     ListClusterJobsResultTypeDef,
     ListClustersResultTypeDef,
     ListCompatibleImagesResultTypeDef,
     ListJobsResultTypeDef,
     ListLongTermPricingResultTypeDef,
     ListPickupLocationsResultTypeDef,
     ListServiceVersionsResultTypeDef,
-    NotificationUnionTypeDef,
+    NotificationTypeDef,
     OnDeviceServiceConfigurationTypeDef,
-    PickupDetailsUnionTypeDef,
+    PickupDetailsTypeDef,
     TaxDocumentsTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -161,20 +161,20 @@
     def create_cluster(
         self,
         *,
         JobType: JobTypeType,
         AddressId: str,
         SnowballType: SnowballTypeType,
         ShippingOption: ShippingOptionType,
-        Resources: JobResourceUnionTypeDef = ...,
+        Resources: JobResourceTypeDef = ...,
         OnDeviceServiceConfiguration: OnDeviceServiceConfigurationTypeDef = ...,
         Description: str = ...,
         KmsKeyARN: str = ...,
         RoleARN: str = ...,
-        Notification: NotificationUnionTypeDef = ...,
+        Notification: NotificationTypeDef = ...,
         ForwardingAddressId: str = ...,
         TaxDocuments: TaxDocumentsTypeDef = ...,
         RemoteManagement: RemoteManagementType = ...,
         InitialClusterSize: int = ...,
         ForceCreateJobs: bool = ...,
         LongTermPricingIds: Sequence[str] = ...,
         SnowballCapacityPreference: SnowballCapacityType = ...
@@ -186,32 +186,32 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/client/#create_cluster)
         """
 
     def create_job(
         self,
         *,
         JobType: JobTypeType = ...,
-        Resources: JobResourceUnionTypeDef = ...,
+        Resources: JobResourceTypeDef = ...,
         OnDeviceServiceConfiguration: OnDeviceServiceConfigurationTypeDef = ...,
         Description: str = ...,
         AddressId: str = ...,
         KmsKeyARN: str = ...,
         RoleARN: str = ...,
         SnowballCapacityPreference: SnowballCapacityType = ...,
         ShippingOption: ShippingOptionType = ...,
-        Notification: NotificationUnionTypeDef = ...,
+        Notification: NotificationTypeDef = ...,
         ClusterId: str = ...,
         SnowballType: SnowballTypeType = ...,
         ForwardingAddressId: str = ...,
         TaxDocuments: TaxDocumentsTypeDef = ...,
         DeviceConfiguration: DeviceConfigurationTypeDef = ...,
         RemoteManagement: RemoteManagementType = ...,
         LongTermPricingId: str = ...,
         ImpactLevel: ImpactLevelType = ...,
-        PickupDetails: PickupDetailsUnionTypeDef = ...
+        PickupDetails: PickupDetailsTypeDef = ...
     ) -> CreateJobResultTypeDef:
         """
         Creates a job to import or export data between Amazon S3 and your on-premises
         data center.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.create_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/client/#create_job)
@@ -416,19 +416,19 @@
 
     def update_cluster(
         self,
         *,
         ClusterId: str,
         RoleARN: str = ...,
         Description: str = ...,
-        Resources: JobResourceUnionTypeDef = ...,
+        Resources: JobResourceTypeDef = ...,
         OnDeviceServiceConfiguration: OnDeviceServiceConfigurationTypeDef = ...,
         AddressId: str = ...,
         ShippingOption: ShippingOptionType = ...,
-        Notification: NotificationUnionTypeDef = ...,
+        Notification: NotificationTypeDef = ...,
         ForwardingAddressId: str = ...
     ) -> Dict[str, Any]:
         """
         While a cluster's `ClusterState` value is in the `AwaitingQuorum` state, you can
         update some of the information associated with a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.update_cluster)
@@ -436,23 +436,23 @@
         """
 
     def update_job(
         self,
         *,
         JobId: str,
         RoleARN: str = ...,
-        Notification: NotificationUnionTypeDef = ...,
-        Resources: JobResourceUnionTypeDef = ...,
+        Notification: NotificationTypeDef = ...,
+        Resources: JobResourceTypeDef = ...,
         OnDeviceServiceConfiguration: OnDeviceServiceConfigurationTypeDef = ...,
         AddressId: str = ...,
         ShippingOption: ShippingOptionType = ...,
         Description: str = ...,
         SnowballCapacityPreference: SnowballCapacityType = ...,
         ForwardingAddressId: str = ...,
-        PickupDetails: PickupDetailsUnionTypeDef = ...
+        PickupDetails: PickupDetailsTypeDef = ...
     ) -> Dict[str, Any]:
         """
         While a job's `JobState` value is `New`, you can update some of the information
         associated with a job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.update_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/client/#update_job)
```

### Comparing `mypy-boto3-snowball-1.28.16/mypy_boto3_snowball/client.pyi` & `mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -51,25 +51,25 @@
     DescribeJobResultTypeDef,
     DescribeReturnShippingLabelResultTypeDef,
     DeviceConfigurationTypeDef,
     GetJobManifestResultTypeDef,
     GetJobUnlockCodeResultTypeDef,
     GetSnowballUsageResultTypeDef,
     GetSoftwareUpdatesResultTypeDef,
-    JobResourceUnionTypeDef,
+    JobResourceTypeDef,
     ListClusterJobsResultTypeDef,
     ListClustersResultTypeDef,
     ListCompatibleImagesResultTypeDef,
     ListJobsResultTypeDef,
     ListLongTermPricingResultTypeDef,
     ListPickupLocationsResultTypeDef,
     ListServiceVersionsResultTypeDef,
-    NotificationUnionTypeDef,
+    NotificationTypeDef,
     OnDeviceServiceConfigurationTypeDef,
-    PickupDetailsUnionTypeDef,
+    PickupDetailsTypeDef,
     TaxDocumentsTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -151,20 +151,20 @@
     def create_cluster(
         self,
         *,
         JobType: JobTypeType,
         AddressId: str,
         SnowballType: SnowballTypeType,
         ShippingOption: ShippingOptionType,
-        Resources: JobResourceUnionTypeDef = ...,
+        Resources: JobResourceTypeDef = ...,
         OnDeviceServiceConfiguration: OnDeviceServiceConfigurationTypeDef = ...,
         Description: str = ...,
         KmsKeyARN: str = ...,
         RoleARN: str = ...,
-        Notification: NotificationUnionTypeDef = ...,
+        Notification: NotificationTypeDef = ...,
         ForwardingAddressId: str = ...,
         TaxDocuments: TaxDocumentsTypeDef = ...,
         RemoteManagement: RemoteManagementType = ...,
         InitialClusterSize: int = ...,
         ForceCreateJobs: bool = ...,
         LongTermPricingIds: Sequence[str] = ...,
         SnowballCapacityPreference: SnowballCapacityType = ...
@@ -175,32 +175,32 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.create_cluster)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/client/#create_cluster)
         """
     def create_job(
         self,
         *,
         JobType: JobTypeType = ...,
-        Resources: JobResourceUnionTypeDef = ...,
+        Resources: JobResourceTypeDef = ...,
         OnDeviceServiceConfiguration: OnDeviceServiceConfigurationTypeDef = ...,
         Description: str = ...,
         AddressId: str = ...,
         KmsKeyARN: str = ...,
         RoleARN: str = ...,
         SnowballCapacityPreference: SnowballCapacityType = ...,
         ShippingOption: ShippingOptionType = ...,
-        Notification: NotificationUnionTypeDef = ...,
+        Notification: NotificationTypeDef = ...,
         ClusterId: str = ...,
         SnowballType: SnowballTypeType = ...,
         ForwardingAddressId: str = ...,
         TaxDocuments: TaxDocumentsTypeDef = ...,
         DeviceConfiguration: DeviceConfigurationTypeDef = ...,
         RemoteManagement: RemoteManagementType = ...,
         LongTermPricingId: str = ...,
         ImpactLevel: ImpactLevelType = ...,
-        PickupDetails: PickupDetailsUnionTypeDef = ...
+        PickupDetails: PickupDetailsTypeDef = ...
     ) -> CreateJobResultTypeDef:
         """
         Creates a job to import or export data between Amazon S3 and your on-premises
         data center.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.create_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/client/#create_job)
@@ -385,42 +385,42 @@
         """
     def update_cluster(
         self,
         *,
         ClusterId: str,
         RoleARN: str = ...,
         Description: str = ...,
-        Resources: JobResourceUnionTypeDef = ...,
+        Resources: JobResourceTypeDef = ...,
         OnDeviceServiceConfiguration: OnDeviceServiceConfigurationTypeDef = ...,
         AddressId: str = ...,
         ShippingOption: ShippingOptionType = ...,
-        Notification: NotificationUnionTypeDef = ...,
+        Notification: NotificationTypeDef = ...,
         ForwardingAddressId: str = ...
     ) -> Dict[str, Any]:
         """
         While a cluster's `ClusterState` value is in the `AwaitingQuorum` state, you can
         update some of the information associated with a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.update_cluster)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/client/#update_cluster)
         """
     def update_job(
         self,
         *,
         JobId: str,
         RoleARN: str = ...,
-        Notification: NotificationUnionTypeDef = ...,
-        Resources: JobResourceUnionTypeDef = ...,
+        Notification: NotificationTypeDef = ...,
+        Resources: JobResourceTypeDef = ...,
         OnDeviceServiceConfiguration: OnDeviceServiceConfigurationTypeDef = ...,
         AddressId: str = ...,
         ShippingOption: ShippingOptionType = ...,
         Description: str = ...,
         SnowballCapacityPreference: SnowballCapacityType = ...,
         ForwardingAddressId: str = ...,
-        PickupDetails: PickupDetailsUnionTypeDef = ...
+        PickupDetails: PickupDetailsTypeDef = ...
     ) -> Dict[str, Any]:
         """
         While a job's `JobState` value is `New`, you can update some of the information
         associated with a job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.update_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/client/#update_job)
```

### Comparing `mypy-boto3-snowball-1.28.16/mypy_boto3_snowball/literals.py` & `mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AddressTypeType",
     "ClusterStateType",
     "DescribeAddressesPaginatorName",
     "DeviceServiceNameType",
     "ImpactLevelType",
     "JobStateType",
@@ -45,15 +44,14 @@
     "SnowballServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AddressTypeType = Literal["AWS_SHIP", "CUST_PICKUP"]
 ClusterStateType = Literal["AwaitingQuorum", "Cancelled", "Complete", "InUse", "Pending"]
 DescribeAddressesPaginatorName = Literal["describe_addresses"]
 DeviceServiceNameType = Literal["NFS_ON_DEVICE_SERVICE", "S3_ON_DEVICE_SERVICE"]
 ImpactLevelType = Literal["IL2", "IL4", "IL5", "IL6", "IL99"]
 JobStateType = Literal[
     "Cancelled",
@@ -215,15 +213,14 @@
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
@@ -302,28 +299,26 @@
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
     "mediapackage-vod",
     "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
-    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
```

### Comparing `mypy-boto3-snowball-1.28.16/mypy_boto3_snowball/literals.pyi` & `mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "AddressTypeType",
     "ClusterStateType",
     "DescribeAddressesPaginatorName",
     "DeviceServiceNameType",
     "ImpactLevelType",
     "JobStateType",
@@ -44,14 +45,15 @@
     "SnowballServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 AddressTypeType = Literal["AWS_SHIP", "CUST_PICKUP"]
 ClusterStateType = Literal["AwaitingQuorum", "Cancelled", "Complete", "InUse", "Pending"]
 DescribeAddressesPaginatorName = Literal["describe_addresses"]
 DeviceServiceNameType = Literal["NFS_ON_DEVICE_SERVICE", "S3_ON_DEVICE_SERVICE"]
 ImpactLevelType = Literal["IL2", "IL4", "IL5", "IL6", "IL99"]
 JobStateType = Literal[
     "Cancelled",
@@ -213,15 +215,14 @@
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
@@ -300,28 +301,26 @@
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
     "mediapackage-vod",
     "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
-    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
```

### Comparing `mypy-boto3-snowball-1.28.16/mypy_boto3_snowball/paginator.py` & `mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,88 +66,88 @@
 class DescribeAddressesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.DescribeAddresses)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/paginators/#describeaddressespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeAddressesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.DescribeAddresses.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/paginators/#describeaddressespaginator)
         """
 
 
 class ListClusterJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListClusterJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/paginators/#listclusterjobspaginator)
     """
 
     def paginate(
-        self, *, ClusterId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ClusterId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListClusterJobsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListClusterJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/paginators/#listclusterjobspaginator)
         """
 
 
 class ListClustersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListClusters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/paginators/#listclusterspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListClustersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListClusters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/paginators/#listclusterspaginator)
         """
 
 
 class ListCompatibleImagesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListCompatibleImages)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/paginators/#listcompatibleimagespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListCompatibleImagesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListCompatibleImages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/paginators/#listcompatibleimagespaginator)
         """
 
 
 class ListJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/paginators/#listjobspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListJobsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/paginators/#listjobspaginator)
         """
 
 
 class ListLongTermPricingPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListLongTermPricing)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/paginators/#listlongtermpricingpaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListLongTermPricingResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListLongTermPricing.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/paginators/#listlongtermpricingpaginator)
         """
```

### Comparing `mypy-boto3-snowball-1.28.16/mypy_boto3_snowball/paginator.pyi` & `mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -63,83 +63,83 @@
 class DescribeAddressesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.DescribeAddresses)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/paginators/#describeaddressespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeAddressesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.DescribeAddresses.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/paginators/#describeaddressespaginator)
         """
 
 class ListClusterJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListClusterJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/paginators/#listclusterjobspaginator)
     """
 
     def paginate(
-        self, *, ClusterId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ClusterId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListClusterJobsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListClusterJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/paginators/#listclusterjobspaginator)
         """
 
 class ListClustersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListClusters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/paginators/#listclusterspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListClustersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListClusters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/paginators/#listclusterspaginator)
         """
 
 class ListCompatibleImagesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListCompatibleImages)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/paginators/#listcompatibleimagespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListCompatibleImagesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListCompatibleImages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/paginators/#listcompatibleimagespaginator)
         """
 
 class ListJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/paginators/#listjobspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListJobsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/paginators/#listjobspaginator)
         """
 
 class ListLongTermPricingPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListLongTermPricing)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/paginators/#listlongtermpricingpaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListLongTermPricingResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListLongTermPricing.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/paginators/#listlongtermpricingpaginator)
         """
```

### Comparing `mypy-boto3-snowball-1.28.16/mypy_boto3_snowball/type_defs.py` & `mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/type_defs.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for snowball service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_snowball.type_defs import AddressTypeDef
+    from mypy_boto3_snowball.type_defs import AddressOutputTypeDef
 
-    data: AddressTypeDef = ...
+    data: AddressOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -40,112 +40,146 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "AddressOutputTypeDef",
     "AddressTypeDef",
     "CancelClusterRequestRequestTypeDef",
     "CancelJobRequestRequestTypeDef",
     "ClusterListEntryTypeDef",
     "NotificationOutputTypeDef",
     "CompatibleImageTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateAddressResultTypeDef",
     "NotificationTypeDef",
     "JobListEntryTypeDef",
+    "PickupDetailsTypeDef",
+    "CreateJobResultTypeDef",
     "CreateLongTermPricingRequestRequestTypeDef",
+    "CreateLongTermPricingResultTypeDef",
     "CreateReturnShippingLabelRequestRequestTypeDef",
+    "CreateReturnShippingLabelResultTypeDef",
     "DataTransferTypeDef",
+    "ServiceVersionOutputTypeDef",
     "ServiceVersionTypeDef",
     "DescribeAddressRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeAddressesRequestDescribeAddressesPaginateTypeDef",
     "DescribeAddressesRequestRequestTypeDef",
     "DescribeClusterRequestRequestTypeDef",
     "DescribeJobRequestRequestTypeDef",
     "DescribeReturnShippingLabelRequestRequestTypeDef",
+    "DescribeReturnShippingLabelResultTypeDef",
+    "EKSOnDeviceServiceConfigurationOutputTypeDef",
     "EKSOnDeviceServiceConfigurationTypeDef",
+    "Ec2AmiResourceOutputTypeDef",
     "Ec2AmiResourceTypeDef",
+    "EventTriggerDefinitionOutputTypeDef",
     "EventTriggerDefinitionTypeDef",
     "GetJobManifestRequestRequestTypeDef",
+    "GetJobManifestResultTypeDef",
     "GetJobUnlockCodeRequestRequestTypeDef",
+    "GetJobUnlockCodeResultTypeDef",
+    "GetSnowballUsageResultTypeDef",
     "GetSoftwareUpdatesRequestRequestTypeDef",
+    "GetSoftwareUpdatesResultTypeDef",
+    "INDTaxDocumentsOutputTypeDef",
     "INDTaxDocumentsTypeDef",
     "JobLogsTypeDef",
     "PickupDetailsOutputTypeDef",
+    "KeyRangeOutputTypeDef",
     "KeyRangeTypeDef",
+    "ListClusterJobsRequestListClusterJobsPaginateTypeDef",
     "ListClusterJobsRequestRequestTypeDef",
+    "ListClustersRequestListClustersPaginateTypeDef",
     "ListClustersRequestRequestTypeDef",
+    "ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef",
     "ListCompatibleImagesRequestRequestTypeDef",
+    "ListJobsRequestListJobsPaginateTypeDef",
     "ListJobsRequestRequestTypeDef",
+    "ListLongTermPricingRequestListLongTermPricingPaginateTypeDef",
     "ListLongTermPricingRequestRequestTypeDef",
     "LongTermPricingListEntryTypeDef",
     "ListPickupLocationsRequestRequestTypeDef",
+    "NFSOnDeviceServiceConfigurationOutputTypeDef",
     "NFSOnDeviceServiceConfigurationTypeDef",
+    "S3OnDeviceServiceConfigurationOutputTypeDef",
+    "TGWOnDeviceServiceConfigurationOutputTypeDef",
     "S3OnDeviceServiceConfigurationTypeDef",
     "TGWOnDeviceServiceConfigurationTypeDef",
-    "TimestampTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
+    "TargetOnDeviceServiceOutputTypeDef",
     "TargetOnDeviceServiceTypeDef",
     "ShipmentTypeDef",
+    "WirelessConnectionOutputTypeDef",
     "WirelessConnectionTypeDef",
     "UpdateJobShipmentStateRequestRequestTypeDef",
     "UpdateLongTermPricingRequestRequestTypeDef",
-    "CreateAddressRequestRequestTypeDef",
-    "CreateAddressResultTypeDef",
-    "CreateJobResultTypeDef",
-    "CreateLongTermPricingResultTypeDef",
-    "CreateReturnShippingLabelResultTypeDef",
     "DescribeAddressResultTypeDef",
     "DescribeAddressesResultTypeDef",
-    "DescribeReturnShippingLabelResultTypeDef",
-    "GetJobManifestResultTypeDef",
-    "GetJobUnlockCodeResultTypeDef",
-    "GetSnowballUsageResultTypeDef",
-    "GetSoftwareUpdatesResultTypeDef",
+    "ListPickupLocationsResultTypeDef",
+    "CreateAddressRequestRequestTypeDef",
     "ListClustersResultTypeDef",
     "ListCompatibleImagesResultTypeDef",
-    "ListPickupLocationsResultTypeDef",
-    "NotificationUnionTypeDef",
     "CreateClusterResultTypeDef",
     "ListClusterJobsResultTypeDef",
     "ListJobsResultTypeDef",
+    "DependentServiceOutputTypeDef",
     "DependentServiceTypeDef",
-    "DescribeAddressesRequestDescribeAddressesPaginateTypeDef",
-    "ListClusterJobsRequestListClusterJobsPaginateTypeDef",
-    "ListClustersRequestListClustersPaginateTypeDef",
-    "ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef",
-    "ListJobsRequestListJobsPaginateTypeDef",
-    "ListLongTermPricingRequestListLongTermPricingPaginateTypeDef",
     "LambdaResourceOutputTypeDef",
     "LambdaResourceTypeDef",
+    "TaxDocumentsOutputTypeDef",
     "TaxDocumentsTypeDef",
     "ListLongTermPricingResultTypeDef",
+    "OnDeviceServiceConfigurationOutputTypeDef",
     "OnDeviceServiceConfigurationTypeDef",
-    "PickupDetailsTypeDef",
     "S3ResourceOutputTypeDef",
     "S3ResourceTypeDef",
     "ShippingDetailsTypeDef",
+    "SnowconeDeviceConfigurationOutputTypeDef",
     "SnowconeDeviceConfigurationTypeDef",
-    "ListServiceVersionsRequestRequestTypeDef",
     "ListServiceVersionsResultTypeDef",
-    "PickupDetailsUnionTypeDef",
+    "ListServiceVersionsRequestRequestTypeDef",
     "JobResourceOutputTypeDef",
     "JobResourceTypeDef",
+    "DeviceConfigurationOutputTypeDef",
     "DeviceConfigurationTypeDef",
     "ClusterMetadataTypeDef",
     "CreateClusterRequestRequestTypeDef",
-    "JobResourceUnionTypeDef",
     "UpdateClusterRequestRequestTypeDef",
     "UpdateJobRequestRequestTypeDef",
-    "CreateJobRequestRequestTypeDef",
     "JobMetadataTypeDef",
+    "CreateJobRequestRequestTypeDef",
     "DescribeClusterResultTypeDef",
     "DescribeJobResultTypeDef",
 )
 
+AddressOutputTypeDef = TypedDict(
+    "AddressOutputTypeDef",
+    {
+        "AddressId": str,
+        "Name": str,
+        "Company": str,
+        "Street1": str,
+        "Street2": str,
+        "Street3": str,
+        "City": str,
+        "StateOrProvince": str,
+        "PrefectureOrDistrict": str,
+        "Landmark": str,
+        "Country": str,
+        "PostalCode": str,
+        "PhoneNumber": str,
+        "IsRestricted": bool,
+        "Type": AddressTypeType,
+    },
+)
+
 AddressTypeDef = TypedDict(
     "AddressTypeDef",
     {
         "AddressId": str,
         "Name": str,
         "Company": str,
         "Street1": str,
@@ -182,45 +216,39 @@
     "ClusterListEntryTypeDef",
     {
         "ClusterId": str,
         "ClusterState": ClusterStateType,
         "CreationDate": datetime,
         "Description": str,
     },
-    total=False,
 )
 
 NotificationOutputTypeDef = TypedDict(
     "NotificationOutputTypeDef",
     {
         "SnsTopicARN": str,
         "JobStatesToNotify": List[JobStateType],
         "NotifyAll": bool,
         "DevicePickupSnsTopicARN": str,
     },
-    total=False,
 )
 
 CompatibleImageTypeDef = TypedDict(
     "CompatibleImageTypeDef",
     {
         "AmiId": str,
         "Name": str,
     },
-    total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateAddressResultTypeDef = TypedDict(
+    "CreateAddressResultTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "AddressId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 NotificationTypeDef = TypedDict(
     "NotificationTypeDef",
     {
         "SnsTopicARN": str,
@@ -238,17 +266,38 @@
         "JobState": JobStateType,
         "IsMaster": bool,
         "JobType": JobTypeType,
         "SnowballType": SnowballTypeType,
         "CreationDate": datetime,
         "Description": str,
     },
+)
+
+PickupDetailsTypeDef = TypedDict(
+    "PickupDetailsTypeDef",
+    {
+        "Name": str,
+        "PhoneNumber": str,
+        "Email": str,
+        "IdentificationNumber": str,
+        "IdentificationExpirationDate": Union[datetime, str],
+        "IdentificationIssuingOrg": str,
+        "DevicePickupId": str,
+    },
     total=False,
 )
 
+CreateJobResultTypeDef = TypedDict(
+    "CreateJobResultTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateLongTermPricingRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLongTermPricingRequestRequestTypeDef",
     {
         "LongTermPricingType": LongTermPricingTypeType,
         "SnowballType": SnowballTypeType,
     },
 )
@@ -264,14 +313,22 @@
 class CreateLongTermPricingRequestRequestTypeDef(
     _RequiredCreateLongTermPricingRequestRequestTypeDef,
     _OptionalCreateLongTermPricingRequestRequestTypeDef,
 ):
     pass
 
 
+CreateLongTermPricingResultTypeDef = TypedDict(
+    "CreateLongTermPricingResultTypeDef",
+    {
+        "LongTermPricingId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateReturnShippingLabelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateReturnShippingLabelRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 _OptionalCreateReturnShippingLabelRequestRequestTypeDef = TypedDict(
@@ -286,23 +343,37 @@
 class CreateReturnShippingLabelRequestRequestTypeDef(
     _RequiredCreateReturnShippingLabelRequestRequestTypeDef,
     _OptionalCreateReturnShippingLabelRequestRequestTypeDef,
 ):
     pass
 
 
+CreateReturnShippingLabelResultTypeDef = TypedDict(
+    "CreateReturnShippingLabelResultTypeDef",
+    {
+        "Status": ShippingLabelStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DataTransferTypeDef = TypedDict(
     "DataTransferTypeDef",
     {
         "BytesTransferred": int,
         "ObjectsTransferred": int,
         "TotalBytes": int,
         "TotalObjects": int,
     },
-    total=False,
+)
+
+ServiceVersionOutputTypeDef = TypedDict(
+    "ServiceVersionOutputTypeDef",
+    {
+        "Version": str,
+    },
 )
 
 ServiceVersionTypeDef = TypedDict(
     "ServiceVersionTypeDef",
     {
         "Version": str,
     },
@@ -312,20 +383,18 @@
 DescribeAddressRequestRequestTypeDef = TypedDict(
     "DescribeAddressRequestRequestTypeDef",
     {
         "AddressId": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DescribeAddressesRequestDescribeAddressesPaginateTypeDef = TypedDict(
+    "DescribeAddressesRequestDescribeAddressesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeAddressesRequestRequestTypeDef = TypedDict(
     "DescribeAddressesRequestRequestTypeDef",
     {
@@ -352,23 +421,49 @@
 DescribeReturnShippingLabelRequestRequestTypeDef = TypedDict(
     "DescribeReturnShippingLabelRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
+DescribeReturnShippingLabelResultTypeDef = TypedDict(
+    "DescribeReturnShippingLabelResultTypeDef",
+    {
+        "Status": ShippingLabelStatusType,
+        "ExpirationDate": datetime,
+        "ReturnShippingLabelURI": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+EKSOnDeviceServiceConfigurationOutputTypeDef = TypedDict(
+    "EKSOnDeviceServiceConfigurationOutputTypeDef",
+    {
+        "KubernetesVersion": str,
+        "EKSAnywhereVersion": str,
+    },
+)
+
 EKSOnDeviceServiceConfigurationTypeDef = TypedDict(
     "EKSOnDeviceServiceConfigurationTypeDef",
     {
         "KubernetesVersion": str,
         "EKSAnywhereVersion": str,
     },
     total=False,
 )
 
+Ec2AmiResourceOutputTypeDef = TypedDict(
+    "Ec2AmiResourceOutputTypeDef",
+    {
+        "AmiId": str,
+        "SnowballAmiId": str,
+    },
+)
+
 _RequiredEc2AmiResourceTypeDef = TypedDict(
     "_RequiredEc2AmiResourceTypeDef",
     {
         "AmiId": str,
     },
 )
 _OptionalEc2AmiResourceTypeDef = TypedDict(
@@ -380,14 +475,21 @@
 )
 
 
 class Ec2AmiResourceTypeDef(_RequiredEc2AmiResourceTypeDef, _OptionalEc2AmiResourceTypeDef):
     pass
 
 
+EventTriggerDefinitionOutputTypeDef = TypedDict(
+    "EventTriggerDefinitionOutputTypeDef",
+    {
+        "EventResourceARN": str,
+    },
+)
+
 EventTriggerDefinitionTypeDef = TypedDict(
     "EventTriggerDefinitionTypeDef",
     {
         "EventResourceARN": str,
     },
     total=False,
 )
@@ -395,28 +497,68 @@
 GetJobManifestRequestRequestTypeDef = TypedDict(
     "GetJobManifestRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
+GetJobManifestResultTypeDef = TypedDict(
+    "GetJobManifestResultTypeDef",
+    {
+        "ManifestURI": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetJobUnlockCodeRequestRequestTypeDef = TypedDict(
     "GetJobUnlockCodeRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
+GetJobUnlockCodeResultTypeDef = TypedDict(
+    "GetJobUnlockCodeResultTypeDef",
+    {
+        "UnlockCode": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetSnowballUsageResultTypeDef = TypedDict(
+    "GetSnowballUsageResultTypeDef",
+    {
+        "SnowballLimit": int,
+        "SnowballsInUse": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetSoftwareUpdatesRequestRequestTypeDef = TypedDict(
     "GetSoftwareUpdatesRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
+GetSoftwareUpdatesResultTypeDef = TypedDict(
+    "GetSoftwareUpdatesResultTypeDef",
+    {
+        "UpdatesURI": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+INDTaxDocumentsOutputTypeDef = TypedDict(
+    "INDTaxDocumentsOutputTypeDef",
+    {
+        "GSTIN": str,
+    },
+)
+
 INDTaxDocumentsTypeDef = TypedDict(
     "INDTaxDocumentsTypeDef",
     {
         "GSTIN": str,
     },
     total=False,
 )
@@ -424,40 +566,68 @@
 JobLogsTypeDef = TypedDict(
     "JobLogsTypeDef",
     {
         "JobCompletionReportURI": str,
         "JobSuccessLogURI": str,
         "JobFailureLogURI": str,
     },
-    total=False,
 )
 
 PickupDetailsOutputTypeDef = TypedDict(
     "PickupDetailsOutputTypeDef",
     {
         "Name": str,
         "PhoneNumber": str,
         "Email": str,
         "IdentificationNumber": str,
         "IdentificationExpirationDate": datetime,
         "IdentificationIssuingOrg": str,
         "DevicePickupId": str,
     },
-    total=False,
+)
+
+KeyRangeOutputTypeDef = TypedDict(
+    "KeyRangeOutputTypeDef",
+    {
+        "BeginMarker": str,
+        "EndMarker": str,
+    },
 )
 
 KeyRangeTypeDef = TypedDict(
     "KeyRangeTypeDef",
     {
         "BeginMarker": str,
         "EndMarker": str,
     },
     total=False,
 )
 
+_RequiredListClusterJobsRequestListClusterJobsPaginateTypeDef = TypedDict(
+    "_RequiredListClusterJobsRequestListClusterJobsPaginateTypeDef",
+    {
+        "ClusterId": str,
+    },
+)
+_OptionalListClusterJobsRequestListClusterJobsPaginateTypeDef = TypedDict(
+    "_OptionalListClusterJobsRequestListClusterJobsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListClusterJobsRequestListClusterJobsPaginateTypeDef(
+    _RequiredListClusterJobsRequestListClusterJobsPaginateTypeDef,
+    _OptionalListClusterJobsRequestListClusterJobsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListClusterJobsRequestRequestTypeDef = TypedDict(
     "_RequiredListClusterJobsRequestRequestTypeDef",
     {
         "ClusterId": str,
     },
 )
 _OptionalListClusterJobsRequestRequestTypeDef = TypedDict(
@@ -472,41 +642,73 @@
 
 class ListClusterJobsRequestRequestTypeDef(
     _RequiredListClusterJobsRequestRequestTypeDef, _OptionalListClusterJobsRequestRequestTypeDef
 ):
     pass
 
 
+ListClustersRequestListClustersPaginateTypeDef = TypedDict(
+    "ListClustersRequestListClustersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListClustersRequestRequestTypeDef = TypedDict(
     "ListClustersRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef = TypedDict(
+    "ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListCompatibleImagesRequestRequestTypeDef = TypedDict(
     "ListCompatibleImagesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListJobsRequestListJobsPaginateTypeDef = TypedDict(
+    "ListJobsRequestListJobsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListJobsRequestRequestTypeDef = TypedDict(
     "ListJobsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListLongTermPricingRequestListLongTermPricingPaginateTypeDef = TypedDict(
+    "ListLongTermPricingRequestListLongTermPricingPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListLongTermPricingRequestRequestTypeDef = TypedDict(
     "ListLongTermPricingRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -522,35 +724,60 @@
         "CurrentActiveJob": str,
         "ReplacementJob": str,
         "IsLongTermPricingAutoRenew": bool,
         "LongTermPricingStatus": str,
         "SnowballType": SnowballTypeType,
         "JobIds": List[str],
     },
-    total=False,
 )
 
 ListPickupLocationsRequestRequestTypeDef = TypedDict(
     "ListPickupLocationsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+NFSOnDeviceServiceConfigurationOutputTypeDef = TypedDict(
+    "NFSOnDeviceServiceConfigurationOutputTypeDef",
+    {
+        "StorageLimit": int,
+        "StorageUnit": Literal["TB"],
+    },
+)
+
 NFSOnDeviceServiceConfigurationTypeDef = TypedDict(
     "NFSOnDeviceServiceConfigurationTypeDef",
     {
         "StorageLimit": int,
         "StorageUnit": Literal["TB"],
     },
     total=False,
 )
 
+S3OnDeviceServiceConfigurationOutputTypeDef = TypedDict(
+    "S3OnDeviceServiceConfigurationOutputTypeDef",
+    {
+        "StorageLimit": float,
+        "StorageUnit": Literal["TB"],
+        "ServiceSize": int,
+        "FaultTolerance": int,
+    },
+)
+
+TGWOnDeviceServiceConfigurationOutputTypeDef = TypedDict(
+    "TGWOnDeviceServiceConfigurationOutputTypeDef",
+    {
+        "StorageLimit": int,
+        "StorageUnit": Literal["TB"],
+    },
+)
+
 S3OnDeviceServiceConfigurationTypeDef = TypedDict(
     "S3OnDeviceServiceConfigurationTypeDef",
     {
         "StorageLimit": float,
         "StorageUnit": Literal["TB"],
         "ServiceSize": int,
         "FaultTolerance": int,
@@ -563,15 +790,43 @@
     {
         "StorageLimit": int,
         "StorageUnit": Literal["TB"],
     },
     total=False,
 )
 
-TimestampTypeDef = Union[datetime, str]
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
+)
+
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
+TargetOnDeviceServiceOutputTypeDef = TypedDict(
+    "TargetOnDeviceServiceOutputTypeDef",
+    {
+        "ServiceName": DeviceServiceNameType,
+        "TransferOption": TransferOptionType,
+    },
+)
+
 TargetOnDeviceServiceTypeDef = TypedDict(
     "TargetOnDeviceServiceTypeDef",
     {
         "ServiceName": DeviceServiceNameType,
         "TransferOption": TransferOptionType,
     },
     total=False,
@@ -579,15 +834,21 @@
 
 ShipmentTypeDef = TypedDict(
     "ShipmentTypeDef",
     {
         "Status": str,
         "TrackingNumber": str,
     },
-    total=False,
+)
+
+WirelessConnectionOutputTypeDef = TypedDict(
+    "WirelessConnectionOutputTypeDef",
+    {
+        "IsWifiEnabled": bool,
+    },
 )
 
 WirelessConnectionTypeDef = TypedDict(
     "WirelessConnectionTypeDef",
     {
         "IsWifiEnabled": bool,
     },
@@ -621,307 +882,178 @@
 class UpdateLongTermPricingRequestRequestTypeDef(
     _RequiredUpdateLongTermPricingRequestRequestTypeDef,
     _OptionalUpdateLongTermPricingRequestRequestTypeDef,
 ):
     pass
 
 
-CreateAddressRequestRequestTypeDef = TypedDict(
-    "CreateAddressRequestRequestTypeDef",
-    {
-        "Address": AddressTypeDef,
-    },
-)
-
-CreateAddressResultTypeDef = TypedDict(
-    "CreateAddressResultTypeDef",
-    {
-        "AddressId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateJobResultTypeDef = TypedDict(
-    "CreateJobResultTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateLongTermPricingResultTypeDef = TypedDict(
-    "CreateLongTermPricingResultTypeDef",
-    {
-        "LongTermPricingId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateReturnShippingLabelResultTypeDef = TypedDict(
-    "CreateReturnShippingLabelResultTypeDef",
-    {
-        "Status": ShippingLabelStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DescribeAddressResultTypeDef = TypedDict(
     "DescribeAddressResultTypeDef",
     {
-        "Address": AddressTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Address": AddressOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeAddressesResultTypeDef = TypedDict(
     "DescribeAddressesResultTypeDef",
     {
-        "Addresses": List[AddressTypeDef],
+        "Addresses": List[AddressOutputTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeReturnShippingLabelResultTypeDef = TypedDict(
-    "DescribeReturnShippingLabelResultTypeDef",
-    {
-        "Status": ShippingLabelStatusType,
-        "ExpirationDate": datetime,
-        "ReturnShippingLabelURI": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetJobManifestResultTypeDef = TypedDict(
-    "GetJobManifestResultTypeDef",
-    {
-        "ManifestURI": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetJobUnlockCodeResultTypeDef = TypedDict(
-    "GetJobUnlockCodeResultTypeDef",
-    {
-        "UnlockCode": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetSnowballUsageResultTypeDef = TypedDict(
-    "GetSnowballUsageResultTypeDef",
+ListPickupLocationsResultTypeDef = TypedDict(
+    "ListPickupLocationsResultTypeDef",
     {
-        "SnowballLimit": int,
-        "SnowballsInUse": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Addresses": List[AddressOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetSoftwareUpdatesResultTypeDef = TypedDict(
-    "GetSoftwareUpdatesResultTypeDef",
+CreateAddressRequestRequestTypeDef = TypedDict(
+    "CreateAddressRequestRequestTypeDef",
     {
-        "UpdatesURI": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Address": AddressTypeDef,
     },
 )
 
 ListClustersResultTypeDef = TypedDict(
     "ListClustersResultTypeDef",
     {
         "ClusterListEntries": List[ClusterListEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListCompatibleImagesResultTypeDef = TypedDict(
     "ListCompatibleImagesResultTypeDef",
     {
         "CompatibleImages": List[CompatibleImageTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListPickupLocationsResultTypeDef = TypedDict(
-    "ListPickupLocationsResultTypeDef",
-    {
-        "Addresses": List[AddressTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-NotificationUnionTypeDef = Union[NotificationTypeDef, NotificationOutputTypeDef]
 CreateClusterResultTypeDef = TypedDict(
     "CreateClusterResultTypeDef",
     {
         "ClusterId": str,
         "JobListEntries": List[JobListEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListClusterJobsResultTypeDef = TypedDict(
     "ListClusterJobsResultTypeDef",
     {
         "JobListEntries": List[JobListEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListJobsResultTypeDef = TypedDict(
     "ListJobsResultTypeDef",
     {
         "JobListEntries": List[JobListEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DependentServiceTypeDef = TypedDict(
-    "DependentServiceTypeDef",
+DependentServiceOutputTypeDef = TypedDict(
+    "DependentServiceOutputTypeDef",
     {
         "ServiceName": ServiceNameType,
-        "ServiceVersion": ServiceVersionTypeDef,
+        "ServiceVersion": ServiceVersionOutputTypeDef,
     },
-    total=False,
 )
 
-DescribeAddressesRequestDescribeAddressesPaginateTypeDef = TypedDict(
-    "DescribeAddressesRequestDescribeAddressesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListClusterJobsRequestListClusterJobsPaginateTypeDef = TypedDict(
-    "_RequiredListClusterJobsRequestListClusterJobsPaginateTypeDef",
-    {
-        "ClusterId": str,
-    },
-)
-_OptionalListClusterJobsRequestListClusterJobsPaginateTypeDef = TypedDict(
-    "_OptionalListClusterJobsRequestListClusterJobsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListClusterJobsRequestListClusterJobsPaginateTypeDef(
-    _RequiredListClusterJobsRequestListClusterJobsPaginateTypeDef,
-    _OptionalListClusterJobsRequestListClusterJobsPaginateTypeDef,
-):
-    pass
-
-
-ListClustersRequestListClustersPaginateTypeDef = TypedDict(
-    "ListClustersRequestListClustersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef = TypedDict(
-    "ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListJobsRequestListJobsPaginateTypeDef = TypedDict(
-    "ListJobsRequestListJobsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListLongTermPricingRequestListLongTermPricingPaginateTypeDef = TypedDict(
-    "ListLongTermPricingRequestListLongTermPricingPaginateTypeDef",
+DependentServiceTypeDef = TypedDict(
+    "DependentServiceTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ServiceName": ServiceNameType,
+        "ServiceVersion": ServiceVersionTypeDef,
     },
     total=False,
 )
 
 LambdaResourceOutputTypeDef = TypedDict(
     "LambdaResourceOutputTypeDef",
     {
         "LambdaArn": str,
-        "EventTriggers": List[EventTriggerDefinitionTypeDef],
+        "EventTriggers": List[EventTriggerDefinitionOutputTypeDef],
     },
-    total=False,
 )
 
 LambdaResourceTypeDef = TypedDict(
     "LambdaResourceTypeDef",
     {
         "LambdaArn": str,
         "EventTriggers": Sequence[EventTriggerDefinitionTypeDef],
     },
     total=False,
 )
 
+TaxDocumentsOutputTypeDef = TypedDict(
+    "TaxDocumentsOutputTypeDef",
+    {
+        "IND": INDTaxDocumentsOutputTypeDef,
+    },
+)
+
 TaxDocumentsTypeDef = TypedDict(
     "TaxDocumentsTypeDef",
     {
         "IND": INDTaxDocumentsTypeDef,
     },
     total=False,
 )
 
 ListLongTermPricingResultTypeDef = TypedDict(
     "ListLongTermPricingResultTypeDef",
     {
         "LongTermPricingEntries": List[LongTermPricingListEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+OnDeviceServiceConfigurationOutputTypeDef = TypedDict(
+    "OnDeviceServiceConfigurationOutputTypeDef",
+    {
+        "NFSOnDeviceService": NFSOnDeviceServiceConfigurationOutputTypeDef,
+        "TGWOnDeviceService": TGWOnDeviceServiceConfigurationOutputTypeDef,
+        "EKSOnDeviceService": EKSOnDeviceServiceConfigurationOutputTypeDef,
+        "S3OnDeviceService": S3OnDeviceServiceConfigurationOutputTypeDef,
     },
 )
 
 OnDeviceServiceConfigurationTypeDef = TypedDict(
     "OnDeviceServiceConfigurationTypeDef",
     {
         "NFSOnDeviceService": NFSOnDeviceServiceConfigurationTypeDef,
         "TGWOnDeviceService": TGWOnDeviceServiceConfigurationTypeDef,
         "EKSOnDeviceService": EKSOnDeviceServiceConfigurationTypeDef,
         "S3OnDeviceService": S3OnDeviceServiceConfigurationTypeDef,
     },
     total=False,
 )
 
-PickupDetailsTypeDef = TypedDict(
-    "PickupDetailsTypeDef",
-    {
-        "Name": str,
-        "PhoneNumber": str,
-        "Email": str,
-        "IdentificationNumber": str,
-        "IdentificationExpirationDate": TimestampTypeDef,
-        "IdentificationIssuingOrg": str,
-        "DevicePickupId": str,
-    },
-    total=False,
-)
-
 S3ResourceOutputTypeDef = TypedDict(
     "S3ResourceOutputTypeDef",
     {
         "BucketArn": str,
-        "KeyRange": KeyRangeTypeDef,
-        "TargetOnDeviceServices": List[TargetOnDeviceServiceTypeDef],
+        "KeyRange": KeyRangeOutputTypeDef,
+        "TargetOnDeviceServices": List[TargetOnDeviceServiceOutputTypeDef],
     },
-    total=False,
 )
 
 S3ResourceTypeDef = TypedDict(
     "S3ResourceTypeDef",
     {
         "BucketArn": str,
         "KeyRange": KeyRangeTypeDef,
@@ -933,25 +1065,42 @@
 ShippingDetailsTypeDef = TypedDict(
     "ShippingDetailsTypeDef",
     {
         "ShippingOption": ShippingOptionType,
         "InboundShipment": ShipmentTypeDef,
         "OutboundShipment": ShipmentTypeDef,
     },
-    total=False,
+)
+
+SnowconeDeviceConfigurationOutputTypeDef = TypedDict(
+    "SnowconeDeviceConfigurationOutputTypeDef",
+    {
+        "WirelessConnection": WirelessConnectionOutputTypeDef,
+    },
 )
 
 SnowconeDeviceConfigurationTypeDef = TypedDict(
     "SnowconeDeviceConfigurationTypeDef",
     {
         "WirelessConnection": WirelessConnectionTypeDef,
     },
     total=False,
 )
 
+ListServiceVersionsResultTypeDef = TypedDict(
+    "ListServiceVersionsResultTypeDef",
+    {
+        "ServiceVersions": List[ServiceVersionOutputTypeDef],
+        "ServiceName": ServiceNameType,
+        "DependentServices": List[DependentServiceOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredListServiceVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListServiceVersionsRequestRequestTypeDef",
     {
         "ServiceName": ServiceNameType,
     },
 )
 _OptionalListServiceVersionsRequestRequestTypeDef = TypedDict(
@@ -968,46 +1117,40 @@
 class ListServiceVersionsRequestRequestTypeDef(
     _RequiredListServiceVersionsRequestRequestTypeDef,
     _OptionalListServiceVersionsRequestRequestTypeDef,
 ):
     pass
 
 
-ListServiceVersionsResultTypeDef = TypedDict(
-    "ListServiceVersionsResultTypeDef",
-    {
-        "ServiceVersions": List[ServiceVersionTypeDef],
-        "ServiceName": ServiceNameType,
-        "DependentServices": List[DependentServiceTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PickupDetailsUnionTypeDef = Union[PickupDetailsTypeDef, PickupDetailsOutputTypeDef]
 JobResourceOutputTypeDef = TypedDict(
     "JobResourceOutputTypeDef",
     {
         "S3Resources": List[S3ResourceOutputTypeDef],
         "LambdaResources": List[LambdaResourceOutputTypeDef],
-        "Ec2AmiResources": List[Ec2AmiResourceTypeDef],
+        "Ec2AmiResources": List[Ec2AmiResourceOutputTypeDef],
     },
-    total=False,
 )
 
 JobResourceTypeDef = TypedDict(
     "JobResourceTypeDef",
     {
         "S3Resources": Sequence[S3ResourceTypeDef],
         "LambdaResources": Sequence[LambdaResourceTypeDef],
         "Ec2AmiResources": Sequence[Ec2AmiResourceTypeDef],
     },
     total=False,
 )
 
+DeviceConfigurationOutputTypeDef = TypedDict(
+    "DeviceConfigurationOutputTypeDef",
+    {
+        "SnowconeDeviceConfiguration": SnowconeDeviceConfigurationOutputTypeDef,
+    },
+)
+
 DeviceConfigurationTypeDef = TypedDict(
     "DeviceConfigurationTypeDef",
     {
         "SnowconeDeviceConfiguration": SnowconeDeviceConfigurationTypeDef,
     },
     total=False,
 )
@@ -1024,18 +1167,17 @@
         "SnowballType": SnowballTypeType,
         "CreationDate": datetime,
         "Resources": JobResourceOutputTypeDef,
         "AddressId": str,
         "ShippingOption": ShippingOptionType,
         "Notification": NotificationOutputTypeDef,
         "ForwardingAddressId": str,
-        "TaxDocuments": TaxDocumentsTypeDef,
-        "OnDeviceServiceConfiguration": OnDeviceServiceConfigurationTypeDef,
+        "TaxDocuments": TaxDocumentsOutputTypeDef,
+        "OnDeviceServiceConfiguration": OnDeviceServiceConfigurationOutputTypeDef,
     },
-    total=False,
 )
 
 _RequiredCreateClusterRequestRequestTypeDef = TypedDict(
     "_RequiredCreateClusterRequestRequestTypeDef",
     {
         "JobType": JobTypeType,
         "AddressId": str,
@@ -1066,15 +1208,14 @@
 
 class CreateClusterRequestRequestTypeDef(
     _RequiredCreateClusterRequestRequestTypeDef, _OptionalCreateClusterRequestRequestTypeDef
 ):
     pass
 
 
-JobResourceUnionTypeDef = Union[JobResourceTypeDef, JobResourceOutputTypeDef]
 _RequiredUpdateClusterRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateClusterRequestRequestTypeDef",
     {
         "ClusterId": str,
     },
 )
 _OptionalUpdateClusterRequestRequestTypeDef = TypedDict(
@@ -1125,81 +1266,80 @@
 
 class UpdateJobRequestRequestTypeDef(
     _RequiredUpdateJobRequestRequestTypeDef, _OptionalUpdateJobRequestRequestTypeDef
 ):
     pass
 
 
-CreateJobRequestRequestTypeDef = TypedDict(
-    "CreateJobRequestRequestTypeDef",
+JobMetadataTypeDef = TypedDict(
+    "JobMetadataTypeDef",
     {
+        "JobId": str,
+        "JobState": JobStateType,
         "JobType": JobTypeType,
-        "Resources": JobResourceTypeDef,
-        "OnDeviceServiceConfiguration": OnDeviceServiceConfigurationTypeDef,
+        "SnowballType": SnowballTypeType,
+        "CreationDate": datetime,
+        "Resources": JobResourceOutputTypeDef,
         "Description": str,
-        "AddressId": str,
         "KmsKeyARN": str,
         "RoleARN": str,
+        "AddressId": str,
+        "ShippingDetails": ShippingDetailsTypeDef,
         "SnowballCapacityPreference": SnowballCapacityType,
-        "ShippingOption": ShippingOptionType,
-        "Notification": NotificationTypeDef,
+        "Notification": NotificationOutputTypeDef,
+        "DataTransferProgress": DataTransferTypeDef,
+        "JobLogInfo": JobLogsTypeDef,
         "ClusterId": str,
-        "SnowballType": SnowballTypeType,
         "ForwardingAddressId": str,
-        "TaxDocuments": TaxDocumentsTypeDef,
-        "DeviceConfiguration": DeviceConfigurationTypeDef,
+        "TaxDocuments": TaxDocumentsOutputTypeDef,
+        "DeviceConfiguration": DeviceConfigurationOutputTypeDef,
         "RemoteManagement": RemoteManagementType,
         "LongTermPricingId": str,
+        "OnDeviceServiceConfiguration": OnDeviceServiceConfigurationOutputTypeDef,
         "ImpactLevel": ImpactLevelType,
-        "PickupDetails": PickupDetailsTypeDef,
+        "PickupDetails": PickupDetailsOutputTypeDef,
+        "SnowballId": str,
     },
-    total=False,
 )
 
-JobMetadataTypeDef = TypedDict(
-    "JobMetadataTypeDef",
+CreateJobRequestRequestTypeDef = TypedDict(
+    "CreateJobRequestRequestTypeDef",
     {
-        "JobId": str,
-        "JobState": JobStateType,
         "JobType": JobTypeType,
-        "SnowballType": SnowballTypeType,
-        "CreationDate": datetime,
-        "Resources": JobResourceOutputTypeDef,
+        "Resources": JobResourceTypeDef,
+        "OnDeviceServiceConfiguration": OnDeviceServiceConfigurationTypeDef,
         "Description": str,
+        "AddressId": str,
         "KmsKeyARN": str,
         "RoleARN": str,
-        "AddressId": str,
-        "ShippingDetails": ShippingDetailsTypeDef,
         "SnowballCapacityPreference": SnowballCapacityType,
-        "Notification": NotificationOutputTypeDef,
-        "DataTransferProgress": DataTransferTypeDef,
-        "JobLogInfo": JobLogsTypeDef,
+        "ShippingOption": ShippingOptionType,
+        "Notification": NotificationTypeDef,
         "ClusterId": str,
+        "SnowballType": SnowballTypeType,
         "ForwardingAddressId": str,
         "TaxDocuments": TaxDocumentsTypeDef,
         "DeviceConfiguration": DeviceConfigurationTypeDef,
         "RemoteManagement": RemoteManagementType,
         "LongTermPricingId": str,
-        "OnDeviceServiceConfiguration": OnDeviceServiceConfigurationTypeDef,
         "ImpactLevel": ImpactLevelType,
-        "PickupDetails": PickupDetailsOutputTypeDef,
-        "SnowballId": str,
+        "PickupDetails": PickupDetailsTypeDef,
     },
     total=False,
 )
 
 DescribeClusterResultTypeDef = TypedDict(
     "DescribeClusterResultTypeDef",
     {
         "ClusterMetadata": ClusterMetadataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeJobResultTypeDef = TypedDict(
     "DescribeJobResultTypeDef",
     {
         "JobMetadata": JobMetadataTypeDef,
         "SubJobMetadata": List[JobMetadataTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-snowball-1.28.16/mypy_boto3_snowball/type_defs.pyi` & `mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/type_defs.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for snowball service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_snowball.type_defs import AddressTypeDef
+    from mypy_boto3_snowball.type_defs import AddressOutputTypeDef
 
-    data: AddressTypeDef = ...
+    data: AddressOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -39,112 +39,146 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "AddressOutputTypeDef",
     "AddressTypeDef",
     "CancelClusterRequestRequestTypeDef",
     "CancelJobRequestRequestTypeDef",
     "ClusterListEntryTypeDef",
     "NotificationOutputTypeDef",
     "CompatibleImageTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateAddressResultTypeDef",
     "NotificationTypeDef",
     "JobListEntryTypeDef",
+    "PickupDetailsTypeDef",
+    "CreateJobResultTypeDef",
     "CreateLongTermPricingRequestRequestTypeDef",
+    "CreateLongTermPricingResultTypeDef",
     "CreateReturnShippingLabelRequestRequestTypeDef",
+    "CreateReturnShippingLabelResultTypeDef",
     "DataTransferTypeDef",
+    "ServiceVersionOutputTypeDef",
     "ServiceVersionTypeDef",
     "DescribeAddressRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeAddressesRequestDescribeAddressesPaginateTypeDef",
     "DescribeAddressesRequestRequestTypeDef",
     "DescribeClusterRequestRequestTypeDef",
     "DescribeJobRequestRequestTypeDef",
     "DescribeReturnShippingLabelRequestRequestTypeDef",
+    "DescribeReturnShippingLabelResultTypeDef",
+    "EKSOnDeviceServiceConfigurationOutputTypeDef",
     "EKSOnDeviceServiceConfigurationTypeDef",
+    "Ec2AmiResourceOutputTypeDef",
     "Ec2AmiResourceTypeDef",
+    "EventTriggerDefinitionOutputTypeDef",
     "EventTriggerDefinitionTypeDef",
     "GetJobManifestRequestRequestTypeDef",
+    "GetJobManifestResultTypeDef",
     "GetJobUnlockCodeRequestRequestTypeDef",
+    "GetJobUnlockCodeResultTypeDef",
+    "GetSnowballUsageResultTypeDef",
     "GetSoftwareUpdatesRequestRequestTypeDef",
+    "GetSoftwareUpdatesResultTypeDef",
+    "INDTaxDocumentsOutputTypeDef",
     "INDTaxDocumentsTypeDef",
     "JobLogsTypeDef",
     "PickupDetailsOutputTypeDef",
+    "KeyRangeOutputTypeDef",
     "KeyRangeTypeDef",
+    "ListClusterJobsRequestListClusterJobsPaginateTypeDef",
     "ListClusterJobsRequestRequestTypeDef",
+    "ListClustersRequestListClustersPaginateTypeDef",
     "ListClustersRequestRequestTypeDef",
+    "ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef",
     "ListCompatibleImagesRequestRequestTypeDef",
+    "ListJobsRequestListJobsPaginateTypeDef",
     "ListJobsRequestRequestTypeDef",
+    "ListLongTermPricingRequestListLongTermPricingPaginateTypeDef",
     "ListLongTermPricingRequestRequestTypeDef",
     "LongTermPricingListEntryTypeDef",
     "ListPickupLocationsRequestRequestTypeDef",
+    "NFSOnDeviceServiceConfigurationOutputTypeDef",
     "NFSOnDeviceServiceConfigurationTypeDef",
+    "S3OnDeviceServiceConfigurationOutputTypeDef",
+    "TGWOnDeviceServiceConfigurationOutputTypeDef",
     "S3OnDeviceServiceConfigurationTypeDef",
     "TGWOnDeviceServiceConfigurationTypeDef",
-    "TimestampTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
+    "TargetOnDeviceServiceOutputTypeDef",
     "TargetOnDeviceServiceTypeDef",
     "ShipmentTypeDef",
+    "WirelessConnectionOutputTypeDef",
     "WirelessConnectionTypeDef",
     "UpdateJobShipmentStateRequestRequestTypeDef",
     "UpdateLongTermPricingRequestRequestTypeDef",
-    "CreateAddressRequestRequestTypeDef",
-    "CreateAddressResultTypeDef",
-    "CreateJobResultTypeDef",
-    "CreateLongTermPricingResultTypeDef",
-    "CreateReturnShippingLabelResultTypeDef",
     "DescribeAddressResultTypeDef",
     "DescribeAddressesResultTypeDef",
-    "DescribeReturnShippingLabelResultTypeDef",
-    "GetJobManifestResultTypeDef",
-    "GetJobUnlockCodeResultTypeDef",
-    "GetSnowballUsageResultTypeDef",
-    "GetSoftwareUpdatesResultTypeDef",
+    "ListPickupLocationsResultTypeDef",
+    "CreateAddressRequestRequestTypeDef",
     "ListClustersResultTypeDef",
     "ListCompatibleImagesResultTypeDef",
-    "ListPickupLocationsResultTypeDef",
-    "NotificationUnionTypeDef",
     "CreateClusterResultTypeDef",
     "ListClusterJobsResultTypeDef",
     "ListJobsResultTypeDef",
+    "DependentServiceOutputTypeDef",
     "DependentServiceTypeDef",
-    "DescribeAddressesRequestDescribeAddressesPaginateTypeDef",
-    "ListClusterJobsRequestListClusterJobsPaginateTypeDef",
-    "ListClustersRequestListClustersPaginateTypeDef",
-    "ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef",
-    "ListJobsRequestListJobsPaginateTypeDef",
-    "ListLongTermPricingRequestListLongTermPricingPaginateTypeDef",
     "LambdaResourceOutputTypeDef",
     "LambdaResourceTypeDef",
+    "TaxDocumentsOutputTypeDef",
     "TaxDocumentsTypeDef",
     "ListLongTermPricingResultTypeDef",
+    "OnDeviceServiceConfigurationOutputTypeDef",
     "OnDeviceServiceConfigurationTypeDef",
-    "PickupDetailsTypeDef",
     "S3ResourceOutputTypeDef",
     "S3ResourceTypeDef",
     "ShippingDetailsTypeDef",
+    "SnowconeDeviceConfigurationOutputTypeDef",
     "SnowconeDeviceConfigurationTypeDef",
-    "ListServiceVersionsRequestRequestTypeDef",
     "ListServiceVersionsResultTypeDef",
-    "PickupDetailsUnionTypeDef",
+    "ListServiceVersionsRequestRequestTypeDef",
     "JobResourceOutputTypeDef",
     "JobResourceTypeDef",
+    "DeviceConfigurationOutputTypeDef",
     "DeviceConfigurationTypeDef",
     "ClusterMetadataTypeDef",
     "CreateClusterRequestRequestTypeDef",
-    "JobResourceUnionTypeDef",
     "UpdateClusterRequestRequestTypeDef",
     "UpdateJobRequestRequestTypeDef",
-    "CreateJobRequestRequestTypeDef",
     "JobMetadataTypeDef",
+    "CreateJobRequestRequestTypeDef",
     "DescribeClusterResultTypeDef",
     "DescribeJobResultTypeDef",
 )
 
+AddressOutputTypeDef = TypedDict(
+    "AddressOutputTypeDef",
+    {
+        "AddressId": str,
+        "Name": str,
+        "Company": str,
+        "Street1": str,
+        "Street2": str,
+        "Street3": str,
+        "City": str,
+        "StateOrProvince": str,
+        "PrefectureOrDistrict": str,
+        "Landmark": str,
+        "Country": str,
+        "PostalCode": str,
+        "PhoneNumber": str,
+        "IsRestricted": bool,
+        "Type": AddressTypeType,
+    },
+)
+
 AddressTypeDef = TypedDict(
     "AddressTypeDef",
     {
         "AddressId": str,
         "Name": str,
         "Company": str,
         "Street1": str,
@@ -181,45 +215,39 @@
     "ClusterListEntryTypeDef",
     {
         "ClusterId": str,
         "ClusterState": ClusterStateType,
         "CreationDate": datetime,
         "Description": str,
     },
-    total=False,
 )
 
 NotificationOutputTypeDef = TypedDict(
     "NotificationOutputTypeDef",
     {
         "SnsTopicARN": str,
         "JobStatesToNotify": List[JobStateType],
         "NotifyAll": bool,
         "DevicePickupSnsTopicARN": str,
     },
-    total=False,
 )
 
 CompatibleImageTypeDef = TypedDict(
     "CompatibleImageTypeDef",
     {
         "AmiId": str,
         "Name": str,
     },
-    total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateAddressResultTypeDef = TypedDict(
+    "CreateAddressResultTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "AddressId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 NotificationTypeDef = TypedDict(
     "NotificationTypeDef",
     {
         "SnsTopicARN": str,
@@ -237,17 +265,38 @@
         "JobState": JobStateType,
         "IsMaster": bool,
         "JobType": JobTypeType,
         "SnowballType": SnowballTypeType,
         "CreationDate": datetime,
         "Description": str,
     },
+)
+
+PickupDetailsTypeDef = TypedDict(
+    "PickupDetailsTypeDef",
+    {
+        "Name": str,
+        "PhoneNumber": str,
+        "Email": str,
+        "IdentificationNumber": str,
+        "IdentificationExpirationDate": Union[datetime, str],
+        "IdentificationIssuingOrg": str,
+        "DevicePickupId": str,
+    },
     total=False,
 )
 
+CreateJobResultTypeDef = TypedDict(
+    "CreateJobResultTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateLongTermPricingRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLongTermPricingRequestRequestTypeDef",
     {
         "LongTermPricingType": LongTermPricingTypeType,
         "SnowballType": SnowballTypeType,
     },
 )
@@ -261,14 +310,22 @@
 
 class CreateLongTermPricingRequestRequestTypeDef(
     _RequiredCreateLongTermPricingRequestRequestTypeDef,
     _OptionalCreateLongTermPricingRequestRequestTypeDef,
 ):
     pass
 
+CreateLongTermPricingResultTypeDef = TypedDict(
+    "CreateLongTermPricingResultTypeDef",
+    {
+        "LongTermPricingId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateReturnShippingLabelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateReturnShippingLabelRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 _OptionalCreateReturnShippingLabelRequestRequestTypeDef = TypedDict(
@@ -281,23 +338,37 @@
 
 class CreateReturnShippingLabelRequestRequestTypeDef(
     _RequiredCreateReturnShippingLabelRequestRequestTypeDef,
     _OptionalCreateReturnShippingLabelRequestRequestTypeDef,
 ):
     pass
 
+CreateReturnShippingLabelResultTypeDef = TypedDict(
+    "CreateReturnShippingLabelResultTypeDef",
+    {
+        "Status": ShippingLabelStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DataTransferTypeDef = TypedDict(
     "DataTransferTypeDef",
     {
         "BytesTransferred": int,
         "ObjectsTransferred": int,
         "TotalBytes": int,
         "TotalObjects": int,
     },
-    total=False,
+)
+
+ServiceVersionOutputTypeDef = TypedDict(
+    "ServiceVersionOutputTypeDef",
+    {
+        "Version": str,
+    },
 )
 
 ServiceVersionTypeDef = TypedDict(
     "ServiceVersionTypeDef",
     {
         "Version": str,
     },
@@ -307,20 +378,18 @@
 DescribeAddressRequestRequestTypeDef = TypedDict(
     "DescribeAddressRequestRequestTypeDef",
     {
         "AddressId": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DescribeAddressesRequestDescribeAddressesPaginateTypeDef = TypedDict(
+    "DescribeAddressesRequestDescribeAddressesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeAddressesRequestRequestTypeDef = TypedDict(
     "DescribeAddressesRequestRequestTypeDef",
     {
@@ -347,23 +416,49 @@
 DescribeReturnShippingLabelRequestRequestTypeDef = TypedDict(
     "DescribeReturnShippingLabelRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
+DescribeReturnShippingLabelResultTypeDef = TypedDict(
+    "DescribeReturnShippingLabelResultTypeDef",
+    {
+        "Status": ShippingLabelStatusType,
+        "ExpirationDate": datetime,
+        "ReturnShippingLabelURI": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+EKSOnDeviceServiceConfigurationOutputTypeDef = TypedDict(
+    "EKSOnDeviceServiceConfigurationOutputTypeDef",
+    {
+        "KubernetesVersion": str,
+        "EKSAnywhereVersion": str,
+    },
+)
+
 EKSOnDeviceServiceConfigurationTypeDef = TypedDict(
     "EKSOnDeviceServiceConfigurationTypeDef",
     {
         "KubernetesVersion": str,
         "EKSAnywhereVersion": str,
     },
     total=False,
 )
 
+Ec2AmiResourceOutputTypeDef = TypedDict(
+    "Ec2AmiResourceOutputTypeDef",
+    {
+        "AmiId": str,
+        "SnowballAmiId": str,
+    },
+)
+
 _RequiredEc2AmiResourceTypeDef = TypedDict(
     "_RequiredEc2AmiResourceTypeDef",
     {
         "AmiId": str,
     },
 )
 _OptionalEc2AmiResourceTypeDef = TypedDict(
@@ -373,14 +468,21 @@
     },
     total=False,
 )
 
 class Ec2AmiResourceTypeDef(_RequiredEc2AmiResourceTypeDef, _OptionalEc2AmiResourceTypeDef):
     pass
 
+EventTriggerDefinitionOutputTypeDef = TypedDict(
+    "EventTriggerDefinitionOutputTypeDef",
+    {
+        "EventResourceARN": str,
+    },
+)
+
 EventTriggerDefinitionTypeDef = TypedDict(
     "EventTriggerDefinitionTypeDef",
     {
         "EventResourceARN": str,
     },
     total=False,
 )
@@ -388,28 +490,68 @@
 GetJobManifestRequestRequestTypeDef = TypedDict(
     "GetJobManifestRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
+GetJobManifestResultTypeDef = TypedDict(
+    "GetJobManifestResultTypeDef",
+    {
+        "ManifestURI": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetJobUnlockCodeRequestRequestTypeDef = TypedDict(
     "GetJobUnlockCodeRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
+GetJobUnlockCodeResultTypeDef = TypedDict(
+    "GetJobUnlockCodeResultTypeDef",
+    {
+        "UnlockCode": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetSnowballUsageResultTypeDef = TypedDict(
+    "GetSnowballUsageResultTypeDef",
+    {
+        "SnowballLimit": int,
+        "SnowballsInUse": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetSoftwareUpdatesRequestRequestTypeDef = TypedDict(
     "GetSoftwareUpdatesRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
+GetSoftwareUpdatesResultTypeDef = TypedDict(
+    "GetSoftwareUpdatesResultTypeDef",
+    {
+        "UpdatesURI": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+INDTaxDocumentsOutputTypeDef = TypedDict(
+    "INDTaxDocumentsOutputTypeDef",
+    {
+        "GSTIN": str,
+    },
+)
+
 INDTaxDocumentsTypeDef = TypedDict(
     "INDTaxDocumentsTypeDef",
     {
         "GSTIN": str,
     },
     total=False,
 )
@@ -417,40 +559,66 @@
 JobLogsTypeDef = TypedDict(
     "JobLogsTypeDef",
     {
         "JobCompletionReportURI": str,
         "JobSuccessLogURI": str,
         "JobFailureLogURI": str,
     },
-    total=False,
 )
 
 PickupDetailsOutputTypeDef = TypedDict(
     "PickupDetailsOutputTypeDef",
     {
         "Name": str,
         "PhoneNumber": str,
         "Email": str,
         "IdentificationNumber": str,
         "IdentificationExpirationDate": datetime,
         "IdentificationIssuingOrg": str,
         "DevicePickupId": str,
     },
-    total=False,
+)
+
+KeyRangeOutputTypeDef = TypedDict(
+    "KeyRangeOutputTypeDef",
+    {
+        "BeginMarker": str,
+        "EndMarker": str,
+    },
 )
 
 KeyRangeTypeDef = TypedDict(
     "KeyRangeTypeDef",
     {
         "BeginMarker": str,
         "EndMarker": str,
     },
     total=False,
 )
 
+_RequiredListClusterJobsRequestListClusterJobsPaginateTypeDef = TypedDict(
+    "_RequiredListClusterJobsRequestListClusterJobsPaginateTypeDef",
+    {
+        "ClusterId": str,
+    },
+)
+_OptionalListClusterJobsRequestListClusterJobsPaginateTypeDef = TypedDict(
+    "_OptionalListClusterJobsRequestListClusterJobsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListClusterJobsRequestListClusterJobsPaginateTypeDef(
+    _RequiredListClusterJobsRequestListClusterJobsPaginateTypeDef,
+    _OptionalListClusterJobsRequestListClusterJobsPaginateTypeDef,
+):
+    pass
+
 _RequiredListClusterJobsRequestRequestTypeDef = TypedDict(
     "_RequiredListClusterJobsRequestRequestTypeDef",
     {
         "ClusterId": str,
     },
 )
 _OptionalListClusterJobsRequestRequestTypeDef = TypedDict(
@@ -463,41 +631,73 @@
 )
 
 class ListClusterJobsRequestRequestTypeDef(
     _RequiredListClusterJobsRequestRequestTypeDef, _OptionalListClusterJobsRequestRequestTypeDef
 ):
     pass
 
+ListClustersRequestListClustersPaginateTypeDef = TypedDict(
+    "ListClustersRequestListClustersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListClustersRequestRequestTypeDef = TypedDict(
     "ListClustersRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef = TypedDict(
+    "ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListCompatibleImagesRequestRequestTypeDef = TypedDict(
     "ListCompatibleImagesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListJobsRequestListJobsPaginateTypeDef = TypedDict(
+    "ListJobsRequestListJobsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListJobsRequestRequestTypeDef = TypedDict(
     "ListJobsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListLongTermPricingRequestListLongTermPricingPaginateTypeDef = TypedDict(
+    "ListLongTermPricingRequestListLongTermPricingPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListLongTermPricingRequestRequestTypeDef = TypedDict(
     "ListLongTermPricingRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -513,35 +713,60 @@
         "CurrentActiveJob": str,
         "ReplacementJob": str,
         "IsLongTermPricingAutoRenew": bool,
         "LongTermPricingStatus": str,
         "SnowballType": SnowballTypeType,
         "JobIds": List[str],
     },
-    total=False,
 )
 
 ListPickupLocationsRequestRequestTypeDef = TypedDict(
     "ListPickupLocationsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+NFSOnDeviceServiceConfigurationOutputTypeDef = TypedDict(
+    "NFSOnDeviceServiceConfigurationOutputTypeDef",
+    {
+        "StorageLimit": int,
+        "StorageUnit": Literal["TB"],
+    },
+)
+
 NFSOnDeviceServiceConfigurationTypeDef = TypedDict(
     "NFSOnDeviceServiceConfigurationTypeDef",
     {
         "StorageLimit": int,
         "StorageUnit": Literal["TB"],
     },
     total=False,
 )
 
+S3OnDeviceServiceConfigurationOutputTypeDef = TypedDict(
+    "S3OnDeviceServiceConfigurationOutputTypeDef",
+    {
+        "StorageLimit": float,
+        "StorageUnit": Literal["TB"],
+        "ServiceSize": int,
+        "FaultTolerance": int,
+    },
+)
+
+TGWOnDeviceServiceConfigurationOutputTypeDef = TypedDict(
+    "TGWOnDeviceServiceConfigurationOutputTypeDef",
+    {
+        "StorageLimit": int,
+        "StorageUnit": Literal["TB"],
+    },
+)
+
 S3OnDeviceServiceConfigurationTypeDef = TypedDict(
     "S3OnDeviceServiceConfigurationTypeDef",
     {
         "StorageLimit": float,
         "StorageUnit": Literal["TB"],
         "ServiceSize": int,
         "FaultTolerance": int,
@@ -554,15 +779,43 @@
     {
         "StorageLimit": int,
         "StorageUnit": Literal["TB"],
     },
     total=False,
 )
 
-TimestampTypeDef = Union[datetime, str]
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
+)
+
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
+TargetOnDeviceServiceOutputTypeDef = TypedDict(
+    "TargetOnDeviceServiceOutputTypeDef",
+    {
+        "ServiceName": DeviceServiceNameType,
+        "TransferOption": TransferOptionType,
+    },
+)
+
 TargetOnDeviceServiceTypeDef = TypedDict(
     "TargetOnDeviceServiceTypeDef",
     {
         "ServiceName": DeviceServiceNameType,
         "TransferOption": TransferOptionType,
     },
     total=False,
@@ -570,15 +823,21 @@
 
 ShipmentTypeDef = TypedDict(
     "ShipmentTypeDef",
     {
         "Status": str,
         "TrackingNumber": str,
     },
-    total=False,
+)
+
+WirelessConnectionOutputTypeDef = TypedDict(
+    "WirelessConnectionOutputTypeDef",
+    {
+        "IsWifiEnabled": bool,
+    },
 )
 
 WirelessConnectionTypeDef = TypedDict(
     "WirelessConnectionTypeDef",
     {
         "IsWifiEnabled": bool,
     },
@@ -610,305 +869,178 @@
 
 class UpdateLongTermPricingRequestRequestTypeDef(
     _RequiredUpdateLongTermPricingRequestRequestTypeDef,
     _OptionalUpdateLongTermPricingRequestRequestTypeDef,
 ):
     pass
 
-CreateAddressRequestRequestTypeDef = TypedDict(
-    "CreateAddressRequestRequestTypeDef",
-    {
-        "Address": AddressTypeDef,
-    },
-)
-
-CreateAddressResultTypeDef = TypedDict(
-    "CreateAddressResultTypeDef",
-    {
-        "AddressId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateJobResultTypeDef = TypedDict(
-    "CreateJobResultTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateLongTermPricingResultTypeDef = TypedDict(
-    "CreateLongTermPricingResultTypeDef",
-    {
-        "LongTermPricingId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateReturnShippingLabelResultTypeDef = TypedDict(
-    "CreateReturnShippingLabelResultTypeDef",
-    {
-        "Status": ShippingLabelStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DescribeAddressResultTypeDef = TypedDict(
     "DescribeAddressResultTypeDef",
     {
-        "Address": AddressTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Address": AddressOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeAddressesResultTypeDef = TypedDict(
     "DescribeAddressesResultTypeDef",
     {
-        "Addresses": List[AddressTypeDef],
+        "Addresses": List[AddressOutputTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeReturnShippingLabelResultTypeDef = TypedDict(
-    "DescribeReturnShippingLabelResultTypeDef",
-    {
-        "Status": ShippingLabelStatusType,
-        "ExpirationDate": datetime,
-        "ReturnShippingLabelURI": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetJobManifestResultTypeDef = TypedDict(
-    "GetJobManifestResultTypeDef",
-    {
-        "ManifestURI": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetJobUnlockCodeResultTypeDef = TypedDict(
-    "GetJobUnlockCodeResultTypeDef",
-    {
-        "UnlockCode": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetSnowballUsageResultTypeDef = TypedDict(
-    "GetSnowballUsageResultTypeDef",
+ListPickupLocationsResultTypeDef = TypedDict(
+    "ListPickupLocationsResultTypeDef",
     {
-        "SnowballLimit": int,
-        "SnowballsInUse": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Addresses": List[AddressOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetSoftwareUpdatesResultTypeDef = TypedDict(
-    "GetSoftwareUpdatesResultTypeDef",
+CreateAddressRequestRequestTypeDef = TypedDict(
+    "CreateAddressRequestRequestTypeDef",
     {
-        "UpdatesURI": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Address": AddressTypeDef,
     },
 )
 
 ListClustersResultTypeDef = TypedDict(
     "ListClustersResultTypeDef",
     {
         "ClusterListEntries": List[ClusterListEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListCompatibleImagesResultTypeDef = TypedDict(
     "ListCompatibleImagesResultTypeDef",
     {
         "CompatibleImages": List[CompatibleImageTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListPickupLocationsResultTypeDef = TypedDict(
-    "ListPickupLocationsResultTypeDef",
-    {
-        "Addresses": List[AddressTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-NotificationUnionTypeDef = Union[NotificationTypeDef, NotificationOutputTypeDef]
 CreateClusterResultTypeDef = TypedDict(
     "CreateClusterResultTypeDef",
     {
         "ClusterId": str,
         "JobListEntries": List[JobListEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListClusterJobsResultTypeDef = TypedDict(
     "ListClusterJobsResultTypeDef",
     {
         "JobListEntries": List[JobListEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListJobsResultTypeDef = TypedDict(
     "ListJobsResultTypeDef",
     {
         "JobListEntries": List[JobListEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DependentServiceTypeDef = TypedDict(
-    "DependentServiceTypeDef",
+DependentServiceOutputTypeDef = TypedDict(
+    "DependentServiceOutputTypeDef",
     {
         "ServiceName": ServiceNameType,
-        "ServiceVersion": ServiceVersionTypeDef,
+        "ServiceVersion": ServiceVersionOutputTypeDef,
     },
-    total=False,
 )
 
-DescribeAddressesRequestDescribeAddressesPaginateTypeDef = TypedDict(
-    "DescribeAddressesRequestDescribeAddressesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListClusterJobsRequestListClusterJobsPaginateTypeDef = TypedDict(
-    "_RequiredListClusterJobsRequestListClusterJobsPaginateTypeDef",
-    {
-        "ClusterId": str,
-    },
-)
-_OptionalListClusterJobsRequestListClusterJobsPaginateTypeDef = TypedDict(
-    "_OptionalListClusterJobsRequestListClusterJobsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListClusterJobsRequestListClusterJobsPaginateTypeDef(
-    _RequiredListClusterJobsRequestListClusterJobsPaginateTypeDef,
-    _OptionalListClusterJobsRequestListClusterJobsPaginateTypeDef,
-):
-    pass
-
-ListClustersRequestListClustersPaginateTypeDef = TypedDict(
-    "ListClustersRequestListClustersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef = TypedDict(
-    "ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListJobsRequestListJobsPaginateTypeDef = TypedDict(
-    "ListJobsRequestListJobsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListLongTermPricingRequestListLongTermPricingPaginateTypeDef = TypedDict(
-    "ListLongTermPricingRequestListLongTermPricingPaginateTypeDef",
+DependentServiceTypeDef = TypedDict(
+    "DependentServiceTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ServiceName": ServiceNameType,
+        "ServiceVersion": ServiceVersionTypeDef,
     },
     total=False,
 )
 
 LambdaResourceOutputTypeDef = TypedDict(
     "LambdaResourceOutputTypeDef",
     {
         "LambdaArn": str,
-        "EventTriggers": List[EventTriggerDefinitionTypeDef],
+        "EventTriggers": List[EventTriggerDefinitionOutputTypeDef],
     },
-    total=False,
 )
 
 LambdaResourceTypeDef = TypedDict(
     "LambdaResourceTypeDef",
     {
         "LambdaArn": str,
         "EventTriggers": Sequence[EventTriggerDefinitionTypeDef],
     },
     total=False,
 )
 
+TaxDocumentsOutputTypeDef = TypedDict(
+    "TaxDocumentsOutputTypeDef",
+    {
+        "IND": INDTaxDocumentsOutputTypeDef,
+    },
+)
+
 TaxDocumentsTypeDef = TypedDict(
     "TaxDocumentsTypeDef",
     {
         "IND": INDTaxDocumentsTypeDef,
     },
     total=False,
 )
 
 ListLongTermPricingResultTypeDef = TypedDict(
     "ListLongTermPricingResultTypeDef",
     {
         "LongTermPricingEntries": List[LongTermPricingListEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+OnDeviceServiceConfigurationOutputTypeDef = TypedDict(
+    "OnDeviceServiceConfigurationOutputTypeDef",
+    {
+        "NFSOnDeviceService": NFSOnDeviceServiceConfigurationOutputTypeDef,
+        "TGWOnDeviceService": TGWOnDeviceServiceConfigurationOutputTypeDef,
+        "EKSOnDeviceService": EKSOnDeviceServiceConfigurationOutputTypeDef,
+        "S3OnDeviceService": S3OnDeviceServiceConfigurationOutputTypeDef,
     },
 )
 
 OnDeviceServiceConfigurationTypeDef = TypedDict(
     "OnDeviceServiceConfigurationTypeDef",
     {
         "NFSOnDeviceService": NFSOnDeviceServiceConfigurationTypeDef,
         "TGWOnDeviceService": TGWOnDeviceServiceConfigurationTypeDef,
         "EKSOnDeviceService": EKSOnDeviceServiceConfigurationTypeDef,
         "S3OnDeviceService": S3OnDeviceServiceConfigurationTypeDef,
     },
     total=False,
 )
 
-PickupDetailsTypeDef = TypedDict(
-    "PickupDetailsTypeDef",
-    {
-        "Name": str,
-        "PhoneNumber": str,
-        "Email": str,
-        "IdentificationNumber": str,
-        "IdentificationExpirationDate": TimestampTypeDef,
-        "IdentificationIssuingOrg": str,
-        "DevicePickupId": str,
-    },
-    total=False,
-)
-
 S3ResourceOutputTypeDef = TypedDict(
     "S3ResourceOutputTypeDef",
     {
         "BucketArn": str,
-        "KeyRange": KeyRangeTypeDef,
-        "TargetOnDeviceServices": List[TargetOnDeviceServiceTypeDef],
+        "KeyRange": KeyRangeOutputTypeDef,
+        "TargetOnDeviceServices": List[TargetOnDeviceServiceOutputTypeDef],
     },
-    total=False,
 )
 
 S3ResourceTypeDef = TypedDict(
     "S3ResourceTypeDef",
     {
         "BucketArn": str,
         "KeyRange": KeyRangeTypeDef,
@@ -920,25 +1052,42 @@
 ShippingDetailsTypeDef = TypedDict(
     "ShippingDetailsTypeDef",
     {
         "ShippingOption": ShippingOptionType,
         "InboundShipment": ShipmentTypeDef,
         "OutboundShipment": ShipmentTypeDef,
     },
-    total=False,
+)
+
+SnowconeDeviceConfigurationOutputTypeDef = TypedDict(
+    "SnowconeDeviceConfigurationOutputTypeDef",
+    {
+        "WirelessConnection": WirelessConnectionOutputTypeDef,
+    },
 )
 
 SnowconeDeviceConfigurationTypeDef = TypedDict(
     "SnowconeDeviceConfigurationTypeDef",
     {
         "WirelessConnection": WirelessConnectionTypeDef,
     },
     total=False,
 )
 
+ListServiceVersionsResultTypeDef = TypedDict(
+    "ListServiceVersionsResultTypeDef",
+    {
+        "ServiceVersions": List[ServiceVersionOutputTypeDef],
+        "ServiceName": ServiceNameType,
+        "DependentServices": List[DependentServiceOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredListServiceVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListServiceVersionsRequestRequestTypeDef",
     {
         "ServiceName": ServiceNameType,
     },
 )
 _OptionalListServiceVersionsRequestRequestTypeDef = TypedDict(
@@ -953,46 +1102,40 @@
 
 class ListServiceVersionsRequestRequestTypeDef(
     _RequiredListServiceVersionsRequestRequestTypeDef,
     _OptionalListServiceVersionsRequestRequestTypeDef,
 ):
     pass
 
-ListServiceVersionsResultTypeDef = TypedDict(
-    "ListServiceVersionsResultTypeDef",
-    {
-        "ServiceVersions": List[ServiceVersionTypeDef],
-        "ServiceName": ServiceNameType,
-        "DependentServices": List[DependentServiceTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PickupDetailsUnionTypeDef = Union[PickupDetailsTypeDef, PickupDetailsOutputTypeDef]
 JobResourceOutputTypeDef = TypedDict(
     "JobResourceOutputTypeDef",
     {
         "S3Resources": List[S3ResourceOutputTypeDef],
         "LambdaResources": List[LambdaResourceOutputTypeDef],
-        "Ec2AmiResources": List[Ec2AmiResourceTypeDef],
+        "Ec2AmiResources": List[Ec2AmiResourceOutputTypeDef],
     },
-    total=False,
 )
 
 JobResourceTypeDef = TypedDict(
     "JobResourceTypeDef",
     {
         "S3Resources": Sequence[S3ResourceTypeDef],
         "LambdaResources": Sequence[LambdaResourceTypeDef],
         "Ec2AmiResources": Sequence[Ec2AmiResourceTypeDef],
     },
     total=False,
 )
 
+DeviceConfigurationOutputTypeDef = TypedDict(
+    "DeviceConfigurationOutputTypeDef",
+    {
+        "SnowconeDeviceConfiguration": SnowconeDeviceConfigurationOutputTypeDef,
+    },
+)
+
 DeviceConfigurationTypeDef = TypedDict(
     "DeviceConfigurationTypeDef",
     {
         "SnowconeDeviceConfiguration": SnowconeDeviceConfigurationTypeDef,
     },
     total=False,
 )
@@ -1009,18 +1152,17 @@
         "SnowballType": SnowballTypeType,
         "CreationDate": datetime,
         "Resources": JobResourceOutputTypeDef,
         "AddressId": str,
         "ShippingOption": ShippingOptionType,
         "Notification": NotificationOutputTypeDef,
         "ForwardingAddressId": str,
-        "TaxDocuments": TaxDocumentsTypeDef,
-        "OnDeviceServiceConfiguration": OnDeviceServiceConfigurationTypeDef,
+        "TaxDocuments": TaxDocumentsOutputTypeDef,
+        "OnDeviceServiceConfiguration": OnDeviceServiceConfigurationOutputTypeDef,
     },
-    total=False,
 )
 
 _RequiredCreateClusterRequestRequestTypeDef = TypedDict(
     "_RequiredCreateClusterRequestRequestTypeDef",
     {
         "JobType": JobTypeType,
         "AddressId": str,
@@ -1049,15 +1191,14 @@
 )
 
 class CreateClusterRequestRequestTypeDef(
     _RequiredCreateClusterRequestRequestTypeDef, _OptionalCreateClusterRequestRequestTypeDef
 ):
     pass
 
-JobResourceUnionTypeDef = Union[JobResourceTypeDef, JobResourceOutputTypeDef]
 _RequiredUpdateClusterRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateClusterRequestRequestTypeDef",
     {
         "ClusterId": str,
     },
 )
 _OptionalUpdateClusterRequestRequestTypeDef = TypedDict(
@@ -1104,81 +1245,80 @@
 )
 
 class UpdateJobRequestRequestTypeDef(
     _RequiredUpdateJobRequestRequestTypeDef, _OptionalUpdateJobRequestRequestTypeDef
 ):
     pass
 
-CreateJobRequestRequestTypeDef = TypedDict(
-    "CreateJobRequestRequestTypeDef",
+JobMetadataTypeDef = TypedDict(
+    "JobMetadataTypeDef",
     {
+        "JobId": str,
+        "JobState": JobStateType,
         "JobType": JobTypeType,
-        "Resources": JobResourceTypeDef,
-        "OnDeviceServiceConfiguration": OnDeviceServiceConfigurationTypeDef,
+        "SnowballType": SnowballTypeType,
+        "CreationDate": datetime,
+        "Resources": JobResourceOutputTypeDef,
         "Description": str,
-        "AddressId": str,
         "KmsKeyARN": str,
         "RoleARN": str,
+        "AddressId": str,
+        "ShippingDetails": ShippingDetailsTypeDef,
         "SnowballCapacityPreference": SnowballCapacityType,
-        "ShippingOption": ShippingOptionType,
-        "Notification": NotificationTypeDef,
+        "Notification": NotificationOutputTypeDef,
+        "DataTransferProgress": DataTransferTypeDef,
+        "JobLogInfo": JobLogsTypeDef,
         "ClusterId": str,
-        "SnowballType": SnowballTypeType,
         "ForwardingAddressId": str,
-        "TaxDocuments": TaxDocumentsTypeDef,
-        "DeviceConfiguration": DeviceConfigurationTypeDef,
+        "TaxDocuments": TaxDocumentsOutputTypeDef,
+        "DeviceConfiguration": DeviceConfigurationOutputTypeDef,
         "RemoteManagement": RemoteManagementType,
         "LongTermPricingId": str,
+        "OnDeviceServiceConfiguration": OnDeviceServiceConfigurationOutputTypeDef,
         "ImpactLevel": ImpactLevelType,
-        "PickupDetails": PickupDetailsTypeDef,
+        "PickupDetails": PickupDetailsOutputTypeDef,
+        "SnowballId": str,
     },
-    total=False,
 )
 
-JobMetadataTypeDef = TypedDict(
-    "JobMetadataTypeDef",
+CreateJobRequestRequestTypeDef = TypedDict(
+    "CreateJobRequestRequestTypeDef",
     {
-        "JobId": str,
-        "JobState": JobStateType,
         "JobType": JobTypeType,
-        "SnowballType": SnowballTypeType,
-        "CreationDate": datetime,
-        "Resources": JobResourceOutputTypeDef,
+        "Resources": JobResourceTypeDef,
+        "OnDeviceServiceConfiguration": OnDeviceServiceConfigurationTypeDef,
         "Description": str,
+        "AddressId": str,
         "KmsKeyARN": str,
         "RoleARN": str,
-        "AddressId": str,
-        "ShippingDetails": ShippingDetailsTypeDef,
         "SnowballCapacityPreference": SnowballCapacityType,
-        "Notification": NotificationOutputTypeDef,
-        "DataTransferProgress": DataTransferTypeDef,
-        "JobLogInfo": JobLogsTypeDef,
+        "ShippingOption": ShippingOptionType,
+        "Notification": NotificationTypeDef,
         "ClusterId": str,
+        "SnowballType": SnowballTypeType,
         "ForwardingAddressId": str,
         "TaxDocuments": TaxDocumentsTypeDef,
         "DeviceConfiguration": DeviceConfigurationTypeDef,
         "RemoteManagement": RemoteManagementType,
         "LongTermPricingId": str,
-        "OnDeviceServiceConfiguration": OnDeviceServiceConfigurationTypeDef,
         "ImpactLevel": ImpactLevelType,
-        "PickupDetails": PickupDetailsOutputTypeDef,
-        "SnowballId": str,
+        "PickupDetails": PickupDetailsTypeDef,
     },
     total=False,
 )
 
 DescribeClusterResultTypeDef = TypedDict(
     "DescribeClusterResultTypeDef",
     {
         "ClusterMetadata": ClusterMetadataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeJobResultTypeDef = TypedDict(
     "DescribeJobResultTypeDef",
     {
         "JobMetadata": JobMetadataTypeDef,
         "SubJobMetadata": List[JobMetadataTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-snowball-1.28.16/mypy_boto3_snowball.egg-info/PKG-INFO` & `mypy-boto3-snowball-1.28.5/mypy_boto3_snowball.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-snowball
-Version: 1.28.16
-Summary: Type annotations for boto3.Snowball 1.28.16 service generated with mypy-boto3-builder 7.17.1
+Version: 1.28.5
+Summary: Type annotations for boto3.Snowball 1.28.5 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 snowball type-annotations botocore mypy typeshed autocomplete
+Keywords: boto3 snowball type-annotations boto3-stubs mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-snowball"></a>
 
 # mypy-boto3-snowball
 
 [![PyPI - mypy-boto3-snowball](https://img.shields.io/pypi/v/mypy-boto3-snowball.svg?color=blue)](https://pypi.org/project/mypy-boto3-snowball)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-snowball.svg?color=blue)](https://pypi.org/project/mypy-boto3-snowball)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-snowball)](https://pepy.tech/project/mypy-boto3-snowball)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-snowball?color=blue)](https://pypistats.org/packages/mypy-boto3-snowball)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Snowball 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball)
+[boto3.Snowball 1.28.5](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball)
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
 [mypy-boto3-snowball docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/).
 
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
@@ -348,123 +348,136 @@
 )
 
 
 def check_value(value: AddressTypeType) -> bool:
     ...
 ```
 
-<a id="type-definitions"></a>
+<a id="typed-dictionaries"></a>
 
-### Type definitions
+### Typed dictionaries
 
 `mypy_boto3_snowball.type_defs` module contains structures and shapes assembled
-to typed dictionaries and unions for additional type checking.
+to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_snowball.type_defs import (
+    AddressOutputTypeDef,
     AddressTypeDef,
     CancelClusterRequestRequestTypeDef,
     CancelJobRequestRequestTypeDef,
     ClusterListEntryTypeDef,
     NotificationOutputTypeDef,
     CompatibleImageTypeDef,
-    ResponseMetadataTypeDef,
+    CreateAddressResultTypeDef,
     NotificationTypeDef,
     JobListEntryTypeDef,
+    PickupDetailsTypeDef,
+    CreateJobResultTypeDef,
     CreateLongTermPricingRequestRequestTypeDef,
+    CreateLongTermPricingResultTypeDef,
     CreateReturnShippingLabelRequestRequestTypeDef,
+    CreateReturnShippingLabelResultTypeDef,
     DataTransferTypeDef,
+    ServiceVersionOutputTypeDef,
     ServiceVersionTypeDef,
     DescribeAddressRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeAddressesRequestDescribeAddressesPaginateTypeDef,
     DescribeAddressesRequestRequestTypeDef,
     DescribeClusterRequestRequestTypeDef,
     DescribeJobRequestRequestTypeDef,
     DescribeReturnShippingLabelRequestRequestTypeDef,
+    DescribeReturnShippingLabelResultTypeDef,
+    EKSOnDeviceServiceConfigurationOutputTypeDef,
     EKSOnDeviceServiceConfigurationTypeDef,
+    Ec2AmiResourceOutputTypeDef,
     Ec2AmiResourceTypeDef,
+    EventTriggerDefinitionOutputTypeDef,
     EventTriggerDefinitionTypeDef,
     GetJobManifestRequestRequestTypeDef,
+    GetJobManifestResultTypeDef,
     GetJobUnlockCodeRequestRequestTypeDef,
+    GetJobUnlockCodeResultTypeDef,
+    GetSnowballUsageResultTypeDef,
     GetSoftwareUpdatesRequestRequestTypeDef,
+    GetSoftwareUpdatesResultTypeDef,
+    INDTaxDocumentsOutputTypeDef,
     INDTaxDocumentsTypeDef,
     JobLogsTypeDef,
     PickupDetailsOutputTypeDef,
+    KeyRangeOutputTypeDef,
     KeyRangeTypeDef,
+    ListClusterJobsRequestListClusterJobsPaginateTypeDef,
     ListClusterJobsRequestRequestTypeDef,
+    ListClustersRequestListClustersPaginateTypeDef,
     ListClustersRequestRequestTypeDef,
+    ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef,
     ListCompatibleImagesRequestRequestTypeDef,
+    ListJobsRequestListJobsPaginateTypeDef,
     ListJobsRequestRequestTypeDef,
+    ListLongTermPricingRequestListLongTermPricingPaginateTypeDef,
     ListLongTermPricingRequestRequestTypeDef,
     LongTermPricingListEntryTypeDef,
     ListPickupLocationsRequestRequestTypeDef,
+    NFSOnDeviceServiceConfigurationOutputTypeDef,
     NFSOnDeviceServiceConfigurationTypeDef,
+    S3OnDeviceServiceConfigurationOutputTypeDef,
+    TGWOnDeviceServiceConfigurationOutputTypeDef,
     S3OnDeviceServiceConfigurationTypeDef,
     TGWOnDeviceServiceConfigurationTypeDef,
-    TimestampTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
+    TargetOnDeviceServiceOutputTypeDef,
     TargetOnDeviceServiceTypeDef,
     ShipmentTypeDef,
+    WirelessConnectionOutputTypeDef,
     WirelessConnectionTypeDef,
     UpdateJobShipmentStateRequestRequestTypeDef,
     UpdateLongTermPricingRequestRequestTypeDef,
-    CreateAddressRequestRequestTypeDef,
-    CreateAddressResultTypeDef,
-    CreateJobResultTypeDef,
-    CreateLongTermPricingResultTypeDef,
-    CreateReturnShippingLabelResultTypeDef,
     DescribeAddressResultTypeDef,
     DescribeAddressesResultTypeDef,
-    DescribeReturnShippingLabelResultTypeDef,
-    GetJobManifestResultTypeDef,
-    GetJobUnlockCodeResultTypeDef,
-    GetSnowballUsageResultTypeDef,
-    GetSoftwareUpdatesResultTypeDef,
+    ListPickupLocationsResultTypeDef,
+    CreateAddressRequestRequestTypeDef,
     ListClustersResultTypeDef,
     ListCompatibleImagesResultTypeDef,
-    ListPickupLocationsResultTypeDef,
-    NotificationUnionTypeDef,
     CreateClusterResultTypeDef,
     ListClusterJobsResultTypeDef,
     ListJobsResultTypeDef,
+    DependentServiceOutputTypeDef,
     DependentServiceTypeDef,
-    DescribeAddressesRequestDescribeAddressesPaginateTypeDef,
-    ListClusterJobsRequestListClusterJobsPaginateTypeDef,
-    ListClustersRequestListClustersPaginateTypeDef,
-    ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef,
-    ListJobsRequestListJobsPaginateTypeDef,
-    ListLongTermPricingRequestListLongTermPricingPaginateTypeDef,
     LambdaResourceOutputTypeDef,
     LambdaResourceTypeDef,
+    TaxDocumentsOutputTypeDef,
     TaxDocumentsTypeDef,
     ListLongTermPricingResultTypeDef,
+    OnDeviceServiceConfigurationOutputTypeDef,
     OnDeviceServiceConfigurationTypeDef,
-    PickupDetailsTypeDef,
     S3ResourceOutputTypeDef,
     S3ResourceTypeDef,
     ShippingDetailsTypeDef,
+    SnowconeDeviceConfigurationOutputTypeDef,
     SnowconeDeviceConfigurationTypeDef,
-    ListServiceVersionsRequestRequestTypeDef,
     ListServiceVersionsResultTypeDef,
-    PickupDetailsUnionTypeDef,
+    ListServiceVersionsRequestRequestTypeDef,
     JobResourceOutputTypeDef,
     JobResourceTypeDef,
+    DeviceConfigurationOutputTypeDef,
     DeviceConfigurationTypeDef,
     ClusterMetadataTypeDef,
     CreateClusterRequestRequestTypeDef,
-    JobResourceUnionTypeDef,
     UpdateClusterRequestRequestTypeDef,
     UpdateJobRequestRequestTypeDef,
-    CreateJobRequestRequestTypeDef,
     JobMetadataTypeDef,
+    CreateJobRequestRequestTypeDef,
     DescribeClusterResultTypeDef,
     DescribeJobResultTypeDef,
 )
 
 
-def get_value() -> AddressTypeDef:
+def get_structure() -> AddressOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-snowball-1.28.16/mypy_boto3_snowball.egg-info/SOURCES.txt` & `mypy-boto3-snowball-1.28.5/mypy_boto3_snowball.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-snowball-1.28.16/setup.py` & `mypy-boto3-snowball-1.28.5/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-snowball",
-    version="1.28.16",
+    version="1.28.5",
     packages=["mypy_boto3_snowball"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Snowball 1.28.16 service generated with mypy-boto3-builder"
-        " 7.17.1"
+        "Type annotations for boto3.Snowball 1.28.5 service generated with mypy-boto3-builder"
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
-    keywords="boto3 snowball type-annotations botocore mypy typeshed autocomplete",
+    keywords="boto3 snowball type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_snowball": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

