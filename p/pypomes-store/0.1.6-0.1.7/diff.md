# Comparing `tmp/pypomes_store-0.1.6.tar.gz` & `tmp/pypomes_store-0.1.7.tar.gz`

## Comparing `pypomes_store-0.1.6.tar` & `pypomes_store-0.1.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 pypomes_store-0.1.6/src/pypomes_store/__init__.py
--rw-r--r--   0        0        0     7714 2020-02-02 00:00:00.000000 pypomes_store-0.1.6/src/pypomes_store/azure_pomes.py
--rw-r--r--   0        0        0    13930 2020-02-02 00:00:00.000000 pypomes_store-0.1.6/src/pypomes_store/minio_pomes.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 pypomes_store-0.1.6/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_store-0.1.6/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_store-0.1.6/README.md
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 pypomes_store-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 pypomes_store-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 pypomes_store-0.1.7/src/pypomes_store/__init__.py
+-rw-r--r--   0        0        0     7714 2020-02-02 00:00:00.000000 pypomes_store-0.1.7/src/pypomes_store/azure_pomes.py
+-rw-r--r--   0        0        0    13930 2020-02-02 00:00:00.000000 pypomes_store-0.1.7/src/pypomes_store/minio_pomes.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 pypomes_store-0.1.7/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_store-0.1.7/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_store-0.1.7/README.md
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 pypomes_store-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 pypomes_store-0.1.7/PKG-INFO
```

### Comparing `pypomes_store-0.1.6/src/pypomes_store/__init__.py` & `pypomes_store-0.1.7/src/pypomes_store/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,9 +16,9 @@
     # minio_pomes
     MINIO_BUCKET, MINIO_HOST, MINIO_ACCESS_KEY, MINIO_SECRET_KEY, MINIO_SECURE_ACCESS, MINIO_TEMP_PATH,
     minio_access, minio_file_store, minio_object_store, minio_object_stat,
     minio_object_delete, minio_objects_list, minio_object_retrieve, minio_object_exists,
     minio_object_tags_retrieve, minio_file_retrieve, minio_setup
 ]
 
-__version__ = "0.1.6"
-__version_info__ = (0, 1, 6)
+__version__ = "0.1.7"
+__version_info__ = (0, 1, 7)
```

### Comparing `pypomes_store-0.1.6/src/pypomes_store/azure_pomes.py` & `pypomes_store-0.1.7/src/pypomes_store/azure_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_store-0.1.6/src/pypomes_store/minio_pomes.py` & `pypomes_store-0.1.7/src/pypomes_store/minio_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_store-0.1.6/LICENSE` & `pypomes_store-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_store-0.1.6/pyproject.toml` & `pypomes_store-0.1.7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_store"
-version = "0.1.6"
+version = "0.1.7"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (object storage modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -21,15 +21,15 @@
 dependencies = [
     "azure-common>=1.1.28",
     "azure-core>=1.28.0",
     "azure-identity>=1.13.0",
     "azure-storage-blob>=12.17.0",
     "minio>=7.1.15",
     "pip>=23.2.1",
-    "pypomes_core>=0.2.2",
+    "pypomes_core>=0.2.1",
     "setuptools>=68.0.0",
     "Unidecode>=1.3.6",
     "wheel>=0.41.0"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/TheWiseCoder/PyPomes-Store"
```

### Comparing `pypomes_store-0.1.6/PKG-INFO` & `pypomes_store-0.1.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypomes_store
-Version: 0.1.6
+Version: 0.1.7
 Summary: A collection of Python pomes, pennyeach (object storage modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-Store
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-Store/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,11 +12,11 @@
 Requires-Python: >=3.10
 Requires-Dist: azure-common>=1.1.28
 Requires-Dist: azure-core>=1.28.0
 Requires-Dist: azure-identity>=1.13.0
 Requires-Dist: azure-storage-blob>=12.17.0
 Requires-Dist: minio>=7.1.15
 Requires-Dist: pip>=23.2.1
-Requires-Dist: pypomes-core>=0.2.2
+Requires-Dist: pypomes-core>=0.2.1
 Requires-Dist: setuptools>=68.0.0
 Requires-Dist: unidecode>=1.3.6
 Requires-Dist: wheel>=0.41.0
```

