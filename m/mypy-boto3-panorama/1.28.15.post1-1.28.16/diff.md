# Comparing `tmp/mypy-boto3-panorama-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-panorama-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-panorama-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:50 2023, max compression
+gzip compressed data, was "mypy-boto3-panorama-1.28.16.tar", last modified: Tue Aug  1 11:37:30 2023, max compression
```

## Comparing `mypy-boto3-panorama-1.28.15.post1.tar` & `mypy-boto3-panorama-1.28.16.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:50.865328 mypy-boto3-panorama-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:52:49.000000 mypy-boto3-panorama-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16584 2023-07-29 10:03:50.861328 mypy-boto3-panorama-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15087 2023-07-29 09:52:49.000000 mypy-boto3-panorama-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:50.853328 mypy-boto3-panorama-1.28.15.post1/mypy_boto3_panorama/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-29 09:52:49.000000 mypy-boto3-panorama-1.28.15.post1/mypy_boto3_panorama/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-29 09:52:49.000000 mypy-boto3-panorama-1.28.15.post1/mypy_boto3_panorama/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-29 09:52:49.000000 mypy-boto3-panorama-1.28.15.post1/mypy_boto3_panorama/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23959 2023-07-29 09:52:50.000000 mypy-boto3-panorama-1.28.15.post1/mypy_boto3_panorama/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    23918 2023-07-29 09:52:50.000000 mypy-boto3-panorama-1.28.15.post1/mypy_boto3_panorama/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11041 2023-07-29 09:52:50.000000 mypy-boto3-panorama-1.28.15.post1/mypy_boto3_panorama/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11039 2023-07-29 09:52:50.000000 mypy-boto3-panorama-1.28.15.post1/mypy_boto3_panorama/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:52:49.000000 mypy-boto3-panorama-1.28.15.post1/mypy_boto3_panorama/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    38825 2023-07-29 09:52:51.000000 mypy-boto3-panorama-1.28.15.post1/mypy_boto3_panorama/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    38782 2023-07-29 09:52:50.000000 mypy-boto3-panorama-1.28.15.post1/mypy_boto3_panorama/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:52:49.000000 mypy-boto3-panorama-1.28.15.post1/mypy_boto3_panorama/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:50.861328 mypy-boto3-panorama-1.28.15.post1/mypy_boto3_panorama.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16584 2023-07-29 10:03:50.000000 mypy-boto3-panorama-1.28.15.post1/mypy_boto3_panorama.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-29 10:03:50.000000 mypy-boto3-panorama-1.28.15.post1/mypy_boto3_panorama.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:50.000000 mypy-boto3-panorama-1.28.15.post1/mypy_boto3_panorama.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:50.000000 mypy-boto3-panorama-1.28.15.post1/mypy_boto3_panorama.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:50.000000 mypy-boto3-panorama-1.28.15.post1/mypy_boto3_panorama.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-29 10:03:50.000000 mypy-boto3-panorama-1.28.15.post1/mypy_boto3_panorama.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:50.865328 mypy-boto3-panorama-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-29 09:52:49.000000 mypy-boto3-panorama-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:30.836795 mypy-boto3-panorama-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:25:48.000000 mypy-boto3-panorama-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16639 2023-08-01 11:37:30.820795 mypy-boto3-panorama-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15151 2023-08-01 11:25:48.000000 mypy-boto3-panorama-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:30.820795 mypy-boto3-panorama-1.28.16/mypy_boto3_panorama/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-08-01 11:25:48.000000 mypy-boto3-panorama-1.28.16/mypy_boto3_panorama/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-08-01 11:25:48.000000 mypy-boto3-panorama-1.28.16/mypy_boto3_panorama/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-08-01 11:25:48.000000 mypy-boto3-panorama-1.28.16/mypy_boto3_panorama/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23800 2023-08-01 11:25:51.000000 mypy-boto3-panorama-1.28.16/mypy_boto3_panorama/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23759 2023-08-01 11:25:48.000000 mypy-boto3-panorama-1.28.16/mypy_boto3_panorama/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11041 2023-08-01 11:25:51.000000 mypy-boto3-panorama-1.28.16/mypy_boto3_panorama/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11039 2023-08-01 11:25:51.000000 mypy-boto3-panorama-1.28.16/mypy_boto3_panorama/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:25:48.000000 mypy-boto3-panorama-1.28.16/mypy_boto3_panorama/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    39005 2023-08-01 11:25:52.000000 mypy-boto3-panorama-1.28.16/mypy_boto3_panorama/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38962 2023-08-01 11:25:52.000000 mypy-boto3-panorama-1.28.16/mypy_boto3_panorama/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:25:48.000000 mypy-boto3-panorama-1.28.16/mypy_boto3_panorama/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:30.820795 mypy-boto3-panorama-1.28.16/mypy_boto3_panorama.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16639 2023-08-01 11:37:30.000000 mypy-boto3-panorama-1.28.16/mypy_boto3_panorama.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-08-01 11:37:30.000000 mypy-boto3-panorama-1.28.16/mypy_boto3_panorama.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:30.000000 mypy-boto3-panorama-1.28.16/mypy_boto3_panorama.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:30.000000 mypy-boto3-panorama-1.28.16/mypy_boto3_panorama.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:30.000000 mypy-boto3-panorama-1.28.16/mypy_boto3_panorama.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-01 11:37:30.000000 mypy-boto3-panorama-1.28.16/mypy_boto3_panorama.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:30.836795 mypy-boto3-panorama-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-08-01 11:25:48.000000 mypy-boto3-panorama-1.28.16/setup.py
```

### Comparing `mypy-boto3-panorama-1.28.15.post1/LICENSE` & `mypy-boto3-panorama-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-panorama-1.28.15.post1/PKG-INFO` & `mypy-boto3-panorama-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-panorama
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Panorama 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.Panorama 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_panorama/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 panorama type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 panorama type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-panorama.svg?color=blue)](https://pypi.org/project/mypy-boto3-panorama)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_panorama/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-panorama)](https://pepy.tech/project/mypy-boto3-panorama)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Panorama 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama)
+[boto3.Panorama 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama)
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
 [mypy-boto3-panorama docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_panorama/).
 
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
@@ -311,51 +311,51 @@
 )
 
 
 def check_value(value: ApplicationInstanceHealthStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_panorama.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_panorama.type_defs import (
     AlternateSoftwareMetadataTypeDef,
     ReportedRuntimeContextStateTypeDef,
     ManifestOverridesPayloadTypeDef,
     ManifestPayloadTypeDef,
     ResponseMetadataTypeDef,
     JobTypeDef,
-    JobResourceTagsOutputTypeDef,
-    JobResourceTagsTypeDef,
     CreatePackageRequestRequestTypeDef,
     StorageLocationTypeDef,
     DeleteDeviceRequestRequestTypeDef,
     DeletePackageRequestRequestTypeDef,
     DeregisterPackageVersionRequestRequestTypeDef,
     DescribeApplicationInstanceDetailsRequestRequestTypeDef,
     DescribeApplicationInstanceRequestRequestTypeDef,
     DescribeDeviceJobRequestRequestTypeDef,
     DescribeDeviceRequestRequestTypeDef,
     LatestDeviceJobTypeDef,
     DescribeNodeFromTemplateJobRequestRequestTypeDef,
+    JobResourceTagsOutputTypeDef,
     DescribeNodeRequestRequestTypeDef,
     DescribePackageImportJobRequestRequestTypeDef,
     DescribePackageRequestRequestTypeDef,
     DescribePackageVersionRequestRequestTypeDef,
     OTAJobConfigTypeDef,
     DeviceJobTypeDef,
     StaticIpConnectionInfoOutputTypeDef,
     StaticIpConnectionInfoTypeDef,
     EthernetStatusTypeDef,
+    JobResourceTagsTypeDef,
     ListApplicationInstanceDependenciesRequestRequestTypeDef,
     PackageObjectTypeDef,
     ListApplicationInstanceNodeInstancesRequestRequestTypeDef,
     NodeInstanceTypeDef,
     ListApplicationInstancesRequestRequestTypeDef,
     ListDevicesJobsRequestRequestTypeDef,
     ListDevicesRequestRequestTypeDef,
@@ -393,23 +393,23 @@
     DescribeDeviceJobResponseTypeDef,
     DescribePackageVersionResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ProvisionDeviceResponseTypeDef,
     SignalApplicationInstanceNodeInstancesResponseTypeDef,
     UpdateDeviceMetadataResponseTypeDef,
     CreateJobForDevicesResponseTypeDef,
-    DescribeNodeFromTemplateJobResponseTypeDef,
-    CreateNodeFromTemplateJobRequestRequestTypeDef,
     CreatePackageResponseTypeDef,
     DescribePackageResponseTypeDef,
     DeviceTypeDef,
+    DescribeNodeFromTemplateJobResponseTypeDef,
     DeviceJobConfigTypeDef,
     ListDevicesJobsResponseTypeDef,
     EthernetPayloadOutputTypeDef,
     EthernetPayloadTypeDef,
+    JobResourceTagsUnionTypeDef,
     ListApplicationInstanceDependenciesResponseTypeDef,
     ListApplicationInstanceNodeInstancesResponseTypeDef,
     ListNodeFromTemplateJobsResponseTypeDef,
     ListNodesResponseTypeDef,
     ListPackageImportJobsResponseTypeDef,
     ListPackagesResponseTypeDef,
     NetworkStatusTypeDef,
@@ -419,24 +419,26 @@
     PackageImportJobOutputConfigTypeDef,
     PackageVersionInputConfigTypeDef,
     ListApplicationInstancesResponseTypeDef,
     ListDevicesResponseTypeDef,
     CreateJobForDevicesRequestRequestTypeDef,
     NetworkPayloadOutputTypeDef,
     NetworkPayloadTypeDef,
+    CreateNodeFromTemplateJobRequestRequestTypeDef,
     DescribeNodeResponseTypeDef,
     PackageImportJobInputConfigTypeDef,
     DescribeDeviceResponseTypeDef,
+    NetworkPayloadUnionTypeDef,
     ProvisionDeviceRequestRequestTypeDef,
     CreatePackageImportJobRequestRequestTypeDef,
     DescribePackageImportJobResponseTypeDef,
 )
 
 
-def get_structure() -> AlternateSoftwareMetadataTypeDef:
+def get_value() -> AlternateSoftwareMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-panorama-1.28.15.post1/README.md` & `mypy-boto3-panorama-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-panorama.svg?color=blue)](https://pypi.org/project/mypy-boto3-panorama)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_panorama/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-panorama)](https://pepy.tech/project/mypy-boto3-panorama)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Panorama 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama)
+[boto3.Panorama 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama)
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
 [mypy-boto3-panorama docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_panorama/).
 
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
@@ -279,51 +279,51 @@
 )
 
 
 def check_value(value: ApplicationInstanceHealthStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_panorama.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_panorama.type_defs import (
     AlternateSoftwareMetadataTypeDef,
     ReportedRuntimeContextStateTypeDef,
     ManifestOverridesPayloadTypeDef,
     ManifestPayloadTypeDef,
     ResponseMetadataTypeDef,
     JobTypeDef,
-    JobResourceTagsOutputTypeDef,
-    JobResourceTagsTypeDef,
     CreatePackageRequestRequestTypeDef,
     StorageLocationTypeDef,
     DeleteDeviceRequestRequestTypeDef,
     DeletePackageRequestRequestTypeDef,
     DeregisterPackageVersionRequestRequestTypeDef,
     DescribeApplicationInstanceDetailsRequestRequestTypeDef,
     DescribeApplicationInstanceRequestRequestTypeDef,
     DescribeDeviceJobRequestRequestTypeDef,
     DescribeDeviceRequestRequestTypeDef,
     LatestDeviceJobTypeDef,
     DescribeNodeFromTemplateJobRequestRequestTypeDef,
+    JobResourceTagsOutputTypeDef,
     DescribeNodeRequestRequestTypeDef,
     DescribePackageImportJobRequestRequestTypeDef,
     DescribePackageRequestRequestTypeDef,
     DescribePackageVersionRequestRequestTypeDef,
     OTAJobConfigTypeDef,
     DeviceJobTypeDef,
     StaticIpConnectionInfoOutputTypeDef,
     StaticIpConnectionInfoTypeDef,
     EthernetStatusTypeDef,
+    JobResourceTagsTypeDef,
     ListApplicationInstanceDependenciesRequestRequestTypeDef,
     PackageObjectTypeDef,
     ListApplicationInstanceNodeInstancesRequestRequestTypeDef,
     NodeInstanceTypeDef,
     ListApplicationInstancesRequestRequestTypeDef,
     ListDevicesJobsRequestRequestTypeDef,
     ListDevicesRequestRequestTypeDef,
@@ -361,23 +361,23 @@
     DescribeDeviceJobResponseTypeDef,
     DescribePackageVersionResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ProvisionDeviceResponseTypeDef,
     SignalApplicationInstanceNodeInstancesResponseTypeDef,
     UpdateDeviceMetadataResponseTypeDef,
     CreateJobForDevicesResponseTypeDef,
-    DescribeNodeFromTemplateJobResponseTypeDef,
-    CreateNodeFromTemplateJobRequestRequestTypeDef,
     CreatePackageResponseTypeDef,
     DescribePackageResponseTypeDef,
     DeviceTypeDef,
+    DescribeNodeFromTemplateJobResponseTypeDef,
     DeviceJobConfigTypeDef,
     ListDevicesJobsResponseTypeDef,
     EthernetPayloadOutputTypeDef,
     EthernetPayloadTypeDef,
+    JobResourceTagsUnionTypeDef,
     ListApplicationInstanceDependenciesResponseTypeDef,
     ListApplicationInstanceNodeInstancesResponseTypeDef,
     ListNodeFromTemplateJobsResponseTypeDef,
     ListNodesResponseTypeDef,
     ListPackageImportJobsResponseTypeDef,
     ListPackagesResponseTypeDef,
     NetworkStatusTypeDef,
@@ -387,24 +387,26 @@
     PackageImportJobOutputConfigTypeDef,
     PackageVersionInputConfigTypeDef,
     ListApplicationInstancesResponseTypeDef,
     ListDevicesResponseTypeDef,
     CreateJobForDevicesRequestRequestTypeDef,
     NetworkPayloadOutputTypeDef,
     NetworkPayloadTypeDef,
+    CreateNodeFromTemplateJobRequestRequestTypeDef,
     DescribeNodeResponseTypeDef,
     PackageImportJobInputConfigTypeDef,
     DescribeDeviceResponseTypeDef,
+    NetworkPayloadUnionTypeDef,
     ProvisionDeviceRequestRequestTypeDef,
     CreatePackageImportJobRequestRequestTypeDef,
     DescribePackageImportJobResponseTypeDef,
 )
 
 
-def get_structure() -> AlternateSoftwareMetadataTypeDef:
+def get_value() -> AlternateSoftwareMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-panorama-1.28.15.post1/mypy_boto3_panorama/__main__.py` & `mypy-boto3-panorama-1.28.16/mypy_boto3_panorama/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Panorama 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.Panorama 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_panorama//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama\nOther"
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

### Comparing `mypy-boto3-panorama-1.28.15.post1/mypy_boto3_panorama/client.py` & `mypy-boto3-panorama-1.28.16/mypy_boto3_panorama/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_panorama.client import PanoramaClient
 
     session = Session()
     client: PanoramaClient = session.client("panorama")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     DeviceAggregatedStatusType,
     JobTypeType,
     ListDevicesSortByType,
@@ -40,30 +40,28 @@
     DescribeDeviceResponseTypeDef,
     DescribeNodeFromTemplateJobResponseTypeDef,
     DescribeNodeResponseTypeDef,
     DescribePackageImportJobResponseTypeDef,
     DescribePackageResponseTypeDef,
     DescribePackageVersionResponseTypeDef,
     DeviceJobConfigTypeDef,
-    JobResourceTagsOutputTypeDef,
-    JobResourceTagsTypeDef,
+    JobResourceTagsUnionTypeDef,
     ListApplicationInstanceDependenciesResponseTypeDef,
     ListApplicationInstanceNodeInstancesResponseTypeDef,
     ListApplicationInstancesResponseTypeDef,
     ListDevicesJobsResponseTypeDef,
     ListDevicesResponseTypeDef,
     ListNodeFromTemplateJobsResponseTypeDef,
     ListNodesResponseTypeDef,
     ListPackageImportJobsResponseTypeDef,
     ListPackagesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ManifestOverridesPayloadTypeDef,
     ManifestPayloadTypeDef,
-    NetworkPayloadOutputTypeDef,
-    NetworkPayloadTypeDef,
+    NetworkPayloadUnionTypeDef,
     NodeSignalTypeDef,
     PackageImportJobInputConfigTypeDef,
     PackageImportJobOutputConfigTypeDef,
     ProvisionDeviceResponseTypeDef,
     SignalApplicationInstanceNodeInstancesResponseTypeDef,
     UpdateDeviceMetadataResponseTypeDef,
 )
@@ -165,15 +163,15 @@
         self,
         *,
         NodeName: str,
         OutputPackageName: str,
         OutputPackageVersion: str,
         TemplateParameters: Mapping[str, str],
         TemplateType: Literal["RTSP_CAMERA_STREAM"],
-        JobTags: Sequence[Union[JobResourceTagsTypeDef, JobResourceTagsOutputTypeDef]] = ...,
+        JobTags: Sequence[JobResourceTagsUnionTypeDef] = ...,
         NodeDescription: str = ...
     ) -> CreateNodeFromTemplateJobResponseTypeDef:
         """
         Creates a camera stream node.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.create_node_from_template_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_panorama/client/#create_node_from_template_job)
@@ -192,15 +190,15 @@
     def create_package_import_job(
         self,
         *,
         ClientToken: str,
         InputConfig: PackageImportJobInputConfigTypeDef,
         JobType: PackageImportJobTypeType,
         OutputConfig: PackageImportJobOutputConfigTypeDef,
-        JobTags: Sequence[Union[JobResourceTagsTypeDef, JobResourceTagsOutputTypeDef]] = ...
+        JobTags: Sequence[JobResourceTagsUnionTypeDef] = ...
     ) -> CreatePackageImportJobResponseTypeDef:
         """
         Imports a node package.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.create_package_import_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_panorama/client/#create_package_import_job)
         """
@@ -455,15 +453,15 @@
         """
 
     def provision_device(
         self,
         *,
         Name: str,
         Description: str = ...,
-        NetworkingConfiguration: Union[NetworkPayloadTypeDef, NetworkPayloadOutputTypeDef] = ...,
+        NetworkingConfiguration: NetworkPayloadUnionTypeDef = ...,
         Tags: Mapping[str, str] = ...
     ) -> ProvisionDeviceResponseTypeDef:
         """
         Creates a device and returns a configuration archive.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.provision_device)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_panorama/client/#provision_device)
```

### Comparing `mypy-boto3-panorama-1.28.15.post1/mypy_boto3_panorama/client.pyi` & `mypy-boto3-panorama-1.28.16/mypy_boto3_panorama/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_panorama.client import PanoramaClient
 
     session = Session()
     client: PanoramaClient = session.client("panorama")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     DeviceAggregatedStatusType,
     JobTypeType,
     ListDevicesSortByType,
@@ -40,30 +40,28 @@
     DescribeDeviceResponseTypeDef,
     DescribeNodeFromTemplateJobResponseTypeDef,
     DescribeNodeResponseTypeDef,
     DescribePackageImportJobResponseTypeDef,
     DescribePackageResponseTypeDef,
     DescribePackageVersionResponseTypeDef,
     DeviceJobConfigTypeDef,
-    JobResourceTagsOutputTypeDef,
-    JobResourceTagsTypeDef,
+    JobResourceTagsUnionTypeDef,
     ListApplicationInstanceDependenciesResponseTypeDef,
     ListApplicationInstanceNodeInstancesResponseTypeDef,
     ListApplicationInstancesResponseTypeDef,
     ListDevicesJobsResponseTypeDef,
     ListDevicesResponseTypeDef,
     ListNodeFromTemplateJobsResponseTypeDef,
     ListNodesResponseTypeDef,
     ListPackageImportJobsResponseTypeDef,
     ListPackagesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ManifestOverridesPayloadTypeDef,
     ManifestPayloadTypeDef,
-    NetworkPayloadOutputTypeDef,
-    NetworkPayloadTypeDef,
+    NetworkPayloadUnionTypeDef,
     NodeSignalTypeDef,
     PackageImportJobInputConfigTypeDef,
     PackageImportJobOutputConfigTypeDef,
     ProvisionDeviceResponseTypeDef,
     SignalApplicationInstanceNodeInstancesResponseTypeDef,
     UpdateDeviceMetadataResponseTypeDef,
 )
@@ -156,15 +154,15 @@
         self,
         *,
         NodeName: str,
         OutputPackageName: str,
         OutputPackageVersion: str,
         TemplateParameters: Mapping[str, str],
         TemplateType: Literal["RTSP_CAMERA_STREAM"],
-        JobTags: Sequence[Union[JobResourceTagsTypeDef, JobResourceTagsOutputTypeDef]] = ...,
+        JobTags: Sequence[JobResourceTagsUnionTypeDef] = ...,
         NodeDescription: str = ...
     ) -> CreateNodeFromTemplateJobResponseTypeDef:
         """
         Creates a camera stream node.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.create_node_from_template_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_panorama/client/#create_node_from_template_job)
@@ -181,15 +179,15 @@
     def create_package_import_job(
         self,
         *,
         ClientToken: str,
         InputConfig: PackageImportJobInputConfigTypeDef,
         JobType: PackageImportJobTypeType,
         OutputConfig: PackageImportJobOutputConfigTypeDef,
-        JobTags: Sequence[Union[JobResourceTagsTypeDef, JobResourceTagsOutputTypeDef]] = ...
+        JobTags: Sequence[JobResourceTagsUnionTypeDef] = ...
     ) -> CreatePackageImportJobResponseTypeDef:
         """
         Imports a node package.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.create_package_import_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_panorama/client/#create_package_import_job)
         """
@@ -420,15 +418,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_panorama/client/#list_tags_for_resource)
         """
     def provision_device(
         self,
         *,
         Name: str,
         Description: str = ...,
-        NetworkingConfiguration: Union[NetworkPayloadTypeDef, NetworkPayloadOutputTypeDef] = ...,
+        NetworkingConfiguration: NetworkPayloadUnionTypeDef = ...,
         Tags: Mapping[str, str] = ...
     ) -> ProvisionDeviceResponseTypeDef:
         """
         Creates a device and returns a configuration archive.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.provision_device)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_panorama/client/#provision_device)
```

### Comparing `mypy-boto3-panorama-1.28.15.post1/mypy_boto3_panorama/literals.py` & `mypy-boto3-panorama-1.28.16/mypy_boto3_panorama/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-panorama-1.28.15.post1/mypy_boto3_panorama/literals.pyi` & `mypy-boto3-panorama-1.28.16/mypy_boto3_panorama/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-panorama-1.28.15.post1/mypy_boto3_panorama/type_defs.py` & `mypy-boto3-panorama-1.28.16/mypy_boto3_panorama/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_panorama/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_panorama.type_defs import AlternateSoftwareMetadataTypeDef
 
-    data: AlternateSoftwareMetadataTypeDef = {...}
+    data: AlternateSoftwareMetadataTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -47,44 +47,43 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AlternateSoftwareMetadataTypeDef",
     "ReportedRuntimeContextStateTypeDef",
     "ManifestOverridesPayloadTypeDef",
     "ManifestPayloadTypeDef",
     "ResponseMetadataTypeDef",
     "JobTypeDef",
-    "JobResourceTagsOutputTypeDef",
-    "JobResourceTagsTypeDef",
     "CreatePackageRequestRequestTypeDef",
     "StorageLocationTypeDef",
     "DeleteDeviceRequestRequestTypeDef",
     "DeletePackageRequestRequestTypeDef",
     "DeregisterPackageVersionRequestRequestTypeDef",
     "DescribeApplicationInstanceDetailsRequestRequestTypeDef",
     "DescribeApplicationInstanceRequestRequestTypeDef",
     "DescribeDeviceJobRequestRequestTypeDef",
     "DescribeDeviceRequestRequestTypeDef",
     "LatestDeviceJobTypeDef",
     "DescribeNodeFromTemplateJobRequestRequestTypeDef",
+    "JobResourceTagsOutputTypeDef",
     "DescribeNodeRequestRequestTypeDef",
     "DescribePackageImportJobRequestRequestTypeDef",
     "DescribePackageRequestRequestTypeDef",
     "DescribePackageVersionRequestRequestTypeDef",
     "OTAJobConfigTypeDef",
     "DeviceJobTypeDef",
     "StaticIpConnectionInfoOutputTypeDef",
     "StaticIpConnectionInfoTypeDef",
     "EthernetStatusTypeDef",
+    "JobResourceTagsTypeDef",
     "ListApplicationInstanceDependenciesRequestRequestTypeDef",
     "PackageObjectTypeDef",
     "ListApplicationInstanceNodeInstancesRequestRequestTypeDef",
     "NodeInstanceTypeDef",
     "ListApplicationInstancesRequestRequestTypeDef",
     "ListDevicesJobsRequestRequestTypeDef",
     "ListDevicesRequestRequestTypeDef",
@@ -122,23 +121,23 @@
     "DescribeDeviceJobResponseTypeDef",
     "DescribePackageVersionResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "ProvisionDeviceResponseTypeDef",
     "SignalApplicationInstanceNodeInstancesResponseTypeDef",
     "UpdateDeviceMetadataResponseTypeDef",
     "CreateJobForDevicesResponseTypeDef",
-    "DescribeNodeFromTemplateJobResponseTypeDef",
-    "CreateNodeFromTemplateJobRequestRequestTypeDef",
     "CreatePackageResponseTypeDef",
     "DescribePackageResponseTypeDef",
     "DeviceTypeDef",
+    "DescribeNodeFromTemplateJobResponseTypeDef",
     "DeviceJobConfigTypeDef",
     "ListDevicesJobsResponseTypeDef",
     "EthernetPayloadOutputTypeDef",
     "EthernetPayloadTypeDef",
+    "JobResourceTagsUnionTypeDef",
     "ListApplicationInstanceDependenciesResponseTypeDef",
     "ListApplicationInstanceNodeInstancesResponseTypeDef",
     "ListNodeFromTemplateJobsResponseTypeDef",
     "ListNodesResponseTypeDef",
     "ListPackageImportJobsResponseTypeDef",
     "ListPackagesResponseTypeDef",
     "NetworkStatusTypeDef",
@@ -148,17 +147,19 @@
     "PackageImportJobOutputConfigTypeDef",
     "PackageVersionInputConfigTypeDef",
     "ListApplicationInstancesResponseTypeDef",
     "ListDevicesResponseTypeDef",
     "CreateJobForDevicesRequestRequestTypeDef",
     "NetworkPayloadOutputTypeDef",
     "NetworkPayloadTypeDef",
+    "CreateNodeFromTemplateJobRequestRequestTypeDef",
     "DescribeNodeResponseTypeDef",
     "PackageImportJobInputConfigTypeDef",
     "DescribeDeviceResponseTypeDef",
+    "NetworkPayloadUnionTypeDef",
     "ProvisionDeviceRequestRequestTypeDef",
     "CreatePackageImportJobRequestRequestTypeDef",
     "DescribePackageImportJobResponseTypeDef",
 )
 
 AlternateSoftwareMetadataTypeDef = TypedDict(
     "AlternateSoftwareMetadataTypeDef",
@@ -210,51 +211,33 @@
     {
         "DeviceId": str,
         "JobId": str,
     },
     total=False,
 )
 
-JobResourceTagsOutputTypeDef = TypedDict(
-    "JobResourceTagsOutputTypeDef",
-    {
-        "ResourceType": Literal["PACKAGE"],
-        "Tags": Dict[str, str],
-    },
-)
-
-JobResourceTagsTypeDef = TypedDict(
-    "JobResourceTagsTypeDef",
-    {
-        "ResourceType": Literal["PACKAGE"],
-        "Tags": Mapping[str, str],
-    },
-)
-
 _RequiredCreatePackageRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePackageRequestRequestTypeDef",
     {
         "PackageName": str,
     },
 )
 _OptionalCreatePackageRequestRequestTypeDef = TypedDict(
     "_OptionalCreatePackageRequestRequestTypeDef",
     {
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreatePackageRequestRequestTypeDef(
     _RequiredCreatePackageRequestRequestTypeDef, _OptionalCreatePackageRequestRequestTypeDef
 ):
     pass
 
-
 StorageLocationTypeDef = TypedDict(
     "StorageLocationTypeDef",
     {
         "BinaryPrefixLocation": str,
         "Bucket": str,
         "GeneratedPrefixLocation": str,
         "ManifestPrefixLocation": str,
@@ -279,21 +262,19 @@
     "_OptionalDeletePackageRequestRequestTypeDef",
     {
         "ForceDelete": bool,
     },
     total=False,
 )
 
-
 class DeletePackageRequestRequestTypeDef(
     _RequiredDeletePackageRequestRequestTypeDef, _OptionalDeletePackageRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDeregisterPackageVersionRequestRequestTypeDef = TypedDict(
     "_RequiredDeregisterPackageVersionRequestRequestTypeDef",
     {
         "PackageId": str,
         "PackageVersion": str,
         "PatchVersion": str,
     },
@@ -303,22 +284,20 @@
     {
         "OwnerAccount": str,
         "UpdatedLatestPatchVersion": str,
     },
     total=False,
 )
 
-
 class DeregisterPackageVersionRequestRequestTypeDef(
     _RequiredDeregisterPackageVersionRequestRequestTypeDef,
     _OptionalDeregisterPackageVersionRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeApplicationInstanceDetailsRequestRequestTypeDef = TypedDict(
     "DescribeApplicationInstanceDetailsRequestRequestTypeDef",
     {
         "ApplicationInstanceId": str,
     },
 )
 
@@ -356,35 +335,41 @@
 DescribeNodeFromTemplateJobRequestRequestTypeDef = TypedDict(
     "DescribeNodeFromTemplateJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
+JobResourceTagsOutputTypeDef = TypedDict(
+    "JobResourceTagsOutputTypeDef",
+    {
+        "ResourceType": Literal["PACKAGE"],
+        "Tags": Dict[str, str],
+    },
+)
+
 _RequiredDescribeNodeRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeNodeRequestRequestTypeDef",
     {
         "NodeId": str,
     },
 )
 _OptionalDescribeNodeRequestRequestTypeDef = TypedDict(
     "_OptionalDescribeNodeRequestRequestTypeDef",
     {
         "OwnerAccount": str,
     },
     total=False,
 )
 
-
 class DescribeNodeRequestRequestTypeDef(
     _RequiredDescribeNodeRequestRequestTypeDef, _OptionalDescribeNodeRequestRequestTypeDef
 ):
     pass
 
-
 DescribePackageImportJobRequestRequestTypeDef = TypedDict(
     "DescribePackageImportJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
@@ -407,41 +392,37 @@
     {
         "OwnerAccount": str,
         "PatchVersion": str,
     },
     total=False,
 )
 
-
 class DescribePackageVersionRequestRequestTypeDef(
     _RequiredDescribePackageVersionRequestRequestTypeDef,
     _OptionalDescribePackageVersionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredOTAJobConfigTypeDef = TypedDict(
     "_RequiredOTAJobConfigTypeDef",
     {
         "ImageVersion": str,
     },
 )
 _OptionalOTAJobConfigTypeDef = TypedDict(
     "_OptionalOTAJobConfigTypeDef",
     {
         "AllowMajorVersionUpdate": bool,
     },
     total=False,
 )
 
-
 class OTAJobConfigTypeDef(_RequiredOTAJobConfigTypeDef, _OptionalOTAJobConfigTypeDef):
     pass
 
-
 DeviceJobTypeDef = TypedDict(
     "DeviceJobTypeDef",
     {
         "CreatedTime": datetime,
         "DeviceId": str,
         "DeviceName": str,
         "JobId": str,
@@ -476,14 +457,22 @@
         "ConnectionStatus": NetworkConnectionStatusType,
         "HwAddress": str,
         "IpAddress": str,
     },
     total=False,
 )
 
+JobResourceTagsTypeDef = TypedDict(
+    "JobResourceTagsTypeDef",
+    {
+        "ResourceType": Literal["PACKAGE"],
+        "Tags": Mapping[str, str],
+    },
+)
+
 _RequiredListApplicationInstanceDependenciesRequestRequestTypeDef = TypedDict(
     "_RequiredListApplicationInstanceDependenciesRequestRequestTypeDef",
     {
         "ApplicationInstanceId": str,
     },
 )
 _OptionalListApplicationInstanceDependenciesRequestRequestTypeDef = TypedDict(
@@ -491,22 +480,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListApplicationInstanceDependenciesRequestRequestTypeDef(
     _RequiredListApplicationInstanceDependenciesRequestRequestTypeDef,
     _OptionalListApplicationInstanceDependenciesRequestRequestTypeDef,
 ):
     pass
 
-
 PackageObjectTypeDef = TypedDict(
     "PackageObjectTypeDef",
     {
         "Name": str,
         "PackageVersion": str,
         "PatchVersion": str,
     },
@@ -523,22 +510,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListApplicationInstanceNodeInstancesRequestRequestTypeDef(
     _RequiredListApplicationInstanceNodeInstancesRequestRequestTypeDef,
     _OptionalListApplicationInstanceNodeInstancesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredNodeInstanceTypeDef = TypedDict(
     "_RequiredNodeInstanceTypeDef",
     {
         "CurrentStatus": NodeInstanceStatusType,
         "NodeInstanceId": str,
     },
 )
@@ -550,19 +535,17 @@
         "PackageName": str,
         "PackagePatchVersion": str,
         "PackageVersion": str,
     },
     total=False,
 )
 
-
 class NodeInstanceTypeDef(_RequiredNodeInstanceTypeDef, _OptionalNodeInstanceTypeDef):
     pass
 
-
 ListApplicationInstancesRequestRequestTypeDef = TypedDict(
     "ListApplicationInstancesRequestRequestTypeDef",
     {
         "DeviceId": str,
         "MaxResults": int,
         "NextToken": str,
         "StatusFilter": StatusFilterType,
@@ -648,19 +631,17 @@
         "Description": str,
         "OwnerAccount": str,
         "PackageArn": str,
     },
     total=False,
 )
 
-
 class NodeTypeDef(_RequiredNodeTypeDef, _OptionalNodeTypeDef):
     pass
 
-
 ListPackageImportJobsRequestRequestTypeDef = TypedDict(
     "ListPackageImportJobsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -780,21 +761,19 @@
     "_OptionalPackageVersionOutputConfigTypeDef",
     {
         "MarkLatest": bool,
     },
     total=False,
 )
 
-
 class PackageVersionOutputConfigTypeDef(
     _RequiredPackageVersionOutputConfigTypeDef, _OptionalPackageVersionOutputConfigTypeDef
 ):
     pass
 
-
 _RequiredS3LocationTypeDef = TypedDict(
     "_RequiredS3LocationTypeDef",
     {
         "BucketName": str,
         "ObjectKey": str,
     },
 )
@@ -802,19 +781,17 @@
     "_OptionalS3LocationTypeDef",
     {
         "Region": str,
     },
     total=False,
 )
 
-
 class S3LocationTypeDef(_RequiredS3LocationTypeDef, _OptionalS3LocationTypeDef):
     pass
 
-
 _RequiredRegisterPackageVersionRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterPackageVersionRequestRequestTypeDef",
     {
         "PackageId": str,
         "PackageVersion": str,
         "PatchVersion": str,
     },
@@ -824,22 +801,20 @@
     {
         "MarkLatest": bool,
         "OwnerAccount": str,
     },
     total=False,
 )
 
-
 class RegisterPackageVersionRequestRequestTypeDef(
     _RequiredRegisterPackageVersionRequestRequestTypeDef,
     _OptionalRegisterPackageVersionRequestRequestTypeDef,
 ):
     pass
 
-
 RemoveApplicationInstanceRequestRequestTypeDef = TypedDict(
     "RemoveApplicationInstanceRequestRequestTypeDef",
     {
         "ApplicationInstanceId": str,
     },
 )
 
@@ -869,22 +844,20 @@
     "_OptionalUpdateDeviceMetadataRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class UpdateDeviceMetadataRequestRequestTypeDef(
     _RequiredUpdateDeviceMetadataRequestRequestTypeDef,
     _OptionalUpdateDeviceMetadataRequestRequestTypeDef,
 ):
     pass
 
-
 ApplicationInstanceTypeDef = TypedDict(
     "ApplicationInstanceTypeDef",
     {
         "ApplicationInstanceId": str,
         "Arn": str,
         "CreatedTime": datetime,
         "DefaultRuntimeContextDevice": str,
@@ -916,22 +889,20 @@
         "Name": str,
         "RuntimeRoleArn": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateApplicationInstanceRequestRequestTypeDef(
     _RequiredCreateApplicationInstanceRequestRequestTypeDef,
     _OptionalCreateApplicationInstanceRequestRequestTypeDef,
 ):
     pass
 
-
 CreateApplicationInstanceResponseTypeDef = TypedDict(
     "CreateApplicationInstanceResponseTypeDef",
     {
         "ApplicationInstanceId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1070,60 +1041,14 @@
     "CreateJobForDevicesResponseTypeDef",
     {
         "Jobs": List[JobTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeNodeFromTemplateJobResponseTypeDef = TypedDict(
-    "DescribeNodeFromTemplateJobResponseTypeDef",
-    {
-        "CreatedTime": datetime,
-        "JobId": str,
-        "JobTags": List[JobResourceTagsOutputTypeDef],
-        "LastUpdatedTime": datetime,
-        "NodeDescription": str,
-        "NodeName": str,
-        "OutputPackageName": str,
-        "OutputPackageVersion": str,
-        "Status": NodeFromTemplateJobStatusType,
-        "StatusMessage": str,
-        "TemplateParameters": Dict[str, str],
-        "TemplateType": Literal["RTSP_CAMERA_STREAM"],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredCreateNodeFromTemplateJobRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateNodeFromTemplateJobRequestRequestTypeDef",
-    {
-        "NodeName": str,
-        "OutputPackageName": str,
-        "OutputPackageVersion": str,
-        "TemplateParameters": Mapping[str, str],
-        "TemplateType": Literal["RTSP_CAMERA_STREAM"],
-    },
-)
-_OptionalCreateNodeFromTemplateJobRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateNodeFromTemplateJobRequestRequestTypeDef",
-    {
-        "JobTags": Sequence[Union[JobResourceTagsTypeDef, JobResourceTagsOutputTypeDef]],
-        "NodeDescription": str,
-    },
-    total=False,
-)
-
-
-class CreateNodeFromTemplateJobRequestRequestTypeDef(
-    _RequiredCreateNodeFromTemplateJobRequestRequestTypeDef,
-    _OptionalCreateNodeFromTemplateJobRequestRequestTypeDef,
-):
-    pass
-
-
 CreatePackageResponseTypeDef = TypedDict(
     "CreatePackageResponseTypeDef",
     {
         "Arn": str,
         "PackageId": str,
         "StorageLocation": StorageLocationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1161,14 +1086,33 @@
         "ProvisioningStatus": DeviceStatusType,
         "Tags": Dict[str, str],
         "Type": DeviceTypeType,
     },
     total=False,
 )
 
+DescribeNodeFromTemplateJobResponseTypeDef = TypedDict(
+    "DescribeNodeFromTemplateJobResponseTypeDef",
+    {
+        "CreatedTime": datetime,
+        "JobId": str,
+        "JobTags": List[JobResourceTagsOutputTypeDef],
+        "LastUpdatedTime": datetime,
+        "NodeDescription": str,
+        "NodeName": str,
+        "OutputPackageName": str,
+        "OutputPackageVersion": str,
+        "Status": NodeFromTemplateJobStatusType,
+        "StatusMessage": str,
+        "TemplateParameters": Dict[str, str],
+        "TemplateType": Literal["RTSP_CAMERA_STREAM"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DeviceJobConfigTypeDef = TypedDict(
     "DeviceJobConfigTypeDef",
     {
         "OTAJobConfig": OTAJobConfigTypeDef,
     },
     total=False,
 )
@@ -1192,40 +1136,37 @@
     "_OptionalEthernetPayloadOutputTypeDef",
     {
         "StaticIpConnectionInfo": StaticIpConnectionInfoOutputTypeDef,
     },
     total=False,
 )
 
-
 class EthernetPayloadOutputTypeDef(
     _RequiredEthernetPayloadOutputTypeDef, _OptionalEthernetPayloadOutputTypeDef
 ):
     pass
 
-
 _RequiredEthernetPayloadTypeDef = TypedDict(
     "_RequiredEthernetPayloadTypeDef",
     {
         "ConnectionType": ConnectionTypeType,
     },
 )
 _OptionalEthernetPayloadTypeDef = TypedDict(
     "_OptionalEthernetPayloadTypeDef",
     {
         "StaticIpConnectionInfo": StaticIpConnectionInfoTypeDef,
     },
     total=False,
 )
 
-
 class EthernetPayloadTypeDef(_RequiredEthernetPayloadTypeDef, _OptionalEthernetPayloadTypeDef):
     pass
 
-
+JobResourceTagsUnionTypeDef = Union[JobResourceTagsTypeDef, JobResourceTagsOutputTypeDef]
 ListApplicationInstanceDependenciesResponseTypeDef = TypedDict(
     "ListApplicationInstanceDependenciesResponseTypeDef",
     {
         "NextToken": str,
         "PackageObjects": List[PackageObjectTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1357,22 +1298,20 @@
     "_OptionalCreateJobForDevicesRequestRequestTypeDef",
     {
         "DeviceJobConfig": DeviceJobConfigTypeDef,
     },
     total=False,
 )
 
-
 class CreateJobForDevicesRequestRequestTypeDef(
     _RequiredCreateJobForDevicesRequestRequestTypeDef,
     _OptionalCreateJobForDevicesRequestRequestTypeDef,
 ):
     pass
 
-
 NetworkPayloadOutputTypeDef = TypedDict(
     "NetworkPayloadOutputTypeDef",
     {
         "Ethernet0": EthernetPayloadOutputTypeDef,
         "Ethernet1": EthernetPayloadOutputTypeDef,
         "Ntp": NtpPayloadOutputTypeDef,
     },
@@ -1385,14 +1324,39 @@
         "Ethernet0": EthernetPayloadTypeDef,
         "Ethernet1": EthernetPayloadTypeDef,
         "Ntp": NtpPayloadTypeDef,
     },
     total=False,
 )
 
+_RequiredCreateNodeFromTemplateJobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateNodeFromTemplateJobRequestRequestTypeDef",
+    {
+        "NodeName": str,
+        "OutputPackageName": str,
+        "OutputPackageVersion": str,
+        "TemplateParameters": Mapping[str, str],
+        "TemplateType": Literal["RTSP_CAMERA_STREAM"],
+    },
+)
+_OptionalCreateNodeFromTemplateJobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateNodeFromTemplateJobRequestRequestTypeDef",
+    {
+        "JobTags": Sequence[JobResourceTagsUnionTypeDef],
+        "NodeDescription": str,
+    },
+    total=False,
+)
+
+class CreateNodeFromTemplateJobRequestRequestTypeDef(
+    _RequiredCreateNodeFromTemplateJobRequestRequestTypeDef,
+    _OptionalCreateNodeFromTemplateJobRequestRequestTypeDef,
+):
+    pass
+
 DescribeNodeResponseTypeDef = TypedDict(
     "DescribeNodeResponseTypeDef",
     {
         "AssetName": str,
         "Category": NodeCategoryType,
         "CreatedTime": datetime,
         "Description": str,
@@ -1441,14 +1405,15 @@
         "SerialNumber": str,
         "Tags": Dict[str, str],
         "Type": DeviceTypeType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+NetworkPayloadUnionTypeDef = Union[NetworkPayloadTypeDef, NetworkPayloadOutputTypeDef]
 _RequiredProvisionDeviceRequestRequestTypeDef = TypedDict(
     "_RequiredProvisionDeviceRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalProvisionDeviceRequestRequestTypeDef = TypedDict(
@@ -1457,46 +1422,42 @@
         "Description": str,
         "NetworkingConfiguration": NetworkPayloadTypeDef,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class ProvisionDeviceRequestRequestTypeDef(
     _RequiredProvisionDeviceRequestRequestTypeDef, _OptionalProvisionDeviceRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreatePackageImportJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePackageImportJobRequestRequestTypeDef",
     {
         "ClientToken": str,
         "InputConfig": PackageImportJobInputConfigTypeDef,
         "JobType": PackageImportJobTypeType,
         "OutputConfig": PackageImportJobOutputConfigTypeDef,
     },
 )
 _OptionalCreatePackageImportJobRequestRequestTypeDef = TypedDict(
     "_OptionalCreatePackageImportJobRequestRequestTypeDef",
     {
-        "JobTags": Sequence[Union[JobResourceTagsTypeDef, JobResourceTagsOutputTypeDef]],
+        "JobTags": Sequence[JobResourceTagsUnionTypeDef],
     },
     total=False,
 )
 
-
 class CreatePackageImportJobRequestRequestTypeDef(
     _RequiredCreatePackageImportJobRequestRequestTypeDef,
     _OptionalCreatePackageImportJobRequestRequestTypeDef,
 ):
     pass
 
-
 DescribePackageImportJobResponseTypeDef = TypedDict(
     "DescribePackageImportJobResponseTypeDef",
     {
         "ClientToken": str,
         "CreatedTime": datetime,
         "InputConfig": PackageImportJobInputConfigTypeDef,
         "JobId": str,
```

### Comparing `mypy-boto3-panorama-1.28.15.post1/mypy_boto3_panorama/type_defs.pyi` & `mypy-boto3-panorama-1.28.16/mypy_boto3_panorama/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_panorama/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_panorama.type_defs import AlternateSoftwareMetadataTypeDef
 
-    data: AlternateSoftwareMetadataTypeDef = {...}
+    data: AlternateSoftwareMetadataTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -47,43 +47,44 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AlternateSoftwareMetadataTypeDef",
     "ReportedRuntimeContextStateTypeDef",
     "ManifestOverridesPayloadTypeDef",
     "ManifestPayloadTypeDef",
     "ResponseMetadataTypeDef",
     "JobTypeDef",
-    "JobResourceTagsOutputTypeDef",
-    "JobResourceTagsTypeDef",
     "CreatePackageRequestRequestTypeDef",
     "StorageLocationTypeDef",
     "DeleteDeviceRequestRequestTypeDef",
     "DeletePackageRequestRequestTypeDef",
     "DeregisterPackageVersionRequestRequestTypeDef",
     "DescribeApplicationInstanceDetailsRequestRequestTypeDef",
     "DescribeApplicationInstanceRequestRequestTypeDef",
     "DescribeDeviceJobRequestRequestTypeDef",
     "DescribeDeviceRequestRequestTypeDef",
     "LatestDeviceJobTypeDef",
     "DescribeNodeFromTemplateJobRequestRequestTypeDef",
+    "JobResourceTagsOutputTypeDef",
     "DescribeNodeRequestRequestTypeDef",
     "DescribePackageImportJobRequestRequestTypeDef",
     "DescribePackageRequestRequestTypeDef",
     "DescribePackageVersionRequestRequestTypeDef",
     "OTAJobConfigTypeDef",
     "DeviceJobTypeDef",
     "StaticIpConnectionInfoOutputTypeDef",
     "StaticIpConnectionInfoTypeDef",
     "EthernetStatusTypeDef",
+    "JobResourceTagsTypeDef",
     "ListApplicationInstanceDependenciesRequestRequestTypeDef",
     "PackageObjectTypeDef",
     "ListApplicationInstanceNodeInstancesRequestRequestTypeDef",
     "NodeInstanceTypeDef",
     "ListApplicationInstancesRequestRequestTypeDef",
     "ListDevicesJobsRequestRequestTypeDef",
     "ListDevicesRequestRequestTypeDef",
@@ -121,23 +122,23 @@
     "DescribeDeviceJobResponseTypeDef",
     "DescribePackageVersionResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "ProvisionDeviceResponseTypeDef",
     "SignalApplicationInstanceNodeInstancesResponseTypeDef",
     "UpdateDeviceMetadataResponseTypeDef",
     "CreateJobForDevicesResponseTypeDef",
-    "DescribeNodeFromTemplateJobResponseTypeDef",
-    "CreateNodeFromTemplateJobRequestRequestTypeDef",
     "CreatePackageResponseTypeDef",
     "DescribePackageResponseTypeDef",
     "DeviceTypeDef",
+    "DescribeNodeFromTemplateJobResponseTypeDef",
     "DeviceJobConfigTypeDef",
     "ListDevicesJobsResponseTypeDef",
     "EthernetPayloadOutputTypeDef",
     "EthernetPayloadTypeDef",
+    "JobResourceTagsUnionTypeDef",
     "ListApplicationInstanceDependenciesResponseTypeDef",
     "ListApplicationInstanceNodeInstancesResponseTypeDef",
     "ListNodeFromTemplateJobsResponseTypeDef",
     "ListNodesResponseTypeDef",
     "ListPackageImportJobsResponseTypeDef",
     "ListPackagesResponseTypeDef",
     "NetworkStatusTypeDef",
@@ -147,17 +148,19 @@
     "PackageImportJobOutputConfigTypeDef",
     "PackageVersionInputConfigTypeDef",
     "ListApplicationInstancesResponseTypeDef",
     "ListDevicesResponseTypeDef",
     "CreateJobForDevicesRequestRequestTypeDef",
     "NetworkPayloadOutputTypeDef",
     "NetworkPayloadTypeDef",
+    "CreateNodeFromTemplateJobRequestRequestTypeDef",
     "DescribeNodeResponseTypeDef",
     "PackageImportJobInputConfigTypeDef",
     "DescribeDeviceResponseTypeDef",
+    "NetworkPayloadUnionTypeDef",
     "ProvisionDeviceRequestRequestTypeDef",
     "CreatePackageImportJobRequestRequestTypeDef",
     "DescribePackageImportJobResponseTypeDef",
 )
 
 AlternateSoftwareMetadataTypeDef = TypedDict(
     "AlternateSoftwareMetadataTypeDef",
@@ -209,49 +212,35 @@
     {
         "DeviceId": str,
         "JobId": str,
     },
     total=False,
 )
 
-JobResourceTagsOutputTypeDef = TypedDict(
-    "JobResourceTagsOutputTypeDef",
-    {
-        "ResourceType": Literal["PACKAGE"],
-        "Tags": Dict[str, str],
-    },
-)
-
-JobResourceTagsTypeDef = TypedDict(
-    "JobResourceTagsTypeDef",
-    {
-        "ResourceType": Literal["PACKAGE"],
-        "Tags": Mapping[str, str],
-    },
-)
-
 _RequiredCreatePackageRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePackageRequestRequestTypeDef",
     {
         "PackageName": str,
     },
 )
 _OptionalCreatePackageRequestRequestTypeDef = TypedDict(
     "_OptionalCreatePackageRequestRequestTypeDef",
     {
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreatePackageRequestRequestTypeDef(
     _RequiredCreatePackageRequestRequestTypeDef, _OptionalCreatePackageRequestRequestTypeDef
 ):
     pass
 
+
 StorageLocationTypeDef = TypedDict(
     "StorageLocationTypeDef",
     {
         "BinaryPrefixLocation": str,
         "Bucket": str,
         "GeneratedPrefixLocation": str,
         "ManifestPrefixLocation": str,
@@ -276,19 +265,21 @@
     "_OptionalDeletePackageRequestRequestTypeDef",
     {
         "ForceDelete": bool,
     },
     total=False,
 )
 
+
 class DeletePackageRequestRequestTypeDef(
     _RequiredDeletePackageRequestRequestTypeDef, _OptionalDeletePackageRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDeregisterPackageVersionRequestRequestTypeDef = TypedDict(
     "_RequiredDeregisterPackageVersionRequestRequestTypeDef",
     {
         "PackageId": str,
         "PackageVersion": str,
         "PatchVersion": str,
     },
@@ -298,20 +289,22 @@
     {
         "OwnerAccount": str,
         "UpdatedLatestPatchVersion": str,
     },
     total=False,
 )
 
+
 class DeregisterPackageVersionRequestRequestTypeDef(
     _RequiredDeregisterPackageVersionRequestRequestTypeDef,
     _OptionalDeregisterPackageVersionRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeApplicationInstanceDetailsRequestRequestTypeDef = TypedDict(
     "DescribeApplicationInstanceDetailsRequestRequestTypeDef",
     {
         "ApplicationInstanceId": str,
     },
 )
 
@@ -349,33 +342,43 @@
 DescribeNodeFromTemplateJobRequestRequestTypeDef = TypedDict(
     "DescribeNodeFromTemplateJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
+JobResourceTagsOutputTypeDef = TypedDict(
+    "JobResourceTagsOutputTypeDef",
+    {
+        "ResourceType": Literal["PACKAGE"],
+        "Tags": Dict[str, str],
+    },
+)
+
 _RequiredDescribeNodeRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeNodeRequestRequestTypeDef",
     {
         "NodeId": str,
     },
 )
 _OptionalDescribeNodeRequestRequestTypeDef = TypedDict(
     "_OptionalDescribeNodeRequestRequestTypeDef",
     {
         "OwnerAccount": str,
     },
     total=False,
 )
 
+
 class DescribeNodeRequestRequestTypeDef(
     _RequiredDescribeNodeRequestRequestTypeDef, _OptionalDescribeNodeRequestRequestTypeDef
 ):
     pass
 
+
 DescribePackageImportJobRequestRequestTypeDef = TypedDict(
     "DescribePackageImportJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
@@ -398,37 +401,41 @@
     {
         "OwnerAccount": str,
         "PatchVersion": str,
     },
     total=False,
 )
 
+
 class DescribePackageVersionRequestRequestTypeDef(
     _RequiredDescribePackageVersionRequestRequestTypeDef,
     _OptionalDescribePackageVersionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredOTAJobConfigTypeDef = TypedDict(
     "_RequiredOTAJobConfigTypeDef",
     {
         "ImageVersion": str,
     },
 )
 _OptionalOTAJobConfigTypeDef = TypedDict(
     "_OptionalOTAJobConfigTypeDef",
     {
         "AllowMajorVersionUpdate": bool,
     },
     total=False,
 )
 
+
 class OTAJobConfigTypeDef(_RequiredOTAJobConfigTypeDef, _OptionalOTAJobConfigTypeDef):
     pass
 
+
 DeviceJobTypeDef = TypedDict(
     "DeviceJobTypeDef",
     {
         "CreatedTime": datetime,
         "DeviceId": str,
         "DeviceName": str,
         "JobId": str,
@@ -463,14 +470,22 @@
         "ConnectionStatus": NetworkConnectionStatusType,
         "HwAddress": str,
         "IpAddress": str,
     },
     total=False,
 )
 
+JobResourceTagsTypeDef = TypedDict(
+    "JobResourceTagsTypeDef",
+    {
+        "ResourceType": Literal["PACKAGE"],
+        "Tags": Mapping[str, str],
+    },
+)
+
 _RequiredListApplicationInstanceDependenciesRequestRequestTypeDef = TypedDict(
     "_RequiredListApplicationInstanceDependenciesRequestRequestTypeDef",
     {
         "ApplicationInstanceId": str,
     },
 )
 _OptionalListApplicationInstanceDependenciesRequestRequestTypeDef = TypedDict(
@@ -478,20 +493,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListApplicationInstanceDependenciesRequestRequestTypeDef(
     _RequiredListApplicationInstanceDependenciesRequestRequestTypeDef,
     _OptionalListApplicationInstanceDependenciesRequestRequestTypeDef,
 ):
     pass
 
+
 PackageObjectTypeDef = TypedDict(
     "PackageObjectTypeDef",
     {
         "Name": str,
         "PackageVersion": str,
         "PatchVersion": str,
     },
@@ -508,20 +525,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListApplicationInstanceNodeInstancesRequestRequestTypeDef(
     _RequiredListApplicationInstanceNodeInstancesRequestRequestTypeDef,
     _OptionalListApplicationInstanceNodeInstancesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredNodeInstanceTypeDef = TypedDict(
     "_RequiredNodeInstanceTypeDef",
     {
         "CurrentStatus": NodeInstanceStatusType,
         "NodeInstanceId": str,
     },
 )
@@ -533,17 +552,19 @@
         "PackageName": str,
         "PackagePatchVersion": str,
         "PackageVersion": str,
     },
     total=False,
 )
 
+
 class NodeInstanceTypeDef(_RequiredNodeInstanceTypeDef, _OptionalNodeInstanceTypeDef):
     pass
 
+
 ListApplicationInstancesRequestRequestTypeDef = TypedDict(
     "ListApplicationInstancesRequestRequestTypeDef",
     {
         "DeviceId": str,
         "MaxResults": int,
         "NextToken": str,
         "StatusFilter": StatusFilterType,
@@ -629,17 +650,19 @@
         "Description": str,
         "OwnerAccount": str,
         "PackageArn": str,
     },
     total=False,
 )
 
+
 class NodeTypeDef(_RequiredNodeTypeDef, _OptionalNodeTypeDef):
     pass
 
+
 ListPackageImportJobsRequestRequestTypeDef = TypedDict(
     "ListPackageImportJobsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -759,19 +782,21 @@
     "_OptionalPackageVersionOutputConfigTypeDef",
     {
         "MarkLatest": bool,
     },
     total=False,
 )
 
+
 class PackageVersionOutputConfigTypeDef(
     _RequiredPackageVersionOutputConfigTypeDef, _OptionalPackageVersionOutputConfigTypeDef
 ):
     pass
 
+
 _RequiredS3LocationTypeDef = TypedDict(
     "_RequiredS3LocationTypeDef",
     {
         "BucketName": str,
         "ObjectKey": str,
     },
 )
@@ -779,17 +804,19 @@
     "_OptionalS3LocationTypeDef",
     {
         "Region": str,
     },
     total=False,
 )
 
+
 class S3LocationTypeDef(_RequiredS3LocationTypeDef, _OptionalS3LocationTypeDef):
     pass
 
+
 _RequiredRegisterPackageVersionRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterPackageVersionRequestRequestTypeDef",
     {
         "PackageId": str,
         "PackageVersion": str,
         "PatchVersion": str,
     },
@@ -799,20 +826,22 @@
     {
         "MarkLatest": bool,
         "OwnerAccount": str,
     },
     total=False,
 )
 
+
 class RegisterPackageVersionRequestRequestTypeDef(
     _RequiredRegisterPackageVersionRequestRequestTypeDef,
     _OptionalRegisterPackageVersionRequestRequestTypeDef,
 ):
     pass
 
+
 RemoveApplicationInstanceRequestRequestTypeDef = TypedDict(
     "RemoveApplicationInstanceRequestRequestTypeDef",
     {
         "ApplicationInstanceId": str,
     },
 )
 
@@ -842,20 +871,22 @@
     "_OptionalUpdateDeviceMetadataRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class UpdateDeviceMetadataRequestRequestTypeDef(
     _RequiredUpdateDeviceMetadataRequestRequestTypeDef,
     _OptionalUpdateDeviceMetadataRequestRequestTypeDef,
 ):
     pass
 
+
 ApplicationInstanceTypeDef = TypedDict(
     "ApplicationInstanceTypeDef",
     {
         "ApplicationInstanceId": str,
         "Arn": str,
         "CreatedTime": datetime,
         "DefaultRuntimeContextDevice": str,
@@ -887,20 +918,22 @@
         "Name": str,
         "RuntimeRoleArn": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateApplicationInstanceRequestRequestTypeDef(
     _RequiredCreateApplicationInstanceRequestRequestTypeDef,
     _OptionalCreateApplicationInstanceRequestRequestTypeDef,
 ):
     pass
 
+
 CreateApplicationInstanceResponseTypeDef = TypedDict(
     "CreateApplicationInstanceResponseTypeDef",
     {
         "ApplicationInstanceId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1039,58 +1072,14 @@
     "CreateJobForDevicesResponseTypeDef",
     {
         "Jobs": List[JobTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeNodeFromTemplateJobResponseTypeDef = TypedDict(
-    "DescribeNodeFromTemplateJobResponseTypeDef",
-    {
-        "CreatedTime": datetime,
-        "JobId": str,
-        "JobTags": List[JobResourceTagsOutputTypeDef],
-        "LastUpdatedTime": datetime,
-        "NodeDescription": str,
-        "NodeName": str,
-        "OutputPackageName": str,
-        "OutputPackageVersion": str,
-        "Status": NodeFromTemplateJobStatusType,
-        "StatusMessage": str,
-        "TemplateParameters": Dict[str, str],
-        "TemplateType": Literal["RTSP_CAMERA_STREAM"],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredCreateNodeFromTemplateJobRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateNodeFromTemplateJobRequestRequestTypeDef",
-    {
-        "NodeName": str,
-        "OutputPackageName": str,
-        "OutputPackageVersion": str,
-        "TemplateParameters": Mapping[str, str],
-        "TemplateType": Literal["RTSP_CAMERA_STREAM"],
-    },
-)
-_OptionalCreateNodeFromTemplateJobRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateNodeFromTemplateJobRequestRequestTypeDef",
-    {
-        "JobTags": Sequence[Union[JobResourceTagsTypeDef, JobResourceTagsOutputTypeDef]],
-        "NodeDescription": str,
-    },
-    total=False,
-)
-
-class CreateNodeFromTemplateJobRequestRequestTypeDef(
-    _RequiredCreateNodeFromTemplateJobRequestRequestTypeDef,
-    _OptionalCreateNodeFromTemplateJobRequestRequestTypeDef,
-):
-    pass
-
 CreatePackageResponseTypeDef = TypedDict(
     "CreatePackageResponseTypeDef",
     {
         "Arn": str,
         "PackageId": str,
         "StorageLocation": StorageLocationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1128,14 +1117,33 @@
         "ProvisioningStatus": DeviceStatusType,
         "Tags": Dict[str, str],
         "Type": DeviceTypeType,
     },
     total=False,
 )
 
+DescribeNodeFromTemplateJobResponseTypeDef = TypedDict(
+    "DescribeNodeFromTemplateJobResponseTypeDef",
+    {
+        "CreatedTime": datetime,
+        "JobId": str,
+        "JobTags": List[JobResourceTagsOutputTypeDef],
+        "LastUpdatedTime": datetime,
+        "NodeDescription": str,
+        "NodeName": str,
+        "OutputPackageName": str,
+        "OutputPackageVersion": str,
+        "Status": NodeFromTemplateJobStatusType,
+        "StatusMessage": str,
+        "TemplateParameters": Dict[str, str],
+        "TemplateType": Literal["RTSP_CAMERA_STREAM"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DeviceJobConfigTypeDef = TypedDict(
     "DeviceJobConfigTypeDef",
     {
         "OTAJobConfig": OTAJobConfigTypeDef,
     },
     total=False,
 )
@@ -1159,36 +1167,41 @@
     "_OptionalEthernetPayloadOutputTypeDef",
     {
         "StaticIpConnectionInfo": StaticIpConnectionInfoOutputTypeDef,
     },
     total=False,
 )
 
+
 class EthernetPayloadOutputTypeDef(
     _RequiredEthernetPayloadOutputTypeDef, _OptionalEthernetPayloadOutputTypeDef
 ):
     pass
 
+
 _RequiredEthernetPayloadTypeDef = TypedDict(
     "_RequiredEthernetPayloadTypeDef",
     {
         "ConnectionType": ConnectionTypeType,
     },
 )
 _OptionalEthernetPayloadTypeDef = TypedDict(
     "_OptionalEthernetPayloadTypeDef",
     {
         "StaticIpConnectionInfo": StaticIpConnectionInfoTypeDef,
     },
     total=False,
 )
 
+
 class EthernetPayloadTypeDef(_RequiredEthernetPayloadTypeDef, _OptionalEthernetPayloadTypeDef):
     pass
 
+
+JobResourceTagsUnionTypeDef = Union[JobResourceTagsTypeDef, JobResourceTagsOutputTypeDef]
 ListApplicationInstanceDependenciesResponseTypeDef = TypedDict(
     "ListApplicationInstanceDependenciesResponseTypeDef",
     {
         "NextToken": str,
         "PackageObjects": List[PackageObjectTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1320,20 +1333,22 @@
     "_OptionalCreateJobForDevicesRequestRequestTypeDef",
     {
         "DeviceJobConfig": DeviceJobConfigTypeDef,
     },
     total=False,
 )
 
+
 class CreateJobForDevicesRequestRequestTypeDef(
     _RequiredCreateJobForDevicesRequestRequestTypeDef,
     _OptionalCreateJobForDevicesRequestRequestTypeDef,
 ):
     pass
 
+
 NetworkPayloadOutputTypeDef = TypedDict(
     "NetworkPayloadOutputTypeDef",
     {
         "Ethernet0": EthernetPayloadOutputTypeDef,
         "Ethernet1": EthernetPayloadOutputTypeDef,
         "Ntp": NtpPayloadOutputTypeDef,
     },
@@ -1346,14 +1361,41 @@
         "Ethernet0": EthernetPayloadTypeDef,
         "Ethernet1": EthernetPayloadTypeDef,
         "Ntp": NtpPayloadTypeDef,
     },
     total=False,
 )
 
+_RequiredCreateNodeFromTemplateJobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateNodeFromTemplateJobRequestRequestTypeDef",
+    {
+        "NodeName": str,
+        "OutputPackageName": str,
+        "OutputPackageVersion": str,
+        "TemplateParameters": Mapping[str, str],
+        "TemplateType": Literal["RTSP_CAMERA_STREAM"],
+    },
+)
+_OptionalCreateNodeFromTemplateJobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateNodeFromTemplateJobRequestRequestTypeDef",
+    {
+        "JobTags": Sequence[JobResourceTagsUnionTypeDef],
+        "NodeDescription": str,
+    },
+    total=False,
+)
+
+
+class CreateNodeFromTemplateJobRequestRequestTypeDef(
+    _RequiredCreateNodeFromTemplateJobRequestRequestTypeDef,
+    _OptionalCreateNodeFromTemplateJobRequestRequestTypeDef,
+):
+    pass
+
+
 DescribeNodeResponseTypeDef = TypedDict(
     "DescribeNodeResponseTypeDef",
     {
         "AssetName": str,
         "Category": NodeCategoryType,
         "CreatedTime": datetime,
         "Description": str,
@@ -1402,14 +1444,15 @@
         "SerialNumber": str,
         "Tags": Dict[str, str],
         "Type": DeviceTypeType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+NetworkPayloadUnionTypeDef = Union[NetworkPayloadTypeDef, NetworkPayloadOutputTypeDef]
 _RequiredProvisionDeviceRequestRequestTypeDef = TypedDict(
     "_RequiredProvisionDeviceRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalProvisionDeviceRequestRequestTypeDef = TypedDict(
@@ -1418,42 +1461,46 @@
         "Description": str,
         "NetworkingConfiguration": NetworkPayloadTypeDef,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class ProvisionDeviceRequestRequestTypeDef(
     _RequiredProvisionDeviceRequestRequestTypeDef, _OptionalProvisionDeviceRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreatePackageImportJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePackageImportJobRequestRequestTypeDef",
     {
         "ClientToken": str,
         "InputConfig": PackageImportJobInputConfigTypeDef,
         "JobType": PackageImportJobTypeType,
         "OutputConfig": PackageImportJobOutputConfigTypeDef,
     },
 )
 _OptionalCreatePackageImportJobRequestRequestTypeDef = TypedDict(
     "_OptionalCreatePackageImportJobRequestRequestTypeDef",
     {
-        "JobTags": Sequence[Union[JobResourceTagsTypeDef, JobResourceTagsOutputTypeDef]],
+        "JobTags": Sequence[JobResourceTagsUnionTypeDef],
     },
     total=False,
 )
 
+
 class CreatePackageImportJobRequestRequestTypeDef(
     _RequiredCreatePackageImportJobRequestRequestTypeDef,
     _OptionalCreatePackageImportJobRequestRequestTypeDef,
 ):
     pass
 
+
 DescribePackageImportJobResponseTypeDef = TypedDict(
     "DescribePackageImportJobResponseTypeDef",
     {
         "ClientToken": str,
         "CreatedTime": datetime,
         "InputConfig": PackageImportJobInputConfigTypeDef,
         "JobId": str,
```

### Comparing `mypy-boto3-panorama-1.28.15.post1/mypy_boto3_panorama.egg-info/PKG-INFO` & `mypy-boto3-panorama-1.28.16/mypy_boto3_panorama.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-panorama
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Panorama 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.Panorama 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_panorama/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 panorama type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 panorama type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-panorama.svg?color=blue)](https://pypi.org/project/mypy-boto3-panorama)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_panorama/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-panorama)](https://pepy.tech/project/mypy-boto3-panorama)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Panorama 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama)
+[boto3.Panorama 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama)
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
 [mypy-boto3-panorama docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_panorama/).
 
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
@@ -311,51 +311,51 @@
 )
 
 
 def check_value(value: ApplicationInstanceHealthStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_panorama.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_panorama.type_defs import (
     AlternateSoftwareMetadataTypeDef,
     ReportedRuntimeContextStateTypeDef,
     ManifestOverridesPayloadTypeDef,
     ManifestPayloadTypeDef,
     ResponseMetadataTypeDef,
     JobTypeDef,
-    JobResourceTagsOutputTypeDef,
-    JobResourceTagsTypeDef,
     CreatePackageRequestRequestTypeDef,
     StorageLocationTypeDef,
     DeleteDeviceRequestRequestTypeDef,
     DeletePackageRequestRequestTypeDef,
     DeregisterPackageVersionRequestRequestTypeDef,
     DescribeApplicationInstanceDetailsRequestRequestTypeDef,
     DescribeApplicationInstanceRequestRequestTypeDef,
     DescribeDeviceJobRequestRequestTypeDef,
     DescribeDeviceRequestRequestTypeDef,
     LatestDeviceJobTypeDef,
     DescribeNodeFromTemplateJobRequestRequestTypeDef,
+    JobResourceTagsOutputTypeDef,
     DescribeNodeRequestRequestTypeDef,
     DescribePackageImportJobRequestRequestTypeDef,
     DescribePackageRequestRequestTypeDef,
     DescribePackageVersionRequestRequestTypeDef,
     OTAJobConfigTypeDef,
     DeviceJobTypeDef,
     StaticIpConnectionInfoOutputTypeDef,
     StaticIpConnectionInfoTypeDef,
     EthernetStatusTypeDef,
+    JobResourceTagsTypeDef,
     ListApplicationInstanceDependenciesRequestRequestTypeDef,
     PackageObjectTypeDef,
     ListApplicationInstanceNodeInstancesRequestRequestTypeDef,
     NodeInstanceTypeDef,
     ListApplicationInstancesRequestRequestTypeDef,
     ListDevicesJobsRequestRequestTypeDef,
     ListDevicesRequestRequestTypeDef,
@@ -393,23 +393,23 @@
     DescribeDeviceJobResponseTypeDef,
     DescribePackageVersionResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ProvisionDeviceResponseTypeDef,
     SignalApplicationInstanceNodeInstancesResponseTypeDef,
     UpdateDeviceMetadataResponseTypeDef,
     CreateJobForDevicesResponseTypeDef,
-    DescribeNodeFromTemplateJobResponseTypeDef,
-    CreateNodeFromTemplateJobRequestRequestTypeDef,
     CreatePackageResponseTypeDef,
     DescribePackageResponseTypeDef,
     DeviceTypeDef,
+    DescribeNodeFromTemplateJobResponseTypeDef,
     DeviceJobConfigTypeDef,
     ListDevicesJobsResponseTypeDef,
     EthernetPayloadOutputTypeDef,
     EthernetPayloadTypeDef,
+    JobResourceTagsUnionTypeDef,
     ListApplicationInstanceDependenciesResponseTypeDef,
     ListApplicationInstanceNodeInstancesResponseTypeDef,
     ListNodeFromTemplateJobsResponseTypeDef,
     ListNodesResponseTypeDef,
     ListPackageImportJobsResponseTypeDef,
     ListPackagesResponseTypeDef,
     NetworkStatusTypeDef,
@@ -419,24 +419,26 @@
     PackageImportJobOutputConfigTypeDef,
     PackageVersionInputConfigTypeDef,
     ListApplicationInstancesResponseTypeDef,
     ListDevicesResponseTypeDef,
     CreateJobForDevicesRequestRequestTypeDef,
     NetworkPayloadOutputTypeDef,
     NetworkPayloadTypeDef,
+    CreateNodeFromTemplateJobRequestRequestTypeDef,
     DescribeNodeResponseTypeDef,
     PackageImportJobInputConfigTypeDef,
     DescribeDeviceResponseTypeDef,
+    NetworkPayloadUnionTypeDef,
     ProvisionDeviceRequestRequestTypeDef,
     CreatePackageImportJobRequestRequestTypeDef,
     DescribePackageImportJobResponseTypeDef,
 )
 
 
-def get_structure() -> AlternateSoftwareMetadataTypeDef:
+def get_value() -> AlternateSoftwareMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-panorama-1.28.15.post1/mypy_boto3_panorama.egg-info/SOURCES.txt` & `mypy-boto3-panorama-1.28.16/mypy_boto3_panorama.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-panorama-1.28.15.post1/setup.py` & `mypy-boto3-panorama-1.28.16/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-panorama",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_panorama"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Panorama 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.Panorama 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 panorama type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 panorama type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_panorama": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_panorama/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

