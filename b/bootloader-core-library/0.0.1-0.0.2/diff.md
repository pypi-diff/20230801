# Comparing `tmp/bootloader_core_library-0.0.1.tar.gz` & `tmp/bootloader_core_library-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bootloader_core_library-0.0.1.tar", max compression
+gzip compressed data, was "bootloader_core_library-0.0.2.tar", max compression
```

## Comparing `bootloader_core_library-0.0.1.tar` & `bootloader_core_library-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      306 2023-08-01 09:50:06.283805 bootloader_core_library-0.0.1/CHANGELOG.md
--rw-r--r--   0        0        0      761 2023-03-31 11:22:24.297536 bootloader_core_library-0.0.1/LICENSE.md
--rw-r--r--   0        0        0      138 2023-08-01 09:48:11.340859 bootloader_core_library-0.0.1/README.md
--rw-r--r--   0        0        0      905 2023-08-01 10:03:14.763803 bootloader_core_library-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      859 2023-03-31 11:21:05.979756 bootloader_core_library-0.0.1/src/bootloader/__init__.py
--rw-r--r--   0        0        0      859 2023-03-31 11:21:05.992853 bootloader_core_library-0.0.1/src/bootloader/ue/__init__.py
--rw-r--r--   0        0        0      859 2023-03-31 11:21:05.975392 bootloader_core_library-0.0.1/src/bootloader/ue/constant/__init__.py
--rw-r--r--   0        0        0     4797 2023-04-25 08:28:27.210905 bootloader_core_library-0.0.1/src/bootloader/ue/constant/ue_asset.py
--rw-r--r--   0        0        0      859 2023-03-31 11:21:05.975392 bootloader_core_library-0.0.1/src/bootloader/ue/model/__init__.py
--rw-r--r--   0        0        0     5358 2023-06-30 03:57:41.936347 bootloader_core_library-0.0.1/src/bootloader/ue/model/ue_asset.py
--rw-r--r--   0        0        0     1060 1970-01-01 00:00:00.000000 bootloader_core_library-0.0.1/setup.py
--rw-r--r--   0        0        0     1134 1970-01-01 00:00:00.000000 bootloader_core_library-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      399 2023-08-01 10:23:39.349344 bootloader_core_library-0.0.2/CHANGELOG.md
+-rw-r--r--   0        0        0      761 2023-03-31 11:22:24.297536 bootloader_core_library-0.0.2/LICENSE.md
+-rw-r--r--   0        0        0      138 2023-08-01 09:48:11.340859 bootloader_core_library-0.0.2/README.md
+-rw-r--r--   0        0        0      905 2023-08-01 10:23:48.453487 bootloader_core_library-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      859 2023-03-31 11:21:05.979756 bootloader_core_library-0.0.2/src/bootloader/__init__.py
+-rw-r--r--   0        0        0      859 2023-03-31 11:21:05.992853 bootloader_core_library-0.0.2/src/bootloader/ue/__init__.py
+-rw-r--r--   0        0        0      859 2023-03-31 11:21:05.975392 bootloader_core_library-0.0.2/src/bootloader/ue/constant/__init__.py
+-rw-r--r--   0        0        0    17273 2023-08-01 10:14:45.867545 bootloader_core_library-0.0.2/src/bootloader/ue/constant/ue_asset.py
+-rw-r--r--   0        0        0      859 2023-03-31 11:21:05.975392 bootloader_core_library-0.0.2/src/bootloader/ue/model/__init__.py
+-rw-r--r--   0        0        0    11251 2023-08-01 10:22:39.615693 bootloader_core_library-0.0.2/src/bootloader/ue/model/ue_asset.py
+-rw-r--r--   0        0        0     1060 1970-01-01 00:00:00.000000 bootloader_core_library-0.0.2/setup.py
+-rw-r--r--   0        0        0     1134 1970-01-01 00:00:00.000000 bootloader_core_library-0.0.2/PKG-INFO
```

### Comparing `bootloader_core_library-0.0.1/LICENSE.md` & `bootloader_core_library-0.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `bootloader_core_library-0.0.1/pyproject.toml` & `bootloader_core_library-0.0.2/pyproject.toml`

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
-version = "0.0.1"
+version = "0.0.2"
 
 [tool.poetry.dependencies]
 perseus-core-library = "^1.19.4"
 python = "^3.10"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `bootloader_core_library-0.0.1/src/bootloader/__init__.py` & `bootloader_core_library-0.0.2/src/bootloader/__init__.py`

 * *Files identical despite different names*

### Comparing `bootloader_core_library-0.0.1/src/bootloader/ue/__init__.py` & `bootloader_core_library-0.0.2/src/bootloader/ue/__init__.py`

 * *Files identical despite different names*

### Comparing `bootloader_core_library-0.0.1/src/bootloader/ue/constant/__init__.py` & `bootloader_core_library-0.0.2/src/bootloader/ue/constant/__init__.py`

 * *Files identical despite different names*

### Comparing `bootloader_core_library-0.0.1/src/bootloader/ue/model/__init__.py` & `bootloader_core_library-0.0.2/src/bootloader/ue/model/__init__.py`

 * *Files identical despite different names*

### Comparing `bootloader_core_library-0.0.1/setup.py` & `bootloader_core_library-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['perseus-core-library>=1.19.4,<2.0.0']
 
 setup_kwargs = {
     'name': 'bootloader-core-library',
-    'version': '0.0.1',
+    'version': '0.0.2',
     'description': 'Repository of reusable Python components to be shared by Python projects using the Bootloader services',
     'long_description': '# Bootloader Core Python Library\n\nRepository of reusable Python components to be shared by Python projects using the Bootloader services.\n',
     'author': 'Daniel CAUNE',
     'author_email': 'daniel@bootloader.studio',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/bootloader-studio/bootloader-core-python-library',
```

### Comparing `bootloader_core_library-0.0.1/PKG-INFO` & `bootloader_core_library-0.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bootloader-core-library
-Version: 0.0.1
+Version: 0.0.2
 Summary: Repository of reusable Python components to be shared by Python projects using the Bootloader services
 Home-page: https://github.com/bootloader-studio/bootloader-core-python-library
 License: SEE LICENSE IN <LICENSE.md>
 Keywords: core,library
 Author: Daniel CAUNE
 Author-email: daniel@bootloader.studio
 Requires-Python: >=3.10,<4.0
```

