# Comparing `tmp/bootloader_core_library-0.0.5.tar.gz` & `tmp/bootloader_core_library-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bootloader_core_library-0.0.5.tar", max compression
+gzip compressed data, was "bootloader_core_library-0.0.6.tar", max compression
```

## Comparing `bootloader_core_library-0.0.5.tar` & `bootloader_core_library-0.0.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      735 2023-08-01 14:34:34.411884 bootloader_core_library-0.0.5/CHANGELOG.md
--rw-r--r--   0        0        0      761 2023-03-31 11:22:24.297536 bootloader_core_library-0.0.5/LICENSE.md
--rw-r--r--   0        0        0      138 2023-08-01 09:48:11.340859 bootloader_core_library-0.0.5/README.md
--rw-r--r--   0        0        0      905 2023-08-01 14:33:48.411313 bootloader_core_library-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      859 2023-03-31 11:21:05.979756 bootloader_core_library-0.0.5/src/bootloader/__init__.py
--rw-r--r--   0        0        0      859 2023-03-31 11:21:05.992853 bootloader_core_library-0.0.5/src/bootloader/ue/__init__.py
--rw-r--r--   0        0        0      859 2023-03-31 11:21:05.975392 bootloader_core_library-0.0.5/src/bootloader/ue/constant/__init__.py
--rw-r--r--   0        0        0    17232 2023-08-01 14:15:12.075340 bootloader_core_library-0.0.5/src/bootloader/ue/constant/ue_asset.py
--rw-r--r--   0        0        0      859 2023-03-31 11:21:05.975392 bootloader_core_library-0.0.5/src/bootloader/ue/model/__init__.py
--rw-r--r--   0        0        0    12147 2023-08-01 14:33:25.790792 bootloader_core_library-0.0.5/src/bootloader/ue/model/ue_asset.py
--rw-r--r--   0        0        0     1060 1970-01-01 00:00:00.000000 bootloader_core_library-0.0.5/setup.py
--rw-r--r--   0        0        0     1134 1970-01-01 00:00:00.000000 bootloader_core_library-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      863 2023-08-01 15:46:21.346633 bootloader_core_library-0.0.6/CHANGELOG.md
+-rw-r--r--   0        0        0      761 2023-03-31 11:22:24.297536 bootloader_core_library-0.0.6/LICENSE.md
+-rw-r--r--   0        0        0      138 2023-08-01 09:48:11.340859 bootloader_core_library-0.0.6/README.md
+-rw-r--r--   0        0        0      905 2023-08-01 15:46:21.354932 bootloader_core_library-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      859 2023-03-31 11:21:05.979756 bootloader_core_library-0.0.6/src/bootloader/__init__.py
+-rw-r--r--   0        0        0      859 2023-03-31 11:21:05.992853 bootloader_core_library-0.0.6/src/bootloader/ue/__init__.py
+-rw-r--r--   0        0        0      859 2023-03-31 11:21:05.975392 bootloader_core_library-0.0.6/src/bootloader/ue/constant/__init__.py
+-rw-r--r--   0        0        0    17232 2023-08-01 14:15:12.075340 bootloader_core_library-0.0.6/src/bootloader/ue/constant/ue_asset.py
+-rw-r--r--   0        0        0      859 2023-03-31 11:21:05.975392 bootloader_core_library-0.0.6/src/bootloader/ue/model/__init__.py
+-rw-r--r--   0        0        0    15017 2023-08-01 15:45:54.887029 bootloader_core_library-0.0.6/src/bootloader/ue/model/ue_asset.py
+-rw-r--r--   0        0        0     1060 1970-01-01 00:00:00.000000 bootloader_core_library-0.0.6/setup.py
+-rw-r--r--   0        0        0     1134 1970-01-01 00:00:00.000000 bootloader_core_library-0.0.6/PKG-INFO
```

### Comparing `bootloader_core_library-0.0.5/CHANGELOG.md` & `bootloader_core_library-0.0.6/CHANGELOG.md`

 * *Files 17% similar despite different names*

```diff
@@ -2,19 +2,22 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), 
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 
+## [0.0.6] - 2024-08-02
+### Added
+- Add the properties "object_status", "references", "tags", "update_time", and "version_code"
+
 ## [0.0.5] - 2024-08-02
 ### Added
 - Allow the properties "asset_name" and "package_name" to be updated
 
-
 ## [0.0.4] - 2024-08-02
 ### Fixed
 - Fix the property "asset" of the class "UnrealEngineAbstractAssetFile"
 
 ## [0.0.3] - 2024-08-02
 ### Changed
 - Update Unreal Engine classes to support both asset's database record and file system
```

### Comparing `bootloader_core_library-0.0.5/LICENSE.md` & `bootloader_core_library-0.0.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `bootloader_core_library-0.0.5/pyproject.toml` & `bootloader_core_library-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ]
 keywords = ["core", "library"]
 license = "SEE LICENSE IN <LICENSE.md>"
 name = "bootloader-core-library"
 packages = [{include = "bootloader", from = "src"}]
 readme = "README.md"
 repository = "https://github.com/bootloader-studio/bootloader-core-python-library"
-version = "0.0.5"
+version = "0.0.6"
 
 [tool.poetry.dependencies]
 perseus-core-library = "^1.19.4"
 python = "^3.10"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `bootloader_core_library-0.0.5/src/bootloader/__init__.py` & `bootloader_core_library-0.0.6/src/bootloader/__init__.py`

 * *Files identical despite different names*

### Comparing `bootloader_core_library-0.0.5/src/bootloader/ue/__init__.py` & `bootloader_core_library-0.0.6/src/bootloader/ue/__init__.py`

 * *Files identical despite different names*

### Comparing `bootloader_core_library-0.0.5/src/bootloader/ue/constant/__init__.py` & `bootloader_core_library-0.0.6/src/bootloader/ue/constant/__init__.py`

 * *Files identical despite different names*

### Comparing `bootloader_core_library-0.0.5/src/bootloader/ue/constant/ue_asset.py` & `bootloader_core_library-0.0.6/src/bootloader/ue/constant/ue_asset.py`

 * *Files identical despite different names*

### Comparing `bootloader_core_library-0.0.5/src/bootloader/ue/model/__init__.py` & `bootloader_core_library-0.0.6/src/bootloader/ue/model/__init__.py`

 * *Files identical despite different names*

### Comparing `bootloader_core_library-0.0.5/src/bootloader/ue/model/ue_asset.py` & `bootloader_core_library-0.0.6/src/bootloader/ue/model/ue_asset.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 import json
 import logging
 import os
 from abc import abstractmethod
 from pathlib import Path
 from uuid import UUID
 
+from majormode.perseus.constant.obj import ObjectStatus
+from majormode.perseus.model.date import ISO8601DateTime
 from majormode.perseus.utils import cast
 
 from bootloader.ue.constant.ue_asset import ASSET_CLASS_NAME_MAPPING
 from bootloader.ue.constant.ue_asset import UnrealEngineAssetClass
 
 
 class UnrealEngineAsset:
@@ -50,15 +52,20 @@
 
     def __init__(
             self,
             asset_name: str,
             asset_class_path: str,
             package_name: str,
             dependencies: list[str] or None,
-            asset_id: UUID = None):
+            asset_id: UUID = None,
+            object_status: ObjectStatus = None,
+            references: list[str] or None = None,
+            tags: list[str] or None = None,
+            update_time: ISO8601DateTime or None = None,
+            version_code: int or None = None):
         """
         Build a new {@link UAsset}.
 
 
         :param asset_name: The name of the asset without the package.
 
         :param asset_class_path: The path name of the asset’s class.
@@ -67,20 +74,41 @@
             found.
 
         :param dependencies: The list of names of the packages that the asset
             depends on.
 
         :param asset_id: The identification of the asset, when already
             registered to the back-end platform.
+
+        :param object_status: The current status of the asset.
+
+        :param references: The list of pacakge names of the asset that depend
+            on this asset.
+
+        :param tags: The list of tags associated with the asset.
+
+        :param update_time: The time of the most recent modification of some
+            mutable attributes of the asset, such as its status, its list of
+            tags, and its picture.
+
+        :param version_code: A positive integer used as an internal version
+            number.  This number helps determine whether one version is more
+            recent than another, with higher numbers indicating more recent
+            versions.
         """
         self.__asset_id = asset_id
         self.__asset_name = asset_name
         self.__asset_class_path = asset_class_path
         self.__package_name = package_name
         self.__dependencies = dependencies
+        self.__references = references
+        self.__tags = tags
+        self.__object_status = object_status
+        self.__update_time = update_time
+        self.__version_code = version_code
 
     @property
     def asset_class(self) -> UnrealEngineAssetClass:
         """
         Return the asset's class.
 
         For example, the class of a `/Script/Engine/SkeletalMesh` asset is
@@ -181,21 +209,23 @@
         return UnrealEngineAsset(
             payload['asset_name'],
             payload['asset_class_path'],
             payload['package_name'],
             payload['dependencies']
         )
 
-    def to_json(self) -> any:
-        return {
-            "asset_name": self.__asset_name,
-            "asset_class_path": self.__asset_class_path,
-            "package_name": self.__package_name,
-            "dependencies": self.__dependencies
-        }
+    @property
+    def object_status(self) -> ObjectStatus or None:
+        """
+        Return The current status of the asset.
+
+
+        :return: The current status of the asset.
+        """
+        return self.__object_status
 
     @property
     def package_name(self) -> str:
         """
         Return the name of the package in which the asset is found.
 
 
@@ -210,14 +240,72 @@
 
 
         :param package_name: The new name of the asset's package.
         """
         logging.debug(f"Changing the package name of the asset {self.__asset_name} with {package_name}")
         self.__package_name = package_name
 
+    @property
+    def references(self) -> list[str] or None:
+        """
+        Return the list of names of the packages of the assets that reference
+        this asset.
+
+
+        :return: The list of names of the packages of the assets that
+            reference this asset.
+        """
+        return self.__references
+
+    @property
+    def tags(self) -> list[str] or None:
+        """
+        Return the list of tags associated to the asset.
+
+
+        :return: The list of tags associated with the asset.
+        """
+        return self.__tags
+
+    def to_json(self) -> any:
+        return {
+            "asset_name": self.__asset_name,
+            "asset_class_path": self.__asset_class_path,
+            "package_name": self.__package_name,
+            "dependencies": self.__dependencies
+        }
+
+    @property
+    def update_time(self) -> ISO8601DateTime or None:
+        """
+        Return the time of the most recent modification of some mutable
+        attributes of the asset.
+
+        The mutable attributes of the asset are its status, the list of
+        its tags, and its picture.
+
+
+        :return: The time of the most recent modification of some mutable
+            attributes of the asset.
+        """
+        return self.__update_time
+
+    @property
+    def version_code(self) -> int or None:
+        """
+        Return a positive integer used as an internal version number.
+
+        This number helps determine whether one version is more recent than
+        another, with higher numbers indicating more recent versions.
+
+
+        :return: A positive integer used as an internal version number.
+        """
+        return self.__version_code
+
 
 class UnrealEngineAbstractAssetFile:
     def __eq__(self, other: UnrealEngineAbstractAssetFile):
         """
         Check whether this asset is the same as another asset.
 
         Two assets are equivalent if they have the same name, the same class,
```

### Comparing `bootloader_core_library-0.0.5/setup.py` & `bootloader_core_library-0.0.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['perseus-core-library>=1.19.4,<2.0.0']
 
 setup_kwargs = {
     'name': 'bootloader-core-library',
-    'version': '0.0.5',
+    'version': '0.0.6',
     'description': 'Repository of reusable Python components to be shared by Python projects using the Bootloader services',
     'long_description': '# Bootloader Core Python Library\n\nRepository of reusable Python components to be shared by Python projects using the Bootloader services.\n',
     'author': 'Daniel CAUNE',
     'author_email': 'daniel@bootloader.studio',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/bootloader-studio/bootloader-core-python-library',
```

### Comparing `bootloader_core_library-0.0.5/PKG-INFO` & `bootloader_core_library-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bootloader-core-library
-Version: 0.0.5
+Version: 0.0.6
 Summary: Repository of reusable Python components to be shared by Python projects using the Bootloader services
 Home-page: https://github.com/bootloader-studio/bootloader-core-python-library
 License: SEE LICENSE IN <LICENSE.md>
 Keywords: core,library
 Author: Daniel CAUNE
 Author-email: daniel@bootloader.studio
 Requires-Python: >=3.10,<4.0
```

