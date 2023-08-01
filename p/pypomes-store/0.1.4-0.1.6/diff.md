# Comparing `tmp/pypomes_store-0.1.4.tar.gz` & `tmp/pypomes_store-0.1.6.tar.gz`

## Comparing `pypomes_store-0.1.4.tar` & `pypomes_store-0.1.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 pypomes_store-0.1.4/src/pypomes_store/__init__.py
--rw-r--r--   0        0        0     7765 2020-02-02 00:00:00.000000 pypomes_store-0.1.4/src/pypomes_store/azure_pomes.py
--rw-r--r--   0        0        0    10545 2020-02-02 00:00:00.000000 pypomes_store-0.1.4/src/pypomes_store/minio_pomes.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pypomes_store-0.1.4/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_store-0.1.4/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_store-0.1.4/README.md
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 pypomes_store-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 pypomes_store-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 pypomes_store-0.1.6/src/pypomes_store/__init__.py
+-rw-r--r--   0        0        0     7714 2020-02-02 00:00:00.000000 pypomes_store-0.1.6/src/pypomes_store/azure_pomes.py
+-rw-r--r--   0        0        0    13930 2020-02-02 00:00:00.000000 pypomes_store-0.1.6/src/pypomes_store/minio_pomes.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 pypomes_store-0.1.6/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_store-0.1.6/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_store-0.1.6/README.md
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 pypomes_store-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 pypomes_store-0.1.6/PKG-INFO
```

### Comparing `pypomes_store-0.1.4/src/pypomes_store/__init__.py` & `pypomes_store-0.1.6/src/pypomes_store/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,9 +16,9 @@
     # minio_pomes
     MINIO_BUCKET, MINIO_HOST, MINIO_ACCESS_KEY, MINIO_SECRET_KEY, MINIO_SECURE_ACCESS, MINIO_TEMP_PATH,
     minio_access, minio_file_store, minio_object_store, minio_object_stat,
     minio_object_delete, minio_objects_list, minio_object_retrieve, minio_object_exists,
     minio_object_tags_retrieve, minio_file_retrieve, minio_setup
 ]
 
-__version__ = "0.1.4"
-__version_info__ = (0, 1, 4)
+__version__ = "0.1.6"
+__version_info__ = (0, 1, 6)
```

### Comparing `pypomes_store-0.1.4/src/pypomes_store/azure_pomes.py` & `pypomes_store-0.1.6/src/pypomes_store/azure_pomes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import io
 import sys
 # noinspection PyPackageRequirements
 from azure.storage.blob import BlobClient, BlobProperties
 from typing import Final
-from pypomes_core.env_pomes import APP_PREFIX, env_get_str
-from pypomes_core.exception_pomes import exc_format
+from pypomes_core import APP_PREFIX, env_get_str, exc_format
 
 # string de conexão com o Azure
 AZURE_CONNECTION_STRING: Final[str] = env_get_str(f"{APP_PREFIX}_AZURE_CONNECTION_STRING")
 
 #  nome do bucket no armazenamento Azure
 AZURE_STORAGE_BUCKET: Final[str] = env_get_str(f"{APP_PREFIX}_AZURE_STORAGE_BUCKET")
 
@@ -130,22 +129,22 @@
     return result
 
 
 def blob_get_mimetype(errors: list[str], blob_path: str,
                       bucket_name: str = AZURE_STORAGE_BUCKET) -> str:
     """
     Obtem e retorna o texxto contido no documento apontado por *file_path*, dentro de  *bucket_name*.
+
     Esse documento deve ser do tipo HTML ou PDF.
 
     :param errors: eventuais erros ocorridos na invocação da função
     :param blob_path: caminho do arquivo no bucket
     :param bucket_name: o nome do bucket (AZURE_STORAGE_BUCKET, se não especificado)
     :return: o texto do blob, codificado em UTF-8
     """
-
     # inicializa a variável de retorno
     result: str | None = None
 
     try:
         with BlobClient.from_connection_string(
             conn_str=AZURE_CONNECTION_STRING,
             container_name=bucket_name,
```

### Comparing `pypomes_store-0.1.4/LICENSE` & `pypomes_store-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_store-0.1.4/pyproject.toml` & `pypomes_store-0.1.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -2,35 +2,35 @@
 requires = [
     "hatchling"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_store"
-version = "0.1.4"
+version = "0.1.6"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (object storage modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
 dependencies = [
     "azure-common>=1.1.28",
-    "azure-core>=1.26.4",
+    "azure-core>=1.28.0",
     "azure-identity>=1.13.0",
-    "azure-storage-blob>=12.16.0",
+    "azure-storage-blob>=12.17.0",
     "minio>=7.1.15",
-    "pip>=23.1.2",
-    "pypomes_core>=0.1.2",
+    "pip>=23.2.1",
+    "pypomes_core>=0.2.2",
     "setuptools>=68.0.0",
-    "unidecode>=1.3.6",
-    "wheel>=0.40.0"
+    "Unidecode>=1.3.6",
+    "wheel>=0.41.0"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/TheWiseCoder/PyPomes-Store"
 "Bug Tracker" = "https://github.com/TheWiseCoder/PyPomes-Store/issues"
```

### Comparing `pypomes_store-0.1.4/PKG-INFO` & `pypomes_store-0.1.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: pypomes_store
-Version: 0.1.4
+Version: 0.1.6
 Summary: A collection of Python pomes, pennyeach (object storage modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-Store
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-Store/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: azure-common>=1.1.28
-Requires-Dist: azure-core>=1.26.4
+Requires-Dist: azure-core>=1.28.0
 Requires-Dist: azure-identity>=1.13.0
-Requires-Dist: azure-storage-blob>=12.16.0
+Requires-Dist: azure-storage-blob>=12.17.0
 Requires-Dist: minio>=7.1.15
-Requires-Dist: pip>=23.1.2
-Requires-Dist: pypomes-core>=0.1.2
+Requires-Dist: pip>=23.2.1
+Requires-Dist: pypomes-core>=0.2.2
 Requires-Dist: setuptools>=68.0.0
 Requires-Dist: unidecode>=1.3.6
-Requires-Dist: wheel>=0.40.0
+Requires-Dist: wheel>=0.41.0
```

