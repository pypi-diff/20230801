# Comparing `tmp/bootloader_core_library-0.0.3.tar.gz` & `tmp/bootloader_core_library-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bootloader_core_library-0.0.3.tar", max compression
+gzip compressed data, was "bootloader_core_library-0.0.4.tar", max compression
```

## Comparing `bootloader_core_library-0.0.3.tar` & `bootloader_core_library-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      523 2023-08-01 13:05:57.452327 bootloader_core_library-0.0.3/CHANGELOG.md
--rw-r--r--   0        0        0      761 2023-03-31 11:22:24.297536 bootloader_core_library-0.0.3/LICENSE.md
--rw-r--r--   0        0        0      138 2023-08-01 09:48:11.340859 bootloader_core_library-0.0.3/README.md
--rw-r--r--   0        0        0      905 2023-08-01 13:05:25.242947 bootloader_core_library-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      859 2023-03-31 11:21:05.979756 bootloader_core_library-0.0.3/src/bootloader/__init__.py
--rw-r--r--   0        0        0      859 2023-03-31 11:21:05.992853 bootloader_core_library-0.0.3/src/bootloader/ue/__init__.py
--rw-r--r--   0        0        0      859 2023-03-31 11:21:05.975392 bootloader_core_library-0.0.3/src/bootloader/ue/constant/__init__.py
--rw-r--r--   0        0        0    17273 2023-08-01 10:14:45.867545 bootloader_core_library-0.0.3/src/bootloader/ue/constant/ue_asset.py
--rw-r--r--   0        0        0      859 2023-03-31 11:21:05.975392 bootloader_core_library-0.0.3/src/bootloader/ue/model/__init__.py
--rw-r--r--   0        0        0    11440 2023-08-01 13:04:52.663967 bootloader_core_library-0.0.3/src/bootloader/ue/model/ue_asset.py
--rw-r--r--   0        0        0     1060 1970-01-01 00:00:00.000000 bootloader_core_library-0.0.3/setup.py
--rw-r--r--   0        0        0     1134 1970-01-01 00:00:00.000000 bootloader_core_library-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      630 2023-08-01 13:38:29.825316 bootloader_core_library-0.0.4/CHANGELOG.md
+-rw-r--r--   0        0        0      761 2023-03-31 11:22:24.297536 bootloader_core_library-0.0.4/LICENSE.md
+-rw-r--r--   0        0        0      138 2023-08-01 09:48:11.340859 bootloader_core_library-0.0.4/README.md
+-rw-r--r--   0        0        0      905 2023-08-01 13:38:34.172254 bootloader_core_library-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      859 2023-03-31 11:21:05.979756 bootloader_core_library-0.0.4/src/bootloader/__init__.py
+-rw-r--r--   0        0        0      859 2023-03-31 11:21:05.992853 bootloader_core_library-0.0.4/src/bootloader/ue/__init__.py
+-rw-r--r--   0        0        0      859 2023-03-31 11:21:05.975392 bootloader_core_library-0.0.4/src/bootloader/ue/constant/__init__.py
+-rw-r--r--   0        0        0    17273 2023-08-01 10:14:45.867545 bootloader_core_library-0.0.4/src/bootloader/ue/constant/ue_asset.py
+-rw-r--r--   0        0        0      859 2023-03-31 11:21:05.975392 bootloader_core_library-0.0.4/src/bootloader/ue/model/__init__.py
+-rw-r--r--   0        0        0    11454 2023-08-01 13:37:50.641657 bootloader_core_library-0.0.4/src/bootloader/ue/model/ue_asset.py
+-rw-r--r--   0        0        0     1060 1970-01-01 00:00:00.000000 bootloader_core_library-0.0.4/setup.py
+-rw-r--r--   0        0        0     1134 1970-01-01 00:00:00.000000 bootloader_core_library-0.0.4/PKG-INFO
```

### Comparing `bootloader_core_library-0.0.3/CHANGELOG.md` & `bootloader_core_library-0.0.4/CHANGELOG.md`

 * *Files 20% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), 
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 
+## [0.0.4] - 2024-08-02
+### Fixed
+- Fix the property "asset" of the class "UnrealEngineAbstractAssetFile"
+
 ## [0.0.3] - 2024-08-02
 ### Changed
 - Update Unreal Engine classes to support both asset's database record and file system
 
 ## [0.0.2] - 2024-08-02
 ### Changed
 - Update both Unreal Engine class and class enumeration
```

### Comparing `bootloader_core_library-0.0.3/LICENSE.md` & `bootloader_core_library-0.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `bootloader_core_library-0.0.3/pyproject.toml` & `bootloader_core_library-0.0.4/pyproject.toml`

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
-version = "0.0.3"
+version = "0.0.4"
 
 [tool.poetry.dependencies]
 perseus-core-library = "^1.19.4"
 python = "^3.10"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `bootloader_core_library-0.0.3/src/bootloader/__init__.py` & `bootloader_core_library-0.0.4/src/bootloader/__init__.py`

 * *Files identical despite different names*

### Comparing `bootloader_core_library-0.0.3/src/bootloader/ue/__init__.py` & `bootloader_core_library-0.0.4/src/bootloader/ue/__init__.py`

 * *Files identical despite different names*

### Comparing `bootloader_core_library-0.0.3/src/bootloader/ue/constant/__init__.py` & `bootloader_core_library-0.0.4/src/bootloader/ue/constant/__init__.py`

 * *Files identical despite different names*

### Comparing `bootloader_core_library-0.0.3/src/bootloader/ue/constant/ue_asset.py` & `bootloader_core_library-0.0.4/src/bootloader/ue/constant/ue_asset.py`

 * *Files identical despite different names*

### Comparing `bootloader_core_library-0.0.3/src/bootloader/ue/model/__init__.py` & `bootloader_core_library-0.0.4/src/bootloader/ue/model/__init__.py`

 * *Files identical despite different names*

### Comparing `bootloader_core_library-0.0.3/src/bootloader/ue/model/ue_asset.py` & `bootloader_core_library-0.0.4/src/bootloader/ue/model/ue_asset.py`

 * *Files 1% similar despite different names*

```diff
@@ -215,14 +215,15 @@
             self,
             asset: UnrealEngineAsset):
         """
         Build a new {@link UAsset}.
         """
         self.__asset = asset
 
+    @property
     def asset(self) -> UnrealEngineAsset:
         """
         Return the information of the asset contained in this file.
 
 
         :return: An asset.
         """
```

### Comparing `bootloader_core_library-0.0.3/setup.py` & `bootloader_core_library-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['perseus-core-library>=1.19.4,<2.0.0']
 
 setup_kwargs = {
     'name': 'bootloader-core-library',
-    'version': '0.0.3',
+    'version': '0.0.4',
     'description': 'Repository of reusable Python components to be shared by Python projects using the Bootloader services',
     'long_description': '# Bootloader Core Python Library\n\nRepository of reusable Python components to be shared by Python projects using the Bootloader services.\n',
     'author': 'Daniel CAUNE',
     'author_email': 'daniel@bootloader.studio',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/bootloader-studio/bootloader-core-python-library',
```

### Comparing `bootloader_core_library-0.0.3/PKG-INFO` & `bootloader_core_library-0.0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bootloader-core-library
-Version: 0.0.3
+Version: 0.0.4
 Summary: Repository of reusable Python components to be shared by Python projects using the Bootloader services
 Home-page: https://github.com/bootloader-studio/bootloader-core-python-library
 License: SEE LICENSE IN <LICENSE.md>
 Keywords: core,library
 Author: Daniel CAUNE
 Author-email: daniel@bootloader.studio
 Requires-Python: >=3.10,<4.0
```

