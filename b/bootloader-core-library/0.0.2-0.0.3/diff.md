# Comparing `tmp/bootloader_core_library-0.0.2.tar.gz` & `tmp/bootloader_core_library-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bootloader_core_library-0.0.2.tar", max compression
+gzip compressed data, was "bootloader_core_library-0.0.3.tar", max compression
```

## Comparing `bootloader_core_library-0.0.2.tar` & `bootloader_core_library-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      399 2023-08-01 10:23:39.349344 bootloader_core_library-0.0.2/CHANGELOG.md
--rw-r--r--   0        0        0      761 2023-03-31 11:22:24.297536 bootloader_core_library-0.0.2/LICENSE.md
--rw-r--r--   0        0        0      138 2023-08-01 09:48:11.340859 bootloader_core_library-0.0.2/README.md
--rw-r--r--   0        0        0      905 2023-08-01 10:23:48.453487 bootloader_core_library-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      859 2023-03-31 11:21:05.979756 bootloader_core_library-0.0.2/src/bootloader/__init__.py
--rw-r--r--   0        0        0      859 2023-03-31 11:21:05.992853 bootloader_core_library-0.0.2/src/bootloader/ue/__init__.py
--rw-r--r--   0        0        0      859 2023-03-31 11:21:05.975392 bootloader_core_library-0.0.2/src/bootloader/ue/constant/__init__.py
--rw-r--r--   0        0        0    17273 2023-08-01 10:14:45.867545 bootloader_core_library-0.0.2/src/bootloader/ue/constant/ue_asset.py
--rw-r--r--   0        0        0      859 2023-03-31 11:21:05.975392 bootloader_core_library-0.0.2/src/bootloader/ue/model/__init__.py
--rw-r--r--   0        0        0    11251 2023-08-01 10:22:39.615693 bootloader_core_library-0.0.2/src/bootloader/ue/model/ue_asset.py
--rw-r--r--   0        0        0     1060 1970-01-01 00:00:00.000000 bootloader_core_library-0.0.2/setup.py
--rw-r--r--   0        0        0     1134 1970-01-01 00:00:00.000000 bootloader_core_library-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      523 2023-08-01 13:05:57.452327 bootloader_core_library-0.0.3/CHANGELOG.md
+-rw-r--r--   0        0        0      761 2023-03-31 11:22:24.297536 bootloader_core_library-0.0.3/LICENSE.md
+-rw-r--r--   0        0        0      138 2023-08-01 09:48:11.340859 bootloader_core_library-0.0.3/README.md
+-rw-r--r--   0        0        0      905 2023-08-01 13:05:25.242947 bootloader_core_library-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      859 2023-03-31 11:21:05.979756 bootloader_core_library-0.0.3/src/bootloader/__init__.py
+-rw-r--r--   0        0        0      859 2023-03-31 11:21:05.992853 bootloader_core_library-0.0.3/src/bootloader/ue/__init__.py
+-rw-r--r--   0        0        0      859 2023-03-31 11:21:05.975392 bootloader_core_library-0.0.3/src/bootloader/ue/constant/__init__.py
+-rw-r--r--   0        0        0    17273 2023-08-01 10:14:45.867545 bootloader_core_library-0.0.3/src/bootloader/ue/constant/ue_asset.py
+-rw-r--r--   0        0        0      859 2023-03-31 11:21:05.975392 bootloader_core_library-0.0.3/src/bootloader/ue/model/__init__.py
+-rw-r--r--   0        0        0    11440 2023-08-01 13:04:52.663967 bootloader_core_library-0.0.3/src/bootloader/ue/model/ue_asset.py
+-rw-r--r--   0        0        0     1060 1970-01-01 00:00:00.000000 bootloader_core_library-0.0.3/setup.py
+-rw-r--r--   0        0        0     1134 1970-01-01 00:00:00.000000 bootloader_core_library-0.0.3/PKG-INFO
```

### Comparing `bootloader_core_library-0.0.2/LICENSE.md` & `bootloader_core_library-0.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `bootloader_core_library-0.0.2/pyproject.toml` & `bootloader_core_library-0.0.3/pyproject.toml`

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
-version = "0.0.2"
+version = "0.0.3"
 
 [tool.poetry.dependencies]
 perseus-core-library = "^1.19.4"
 python = "^3.10"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `bootloader_core_library-0.0.2/src/bootloader/__init__.py` & `bootloader_core_library-0.0.3/src/bootloader/__init__.py`

 * *Files identical despite different names*

### Comparing `bootloader_core_library-0.0.2/src/bootloader/ue/__init__.py` & `bootloader_core_library-0.0.3/src/bootloader/ue/__init__.py`

 * *Files identical despite different names*

### Comparing `bootloader_core_library-0.0.2/src/bootloader/ue/constant/__init__.py` & `bootloader_core_library-0.0.3/src/bootloader/ue/constant/__init__.py`

 * *Files identical despite different names*

### Comparing `bootloader_core_library-0.0.2/src/bootloader/ue/constant/ue_asset.py` & `bootloader_core_library-0.0.3/src/bootloader/ue/constant/ue_asset.py`

 * *Files identical despite different names*

### Comparing `bootloader_core_library-0.0.2/src/bootloader/ue/model/__init__.py` & `bootloader_core_library-0.0.3/src/bootloader/ue/model/__init__.py`

 * *Files identical despite different names*

### Comparing `bootloader_core_library-0.0.2/src/bootloader/ue/model/ue_asset.py` & `bootloader_core_library-0.0.3/src/bootloader/ue/model/ue_asset.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 from __future__ import annotations
 
 import hashlib
 import json
 import logging
 import os
+from abc import abstractmethod
 from pathlib import Path
 from uuid import UUID
 
 from majormode.perseus.utils import cast
 
 from bootloader.ue.constant.ue_asset import ASSET_CLASS_NAME_MAPPING
 from bootloader.ue.constant.ue_asset import UnrealEngineAssetClass
@@ -30,66 +31,56 @@
 
 class UnrealEngineAsset:
     def __eq__(self, other: UnrealEngineAsset):
         """
         Check whether this asset is the same as another asset.
 
         Two assets are equivalent if they have the same name, the same class,
-        the same package name, and the same file's checksum.
+        and the same package name.
 
 
         :param other: Another asset.
 
 
         :return: ``True`` if the two assets are the same; ``False`` otherwise.
         """
         return other is not None \
-            and self.__file_checksum == other.file_checksum \
             and self.__asset_class_path == other.asset_class_path \
             and self.__asset_name == other.asset_name \
             and self.__package_name == other.package_name
 
     def __init__(
             self,
             asset_name: str,
             asset_class_path: str,
             package_name: str,
             dependencies: list[str] or None,
-            file_size: int,
-            file_checksum: str,
             asset_id: UUID = None):
         """
         Build a new {@link UAsset}.
 
 
         :param asset_name: The name of the asset without the package.
 
         :param asset_class_path: The path name of the asset’s class.
 
         :param package_name: The name of the package in which the asset is
             found.
 
-        :param dependencies: The list of package names of the assets that this
-            asset depends on.
-
-        :param file_size: The size in bytes of the asset file.
-
-        :param file_checksum: The SHA256 message digest of the binary data of
-            the asset file.
+        :param dependencies: The list of names of the packages that the asset
+            depends on.
 
         :param asset_id: The identification of the asset, when already
             registered to the back-end platform.
         """
         self.__asset_id = asset_id
         self.__asset_name = asset_name
         self.__asset_class_path = asset_class_path
         self.__package_name = package_name
         self.__dependencies = dependencies
-        self.__file_size = file_size
-        self.__file_checksum = file_checksum
 
     @property
     def asset_class(self) -> UnrealEngineAssetClass:
         """
         Return the asset's class.
 
         For example, the class of a `/Script/Engine/SkeletalMesh` asset is
@@ -159,211 +150,251 @@
         :return: The name of the asset without the package.
         """
         return self.__asset_name
 
     @property
     def dependencies(self) -> list[str] or None:
         """
-        Return the list of the package names of the assets that this asset
-        depends on.
+        Return the list of names of the packages that the asset depends on.
 
 
-        :return: The list of package names of the assets that this asset
-            depends on.
+        :return: The list of names of the packages that the asset depends on.
         """
         return self.__dependencies
 
-    @property
-    def file_checksum(self) -> str:
-        return self.__file_checksum
-
-    @property
-    def file_size(self) -> int:
-        return self.__file_size
-
     @staticmethod
-    def from_json(payload: any) -> UnrealEngineAsset:
+    def from_json(payload: any):
+        if isinstance(payload, str):
+            payload = json.loads(payload)
+
+        # @todo: Check data consistency (type, path, list of strings, etc.)
         return UnrealEngineAsset(
             payload['asset_name'],
             payload['asset_class_path'],
             payload['package_name'],
-            payload.get('dependencies'),
-            payload['file_size'],
-            payload['file_checksum']
+            payload['dependencies']
         )
 
     def to_json(self) -> any:
         return {
-            'asset_name': self.__asset_name,
-            'asset_class_path': self.__asset_class_path,
-            'package_name': self.__package_name,
-            'dependencies': self.__dependencies,
-            'file_size': self.__file_size,
+            "asset_name": self.__asset_name,
+            "asset_class_path": self.__asset_class_path,
+            "package_name": self.__package_name,
+            "dependencies": self.__dependencies
         }
 
     @property
     def package_name(self) -> str:
         """
         Return the name of the package in which the asset is found.
 
 
         :return: The name of the package in which the asset is found.
         """
         return self.__package_name
 
 
-# class UnrealEngineAsset:
-#     def __init__(
-#             self,
-#             asset_name: str,
-#             asset_class_path: str,
-#             package_name: str,
-#             dependencies: list[str] or None):
-#         """
-#         Build a new {@link UAsset}.
-#
-#
-#         :param asset_name: The name of the asset without the package.
-#
-#         :param asset_class_path: The path name of the asset’s class.
-#
-#         :param package_name: The name of the package in which the asset is
-#             found.
-#
-#         :param dependencies: The list of names of the packages that the asset
-#             depends on.
-#         """
-#         self.__asset_name = asset_name
-#         self.__asset_class_path = asset_class_path
-#         self.__package_name = package_name
-#         self.__dependencies = dependencies
-#
-#     @property
-#     def asset_class_path(self) -> str:
-#         """
-#         Return the path name of the asset's class.
-#
-#         Examples:
-#
-#         ```text
-#         /Script/Engine/SkeletalMesh
-#         /Script/Engine/Skeleton
-#         /Script/Engine/Texture2D
-#         ```
-#
-#         :return: The path name of the asset's class.
-#         """
-#         return self.__asset_class_path
-#
-#     @property
-#     def asset_name(self) -> str:
-#         """
-#         Return the name of the asset.
-#
-#
-#         :return: The name of the asset without the package.
-#         """
-#         return self.__asset_name
-#
-#     @property
-#     def dependencies(self) -> list[str] or None:
-#         """
-#         Return the list of names of the packages that the asset depends on.
-#
-#
-#         :return: The list of names of the packages that the asset depends on.
-#         """
-#         return self.__dependencies
-#
-#     @staticmethod
-#     def from_json(payload: any):
-#         if isinstance(payload, str):
-#             payload = json.loads(payload)
-#
-#         # @todo: Check data consistency (type, path, list of strings, etc.)
-#         return UnrealEngineAsset(
-#             payload['asset_name'],
-#             payload['asset_class_path'],
-#             payload['package_name'],
-#             payload['dependencies']
-#         )
-#
-#     def to_json(self) -> any:
-#         return {
-#             "asset_name": self.__asset_name,
-#             "asset_class_path": self.__asset_class_path,
-#             "package_name": self.__package_name,
-#             "dependencies": self.__dependencies
-#         }
-#
-#     @property
-#     def package_name(self) -> str:
-#         """
-#         Return the name of the package in which the asset is found.
-#
-#
-#         :return: The name of the package in which the asset is found.
-#         """
-#         return self.__package_name
-#
-#
-# class UAssetFile:
-#     FILE_READ_BLOCK_SIZE = 4096
-#
-#     def __init__(
-#             self,
-#             asset,
-#             file_path_name):
-#         if not os.path.exists(file_path_name):
-#             error_message = f"The file {file_path_name} of the asset {asset.asset_name} doesn't exist"
-#             logging.error(error_message)
-#             raise FileNotFoundError(error_message)
-#
-#         self.__asset = asset
-#         self.__file_path_name = file_path_name
-#         self.__file_status = None  # This attribute is lazy loaded (cf. property `file_status`)
-#         self.__file_checksum = None  # This attribute is lazy loaded (cf. property `file_checksum`)
-#
-#     def __calculate_file_checksum(self) -> str:
-#         sha256_hash = hashlib.sha256()
-#
-#         with open(self.__file_path_name, 'rb') as fd:
-#             # Read and update hash string value in blocks of bytes.
-#             for byte_block in iter(lambda: fd.read(self.FILE_READ_BLOCK_SIZE), b''):
-#                 sha256_hash.update(byte_block)
-#
-#         return sha256_hash.hexdigest()
-#
-#     @property
-#     def asset(self) -> UnrealEngineAsset:
-#         return self.__asset
-#
-#     @property
-#     def file_checksum(self) -> str:
-#         if self.__file_checksum is None:
-#             self.__file_checksum = self.__calculate_file_checksum()
-#
-#         return self.__file_checksum
-#
-#     @property
-#     def file_path_name(self) -> Path:
-#         return self.__file_path_name
-#
-#     @property
-#     def file_status(self) -> os.stat_result:
-#         """
-#         Return the detailed status of the asset file.
-#
-#
-#         :return: The detailed status of the asset file.
-#         """
-#         if self.__file_status is None:
-#             self.__file_status = Path.stat(self.__file_path_name)
-#
-#         return self.__file_status
-#
-#     def to_json(self) -> any:
-#         payload = self.__asset.to_json()
-#         payload['file_size'] = self.file_status.st_size
-#         payload['file_checksum'] = self.file_checksum
-#         return payload
+class UnrealEngineAbstractAssetFile:
+    def __eq__(self, other: UnrealEngineAbstractAssetFile):
+        """
+        Check whether this asset is the same as another asset.
+
+        Two assets are equivalent if they have the same name, the same class,
+        the same package name, and the same file's checksum.
+
+
+        :param other: Another asset.
+
+
+        :return: ``True`` if the two assets are the same; ``False`` otherwise.
+        """
+        return other is not None \
+            and self.file_checksum == other.file_checksum \
+            and self.__asset == other.asset
+
+    def __init__(
+            self,
+            asset: UnrealEngineAsset):
+        """
+        Build a new {@link UAsset}.
+        """
+        self.__asset = asset
+
+    def asset(self) -> UnrealEngineAsset:
+        """
+        Return the information of the asset contained in this file.
+
+
+        :return: An asset.
+        """
+        return self.__asset
+
+    @property
+    @abstractmethod
+    def file_checksum(self) -> str:
+        """
+        Return the SHA256 message digest of the binary data of the asset file.
+
+
+        :return: The SHA256 message digest of the binary data of the asset
+            file.
+        """
+        pass
+
+    @property
+    @abstractmethod
+    def file_size(self) -> int:
+        """
+        Return the size of the asset file.
+
+
+        :return: The size in bytes of the asset file.
+        """
+        pass
+
+    def to_json(self) -> any:
+        """
+        Serialize the asset's information to a JSON expression.
+
+
+        :return: A JSON expression representing the asset's information.
+        """
+        payload = self.__asset.to_json()
+        payload['file_size'] = self.file_size
+        payload['file_checksum'] = self.file_checksum
+        return payload
+
+
+class UnrealEngineRecordAssetFile(UnrealEngineAbstractAssetFile):
+    """
+    Represent the information of an asset as registered in a database.
+    """
+    def __init__(
+            self,
+            asset: UnrealEngineAsset,
+            file_size: int,
+            file_checksum: str):
+        """
+        :param asset:
 
+        :param file_checksum: The SHA256 message digest of the binary data of
+            the asset file.
+
+        """
+        super().__init__(asset)
+        self.__file_checksum = file_checksum
+        self.__file_size = file_size
+
+    @property
+    def file_checksum(self) -> str:
+        """
+        Return the SHA256 message digest of the binary data of the asset file.
+
+
+        :return: The SHA256 message digest of the binary data of the asset
+            file.
+        """
+        return self.__file_checksum
+
+    @property
+    def file_size(self) -> int:
+        """
+        Return the size of the asset file.
+
+
+        :return: The size in bytes of the asset file.
+        """
+        return self.__file_size
+
+    @staticmethod
+    def from_json(payload: any) -> UnrealEngineRecordAssetFile:
+        """
+        Return an asset as stored in a database record.
+
+        :param payload: The JSON data of the asset.
+
+
+        :return: An asset.
+        """
+        asset = UnrealEngineAsset.from_json(payload)
+        return UnrealEngineRecordAssetFile(
+            asset,
+            payload['file_size'],
+            payload['file_checksum']
+        )
+
+
+class UnrealEngineRealAssetFile(UnrealEngineAbstractAssetFile):
+    """
+    Represent the file of an asset stored on the file system.
+    """
+    FILE_READ_BLOCK_SIZE = 4096
+
+    def __init__(
+            self,
+            asset: UnrealEngineAsset,
+            file_path_name: Path):
+        super().__init__(asset)
+
+        if not os.path.exists(file_path_name):
+            error_message = f"The file {file_path_name} of the asset {asset.asset_name} doesn't exist"
+            logging.error(error_message)
+            raise FileNotFoundError(error_message)
+
+        file_status = Path.stat(file_path_name)
+        self.__file_size = file_status.st_size
+
+        self.__asset = asset
+        self.__file_path_name = file_path_name
+        self.__file_checksum = None  # This attribute is lazy loaded (cf. property `file_checksum`)
+
+    def __calculate_file_checksum(self) -> str:
+        """
+        Calculate the SHA256 message digest of the binary data of the asset
+        file.
+
+
+        :return: The SHA256 message digest of the binary data of the asset
+            file.
+        """
+        sha256_hash = hashlib.sha256()
+
+        with open(self.__file_path_name, 'rb') as fd:
+            # Read and update hash string value in blocks of bytes.
+            for byte_block in iter(lambda: fd.read(self.FILE_READ_BLOCK_SIZE), b''):
+                sha256_hash.update(byte_block)
+
+        return sha256_hash.hexdigest()
+
+    @property
+    def file_checksum(self) -> str:
+        """
+        Return the SHA256 message digest of the binary data of the asset file.
+
+
+        :return: The SHA256 message digest of the binary data of the asset
+            file.
+        """
+        if self.__file_checksum is None:
+            self.__file_checksum = self.__calculate_file_checksum()
+
+        return self.__file_checksum
+
+    @property
+    def file_path_name(self) -> Path:
+        """
+        Return the path and name of the asset's file.
+
+
+        :return: The path and name of the asset's file.
+        """
+        return self.__file_path_name
+
+    @property
+    def file_size(self) -> int:
+        """
+        Return the size of the asset file.
+
+
+        :return: The size in bytes of the asset file.
+        """
+        return self.__file_size
```

### Comparing `bootloader_core_library-0.0.2/setup.py` & `bootloader_core_library-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['perseus-core-library>=1.19.4,<2.0.0']
 
 setup_kwargs = {
     'name': 'bootloader-core-library',
-    'version': '0.0.2',
+    'version': '0.0.3',
     'description': 'Repository of reusable Python components to be shared by Python projects using the Bootloader services',
     'long_description': '# Bootloader Core Python Library\n\nRepository of reusable Python components to be shared by Python projects using the Bootloader services.\n',
     'author': 'Daniel CAUNE',
     'author_email': 'daniel@bootloader.studio',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/bootloader-studio/bootloader-core-python-library',
```

### Comparing `bootloader_core_library-0.0.2/PKG-INFO` & `bootloader_core_library-0.0.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bootloader-core-library
-Version: 0.0.2
+Version: 0.0.3
 Summary: Repository of reusable Python components to be shared by Python projects using the Bootloader services
 Home-page: https://github.com/bootloader-studio/bootloader-core-python-library
 License: SEE LICENSE IN <LICENSE.md>
 Keywords: core,library
 Author: Daniel CAUNE
 Author-email: daniel@bootloader.studio
 Requires-Python: >=3.10,<4.0
```

