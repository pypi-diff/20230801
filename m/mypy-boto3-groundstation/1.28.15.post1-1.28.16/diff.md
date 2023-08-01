# Comparing `tmp/mypy-boto3-groundstation-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-groundstation-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-groundstation-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:13 2023, max compression
+gzip compressed data, was "mypy-boto3-groundstation-1.28.16.tar", last modified: Tue Aug  1 11:36:53 2023, max compression
```

## Comparing `mypy-boto3-groundstation-1.28.15.post1.tar` & `mypy-boto3-groundstation-1.28.16.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:13.561169 mypy-boto3-groundstation-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:46:41.000000 mypy-boto3-groundstation-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19327 2023-07-29 10:03:13.561169 mypy-boto3-groundstation-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17810 2023-07-29 09:46:41.000000 mypy-boto3-groundstation-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:13.553169 mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation/
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-29 09:46:41.000000 mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-29 09:46:41.000000 mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-29 09:46:41.000000 mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26919 2023-07-29 09:46:41.000000 mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    26871 2023-07-29 09:46:41.000000 mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10977 2023-07-29 09:46:41.000000 mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10975 2023-07-29 09:46:41.000000 mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8978 2023-07-29 09:46:41.000000 mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-07-29 09:46:41.000000 mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:46:41.000000 mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    40832 2023-07-29 09:46:44.000000 mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    40783 2023-07-29 09:46:42.000000 mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:46:41.000000 mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-29 09:46:41.000000 mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-29 09:46:41.000000 mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:13.561169 mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19327 2023-07-29 10:03:13.000000 mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-29 10:03:13.000000 mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:13.000000 mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:13.000000 mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:13.000000 mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-29 10:03:13.000000 mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:13.561169 mypy-boto3-groundstation-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-29 09:46:40.000000 mypy-boto3-groundstation-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:53.536879 mypy-boto3-groundstation-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:19:18.000000 mypy-boto3-groundstation-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19372 2023-08-01 11:36:53.536879 mypy-boto3-groundstation-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17864 2023-08-01 11:19:18.000000 mypy-boto3-groundstation-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:53.536879 mypy-boto3-groundstation-1.28.16/mypy_boto3_groundstation/
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-08-01 11:19:18.000000 mypy-boto3-groundstation-1.28.16/mypy_boto3_groundstation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-08-01 11:19:18.000000 mypy-boto3-groundstation-1.28.16/mypy_boto3_groundstation/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-08-01 11:19:18.000000 mypy-boto3-groundstation-1.28.16/mypy_boto3_groundstation/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26815 2023-08-01 11:19:20.000000 mypy-boto3-groundstation-1.28.16/mypy_boto3_groundstation/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26767 2023-08-01 11:19:20.000000 mypy-boto3-groundstation-1.28.16/mypy_boto3_groundstation/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10977 2023-08-01 11:19:21.000000 mypy-boto3-groundstation-1.28.16/mypy_boto3_groundstation/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10975 2023-08-01 11:19:21.000000 mypy-boto3-groundstation-1.28.16/mypy_boto3_groundstation/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-08-01 11:19:20.000000 mypy-boto3-groundstation-1.28.16/mypy_boto3_groundstation/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8938 2023-08-01 11:19:20.000000 mypy-boto3-groundstation-1.28.16/mypy_boto3_groundstation/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:19:18.000000 mypy-boto3-groundstation-1.28.16/mypy_boto3_groundstation/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    40935 2023-08-01 11:19:22.000000 mypy-boto3-groundstation-1.28.16/mypy_boto3_groundstation/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40886 2023-08-01 11:19:21.000000 mypy-boto3-groundstation-1.28.16/mypy_boto3_groundstation/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:19:18.000000 mypy-boto3-groundstation-1.28.16/mypy_boto3_groundstation/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-08-01 11:19:20.000000 mypy-boto3-groundstation-1.28.16/mypy_boto3_groundstation/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-08-01 11:19:20.000000 mypy-boto3-groundstation-1.28.16/mypy_boto3_groundstation/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:53.536879 mypy-boto3-groundstation-1.28.16/mypy_boto3_groundstation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19372 2023-08-01 11:36:53.000000 mypy-boto3-groundstation-1.28.16/mypy_boto3_groundstation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-08-01 11:36:53.000000 mypy-boto3-groundstation-1.28.16/mypy_boto3_groundstation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:53.000000 mypy-boto3-groundstation-1.28.16/mypy_boto3_groundstation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:53.000000 mypy-boto3-groundstation-1.28.16/mypy_boto3_groundstation.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:53.000000 mypy-boto3-groundstation-1.28.16/mypy_boto3_groundstation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-01 11:36:53.000000 mypy-boto3-groundstation-1.28.16/mypy_boto3_groundstation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:53.536879 mypy-boto3-groundstation-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-08-01 11:19:18.000000 mypy-boto3-groundstation-1.28.16/setup.py
```

### Comparing `mypy-boto3-groundstation-1.28.15.post1/LICENSE` & `mypy-boto3-groundstation-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-groundstation-1.28.15.post1/PKG-INFO` & `mypy-boto3-groundstation-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-groundstation
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.GroundStation 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.GroundStation 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 groundstation type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 groundstation type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-groundstation.svg?color=blue)](https://pypi.org/project/mypy-boto3-groundstation)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-groundstation)](https://pepy.tech/project/mypy-boto3-groundstation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GroundStation 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation)
+[boto3.GroundStation 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation)
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
 [mypy-boto3-groundstation docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/).
 
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
@@ -375,20 +375,20 @@
 )
 
 
 def check_value(value: AgentStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_groundstation.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_groundstation.type_defs import (
     ComponentVersionTypeDef,
     AggregateStatusTypeDef,
     AntennaDemodDecodeDetailsTypeDef,
     DecodeConfigTypeDef,
@@ -401,14 +401,15 @@
     ConfigListItemTypeDef,
     DataflowEndpointConfigTypeDef,
     S3RecordingConfigTypeDef,
     TrackingConfigTypeDef,
     UplinkEchoConfigTypeDef,
     SocketAddressTypeDef,
     ElevationTypeDef,
+    TimestampTypeDef,
     KmsKeyTypeDef,
     DataflowEndpointListItemTypeDef,
     DeleteConfigRequestRequestTypeDef,
     DeleteDataflowEndpointGroupRequestRequestTypeDef,
     DeleteEphemerisRequestRequestTypeDef,
     DeleteMissionProfileRequestRequestTypeDef,
     WaiterConfigTypeDef,
@@ -427,24 +428,20 @@
     GetMinuteUsageRequestRequestTypeDef,
     GetMissionProfileRequestRequestTypeDef,
     GetSatelliteRequestRequestTypeDef,
     GroundStationDataTypeDef,
     IntegerRangeTypeDef,
     PaginatorConfigTypeDef,
     ListConfigsRequestRequestTypeDef,
-    ListContactsRequestRequestTypeDef,
     ListDataflowEndpointGroupsRequestRequestTypeDef,
-    ListEphemeridesRequestRequestTypeDef,
     ListGroundStationsRequestRequestTypeDef,
     ListMissionProfilesRequestRequestTypeDef,
     MissionProfileListItemTypeDef,
     ListSatellitesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ReserveContactRequestRequestTypeDef,
-    TimeRangeTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateEphemerisRequestRequestTypeDef,
     AgentDetailsTypeDef,
     UpdateAgentStatusRequestRequestTypeDef,
     ConfigIdResponseTypeDef,
     ContactIdResponseTypeDef,
@@ -456,14 +453,18 @@
     MissionProfileIdResponseTypeDef,
     RegisterAgentResponseTypeDef,
     UpdateAgentStatusResponseTypeDef,
     ListConfigsResponseTypeDef,
     ConnectionDetailsTypeDef,
     DataflowEndpointTypeDef,
     ContactDataTypeDef,
+    ListContactsRequestRequestTypeDef,
+    ListEphemeridesRequestRequestTypeDef,
+    ReserveContactRequestRequestTypeDef,
+    TimeRangeTypeDef,
     CreateMissionProfileRequestRequestTypeDef,
     GetMissionProfileResponseTypeDef,
     UpdateMissionProfileRequestRequestTypeDef,
     ListDataflowEndpointGroupsResponseTypeDef,
     DescribeContactRequestContactScheduledWaitTypeDef,
     EphemerisDescriptionTypeDef,
     EphemerisItemTypeDef,
@@ -478,17 +479,17 @@
     ListContactsRequestListContactsPaginateTypeDef,
     ListDataflowEndpointGroupsRequestListDataflowEndpointGroupsPaginateTypeDef,
     ListEphemeridesRequestListEphemeridesPaginateTypeDef,
     ListGroundStationsRequestListGroundStationsPaginateTypeDef,
     ListMissionProfilesRequestListMissionProfilesPaginateTypeDef,
     ListSatellitesRequestListSatellitesPaginateTypeDef,
     ListMissionProfilesResponseTypeDef,
-    TLEDataTypeDef,
     RegisterAgentRequestRequestTypeDef,
     ListContactsResponseTypeDef,
+    TLEDataTypeDef,
     EphemerisTypeDescriptionTypeDef,
     ListEphemeridesResponseTypeDef,
     ListSatellitesResponseTypeDef,
     AntennaDownlinkConfigTypeDef,
     AntennaDownlinkDemodDecodeConfigTypeDef,
     AntennaUplinkConfigTypeDef,
     RangedConnectionDetailsTypeDef,
@@ -501,23 +502,24 @@
     GetConfigResponseTypeDef,
     UpdateConfigRequestRequestTypeDef,
     EndpointDetailsOutputTypeDef,
     EndpointDetailsTypeDef,
     CreateEphemerisRequestRequestTypeDef,
     ConfigDetailsTypeDef,
     GetDataflowEndpointGroupResponseTypeDef,
-    CreateDataflowEndpointGroupRequestRequestTypeDef,
+    EndpointDetailsUnionTypeDef,
     DestinationTypeDef,
     SourceTypeDef,
+    CreateDataflowEndpointGroupRequestRequestTypeDef,
     DataflowDetailTypeDef,
     DescribeContactResponseTypeDef,
 )
 
 
-def get_structure() -> ComponentVersionTypeDef:
+def get_value() -> ComponentVersionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-groundstation-1.28.15.post1/README.md` & `mypy-boto3-groundstation-1.28.16/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-groundstation.svg?color=blue)](https://pypi.org/project/mypy-boto3-groundstation)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-groundstation)](https://pepy.tech/project/mypy-boto3-groundstation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GroundStation 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation)
+[boto3.GroundStation 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation)
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
 [mypy-boto3-groundstation docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/).
 
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
@@ -343,20 +343,20 @@
 )
 
 
 def check_value(value: AgentStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_groundstation.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_groundstation.type_defs import (
     ComponentVersionTypeDef,
     AggregateStatusTypeDef,
     AntennaDemodDecodeDetailsTypeDef,
     DecodeConfigTypeDef,
@@ -369,14 +369,15 @@
     ConfigListItemTypeDef,
     DataflowEndpointConfigTypeDef,
     S3RecordingConfigTypeDef,
     TrackingConfigTypeDef,
     UplinkEchoConfigTypeDef,
     SocketAddressTypeDef,
     ElevationTypeDef,
+    TimestampTypeDef,
     KmsKeyTypeDef,
     DataflowEndpointListItemTypeDef,
     DeleteConfigRequestRequestTypeDef,
     DeleteDataflowEndpointGroupRequestRequestTypeDef,
     DeleteEphemerisRequestRequestTypeDef,
     DeleteMissionProfileRequestRequestTypeDef,
     WaiterConfigTypeDef,
@@ -395,24 +396,20 @@
     GetMinuteUsageRequestRequestTypeDef,
     GetMissionProfileRequestRequestTypeDef,
     GetSatelliteRequestRequestTypeDef,
     GroundStationDataTypeDef,
     IntegerRangeTypeDef,
     PaginatorConfigTypeDef,
     ListConfigsRequestRequestTypeDef,
-    ListContactsRequestRequestTypeDef,
     ListDataflowEndpointGroupsRequestRequestTypeDef,
-    ListEphemeridesRequestRequestTypeDef,
     ListGroundStationsRequestRequestTypeDef,
     ListMissionProfilesRequestRequestTypeDef,
     MissionProfileListItemTypeDef,
     ListSatellitesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ReserveContactRequestRequestTypeDef,
-    TimeRangeTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateEphemerisRequestRequestTypeDef,
     AgentDetailsTypeDef,
     UpdateAgentStatusRequestRequestTypeDef,
     ConfigIdResponseTypeDef,
     ContactIdResponseTypeDef,
@@ -424,14 +421,18 @@
     MissionProfileIdResponseTypeDef,
     RegisterAgentResponseTypeDef,
     UpdateAgentStatusResponseTypeDef,
     ListConfigsResponseTypeDef,
     ConnectionDetailsTypeDef,
     DataflowEndpointTypeDef,
     ContactDataTypeDef,
+    ListContactsRequestRequestTypeDef,
+    ListEphemeridesRequestRequestTypeDef,
+    ReserveContactRequestRequestTypeDef,
+    TimeRangeTypeDef,
     CreateMissionProfileRequestRequestTypeDef,
     GetMissionProfileResponseTypeDef,
     UpdateMissionProfileRequestRequestTypeDef,
     ListDataflowEndpointGroupsResponseTypeDef,
     DescribeContactRequestContactScheduledWaitTypeDef,
     EphemerisDescriptionTypeDef,
     EphemerisItemTypeDef,
@@ -446,17 +447,17 @@
     ListContactsRequestListContactsPaginateTypeDef,
     ListDataflowEndpointGroupsRequestListDataflowEndpointGroupsPaginateTypeDef,
     ListEphemeridesRequestListEphemeridesPaginateTypeDef,
     ListGroundStationsRequestListGroundStationsPaginateTypeDef,
     ListMissionProfilesRequestListMissionProfilesPaginateTypeDef,
     ListSatellitesRequestListSatellitesPaginateTypeDef,
     ListMissionProfilesResponseTypeDef,
-    TLEDataTypeDef,
     RegisterAgentRequestRequestTypeDef,
     ListContactsResponseTypeDef,
+    TLEDataTypeDef,
     EphemerisTypeDescriptionTypeDef,
     ListEphemeridesResponseTypeDef,
     ListSatellitesResponseTypeDef,
     AntennaDownlinkConfigTypeDef,
     AntennaDownlinkDemodDecodeConfigTypeDef,
     AntennaUplinkConfigTypeDef,
     RangedConnectionDetailsTypeDef,
@@ -469,23 +470,24 @@
     GetConfigResponseTypeDef,
     UpdateConfigRequestRequestTypeDef,
     EndpointDetailsOutputTypeDef,
     EndpointDetailsTypeDef,
     CreateEphemerisRequestRequestTypeDef,
     ConfigDetailsTypeDef,
     GetDataflowEndpointGroupResponseTypeDef,
-    CreateDataflowEndpointGroupRequestRequestTypeDef,
+    EndpointDetailsUnionTypeDef,
     DestinationTypeDef,
     SourceTypeDef,
+    CreateDataflowEndpointGroupRequestRequestTypeDef,
     DataflowDetailTypeDef,
     DescribeContactResponseTypeDef,
 )
 
 
-def get_structure() -> ComponentVersionTypeDef:
+def get_value() -> ComponentVersionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation/__init__.py` & `mypy-boto3-groundstation-1.28.16/mypy_boto3_groundstation/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation/__init__.pyi` & `mypy-boto3-groundstation-1.28.16/mypy_boto3_groundstation/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation/__main__.py` & `mypy-boto3-groundstation-1.28.16/mypy_boto3_groundstation/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.GroundStation 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.GroundStation 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation\nOther"
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

### Comparing `mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation/client.py` & `mypy-boto3-groundstation-1.28.16/mypy_boto3_groundstation/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_groundstation.client import GroundStationClient
 
     session = Session()
     client: GroundStationClient = session.client("groundstation")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ConfigCapabilityTypeType, ContactStatusType, EphemerisStatusType
 from .paginator import (
     ListConfigsPaginator,
     ListContactsPaginator,
@@ -36,16 +35,15 @@
     ConfigIdResponseTypeDef,
     ConfigTypeDataTypeDef,
     ContactIdResponseTypeDef,
     DataflowEndpointGroupIdResponseTypeDef,
     DescribeContactResponseTypeDef,
     DescribeEphemerisResponseTypeDef,
     DiscoveryDataTypeDef,
-    EndpointDetailsOutputTypeDef,
-    EndpointDetailsTypeDef,
+    EndpointDetailsUnionTypeDef,
     EphemerisDataTypeDef,
     EphemerisIdResponseTypeDef,
     GetAgentConfigurationResponseTypeDef,
     GetConfigResponseTypeDef,
     GetDataflowEndpointGroupResponseTypeDef,
     GetMinuteUsageResponseTypeDef,
     GetMissionProfileResponseTypeDef,
@@ -57,14 +55,15 @@
     ListEphemeridesResponseTypeDef,
     ListGroundStationsResponseTypeDef,
     ListMissionProfilesResponseTypeDef,
     ListSatellitesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     MissionProfileIdResponseTypeDef,
     RegisterAgentResponseTypeDef,
+    TimestampTypeDef,
     UpdateAgentStatusResponseTypeDef,
 )
 from .waiter import ContactScheduledWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -140,15 +139,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.create_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/client/#create_config)
         """
 
     def create_dataflow_endpoint_group(
         self,
         *,
-        endpointDetails: Sequence[Union[EndpointDetailsTypeDef, EndpointDetailsOutputTypeDef]],
+        endpointDetails: Sequence[EndpointDetailsUnionTypeDef],
         contactPostPassDurationSeconds: int = ...,
         contactPrePassDurationSeconds: int = ...,
         tags: Mapping[str, str] = ...
     ) -> DataflowEndpointGroupIdResponseTypeDef:
         """
         Creates a `DataflowEndpoint` group containing the specified list of
         `DataflowEndpoint` objects.
@@ -160,15 +159,15 @@
     def create_ephemeris(
         self,
         *,
         name: str,
         satelliteId: str,
         enabled: bool = ...,
         ephemeris: EphemerisDataTypeDef = ...,
-        expirationTime: Union[datetime, str] = ...,
+        expirationTime: TimestampTypeDef = ...,
         kmsKeyArn: str = ...,
         priority: int = ...,
         tags: Mapping[str, str] = ...
     ) -> EphemerisIdResponseTypeDef:
         """
         Creates an Ephemeris with the specified `EphemerisData`.
 
@@ -324,16 +323,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.list_configs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/client/#list_configs)
         """
 
     def list_contacts(
         self,
         *,
-        endTime: Union[datetime, str],
-        startTime: Union[datetime, str],
+        endTime: TimestampTypeDef,
+        startTime: TimestampTypeDef,
         statusList: Sequence[ContactStatusType],
         groundStation: str = ...,
         maxResults: int = ...,
         missionProfileArn: str = ...,
         nextToken: str = ...,
         satelliteArn: str = ...
     ) -> ListContactsResponseTypeDef:
@@ -353,17 +352,17 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.list_dataflow_endpoint_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/client/#list_dataflow_endpoint_groups)
         """
 
     def list_ephemerides(
         self,
         *,
-        endTime: Union[datetime, str],
+        endTime: TimestampTypeDef,
         satelliteId: str,
-        startTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
         maxResults: int = ...,
         nextToken: str = ...,
         statusList: Sequence[EphemerisStatusType] = ...
     ) -> ListEphemeridesResponseTypeDef:
         """
         List existing ephemerides.
 
@@ -418,19 +417,19 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.register_agent)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/client/#register_agent)
         """
 
     def reserve_contact(
         self,
         *,
-        endTime: Union[datetime, str],
+        endTime: TimestampTypeDef,
         groundStation: str,
         missionProfileArn: str,
         satelliteArn: str,
-        startTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
         tags: Mapping[str, str] = ...
     ) -> ContactIdResponseTypeDef:
         """
         Reserves a contact using specified parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.reserve_contact)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/client/#reserve_contact)
```

### Comparing `mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation/client.pyi` & `mypy-boto3-groundstation-1.28.16/mypy_boto3_groundstation/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_groundstation.client import GroundStationClient
 
     session = Session()
     client: GroundStationClient = session.client("groundstation")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ConfigCapabilityTypeType, ContactStatusType, EphemerisStatusType
 from .paginator import (
     ListConfigsPaginator,
     ListContactsPaginator,
@@ -36,16 +35,15 @@
     ConfigIdResponseTypeDef,
     ConfigTypeDataTypeDef,
     ContactIdResponseTypeDef,
     DataflowEndpointGroupIdResponseTypeDef,
     DescribeContactResponseTypeDef,
     DescribeEphemerisResponseTypeDef,
     DiscoveryDataTypeDef,
-    EndpointDetailsOutputTypeDef,
-    EndpointDetailsTypeDef,
+    EndpointDetailsUnionTypeDef,
     EphemerisDataTypeDef,
     EphemerisIdResponseTypeDef,
     GetAgentConfigurationResponseTypeDef,
     GetConfigResponseTypeDef,
     GetDataflowEndpointGroupResponseTypeDef,
     GetMinuteUsageResponseTypeDef,
     GetMissionProfileResponseTypeDef,
@@ -57,14 +55,15 @@
     ListEphemeridesResponseTypeDef,
     ListGroundStationsResponseTypeDef,
     ListMissionProfilesResponseTypeDef,
     ListSatellitesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     MissionProfileIdResponseTypeDef,
     RegisterAgentResponseTypeDef,
+    TimestampTypeDef,
     UpdateAgentStatusResponseTypeDef,
 )
 from .waiter import ContactScheduledWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -131,15 +130,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.create_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/client/#create_config)
         """
     def create_dataflow_endpoint_group(
         self,
         *,
-        endpointDetails: Sequence[Union[EndpointDetailsTypeDef, EndpointDetailsOutputTypeDef]],
+        endpointDetails: Sequence[EndpointDetailsUnionTypeDef],
         contactPostPassDurationSeconds: int = ...,
         contactPrePassDurationSeconds: int = ...,
         tags: Mapping[str, str] = ...
     ) -> DataflowEndpointGroupIdResponseTypeDef:
         """
         Creates a `DataflowEndpoint` group containing the specified list of
         `DataflowEndpoint` objects.
@@ -150,15 +149,15 @@
     def create_ephemeris(
         self,
         *,
         name: str,
         satelliteId: str,
         enabled: bool = ...,
         ephemeris: EphemerisDataTypeDef = ...,
-        expirationTime: Union[datetime, str] = ...,
+        expirationTime: TimestampTypeDef = ...,
         kmsKeyArn: str = ...,
         priority: int = ...,
         tags: Mapping[str, str] = ...
     ) -> EphemerisIdResponseTypeDef:
         """
         Creates an Ephemeris with the specified `EphemerisData`.
 
@@ -298,16 +297,16 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.list_configs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/client/#list_configs)
         """
     def list_contacts(
         self,
         *,
-        endTime: Union[datetime, str],
-        startTime: Union[datetime, str],
+        endTime: TimestampTypeDef,
+        startTime: TimestampTypeDef,
         statusList: Sequence[ContactStatusType],
         groundStation: str = ...,
         maxResults: int = ...,
         missionProfileArn: str = ...,
         nextToken: str = ...,
         satelliteArn: str = ...
     ) -> ListContactsResponseTypeDef:
@@ -325,17 +324,17 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.list_dataflow_endpoint_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/client/#list_dataflow_endpoint_groups)
         """
     def list_ephemerides(
         self,
         *,
-        endTime: Union[datetime, str],
+        endTime: TimestampTypeDef,
         satelliteId: str,
-        startTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
         maxResults: int = ...,
         nextToken: str = ...,
         statusList: Sequence[EphemerisStatusType] = ...
     ) -> ListEphemeridesResponseTypeDef:
         """
         List existing ephemerides.
 
@@ -384,19 +383,19 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.register_agent)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/client/#register_agent)
         """
     def reserve_contact(
         self,
         *,
-        endTime: Union[datetime, str],
+        endTime: TimestampTypeDef,
         groundStation: str,
         missionProfileArn: str,
         satelliteArn: str,
-        startTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
         tags: Mapping[str, str] = ...
     ) -> ContactIdResponseTypeDef:
         """
         Reserves a contact using specified parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.reserve_contact)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/client/#reserve_contact)
```

### Comparing `mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation/literals.py` & `mypy-boto3-groundstation-1.28.16/mypy_boto3_groundstation/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation/literals.pyi` & `mypy-boto3-groundstation-1.28.16/mypy_boto3_groundstation/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation/paginator.py` & `mypy-boto3-groundstation-1.28.16/mypy_boto3_groundstation/paginator.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,29 +27,29 @@
     list_dataflow_endpoint_groups_paginator: ListDataflowEndpointGroupsPaginator = client.get_paginator("list_dataflow_endpoint_groups")
     list_ephemerides_paginator: ListEphemeridesPaginator = client.get_paginator("list_ephemerides")
     list_ground_stations_paginator: ListGroundStationsPaginator = client.get_paginator("list_ground_stations")
     list_mission_profiles_paginator: ListMissionProfilesPaginator = client.get_paginator("list_mission_profiles")
     list_satellites_paginator: ListSatellitesPaginator = client.get_paginator("list_satellites")
     ```
 """
-from datetime import datetime
-from typing import Generic, Iterator, Sequence, TypeVar, Union
+from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import ContactStatusType, EphemerisStatusType
 from .type_defs import (
     ListConfigsResponseTypeDef,
     ListContactsResponseTypeDef,
     ListDataflowEndpointGroupsResponseTypeDef,
     ListEphemeridesResponseTypeDef,
     ListGroundStationsResponseTypeDef,
     ListMissionProfilesResponseTypeDef,
     ListSatellitesResponseTypeDef,
     PaginatorConfigTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "ListConfigsPaginator",
     "ListContactsPaginator",
     "ListDataflowEndpointGroupsPaginator",
     "ListEphemeridesPaginator",
@@ -89,16 +89,16 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Paginator.ListContacts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/paginators/#listcontactspaginator)
     """
 
     def paginate(
         self,
         *,
-        endTime: Union[datetime, str],
-        startTime: Union[datetime, str],
+        endTime: TimestampTypeDef,
+        startTime: TimestampTypeDef,
         statusList: Sequence[ContactStatusType],
         groundStation: str = ...,
         missionProfileArn: str = ...,
         satelliteArn: str = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListContactsResponseTypeDef]:
         """
@@ -127,17 +127,17 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Paginator.ListEphemerides)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/paginators/#listephemeridespaginator)
     """
 
     def paginate(
         self,
         *,
-        endTime: Union[datetime, str],
+        endTime: TimestampTypeDef,
         satelliteId: str,
-        startTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
         statusList: Sequence[EphemerisStatusType] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListEphemeridesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Paginator.ListEphemerides.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/paginators/#listephemeridespaginator)
         """
```

### Comparing `mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation/paginator.pyi` & `mypy-boto3-groundstation-1.28.16/mypy_boto3_groundstation/paginator.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -27,29 +27,29 @@
     list_dataflow_endpoint_groups_paginator: ListDataflowEndpointGroupsPaginator = client.get_paginator("list_dataflow_endpoint_groups")
     list_ephemerides_paginator: ListEphemeridesPaginator = client.get_paginator("list_ephemerides")
     list_ground_stations_paginator: ListGroundStationsPaginator = client.get_paginator("list_ground_stations")
     list_mission_profiles_paginator: ListMissionProfilesPaginator = client.get_paginator("list_mission_profiles")
     list_satellites_paginator: ListSatellitesPaginator = client.get_paginator("list_satellites")
     ```
 """
-from datetime import datetime
-from typing import Generic, Iterator, Sequence, TypeVar, Union
+from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import ContactStatusType, EphemerisStatusType
 from .type_defs import (
     ListConfigsResponseTypeDef,
     ListContactsResponseTypeDef,
     ListDataflowEndpointGroupsResponseTypeDef,
     ListEphemeridesResponseTypeDef,
     ListGroundStationsResponseTypeDef,
     ListMissionProfilesResponseTypeDef,
     ListSatellitesResponseTypeDef,
     PaginatorConfigTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "ListConfigsPaginator",
     "ListContactsPaginator",
     "ListDataflowEndpointGroupsPaginator",
     "ListEphemeridesPaginator",
@@ -85,16 +85,16 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Paginator.ListContacts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/paginators/#listcontactspaginator)
     """
 
     def paginate(
         self,
         *,
-        endTime: Union[datetime, str],
-        startTime: Union[datetime, str],
+        endTime: TimestampTypeDef,
+        startTime: TimestampTypeDef,
         statusList: Sequence[ContactStatusType],
         groundStation: str = ...,
         missionProfileArn: str = ...,
         satelliteArn: str = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListContactsResponseTypeDef]:
         """
@@ -121,17 +121,17 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Paginator.ListEphemerides)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/paginators/#listephemeridespaginator)
     """
 
     def paginate(
         self,
         *,
-        endTime: Union[datetime, str],
+        endTime: TimestampTypeDef,
         satelliteId: str,
-        startTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
         statusList: Sequence[EphemerisStatusType] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListEphemeridesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Paginator.ListEphemerides.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/paginators/#listephemeridespaginator)
         """
```

### Comparing `mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation/type_defs.py` & `mypy-boto3-groundstation-1.28.16/mypy_boto3_groundstation/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_groundstation.type_defs import ComponentVersionTypeDef
 
-    data: ComponentVersionTypeDef = {...}
+    data: ComponentVersionTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -57,14 +57,15 @@
     "ConfigListItemTypeDef",
     "DataflowEndpointConfigTypeDef",
     "S3RecordingConfigTypeDef",
     "TrackingConfigTypeDef",
     "UplinkEchoConfigTypeDef",
     "SocketAddressTypeDef",
     "ElevationTypeDef",
+    "TimestampTypeDef",
     "KmsKeyTypeDef",
     "DataflowEndpointListItemTypeDef",
     "DeleteConfigRequestRequestTypeDef",
     "DeleteDataflowEndpointGroupRequestRequestTypeDef",
     "DeleteEphemerisRequestRequestTypeDef",
     "DeleteMissionProfileRequestRequestTypeDef",
     "WaiterConfigTypeDef",
@@ -83,24 +84,20 @@
     "GetMinuteUsageRequestRequestTypeDef",
     "GetMissionProfileRequestRequestTypeDef",
     "GetSatelliteRequestRequestTypeDef",
     "GroundStationDataTypeDef",
     "IntegerRangeTypeDef",
     "PaginatorConfigTypeDef",
     "ListConfigsRequestRequestTypeDef",
-    "ListContactsRequestRequestTypeDef",
     "ListDataflowEndpointGroupsRequestRequestTypeDef",
-    "ListEphemeridesRequestRequestTypeDef",
     "ListGroundStationsRequestRequestTypeDef",
     "ListMissionProfilesRequestRequestTypeDef",
     "MissionProfileListItemTypeDef",
     "ListSatellitesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ReserveContactRequestRequestTypeDef",
-    "TimeRangeTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateEphemerisRequestRequestTypeDef",
     "AgentDetailsTypeDef",
     "UpdateAgentStatusRequestRequestTypeDef",
     "ConfigIdResponseTypeDef",
     "ContactIdResponseTypeDef",
@@ -112,14 +109,18 @@
     "MissionProfileIdResponseTypeDef",
     "RegisterAgentResponseTypeDef",
     "UpdateAgentStatusResponseTypeDef",
     "ListConfigsResponseTypeDef",
     "ConnectionDetailsTypeDef",
     "DataflowEndpointTypeDef",
     "ContactDataTypeDef",
+    "ListContactsRequestRequestTypeDef",
+    "ListEphemeridesRequestRequestTypeDef",
+    "ReserveContactRequestRequestTypeDef",
+    "TimeRangeTypeDef",
     "CreateMissionProfileRequestRequestTypeDef",
     "GetMissionProfileResponseTypeDef",
     "UpdateMissionProfileRequestRequestTypeDef",
     "ListDataflowEndpointGroupsResponseTypeDef",
     "DescribeContactRequestContactScheduledWaitTypeDef",
     "EphemerisDescriptionTypeDef",
     "EphemerisItemTypeDef",
@@ -134,17 +135,17 @@
     "ListContactsRequestListContactsPaginateTypeDef",
     "ListDataflowEndpointGroupsRequestListDataflowEndpointGroupsPaginateTypeDef",
     "ListEphemeridesRequestListEphemeridesPaginateTypeDef",
     "ListGroundStationsRequestListGroundStationsPaginateTypeDef",
     "ListMissionProfilesRequestListMissionProfilesPaginateTypeDef",
     "ListSatellitesRequestListSatellitesPaginateTypeDef",
     "ListMissionProfilesResponseTypeDef",
-    "TLEDataTypeDef",
     "RegisterAgentRequestRequestTypeDef",
     "ListContactsResponseTypeDef",
+    "TLEDataTypeDef",
     "EphemerisTypeDescriptionTypeDef",
     "ListEphemeridesResponseTypeDef",
     "ListSatellitesResponseTypeDef",
     "AntennaDownlinkConfigTypeDef",
     "AntennaDownlinkDemodDecodeConfigTypeDef",
     "AntennaUplinkConfigTypeDef",
     "RangedConnectionDetailsTypeDef",
@@ -157,17 +158,18 @@
     "GetConfigResponseTypeDef",
     "UpdateConfigRequestRequestTypeDef",
     "EndpointDetailsOutputTypeDef",
     "EndpointDetailsTypeDef",
     "CreateEphemerisRequestRequestTypeDef",
     "ConfigDetailsTypeDef",
     "GetDataflowEndpointGroupResponseTypeDef",
-    "CreateDataflowEndpointGroupRequestRequestTypeDef",
+    "EndpointDetailsUnionTypeDef",
     "DestinationTypeDef",
     "SourceTypeDef",
+    "CreateDataflowEndpointGroupRequestRequestTypeDef",
     "DataflowDetailTypeDef",
     "DescribeContactResponseTypeDef",
 )
 
 ComponentVersionTypeDef = TypedDict(
     "ComponentVersionTypeDef",
     {
@@ -359,14 +361,15 @@
     "ElevationTypeDef",
     {
         "unit": AngleUnitsType,
         "value": float,
     },
 )
 
+TimestampTypeDef = Union[datetime, str]
 KmsKeyTypeDef = TypedDict(
     "KmsKeyTypeDef",
     {
         "kmsAliasArn": str,
         "kmsKeyArn": str,
     },
     total=False,
@@ -586,75 +589,23 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-_RequiredListContactsRequestRequestTypeDef = TypedDict(
-    "_RequiredListContactsRequestRequestTypeDef",
-    {
-        "endTime": Union[datetime, str],
-        "startTime": Union[datetime, str],
-        "statusList": Sequence[ContactStatusType],
-    },
-)
-_OptionalListContactsRequestRequestTypeDef = TypedDict(
-    "_OptionalListContactsRequestRequestTypeDef",
-    {
-        "groundStation": str,
-        "maxResults": int,
-        "missionProfileArn": str,
-        "nextToken": str,
-        "satelliteArn": str,
-    },
-    total=False,
-)
-
-
-class ListContactsRequestRequestTypeDef(
-    _RequiredListContactsRequestRequestTypeDef, _OptionalListContactsRequestRequestTypeDef
-):
-    pass
-
-
 ListDataflowEndpointGroupsRequestRequestTypeDef = TypedDict(
     "ListDataflowEndpointGroupsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-_RequiredListEphemeridesRequestRequestTypeDef = TypedDict(
-    "_RequiredListEphemeridesRequestRequestTypeDef",
-    {
-        "endTime": Union[datetime, str],
-        "satelliteId": str,
-        "startTime": Union[datetime, str],
-    },
-)
-_OptionalListEphemeridesRequestRequestTypeDef = TypedDict(
-    "_OptionalListEphemeridesRequestRequestTypeDef",
-    {
-        "maxResults": int,
-        "nextToken": str,
-        "statusList": Sequence[EphemerisStatusType],
-    },
-    total=False,
-)
-
-
-class ListEphemeridesRequestRequestTypeDef(
-    _RequiredListEphemeridesRequestRequestTypeDef, _OptionalListEphemeridesRequestRequestTypeDef
-):
-    pass
-
-
 ListGroundStationsRequestRequestTypeDef = TypedDict(
     "ListGroundStationsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "satelliteId": str,
     },
@@ -693,47 +644,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-_RequiredReserveContactRequestRequestTypeDef = TypedDict(
-    "_RequiredReserveContactRequestRequestTypeDef",
-    {
-        "endTime": Union[datetime, str],
-        "groundStation": str,
-        "missionProfileArn": str,
-        "satelliteArn": str,
-        "startTime": Union[datetime, str],
-    },
-)
-_OptionalReserveContactRequestRequestTypeDef = TypedDict(
-    "_OptionalReserveContactRequestRequestTypeDef",
-    {
-        "tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class ReserveContactRequestRequestTypeDef(
-    _RequiredReserveContactRequestRequestTypeDef, _OptionalReserveContactRequestRequestTypeDef
-):
-    pass
-
-
-TimeRangeTypeDef = TypedDict(
-    "TimeRangeTypeDef",
-    {
-        "endTime": Union[datetime, str],
-        "startTime": Union[datetime, str],
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -946,14 +864,99 @@
         "satelliteArn": str,
         "startTime": datetime,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
+_RequiredListContactsRequestRequestTypeDef = TypedDict(
+    "_RequiredListContactsRequestRequestTypeDef",
+    {
+        "endTime": TimestampTypeDef,
+        "startTime": TimestampTypeDef,
+        "statusList": Sequence[ContactStatusType],
+    },
+)
+_OptionalListContactsRequestRequestTypeDef = TypedDict(
+    "_OptionalListContactsRequestRequestTypeDef",
+    {
+        "groundStation": str,
+        "maxResults": int,
+        "missionProfileArn": str,
+        "nextToken": str,
+        "satelliteArn": str,
+    },
+    total=False,
+)
+
+
+class ListContactsRequestRequestTypeDef(
+    _RequiredListContactsRequestRequestTypeDef, _OptionalListContactsRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredListEphemeridesRequestRequestTypeDef = TypedDict(
+    "_RequiredListEphemeridesRequestRequestTypeDef",
+    {
+        "endTime": TimestampTypeDef,
+        "satelliteId": str,
+        "startTime": TimestampTypeDef,
+    },
+)
+_OptionalListEphemeridesRequestRequestTypeDef = TypedDict(
+    "_OptionalListEphemeridesRequestRequestTypeDef",
+    {
+        "maxResults": int,
+        "nextToken": str,
+        "statusList": Sequence[EphemerisStatusType],
+    },
+    total=False,
+)
+
+
+class ListEphemeridesRequestRequestTypeDef(
+    _RequiredListEphemeridesRequestRequestTypeDef, _OptionalListEphemeridesRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredReserveContactRequestRequestTypeDef = TypedDict(
+    "_RequiredReserveContactRequestRequestTypeDef",
+    {
+        "endTime": TimestampTypeDef,
+        "groundStation": str,
+        "missionProfileArn": str,
+        "satelliteArn": str,
+        "startTime": TimestampTypeDef,
+    },
+)
+_OptionalReserveContactRequestRequestTypeDef = TypedDict(
+    "_OptionalReserveContactRequestRequestTypeDef",
+    {
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class ReserveContactRequestRequestTypeDef(
+    _RequiredReserveContactRequestRequestTypeDef, _OptionalReserveContactRequestRequestTypeDef
+):
+    pass
+
+
+TimeRangeTypeDef = TypedDict(
+    "TimeRangeTypeDef",
+    {
+        "endTime": TimestampTypeDef,
+        "startTime": TimestampTypeDef,
+    },
+)
+
 _RequiredCreateMissionProfileRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMissionProfileRequestRequestTypeDef",
     {
         "dataflowEdges": Sequence[Sequence[str]],
         "minimumViableContactDurationSeconds": int,
         "name": str,
         "trackingConfigArn": str,
@@ -1179,16 +1182,16 @@
     },
     total=False,
 )
 
 _RequiredListContactsRequestListContactsPaginateTypeDef = TypedDict(
     "_RequiredListContactsRequestListContactsPaginateTypeDef",
     {
-        "endTime": Union[datetime, str],
-        "startTime": Union[datetime, str],
+        "endTime": TimestampTypeDef,
+        "startTime": TimestampTypeDef,
         "statusList": Sequence[ContactStatusType],
     },
 )
 _OptionalListContactsRequestListContactsPaginateTypeDef = TypedDict(
     "_OptionalListContactsRequestListContactsPaginateTypeDef",
     {
         "groundStation": str,
@@ -1214,17 +1217,17 @@
     },
     total=False,
 )
 
 _RequiredListEphemeridesRequestListEphemeridesPaginateTypeDef = TypedDict(
     "_RequiredListEphemeridesRequestListEphemeridesPaginateTypeDef",
     {
-        "endTime": Union[datetime, str],
+        "endTime": TimestampTypeDef,
         "satelliteId": str,
-        "startTime": Union[datetime, str],
+        "startTime": TimestampTypeDef,
     },
 )
 _OptionalListEphemeridesRequestListEphemeridesPaginateTypeDef = TypedDict(
     "_OptionalListEphemeridesRequestListEphemeridesPaginateTypeDef",
     {
         "statusList": Sequence[EphemerisStatusType],
         "PaginationConfig": PaginatorConfigTypeDef,
@@ -1270,23 +1273,14 @@
     {
         "missionProfileList": List[MissionProfileListItemTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TLEDataTypeDef = TypedDict(
-    "TLEDataTypeDef",
-    {
-        "tleLine1": str,
-        "tleLine2": str,
-        "validTimeRange": TimeRangeTypeDef,
-    },
-)
-
 RegisterAgentRequestRequestTypeDef = TypedDict(
     "RegisterAgentRequestRequestTypeDef",
     {
         "agentDetails": AgentDetailsTypeDef,
         "discoveryData": DiscoveryDataTypeDef,
     },
 )
@@ -1296,14 +1290,23 @@
     {
         "contactList": List[ContactDataTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+TLEDataTypeDef = TypedDict(
+    "TLEDataTypeDef",
+    {
+        "tleLine1": str,
+        "tleLine2": str,
+        "validTimeRange": TimeRangeTypeDef,
+    },
+)
+
 EphemerisTypeDescriptionTypeDef = TypedDict(
     "EphemerisTypeDescriptionTypeDef",
     {
         "oem": EphemerisDescriptionTypeDef,
         "tle": EphemerisDescriptionTypeDef,
     },
     total=False,
@@ -1536,15 +1539,15 @@
     },
 )
 _OptionalCreateEphemerisRequestRequestTypeDef = TypedDict(
     "_OptionalCreateEphemerisRequestRequestTypeDef",
     {
         "enabled": bool,
         "ephemeris": EphemerisDataTypeDef,
-        "expirationTime": Union[datetime, str],
+        "expirationTime": TimestampTypeDef,
         "kmsKeyArn": str,
         "priority": int,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
@@ -1574,18 +1577,41 @@
         "dataflowEndpointGroupId": str,
         "endpointsDetails": List[EndpointDetailsOutputTypeDef],
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+EndpointDetailsUnionTypeDef = Union[EndpointDetailsTypeDef, EndpointDetailsOutputTypeDef]
+DestinationTypeDef = TypedDict(
+    "DestinationTypeDef",
+    {
+        "configDetails": ConfigDetailsTypeDef,
+        "configId": str,
+        "configType": ConfigCapabilityTypeType,
+        "dataflowDestinationRegion": str,
+    },
+    total=False,
+)
+
+SourceTypeDef = TypedDict(
+    "SourceTypeDef",
+    {
+        "configDetails": ConfigDetailsTypeDef,
+        "configId": str,
+        "configType": ConfigCapabilityTypeType,
+        "dataflowSourceRegion": str,
+    },
+    total=False,
+)
+
 _RequiredCreateDataflowEndpointGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDataflowEndpointGroupRequestRequestTypeDef",
     {
-        "endpointDetails": Sequence[Union[EndpointDetailsTypeDef, EndpointDetailsOutputTypeDef]],
+        "endpointDetails": Sequence[EndpointDetailsUnionTypeDef],
     },
 )
 _OptionalCreateDataflowEndpointGroupRequestRequestTypeDef = TypedDict(
     "_OptionalCreateDataflowEndpointGroupRequestRequestTypeDef",
     {
         "contactPostPassDurationSeconds": int,
         "contactPrePassDurationSeconds": int,
@@ -1598,36 +1624,14 @@
 class CreateDataflowEndpointGroupRequestRequestTypeDef(
     _RequiredCreateDataflowEndpointGroupRequestRequestTypeDef,
     _OptionalCreateDataflowEndpointGroupRequestRequestTypeDef,
 ):
     pass
 
 
-DestinationTypeDef = TypedDict(
-    "DestinationTypeDef",
-    {
-        "configDetails": ConfigDetailsTypeDef,
-        "configId": str,
-        "configType": ConfigCapabilityTypeType,
-        "dataflowDestinationRegion": str,
-    },
-    total=False,
-)
-
-SourceTypeDef = TypedDict(
-    "SourceTypeDef",
-    {
-        "configDetails": ConfigDetailsTypeDef,
-        "configId": str,
-        "configType": ConfigCapabilityTypeType,
-        "dataflowSourceRegion": str,
-    },
-    total=False,
-)
-
 DataflowDetailTypeDef = TypedDict(
     "DataflowDetailTypeDef",
     {
         "destination": DestinationTypeDef,
         "errorMessage": str,
         "source": SourceTypeDef,
     },
```

### Comparing `mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation/type_defs.pyi` & `mypy-boto3-groundstation-1.28.16/mypy_boto3_groundstation/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_groundstation.type_defs import ComponentVersionTypeDef
 
-    data: ComponentVersionTypeDef = {...}
+    data: ComponentVersionTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -56,14 +56,15 @@
     "ConfigListItemTypeDef",
     "DataflowEndpointConfigTypeDef",
     "S3RecordingConfigTypeDef",
     "TrackingConfigTypeDef",
     "UplinkEchoConfigTypeDef",
     "SocketAddressTypeDef",
     "ElevationTypeDef",
+    "TimestampTypeDef",
     "KmsKeyTypeDef",
     "DataflowEndpointListItemTypeDef",
     "DeleteConfigRequestRequestTypeDef",
     "DeleteDataflowEndpointGroupRequestRequestTypeDef",
     "DeleteEphemerisRequestRequestTypeDef",
     "DeleteMissionProfileRequestRequestTypeDef",
     "WaiterConfigTypeDef",
@@ -82,24 +83,20 @@
     "GetMinuteUsageRequestRequestTypeDef",
     "GetMissionProfileRequestRequestTypeDef",
     "GetSatelliteRequestRequestTypeDef",
     "GroundStationDataTypeDef",
     "IntegerRangeTypeDef",
     "PaginatorConfigTypeDef",
     "ListConfigsRequestRequestTypeDef",
-    "ListContactsRequestRequestTypeDef",
     "ListDataflowEndpointGroupsRequestRequestTypeDef",
-    "ListEphemeridesRequestRequestTypeDef",
     "ListGroundStationsRequestRequestTypeDef",
     "ListMissionProfilesRequestRequestTypeDef",
     "MissionProfileListItemTypeDef",
     "ListSatellitesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ReserveContactRequestRequestTypeDef",
-    "TimeRangeTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateEphemerisRequestRequestTypeDef",
     "AgentDetailsTypeDef",
     "UpdateAgentStatusRequestRequestTypeDef",
     "ConfigIdResponseTypeDef",
     "ContactIdResponseTypeDef",
@@ -111,14 +108,18 @@
     "MissionProfileIdResponseTypeDef",
     "RegisterAgentResponseTypeDef",
     "UpdateAgentStatusResponseTypeDef",
     "ListConfigsResponseTypeDef",
     "ConnectionDetailsTypeDef",
     "DataflowEndpointTypeDef",
     "ContactDataTypeDef",
+    "ListContactsRequestRequestTypeDef",
+    "ListEphemeridesRequestRequestTypeDef",
+    "ReserveContactRequestRequestTypeDef",
+    "TimeRangeTypeDef",
     "CreateMissionProfileRequestRequestTypeDef",
     "GetMissionProfileResponseTypeDef",
     "UpdateMissionProfileRequestRequestTypeDef",
     "ListDataflowEndpointGroupsResponseTypeDef",
     "DescribeContactRequestContactScheduledWaitTypeDef",
     "EphemerisDescriptionTypeDef",
     "EphemerisItemTypeDef",
@@ -133,17 +134,17 @@
     "ListContactsRequestListContactsPaginateTypeDef",
     "ListDataflowEndpointGroupsRequestListDataflowEndpointGroupsPaginateTypeDef",
     "ListEphemeridesRequestListEphemeridesPaginateTypeDef",
     "ListGroundStationsRequestListGroundStationsPaginateTypeDef",
     "ListMissionProfilesRequestListMissionProfilesPaginateTypeDef",
     "ListSatellitesRequestListSatellitesPaginateTypeDef",
     "ListMissionProfilesResponseTypeDef",
-    "TLEDataTypeDef",
     "RegisterAgentRequestRequestTypeDef",
     "ListContactsResponseTypeDef",
+    "TLEDataTypeDef",
     "EphemerisTypeDescriptionTypeDef",
     "ListEphemeridesResponseTypeDef",
     "ListSatellitesResponseTypeDef",
     "AntennaDownlinkConfigTypeDef",
     "AntennaDownlinkDemodDecodeConfigTypeDef",
     "AntennaUplinkConfigTypeDef",
     "RangedConnectionDetailsTypeDef",
@@ -156,17 +157,18 @@
     "GetConfigResponseTypeDef",
     "UpdateConfigRequestRequestTypeDef",
     "EndpointDetailsOutputTypeDef",
     "EndpointDetailsTypeDef",
     "CreateEphemerisRequestRequestTypeDef",
     "ConfigDetailsTypeDef",
     "GetDataflowEndpointGroupResponseTypeDef",
-    "CreateDataflowEndpointGroupRequestRequestTypeDef",
+    "EndpointDetailsUnionTypeDef",
     "DestinationTypeDef",
     "SourceTypeDef",
+    "CreateDataflowEndpointGroupRequestRequestTypeDef",
     "DataflowDetailTypeDef",
     "DescribeContactResponseTypeDef",
 )
 
 ComponentVersionTypeDef = TypedDict(
     "ComponentVersionTypeDef",
     {
@@ -350,14 +352,15 @@
     "ElevationTypeDef",
     {
         "unit": AngleUnitsType,
         "value": float,
     },
 )
 
+TimestampTypeDef = Union[datetime, str]
 KmsKeyTypeDef = TypedDict(
     "KmsKeyTypeDef",
     {
         "kmsAliasArn": str,
         "kmsKeyArn": str,
     },
     total=False,
@@ -575,71 +578,23 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-_RequiredListContactsRequestRequestTypeDef = TypedDict(
-    "_RequiredListContactsRequestRequestTypeDef",
-    {
-        "endTime": Union[datetime, str],
-        "startTime": Union[datetime, str],
-        "statusList": Sequence[ContactStatusType],
-    },
-)
-_OptionalListContactsRequestRequestTypeDef = TypedDict(
-    "_OptionalListContactsRequestRequestTypeDef",
-    {
-        "groundStation": str,
-        "maxResults": int,
-        "missionProfileArn": str,
-        "nextToken": str,
-        "satelliteArn": str,
-    },
-    total=False,
-)
-
-class ListContactsRequestRequestTypeDef(
-    _RequiredListContactsRequestRequestTypeDef, _OptionalListContactsRequestRequestTypeDef
-):
-    pass
-
 ListDataflowEndpointGroupsRequestRequestTypeDef = TypedDict(
     "ListDataflowEndpointGroupsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-_RequiredListEphemeridesRequestRequestTypeDef = TypedDict(
-    "_RequiredListEphemeridesRequestRequestTypeDef",
-    {
-        "endTime": Union[datetime, str],
-        "satelliteId": str,
-        "startTime": Union[datetime, str],
-    },
-)
-_OptionalListEphemeridesRequestRequestTypeDef = TypedDict(
-    "_OptionalListEphemeridesRequestRequestTypeDef",
-    {
-        "maxResults": int,
-        "nextToken": str,
-        "statusList": Sequence[EphemerisStatusType],
-    },
-    total=False,
-)
-
-class ListEphemeridesRequestRequestTypeDef(
-    _RequiredListEphemeridesRequestRequestTypeDef, _OptionalListEphemeridesRequestRequestTypeDef
-):
-    pass
-
 ListGroundStationsRequestRequestTypeDef = TypedDict(
     "ListGroundStationsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "satelliteId": str,
     },
@@ -678,45 +633,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-_RequiredReserveContactRequestRequestTypeDef = TypedDict(
-    "_RequiredReserveContactRequestRequestTypeDef",
-    {
-        "endTime": Union[datetime, str],
-        "groundStation": str,
-        "missionProfileArn": str,
-        "satelliteArn": str,
-        "startTime": Union[datetime, str],
-    },
-)
-_OptionalReserveContactRequestRequestTypeDef = TypedDict(
-    "_OptionalReserveContactRequestRequestTypeDef",
-    {
-        "tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-class ReserveContactRequestRequestTypeDef(
-    _RequiredReserveContactRequestRequestTypeDef, _OptionalReserveContactRequestRequestTypeDef
-):
-    pass
-
-TimeRangeTypeDef = TypedDict(
-    "TimeRangeTypeDef",
-    {
-        "endTime": Union[datetime, str],
-        "startTime": Union[datetime, str],
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -923,14 +847,93 @@
         "satelliteArn": str,
         "startTime": datetime,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
+_RequiredListContactsRequestRequestTypeDef = TypedDict(
+    "_RequiredListContactsRequestRequestTypeDef",
+    {
+        "endTime": TimestampTypeDef,
+        "startTime": TimestampTypeDef,
+        "statusList": Sequence[ContactStatusType],
+    },
+)
+_OptionalListContactsRequestRequestTypeDef = TypedDict(
+    "_OptionalListContactsRequestRequestTypeDef",
+    {
+        "groundStation": str,
+        "maxResults": int,
+        "missionProfileArn": str,
+        "nextToken": str,
+        "satelliteArn": str,
+    },
+    total=False,
+)
+
+class ListContactsRequestRequestTypeDef(
+    _RequiredListContactsRequestRequestTypeDef, _OptionalListContactsRequestRequestTypeDef
+):
+    pass
+
+_RequiredListEphemeridesRequestRequestTypeDef = TypedDict(
+    "_RequiredListEphemeridesRequestRequestTypeDef",
+    {
+        "endTime": TimestampTypeDef,
+        "satelliteId": str,
+        "startTime": TimestampTypeDef,
+    },
+)
+_OptionalListEphemeridesRequestRequestTypeDef = TypedDict(
+    "_OptionalListEphemeridesRequestRequestTypeDef",
+    {
+        "maxResults": int,
+        "nextToken": str,
+        "statusList": Sequence[EphemerisStatusType],
+    },
+    total=False,
+)
+
+class ListEphemeridesRequestRequestTypeDef(
+    _RequiredListEphemeridesRequestRequestTypeDef, _OptionalListEphemeridesRequestRequestTypeDef
+):
+    pass
+
+_RequiredReserveContactRequestRequestTypeDef = TypedDict(
+    "_RequiredReserveContactRequestRequestTypeDef",
+    {
+        "endTime": TimestampTypeDef,
+        "groundStation": str,
+        "missionProfileArn": str,
+        "satelliteArn": str,
+        "startTime": TimestampTypeDef,
+    },
+)
+_OptionalReserveContactRequestRequestTypeDef = TypedDict(
+    "_OptionalReserveContactRequestRequestTypeDef",
+    {
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+class ReserveContactRequestRequestTypeDef(
+    _RequiredReserveContactRequestRequestTypeDef, _OptionalReserveContactRequestRequestTypeDef
+):
+    pass
+
+TimeRangeTypeDef = TypedDict(
+    "TimeRangeTypeDef",
+    {
+        "endTime": TimestampTypeDef,
+        "startTime": TimestampTypeDef,
+    },
+)
+
 _RequiredCreateMissionProfileRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMissionProfileRequestRequestTypeDef",
     {
         "dataflowEdges": Sequence[Sequence[str]],
         "minimumViableContactDurationSeconds": int,
         "name": str,
         "trackingConfigArn": str,
@@ -1146,16 +1149,16 @@
     },
     total=False,
 )
 
 _RequiredListContactsRequestListContactsPaginateTypeDef = TypedDict(
     "_RequiredListContactsRequestListContactsPaginateTypeDef",
     {
-        "endTime": Union[datetime, str],
-        "startTime": Union[datetime, str],
+        "endTime": TimestampTypeDef,
+        "startTime": TimestampTypeDef,
         "statusList": Sequence[ContactStatusType],
     },
 )
 _OptionalListContactsRequestListContactsPaginateTypeDef = TypedDict(
     "_OptionalListContactsRequestListContactsPaginateTypeDef",
     {
         "groundStation": str,
@@ -1179,17 +1182,17 @@
     },
     total=False,
 )
 
 _RequiredListEphemeridesRequestListEphemeridesPaginateTypeDef = TypedDict(
     "_RequiredListEphemeridesRequestListEphemeridesPaginateTypeDef",
     {
-        "endTime": Union[datetime, str],
+        "endTime": TimestampTypeDef,
         "satelliteId": str,
-        "startTime": Union[datetime, str],
+        "startTime": TimestampTypeDef,
     },
 )
 _OptionalListEphemeridesRequestListEphemeridesPaginateTypeDef = TypedDict(
     "_OptionalListEphemeridesRequestListEphemeridesPaginateTypeDef",
     {
         "statusList": Sequence[EphemerisStatusType],
         "PaginationConfig": PaginatorConfigTypeDef,
@@ -1233,23 +1236,14 @@
     {
         "missionProfileList": List[MissionProfileListItemTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TLEDataTypeDef = TypedDict(
-    "TLEDataTypeDef",
-    {
-        "tleLine1": str,
-        "tleLine2": str,
-        "validTimeRange": TimeRangeTypeDef,
-    },
-)
-
 RegisterAgentRequestRequestTypeDef = TypedDict(
     "RegisterAgentRequestRequestTypeDef",
     {
         "agentDetails": AgentDetailsTypeDef,
         "discoveryData": DiscoveryDataTypeDef,
     },
 )
@@ -1259,14 +1253,23 @@
     {
         "contactList": List[ContactDataTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+TLEDataTypeDef = TypedDict(
+    "TLEDataTypeDef",
+    {
+        "tleLine1": str,
+        "tleLine2": str,
+        "validTimeRange": TimeRangeTypeDef,
+    },
+)
+
 EphemerisTypeDescriptionTypeDef = TypedDict(
     "EphemerisTypeDescriptionTypeDef",
     {
         "oem": EphemerisDescriptionTypeDef,
         "tle": EphemerisDescriptionTypeDef,
     },
     total=False,
@@ -1491,15 +1494,15 @@
     },
 )
 _OptionalCreateEphemerisRequestRequestTypeDef = TypedDict(
     "_OptionalCreateEphemerisRequestRequestTypeDef",
     {
         "enabled": bool,
         "ephemeris": EphemerisDataTypeDef,
-        "expirationTime": Union[datetime, str],
+        "expirationTime": TimestampTypeDef,
         "kmsKeyArn": str,
         "priority": int,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
@@ -1527,36 +1530,15 @@
         "dataflowEndpointGroupId": str,
         "endpointsDetails": List[EndpointDetailsOutputTypeDef],
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateDataflowEndpointGroupRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateDataflowEndpointGroupRequestRequestTypeDef",
-    {
-        "endpointDetails": Sequence[Union[EndpointDetailsTypeDef, EndpointDetailsOutputTypeDef]],
-    },
-)
-_OptionalCreateDataflowEndpointGroupRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateDataflowEndpointGroupRequestRequestTypeDef",
-    {
-        "contactPostPassDurationSeconds": int,
-        "contactPrePassDurationSeconds": int,
-        "tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-class CreateDataflowEndpointGroupRequestRequestTypeDef(
-    _RequiredCreateDataflowEndpointGroupRequestRequestTypeDef,
-    _OptionalCreateDataflowEndpointGroupRequestRequestTypeDef,
-):
-    pass
-
+EndpointDetailsUnionTypeDef = Union[EndpointDetailsTypeDef, EndpointDetailsOutputTypeDef]
 DestinationTypeDef = TypedDict(
     "DestinationTypeDef",
     {
         "configDetails": ConfigDetailsTypeDef,
         "configId": str,
         "configType": ConfigCapabilityTypeType,
         "dataflowDestinationRegion": str,
@@ -1571,14 +1553,36 @@
         "configId": str,
         "configType": ConfigCapabilityTypeType,
         "dataflowSourceRegion": str,
     },
     total=False,
 )
 
+_RequiredCreateDataflowEndpointGroupRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDataflowEndpointGroupRequestRequestTypeDef",
+    {
+        "endpointDetails": Sequence[EndpointDetailsUnionTypeDef],
+    },
+)
+_OptionalCreateDataflowEndpointGroupRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDataflowEndpointGroupRequestRequestTypeDef",
+    {
+        "contactPostPassDurationSeconds": int,
+        "contactPrePassDurationSeconds": int,
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+class CreateDataflowEndpointGroupRequestRequestTypeDef(
+    _RequiredCreateDataflowEndpointGroupRequestRequestTypeDef,
+    _OptionalCreateDataflowEndpointGroupRequestRequestTypeDef,
+):
+    pass
+
 DataflowDetailTypeDef = TypedDict(
     "DataflowDetailTypeDef",
     {
         "destination": DestinationTypeDef,
         "errorMessage": str,
         "source": SourceTypeDef,
     },
```

### Comparing `mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation/waiter.py` & `mypy-boto3-groundstation-1.28.16/mypy_boto3_groundstation/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation/waiter.pyi` & `mypy-boto3-groundstation-1.28.16/mypy_boto3_groundstation/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation.egg-info/PKG-INFO` & `mypy-boto3-groundstation-1.28.16/mypy_boto3_groundstation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-groundstation
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.GroundStation 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.GroundStation 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 groundstation type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 groundstation type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-groundstation.svg?color=blue)](https://pypi.org/project/mypy-boto3-groundstation)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-groundstation)](https://pepy.tech/project/mypy-boto3-groundstation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GroundStation 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation)
+[boto3.GroundStation 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation)
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
 [mypy-boto3-groundstation docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/).
 
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
@@ -375,20 +375,20 @@
 )
 
 
 def check_value(value: AgentStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_groundstation.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_groundstation.type_defs import (
     ComponentVersionTypeDef,
     AggregateStatusTypeDef,
     AntennaDemodDecodeDetailsTypeDef,
     DecodeConfigTypeDef,
@@ -401,14 +401,15 @@
     ConfigListItemTypeDef,
     DataflowEndpointConfigTypeDef,
     S3RecordingConfigTypeDef,
     TrackingConfigTypeDef,
     UplinkEchoConfigTypeDef,
     SocketAddressTypeDef,
     ElevationTypeDef,
+    TimestampTypeDef,
     KmsKeyTypeDef,
     DataflowEndpointListItemTypeDef,
     DeleteConfigRequestRequestTypeDef,
     DeleteDataflowEndpointGroupRequestRequestTypeDef,
     DeleteEphemerisRequestRequestTypeDef,
     DeleteMissionProfileRequestRequestTypeDef,
     WaiterConfigTypeDef,
@@ -427,24 +428,20 @@
     GetMinuteUsageRequestRequestTypeDef,
     GetMissionProfileRequestRequestTypeDef,
     GetSatelliteRequestRequestTypeDef,
     GroundStationDataTypeDef,
     IntegerRangeTypeDef,
     PaginatorConfigTypeDef,
     ListConfigsRequestRequestTypeDef,
-    ListContactsRequestRequestTypeDef,
     ListDataflowEndpointGroupsRequestRequestTypeDef,
-    ListEphemeridesRequestRequestTypeDef,
     ListGroundStationsRequestRequestTypeDef,
     ListMissionProfilesRequestRequestTypeDef,
     MissionProfileListItemTypeDef,
     ListSatellitesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ReserveContactRequestRequestTypeDef,
-    TimeRangeTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateEphemerisRequestRequestTypeDef,
     AgentDetailsTypeDef,
     UpdateAgentStatusRequestRequestTypeDef,
     ConfigIdResponseTypeDef,
     ContactIdResponseTypeDef,
@@ -456,14 +453,18 @@
     MissionProfileIdResponseTypeDef,
     RegisterAgentResponseTypeDef,
     UpdateAgentStatusResponseTypeDef,
     ListConfigsResponseTypeDef,
     ConnectionDetailsTypeDef,
     DataflowEndpointTypeDef,
     ContactDataTypeDef,
+    ListContactsRequestRequestTypeDef,
+    ListEphemeridesRequestRequestTypeDef,
+    ReserveContactRequestRequestTypeDef,
+    TimeRangeTypeDef,
     CreateMissionProfileRequestRequestTypeDef,
     GetMissionProfileResponseTypeDef,
     UpdateMissionProfileRequestRequestTypeDef,
     ListDataflowEndpointGroupsResponseTypeDef,
     DescribeContactRequestContactScheduledWaitTypeDef,
     EphemerisDescriptionTypeDef,
     EphemerisItemTypeDef,
@@ -478,17 +479,17 @@
     ListContactsRequestListContactsPaginateTypeDef,
     ListDataflowEndpointGroupsRequestListDataflowEndpointGroupsPaginateTypeDef,
     ListEphemeridesRequestListEphemeridesPaginateTypeDef,
     ListGroundStationsRequestListGroundStationsPaginateTypeDef,
     ListMissionProfilesRequestListMissionProfilesPaginateTypeDef,
     ListSatellitesRequestListSatellitesPaginateTypeDef,
     ListMissionProfilesResponseTypeDef,
-    TLEDataTypeDef,
     RegisterAgentRequestRequestTypeDef,
     ListContactsResponseTypeDef,
+    TLEDataTypeDef,
     EphemerisTypeDescriptionTypeDef,
     ListEphemeridesResponseTypeDef,
     ListSatellitesResponseTypeDef,
     AntennaDownlinkConfigTypeDef,
     AntennaDownlinkDemodDecodeConfigTypeDef,
     AntennaUplinkConfigTypeDef,
     RangedConnectionDetailsTypeDef,
@@ -501,23 +502,24 @@
     GetConfigResponseTypeDef,
     UpdateConfigRequestRequestTypeDef,
     EndpointDetailsOutputTypeDef,
     EndpointDetailsTypeDef,
     CreateEphemerisRequestRequestTypeDef,
     ConfigDetailsTypeDef,
     GetDataflowEndpointGroupResponseTypeDef,
-    CreateDataflowEndpointGroupRequestRequestTypeDef,
+    EndpointDetailsUnionTypeDef,
     DestinationTypeDef,
     SourceTypeDef,
+    CreateDataflowEndpointGroupRequestRequestTypeDef,
     DataflowDetailTypeDef,
     DescribeContactResponseTypeDef,
 )
 
 
-def get_structure() -> ComponentVersionTypeDef:
+def get_value() -> ComponentVersionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation.egg-info/SOURCES.txt` & `mypy-boto3-groundstation-1.28.16/mypy_boto3_groundstation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-groundstation-1.28.15.post1/setup.py` & `mypy-boto3-groundstation-1.28.16/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-groundstation",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_groundstation"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.GroundStation 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.GroundStation 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 groundstation type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 groundstation type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_groundstation": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

