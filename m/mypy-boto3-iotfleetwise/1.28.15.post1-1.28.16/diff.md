# Comparing `tmp/mypy-boto3-iotfleetwise-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-iotfleetwise-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iotfleetwise-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:21 2023, max compression
+gzip compressed data, was "mypy-boto3-iotfleetwise-1.28.16.tar", last modified: Tue Aug  1 11:37:02 2023, max compression
```

## Comparing `mypy-boto3-iotfleetwise-1.28.15.post1.tar` & `mypy-boto3-iotfleetwise-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:21.805189 mypy-boto3-iotfleetwise-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:48:00.000000 mypy-boto3-iotfleetwise-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21522 2023-07-29 10:03:21.793189 mypy-boto3-iotfleetwise-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20009 2023-07-29 09:48:00.000000 mypy-boto3-iotfleetwise-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:21.789189 mypy-boto3-iotfleetwise-1.28.15.post1/mypy_boto3_iotfleetwise/
--rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-07-29 09:48:00.000000 mypy-boto3-iotfleetwise-1.28.15.post1/mypy_boto3_iotfleetwise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-07-29 09:48:00.000000 mypy-boto3-iotfleetwise-1.28.15.post1/mypy_boto3_iotfleetwise/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-29 09:48:00.000000 mypy-boto3-iotfleetwise-1.28.15.post1/mypy_boto3_iotfleetwise/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40971 2023-07-29 09:48:01.000000 mypy-boto3-iotfleetwise-1.28.15.post1/mypy_boto3_iotfleetwise/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    40901 2023-07-29 09:48:01.000000 mypy-boto3-iotfleetwise-1.28.15.post1/mypy_boto3_iotfleetwise/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11507 2023-07-29 09:48:01.000000 mypy-boto3-iotfleetwise-1.28.15.post1/mypy_boto3_iotfleetwise/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11505 2023-07-29 09:48:01.000000 mypy-boto3-iotfleetwise-1.28.15.post1/mypy_boto3_iotfleetwise/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15488 2023-07-29 09:48:01.000000 mypy-boto3-iotfleetwise-1.28.15.post1/mypy_boto3_iotfleetwise/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15473 2023-07-29 09:48:01.000000 mypy-boto3-iotfleetwise-1.28.15.post1/mypy_boto3_iotfleetwise/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:48:00.000000 mypy-boto3-iotfleetwise-1.28.15.post1/mypy_boto3_iotfleetwise/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    60350 2023-07-29 09:48:03.000000 mypy-boto3-iotfleetwise-1.28.15.post1/mypy_boto3_iotfleetwise/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    60244 2023-07-29 09:48:02.000000 mypy-boto3-iotfleetwise-1.28.15.post1/mypy_boto3_iotfleetwise/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:48:00.000000 mypy-boto3-iotfleetwise-1.28.15.post1/mypy_boto3_iotfleetwise/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:21.793189 mypy-boto3-iotfleetwise-1.28.15.post1/mypy_boto3_iotfleetwise.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21522 2023-07-29 10:03:21.000000 mypy-boto3-iotfleetwise-1.28.15.post1/mypy_boto3_iotfleetwise.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-29 10:03:21.000000 mypy-boto3-iotfleetwise-1.28.15.post1/mypy_boto3_iotfleetwise.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:21.000000 mypy-boto3-iotfleetwise-1.28.15.post1/mypy_boto3_iotfleetwise.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:21.000000 mypy-boto3-iotfleetwise-1.28.15.post1/mypy_boto3_iotfleetwise.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:21.000000 mypy-boto3-iotfleetwise-1.28.15.post1/mypy_boto3_iotfleetwise.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-29 10:03:21.000000 mypy-boto3-iotfleetwise-1.28.15.post1/mypy_boto3_iotfleetwise.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:21.805189 mypy-boto3-iotfleetwise-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-29 09:48:00.000000 mypy-boto3-iotfleetwise-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:02.292861 mypy-boto3-iotfleetwise-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:20:43.000000 mypy-boto3-iotfleetwise-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21573 2023-08-01 11:37:02.280861 mypy-boto3-iotfleetwise-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20069 2023-08-01 11:20:43.000000 mypy-boto3-iotfleetwise-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:02.272861 mypy-boto3-iotfleetwise-1.28.16/mypy_boto3_iotfleetwise/
+-rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-08-01 11:20:44.000000 mypy-boto3-iotfleetwise-1.28.16/mypy_boto3_iotfleetwise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-08-01 11:20:44.000000 mypy-boto3-iotfleetwise-1.28.16/mypy_boto3_iotfleetwise/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-01 11:20:44.000000 mypy-boto3-iotfleetwise-1.28.16/mypy_boto3_iotfleetwise/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40867 2023-08-01 11:20:44.000000 mypy-boto3-iotfleetwise-1.28.16/mypy_boto3_iotfleetwise/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40797 2023-08-01 11:20:44.000000 mypy-boto3-iotfleetwise-1.28.16/mypy_boto3_iotfleetwise/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11507 2023-08-01 11:20:44.000000 mypy-boto3-iotfleetwise-1.28.16/mypy_boto3_iotfleetwise/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11505 2023-08-01 11:20:44.000000 mypy-boto3-iotfleetwise-1.28.16/mypy_boto3_iotfleetwise/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15488 2023-08-01 11:20:44.000000 mypy-boto3-iotfleetwise-1.28.16/mypy_boto3_iotfleetwise/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15473 2023-08-01 11:20:44.000000 mypy-boto3-iotfleetwise-1.28.16/mypy_boto3_iotfleetwise/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:20:44.000000 mypy-boto3-iotfleetwise-1.28.16/mypy_boto3_iotfleetwise/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    60467 2023-08-01 11:20:48.000000 mypy-boto3-iotfleetwise-1.28.16/mypy_boto3_iotfleetwise/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60361 2023-08-01 11:20:45.000000 mypy-boto3-iotfleetwise-1.28.16/mypy_boto3_iotfleetwise/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:20:43.000000 mypy-boto3-iotfleetwise-1.28.16/mypy_boto3_iotfleetwise/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:02.280861 mypy-boto3-iotfleetwise-1.28.16/mypy_boto3_iotfleetwise.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21573 2023-08-01 11:37:02.000000 mypy-boto3-iotfleetwise-1.28.16/mypy_boto3_iotfleetwise.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-01 11:37:02.000000 mypy-boto3-iotfleetwise-1.28.16/mypy_boto3_iotfleetwise.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:02.000000 mypy-boto3-iotfleetwise-1.28.16/mypy_boto3_iotfleetwise.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:02.000000 mypy-boto3-iotfleetwise-1.28.16/mypy_boto3_iotfleetwise.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:02.000000 mypy-boto3-iotfleetwise-1.28.16/mypy_boto3_iotfleetwise.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-01 11:37:02.000000 mypy-boto3-iotfleetwise-1.28.16/mypy_boto3_iotfleetwise.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:02.292861 mypy-boto3-iotfleetwise-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-08-01 11:20:43.000000 mypy-boto3-iotfleetwise-1.28.16/setup.py
```

### Comparing `mypy-boto3-iotfleetwise-1.28.15.post1/LICENSE` & `mypy-boto3-iotfleetwise-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotfleetwise-1.28.15.post1/PKG-INFO` & `mypy-boto3-iotfleetwise-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotfleetwise
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.IoTFleetWise 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.IoTFleetWise 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 iotfleetwise type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 iotfleetwise type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotfleetwise.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotfleetwise)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotfleetwise)](https://pepy.tech/project/mypy-boto3-iotfleetwise)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTFleetWise 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise)
+[boto3.IoTFleetWise 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise)
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
 [mypy-boto3-iotfleetwise docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/).
 
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
@@ -383,44 +383,45 @@
 )
 
 
 def check_value(value: CampaignStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_iotfleetwise.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_iotfleetwise.type_defs import (
     ActuatorOutputTypeDef,
     ActuatorTypeDef,
     AssociateVehicleFleetRequestRequestTypeDef,
     AttributeOutputTypeDef,
     AttributeTypeDef,
     CreateVehicleErrorTypeDef,
     CreateVehicleResponseItemTypeDef,
     ResponseMetadataTypeDef,
     UpdateVehicleRequestItemTypeDef,
     UpdateVehicleErrorTypeDef,
     UpdateVehicleResponseItemTypeDef,
+    BlobTypeDef,
     BranchTypeDef,
     CampaignSummaryTypeDef,
-    CanDbcDefinitionTypeDef,
     CanInterfaceTypeDef,
     CanSignalTypeDef,
     CloudWatchLogDeliveryOptionsTypeDef,
     ConditionBasedCollectionSchemeTypeDef,
     TimeBasedCollectionSchemeTypeDef,
     SignalInformationTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
     S3ConfigTypeDef,
     TimestreamConfigTypeDef,
     DecoderManifestSummaryTypeDef,
     DeleteCampaignRequestRequestTypeDef,
     DeleteDecoderManifestRequestRequestTypeDef,
     DeleteFleetRequestRequestTypeDef,
     DeleteModelManifestRequestRequestTypeDef,
@@ -493,16 +494,16 @@
     UpdateDecoderManifestResponseTypeDef,
     UpdateFleetResponseTypeDef,
     UpdateModelManifestResponseTypeDef,
     UpdateSignalCatalogResponseTypeDef,
     UpdateVehicleResponseTypeDef,
     BatchUpdateVehicleRequestRequestTypeDef,
     BatchUpdateVehicleResponseTypeDef,
+    CanDbcDefinitionTypeDef,
     ListCampaignsResponseTypeDef,
-    NetworkFileDefinitionTypeDef,
     GetLoggingOptionsResponseTypeDef,
     PutLoggingOptionsRequestRequestTypeDef,
     CollectionSchemeTypeDef,
     CreateFleetRequestRequestTypeDef,
     CreateModelManifestRequestRequestTypeDef,
     CreateVehicleRequestItemTypeDef,
     CreateVehicleRequestRequestTypeDef,
@@ -533,30 +534,32 @@
     ListVehiclesResponseTypeDef,
     NetworkInterfaceTypeDef,
     NodeOutputTypeDef,
     NodeTypeDef,
     SignalDecoderTypeDef,
     RegisterAccountRequestRequestTypeDef,
     RegisterAccountResponseTypeDef,
-    ImportDecoderManifestRequestRequestTypeDef,
+    NetworkFileDefinitionTypeDef,
     BatchCreateVehicleRequestRequestTypeDef,
     CreateCampaignRequestRequestTypeDef,
     GetCampaignResponseTypeDef,
     ListDecoderManifestNetworkInterfacesResponseTypeDef,
     ListModelManifestNodesResponseTypeDef,
     ListSignalCatalogNodesResponseTypeDef,
-    CreateSignalCatalogRequestRequestTypeDef,
-    UpdateSignalCatalogRequestRequestTypeDef,
+    NodeUnionTypeDef,
     CreateDecoderManifestRequestRequestTypeDef,
     ListDecoderManifestSignalsResponseTypeDef,
     UpdateDecoderManifestRequestRequestTypeDef,
+    ImportDecoderManifestRequestRequestTypeDef,
+    CreateSignalCatalogRequestRequestTypeDef,
+    UpdateSignalCatalogRequestRequestTypeDef,
 )
 
 
-def get_structure() -> ActuatorOutputTypeDef:
+def get_value() -> ActuatorOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iotfleetwise-1.28.15.post1/README.md` & `mypy-boto3-iotfleetwise-1.28.16/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotfleetwise.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotfleetwise)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotfleetwise)](https://pepy.tech/project/mypy-boto3-iotfleetwise)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTFleetWise 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise)
+[boto3.IoTFleetWise 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise)
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
 [mypy-boto3-iotfleetwise docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/).
 
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
@@ -351,44 +351,45 @@
 )
 
 
 def check_value(value: CampaignStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_iotfleetwise.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_iotfleetwise.type_defs import (
     ActuatorOutputTypeDef,
     ActuatorTypeDef,
     AssociateVehicleFleetRequestRequestTypeDef,
     AttributeOutputTypeDef,
     AttributeTypeDef,
     CreateVehicleErrorTypeDef,
     CreateVehicleResponseItemTypeDef,
     ResponseMetadataTypeDef,
     UpdateVehicleRequestItemTypeDef,
     UpdateVehicleErrorTypeDef,
     UpdateVehicleResponseItemTypeDef,
+    BlobTypeDef,
     BranchTypeDef,
     CampaignSummaryTypeDef,
-    CanDbcDefinitionTypeDef,
     CanInterfaceTypeDef,
     CanSignalTypeDef,
     CloudWatchLogDeliveryOptionsTypeDef,
     ConditionBasedCollectionSchemeTypeDef,
     TimeBasedCollectionSchemeTypeDef,
     SignalInformationTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
     S3ConfigTypeDef,
     TimestreamConfigTypeDef,
     DecoderManifestSummaryTypeDef,
     DeleteCampaignRequestRequestTypeDef,
     DeleteDecoderManifestRequestRequestTypeDef,
     DeleteFleetRequestRequestTypeDef,
     DeleteModelManifestRequestRequestTypeDef,
@@ -461,16 +462,16 @@
     UpdateDecoderManifestResponseTypeDef,
     UpdateFleetResponseTypeDef,
     UpdateModelManifestResponseTypeDef,
     UpdateSignalCatalogResponseTypeDef,
     UpdateVehicleResponseTypeDef,
     BatchUpdateVehicleRequestRequestTypeDef,
     BatchUpdateVehicleResponseTypeDef,
+    CanDbcDefinitionTypeDef,
     ListCampaignsResponseTypeDef,
-    NetworkFileDefinitionTypeDef,
     GetLoggingOptionsResponseTypeDef,
     PutLoggingOptionsRequestRequestTypeDef,
     CollectionSchemeTypeDef,
     CreateFleetRequestRequestTypeDef,
     CreateModelManifestRequestRequestTypeDef,
     CreateVehicleRequestItemTypeDef,
     CreateVehicleRequestRequestTypeDef,
@@ -501,30 +502,32 @@
     ListVehiclesResponseTypeDef,
     NetworkInterfaceTypeDef,
     NodeOutputTypeDef,
     NodeTypeDef,
     SignalDecoderTypeDef,
     RegisterAccountRequestRequestTypeDef,
     RegisterAccountResponseTypeDef,
-    ImportDecoderManifestRequestRequestTypeDef,
+    NetworkFileDefinitionTypeDef,
     BatchCreateVehicleRequestRequestTypeDef,
     CreateCampaignRequestRequestTypeDef,
     GetCampaignResponseTypeDef,
     ListDecoderManifestNetworkInterfacesResponseTypeDef,
     ListModelManifestNodesResponseTypeDef,
     ListSignalCatalogNodesResponseTypeDef,
-    CreateSignalCatalogRequestRequestTypeDef,
-    UpdateSignalCatalogRequestRequestTypeDef,
+    NodeUnionTypeDef,
     CreateDecoderManifestRequestRequestTypeDef,
     ListDecoderManifestSignalsResponseTypeDef,
     UpdateDecoderManifestRequestRequestTypeDef,
+    ImportDecoderManifestRequestRequestTypeDef,
+    CreateSignalCatalogRequestRequestTypeDef,
+    UpdateSignalCatalogRequestRequestTypeDef,
 )
 
 
-def get_structure() -> ActuatorOutputTypeDef:
+def get_value() -> ActuatorOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iotfleetwise-1.28.15.post1/mypy_boto3_iotfleetwise/__init__.py` & `mypy-boto3-iotfleetwise-1.28.16/mypy_boto3_iotfleetwise/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotfleetwise-1.28.15.post1/mypy_boto3_iotfleetwise/__init__.pyi` & `mypy-boto3-iotfleetwise-1.28.16/mypy_boto3_iotfleetwise/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotfleetwise-1.28.15.post1/mypy_boto3_iotfleetwise/__main__.py` & `mypy-boto3-iotfleetwise-1.28.16/mypy_boto3_iotfleetwise/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IoTFleetWise 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.IoTFleetWise 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise\nOther"
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

### Comparing `mypy-boto3-iotfleetwise-1.28.15.post1/mypy_boto3_iotfleetwise/client.py` & `mypy-boto3-iotfleetwise-1.28.16/mypy_boto3_iotfleetwise/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_iotfleetwise.client import IoTFleetWiseClient
 
     session = Session()
     client: IoTFleetWiseClient = session.client("iotfleetwise")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     CompressionType,
     DiagnosticsModeType,
     ManifestStatusType,
@@ -86,20 +85,20 @@
     ListSignalCatalogNodesResponseTypeDef,
     ListSignalCatalogsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListVehiclesInFleetResponseTypeDef,
     ListVehiclesResponseTypeDef,
     NetworkFileDefinitionTypeDef,
     NetworkInterfaceTypeDef,
-    NodeOutputTypeDef,
-    NodeTypeDef,
+    NodeUnionTypeDef,
     RegisterAccountResponseTypeDef,
     SignalDecoderTypeDef,
     SignalInformationTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
     TimestreamResourcesTypeDef,
     UpdateCampaignResponseTypeDef,
     UpdateDecoderManifestResponseTypeDef,
     UpdateFleetResponseTypeDef,
     UpdateModelManifestResponseTypeDef,
     UpdateSignalCatalogResponseTypeDef,
     UpdateVehicleRequestItemTypeDef,
@@ -202,16 +201,16 @@
         self,
         *,
         name: str,
         signalCatalogArn: str,
         targetArn: str,
         collectionScheme: CollectionSchemeTypeDef,
         description: str = ...,
-        startTime: Union[datetime, str] = ...,
-        expiryTime: Union[datetime, str] = ...,
+        startTime: TimestampTypeDef = ...,
+        expiryTime: TimestampTypeDef = ...,
         postTriggerCollectionDuration: int = ...,
         diagnosticsMode: DiagnosticsModeType = ...,
         spoolingMode: SpoolingModeType = ...,
         compression: CompressionType = ...,
         priority: int = ...,
         signalsToCollect: Sequence[SignalInformationTypeDef] = ...,
         dataExtraDimensions: Sequence[str] = ...,
@@ -275,15 +274,15 @@
         """
 
     def create_signal_catalog(
         self,
         *,
         name: str,
         description: str = ...,
-        nodes: Sequence[Union[NodeTypeDef, NodeOutputTypeDef]] = ...,
+        nodes: Sequence[NodeUnionTypeDef] = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateSignalCatalogResponseTypeDef:
         """
         Creates a collection of standardized signals that can be reused to create
         vehicle models.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Client.create_signal_catalog)
@@ -708,16 +707,16 @@
         """
 
     def update_signal_catalog(
         self,
         *,
         name: str,
         description: str = ...,
-        nodesToAdd: Sequence[Union[NodeTypeDef, NodeOutputTypeDef]] = ...,
-        nodesToUpdate: Sequence[Union[NodeTypeDef, NodeOutputTypeDef]] = ...,
+        nodesToAdd: Sequence[NodeUnionTypeDef] = ...,
+        nodesToUpdate: Sequence[NodeUnionTypeDef] = ...,
         nodesToRemove: Sequence[str] = ...
     ) -> UpdateSignalCatalogResponseTypeDef:
         """
         Updates a signal catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Client.update_signal_catalog)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/client/#update_signal_catalog)
```

### Comparing `mypy-boto3-iotfleetwise-1.28.15.post1/mypy_boto3_iotfleetwise/client.pyi` & `mypy-boto3-iotfleetwise-1.28.16/mypy_boto3_iotfleetwise/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_iotfleetwise.client import IoTFleetWiseClient
 
     session = Session()
     client: IoTFleetWiseClient = session.client("iotfleetwise")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     CompressionType,
     DiagnosticsModeType,
     ManifestStatusType,
@@ -86,20 +85,20 @@
     ListSignalCatalogNodesResponseTypeDef,
     ListSignalCatalogsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListVehiclesInFleetResponseTypeDef,
     ListVehiclesResponseTypeDef,
     NetworkFileDefinitionTypeDef,
     NetworkInterfaceTypeDef,
-    NodeOutputTypeDef,
-    NodeTypeDef,
+    NodeUnionTypeDef,
     RegisterAccountResponseTypeDef,
     SignalDecoderTypeDef,
     SignalInformationTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
     TimestreamResourcesTypeDef,
     UpdateCampaignResponseTypeDef,
     UpdateDecoderManifestResponseTypeDef,
     UpdateFleetResponseTypeDef,
     UpdateModelManifestResponseTypeDef,
     UpdateSignalCatalogResponseTypeDef,
     UpdateVehicleRequestItemTypeDef,
@@ -192,16 +191,16 @@
         self,
         *,
         name: str,
         signalCatalogArn: str,
         targetArn: str,
         collectionScheme: CollectionSchemeTypeDef,
         description: str = ...,
-        startTime: Union[datetime, str] = ...,
-        expiryTime: Union[datetime, str] = ...,
+        startTime: TimestampTypeDef = ...,
+        expiryTime: TimestampTypeDef = ...,
         postTriggerCollectionDuration: int = ...,
         diagnosticsMode: DiagnosticsModeType = ...,
         spoolingMode: SpoolingModeType = ...,
         compression: CompressionType = ...,
         priority: int = ...,
         signalsToCollect: Sequence[SignalInformationTypeDef] = ...,
         dataExtraDimensions: Sequence[str] = ...,
@@ -261,15 +260,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/client/#create_model_manifest)
         """
     def create_signal_catalog(
         self,
         *,
         name: str,
         description: str = ...,
-        nodes: Sequence[Union[NodeTypeDef, NodeOutputTypeDef]] = ...,
+        nodes: Sequence[NodeUnionTypeDef] = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateSignalCatalogResponseTypeDef:
         """
         Creates a collection of standardized signals that can be reused to create
         vehicle models.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Client.create_signal_catalog)
@@ -652,16 +651,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/client/#update_model_manifest)
         """
     def update_signal_catalog(
         self,
         *,
         name: str,
         description: str = ...,
-        nodesToAdd: Sequence[Union[NodeTypeDef, NodeOutputTypeDef]] = ...,
-        nodesToUpdate: Sequence[Union[NodeTypeDef, NodeOutputTypeDef]] = ...,
+        nodesToAdd: Sequence[NodeUnionTypeDef] = ...,
+        nodesToUpdate: Sequence[NodeUnionTypeDef] = ...,
         nodesToRemove: Sequence[str] = ...
     ) -> UpdateSignalCatalogResponseTypeDef:
         """
         Updates a signal catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Client.update_signal_catalog)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/client/#update_signal_catalog)
```

### Comparing `mypy-boto3-iotfleetwise-1.28.15.post1/mypy_boto3_iotfleetwise/literals.py` & `mypy-boto3-iotfleetwise-1.28.16/mypy_boto3_iotfleetwise/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotfleetwise-1.28.15.post1/mypy_boto3_iotfleetwise/literals.pyi` & `mypy-boto3-iotfleetwise-1.28.16/mypy_boto3_iotfleetwise/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotfleetwise-1.28.15.post1/mypy_boto3_iotfleetwise/paginator.py` & `mypy-boto3-iotfleetwise-1.28.16/mypy_boto3_iotfleetwise/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotfleetwise-1.28.15.post1/mypy_boto3_iotfleetwise/paginator.pyi` & `mypy-boto3-iotfleetwise-1.28.16/mypy_boto3_iotfleetwise/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotfleetwise-1.28.15.post1/mypy_boto3_iotfleetwise/type_defs.py` & `mypy-boto3-iotfleetwise-1.28.16/mypy_boto3_iotfleetwise/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_iotfleetwise.type_defs import ActuatorOutputTypeDef
 
-    data: ActuatorOutputTypeDef = {...}
+    data: ActuatorOutputTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -51,24 +51,25 @@
     "AttributeTypeDef",
     "CreateVehicleErrorTypeDef",
     "CreateVehicleResponseItemTypeDef",
     "ResponseMetadataTypeDef",
     "UpdateVehicleRequestItemTypeDef",
     "UpdateVehicleErrorTypeDef",
     "UpdateVehicleResponseItemTypeDef",
+    "BlobTypeDef",
     "BranchTypeDef",
     "CampaignSummaryTypeDef",
-    "CanDbcDefinitionTypeDef",
     "CanInterfaceTypeDef",
     "CanSignalTypeDef",
     "CloudWatchLogDeliveryOptionsTypeDef",
     "ConditionBasedCollectionSchemeTypeDef",
     "TimeBasedCollectionSchemeTypeDef",
     "SignalInformationTypeDef",
     "TagTypeDef",
+    "TimestampTypeDef",
     "S3ConfigTypeDef",
     "TimestreamConfigTypeDef",
     "DecoderManifestSummaryTypeDef",
     "DeleteCampaignRequestRequestTypeDef",
     "DeleteDecoderManifestRequestRequestTypeDef",
     "DeleteFleetRequestRequestTypeDef",
     "DeleteModelManifestRequestRequestTypeDef",
@@ -141,16 +142,16 @@
     "UpdateDecoderManifestResponseTypeDef",
     "UpdateFleetResponseTypeDef",
     "UpdateModelManifestResponseTypeDef",
     "UpdateSignalCatalogResponseTypeDef",
     "UpdateVehicleResponseTypeDef",
     "BatchUpdateVehicleRequestRequestTypeDef",
     "BatchUpdateVehicleResponseTypeDef",
+    "CanDbcDefinitionTypeDef",
     "ListCampaignsResponseTypeDef",
-    "NetworkFileDefinitionTypeDef",
     "GetLoggingOptionsResponseTypeDef",
     "PutLoggingOptionsRequestRequestTypeDef",
     "CollectionSchemeTypeDef",
     "CreateFleetRequestRequestTypeDef",
     "CreateModelManifestRequestRequestTypeDef",
     "CreateVehicleRequestItemTypeDef",
     "CreateVehicleRequestRequestTypeDef",
@@ -181,26 +182,28 @@
     "ListVehiclesResponseTypeDef",
     "NetworkInterfaceTypeDef",
     "NodeOutputTypeDef",
     "NodeTypeDef",
     "SignalDecoderTypeDef",
     "RegisterAccountRequestRequestTypeDef",
     "RegisterAccountResponseTypeDef",
-    "ImportDecoderManifestRequestRequestTypeDef",
+    "NetworkFileDefinitionTypeDef",
     "BatchCreateVehicleRequestRequestTypeDef",
     "CreateCampaignRequestRequestTypeDef",
     "GetCampaignResponseTypeDef",
     "ListDecoderManifestNetworkInterfacesResponseTypeDef",
     "ListModelManifestNodesResponseTypeDef",
     "ListSignalCatalogNodesResponseTypeDef",
-    "CreateSignalCatalogRequestRequestTypeDef",
-    "UpdateSignalCatalogRequestRequestTypeDef",
+    "NodeUnionTypeDef",
     "CreateDecoderManifestRequestRequestTypeDef",
     "ListDecoderManifestSignalsResponseTypeDef",
     "UpdateDecoderManifestRequestRequestTypeDef",
+    "ImportDecoderManifestRequestRequestTypeDef",
+    "CreateSignalCatalogRequestRequestTypeDef",
+    "UpdateSignalCatalogRequestRequestTypeDef",
 )
 
 _RequiredActuatorOutputTypeDef = TypedDict(
     "_RequiredActuatorOutputTypeDef",
     {
         "fullyQualifiedName": str,
         "dataType": NodeDataTypeType,
@@ -387,14 +390,15 @@
     {
         "vehicleName": str,
         "arn": str,
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 _RequiredBranchTypeDef = TypedDict(
     "_RequiredBranchTypeDef",
     {
         "fullyQualifiedName": str,
     },
 )
 _OptionalBranchTypeDef = TypedDict(
@@ -433,34 +437,14 @@
 )
 
 
 class CampaignSummaryTypeDef(_RequiredCampaignSummaryTypeDef, _OptionalCampaignSummaryTypeDef):
     pass
 
 
-_RequiredCanDbcDefinitionTypeDef = TypedDict(
-    "_RequiredCanDbcDefinitionTypeDef",
-    {
-        "networkInterface": str,
-        "canDbcFiles": Sequence[Union[str, bytes, IO[Any], StreamingBody]],
-    },
-)
-_OptionalCanDbcDefinitionTypeDef = TypedDict(
-    "_OptionalCanDbcDefinitionTypeDef",
-    {
-        "signalsMap": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class CanDbcDefinitionTypeDef(_RequiredCanDbcDefinitionTypeDef, _OptionalCanDbcDefinitionTypeDef):
-    pass
-
-
 _RequiredCanInterfaceTypeDef = TypedDict(
     "_RequiredCanInterfaceTypeDef",
     {
         "name": str,
     },
 )
 _OptionalCanInterfaceTypeDef = TypedDict(
@@ -579,14 +563,15 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
+TimestampTypeDef = Union[datetime, str]
 _RequiredS3ConfigTypeDef = TypedDict(
     "_RequiredS3ConfigTypeDef",
     {
         "bucketArn": str,
     },
 )
 _OptionalS3ConfigTypeDef = TypedDict(
@@ -1608,31 +1593,43 @@
     {
         "vehicles": List[UpdateVehicleResponseItemTypeDef],
         "errors": List[UpdateVehicleErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCanDbcDefinitionTypeDef = TypedDict(
+    "_RequiredCanDbcDefinitionTypeDef",
+    {
+        "networkInterface": str,
+        "canDbcFiles": Sequence[BlobTypeDef],
+    },
+)
+_OptionalCanDbcDefinitionTypeDef = TypedDict(
+    "_OptionalCanDbcDefinitionTypeDef",
+    {
+        "signalsMap": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class CanDbcDefinitionTypeDef(_RequiredCanDbcDefinitionTypeDef, _OptionalCanDbcDefinitionTypeDef):
+    pass
+
+
 ListCampaignsResponseTypeDef = TypedDict(
     "ListCampaignsResponseTypeDef",
     {
         "campaignSummaries": List[CampaignSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-NetworkFileDefinitionTypeDef = TypedDict(
-    "NetworkFileDefinitionTypeDef",
-    {
-        "canDbc": CanDbcDefinitionTypeDef,
-    },
-    total=False,
-)
-
 GetLoggingOptionsResponseTypeDef = TypedDict(
     "GetLoggingOptionsResponseTypeDef",
     {
         "cloudWatchLogDelivery": CloudWatchLogDeliveryOptionsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2168,20 +2165,20 @@
         "iamResources": IamResourcesTypeDef,
         "creationTime": datetime,
         "lastModificationTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ImportDecoderManifestRequestRequestTypeDef = TypedDict(
-    "ImportDecoderManifestRequestRequestTypeDef",
+NetworkFileDefinitionTypeDef = TypedDict(
+    "NetworkFileDefinitionTypeDef",
     {
-        "name": str,
-        "networkFileDefinitions": Sequence[NetworkFileDefinitionTypeDef],
+        "canDbc": CanDbcDefinitionTypeDef,
     },
+    total=False,
 )
 
 BatchCreateVehicleRequestRequestTypeDef = TypedDict(
     "BatchCreateVehicleRequestRequestTypeDef",
     {
         "vehicles": Sequence[CreateVehicleRequestItemTypeDef],
     },
@@ -2196,16 +2193,16 @@
         "collectionScheme": CollectionSchemeTypeDef,
     },
 )
 _OptionalCreateCampaignRequestRequestTypeDef = TypedDict(
     "_OptionalCreateCampaignRequestRequestTypeDef",
     {
         "description": str,
-        "startTime": Union[datetime, str],
-        "expiryTime": Union[datetime, str],
+        "startTime": TimestampTypeDef,
+        "expiryTime": TimestampTypeDef,
         "postTriggerCollectionDuration": int,
         "diagnosticsMode": DiagnosticsModeType,
         "spoolingMode": SpoolingModeType,
         "compression": CompressionType,
         "priority": int,
         "signalsToCollect": Sequence[SignalInformationTypeDef],
         "dataExtraDimensions": Sequence[str],
@@ -2271,63 +2268,15 @@
     {
         "nodes": List[NodeOutputTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateSignalCatalogRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateSignalCatalogRequestRequestTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalCreateSignalCatalogRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateSignalCatalogRequestRequestTypeDef",
-    {
-        "description": str,
-        "nodes": Sequence[Union[NodeTypeDef, NodeOutputTypeDef]],
-        "tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-
-class CreateSignalCatalogRequestRequestTypeDef(
-    _RequiredCreateSignalCatalogRequestRequestTypeDef,
-    _OptionalCreateSignalCatalogRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredUpdateSignalCatalogRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateSignalCatalogRequestRequestTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalUpdateSignalCatalogRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateSignalCatalogRequestRequestTypeDef",
-    {
-        "description": str,
-        "nodesToAdd": Sequence[Union[NodeTypeDef, NodeOutputTypeDef]],
-        "nodesToUpdate": Sequence[Union[NodeTypeDef, NodeOutputTypeDef]],
-        "nodesToRemove": Sequence[str],
-    },
-    total=False,
-)
-
-
-class UpdateSignalCatalogRequestRequestTypeDef(
-    _RequiredUpdateSignalCatalogRequestRequestTypeDef,
-    _OptionalUpdateSignalCatalogRequestRequestTypeDef,
-):
-    pass
-
-
+NodeUnionTypeDef = Union[NodeTypeDef, NodeOutputTypeDef]
 _RequiredCreateDecoderManifestRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDecoderManifestRequestRequestTypeDef",
     {
         "name": str,
         "modelManifestArn": str,
     },
 )
@@ -2382,7 +2331,64 @@
 
 
 class UpdateDecoderManifestRequestRequestTypeDef(
     _RequiredUpdateDecoderManifestRequestRequestTypeDef,
     _OptionalUpdateDecoderManifestRequestRequestTypeDef,
 ):
     pass
+
+
+ImportDecoderManifestRequestRequestTypeDef = TypedDict(
+    "ImportDecoderManifestRequestRequestTypeDef",
+    {
+        "name": str,
+        "networkFileDefinitions": Sequence[NetworkFileDefinitionTypeDef],
+    },
+)
+
+_RequiredCreateSignalCatalogRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateSignalCatalogRequestRequestTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalCreateSignalCatalogRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateSignalCatalogRequestRequestTypeDef",
+    {
+        "description": str,
+        "nodes": Sequence[NodeUnionTypeDef],
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateSignalCatalogRequestRequestTypeDef(
+    _RequiredCreateSignalCatalogRequestRequestTypeDef,
+    _OptionalCreateSignalCatalogRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredUpdateSignalCatalogRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateSignalCatalogRequestRequestTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalUpdateSignalCatalogRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateSignalCatalogRequestRequestTypeDef",
+    {
+        "description": str,
+        "nodesToAdd": Sequence[NodeUnionTypeDef],
+        "nodesToUpdate": Sequence[NodeUnionTypeDef],
+        "nodesToRemove": Sequence[str],
+    },
+    total=False,
+)
+
+
+class UpdateSignalCatalogRequestRequestTypeDef(
+    _RequiredUpdateSignalCatalogRequestRequestTypeDef,
+    _OptionalUpdateSignalCatalogRequestRequestTypeDef,
+):
+    pass
```

### Comparing `mypy-boto3-iotfleetwise-1.28.15.post1/mypy_boto3_iotfleetwise/type_defs.pyi` & `mypy-boto3-iotfleetwise-1.28.16/mypy_boto3_iotfleetwise/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_iotfleetwise.type_defs import ActuatorOutputTypeDef
 
-    data: ActuatorOutputTypeDef = {...}
+    data: ActuatorOutputTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -50,24 +50,25 @@
     "AttributeTypeDef",
     "CreateVehicleErrorTypeDef",
     "CreateVehicleResponseItemTypeDef",
     "ResponseMetadataTypeDef",
     "UpdateVehicleRequestItemTypeDef",
     "UpdateVehicleErrorTypeDef",
     "UpdateVehicleResponseItemTypeDef",
+    "BlobTypeDef",
     "BranchTypeDef",
     "CampaignSummaryTypeDef",
-    "CanDbcDefinitionTypeDef",
     "CanInterfaceTypeDef",
     "CanSignalTypeDef",
     "CloudWatchLogDeliveryOptionsTypeDef",
     "ConditionBasedCollectionSchemeTypeDef",
     "TimeBasedCollectionSchemeTypeDef",
     "SignalInformationTypeDef",
     "TagTypeDef",
+    "TimestampTypeDef",
     "S3ConfigTypeDef",
     "TimestreamConfigTypeDef",
     "DecoderManifestSummaryTypeDef",
     "DeleteCampaignRequestRequestTypeDef",
     "DeleteDecoderManifestRequestRequestTypeDef",
     "DeleteFleetRequestRequestTypeDef",
     "DeleteModelManifestRequestRequestTypeDef",
@@ -140,16 +141,16 @@
     "UpdateDecoderManifestResponseTypeDef",
     "UpdateFleetResponseTypeDef",
     "UpdateModelManifestResponseTypeDef",
     "UpdateSignalCatalogResponseTypeDef",
     "UpdateVehicleResponseTypeDef",
     "BatchUpdateVehicleRequestRequestTypeDef",
     "BatchUpdateVehicleResponseTypeDef",
+    "CanDbcDefinitionTypeDef",
     "ListCampaignsResponseTypeDef",
-    "NetworkFileDefinitionTypeDef",
     "GetLoggingOptionsResponseTypeDef",
     "PutLoggingOptionsRequestRequestTypeDef",
     "CollectionSchemeTypeDef",
     "CreateFleetRequestRequestTypeDef",
     "CreateModelManifestRequestRequestTypeDef",
     "CreateVehicleRequestItemTypeDef",
     "CreateVehicleRequestRequestTypeDef",
@@ -180,26 +181,28 @@
     "ListVehiclesResponseTypeDef",
     "NetworkInterfaceTypeDef",
     "NodeOutputTypeDef",
     "NodeTypeDef",
     "SignalDecoderTypeDef",
     "RegisterAccountRequestRequestTypeDef",
     "RegisterAccountResponseTypeDef",
-    "ImportDecoderManifestRequestRequestTypeDef",
+    "NetworkFileDefinitionTypeDef",
     "BatchCreateVehicleRequestRequestTypeDef",
     "CreateCampaignRequestRequestTypeDef",
     "GetCampaignResponseTypeDef",
     "ListDecoderManifestNetworkInterfacesResponseTypeDef",
     "ListModelManifestNodesResponseTypeDef",
     "ListSignalCatalogNodesResponseTypeDef",
-    "CreateSignalCatalogRequestRequestTypeDef",
-    "UpdateSignalCatalogRequestRequestTypeDef",
+    "NodeUnionTypeDef",
     "CreateDecoderManifestRequestRequestTypeDef",
     "ListDecoderManifestSignalsResponseTypeDef",
     "UpdateDecoderManifestRequestRequestTypeDef",
+    "ImportDecoderManifestRequestRequestTypeDef",
+    "CreateSignalCatalogRequestRequestTypeDef",
+    "UpdateSignalCatalogRequestRequestTypeDef",
 )
 
 _RequiredActuatorOutputTypeDef = TypedDict(
     "_RequiredActuatorOutputTypeDef",
     {
         "fullyQualifiedName": str,
         "dataType": NodeDataTypeType,
@@ -376,14 +379,15 @@
     {
         "vehicleName": str,
         "arn": str,
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 _RequiredBranchTypeDef = TypedDict(
     "_RequiredBranchTypeDef",
     {
         "fullyQualifiedName": str,
     },
 )
 _OptionalBranchTypeDef = TypedDict(
@@ -418,32 +422,14 @@
     },
     total=False,
 )
 
 class CampaignSummaryTypeDef(_RequiredCampaignSummaryTypeDef, _OptionalCampaignSummaryTypeDef):
     pass
 
-_RequiredCanDbcDefinitionTypeDef = TypedDict(
-    "_RequiredCanDbcDefinitionTypeDef",
-    {
-        "networkInterface": str,
-        "canDbcFiles": Sequence[Union[str, bytes, IO[Any], StreamingBody]],
-    },
-)
-_OptionalCanDbcDefinitionTypeDef = TypedDict(
-    "_OptionalCanDbcDefinitionTypeDef",
-    {
-        "signalsMap": Mapping[str, str],
-    },
-    total=False,
-)
-
-class CanDbcDefinitionTypeDef(_RequiredCanDbcDefinitionTypeDef, _OptionalCanDbcDefinitionTypeDef):
-    pass
-
 _RequiredCanInterfaceTypeDef = TypedDict(
     "_RequiredCanInterfaceTypeDef",
     {
         "name": str,
     },
 )
 _OptionalCanInterfaceTypeDef = TypedDict(
@@ -552,14 +538,15 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
+TimestampTypeDef = Union[datetime, str]
 _RequiredS3ConfigTypeDef = TypedDict(
     "_RequiredS3ConfigTypeDef",
     {
         "bucketArn": str,
     },
 )
 _OptionalS3ConfigTypeDef = TypedDict(
@@ -1539,31 +1526,41 @@
     {
         "vehicles": List[UpdateVehicleResponseItemTypeDef],
         "errors": List[UpdateVehicleErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCanDbcDefinitionTypeDef = TypedDict(
+    "_RequiredCanDbcDefinitionTypeDef",
+    {
+        "networkInterface": str,
+        "canDbcFiles": Sequence[BlobTypeDef],
+    },
+)
+_OptionalCanDbcDefinitionTypeDef = TypedDict(
+    "_OptionalCanDbcDefinitionTypeDef",
+    {
+        "signalsMap": Mapping[str, str],
+    },
+    total=False,
+)
+
+class CanDbcDefinitionTypeDef(_RequiredCanDbcDefinitionTypeDef, _OptionalCanDbcDefinitionTypeDef):
+    pass
+
 ListCampaignsResponseTypeDef = TypedDict(
     "ListCampaignsResponseTypeDef",
     {
         "campaignSummaries": List[CampaignSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-NetworkFileDefinitionTypeDef = TypedDict(
-    "NetworkFileDefinitionTypeDef",
-    {
-        "canDbc": CanDbcDefinitionTypeDef,
-    },
-    total=False,
-)
-
 GetLoggingOptionsResponseTypeDef = TypedDict(
     "GetLoggingOptionsResponseTypeDef",
     {
         "cloudWatchLogDelivery": CloudWatchLogDeliveryOptionsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2071,20 +2068,20 @@
         "iamResources": IamResourcesTypeDef,
         "creationTime": datetime,
         "lastModificationTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ImportDecoderManifestRequestRequestTypeDef = TypedDict(
-    "ImportDecoderManifestRequestRequestTypeDef",
+NetworkFileDefinitionTypeDef = TypedDict(
+    "NetworkFileDefinitionTypeDef",
     {
-        "name": str,
-        "networkFileDefinitions": Sequence[NetworkFileDefinitionTypeDef],
+        "canDbc": CanDbcDefinitionTypeDef,
     },
+    total=False,
 )
 
 BatchCreateVehicleRequestRequestTypeDef = TypedDict(
     "BatchCreateVehicleRequestRequestTypeDef",
     {
         "vehicles": Sequence[CreateVehicleRequestItemTypeDef],
     },
@@ -2099,16 +2096,16 @@
         "collectionScheme": CollectionSchemeTypeDef,
     },
 )
 _OptionalCreateCampaignRequestRequestTypeDef = TypedDict(
     "_OptionalCreateCampaignRequestRequestTypeDef",
     {
         "description": str,
-        "startTime": Union[datetime, str],
-        "expiryTime": Union[datetime, str],
+        "startTime": TimestampTypeDef,
+        "expiryTime": TimestampTypeDef,
         "postTriggerCollectionDuration": int,
         "diagnosticsMode": DiagnosticsModeType,
         "spoolingMode": SpoolingModeType,
         "compression": CompressionType,
         "priority": int,
         "signalsToCollect": Sequence[SignalInformationTypeDef],
         "dataExtraDimensions": Sequence[str],
@@ -2172,59 +2169,15 @@
     {
         "nodes": List[NodeOutputTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateSignalCatalogRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateSignalCatalogRequestRequestTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalCreateSignalCatalogRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateSignalCatalogRequestRequestTypeDef",
-    {
-        "description": str,
-        "nodes": Sequence[Union[NodeTypeDef, NodeOutputTypeDef]],
-        "tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-class CreateSignalCatalogRequestRequestTypeDef(
-    _RequiredCreateSignalCatalogRequestRequestTypeDef,
-    _OptionalCreateSignalCatalogRequestRequestTypeDef,
-):
-    pass
-
-_RequiredUpdateSignalCatalogRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateSignalCatalogRequestRequestTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalUpdateSignalCatalogRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateSignalCatalogRequestRequestTypeDef",
-    {
-        "description": str,
-        "nodesToAdd": Sequence[Union[NodeTypeDef, NodeOutputTypeDef]],
-        "nodesToUpdate": Sequence[Union[NodeTypeDef, NodeOutputTypeDef]],
-        "nodesToRemove": Sequence[str],
-    },
-    total=False,
-)
-
-class UpdateSignalCatalogRequestRequestTypeDef(
-    _RequiredUpdateSignalCatalogRequestRequestTypeDef,
-    _OptionalUpdateSignalCatalogRequestRequestTypeDef,
-):
-    pass
-
+NodeUnionTypeDef = Union[NodeTypeDef, NodeOutputTypeDef]
 _RequiredCreateDecoderManifestRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDecoderManifestRequestRequestTypeDef",
     {
         "name": str,
         "modelManifestArn": str,
     },
 )
@@ -2276,7 +2229,60 @@
 )
 
 class UpdateDecoderManifestRequestRequestTypeDef(
     _RequiredUpdateDecoderManifestRequestRequestTypeDef,
     _OptionalUpdateDecoderManifestRequestRequestTypeDef,
 ):
     pass
+
+ImportDecoderManifestRequestRequestTypeDef = TypedDict(
+    "ImportDecoderManifestRequestRequestTypeDef",
+    {
+        "name": str,
+        "networkFileDefinitions": Sequence[NetworkFileDefinitionTypeDef],
+    },
+)
+
+_RequiredCreateSignalCatalogRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateSignalCatalogRequestRequestTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalCreateSignalCatalogRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateSignalCatalogRequestRequestTypeDef",
+    {
+        "description": str,
+        "nodes": Sequence[NodeUnionTypeDef],
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class CreateSignalCatalogRequestRequestTypeDef(
+    _RequiredCreateSignalCatalogRequestRequestTypeDef,
+    _OptionalCreateSignalCatalogRequestRequestTypeDef,
+):
+    pass
+
+_RequiredUpdateSignalCatalogRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateSignalCatalogRequestRequestTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalUpdateSignalCatalogRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateSignalCatalogRequestRequestTypeDef",
+    {
+        "description": str,
+        "nodesToAdd": Sequence[NodeUnionTypeDef],
+        "nodesToUpdate": Sequence[NodeUnionTypeDef],
+        "nodesToRemove": Sequence[str],
+    },
+    total=False,
+)
+
+class UpdateSignalCatalogRequestRequestTypeDef(
+    _RequiredUpdateSignalCatalogRequestRequestTypeDef,
+    _OptionalUpdateSignalCatalogRequestRequestTypeDef,
+):
+    pass
```

### Comparing `mypy-boto3-iotfleetwise-1.28.15.post1/mypy_boto3_iotfleetwise.egg-info/PKG-INFO` & `mypy-boto3-iotfleetwise-1.28.16/mypy_boto3_iotfleetwise.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotfleetwise
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.IoTFleetWise 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.IoTFleetWise 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 iotfleetwise type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 iotfleetwise type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotfleetwise.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotfleetwise)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotfleetwise)](https://pepy.tech/project/mypy-boto3-iotfleetwise)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTFleetWise 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise)
+[boto3.IoTFleetWise 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise)
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
 [mypy-boto3-iotfleetwise docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/).
 
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
@@ -383,44 +383,45 @@
 )
 
 
 def check_value(value: CampaignStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_iotfleetwise.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_iotfleetwise.type_defs import (
     ActuatorOutputTypeDef,
     ActuatorTypeDef,
     AssociateVehicleFleetRequestRequestTypeDef,
     AttributeOutputTypeDef,
     AttributeTypeDef,
     CreateVehicleErrorTypeDef,
     CreateVehicleResponseItemTypeDef,
     ResponseMetadataTypeDef,
     UpdateVehicleRequestItemTypeDef,
     UpdateVehicleErrorTypeDef,
     UpdateVehicleResponseItemTypeDef,
+    BlobTypeDef,
     BranchTypeDef,
     CampaignSummaryTypeDef,
-    CanDbcDefinitionTypeDef,
     CanInterfaceTypeDef,
     CanSignalTypeDef,
     CloudWatchLogDeliveryOptionsTypeDef,
     ConditionBasedCollectionSchemeTypeDef,
     TimeBasedCollectionSchemeTypeDef,
     SignalInformationTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
     S3ConfigTypeDef,
     TimestreamConfigTypeDef,
     DecoderManifestSummaryTypeDef,
     DeleteCampaignRequestRequestTypeDef,
     DeleteDecoderManifestRequestRequestTypeDef,
     DeleteFleetRequestRequestTypeDef,
     DeleteModelManifestRequestRequestTypeDef,
@@ -493,16 +494,16 @@
     UpdateDecoderManifestResponseTypeDef,
     UpdateFleetResponseTypeDef,
     UpdateModelManifestResponseTypeDef,
     UpdateSignalCatalogResponseTypeDef,
     UpdateVehicleResponseTypeDef,
     BatchUpdateVehicleRequestRequestTypeDef,
     BatchUpdateVehicleResponseTypeDef,
+    CanDbcDefinitionTypeDef,
     ListCampaignsResponseTypeDef,
-    NetworkFileDefinitionTypeDef,
     GetLoggingOptionsResponseTypeDef,
     PutLoggingOptionsRequestRequestTypeDef,
     CollectionSchemeTypeDef,
     CreateFleetRequestRequestTypeDef,
     CreateModelManifestRequestRequestTypeDef,
     CreateVehicleRequestItemTypeDef,
     CreateVehicleRequestRequestTypeDef,
@@ -533,30 +534,32 @@
     ListVehiclesResponseTypeDef,
     NetworkInterfaceTypeDef,
     NodeOutputTypeDef,
     NodeTypeDef,
     SignalDecoderTypeDef,
     RegisterAccountRequestRequestTypeDef,
     RegisterAccountResponseTypeDef,
-    ImportDecoderManifestRequestRequestTypeDef,
+    NetworkFileDefinitionTypeDef,
     BatchCreateVehicleRequestRequestTypeDef,
     CreateCampaignRequestRequestTypeDef,
     GetCampaignResponseTypeDef,
     ListDecoderManifestNetworkInterfacesResponseTypeDef,
     ListModelManifestNodesResponseTypeDef,
     ListSignalCatalogNodesResponseTypeDef,
-    CreateSignalCatalogRequestRequestTypeDef,
-    UpdateSignalCatalogRequestRequestTypeDef,
+    NodeUnionTypeDef,
     CreateDecoderManifestRequestRequestTypeDef,
     ListDecoderManifestSignalsResponseTypeDef,
     UpdateDecoderManifestRequestRequestTypeDef,
+    ImportDecoderManifestRequestRequestTypeDef,
+    CreateSignalCatalogRequestRequestTypeDef,
+    UpdateSignalCatalogRequestRequestTypeDef,
 )
 
 
-def get_structure() -> ActuatorOutputTypeDef:
+def get_value() -> ActuatorOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iotfleetwise-1.28.15.post1/mypy_boto3_iotfleetwise.egg-info/SOURCES.txt` & `mypy-boto3-iotfleetwise-1.28.16/mypy_boto3_iotfleetwise.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotfleetwise-1.28.15.post1/setup.py` & `mypy-boto3-iotfleetwise-1.28.16/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-iotfleetwise",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_iotfleetwise"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IoTFleetWise 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.IoTFleetWise 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 iotfleetwise type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 iotfleetwise type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_iotfleetwise": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

