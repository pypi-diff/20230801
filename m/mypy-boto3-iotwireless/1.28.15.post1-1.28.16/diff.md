# Comparing `tmp/mypy-boto3-iotwireless-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-iotwireless-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iotwireless-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:23 2023, max compression
+gzip compressed data, was "mypy-boto3-iotwireless-1.28.16.tar", last modified: Tue Aug  1 11:37:03 2023, max compression
```

## Comparing `mypy-boto3-iotwireless-1.28.15.post1.tar` & `mypy-boto3-iotwireless-1.28.16.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:23.557198 mypy-boto3-iotwireless-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:48:18.000000 mypy-boto3-iotwireless-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    25742 2023-07-29 10:03:23.557198 mypy-boto3-iotwireless-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24233 2023-07-29 09:48:18.000000 mypy-boto3-iotwireless-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:23.549198 mypy-boto3-iotwireless-1.28.15.post1/mypy_boto3_iotwireless/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-29 09:48:18.000000 mypy-boto3-iotwireless-1.28.15.post1/mypy_boto3_iotwireless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-29 09:48:18.000000 mypy-boto3-iotwireless-1.28.15.post1/mypy_boto3_iotwireless/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-29 09:48:18.000000 mypy-boto3-iotwireless-1.28.15.post1/mypy_boto3_iotwireless/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    72698 2023-07-29 09:48:19.000000 mypy-boto3-iotwireless-1.28.15.post1/mypy_boto3_iotwireless/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    72582 2023-07-29 09:48:18.000000 mypy-boto3-iotwireless-1.28.15.post1/mypy_boto3_iotwireless/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12314 2023-07-29 09:48:19.000000 mypy-boto3-iotwireless-1.28.15.post1/mypy_boto3_iotwireless/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12312 2023-07-29 09:48:19.000000 mypy-boto3-iotwireless-1.28.15.post1/mypy_boto3_iotwireless/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:48:18.000000 mypy-boto3-iotwireless-1.28.15.post1/mypy_boto3_iotwireless/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   101300 2023-07-29 09:48:24.000000 mypy-boto3-iotwireless-1.28.15.post1/mypy_boto3_iotwireless/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   101207 2023-07-29 09:48:22.000000 mypy-boto3-iotwireless-1.28.15.post1/mypy_boto3_iotwireless/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:48:18.000000 mypy-boto3-iotwireless-1.28.15.post1/mypy_boto3_iotwireless/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:23.557198 mypy-boto3-iotwireless-1.28.15.post1/mypy_boto3_iotwireless.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25742 2023-07-29 10:03:23.000000 mypy-boto3-iotwireless-1.28.15.post1/mypy_boto3_iotwireless.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-29 10:03:23.000000 mypy-boto3-iotwireless-1.28.15.post1/mypy_boto3_iotwireless.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:23.000000 mypy-boto3-iotwireless-1.28.15.post1/mypy_boto3_iotwireless.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:23.000000 mypy-boto3-iotwireless-1.28.15.post1/mypy_boto3_iotwireless.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:23.000000 mypy-boto3-iotwireless-1.28.15.post1/mypy_boto3_iotwireless.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-29 10:03:23.000000 mypy-boto3-iotwireless-1.28.15.post1/mypy_boto3_iotwireless.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:23.557198 mypy-boto3-iotwireless-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-29 09:48:18.000000 mypy-boto3-iotwireless-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:03.436858 mypy-boto3-iotwireless-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:21:03.000000 mypy-boto3-iotwireless-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    25996 2023-08-01 11:37:03.436858 mypy-boto3-iotwireless-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24496 2023-08-01 11:21:03.000000 mypy-boto3-iotwireless-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:03.424858 mypy-boto3-iotwireless-1.28.16/mypy_boto3_iotwireless/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-08-01 11:21:03.000000 mypy-boto3-iotwireless-1.28.16/mypy_boto3_iotwireless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-08-01 11:21:03.000000 mypy-boto3-iotwireless-1.28.16/mypy_boto3_iotwireless/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-08-01 11:21:03.000000 mypy-boto3-iotwireless-1.28.16/mypy_boto3_iotwireless/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72130 2023-08-01 11:21:05.000000 mypy-boto3-iotwireless-1.28.16/mypy_boto3_iotwireless/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72014 2023-08-01 11:21:03.000000 mypy-boto3-iotwireless-1.28.16/mypy_boto3_iotwireless/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12314 2023-08-01 11:21:06.000000 mypy-boto3-iotwireless-1.28.16/mypy_boto3_iotwireless/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12312 2023-08-01 11:21:06.000000 mypy-boto3-iotwireless-1.28.16/mypy_boto3_iotwireless/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:21:03.000000 mypy-boto3-iotwireless-1.28.16/mypy_boto3_iotwireless/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   102152 2023-08-01 11:21:09.000000 mypy-boto3-iotwireless-1.28.16/mypy_boto3_iotwireless/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   102059 2023-08-01 11:21:07.000000 mypy-boto3-iotwireless-1.28.16/mypy_boto3_iotwireless/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:21:03.000000 mypy-boto3-iotwireless-1.28.16/mypy_boto3_iotwireless/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:03.436858 mypy-boto3-iotwireless-1.28.16/mypy_boto3_iotwireless.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25996 2023-08-01 11:37:03.000000 mypy-boto3-iotwireless-1.28.16/mypy_boto3_iotwireless.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-08-01 11:37:03.000000 mypy-boto3-iotwireless-1.28.16/mypy_boto3_iotwireless.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:03.000000 mypy-boto3-iotwireless-1.28.16/mypy_boto3_iotwireless.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:03.000000 mypy-boto3-iotwireless-1.28.16/mypy_boto3_iotwireless.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:03.000000 mypy-boto3-iotwireless-1.28.16/mypy_boto3_iotwireless.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-01 11:37:03.000000 mypy-boto3-iotwireless-1.28.16/mypy_boto3_iotwireless.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:03.436858 mypy-boto3-iotwireless-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-08-01 11:21:03.000000 mypy-boto3-iotwireless-1.28.16/setup.py
```

### Comparing `mypy-boto3-iotwireless-1.28.15.post1/LICENSE` & `mypy-boto3-iotwireless-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotwireless-1.28.15.post1/PKG-INFO` & `mypy-boto3-iotwireless-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotwireless
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.IoTWireless 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.IoTWireless 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 iotwireless type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 iotwireless type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotwireless.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotwireless)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotwireless)](https://pepy.tech/project/mypy-boto3-iotwireless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTWireless 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless)
+[boto3.IoTWireless 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless)
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
 [mypy-boto3-iotwireless docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/).
 
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
@@ -326,20 +326,20 @@
 )
 
 
 def check_value(value: ApplicationConfigTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_iotwireless.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_iotwireless.type_defs import (
     SessionKeysAbpV10XTypeDef,
     SessionKeysAbpV11TypeDef,
     AccuracyTypeDef,
     ApplicationConfigTypeDef,
@@ -350,14 +350,15 @@
     AssociateWirelessDeviceWithFuotaTaskRequestRequestTypeDef,
     AssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef,
     AssociateWirelessDeviceWithThingRequestRequestTypeDef,
     AssociateWirelessGatewayWithCertificateRequestRequestTypeDef,
     AssociateWirelessGatewayWithThingRequestRequestTypeDef,
     BeaconingOutputTypeDef,
     BeaconingTypeDef,
+    BlobTypeDef,
     CancelMulticastGroupSessionRequestRequestTypeDef,
     CdmaLocalIdTypeDef,
     CdmaNmrObjTypeDef,
     CertificateListTypeDef,
     LoRaWANConnectionStatusEventNotificationConfigurationsTypeDef,
     LoRaWANConnectionStatusResourceTypeEventConfigurationTypeDef,
     LoRaWANDeviceProfileTypeDef,
@@ -406,14 +407,15 @@
     LoRaWANMulticastSessionOutputTypeDef,
     GetNetworkAnalyzerConfigurationRequestRequestTypeDef,
     GetPartnerAccountRequestRequestTypeDef,
     SidewalkAccountInfoWithFingerprintTypeDef,
     GetPositionConfigurationRequestRequestTypeDef,
     GnssTypeDef,
     IpTypeDef,
+    TimestampTypeDef,
     WiFiAccessPointTypeDef,
     GetPositionRequestRequestTypeDef,
     GetResourceEventConfigurationRequestRequestTypeDef,
     GetResourceLogLevelRequestRequestTypeDef,
     GetResourcePositionRequestRequestTypeDef,
     GetServiceEndpointRequestRequestTypeDef,
     GetServiceProfileRequestRequestTypeDef,
@@ -457,16 +459,14 @@
     ListWirelessGatewaysRequestRequestTypeDef,
     LoRaWANGatewayMetadataTypeDef,
     OtaaV10XTypeDef,
     OtaaV11TypeDef,
     LoRaWANGatewayVersionTypeDef,
     LoRaWANListDeviceTypeDef,
     LoRaWANMulticastMetadataTypeDef,
-    LoRaWANMulticastSessionTypeDef,
-    LoRaWANStartFuotaTaskTypeDef,
     UpdateAbpV10XTypeDef,
     UpdateAbpV11TypeDef,
     LteLocalIdTypeDef,
     LteNmrObjTypeDef,
     SemtechGnssConfigurationTypeDef,
     SemtechGnssDetailTypeDef,
     PutResourceLogLevelRequestRequestTypeDef,
@@ -478,15 +478,14 @@
     SidewalkUpdateImportInfoTypeDef,
     TdscdmaLocalIdTypeDef,
     TdscdmaNmrObjTypeDef,
     TestWirelessDeviceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDestinationRequestRequestTypeDef,
     UpdatePositionRequestRequestTypeDef,
-    UpdateResourcePositionRequestRequestTypeDef,
     UpdateWirelessGatewayRequestRequestTypeDef,
     WcdmaLocalIdTypeDef,
     WcdmaNmrObjTypeDef,
     WirelessDeviceEventLogOptionTypeDef,
     WirelessGatewayEventLogOptionTypeDef,
     AbpV10XTypeDef,
     AbpV11TypeDef,
@@ -520,14 +519,15 @@
     SendDataToMulticastGroupResponseTypeDef,
     SendDataToWirelessDeviceResponseTypeDef,
     StartSingleWirelessDeviceImportTaskResponseTypeDef,
     StartWirelessDeviceImportTaskResponseTypeDef,
     TestWirelessDeviceResponseTypeDef,
     LoRaWANGatewayOutputTypeDef,
     LoRaWANGatewayTypeDef,
+    UpdateResourcePositionRequestRequestTypeDef,
     CdmaObjTypeDef,
     SidewalkDeviceTypeDef,
     SidewalkListDeviceTypeDef,
     ConnectionStatusEventConfigurationTypeDef,
     ConnectionStatusResourceTypeEventConfigurationTypeDef,
     CreateDeviceProfileRequestRequestTypeDef,
     CreateFuotaTaskRequestRequestTypeDef,
@@ -549,19 +549,22 @@
     ProximityResourceTypeEventConfigurationTypeDef,
     FPortsOutputTypeDef,
     FPortsTypeDef,
     UpdateFPortsTypeDef,
     ListFuotaTasksResponseTypeDef,
     ParticipatingGatewaysOutputTypeDef,
     ParticipatingGatewaysTypeDef,
+    LoRaWANDeviceProfileUnionTypeDef,
     GetFuotaTaskResponseTypeDef,
     GetMulticastGroupResponseTypeDef,
     GetMulticastGroupSessionResponseTypeDef,
     GetPartnerAccountResponseTypeDef,
     ListPartnerAccountsResponseTypeDef,
+    LoRaWANMulticastSessionTypeDef,
+    LoRaWANStartFuotaTaskTypeDef,
     GetServiceProfileResponseTypeDef,
     GetWirelessDeviceImportTaskResponseTypeDef,
     WirelessDeviceImportTaskTypeDef,
     GsmNmrObjTypeDef,
     ImportedWirelessDeviceTypeDef,
     JoinEventConfigurationTypeDef,
     JoinResourceTypeEventConfigurationTypeDef,
@@ -570,16 +573,14 @@
     ListNetworkAnalyzerConfigurationsResponseTypeDef,
     ListServiceProfilesResponseTypeDef,
     LoRaWANDeviceMetadataTypeDef,
     LoRaWANGatewayCurrentVersionTypeDef,
     LoRaWANUpdateGatewayTaskCreateTypeDef,
     LoRaWANUpdateGatewayTaskEntryTypeDef,
     MulticastWirelessMetadataTypeDef,
-    StartMulticastGroupSessionRequestRequestTypeDef,
-    StartFuotaTaskRequestRequestTypeDef,
     LteObjTypeDef,
     PositionSolverConfigurationsTypeDef,
     PositionSolverDetailsTypeDef,
     StartSingleWirelessDeviceImportTaskRequestRequestTypeDef,
     StartWirelessDeviceImportTaskRequestRequestTypeDef,
     UpdatePartnerAccountRequestRequestTypeDef,
     UpdateWirelessDeviceImportTaskRequestRequestTypeDef,
@@ -588,21 +589,25 @@
     WirelessDeviceLogOptionOutputTypeDef,
     WirelessDeviceLogOptionTypeDef,
     WirelessGatewayLogOptionOutputTypeDef,
     WirelessGatewayLogOptionTypeDef,
     GetWirelessGatewayResponseTypeDef,
     WirelessGatewayStatisticsTypeDef,
     CreateWirelessGatewayRequestRequestTypeDef,
+    LoRaWANGatewayUnionTypeDef,
     WirelessDeviceStatisticsTypeDef,
     GetDeviceProfileResponseTypeDef,
     LoRaWANDeviceOutputTypeDef,
     LoRaWANDeviceTypeDef,
     LoRaWANUpdateDeviceTypeDef,
     LoRaWANSendDataToDeviceOutputTypeDef,
     LoRaWANSendDataToDeviceTypeDef,
+    LoRaWANMulticastSessionUnionTypeDef,
+    StartMulticastGroupSessionRequestRequestTypeDef,
+    StartFuotaTaskRequestRequestTypeDef,
     ListWirelessDeviceImportTasksResponseTypeDef,
     GsmObjTypeDef,
     ListDevicesForWirelessDeviceImportTaskResponseTypeDef,
     EventNotificationItemConfigurationsTypeDef,
     GetResourceEventConfigurationResponseTypeDef,
     UpdateResourceEventConfigurationRequestRequestTypeDef,
     GetEventConfigurationByResourceTypesResponseTypeDef,
@@ -611,37 +616,40 @@
     GetWirelessGatewayFirmwareInformationResponseTypeDef,
     UpdateWirelessGatewayTaskCreateTypeDef,
     UpdateWirelessGatewayTaskEntryTypeDef,
     SendDataToMulticastGroupRequestRequestTypeDef,
     PutPositionConfigurationRequestRequestTypeDef,
     GetPositionConfigurationResponseTypeDef,
     PositionConfigurationItemTypeDef,
+    WirelessDeviceLogOptionUnionTypeDef,
     GetLogLevelsByResourceTypesResponseTypeDef,
-    UpdateLogLevelsByResourceTypesRequestRequestTypeDef,
+    WirelessGatewayLogOptionUnionTypeDef,
     ListWirelessGatewaysResponseTypeDef,
     ListWirelessDevicesResponseTypeDef,
     GetWirelessDeviceResponseTypeDef,
     CreateWirelessDeviceRequestRequestTypeDef,
+    LoRaWANDeviceUnionTypeDef,
     UpdateWirelessDeviceRequestRequestTypeDef,
     DownlinkQueueMessageTypeDef,
     WirelessMetadataTypeDef,
     CellTowersTypeDef,
     EventConfigurationItemTypeDef,
     CreateWirelessGatewayTaskDefinitionRequestRequestTypeDef,
     GetWirelessGatewayTaskDefinitionResponseTypeDef,
     ListWirelessGatewayTaskDefinitionsResponseTypeDef,
     ListPositionConfigurationsResponseTypeDef,
+    UpdateLogLevelsByResourceTypesRequestRequestTypeDef,
     ListQueuedMessagesResponseTypeDef,
     SendDataToWirelessDeviceRequestRequestTypeDef,
     GetPositionEstimateRequestRequestTypeDef,
     ListEventConfigurationsResponseTypeDef,
 )
 
 
-def get_structure() -> SessionKeysAbpV10XTypeDef:
+def get_value() -> SessionKeysAbpV10XTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iotwireless-1.28.15.post1/README.md` & `mypy-boto3-iotwireless-1.28.16/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotwireless.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotwireless)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotwireless)](https://pepy.tech/project/mypy-boto3-iotwireless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTWireless 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless)
+[boto3.IoTWireless 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless)
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
 [mypy-boto3-iotwireless docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/).
 
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
@@ -294,20 +294,20 @@
 )
 
 
 def check_value(value: ApplicationConfigTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_iotwireless.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_iotwireless.type_defs import (
     SessionKeysAbpV10XTypeDef,
     SessionKeysAbpV11TypeDef,
     AccuracyTypeDef,
     ApplicationConfigTypeDef,
@@ -318,14 +318,15 @@
     AssociateWirelessDeviceWithFuotaTaskRequestRequestTypeDef,
     AssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef,
     AssociateWirelessDeviceWithThingRequestRequestTypeDef,
     AssociateWirelessGatewayWithCertificateRequestRequestTypeDef,
     AssociateWirelessGatewayWithThingRequestRequestTypeDef,
     BeaconingOutputTypeDef,
     BeaconingTypeDef,
+    BlobTypeDef,
     CancelMulticastGroupSessionRequestRequestTypeDef,
     CdmaLocalIdTypeDef,
     CdmaNmrObjTypeDef,
     CertificateListTypeDef,
     LoRaWANConnectionStatusEventNotificationConfigurationsTypeDef,
     LoRaWANConnectionStatusResourceTypeEventConfigurationTypeDef,
     LoRaWANDeviceProfileTypeDef,
@@ -374,14 +375,15 @@
     LoRaWANMulticastSessionOutputTypeDef,
     GetNetworkAnalyzerConfigurationRequestRequestTypeDef,
     GetPartnerAccountRequestRequestTypeDef,
     SidewalkAccountInfoWithFingerprintTypeDef,
     GetPositionConfigurationRequestRequestTypeDef,
     GnssTypeDef,
     IpTypeDef,
+    TimestampTypeDef,
     WiFiAccessPointTypeDef,
     GetPositionRequestRequestTypeDef,
     GetResourceEventConfigurationRequestRequestTypeDef,
     GetResourceLogLevelRequestRequestTypeDef,
     GetResourcePositionRequestRequestTypeDef,
     GetServiceEndpointRequestRequestTypeDef,
     GetServiceProfileRequestRequestTypeDef,
@@ -425,16 +427,14 @@
     ListWirelessGatewaysRequestRequestTypeDef,
     LoRaWANGatewayMetadataTypeDef,
     OtaaV10XTypeDef,
     OtaaV11TypeDef,
     LoRaWANGatewayVersionTypeDef,
     LoRaWANListDeviceTypeDef,
     LoRaWANMulticastMetadataTypeDef,
-    LoRaWANMulticastSessionTypeDef,
-    LoRaWANStartFuotaTaskTypeDef,
     UpdateAbpV10XTypeDef,
     UpdateAbpV11TypeDef,
     LteLocalIdTypeDef,
     LteNmrObjTypeDef,
     SemtechGnssConfigurationTypeDef,
     SemtechGnssDetailTypeDef,
     PutResourceLogLevelRequestRequestTypeDef,
@@ -446,15 +446,14 @@
     SidewalkUpdateImportInfoTypeDef,
     TdscdmaLocalIdTypeDef,
     TdscdmaNmrObjTypeDef,
     TestWirelessDeviceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDestinationRequestRequestTypeDef,
     UpdatePositionRequestRequestTypeDef,
-    UpdateResourcePositionRequestRequestTypeDef,
     UpdateWirelessGatewayRequestRequestTypeDef,
     WcdmaLocalIdTypeDef,
     WcdmaNmrObjTypeDef,
     WirelessDeviceEventLogOptionTypeDef,
     WirelessGatewayEventLogOptionTypeDef,
     AbpV10XTypeDef,
     AbpV11TypeDef,
@@ -488,14 +487,15 @@
     SendDataToMulticastGroupResponseTypeDef,
     SendDataToWirelessDeviceResponseTypeDef,
     StartSingleWirelessDeviceImportTaskResponseTypeDef,
     StartWirelessDeviceImportTaskResponseTypeDef,
     TestWirelessDeviceResponseTypeDef,
     LoRaWANGatewayOutputTypeDef,
     LoRaWANGatewayTypeDef,
+    UpdateResourcePositionRequestRequestTypeDef,
     CdmaObjTypeDef,
     SidewalkDeviceTypeDef,
     SidewalkListDeviceTypeDef,
     ConnectionStatusEventConfigurationTypeDef,
     ConnectionStatusResourceTypeEventConfigurationTypeDef,
     CreateDeviceProfileRequestRequestTypeDef,
     CreateFuotaTaskRequestRequestTypeDef,
@@ -517,19 +517,22 @@
     ProximityResourceTypeEventConfigurationTypeDef,
     FPortsOutputTypeDef,
     FPortsTypeDef,
     UpdateFPortsTypeDef,
     ListFuotaTasksResponseTypeDef,
     ParticipatingGatewaysOutputTypeDef,
     ParticipatingGatewaysTypeDef,
+    LoRaWANDeviceProfileUnionTypeDef,
     GetFuotaTaskResponseTypeDef,
     GetMulticastGroupResponseTypeDef,
     GetMulticastGroupSessionResponseTypeDef,
     GetPartnerAccountResponseTypeDef,
     ListPartnerAccountsResponseTypeDef,
+    LoRaWANMulticastSessionTypeDef,
+    LoRaWANStartFuotaTaskTypeDef,
     GetServiceProfileResponseTypeDef,
     GetWirelessDeviceImportTaskResponseTypeDef,
     WirelessDeviceImportTaskTypeDef,
     GsmNmrObjTypeDef,
     ImportedWirelessDeviceTypeDef,
     JoinEventConfigurationTypeDef,
     JoinResourceTypeEventConfigurationTypeDef,
@@ -538,16 +541,14 @@
     ListNetworkAnalyzerConfigurationsResponseTypeDef,
     ListServiceProfilesResponseTypeDef,
     LoRaWANDeviceMetadataTypeDef,
     LoRaWANGatewayCurrentVersionTypeDef,
     LoRaWANUpdateGatewayTaskCreateTypeDef,
     LoRaWANUpdateGatewayTaskEntryTypeDef,
     MulticastWirelessMetadataTypeDef,
-    StartMulticastGroupSessionRequestRequestTypeDef,
-    StartFuotaTaskRequestRequestTypeDef,
     LteObjTypeDef,
     PositionSolverConfigurationsTypeDef,
     PositionSolverDetailsTypeDef,
     StartSingleWirelessDeviceImportTaskRequestRequestTypeDef,
     StartWirelessDeviceImportTaskRequestRequestTypeDef,
     UpdatePartnerAccountRequestRequestTypeDef,
     UpdateWirelessDeviceImportTaskRequestRequestTypeDef,
@@ -556,21 +557,25 @@
     WirelessDeviceLogOptionOutputTypeDef,
     WirelessDeviceLogOptionTypeDef,
     WirelessGatewayLogOptionOutputTypeDef,
     WirelessGatewayLogOptionTypeDef,
     GetWirelessGatewayResponseTypeDef,
     WirelessGatewayStatisticsTypeDef,
     CreateWirelessGatewayRequestRequestTypeDef,
+    LoRaWANGatewayUnionTypeDef,
     WirelessDeviceStatisticsTypeDef,
     GetDeviceProfileResponseTypeDef,
     LoRaWANDeviceOutputTypeDef,
     LoRaWANDeviceTypeDef,
     LoRaWANUpdateDeviceTypeDef,
     LoRaWANSendDataToDeviceOutputTypeDef,
     LoRaWANSendDataToDeviceTypeDef,
+    LoRaWANMulticastSessionUnionTypeDef,
+    StartMulticastGroupSessionRequestRequestTypeDef,
+    StartFuotaTaskRequestRequestTypeDef,
     ListWirelessDeviceImportTasksResponseTypeDef,
     GsmObjTypeDef,
     ListDevicesForWirelessDeviceImportTaskResponseTypeDef,
     EventNotificationItemConfigurationsTypeDef,
     GetResourceEventConfigurationResponseTypeDef,
     UpdateResourceEventConfigurationRequestRequestTypeDef,
     GetEventConfigurationByResourceTypesResponseTypeDef,
@@ -579,37 +584,40 @@
     GetWirelessGatewayFirmwareInformationResponseTypeDef,
     UpdateWirelessGatewayTaskCreateTypeDef,
     UpdateWirelessGatewayTaskEntryTypeDef,
     SendDataToMulticastGroupRequestRequestTypeDef,
     PutPositionConfigurationRequestRequestTypeDef,
     GetPositionConfigurationResponseTypeDef,
     PositionConfigurationItemTypeDef,
+    WirelessDeviceLogOptionUnionTypeDef,
     GetLogLevelsByResourceTypesResponseTypeDef,
-    UpdateLogLevelsByResourceTypesRequestRequestTypeDef,
+    WirelessGatewayLogOptionUnionTypeDef,
     ListWirelessGatewaysResponseTypeDef,
     ListWirelessDevicesResponseTypeDef,
     GetWirelessDeviceResponseTypeDef,
     CreateWirelessDeviceRequestRequestTypeDef,
+    LoRaWANDeviceUnionTypeDef,
     UpdateWirelessDeviceRequestRequestTypeDef,
     DownlinkQueueMessageTypeDef,
     WirelessMetadataTypeDef,
     CellTowersTypeDef,
     EventConfigurationItemTypeDef,
     CreateWirelessGatewayTaskDefinitionRequestRequestTypeDef,
     GetWirelessGatewayTaskDefinitionResponseTypeDef,
     ListWirelessGatewayTaskDefinitionsResponseTypeDef,
     ListPositionConfigurationsResponseTypeDef,
+    UpdateLogLevelsByResourceTypesRequestRequestTypeDef,
     ListQueuedMessagesResponseTypeDef,
     SendDataToWirelessDeviceRequestRequestTypeDef,
     GetPositionEstimateRequestRequestTypeDef,
     ListEventConfigurationsResponseTypeDef,
 )
 
 
-def get_structure() -> SessionKeysAbpV10XTypeDef:
+def get_value() -> SessionKeysAbpV10XTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iotwireless-1.28.15.post1/mypy_boto3_iotwireless/__main__.py` & `mypy-boto3-iotwireless-1.28.16/mypy_boto3_iotwireless/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IoTWireless 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.IoTWireless 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless\nOther"
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

### Comparing `mypy-boto3-iotwireless-1.28.15.post1/mypy_boto3_iotwireless/client.py` & `mypy-boto3-iotwireless-1.28.16/mypy_boto3_iotwireless/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,19 +10,17 @@
     from mypy_boto3_iotwireless.client import IoTWirelessClient
 
     session = Session()
     client: IoTWirelessClient = session.client("iotwireless")
     ```
 """
 import sys
-from datetime import datetime
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
 from .literals import (
     DeviceProfileTypeType,
     EventNotificationResourceTypeType,
     ExpressionTypeType,
     IdentifierTypeType,
     LogLevelType,
@@ -33,14 +31,15 @@
     WirelessDeviceTypeType,
     WirelessGatewayIdTypeType,
     WirelessGatewayServiceTypeType,
 )
 from .type_defs import (
     AssociateAwsAccountWithPartnerAccountResponseTypeDef,
     AssociateWirelessGatewayWithCertificateResponseTypeDef,
+    BlobTypeDef,
     CellTowersTypeDef,
     ConnectionStatusEventConfigurationTypeDef,
     ConnectionStatusResourceTypeEventConfigurationTypeDef,
     CreateDestinationResponseTypeDef,
     CreateDeviceProfileResponseTypeDef,
     CreateFuotaTaskResponseTypeDef,
     CreateMulticastGroupResponseTypeDef,
@@ -95,23 +94,19 @@
     ListQueuedMessagesResponseTypeDef,
     ListServiceProfilesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWirelessDeviceImportTasksResponseTypeDef,
     ListWirelessDevicesResponseTypeDef,
     ListWirelessGatewaysResponseTypeDef,
     ListWirelessGatewayTaskDefinitionsResponseTypeDef,
-    LoRaWANDeviceOutputTypeDef,
-    LoRaWANDeviceProfileOutputTypeDef,
-    LoRaWANDeviceProfileTypeDef,
-    LoRaWANDeviceTypeDef,
+    LoRaWANDeviceProfileUnionTypeDef,
+    LoRaWANDeviceUnionTypeDef,
     LoRaWANFuotaTaskTypeDef,
-    LoRaWANGatewayOutputTypeDef,
-    LoRaWANGatewayTypeDef,
-    LoRaWANMulticastSessionOutputTypeDef,
-    LoRaWANMulticastSessionTypeDef,
+    LoRaWANGatewayUnionTypeDef,
+    LoRaWANMulticastSessionUnionTypeDef,
     LoRaWANMulticastTypeDef,
     LoRaWANServiceProfileTypeDef,
     LoRaWANStartFuotaTaskTypeDef,
     LoRaWANUpdateDeviceTypeDef,
     MessageDeliveryStatusEventConfigurationTypeDef,
     MessageDeliveryStatusResourceTypeEventConfigurationTypeDef,
     MulticastWirelessMetadataTypeDef,
@@ -126,21 +121,20 @@
     SidewalkStartImportInfoTypeDef,
     SidewalkUpdateAccountTypeDef,
     SidewalkUpdateImportInfoTypeDef,
     StartSingleWirelessDeviceImportTaskResponseTypeDef,
     StartWirelessDeviceImportTaskResponseTypeDef,
     TagTypeDef,
     TestWirelessDeviceResponseTypeDef,
+    TimestampTypeDef,
     TraceContentTypeDef,
     UpdateWirelessGatewayTaskCreateTypeDef,
     WiFiAccessPointTypeDef,
-    WirelessDeviceLogOptionOutputTypeDef,
-    WirelessDeviceLogOptionTypeDef,
-    WirelessGatewayLogOptionOutputTypeDef,
-    WirelessGatewayLogOptionTypeDef,
+    WirelessDeviceLogOptionUnionTypeDef,
+    WirelessGatewayLogOptionUnionTypeDef,
     WirelessMetadataTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -297,15 +291,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/client/#create_destination)
         """
 
     def create_device_profile(
         self,
         *,
         Name: str = ...,
-        LoRaWAN: Union[LoRaWANDeviceProfileTypeDef, LoRaWANDeviceProfileOutputTypeDef] = ...,
+        LoRaWAN: LoRaWANDeviceProfileUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ClientRequestToken: str = ...,
         Sidewalk: Mapping[str, Any] = ...
     ) -> CreateDeviceProfileResponseTypeDef:
         """
         Creates a new device profile.
 
@@ -388,30 +382,30 @@
         self,
         *,
         Type: WirelessDeviceTypeType,
         DestinationName: str,
         Name: str = ...,
         Description: str = ...,
         ClientRequestToken: str = ...,
-        LoRaWAN: Union[LoRaWANDeviceTypeDef, LoRaWANDeviceOutputTypeDef] = ...,
+        LoRaWAN: LoRaWANDeviceUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         Positioning: PositioningConfigStatusType = ...,
         Sidewalk: SidewalkCreateWirelessDeviceTypeDef = ...
     ) -> CreateWirelessDeviceResponseTypeDef:
         """
         Provisions a wireless device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.create_wireless_device)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/client/#create_wireless_device)
         """
 
     def create_wireless_gateway(
         self,
         *,
-        LoRaWAN: Union[LoRaWANGatewayTypeDef, LoRaWANGatewayOutputTypeDef],
+        LoRaWAN: LoRaWANGatewayUnionTypeDef,
         Name: str = ...,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ClientRequestToken: str = ...
     ) -> CreateWirelessGatewayResponseTypeDef:
         """
         Provisions a wireless gateway.
@@ -733,15 +727,15 @@
     def get_position_estimate(
         self,
         *,
         WiFiAccessPoints: Sequence[WiFiAccessPointTypeDef] = ...,
         CellTowers: CellTowersTypeDef = ...,
         Ip: IpTypeDef = ...,
         Gnss: GnssTypeDef = ...,
-        Timestamp: Union[datetime, str] = ...
+        Timestamp: TimestampTypeDef = ...
     ) -> GetPositionEstimateResponseTypeDef:
         """
         Get estimated position information as a payload in GeoJSON format.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.get_position_estimate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/client/#get_position_estimate)
         """
@@ -1193,18 +1187,15 @@
         Starts a FUOTA task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.start_fuota_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/client/#start_fuota_task)
         """
 
     def start_multicast_group_session(
-        self,
-        *,
-        Id: str,
-        LoRaWAN: Union[LoRaWANMulticastSessionTypeDef, LoRaWANMulticastSessionOutputTypeDef]
+        self, *, Id: str, LoRaWAN: LoRaWANMulticastSessionUnionTypeDef
     ) -> Dict[str, Any]:
         """
         Starts a multicast group session.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.start_multicast_group_session)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/client/#start_multicast_group_session)
         """
@@ -1317,20 +1308,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/client/#update_fuota_task)
         """
 
     def update_log_levels_by_resource_types(
         self,
         *,
         DefaultLogLevel: LogLevelType = ...,
-        WirelessDeviceLogOptions: Sequence[
-            Union[WirelessDeviceLogOptionTypeDef, WirelessDeviceLogOptionOutputTypeDef]
-        ] = ...,
-        WirelessGatewayLogOptions: Sequence[
-            Union[WirelessGatewayLogOptionTypeDef, WirelessGatewayLogOptionOutputTypeDef]
-        ] = ...
+        WirelessDeviceLogOptions: Sequence[WirelessDeviceLogOptionUnionTypeDef] = ...,
+        WirelessGatewayLogOptions: Sequence[WirelessGatewayLogOptionUnionTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Set default log level, or log levels by resource types.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.update_log_levels_by_resource_types)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/client/#update_log_levels_by_resource_types)
         """
@@ -1418,15 +1405,15 @@
         """
 
     def update_resource_position(
         self,
         *,
         ResourceIdentifier: str,
         ResourceType: PositionResourceTypeType,
-        GeoJsonPayload: Union[str, bytes, IO[Any], StreamingBody] = ...
+        GeoJsonPayload: BlobTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Update the position information of a given wireless device or a wireless gateway
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.update_resource_position)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/client/#update_resource_position)
```

### Comparing `mypy-boto3-iotwireless-1.28.15.post1/mypy_boto3_iotwireless/client.pyi` & `mypy-boto3-iotwireless-1.28.16/mypy_boto3_iotwireless/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,19 +10,17 @@
     from mypy_boto3_iotwireless.client import IoTWirelessClient
 
     session = Session()
     client: IoTWirelessClient = session.client("iotwireless")
     ```
 """
 import sys
-from datetime import datetime
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
 from .literals import (
     DeviceProfileTypeType,
     EventNotificationResourceTypeType,
     ExpressionTypeType,
     IdentifierTypeType,
     LogLevelType,
@@ -33,14 +31,15 @@
     WirelessDeviceTypeType,
     WirelessGatewayIdTypeType,
     WirelessGatewayServiceTypeType,
 )
 from .type_defs import (
     AssociateAwsAccountWithPartnerAccountResponseTypeDef,
     AssociateWirelessGatewayWithCertificateResponseTypeDef,
+    BlobTypeDef,
     CellTowersTypeDef,
     ConnectionStatusEventConfigurationTypeDef,
     ConnectionStatusResourceTypeEventConfigurationTypeDef,
     CreateDestinationResponseTypeDef,
     CreateDeviceProfileResponseTypeDef,
     CreateFuotaTaskResponseTypeDef,
     CreateMulticastGroupResponseTypeDef,
@@ -95,23 +94,19 @@
     ListQueuedMessagesResponseTypeDef,
     ListServiceProfilesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWirelessDeviceImportTasksResponseTypeDef,
     ListWirelessDevicesResponseTypeDef,
     ListWirelessGatewaysResponseTypeDef,
     ListWirelessGatewayTaskDefinitionsResponseTypeDef,
-    LoRaWANDeviceOutputTypeDef,
-    LoRaWANDeviceProfileOutputTypeDef,
-    LoRaWANDeviceProfileTypeDef,
-    LoRaWANDeviceTypeDef,
+    LoRaWANDeviceProfileUnionTypeDef,
+    LoRaWANDeviceUnionTypeDef,
     LoRaWANFuotaTaskTypeDef,
-    LoRaWANGatewayOutputTypeDef,
-    LoRaWANGatewayTypeDef,
-    LoRaWANMulticastSessionOutputTypeDef,
-    LoRaWANMulticastSessionTypeDef,
+    LoRaWANGatewayUnionTypeDef,
+    LoRaWANMulticastSessionUnionTypeDef,
     LoRaWANMulticastTypeDef,
     LoRaWANServiceProfileTypeDef,
     LoRaWANStartFuotaTaskTypeDef,
     LoRaWANUpdateDeviceTypeDef,
     MessageDeliveryStatusEventConfigurationTypeDef,
     MessageDeliveryStatusResourceTypeEventConfigurationTypeDef,
     MulticastWirelessMetadataTypeDef,
@@ -126,21 +121,20 @@
     SidewalkStartImportInfoTypeDef,
     SidewalkUpdateAccountTypeDef,
     SidewalkUpdateImportInfoTypeDef,
     StartSingleWirelessDeviceImportTaskResponseTypeDef,
     StartWirelessDeviceImportTaskResponseTypeDef,
     TagTypeDef,
     TestWirelessDeviceResponseTypeDef,
+    TimestampTypeDef,
     TraceContentTypeDef,
     UpdateWirelessGatewayTaskCreateTypeDef,
     WiFiAccessPointTypeDef,
-    WirelessDeviceLogOptionOutputTypeDef,
-    WirelessDeviceLogOptionTypeDef,
-    WirelessGatewayLogOptionOutputTypeDef,
-    WirelessGatewayLogOptionTypeDef,
+    WirelessDeviceLogOptionUnionTypeDef,
+    WirelessGatewayLogOptionUnionTypeDef,
     WirelessMetadataTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -281,15 +275,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.create_destination)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/client/#create_destination)
         """
     def create_device_profile(
         self,
         *,
         Name: str = ...,
-        LoRaWAN: Union[LoRaWANDeviceProfileTypeDef, LoRaWANDeviceProfileOutputTypeDef] = ...,
+        LoRaWAN: LoRaWANDeviceProfileUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ClientRequestToken: str = ...,
         Sidewalk: Mapping[str, Any] = ...
     ) -> CreateDeviceProfileResponseTypeDef:
         """
         Creates a new device profile.
 
@@ -367,29 +361,29 @@
         self,
         *,
         Type: WirelessDeviceTypeType,
         DestinationName: str,
         Name: str = ...,
         Description: str = ...,
         ClientRequestToken: str = ...,
-        LoRaWAN: Union[LoRaWANDeviceTypeDef, LoRaWANDeviceOutputTypeDef] = ...,
+        LoRaWAN: LoRaWANDeviceUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         Positioning: PositioningConfigStatusType = ...,
         Sidewalk: SidewalkCreateWirelessDeviceTypeDef = ...
     ) -> CreateWirelessDeviceResponseTypeDef:
         """
         Provisions a wireless device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.create_wireless_device)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/client/#create_wireless_device)
         """
     def create_wireless_gateway(
         self,
         *,
-        LoRaWAN: Union[LoRaWANGatewayTypeDef, LoRaWANGatewayOutputTypeDef],
+        LoRaWAN: LoRaWANGatewayUnionTypeDef,
         Name: str = ...,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ClientRequestToken: str = ...
     ) -> CreateWirelessGatewayResponseTypeDef:
         """
         Provisions a wireless gateway.
@@ -676,15 +670,15 @@
     def get_position_estimate(
         self,
         *,
         WiFiAccessPoints: Sequence[WiFiAccessPointTypeDef] = ...,
         CellTowers: CellTowersTypeDef = ...,
         Ip: IpTypeDef = ...,
         Gnss: GnssTypeDef = ...,
-        Timestamp: Union[datetime, str] = ...
+        Timestamp: TimestampTypeDef = ...
     ) -> GetPositionEstimateResponseTypeDef:
         """
         Get estimated position information as a payload in GeoJSON format.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.get_position_estimate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/client/#get_position_estimate)
         """
@@ -1095,18 +1089,15 @@
         """
         Starts a FUOTA task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.start_fuota_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/client/#start_fuota_task)
         """
     def start_multicast_group_session(
-        self,
-        *,
-        Id: str,
-        LoRaWAN: Union[LoRaWANMulticastSessionTypeDef, LoRaWANMulticastSessionOutputTypeDef]
+        self, *, Id: str, LoRaWAN: LoRaWANMulticastSessionUnionTypeDef
     ) -> Dict[str, Any]:
         """
         Starts a multicast group session.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.start_multicast_group_session)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/client/#start_multicast_group_session)
         """
@@ -1210,20 +1201,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.update_fuota_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/client/#update_fuota_task)
         """
     def update_log_levels_by_resource_types(
         self,
         *,
         DefaultLogLevel: LogLevelType = ...,
-        WirelessDeviceLogOptions: Sequence[
-            Union[WirelessDeviceLogOptionTypeDef, WirelessDeviceLogOptionOutputTypeDef]
-        ] = ...,
-        WirelessGatewayLogOptions: Sequence[
-            Union[WirelessGatewayLogOptionTypeDef, WirelessGatewayLogOptionOutputTypeDef]
-        ] = ...
+        WirelessDeviceLogOptions: Sequence[WirelessDeviceLogOptionUnionTypeDef] = ...,
+        WirelessGatewayLogOptions: Sequence[WirelessGatewayLogOptionUnionTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Set default log level, or log levels by resource types.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.update_log_levels_by_resource_types)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/client/#update_log_levels_by_resource_types)
         """
@@ -1305,15 +1292,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/client/#update_resource_event_configuration)
         """
     def update_resource_position(
         self,
         *,
         ResourceIdentifier: str,
         ResourceType: PositionResourceTypeType,
-        GeoJsonPayload: Union[str, bytes, IO[Any], StreamingBody] = ...
+        GeoJsonPayload: BlobTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Update the position information of a given wireless device or a wireless gateway
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.update_resource_position)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/client/#update_resource_position)
```

### Comparing `mypy-boto3-iotwireless-1.28.15.post1/mypy_boto3_iotwireless/literals.py` & `mypy-boto3-iotwireless-1.28.16/mypy_boto3_iotwireless/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotwireless-1.28.15.post1/mypy_boto3_iotwireless/literals.pyi` & `mypy-boto3-iotwireless-1.28.16/mypy_boto3_iotwireless/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotwireless-1.28.15.post1/mypy_boto3_iotwireless/type_defs.py` & `mypy-boto3-iotwireless-1.28.16/mypy_boto3_iotwireless/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_iotwireless.type_defs import SessionKeysAbpV10XTypeDef
 
-    data: SessionKeysAbpV10XTypeDef = {...}
+    data: SessionKeysAbpV10XTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -75,14 +75,15 @@
     "AssociateWirelessDeviceWithFuotaTaskRequestRequestTypeDef",
     "AssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef",
     "AssociateWirelessDeviceWithThingRequestRequestTypeDef",
     "AssociateWirelessGatewayWithCertificateRequestRequestTypeDef",
     "AssociateWirelessGatewayWithThingRequestRequestTypeDef",
     "BeaconingOutputTypeDef",
     "BeaconingTypeDef",
+    "BlobTypeDef",
     "CancelMulticastGroupSessionRequestRequestTypeDef",
     "CdmaLocalIdTypeDef",
     "CdmaNmrObjTypeDef",
     "CertificateListTypeDef",
     "LoRaWANConnectionStatusEventNotificationConfigurationsTypeDef",
     "LoRaWANConnectionStatusResourceTypeEventConfigurationTypeDef",
     "LoRaWANDeviceProfileTypeDef",
@@ -131,14 +132,15 @@
     "LoRaWANMulticastSessionOutputTypeDef",
     "GetNetworkAnalyzerConfigurationRequestRequestTypeDef",
     "GetPartnerAccountRequestRequestTypeDef",
     "SidewalkAccountInfoWithFingerprintTypeDef",
     "GetPositionConfigurationRequestRequestTypeDef",
     "GnssTypeDef",
     "IpTypeDef",
+    "TimestampTypeDef",
     "WiFiAccessPointTypeDef",
     "GetPositionRequestRequestTypeDef",
     "GetResourceEventConfigurationRequestRequestTypeDef",
     "GetResourceLogLevelRequestRequestTypeDef",
     "GetResourcePositionRequestRequestTypeDef",
     "GetServiceEndpointRequestRequestTypeDef",
     "GetServiceProfileRequestRequestTypeDef",
@@ -182,16 +184,14 @@
     "ListWirelessGatewaysRequestRequestTypeDef",
     "LoRaWANGatewayMetadataTypeDef",
     "OtaaV10XTypeDef",
     "OtaaV11TypeDef",
     "LoRaWANGatewayVersionTypeDef",
     "LoRaWANListDeviceTypeDef",
     "LoRaWANMulticastMetadataTypeDef",
-    "LoRaWANMulticastSessionTypeDef",
-    "LoRaWANStartFuotaTaskTypeDef",
     "UpdateAbpV10XTypeDef",
     "UpdateAbpV11TypeDef",
     "LteLocalIdTypeDef",
     "LteNmrObjTypeDef",
     "SemtechGnssConfigurationTypeDef",
     "SemtechGnssDetailTypeDef",
     "PutResourceLogLevelRequestRequestTypeDef",
@@ -203,15 +203,14 @@
     "SidewalkUpdateImportInfoTypeDef",
     "TdscdmaLocalIdTypeDef",
     "TdscdmaNmrObjTypeDef",
     "TestWirelessDeviceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDestinationRequestRequestTypeDef",
     "UpdatePositionRequestRequestTypeDef",
-    "UpdateResourcePositionRequestRequestTypeDef",
     "UpdateWirelessGatewayRequestRequestTypeDef",
     "WcdmaLocalIdTypeDef",
     "WcdmaNmrObjTypeDef",
     "WirelessDeviceEventLogOptionTypeDef",
     "WirelessGatewayEventLogOptionTypeDef",
     "AbpV10XTypeDef",
     "AbpV11TypeDef",
@@ -245,14 +244,15 @@
     "SendDataToMulticastGroupResponseTypeDef",
     "SendDataToWirelessDeviceResponseTypeDef",
     "StartSingleWirelessDeviceImportTaskResponseTypeDef",
     "StartWirelessDeviceImportTaskResponseTypeDef",
     "TestWirelessDeviceResponseTypeDef",
     "LoRaWANGatewayOutputTypeDef",
     "LoRaWANGatewayTypeDef",
+    "UpdateResourcePositionRequestRequestTypeDef",
     "CdmaObjTypeDef",
     "SidewalkDeviceTypeDef",
     "SidewalkListDeviceTypeDef",
     "ConnectionStatusEventConfigurationTypeDef",
     "ConnectionStatusResourceTypeEventConfigurationTypeDef",
     "CreateDeviceProfileRequestRequestTypeDef",
     "CreateFuotaTaskRequestRequestTypeDef",
@@ -274,19 +274,22 @@
     "ProximityResourceTypeEventConfigurationTypeDef",
     "FPortsOutputTypeDef",
     "FPortsTypeDef",
     "UpdateFPortsTypeDef",
     "ListFuotaTasksResponseTypeDef",
     "ParticipatingGatewaysOutputTypeDef",
     "ParticipatingGatewaysTypeDef",
+    "LoRaWANDeviceProfileUnionTypeDef",
     "GetFuotaTaskResponseTypeDef",
     "GetMulticastGroupResponseTypeDef",
     "GetMulticastGroupSessionResponseTypeDef",
     "GetPartnerAccountResponseTypeDef",
     "ListPartnerAccountsResponseTypeDef",
+    "LoRaWANMulticastSessionTypeDef",
+    "LoRaWANStartFuotaTaskTypeDef",
     "GetServiceProfileResponseTypeDef",
     "GetWirelessDeviceImportTaskResponseTypeDef",
     "WirelessDeviceImportTaskTypeDef",
     "GsmNmrObjTypeDef",
     "ImportedWirelessDeviceTypeDef",
     "JoinEventConfigurationTypeDef",
     "JoinResourceTypeEventConfigurationTypeDef",
@@ -295,16 +298,14 @@
     "ListNetworkAnalyzerConfigurationsResponseTypeDef",
     "ListServiceProfilesResponseTypeDef",
     "LoRaWANDeviceMetadataTypeDef",
     "LoRaWANGatewayCurrentVersionTypeDef",
     "LoRaWANUpdateGatewayTaskCreateTypeDef",
     "LoRaWANUpdateGatewayTaskEntryTypeDef",
     "MulticastWirelessMetadataTypeDef",
-    "StartMulticastGroupSessionRequestRequestTypeDef",
-    "StartFuotaTaskRequestRequestTypeDef",
     "LteObjTypeDef",
     "PositionSolverConfigurationsTypeDef",
     "PositionSolverDetailsTypeDef",
     "StartSingleWirelessDeviceImportTaskRequestRequestTypeDef",
     "StartWirelessDeviceImportTaskRequestRequestTypeDef",
     "UpdatePartnerAccountRequestRequestTypeDef",
     "UpdateWirelessDeviceImportTaskRequestRequestTypeDef",
@@ -313,21 +314,25 @@
     "WirelessDeviceLogOptionOutputTypeDef",
     "WirelessDeviceLogOptionTypeDef",
     "WirelessGatewayLogOptionOutputTypeDef",
     "WirelessGatewayLogOptionTypeDef",
     "GetWirelessGatewayResponseTypeDef",
     "WirelessGatewayStatisticsTypeDef",
     "CreateWirelessGatewayRequestRequestTypeDef",
+    "LoRaWANGatewayUnionTypeDef",
     "WirelessDeviceStatisticsTypeDef",
     "GetDeviceProfileResponseTypeDef",
     "LoRaWANDeviceOutputTypeDef",
     "LoRaWANDeviceTypeDef",
     "LoRaWANUpdateDeviceTypeDef",
     "LoRaWANSendDataToDeviceOutputTypeDef",
     "LoRaWANSendDataToDeviceTypeDef",
+    "LoRaWANMulticastSessionUnionTypeDef",
+    "StartMulticastGroupSessionRequestRequestTypeDef",
+    "StartFuotaTaskRequestRequestTypeDef",
     "ListWirelessDeviceImportTasksResponseTypeDef",
     "GsmObjTypeDef",
     "ListDevicesForWirelessDeviceImportTaskResponseTypeDef",
     "EventNotificationItemConfigurationsTypeDef",
     "GetResourceEventConfigurationResponseTypeDef",
     "UpdateResourceEventConfigurationRequestRequestTypeDef",
     "GetEventConfigurationByResourceTypesResponseTypeDef",
@@ -336,29 +341,32 @@
     "GetWirelessGatewayFirmwareInformationResponseTypeDef",
     "UpdateWirelessGatewayTaskCreateTypeDef",
     "UpdateWirelessGatewayTaskEntryTypeDef",
     "SendDataToMulticastGroupRequestRequestTypeDef",
     "PutPositionConfigurationRequestRequestTypeDef",
     "GetPositionConfigurationResponseTypeDef",
     "PositionConfigurationItemTypeDef",
+    "WirelessDeviceLogOptionUnionTypeDef",
     "GetLogLevelsByResourceTypesResponseTypeDef",
-    "UpdateLogLevelsByResourceTypesRequestRequestTypeDef",
+    "WirelessGatewayLogOptionUnionTypeDef",
     "ListWirelessGatewaysResponseTypeDef",
     "ListWirelessDevicesResponseTypeDef",
     "GetWirelessDeviceResponseTypeDef",
     "CreateWirelessDeviceRequestRequestTypeDef",
+    "LoRaWANDeviceUnionTypeDef",
     "UpdateWirelessDeviceRequestRequestTypeDef",
     "DownlinkQueueMessageTypeDef",
     "WirelessMetadataTypeDef",
     "CellTowersTypeDef",
     "EventConfigurationItemTypeDef",
     "CreateWirelessGatewayTaskDefinitionRequestRequestTypeDef",
     "GetWirelessGatewayTaskDefinitionResponseTypeDef",
     "ListWirelessGatewayTaskDefinitionsResponseTypeDef",
     "ListPositionConfigurationsResponseTypeDef",
+    "UpdateLogLevelsByResourceTypesRequestRequestTypeDef",
     "ListQueuedMessagesResponseTypeDef",
     "SendDataToWirelessDeviceRequestRequestTypeDef",
     "GetPositionEstimateRequestRequestTypeDef",
     "ListEventConfigurationsResponseTypeDef",
 )
 
 SessionKeysAbpV10XTypeDef = TypedDict(
@@ -490,14 +498,15 @@
     {
         "DataRate": int,
         "Frequencies": Sequence[int],
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CancelMulticastGroupSessionRequestRequestTypeDef = TypedDict(
     "CancelMulticastGroupSessionRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -1053,14 +1062,15 @@
 IpTypeDef = TypedDict(
     "IpTypeDef",
     {
         "IpAddress": str,
     },
 )
 
+TimestampTypeDef = Union[datetime, str]
 WiFiAccessPointTypeDef = TypedDict(
     "WiFiAccessPointTypeDef",
     {
         "MacAddress": str,
         "Rss": int,
     },
 )
@@ -1588,34 +1598,14 @@
     "LoRaWANMulticastMetadataTypeDef",
     {
         "FPort": int,
     },
     total=False,
 )
 
-LoRaWANMulticastSessionTypeDef = TypedDict(
-    "LoRaWANMulticastSessionTypeDef",
-    {
-        "DlDr": int,
-        "DlFreq": int,
-        "SessionStartTime": Union[datetime, str],
-        "SessionTimeout": int,
-        "PingSlotPeriod": int,
-    },
-    total=False,
-)
-
-LoRaWANStartFuotaTaskTypeDef = TypedDict(
-    "LoRaWANStartFuotaTaskTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-    },
-    total=False,
-)
-
 UpdateAbpV10XTypeDef = TypedDict(
     "UpdateAbpV10XTypeDef",
     {
         "FCntStart": int,
     },
     total=False,
 )
@@ -1811,37 +1801,14 @@
     {
         "ResourceIdentifier": str,
         "ResourceType": PositionResourceTypeType,
         "Position": Sequence[float],
     },
 )
 
-_RequiredUpdateResourcePositionRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateResourcePositionRequestRequestTypeDef",
-    {
-        "ResourceIdentifier": str,
-        "ResourceType": PositionResourceTypeType,
-    },
-)
-_OptionalUpdateResourcePositionRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateResourcePositionRequestRequestTypeDef",
-    {
-        "GeoJsonPayload": Union[str, bytes, IO[Any], StreamingBody],
-    },
-    total=False,
-)
-
-
-class UpdateResourcePositionRequestRequestTypeDef(
-    _RequiredUpdateResourcePositionRequestRequestTypeDef,
-    _OptionalUpdateResourcePositionRequestRequestTypeDef,
-):
-    pass
-
-
 _RequiredUpdateWirelessGatewayRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateWirelessGatewayRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalUpdateWirelessGatewayRequestRequestTypeDef = TypedDict(
@@ -2305,14 +2272,37 @@
         "SubBands": Sequence[int],
         "Beaconing": BeaconingTypeDef,
         "MaxEirp": float,
     },
     total=False,
 )
 
+_RequiredUpdateResourcePositionRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateResourcePositionRequestRequestTypeDef",
+    {
+        "ResourceIdentifier": str,
+        "ResourceType": PositionResourceTypeType,
+    },
+)
+_OptionalUpdateResourcePositionRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateResourcePositionRequestRequestTypeDef",
+    {
+        "GeoJsonPayload": BlobTypeDef,
+    },
+    total=False,
+)
+
+
+class UpdateResourcePositionRequestRequestTypeDef(
+    _RequiredUpdateResourcePositionRequestRequestTypeDef,
+    _OptionalUpdateResourcePositionRequestRequestTypeDef,
+):
+    pass
+
+
 _RequiredCdmaObjTypeDef = TypedDict(
     "_RequiredCdmaObjTypeDef",
     {
         "SystemId": int,
         "NetworkId": int,
         "BaseStationId": int,
     },
@@ -2715,14 +2705,17 @@
     {
         "DownlinkMode": DownlinkModeType,
         "GatewayList": Sequence[GatewayListItemTypeDef],
         "TransmissionInterval": int,
     },
 )
 
+LoRaWANDeviceProfileUnionTypeDef = Union[
+    LoRaWANDeviceProfileTypeDef, LoRaWANDeviceProfileOutputTypeDef
+]
 GetFuotaTaskResponseTypeDef = TypedDict(
     "GetFuotaTaskResponseTypeDef",
     {
         "Arn": str,
         "Id": str,
         "Status": FuotaTaskStatusType,
         "Name": str,
@@ -2774,14 +2767,34 @@
     {
         "NextToken": str,
         "Sidewalk": List[SidewalkAccountInfoWithFingerprintTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+LoRaWANMulticastSessionTypeDef = TypedDict(
+    "LoRaWANMulticastSessionTypeDef",
+    {
+        "DlDr": int,
+        "DlFreq": int,
+        "SessionStartTime": TimestampTypeDef,
+        "SessionTimeout": int,
+        "PingSlotPeriod": int,
+    },
+    total=False,
+)
+
+LoRaWANStartFuotaTaskTypeDef = TypedDict(
+    "LoRaWANStartFuotaTaskTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+    },
+    total=False,
+)
+
 GetServiceProfileResponseTypeDef = TypedDict(
     "GetServiceProfileResponseTypeDef",
     {
         "Arn": str,
         "Name": str,
         "Id": str,
         "LoRaWAN": LoRaWANGetServiceProfileInfoTypeDef,
@@ -2952,43 +2965,14 @@
     "MulticastWirelessMetadataTypeDef",
     {
         "LoRaWAN": LoRaWANMulticastMetadataTypeDef,
     },
     total=False,
 )
 
-StartMulticastGroupSessionRequestRequestTypeDef = TypedDict(
-    "StartMulticastGroupSessionRequestRequestTypeDef",
-    {
-        "Id": str,
-        "LoRaWAN": LoRaWANMulticastSessionTypeDef,
-    },
-)
-
-_RequiredStartFuotaTaskRequestRequestTypeDef = TypedDict(
-    "_RequiredStartFuotaTaskRequestRequestTypeDef",
-    {
-        "Id": str,
-    },
-)
-_OptionalStartFuotaTaskRequestRequestTypeDef = TypedDict(
-    "_OptionalStartFuotaTaskRequestRequestTypeDef",
-    {
-        "LoRaWAN": LoRaWANStartFuotaTaskTypeDef,
-    },
-    total=False,
-)
-
-
-class StartFuotaTaskRequestRequestTypeDef(
-    _RequiredStartFuotaTaskRequestRequestTypeDef, _OptionalStartFuotaTaskRequestRequestTypeDef
-):
-    pass
-
-
 _RequiredLteObjTypeDef = TypedDict(
     "_RequiredLteObjTypeDef",
     {
         "Mcc": int,
         "Mnc": int,
         "EutranCid": int,
     },
@@ -3281,14 +3265,15 @@
 class CreateWirelessGatewayRequestRequestTypeDef(
     _RequiredCreateWirelessGatewayRequestRequestTypeDef,
     _OptionalCreateWirelessGatewayRequestRequestTypeDef,
 ):
     pass
 
 
+LoRaWANGatewayUnionTypeDef = Union[LoRaWANGatewayTypeDef, LoRaWANGatewayOutputTypeDef]
 WirelessDeviceStatisticsTypeDef = TypedDict(
     "WirelessDeviceStatisticsTypeDef",
     {
         "Arn": str,
         "Id": str,
         "Type": WirelessDeviceTypeType,
         "Name": str,
@@ -3371,14 +3356,46 @@
     {
         "FPort": int,
         "ParticipatingGateways": ParticipatingGatewaysTypeDef,
     },
     total=False,
 )
 
+LoRaWANMulticastSessionUnionTypeDef = Union[
+    LoRaWANMulticastSessionTypeDef, LoRaWANMulticastSessionOutputTypeDef
+]
+StartMulticastGroupSessionRequestRequestTypeDef = TypedDict(
+    "StartMulticastGroupSessionRequestRequestTypeDef",
+    {
+        "Id": str,
+        "LoRaWAN": LoRaWANMulticastSessionTypeDef,
+    },
+)
+
+_RequiredStartFuotaTaskRequestRequestTypeDef = TypedDict(
+    "_RequiredStartFuotaTaskRequestRequestTypeDef",
+    {
+        "Id": str,
+    },
+)
+_OptionalStartFuotaTaskRequestRequestTypeDef = TypedDict(
+    "_OptionalStartFuotaTaskRequestRequestTypeDef",
+    {
+        "LoRaWAN": LoRaWANStartFuotaTaskTypeDef,
+    },
+    total=False,
+)
+
+
+class StartFuotaTaskRequestRequestTypeDef(
+    _RequiredStartFuotaTaskRequestRequestTypeDef, _OptionalStartFuotaTaskRequestRequestTypeDef
+):
+    pass
+
+
 ListWirelessDeviceImportTasksResponseTypeDef = TypedDict(
     "ListWirelessDeviceImportTasksResponseTypeDef",
     {
         "NextToken": str,
         "WirelessDeviceImportTaskList": List[WirelessDeviceImportTaskTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -3583,38 +3600,30 @@
         "ResourceType": PositionResourceTypeType,
         "Solvers": PositionSolverDetailsTypeDef,
         "Destination": str,
     },
     total=False,
 )
 
+WirelessDeviceLogOptionUnionTypeDef = Union[
+    WirelessDeviceLogOptionTypeDef, WirelessDeviceLogOptionOutputTypeDef
+]
 GetLogLevelsByResourceTypesResponseTypeDef = TypedDict(
     "GetLogLevelsByResourceTypesResponseTypeDef",
     {
         "DefaultLogLevel": LogLevelType,
         "WirelessGatewayLogOptions": List[WirelessGatewayLogOptionOutputTypeDef],
         "WirelessDeviceLogOptions": List[WirelessDeviceLogOptionOutputTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateLogLevelsByResourceTypesRequestRequestTypeDef = TypedDict(
-    "UpdateLogLevelsByResourceTypesRequestRequestTypeDef",
-    {
-        "DefaultLogLevel": LogLevelType,
-        "WirelessDeviceLogOptions": Sequence[
-            Union[WirelessDeviceLogOptionTypeDef, WirelessDeviceLogOptionOutputTypeDef]
-        ],
-        "WirelessGatewayLogOptions": Sequence[
-            Union[WirelessGatewayLogOptionTypeDef, WirelessGatewayLogOptionOutputTypeDef]
-        ],
-    },
-    total=False,
-)
-
+WirelessGatewayLogOptionUnionTypeDef = Union[
+    WirelessGatewayLogOptionTypeDef, WirelessGatewayLogOptionOutputTypeDef
+]
 ListWirelessGatewaysResponseTypeDef = TypedDict(
     "ListWirelessGatewaysResponseTypeDef",
     {
         "NextToken": str,
         "WirelessGatewayList": List[WirelessGatewayStatisticsTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -3672,14 +3681,15 @@
 class CreateWirelessDeviceRequestRequestTypeDef(
     _RequiredCreateWirelessDeviceRequestRequestTypeDef,
     _OptionalCreateWirelessDeviceRequestRequestTypeDef,
 ):
     pass
 
 
+LoRaWANDeviceUnionTypeDef = Union[LoRaWANDeviceTypeDef, LoRaWANDeviceOutputTypeDef]
 _RequiredUpdateWirelessDeviceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateWirelessDeviceRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalUpdateWirelessDeviceRequestRequestTypeDef = TypedDict(
@@ -3795,14 +3805,24 @@
     {
         "PositionConfigurationList": List[PositionConfigurationItemTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+UpdateLogLevelsByResourceTypesRequestRequestTypeDef = TypedDict(
+    "UpdateLogLevelsByResourceTypesRequestRequestTypeDef",
+    {
+        "DefaultLogLevel": LogLevelType,
+        "WirelessDeviceLogOptions": Sequence[WirelessDeviceLogOptionUnionTypeDef],
+        "WirelessGatewayLogOptions": Sequence[WirelessGatewayLogOptionUnionTypeDef],
+    },
+    total=False,
+)
+
 ListQueuedMessagesResponseTypeDef = TypedDict(
     "ListQueuedMessagesResponseTypeDef",
     {
         "NextToken": str,
         "DownlinkQueueMessagesList": List[DownlinkQueueMessageTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -3835,15 +3855,15 @@
 GetPositionEstimateRequestRequestTypeDef = TypedDict(
     "GetPositionEstimateRequestRequestTypeDef",
     {
         "WiFiAccessPoints": Sequence[WiFiAccessPointTypeDef],
         "CellTowers": CellTowersTypeDef,
         "Ip": IpTypeDef,
         "Gnss": GnssTypeDef,
-        "Timestamp": Union[datetime, str],
+        "Timestamp": TimestampTypeDef,
     },
     total=False,
 )
 
 ListEventConfigurationsResponseTypeDef = TypedDict(
     "ListEventConfigurationsResponseTypeDef",
     {
```

### Comparing `mypy-boto3-iotwireless-1.28.15.post1/mypy_boto3_iotwireless/type_defs.pyi` & `mypy-boto3-iotwireless-1.28.16/mypy_boto3_iotwireless/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_iotwireless.type_defs import SessionKeysAbpV10XTypeDef
 
-    data: SessionKeysAbpV10XTypeDef = {...}
+    data: SessionKeysAbpV10XTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -74,14 +74,15 @@
     "AssociateWirelessDeviceWithFuotaTaskRequestRequestTypeDef",
     "AssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef",
     "AssociateWirelessDeviceWithThingRequestRequestTypeDef",
     "AssociateWirelessGatewayWithCertificateRequestRequestTypeDef",
     "AssociateWirelessGatewayWithThingRequestRequestTypeDef",
     "BeaconingOutputTypeDef",
     "BeaconingTypeDef",
+    "BlobTypeDef",
     "CancelMulticastGroupSessionRequestRequestTypeDef",
     "CdmaLocalIdTypeDef",
     "CdmaNmrObjTypeDef",
     "CertificateListTypeDef",
     "LoRaWANConnectionStatusEventNotificationConfigurationsTypeDef",
     "LoRaWANConnectionStatusResourceTypeEventConfigurationTypeDef",
     "LoRaWANDeviceProfileTypeDef",
@@ -130,14 +131,15 @@
     "LoRaWANMulticastSessionOutputTypeDef",
     "GetNetworkAnalyzerConfigurationRequestRequestTypeDef",
     "GetPartnerAccountRequestRequestTypeDef",
     "SidewalkAccountInfoWithFingerprintTypeDef",
     "GetPositionConfigurationRequestRequestTypeDef",
     "GnssTypeDef",
     "IpTypeDef",
+    "TimestampTypeDef",
     "WiFiAccessPointTypeDef",
     "GetPositionRequestRequestTypeDef",
     "GetResourceEventConfigurationRequestRequestTypeDef",
     "GetResourceLogLevelRequestRequestTypeDef",
     "GetResourcePositionRequestRequestTypeDef",
     "GetServiceEndpointRequestRequestTypeDef",
     "GetServiceProfileRequestRequestTypeDef",
@@ -181,16 +183,14 @@
     "ListWirelessGatewaysRequestRequestTypeDef",
     "LoRaWANGatewayMetadataTypeDef",
     "OtaaV10XTypeDef",
     "OtaaV11TypeDef",
     "LoRaWANGatewayVersionTypeDef",
     "LoRaWANListDeviceTypeDef",
     "LoRaWANMulticastMetadataTypeDef",
-    "LoRaWANMulticastSessionTypeDef",
-    "LoRaWANStartFuotaTaskTypeDef",
     "UpdateAbpV10XTypeDef",
     "UpdateAbpV11TypeDef",
     "LteLocalIdTypeDef",
     "LteNmrObjTypeDef",
     "SemtechGnssConfigurationTypeDef",
     "SemtechGnssDetailTypeDef",
     "PutResourceLogLevelRequestRequestTypeDef",
@@ -202,15 +202,14 @@
     "SidewalkUpdateImportInfoTypeDef",
     "TdscdmaLocalIdTypeDef",
     "TdscdmaNmrObjTypeDef",
     "TestWirelessDeviceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDestinationRequestRequestTypeDef",
     "UpdatePositionRequestRequestTypeDef",
-    "UpdateResourcePositionRequestRequestTypeDef",
     "UpdateWirelessGatewayRequestRequestTypeDef",
     "WcdmaLocalIdTypeDef",
     "WcdmaNmrObjTypeDef",
     "WirelessDeviceEventLogOptionTypeDef",
     "WirelessGatewayEventLogOptionTypeDef",
     "AbpV10XTypeDef",
     "AbpV11TypeDef",
@@ -244,14 +243,15 @@
     "SendDataToMulticastGroupResponseTypeDef",
     "SendDataToWirelessDeviceResponseTypeDef",
     "StartSingleWirelessDeviceImportTaskResponseTypeDef",
     "StartWirelessDeviceImportTaskResponseTypeDef",
     "TestWirelessDeviceResponseTypeDef",
     "LoRaWANGatewayOutputTypeDef",
     "LoRaWANGatewayTypeDef",
+    "UpdateResourcePositionRequestRequestTypeDef",
     "CdmaObjTypeDef",
     "SidewalkDeviceTypeDef",
     "SidewalkListDeviceTypeDef",
     "ConnectionStatusEventConfigurationTypeDef",
     "ConnectionStatusResourceTypeEventConfigurationTypeDef",
     "CreateDeviceProfileRequestRequestTypeDef",
     "CreateFuotaTaskRequestRequestTypeDef",
@@ -273,19 +273,22 @@
     "ProximityResourceTypeEventConfigurationTypeDef",
     "FPortsOutputTypeDef",
     "FPortsTypeDef",
     "UpdateFPortsTypeDef",
     "ListFuotaTasksResponseTypeDef",
     "ParticipatingGatewaysOutputTypeDef",
     "ParticipatingGatewaysTypeDef",
+    "LoRaWANDeviceProfileUnionTypeDef",
     "GetFuotaTaskResponseTypeDef",
     "GetMulticastGroupResponseTypeDef",
     "GetMulticastGroupSessionResponseTypeDef",
     "GetPartnerAccountResponseTypeDef",
     "ListPartnerAccountsResponseTypeDef",
+    "LoRaWANMulticastSessionTypeDef",
+    "LoRaWANStartFuotaTaskTypeDef",
     "GetServiceProfileResponseTypeDef",
     "GetWirelessDeviceImportTaskResponseTypeDef",
     "WirelessDeviceImportTaskTypeDef",
     "GsmNmrObjTypeDef",
     "ImportedWirelessDeviceTypeDef",
     "JoinEventConfigurationTypeDef",
     "JoinResourceTypeEventConfigurationTypeDef",
@@ -294,16 +297,14 @@
     "ListNetworkAnalyzerConfigurationsResponseTypeDef",
     "ListServiceProfilesResponseTypeDef",
     "LoRaWANDeviceMetadataTypeDef",
     "LoRaWANGatewayCurrentVersionTypeDef",
     "LoRaWANUpdateGatewayTaskCreateTypeDef",
     "LoRaWANUpdateGatewayTaskEntryTypeDef",
     "MulticastWirelessMetadataTypeDef",
-    "StartMulticastGroupSessionRequestRequestTypeDef",
-    "StartFuotaTaskRequestRequestTypeDef",
     "LteObjTypeDef",
     "PositionSolverConfigurationsTypeDef",
     "PositionSolverDetailsTypeDef",
     "StartSingleWirelessDeviceImportTaskRequestRequestTypeDef",
     "StartWirelessDeviceImportTaskRequestRequestTypeDef",
     "UpdatePartnerAccountRequestRequestTypeDef",
     "UpdateWirelessDeviceImportTaskRequestRequestTypeDef",
@@ -312,21 +313,25 @@
     "WirelessDeviceLogOptionOutputTypeDef",
     "WirelessDeviceLogOptionTypeDef",
     "WirelessGatewayLogOptionOutputTypeDef",
     "WirelessGatewayLogOptionTypeDef",
     "GetWirelessGatewayResponseTypeDef",
     "WirelessGatewayStatisticsTypeDef",
     "CreateWirelessGatewayRequestRequestTypeDef",
+    "LoRaWANGatewayUnionTypeDef",
     "WirelessDeviceStatisticsTypeDef",
     "GetDeviceProfileResponseTypeDef",
     "LoRaWANDeviceOutputTypeDef",
     "LoRaWANDeviceTypeDef",
     "LoRaWANUpdateDeviceTypeDef",
     "LoRaWANSendDataToDeviceOutputTypeDef",
     "LoRaWANSendDataToDeviceTypeDef",
+    "LoRaWANMulticastSessionUnionTypeDef",
+    "StartMulticastGroupSessionRequestRequestTypeDef",
+    "StartFuotaTaskRequestRequestTypeDef",
     "ListWirelessDeviceImportTasksResponseTypeDef",
     "GsmObjTypeDef",
     "ListDevicesForWirelessDeviceImportTaskResponseTypeDef",
     "EventNotificationItemConfigurationsTypeDef",
     "GetResourceEventConfigurationResponseTypeDef",
     "UpdateResourceEventConfigurationRequestRequestTypeDef",
     "GetEventConfigurationByResourceTypesResponseTypeDef",
@@ -335,29 +340,32 @@
     "GetWirelessGatewayFirmwareInformationResponseTypeDef",
     "UpdateWirelessGatewayTaskCreateTypeDef",
     "UpdateWirelessGatewayTaskEntryTypeDef",
     "SendDataToMulticastGroupRequestRequestTypeDef",
     "PutPositionConfigurationRequestRequestTypeDef",
     "GetPositionConfigurationResponseTypeDef",
     "PositionConfigurationItemTypeDef",
+    "WirelessDeviceLogOptionUnionTypeDef",
     "GetLogLevelsByResourceTypesResponseTypeDef",
-    "UpdateLogLevelsByResourceTypesRequestRequestTypeDef",
+    "WirelessGatewayLogOptionUnionTypeDef",
     "ListWirelessGatewaysResponseTypeDef",
     "ListWirelessDevicesResponseTypeDef",
     "GetWirelessDeviceResponseTypeDef",
     "CreateWirelessDeviceRequestRequestTypeDef",
+    "LoRaWANDeviceUnionTypeDef",
     "UpdateWirelessDeviceRequestRequestTypeDef",
     "DownlinkQueueMessageTypeDef",
     "WirelessMetadataTypeDef",
     "CellTowersTypeDef",
     "EventConfigurationItemTypeDef",
     "CreateWirelessGatewayTaskDefinitionRequestRequestTypeDef",
     "GetWirelessGatewayTaskDefinitionResponseTypeDef",
     "ListWirelessGatewayTaskDefinitionsResponseTypeDef",
     "ListPositionConfigurationsResponseTypeDef",
+    "UpdateLogLevelsByResourceTypesRequestRequestTypeDef",
     "ListQueuedMessagesResponseTypeDef",
     "SendDataToWirelessDeviceRequestRequestTypeDef",
     "GetPositionEstimateRequestRequestTypeDef",
     "ListEventConfigurationsResponseTypeDef",
 )
 
 SessionKeysAbpV10XTypeDef = TypedDict(
@@ -489,14 +497,15 @@
     {
         "DataRate": int,
         "Frequencies": Sequence[int],
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CancelMulticastGroupSessionRequestRequestTypeDef = TypedDict(
     "CancelMulticastGroupSessionRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -1042,14 +1051,15 @@
 IpTypeDef = TypedDict(
     "IpTypeDef",
     {
         "IpAddress": str,
     },
 )
 
+TimestampTypeDef = Union[datetime, str]
 WiFiAccessPointTypeDef = TypedDict(
     "WiFiAccessPointTypeDef",
     {
         "MacAddress": str,
         "Rss": int,
     },
 )
@@ -1567,34 +1577,14 @@
     "LoRaWANMulticastMetadataTypeDef",
     {
         "FPort": int,
     },
     total=False,
 )
 
-LoRaWANMulticastSessionTypeDef = TypedDict(
-    "LoRaWANMulticastSessionTypeDef",
-    {
-        "DlDr": int,
-        "DlFreq": int,
-        "SessionStartTime": Union[datetime, str],
-        "SessionTimeout": int,
-        "PingSlotPeriod": int,
-    },
-    total=False,
-)
-
-LoRaWANStartFuotaTaskTypeDef = TypedDict(
-    "LoRaWANStartFuotaTaskTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-    },
-    total=False,
-)
-
 UpdateAbpV10XTypeDef = TypedDict(
     "UpdateAbpV10XTypeDef",
     {
         "FCntStart": int,
     },
     total=False,
 )
@@ -1784,35 +1774,14 @@
     {
         "ResourceIdentifier": str,
         "ResourceType": PositionResourceTypeType,
         "Position": Sequence[float],
     },
 )
 
-_RequiredUpdateResourcePositionRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateResourcePositionRequestRequestTypeDef",
-    {
-        "ResourceIdentifier": str,
-        "ResourceType": PositionResourceTypeType,
-    },
-)
-_OptionalUpdateResourcePositionRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateResourcePositionRequestRequestTypeDef",
-    {
-        "GeoJsonPayload": Union[str, bytes, IO[Any], StreamingBody],
-    },
-    total=False,
-)
-
-class UpdateResourcePositionRequestRequestTypeDef(
-    _RequiredUpdateResourcePositionRequestRequestTypeDef,
-    _OptionalUpdateResourcePositionRequestRequestTypeDef,
-):
-    pass
-
 _RequiredUpdateWirelessGatewayRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateWirelessGatewayRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalUpdateWirelessGatewayRequestRequestTypeDef = TypedDict(
@@ -2264,14 +2233,35 @@
         "SubBands": Sequence[int],
         "Beaconing": BeaconingTypeDef,
         "MaxEirp": float,
     },
     total=False,
 )
 
+_RequiredUpdateResourcePositionRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateResourcePositionRequestRequestTypeDef",
+    {
+        "ResourceIdentifier": str,
+        "ResourceType": PositionResourceTypeType,
+    },
+)
+_OptionalUpdateResourcePositionRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateResourcePositionRequestRequestTypeDef",
+    {
+        "GeoJsonPayload": BlobTypeDef,
+    },
+    total=False,
+)
+
+class UpdateResourcePositionRequestRequestTypeDef(
+    _RequiredUpdateResourcePositionRequestRequestTypeDef,
+    _OptionalUpdateResourcePositionRequestRequestTypeDef,
+):
+    pass
+
 _RequiredCdmaObjTypeDef = TypedDict(
     "_RequiredCdmaObjTypeDef",
     {
         "SystemId": int,
         "NetworkId": int,
         "BaseStationId": int,
     },
@@ -2660,14 +2650,17 @@
     {
         "DownlinkMode": DownlinkModeType,
         "GatewayList": Sequence[GatewayListItemTypeDef],
         "TransmissionInterval": int,
     },
 )
 
+LoRaWANDeviceProfileUnionTypeDef = Union[
+    LoRaWANDeviceProfileTypeDef, LoRaWANDeviceProfileOutputTypeDef
+]
 GetFuotaTaskResponseTypeDef = TypedDict(
     "GetFuotaTaskResponseTypeDef",
     {
         "Arn": str,
         "Id": str,
         "Status": FuotaTaskStatusType,
         "Name": str,
@@ -2719,14 +2712,34 @@
     {
         "NextToken": str,
         "Sidewalk": List[SidewalkAccountInfoWithFingerprintTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+LoRaWANMulticastSessionTypeDef = TypedDict(
+    "LoRaWANMulticastSessionTypeDef",
+    {
+        "DlDr": int,
+        "DlFreq": int,
+        "SessionStartTime": TimestampTypeDef,
+        "SessionTimeout": int,
+        "PingSlotPeriod": int,
+    },
+    total=False,
+)
+
+LoRaWANStartFuotaTaskTypeDef = TypedDict(
+    "LoRaWANStartFuotaTaskTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+    },
+    total=False,
+)
+
 GetServiceProfileResponseTypeDef = TypedDict(
     "GetServiceProfileResponseTypeDef",
     {
         "Arn": str,
         "Name": str,
         "Id": str,
         "LoRaWAN": LoRaWANGetServiceProfileInfoTypeDef,
@@ -2895,41 +2908,14 @@
     "MulticastWirelessMetadataTypeDef",
     {
         "LoRaWAN": LoRaWANMulticastMetadataTypeDef,
     },
     total=False,
 )
 
-StartMulticastGroupSessionRequestRequestTypeDef = TypedDict(
-    "StartMulticastGroupSessionRequestRequestTypeDef",
-    {
-        "Id": str,
-        "LoRaWAN": LoRaWANMulticastSessionTypeDef,
-    },
-)
-
-_RequiredStartFuotaTaskRequestRequestTypeDef = TypedDict(
-    "_RequiredStartFuotaTaskRequestRequestTypeDef",
-    {
-        "Id": str,
-    },
-)
-_OptionalStartFuotaTaskRequestRequestTypeDef = TypedDict(
-    "_OptionalStartFuotaTaskRequestRequestTypeDef",
-    {
-        "LoRaWAN": LoRaWANStartFuotaTaskTypeDef,
-    },
-    total=False,
-)
-
-class StartFuotaTaskRequestRequestTypeDef(
-    _RequiredStartFuotaTaskRequestRequestTypeDef, _OptionalStartFuotaTaskRequestRequestTypeDef
-):
-    pass
-
 _RequiredLteObjTypeDef = TypedDict(
     "_RequiredLteObjTypeDef",
     {
         "Mcc": int,
         "Mnc": int,
         "EutranCid": int,
     },
@@ -3202,14 +3188,15 @@
 
 class CreateWirelessGatewayRequestRequestTypeDef(
     _RequiredCreateWirelessGatewayRequestRequestTypeDef,
     _OptionalCreateWirelessGatewayRequestRequestTypeDef,
 ):
     pass
 
+LoRaWANGatewayUnionTypeDef = Union[LoRaWANGatewayTypeDef, LoRaWANGatewayOutputTypeDef]
 WirelessDeviceStatisticsTypeDef = TypedDict(
     "WirelessDeviceStatisticsTypeDef",
     {
         "Arn": str,
         "Id": str,
         "Type": WirelessDeviceTypeType,
         "Name": str,
@@ -3292,14 +3279,44 @@
     {
         "FPort": int,
         "ParticipatingGateways": ParticipatingGatewaysTypeDef,
     },
     total=False,
 )
 
+LoRaWANMulticastSessionUnionTypeDef = Union[
+    LoRaWANMulticastSessionTypeDef, LoRaWANMulticastSessionOutputTypeDef
+]
+StartMulticastGroupSessionRequestRequestTypeDef = TypedDict(
+    "StartMulticastGroupSessionRequestRequestTypeDef",
+    {
+        "Id": str,
+        "LoRaWAN": LoRaWANMulticastSessionTypeDef,
+    },
+)
+
+_RequiredStartFuotaTaskRequestRequestTypeDef = TypedDict(
+    "_RequiredStartFuotaTaskRequestRequestTypeDef",
+    {
+        "Id": str,
+    },
+)
+_OptionalStartFuotaTaskRequestRequestTypeDef = TypedDict(
+    "_OptionalStartFuotaTaskRequestRequestTypeDef",
+    {
+        "LoRaWAN": LoRaWANStartFuotaTaskTypeDef,
+    },
+    total=False,
+)
+
+class StartFuotaTaskRequestRequestTypeDef(
+    _RequiredStartFuotaTaskRequestRequestTypeDef, _OptionalStartFuotaTaskRequestRequestTypeDef
+):
+    pass
+
 ListWirelessDeviceImportTasksResponseTypeDef = TypedDict(
     "ListWirelessDeviceImportTasksResponseTypeDef",
     {
         "NextToken": str,
         "WirelessDeviceImportTaskList": List[WirelessDeviceImportTaskTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -3498,38 +3515,30 @@
         "ResourceType": PositionResourceTypeType,
         "Solvers": PositionSolverDetailsTypeDef,
         "Destination": str,
     },
     total=False,
 )
 
+WirelessDeviceLogOptionUnionTypeDef = Union[
+    WirelessDeviceLogOptionTypeDef, WirelessDeviceLogOptionOutputTypeDef
+]
 GetLogLevelsByResourceTypesResponseTypeDef = TypedDict(
     "GetLogLevelsByResourceTypesResponseTypeDef",
     {
         "DefaultLogLevel": LogLevelType,
         "WirelessGatewayLogOptions": List[WirelessGatewayLogOptionOutputTypeDef],
         "WirelessDeviceLogOptions": List[WirelessDeviceLogOptionOutputTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateLogLevelsByResourceTypesRequestRequestTypeDef = TypedDict(
-    "UpdateLogLevelsByResourceTypesRequestRequestTypeDef",
-    {
-        "DefaultLogLevel": LogLevelType,
-        "WirelessDeviceLogOptions": Sequence[
-            Union[WirelessDeviceLogOptionTypeDef, WirelessDeviceLogOptionOutputTypeDef]
-        ],
-        "WirelessGatewayLogOptions": Sequence[
-            Union[WirelessGatewayLogOptionTypeDef, WirelessGatewayLogOptionOutputTypeDef]
-        ],
-    },
-    total=False,
-)
-
+WirelessGatewayLogOptionUnionTypeDef = Union[
+    WirelessGatewayLogOptionTypeDef, WirelessGatewayLogOptionOutputTypeDef
+]
 ListWirelessGatewaysResponseTypeDef = TypedDict(
     "ListWirelessGatewaysResponseTypeDef",
     {
         "NextToken": str,
         "WirelessGatewayList": List[WirelessGatewayStatisticsTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -3585,14 +3594,15 @@
 
 class CreateWirelessDeviceRequestRequestTypeDef(
     _RequiredCreateWirelessDeviceRequestRequestTypeDef,
     _OptionalCreateWirelessDeviceRequestRequestTypeDef,
 ):
     pass
 
+LoRaWANDeviceUnionTypeDef = Union[LoRaWANDeviceTypeDef, LoRaWANDeviceOutputTypeDef]
 _RequiredUpdateWirelessDeviceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateWirelessDeviceRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalUpdateWirelessDeviceRequestRequestTypeDef = TypedDict(
@@ -3704,14 +3714,24 @@
     {
         "PositionConfigurationList": List[PositionConfigurationItemTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+UpdateLogLevelsByResourceTypesRequestRequestTypeDef = TypedDict(
+    "UpdateLogLevelsByResourceTypesRequestRequestTypeDef",
+    {
+        "DefaultLogLevel": LogLevelType,
+        "WirelessDeviceLogOptions": Sequence[WirelessDeviceLogOptionUnionTypeDef],
+        "WirelessGatewayLogOptions": Sequence[WirelessGatewayLogOptionUnionTypeDef],
+    },
+    total=False,
+)
+
 ListQueuedMessagesResponseTypeDef = TypedDict(
     "ListQueuedMessagesResponseTypeDef",
     {
         "NextToken": str,
         "DownlinkQueueMessagesList": List[DownlinkQueueMessageTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -3742,15 +3762,15 @@
 GetPositionEstimateRequestRequestTypeDef = TypedDict(
     "GetPositionEstimateRequestRequestTypeDef",
     {
         "WiFiAccessPoints": Sequence[WiFiAccessPointTypeDef],
         "CellTowers": CellTowersTypeDef,
         "Ip": IpTypeDef,
         "Gnss": GnssTypeDef,
-        "Timestamp": Union[datetime, str],
+        "Timestamp": TimestampTypeDef,
     },
     total=False,
 )
 
 ListEventConfigurationsResponseTypeDef = TypedDict(
     "ListEventConfigurationsResponseTypeDef",
     {
```

### Comparing `mypy-boto3-iotwireless-1.28.15.post1/mypy_boto3_iotwireless.egg-info/PKG-INFO` & `mypy-boto3-iotwireless-1.28.16/mypy_boto3_iotwireless.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotwireless
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.IoTWireless 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.IoTWireless 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 iotwireless type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 iotwireless type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotwireless.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotwireless)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotwireless)](https://pepy.tech/project/mypy-boto3-iotwireless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTWireless 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless)
+[boto3.IoTWireless 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless)
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
 [mypy-boto3-iotwireless docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/).
 
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
@@ -326,20 +326,20 @@
 )
 
 
 def check_value(value: ApplicationConfigTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_iotwireless.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_iotwireless.type_defs import (
     SessionKeysAbpV10XTypeDef,
     SessionKeysAbpV11TypeDef,
     AccuracyTypeDef,
     ApplicationConfigTypeDef,
@@ -350,14 +350,15 @@
     AssociateWirelessDeviceWithFuotaTaskRequestRequestTypeDef,
     AssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef,
     AssociateWirelessDeviceWithThingRequestRequestTypeDef,
     AssociateWirelessGatewayWithCertificateRequestRequestTypeDef,
     AssociateWirelessGatewayWithThingRequestRequestTypeDef,
     BeaconingOutputTypeDef,
     BeaconingTypeDef,
+    BlobTypeDef,
     CancelMulticastGroupSessionRequestRequestTypeDef,
     CdmaLocalIdTypeDef,
     CdmaNmrObjTypeDef,
     CertificateListTypeDef,
     LoRaWANConnectionStatusEventNotificationConfigurationsTypeDef,
     LoRaWANConnectionStatusResourceTypeEventConfigurationTypeDef,
     LoRaWANDeviceProfileTypeDef,
@@ -406,14 +407,15 @@
     LoRaWANMulticastSessionOutputTypeDef,
     GetNetworkAnalyzerConfigurationRequestRequestTypeDef,
     GetPartnerAccountRequestRequestTypeDef,
     SidewalkAccountInfoWithFingerprintTypeDef,
     GetPositionConfigurationRequestRequestTypeDef,
     GnssTypeDef,
     IpTypeDef,
+    TimestampTypeDef,
     WiFiAccessPointTypeDef,
     GetPositionRequestRequestTypeDef,
     GetResourceEventConfigurationRequestRequestTypeDef,
     GetResourceLogLevelRequestRequestTypeDef,
     GetResourcePositionRequestRequestTypeDef,
     GetServiceEndpointRequestRequestTypeDef,
     GetServiceProfileRequestRequestTypeDef,
@@ -457,16 +459,14 @@
     ListWirelessGatewaysRequestRequestTypeDef,
     LoRaWANGatewayMetadataTypeDef,
     OtaaV10XTypeDef,
     OtaaV11TypeDef,
     LoRaWANGatewayVersionTypeDef,
     LoRaWANListDeviceTypeDef,
     LoRaWANMulticastMetadataTypeDef,
-    LoRaWANMulticastSessionTypeDef,
-    LoRaWANStartFuotaTaskTypeDef,
     UpdateAbpV10XTypeDef,
     UpdateAbpV11TypeDef,
     LteLocalIdTypeDef,
     LteNmrObjTypeDef,
     SemtechGnssConfigurationTypeDef,
     SemtechGnssDetailTypeDef,
     PutResourceLogLevelRequestRequestTypeDef,
@@ -478,15 +478,14 @@
     SidewalkUpdateImportInfoTypeDef,
     TdscdmaLocalIdTypeDef,
     TdscdmaNmrObjTypeDef,
     TestWirelessDeviceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDestinationRequestRequestTypeDef,
     UpdatePositionRequestRequestTypeDef,
-    UpdateResourcePositionRequestRequestTypeDef,
     UpdateWirelessGatewayRequestRequestTypeDef,
     WcdmaLocalIdTypeDef,
     WcdmaNmrObjTypeDef,
     WirelessDeviceEventLogOptionTypeDef,
     WirelessGatewayEventLogOptionTypeDef,
     AbpV10XTypeDef,
     AbpV11TypeDef,
@@ -520,14 +519,15 @@
     SendDataToMulticastGroupResponseTypeDef,
     SendDataToWirelessDeviceResponseTypeDef,
     StartSingleWirelessDeviceImportTaskResponseTypeDef,
     StartWirelessDeviceImportTaskResponseTypeDef,
     TestWirelessDeviceResponseTypeDef,
     LoRaWANGatewayOutputTypeDef,
     LoRaWANGatewayTypeDef,
+    UpdateResourcePositionRequestRequestTypeDef,
     CdmaObjTypeDef,
     SidewalkDeviceTypeDef,
     SidewalkListDeviceTypeDef,
     ConnectionStatusEventConfigurationTypeDef,
     ConnectionStatusResourceTypeEventConfigurationTypeDef,
     CreateDeviceProfileRequestRequestTypeDef,
     CreateFuotaTaskRequestRequestTypeDef,
@@ -549,19 +549,22 @@
     ProximityResourceTypeEventConfigurationTypeDef,
     FPortsOutputTypeDef,
     FPortsTypeDef,
     UpdateFPortsTypeDef,
     ListFuotaTasksResponseTypeDef,
     ParticipatingGatewaysOutputTypeDef,
     ParticipatingGatewaysTypeDef,
+    LoRaWANDeviceProfileUnionTypeDef,
     GetFuotaTaskResponseTypeDef,
     GetMulticastGroupResponseTypeDef,
     GetMulticastGroupSessionResponseTypeDef,
     GetPartnerAccountResponseTypeDef,
     ListPartnerAccountsResponseTypeDef,
+    LoRaWANMulticastSessionTypeDef,
+    LoRaWANStartFuotaTaskTypeDef,
     GetServiceProfileResponseTypeDef,
     GetWirelessDeviceImportTaskResponseTypeDef,
     WirelessDeviceImportTaskTypeDef,
     GsmNmrObjTypeDef,
     ImportedWirelessDeviceTypeDef,
     JoinEventConfigurationTypeDef,
     JoinResourceTypeEventConfigurationTypeDef,
@@ -570,16 +573,14 @@
     ListNetworkAnalyzerConfigurationsResponseTypeDef,
     ListServiceProfilesResponseTypeDef,
     LoRaWANDeviceMetadataTypeDef,
     LoRaWANGatewayCurrentVersionTypeDef,
     LoRaWANUpdateGatewayTaskCreateTypeDef,
     LoRaWANUpdateGatewayTaskEntryTypeDef,
     MulticastWirelessMetadataTypeDef,
-    StartMulticastGroupSessionRequestRequestTypeDef,
-    StartFuotaTaskRequestRequestTypeDef,
     LteObjTypeDef,
     PositionSolverConfigurationsTypeDef,
     PositionSolverDetailsTypeDef,
     StartSingleWirelessDeviceImportTaskRequestRequestTypeDef,
     StartWirelessDeviceImportTaskRequestRequestTypeDef,
     UpdatePartnerAccountRequestRequestTypeDef,
     UpdateWirelessDeviceImportTaskRequestRequestTypeDef,
@@ -588,21 +589,25 @@
     WirelessDeviceLogOptionOutputTypeDef,
     WirelessDeviceLogOptionTypeDef,
     WirelessGatewayLogOptionOutputTypeDef,
     WirelessGatewayLogOptionTypeDef,
     GetWirelessGatewayResponseTypeDef,
     WirelessGatewayStatisticsTypeDef,
     CreateWirelessGatewayRequestRequestTypeDef,
+    LoRaWANGatewayUnionTypeDef,
     WirelessDeviceStatisticsTypeDef,
     GetDeviceProfileResponseTypeDef,
     LoRaWANDeviceOutputTypeDef,
     LoRaWANDeviceTypeDef,
     LoRaWANUpdateDeviceTypeDef,
     LoRaWANSendDataToDeviceOutputTypeDef,
     LoRaWANSendDataToDeviceTypeDef,
+    LoRaWANMulticastSessionUnionTypeDef,
+    StartMulticastGroupSessionRequestRequestTypeDef,
+    StartFuotaTaskRequestRequestTypeDef,
     ListWirelessDeviceImportTasksResponseTypeDef,
     GsmObjTypeDef,
     ListDevicesForWirelessDeviceImportTaskResponseTypeDef,
     EventNotificationItemConfigurationsTypeDef,
     GetResourceEventConfigurationResponseTypeDef,
     UpdateResourceEventConfigurationRequestRequestTypeDef,
     GetEventConfigurationByResourceTypesResponseTypeDef,
@@ -611,37 +616,40 @@
     GetWirelessGatewayFirmwareInformationResponseTypeDef,
     UpdateWirelessGatewayTaskCreateTypeDef,
     UpdateWirelessGatewayTaskEntryTypeDef,
     SendDataToMulticastGroupRequestRequestTypeDef,
     PutPositionConfigurationRequestRequestTypeDef,
     GetPositionConfigurationResponseTypeDef,
     PositionConfigurationItemTypeDef,
+    WirelessDeviceLogOptionUnionTypeDef,
     GetLogLevelsByResourceTypesResponseTypeDef,
-    UpdateLogLevelsByResourceTypesRequestRequestTypeDef,
+    WirelessGatewayLogOptionUnionTypeDef,
     ListWirelessGatewaysResponseTypeDef,
     ListWirelessDevicesResponseTypeDef,
     GetWirelessDeviceResponseTypeDef,
     CreateWirelessDeviceRequestRequestTypeDef,
+    LoRaWANDeviceUnionTypeDef,
     UpdateWirelessDeviceRequestRequestTypeDef,
     DownlinkQueueMessageTypeDef,
     WirelessMetadataTypeDef,
     CellTowersTypeDef,
     EventConfigurationItemTypeDef,
     CreateWirelessGatewayTaskDefinitionRequestRequestTypeDef,
     GetWirelessGatewayTaskDefinitionResponseTypeDef,
     ListWirelessGatewayTaskDefinitionsResponseTypeDef,
     ListPositionConfigurationsResponseTypeDef,
+    UpdateLogLevelsByResourceTypesRequestRequestTypeDef,
     ListQueuedMessagesResponseTypeDef,
     SendDataToWirelessDeviceRequestRequestTypeDef,
     GetPositionEstimateRequestRequestTypeDef,
     ListEventConfigurationsResponseTypeDef,
 )
 
 
-def get_structure() -> SessionKeysAbpV10XTypeDef:
+def get_value() -> SessionKeysAbpV10XTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iotwireless-1.28.15.post1/mypy_boto3_iotwireless.egg-info/SOURCES.txt` & `mypy-boto3-iotwireless-1.28.16/mypy_boto3_iotwireless.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotwireless-1.28.15.post1/setup.py` & `mypy-boto3-iotwireless-1.28.16/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-iotwireless",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_iotwireless"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IoTWireless 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.IoTWireless 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 iotwireless type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 iotwireless type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_iotwireless": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

