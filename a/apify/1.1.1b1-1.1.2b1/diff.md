# Comparing `tmp/apify-1.1.1b1.tar.gz` & `tmp/apify-1.1.2b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apify-1.1.1b1.tar", last modified: Tue May 23 17:08:47 2023, max compression
+gzip compressed data, was "apify-1.1.2b1.tar", last modified: Tue Aug  1 11:36:24 2023, max compression
```

## Comparing `apify-1.1.1b1.tar` & `apify-1.1.2b1.tar`

### file list

```diff
@@ -1,46 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:08:47.826235 apify-1.1.1b1/
--rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-05-23 17:07:59.000000 apify-1.1.1b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-05-23 17:08:47.826235 apify-1.1.1b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-05-23 17:07:59.000000 apify-1.1.1b1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-05-23 17:08:42.000000 apify-1.1.1b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 17:08:47.826235 apify-1.1.1b1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:08:47.818235 apify-1.1.1b1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:08:47.822235 apify-1.1.1b1/src/apify/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-23 17:07:59.000000 apify-1.1.1b1/src/apify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-05-23 17:07:59.000000 apify-1.1.1b1/src/apify/_crypto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:08:47.822235 apify-1.1.1b1/src/apify/_memory_storage/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-23 17:07:59.000000 apify-1.1.1b1/src/apify/_memory_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-05-23 17:07:59.000000 apify-1.1.1b1/src/apify/_memory_storage/file_storage_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10118 2023-05-23 17:07:59.000000 apify-1.1.1b1/src/apify/_memory_storage/memory_storage_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:08:47.826235 apify-1.1.1b1/src/apify/_memory_storage/resource_clients/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-23 17:07:59.000000 apify-1.1.1b1/src/apify/_memory_storage/resource_clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-05-23 17:07:59.000000 apify-1.1.1b1/src/apify/_memory_storage/resource_clients/base_resource_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-05-23 17:07:59.000000 apify-1.1.1b1/src/apify/_memory_storage/resource_clients/base_resource_collection_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    19664 2023-05-23 17:07:59.000000 apify-1.1.1b1/src/apify/_memory_storage/resource_clients/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-05-23 17:07:59.000000 apify-1.1.1b1/src/apify/_memory_storage/resource_clients/dataset_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    19736 2023-05-23 17:07:59.000000 apify-1.1.1b1/src/apify/_memory_storage/resource_clients/key_value_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-23 17:07:59.000000 apify-1.1.1b1/src/apify/_memory_storage/resource_clients/key_value_store_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    19050 2023-05-23 17:07:59.000000 apify-1.1.1b1/src/apify/_memory_storage/resource_clients/request_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-23 17:07:59.000000 apify-1.1.1b1/src/apify/_memory_storage/resource_clients/request_queue_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-23 17:07:59.000000 apify-1.1.1b1/src/apify/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    15528 2023-05-23 17:07:59.000000 apify-1.1.1b1/src/apify/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    58928 2023-05-23 17:07:59.000000 apify-1.1.1b1/src/apify/actor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8717 2023-05-23 17:07:59.000000 apify-1.1.1b1/src/apify/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7045 2023-05-23 17:07:59.000000 apify-1.1.1b1/src/apify/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    10430 2023-05-23 17:07:59.000000 apify-1.1.1b1/src/apify/event_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-05-23 17:07:59.000000 apify-1.1.1b1/src/apify/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    15522 2023-05-23 17:07:59.000000 apify-1.1.1b1/src/apify/proxy_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 17:07:59.000000 apify-1.1.1b1/src/apify/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:08:47.826235 apify-1.1.1b1/src/apify/storages/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-23 17:07:59.000000 apify-1.1.1b1/src/apify/storages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7095 2023-05-23 17:07:59.000000 apify-1.1.1b1/src/apify/storages/base_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)    23398 2023-05-23 17:07:59.000000 apify-1.1.1b1/src/apify/storages/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10102 2023-05-23 17:07:59.000000 apify-1.1.1b1/src/apify/storages/key_value_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    25879 2023-05-23 17:07:59.000000 apify-1.1.1b1/src/apify/storages/request_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-05-23 17:07:59.000000 apify-1.1.1b1/src/apify/storages/storage_client_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:08:47.822235 apify-1.1.1b1/src/apify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-05-23 17:08:47.000000 apify-1.1.1b1/src/apify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-23 17:08:47.000000 apify-1.1.1b1/src/apify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 17:08:47.000000 apify-1.1.1b1/src/apify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-23 17:08:47.000000 apify-1.1.1b1/src/apify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-23 17:08:47.000000 apify-1.1.1b1/src/apify.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:24.509369 apify-1.1.2b1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-08-01 11:35:43.000000 apify-1.1.2b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-08-01 11:36:24.509369 apify-1.1.2b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-08-01 11:35:43.000000 apify-1.1.2b1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-08-01 11:36:20.000000 apify-1.1.2b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:24.509369 apify-1.1.2b1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:24.501368 apify-1.1.2b1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:24.505369 apify-1.1.2b1/src/apify/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-08-01 11:35:43.000000 apify-1.1.2b1/src/apify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-08-01 11:35:43.000000 apify-1.1.2b1/src/apify/_crypto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:24.505369 apify-1.1.2b1/src/apify/_memory_storage/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-01 11:35:43.000000 apify-1.1.2b1/src/apify/_memory_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-08-01 11:35:43.000000 apify-1.1.2b1/src/apify/_memory_storage/file_storage_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10160 2023-08-01 11:35:43.000000 apify-1.1.2b1/src/apify/_memory_storage/memory_storage_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:24.509369 apify-1.1.2b1/src/apify/_memory_storage/resource_clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-08-01 11:35:43.000000 apify-1.1.2b1/src/apify/_memory_storage/resource_clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-08-01 11:35:43.000000 apify-1.1.2b1/src/apify/_memory_storage/resource_clients/base_resource_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-08-01 11:35:43.000000 apify-1.1.2b1/src/apify/_memory_storage/resource_clients/base_resource_collection_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19703 2023-08-01 11:35:43.000000 apify-1.1.2b1/src/apify/_memory_storage/resource_clients/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-08-01 11:35:43.000000 apify-1.1.2b1/src/apify/_memory_storage/resource_clients/dataset_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19749 2023-08-01 11:35:43.000000 apify-1.1.2b1/src/apify/_memory_storage/resource_clients/key_value_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-08-01 11:35:43.000000 apify-1.1.2b1/src/apify/_memory_storage/resource_clients/key_value_store_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19044 2023-08-01 11:35:43.000000 apify-1.1.2b1/src/apify/_memory_storage/resource_clients/request_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-08-01 11:35:43.000000 apify-1.1.2b1/src/apify/_memory_storage/resource_clients/request_queue_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12574 2023-08-01 11:35:43.000000 apify-1.1.2b1/src/apify/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58948 2023-08-01 11:35:43.000000 apify-1.1.2b1/src/apify/actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8730 2023-08-01 11:35:43.000000 apify-1.1.2b1/src/apify/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-08-01 11:35:43.000000 apify-1.1.2b1/src/apify/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10448 2023-08-01 11:35:43.000000 apify-1.1.2b1/src/apify/event_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-08-01 11:35:43.000000 apify-1.1.2b1/src/apify/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15545 2023-08-01 11:35:43.000000 apify-1.1.2b1/src/apify/proxy_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:35:43.000000 apify-1.1.2b1/src/apify/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:24.509369 apify-1.1.2b1/src/apify/storages/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-08-01 11:35:43.000000 apify-1.1.2b1/src/apify/storages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-08-01 11:35:43.000000 apify-1.1.2b1/src/apify/storages/base_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23436 2023-08-01 11:35:43.000000 apify-1.1.2b1/src/apify/storages/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10132 2023-08-01 11:35:43.000000 apify-1.1.2b1/src/apify/storages/key_value_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25909 2023-08-01 11:35:43.000000 apify-1.1.2b1/src/apify/storages/request_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-08-01 11:35:43.000000 apify-1.1.2b1/src/apify/storages/storage_client_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:24.505369 apify-1.1.2b1/src/apify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-08-01 11:36:24.000000 apify-1.1.2b1/src/apify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-08-01 11:36:24.000000 apify-1.1.2b1/src/apify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:24.000000 apify-1.1.2b1/src/apify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-08-01 11:36:24.000000 apify-1.1.2b1/src/apify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-01 11:36:24.000000 apify-1.1.2b1/src/apify.egg-info/top_level.txt
```

### Comparing `apify-1.1.1b1/LICENSE` & `apify-1.1.2b1/LICENSE`

 * *Files identical despite different names*

### Comparing `apify-1.1.1b1/PKG-INFO` & `apify-1.1.2b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apify
-Version: 1.1.1b1
+Version: 1.1.2b1
 Summary: Apify SDK for Python
 Author-email: "Apify Technologies s.r.o." <support@apify.com>
 License: Apache Software License
 Project-URL: Homepage, https://docs.apify.com/sdk/python/
 Project-URL: Documentation, https://docs.apify.com/sdk/python/
 Project-URL: Source, https://github.com/apify/apify-sdk-python
 Project-URL: Issue tracker, https://github.com/apify/apify-sdk-python/issues
```

### Comparing `apify-1.1.1b1/README.md` & `apify-1.1.2b1/README.md`

 * *Files identical despite different names*

### Comparing `apify-1.1.1b1/pyproject.toml` & `apify-1.1.2b1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [project]
 
 name = "apify"
 
-version = "1.1.1b1"
+version = "1.1.2b1"
 description = "Apify SDK for Python"
 
 readme = "README.md"
 
 license = {text = "Apache Software License"}
 
 authors = [
 
-    {name = "Apify Technologies s.r.o.", email = "support@apify.com" }
+    { name = "Apify Technologies s.r.o.", email = "support@apify.com" },
 
 ]
 
 keywords = ["apify", "sdk", "actor", "scraping", "automation"]
 
 
 
@@ -47,15 +47,17 @@
 
 dependencies = [
 
     "aiofiles >= 22.1.0",
 
     "aioshutil >= 1.0",
 
-    "apify-client >= 1.2.0",
+    "apify-client >= 1.3.1",
+
+    "apify-shared >= 1.0.0",
 
     "colorama >= 0.4.6",
 
     "cryptography >= 39.0.0",
 
     "httpx >= 0.24.1",
```

### Comparing `apify-1.1.1b1/src/apify/_crypto.py` & `apify-1.1.2b1/src/apify/_crypto.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 from typing import Any
 
 from cryptography.exceptions import InvalidTag as InvalidTagException
 from cryptography.hazmat.primitives import hashes, serialization
 from cryptography.hazmat.primitives.asymmetric import padding, rsa
 from cryptography.hazmat.primitives.ciphers import Cipher, algorithms, modes
 
-from ._utils import ignore_docs
+from apify_shared.utils import ignore_docs
+
 from .consts import ENCRYPTED_INPUT_VALUE_REGEXP
 
 ENCRYPTION_KEY_LENGTH = 32
 ENCRYPTION_IV_LENGTH = 16
 ENCRYPTION_AUTH_TAG_LENGTH = 16
```

### Comparing `apify-1.1.1b1/src/apify/_memory_storage/file_storage_utils.py` & `apify-1.1.2b1/src/apify/_memory_storage/file_storage_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 import os
 from typing import Dict, List, Tuple
 
 import aiofiles
 from aiofiles.os import makedirs
 
-from .._utils import _force_remove, _json_dumps
+from apify_shared.utils import json_dumps
+
+from .._utils import _force_remove
 
 
 async def _update_metadata(*, data: Dict, entity_directory: str, write_metadata: bool) -> None:
     # Skip writing the actual metadata file. This is done after ensuring the directory exists so we have the directory present
     if not write_metadata:
         return
 
     # Ensure the directory for the entity exists
     await makedirs(entity_directory, exist_ok=True)
 
     # Write the metadata to the file
     file_path = os.path.join(entity_directory, '__metadata__.json')
     async with aiofiles.open(file_path, mode='wb') as f:
-        await f.write(_json_dumps(data).encode('utf-8'))
+        await f.write(json_dumps(data).encode('utf-8'))
 
 
 async def _update_dataset_items(
     *,
     data: List[Tuple[str, Dict]],
     entity_directory: str,
     persist_storage: bool,
@@ -34,15 +36,15 @@
     # Ensure the directory for the entity exists
     await makedirs(entity_directory, exist_ok=True)
 
     # Save all the new items to the disk
     for idx, item in data:
         file_path = os.path.join(entity_directory, f'{idx}.json')
         async with aiofiles.open(file_path, mode='wb') as f:
-            await f.write(_json_dumps(item).encode('utf-8'))
+            await f.write(json_dumps(item).encode('utf-8'))
 
 
 async def _update_request_queue_item(
     *,
     request_id: str,
     request: Dict,
     entity_directory: str,
@@ -54,15 +56,15 @@
 
     # Ensure the directory for the entity exists
     await makedirs(entity_directory, exist_ok=True)
 
     # Write the request to the file
     file_path = os.path.join(entity_directory, f'{request_id}.json')
     async with aiofiles.open(file_path, mode='wb') as f:
-        await f.write(_json_dumps(request).encode('utf-8'))
+        await f.write(json_dumps(request).encode('utf-8'))
 
 
 async def _delete_request(*, request_id: str, entity_directory: str) -> None:
     # Ensure the directory for the entity exists
     await makedirs(entity_directory, exist_ok=True)
 
     file_path = os.path.join(entity_directory, f'{request_id}.json')
```

### Comparing `apify-1.1.1b1/src/apify/_memory_storage/memory_storage_client.py` & `apify-1.1.2b1/src/apify/_memory_storage/memory_storage_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,18 @@
 from pathlib import Path
 from typing import List, Optional
 
 import aioshutil
 from aiofiles import ospath
 from aiofiles.os import rename, scandir
 
-from .._utils import _maybe_parse_bool, ignore_docs
-from ..consts import ApifyEnvVars
+from apify_shared.consts import ApifyEnvVars
+from apify_shared.utils import ignore_docs
+
+from .._utils import _maybe_parse_bool
 from .resource_clients.dataset import DatasetClient
 from .resource_clients.dataset_collection import DatasetCollectionClient
 from .resource_clients.key_value_store import KeyValueStoreClient
 from .resource_clients.key_value_store_collection import KeyValueStoreCollectionClient
 from .resource_clients.request_queue import RequestQueueClient
 from .resource_clients.request_queue_collection import RequestQueueCollectionClient
```

### Comparing `apify-1.1.1b1/src/apify/_memory_storage/resource_clients/__init__.py` & `apify-1.1.2b1/src/apify/_memory_storage/resource_clients/__init__.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.1b1/src/apify/_memory_storage/resource_clients/base_resource_client.py` & `apify-1.1.2b1/src/apify/_memory_storage/resource_clients/base_resource_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import os
 from abc import ABC, abstractmethod
 from typing import TYPE_CHECKING, Dict, List, Optional
 
 from typing_extensions import Self
 
-from ..._utils import ignore_docs
+from apify_shared.utils import ignore_docs
 
 if TYPE_CHECKING:
     from ..memory_storage_client import MemoryStorageClient
 
 
 @ignore_docs
 class BaseResourceClient(ABC):
```

### Comparing `apify-1.1.1b1/src/apify/_memory_storage/resource_clients/base_resource_collection_client.py` & `apify-1.1.2b1/src/apify/_memory_storage/resource_clients/base_resource_collection_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from abc import ABC, abstractmethod
 from operator import itemgetter
 from typing import TYPE_CHECKING, Dict, Generic, List, Optional, Type, TypeVar
 
-from apify_client._utils import ListPage
+from apify_shared.models import ListPage
+from apify_shared.utils import ignore_docs
 
-from ..._utils import ignore_docs
 from ..file_storage_utils import _update_metadata
 from .base_resource_client import BaseResourceClient
 
 if TYPE_CHECKING:
     from ..memory_storage_client import MemoryStorageClient
```

### Comparing `apify-1.1.1b1/src/apify/_memory_storage/resource_clients/dataset.py` & `apify-1.1.2b1/src/apify/_memory_storage/resource_clients/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 import json
 import os
 from datetime import datetime, timezone
 from typing import TYPE_CHECKING, Any, AsyncIterator, Dict, List, Optional, Tuple
 
 import aioshutil
 
-from apify_client._utils import ListPage
+from apify_shared.models import ListPage
+from apify_shared.types import JSONSerializable
+from apify_shared.utils import ignore_docs
 
 from ..._crypto import _crypto_random_object_id
-from ..._types import JSONSerializable
-from ..._utils import _force_rename, _raise_on_duplicate_storage, _raise_on_non_existing_storage, ignore_docs
+from ..._utils import _force_rename, _raise_on_duplicate_storage, _raise_on_non_existing_storage
 from ...consts import _StorageTypes
 from ..file_storage_utils import _update_dataset_items, _update_metadata
 from .base_resource_client import BaseResourceClient
 
 if TYPE_CHECKING:
     from ..memory_storage_client import MemoryStorageClient
```

### Comparing `apify-1.1.1b1/src/apify/_memory_storage/resource_clients/dataset_collection.py` & `apify-1.1.2b1/src/apify/_memory_storage/resource_clients/dataset_collection.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Dict, List, Optional, Type
 
-from apify_client._utils import ListPage
+from apify_shared.models import ListPage
+from apify_shared.utils import ignore_docs
 
-from ..._utils import ignore_docs
 from .base_resource_collection_client import BaseResourceCollectionClient
 from .dataset import DatasetClient
 
 
 @ignore_docs
 class DatasetCollectionClient(BaseResourceCollectionClient):
     """Sub-client for manipulating datasets."""
```

### Comparing `apify-1.1.1b1/src/apify/_memory_storage/resource_clients/key_value_store.py` & `apify-1.1.2b1/src/apify/_memory_storage/resource_clients/key_value_store.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,25 +9,24 @@
 from typing import TYPE_CHECKING, Any, AsyncIterator, Dict, List, Optional, TypedDict
 
 import aiofiles
 import aioshutil
 from aiofiles.os import makedirs
 from typing_extensions import NotRequired
 
+from apify_shared.utils import ignore_docs, is_file_or_bytes, json_dumps
+
 from ..._crypto import _crypto_random_object_id
 from ..._utils import (
     _force_remove,
     _force_rename,
     _guess_file_extension,
-    _is_file_or_bytes,
-    _json_dumps,
     _maybe_parse_body,
     _raise_on_duplicate_storage,
     _raise_on_non_existing_storage,
-    ignore_docs,
 )
 from ...consts import DEFAULT_API_PARAM_LIMIT, _StorageTypes
 from ...log import logger
 from ..file_storage_utils import _update_metadata
 from .base_resource_client import BaseResourceClient
 
 if TYPE_CHECKING:
@@ -288,23 +287,23 @@
         if existing_store_by_id is None:
             _raise_on_non_existing_storage(_StorageTypes.KEY_VALUE_STORE, self._id)
 
         if isinstance(value, io.IOBase):
             raise NotImplementedError('File-like values are not supported in local memory storage')
 
         if content_type is None:
-            if _is_file_or_bytes(value):
+            if is_file_or_bytes(value):
                 content_type = 'application/octet-stream'
             elif isinstance(value, str):
                 content_type = 'text/plain; charset=utf-8'
             else:
                 content_type = 'application/json; charset=utf-8'
 
-        if 'application/json' in content_type and not _is_file_or_bytes(value) and not isinstance(value, str):
-            value = _json_dumps(value).encode('utf-8')
+        if 'application/json' in content_type and not is_file_or_bytes(value) and not isinstance(value, str):
+            value = json_dumps(value).encode('utf-8')
 
         async with existing_store_by_id._file_operation_lock:
             await existing_store_by_id._update_timestamps(True)
             record: KeyValueStoreRecord = {
                 'key': key,
                 'value': value,
                 'contentType': content_type,
@@ -337,15 +336,15 @@
             record['value'] = record['value'].encode('utf-8')
 
         async with aiofiles.open(record_path, mode='wb') as f:
             await f.write(record['value'])
 
         if self._memory_storage_client._write_metadata:
             async with aiofiles.open(record_metadata_path, mode='wb') as f:
-                await f.write(_json_dumps({
+                await f.write(json_dumps({
                     'key': record['key'],
                     'contentType': record['contentType'],
                 }).encode('utf-8'))
 
     async def delete_record(self, key: str) -> None:
         """Delete the specified record from the key-value store.
```

### Comparing `apify-1.1.1b1/src/apify/_memory_storage/resource_clients/key_value_store_collection.py` & `apify-1.1.2b1/src/apify/_memory_storage/resource_clients/key_value_store_collection.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Dict, List, Optional, Type
 
-from apify_client._utils import ListPage
+from apify_shared.models import ListPage
+from apify_shared.utils import ignore_docs
 
-from ..._utils import ignore_docs
 from .base_resource_collection_client import BaseResourceCollectionClient
 from .key_value_store import KeyValueStoreClient
 
 
 @ignore_docs
 class KeyValueStoreCollectionClient(BaseResourceCollectionClient):
     """Sub-client for manipulating key-value stores."""
```

### Comparing `apify-1.1.1b1/src/apify/_memory_storage/resource_clients/request_queue.py` & `apify-1.1.2b1/src/apify/_memory_storage/resource_clients/request_queue.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,24 +4,18 @@
 from datetime import datetime, timezone
 from decimal import Decimal
 from typing import TYPE_CHECKING, Dict, List, Optional
 
 import aioshutil
 from sortedcollections import ValueSortedDict  # type: ignore
 
+from apify_shared.utils import filter_out_none_values_recursively, ignore_docs, json_dumps
+
 from ..._crypto import _crypto_random_object_id
-from ..._utils import (
-    _filter_out_none_values_recursively,
-    _force_rename,
-    _json_dumps,
-    _raise_on_duplicate_storage,
-    _raise_on_non_existing_storage,
-    _unique_key_to_request_id,
-    ignore_docs,
-)
+from ..._utils import _force_rename, _raise_on_duplicate_storage, _raise_on_non_existing_storage, _unique_key_to_request_id
 from ...consts import _StorageTypes
 from ..file_storage_utils import _delete_request, _update_metadata, _update_request_queue_item
 from .base_resource_client import BaseResourceClient
 
 if TYPE_CHECKING:
     from ..memory_storage_client import MemoryStorageClient
 
@@ -355,24 +349,24 @@
             write_metadata=self._memory_storage_client._write_metadata,
         )
 
     def _json_to_request(self, request_json: Optional[str]) -> Optional[dict]:
         if request_json is None:
             return None
         request = json.loads(request_json)
-        return _filter_out_none_values_recursively(request)
+        return filter_out_none_values_recursively(request)
 
     def _create_internal_request(self, request: Dict, forefront: Optional[bool]) -> Dict:
         order_no = self._calculate_order_no(request, forefront)
         id = _unique_key_to_request_id(request['uniqueKey'])
 
         if request.get('id') is not None and request['id'] != id:
             raise ValueError('Request ID does not match its unique_key.')
 
-        json_request = _json_dumps({**request, 'id': id})
+        json_request = json_dumps({**request, 'id': id})
         return {
             'id': id,
             'json': json_request,
             'method': request.get('method'),
             'orderNo': order_no,
             'retryCount': request.get('retryCount', 0),
             'uniqueKey': request['uniqueKey'],
```

### Comparing `apify-1.1.1b1/src/apify/_memory_storage/resource_clients/request_queue_collection.py` & `apify-1.1.2b1/src/apify/_memory_storage/resource_clients/request_queue_collection.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Dict, List, Optional, Type
 
-from apify_client._utils import ListPage
+from apify_shared.models import ListPage
+from apify_shared.utils import ignore_docs
 
-from ..._utils import ignore_docs
 from .base_resource_collection_client import BaseResourceCollectionClient
 from .request_queue import RequestQueueClient
 
 
 @ignore_docs
 class RequestQueueCollectionClient(BaseResourceCollectionClient):
     """Sub-client for manipulating request queues."""
```

### Comparing `apify-1.1.1b1/src/apify/_utils.py` & `apify-1.1.2b1/src/apify/_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,56 +1,50 @@
 import asyncio
 import base64
 import builtins
 import contextlib
 import functools
 import hashlib
 import inspect
-import io
 import json
 import mimetypes
 import os
 import re
 import sys
 import time
 from collections import OrderedDict
 from collections.abc import MutableMapping
 from datetime import datetime, timezone
-from enum import Enum
 from importlib import metadata
 from typing import Any, Callable, Dict, Generic, ItemsView, Iterator, List, NoReturn, Optional
 from typing import OrderedDict as OrderedDictType
 from typing import Tuple, Type, TypeVar, Union, ValuesView, cast, overload
 
 import aioshutil
 import psutil
 from aiofiles import ospath
 from aiofiles.os import remove, rename
 
-from .consts import (
-    _BOOL_ENV_VARS_TYPE,
-    _DATETIME_ENV_VARS_TYPE,
-    _FLOAT_ENV_VARS_TYPE,
-    _INTEGER_ENV_VARS_TYPE,
-    _STRING_ENV_VARS_TYPE,
+from apify_shared.consts import (
     BOOL_ENV_VARS,
+    BOOL_ENV_VARS_TYPE,
     DATETIME_ENV_VARS,
+    DATETIME_ENV_VARS_TYPE,
     FLOAT_ENV_VARS,
+    FLOAT_ENV_VARS_TYPE,
     INTEGER_ENV_VARS,
-    REQUEST_ID_LENGTH,
+    INTEGER_ENV_VARS_TYPE,
+    STRING_ENV_VARS_TYPE,
     ApifyEnvVars,
-    _StorageTypes,
 )
+from apify_shared.utils import ignore_docs, is_content_type_json, is_content_type_text, is_content_type_xml, maybe_extract_enum_member_value
 
-T = TypeVar('T')
-
+from .consts import REQUEST_ID_LENGTH, _StorageTypes
 
-def ignore_docs(method: T) -> T:
-    """Mark that a method's documentation should not be rendered. Functionally, this decorator is a noop."""
-    return method
+T = TypeVar('T')
 
 
 def _get_system_info() -> Dict:
     python_version = '.'.join([str(x) for x in sys.version_info[:3]])
 
     system_info: Dict[str, Union[str, bool]] = {
         'apify_sdk_version': metadata.version('apify'),
@@ -95,77 +89,71 @@
 
         Returns:
             The result of the getter.
         """
         return self.getter(obj or owner)
 
 
-def _maybe_extract_enum_member_value(maybe_enum_member: Any) -> Any:
-    if isinstance(maybe_enum_member, Enum):
-        return maybe_enum_member.value
-    return maybe_enum_member
-
-
 @overload
-def _fetch_and_parse_env_var(env_var: _BOOL_ENV_VARS_TYPE) -> Optional[bool]:
+def _fetch_and_parse_env_var(env_var: BOOL_ENV_VARS_TYPE) -> Optional[bool]:
     ...
 
 
 @overload
-def _fetch_and_parse_env_var(env_var: _BOOL_ENV_VARS_TYPE, default: bool) -> bool:
+def _fetch_and_parse_env_var(env_var: BOOL_ENV_VARS_TYPE, default: bool) -> bool:
     ...
 
 
 @overload
-def _fetch_and_parse_env_var(env_var: _DATETIME_ENV_VARS_TYPE) -> Optional[Union[datetime, str]]:
+def _fetch_and_parse_env_var(env_var: DATETIME_ENV_VARS_TYPE) -> Optional[Union[datetime, str]]:
     ...
 
 
 @overload
-def _fetch_and_parse_env_var(env_var: _DATETIME_ENV_VARS_TYPE, default: datetime) -> Union[datetime, str]:
+def _fetch_and_parse_env_var(env_var: DATETIME_ENV_VARS_TYPE, default: datetime) -> Union[datetime, str]:
     ...
 
 
 @overload
-def _fetch_and_parse_env_var(env_var: _FLOAT_ENV_VARS_TYPE) -> Optional[float]:
+def _fetch_and_parse_env_var(env_var: FLOAT_ENV_VARS_TYPE) -> Optional[float]:
     ...
 
 
 @overload
-def _fetch_and_parse_env_var(env_var: _FLOAT_ENV_VARS_TYPE, default: float) -> float:
+def _fetch_and_parse_env_var(env_var: FLOAT_ENV_VARS_TYPE, default: float) -> float:
     ...
 
 
 @overload
-def _fetch_and_parse_env_var(env_var: _INTEGER_ENV_VARS_TYPE) -> Optional[int]:
+def _fetch_and_parse_env_var(env_var: INTEGER_ENV_VARS_TYPE) -> Optional[int]:
     ...
 
 
 @overload
-def _fetch_and_parse_env_var(env_var: _INTEGER_ENV_VARS_TYPE, default: int) -> int:
+def _fetch_and_parse_env_var(env_var: INTEGER_ENV_VARS_TYPE, default: int) -> int:
     ...
 
 
 @overload
-def _fetch_and_parse_env_var(env_var: _STRING_ENV_VARS_TYPE, default: str) -> str:
+def _fetch_and_parse_env_var(env_var: STRING_ENV_VARS_TYPE, default: str) -> str:
     ...
 
 
 @overload
-def _fetch_and_parse_env_var(env_var: _STRING_ENV_VARS_TYPE) -> Optional[str]:
+def _fetch_and_parse_env_var(env_var: STRING_ENV_VARS_TYPE) -> Optional[str]:
     ...
 
 
 @overload
 def _fetch_and_parse_env_var(env_var: ApifyEnvVars) -> Optional[Any]:
     ...
 
 
 def _fetch_and_parse_env_var(env_var: Any, default: Any = None) -> Any:
-    env_var_name = str(_maybe_extract_enum_member_value(env_var))
+    env_var_name = str(maybe_extract_enum_member_value(env_var))
 
     val = os.getenv(env_var_name)
     if not val:
         return default
 
     if env_var in BOOL_ENV_VARS:
         return _maybe_parse_bool(val)
@@ -245,44 +233,21 @@
 
 async def _force_remove(filename: str) -> None:
     """JS-like rm(filename, { force: true })."""
     with contextlib.suppress(FileNotFoundError):
         await remove(filename)
 
 
-def _filter_out_none_values_recursively(dictionary: Dict) -> Dict:
-    """Return copy of the dictionary, recursively omitting all keys for which values are None."""
-    return cast(dict, _filter_out_none_values_recursively_internal(dictionary))
-
-
-# Unfortunately, it's necessary to have an internal function for the correct result typing, without having to create complicated overloads
-def _filter_out_none_values_recursively_internal(dictionary: Dict, remove_empty_dicts: Optional[bool] = None) -> Optional[Dict]:
-    result = {}
-    for k, v in dictionary.items():
-        if isinstance(v, dict):
-            v = _filter_out_none_values_recursively_internal(v, remove_empty_dicts is True or remove_empty_dicts is None)
-        if v is not None:
-            result[k] = v
-    if not result and remove_empty_dicts:
-        return None
-    return result
-
-
-def _json_dumps(obj: Any) -> str:
-    """Dump JSON to a string with the correct settings and serializer."""
-    return json.dumps(obj, ensure_ascii=False, indent=2, default=str)
-
-
 def _raise_on_non_existing_storage(client_type: _StorageTypes, id: str) -> NoReturn:
-    client_type = _maybe_extract_enum_member_value(client_type)
+    client_type = maybe_extract_enum_member_value(client_type)
     raise ValueError(f'{client_type} with id "{id}" does not exist.')
 
 
 def _raise_on_duplicate_storage(client_type: _StorageTypes, key_name: str, value: str) -> NoReturn:
-    client_type = _maybe_extract_enum_member_value(client_type)
+    client_type = maybe_extract_enum_member_value(client_type)
     raise ValueError(f'{client_type} with {key_name} "{value}" already exists.')
 
 
 def _guess_file_extension(content_type: str) -> Optional[str]:
     """Guess the file extension based on content type."""
     # e.g. mimetypes.guess_extension('application/json ') does not work...
     actual_content_type = content_type.split(';')[0].strip()
@@ -296,37 +261,18 @@
     # Guess the extension from the mime type
     ext = mimetypes.guess_extension(actual_content_type)
 
     # Remove the leading dot if extension successfully parsed
     return ext[1:] if ext is not None else ext
 
 
-def _is_content_type_json(content_type: str) -> bool:
-    return bool(re.search(r'^application/json', content_type, flags=re.IGNORECASE))
-
-
-def _is_content_type_xml(content_type: str) -> bool:
-    return bool(re.search(r'^application/.*xml$', content_type, flags=re.IGNORECASE))
-
-
-def _is_content_type_text(content_type: str) -> bool:
-    return bool(re.search(r'^text/', content_type, flags=re.IGNORECASE))
-
-
-def _is_file_or_bytes(value: Any) -> bool:
-    # The check for IOBase is not ideal, it would be better to use duck typing,
-    # but then the check would be super complex, judging from how the 'requests' library does it.
-    # This way should be good enough for the vast majority of use cases, if it causes issues, we can improve it later.
-    return isinstance(value, (bytes, bytearray, io.IOBase))
-
-
 def _maybe_parse_body(body: bytes, content_type: str) -> Any:
-    if _is_content_type_json(content_type):
+    if is_content_type_json(content_type):
         return json.loads(body.decode('utf-8'))  # Returns any
-    elif _is_content_type_xml(content_type) or _is_content_type_text(content_type):
+    elif is_content_type_xml(content_type) or is_content_type_text(content_type):
         return body.decode('utf-8')
     return body
 
 
 def _unique_key_to_request_id(unique_key: str) -> str:
     """Generate request ID based on unique key in a deterministic way."""
     id = re.sub(r'(\+|\/|=)', '', base64.b64encode(hashlib.sha256(unique_key.encode('utf-8')).digest()).decode('utf-8'))
@@ -441,30 +387,7 @@
     else:
         raise ValueError('Wrong input!')
 
 
 PARSE_DATE_FIELDS_MAX_DEPTH = 3
 PARSE_DATE_FIELDS_KEY_SUFFIX = 'At'
 ListOrDictOrAny = TypeVar('ListOrDictOrAny', List, Dict, Any)
-
-
-def _parse_date_fields(data: ListOrDictOrAny, max_depth: int = PARSE_DATE_FIELDS_MAX_DEPTH) -> ListOrDictOrAny:
-    if max_depth < 0:
-        return data
-
-    if isinstance(data, list):
-        return [_parse_date_fields(item, max_depth - 1) for item in data]
-
-    if isinstance(data, dict):
-        def parse(key: str, value: object) -> object:
-            parsed_value = value
-            if key.endswith(PARSE_DATE_FIELDS_KEY_SUFFIX) and isinstance(value, str):
-                parsed_value = _maybe_parse_datetime(value)
-            elif isinstance(value, dict):
-                parsed_value = _parse_date_fields(value, max_depth - 1)
-            elif isinstance(value, list):
-                parsed_value = _parse_date_fields(value, max_depth)
-            return parsed_value
-
-        return {key: parse(key, value) for (key, value) in data.items()}
-
-    return data
```

### Comparing `apify-1.1.1b1/src/apify/actor.py` & `apify-1.1.2b1/src/apify/actor.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,32 +4,31 @@
 import os
 import sys
 from datetime import datetime, timezone
 from types import TracebackType
 from typing import Any, Awaitable, Callable, Dict, List, Optional, Type, TypeVar, Union, cast
 
 from apify_client import ApifyClientAsync
-from apify_client.consts import WebhookEventType
+from apify_shared.consts import ActorEventTypes, ActorExitCodes, ApifyEnvVars, WebhookEventType
+from apify_shared.utils import ignore_docs, maybe_extract_enum_member_value
 
 from ._crypto import _decrypt_input_secrets, _load_private_key
 from ._memory_storage import MemoryStorageClient
 from ._utils import (
     _fetch_and_parse_env_var,
     _get_cpu_usage_percent,
     _get_memory_usage_bytes,
     _get_system_info,
     _is_running_in_ipython,
-    _maybe_extract_enum_member_value,
     _run_func_at_interval_async,
     _wrap_internal,
     dualproperty,
-    ignore_docs,
 )
 from .config import Configuration
-from .consts import EVENT_LISTENERS_TIMEOUT_SECS, ActorEventTypes, ActorExitCodes, ApifyEnvVars
+from .consts import EVENT_LISTENERS_TIMEOUT_SECS
 from .event_manager import EventManager
 from .log import logger
 from .proxy_configuration import ProxyConfiguration
 from .storages import Dataset, KeyValueStore, RequestQueue, StorageClientManager
 
 MainReturnType = TypeVar('MainReturnType')
 
@@ -329,15 +328,15 @@
         event_listeners_timeout_secs: Optional[float] = EVENT_LISTENERS_TIMEOUT_SECS,
         status_message: Optional[str] = None,
     ) -> None:
         self._raise_if_not_initialized()
 
         self._is_exiting = True
 
-        exit_code = _maybe_extract_enum_member_value(exit_code)
+        exit_code = maybe_extract_enum_member_value(exit_code)
 
         self.log.info('Exiting actor', extra={'exit_code': exit_code})
 
         await self._cancel_event_emitting_intervals()
 
         # Send final persist state event
         if not self._was_final_persist_state_emitted:
```

### Comparing `apify-1.1.1b1/src/apify/config.py` & `apify-1.1.2b1/src/apify/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Optional
 
+from apify_shared.consts import ApifyEnvVars
+
 from ._utils import _fetch_and_parse_env_var
-from .consts import ApifyEnvVars
 
 
 class Configuration:
     """A class for specifying the configuration of an actor.
 
     Can be used either globally via `Configuration.get_global_configuration()`,
     or it can be specific to each `Actor` instance on the `actor.config` property.
```

### Comparing `apify-1.1.1b1/src/apify/event_manager.py` & `apify-1.1.2b1/src/apify/event_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 import json
 from collections import defaultdict
 from typing import Any, Callable, Coroutine, Dict, List, Optional, Set, Union
 
 import websockets.client
 from pyee.asyncio import AsyncIOEventEmitter
 
-from ._utils import _maybe_extract_enum_member_value, _parse_date_fields, ignore_docs
+from apify_shared.consts import ActorEventTypes
+from apify_shared.utils import ignore_docs, maybe_extract_enum_member_value, parse_date_fields
+
 from .config import Configuration
-from .consts import ActorEventTypes
 from .log import logger
 
 ListenerType = Union[Callable[[], None], Callable[[Any], None], Callable[[], Coroutine[Any, Any, None]], Callable[[Any], Coroutine[Any, Any, None]]]
 
 
 @ignore_docs
 class EventManager:
@@ -115,15 +116,15 @@
             except TypeError:
                 try:
                     signature.bind()
                     listener_argument_count = 0
                 except TypeError:
                     raise ValueError('The "listener" argument must be a callable which accepts 0 or 1 arguments!')
 
-        event_name = _maybe_extract_enum_member_value(event_name)
+        event_name = maybe_extract_enum_member_value(event_name)
 
         async def inner_wrapper(event_data: Any) -> None:
             if inspect.iscoroutinefunction(listener):
                 if listener_argument_count == 0:
                     await listener()
                 else:
                     await listener(event_data)
@@ -156,15 +157,15 @@
         Args:
             event_name (ActorEventTypes): The actor event for which to remove listeners.
             listener (Callable, optional): The listener which is supposed to be removed. If not passed, all listeners of this event are removed.
         """
         if not self._initialized:
             raise RuntimeError('EventManager was not initialized!')
 
-        event_name = _maybe_extract_enum_member_value(event_name)
+        event_name = maybe_extract_enum_member_value(event_name)
 
         if listener:
             for listener_wrapper in self._listeners_to_wrappers[event_name][listener]:
                 self._event_emitter.remove_listener(event_name, listener_wrapper)
             self._listeners_to_wrappers[event_name][listener] = []
         else:
             self._listeners_to_wrappers[event_name] = defaultdict(list)
@@ -173,15 +174,15 @@
     def emit(self, event_name: ActorEventTypes, data: Any) -> None:
         """Emit an actor event manually.
 
         Args:
             event_name (ActorEventTypes): The actor event which should be emitted.
             data (Any): The data that should be emitted with the event.
         """
-        event_name = _maybe_extract_enum_member_value(event_name)
+        event_name = maybe_extract_enum_member_value(event_name)
 
         self._event_emitter.emit(event_name, data)
 
     async def wait_for_all_listeners_to_complete(self, *, timeout_secs: Optional[float] = None) -> None:
         """Wait for all event listeners which are currently being executed to complete.
 
         Args:
@@ -215,15 +216,15 @@
             async with websockets.client.connect(self._config.actor_events_ws_url) as websocket:
                 self._platform_events_websocket = websocket
                 self._connected_to_platform_websocket.set_result(True)
                 async for message in websocket:
                     try:
                         parsed_message = json.loads(message)
                         assert isinstance(parsed_message, dict)
-                        parsed_message = _parse_date_fields(parsed_message)
+                        parsed_message = parse_date_fields(parsed_message)
                         event_name = parsed_message['name']
                         event_data = parsed_message.get('data')  # 'data' can be missing
 
                         self._event_emitter.emit(event_name, event_data)
 
                     except Exception:
                         logger.exception('Cannot parse actor event', extra={'message': message})
```

### Comparing `apify-1.1.1b1/src/apify/log.py` & `apify-1.1.2b1/src/apify/log.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import logging
 import textwrap
 import traceback
 from typing import Any, Dict
 
 from colorama import Fore, Style, just_fix_windows_console
 
-from ._utils import ignore_docs
+from apify_shared.utils import ignore_docs
 
 just_fix_windows_console()
 
 
 # Name of the logger used throughout the library (resolves to 'apify')
 logger_name = __name__.split('.')[0]
```

### Comparing `apify-1.1.1b1/src/apify/proxy_configuration.py` & `apify-1.1.2b1/src/apify/proxy_configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 from typing import Any, Awaitable, Callable, Dict, List, Optional, Pattern, TypedDict, Union
 from urllib.parse import urljoin, urlparse
 
 import httpx
 from typing_extensions import NotRequired
 
 from apify_client import ApifyClientAsync
+from apify_shared.consts import ApifyEnvVars
+from apify_shared.utils import ignore_docs
 
-from ._utils import ignore_docs
 from .config import Configuration
-from .consts import ApifyEnvVars
 from .log import logger
 
 APIFY_PROXY_VALUE_REGEX = re.compile(r'^[\w._~]+$')
 COUNTRY_CODE_REGEX = re.compile(r'^[A-Z]{2}$')
 SESSION_ID_MAX_LENGTH = 50
```

### Comparing `apify-1.1.1b1/src/apify/storages/base_storage.py` & `apify-1.1.2b1/src/apify/storages/base_storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import asyncio
 from abc import ABC, abstractmethod
 from typing import Dict, Generic, Optional, TypeVar, Union, cast
 
 from typing_extensions import Self
 
 from apify_client import ApifyClientAsync
+from apify_shared.utils import ignore_docs
 
 from .._memory_storage import MemoryStorageClient
 from .._memory_storage.resource_clients import BaseResourceClient, BaseResourceCollectionClient
-from .._utils import ignore_docs
 from ..config import Configuration
 from .storage_client_manager import StorageClientManager
 
 BaseResourceClientType = TypeVar('BaseResourceClientType', bound=BaseResourceClient)
 BaseResourceCollectionClientType = TypeVar('BaseResourceCollectionClientType', bound=BaseResourceCollectionClient)
```

### Comparing `apify-1.1.1b1/src/apify/storages/dataset.py` & `apify-1.1.2b1/src/apify/storages/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 import csv
 import io
 import math
 from typing import AsyncIterator, Dict, Iterable, Iterator, List, Optional, Union
 
 from apify_client import ApifyClientAsync
-from apify_client._utils import ListPage
 from apify_client.clients import DatasetClientAsync, DatasetCollectionClientAsync
+from apify_shared.models import ListPage
+from apify_shared.types import JSONSerializable
+from apify_shared.utils import ignore_docs, json_dumps
 
 from .._memory_storage import MemoryStorageClient
 from .._memory_storage.resource_clients import DatasetClient, DatasetCollectionClient
-from .._types import JSONSerializable
-from .._utils import _json_dumps, _wrap_internal, ignore_docs
+from .._utils import _wrap_internal
 from ..config import Configuration
 from ..consts import MAX_PAYLOAD_SIZE_BYTES
 from .base_storage import BaseStorage
 from .key_value_store import KeyValueStore
 
 SAFETY_BUFFER_PERCENT = 0.01 / 100  # 0.01%
 EFFECTIVE_LIMIT_BYTES = MAX_PAYLOAD_SIZE_BYTES - math.ceil(MAX_PAYLOAD_SIZE_BYTES * SAFETY_BUFFER_PERCENT)
 
 
 def _check_and_serialize(item: JSONSerializable, index: Optional[int] = None) -> str:
     """Accept a JSON serializable object as an input, validate its serializability and its serialized size against `EFFECTIVE_LIMIT_BYTES`."""
     s = ' ' if index is None else f' at index {index} '
 
     try:
-        payload = _json_dumps(item)
+        payload = json_dumps(item)
     except Exception as e:
         raise ValueError(f'Data item{s}is not serializable to JSON.') from e
 
     length_bytes = len(payload.encode('utf-8'))
     if length_bytes > EFFECTIVE_LIMIT_BYTES:
         raise ValueError(f'Data item{s}is too large (size: {length_bytes} bytes, limit: {EFFECTIVE_LIMIT_BYTES} bytes)')
```

### Comparing `apify-1.1.1b1/src/apify/storages/key_value_store.py` & `apify-1.1.2b1/src/apify/storages/key_value_store.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from typing import Any, AsyncIterator, NamedTuple, Optional, TypedDict, TypeVar, Union, overload
 
 from apify_client import ApifyClientAsync
 from apify_client.clients import KeyValueStoreClientAsync, KeyValueStoreCollectionClientAsync
+from apify_shared.utils import ignore_docs
 
 from .._memory_storage import MemoryStorageClient
 from .._memory_storage.resource_clients import KeyValueStoreClient, KeyValueStoreCollectionClient
-from .._utils import _wrap_internal, ignore_docs
+from .._utils import _wrap_internal
 from ..config import Configuration
 from .base_storage import BaseStorage
 
 T = TypeVar('T')
 IterateKeysInfo = TypedDict('IterateKeysInfo', {'size': int})
 IterateKeysTuple = NamedTuple('IterateKeysTuple', [('key', str), ('info', IterateKeysInfo)])
```

### Comparing `apify-1.1.1b1/src/apify/storages/request_queue.py` & `apify-1.1.2b1/src/apify/storages/request_queue.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,19 +3,20 @@
 from datetime import datetime, timezone
 from typing import Coroutine, Dict, Optional
 from typing import OrderedDict as OrderedDictType
 from typing import Set, Union
 
 from apify_client import ApifyClientAsync
 from apify_client.clients import RequestQueueClientAsync, RequestQueueCollectionClientAsync
+from apify_shared.utils import ignore_docs
 
 from .._crypto import _crypto_random_object_id
 from .._memory_storage import MemoryStorageClient
 from .._memory_storage.resource_clients import RequestQueueClient, RequestQueueCollectionClient
-from .._utils import LRUCache, _budget_ow, _unique_key_to_request_id, ignore_docs
+from .._utils import LRUCache, _budget_ow, _unique_key_to_request_id
 from ..config import Configuration
 from ..consts import REQUEST_QUEUE_HEAD_MAX_LIMIT
 from ..log import logger
 from .base_storage import BaseStorage
 
 MAX_CACHED_REQUESTS = 1_000_000
```

### Comparing `apify-1.1.1b1/src/apify/storages/storage_client_manager.py` & `apify-1.1.2b1/src/apify/storages/storage_client_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Optional, Union
 
 from apify_client import ApifyClientAsync
+from apify_shared.utils import ignore_docs
 
 from .._memory_storage import MemoryStorageClient
-from .._utils import ignore_docs
 from ..config import Configuration
 
 
 @ignore_docs
 class StorageClientManager:
     """A class for managing storage clients."""
```

### Comparing `apify-1.1.1b1/src/apify.egg-info/PKG-INFO` & `apify-1.1.2b1/src/apify.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apify
-Version: 1.1.1b1
+Version: 1.1.2b1
 Summary: Apify SDK for Python
 Author-email: "Apify Technologies s.r.o." <support@apify.com>
 License: Apache Software License
 Project-URL: Homepage, https://docs.apify.com/sdk/python/
 Project-URL: Documentation, https://docs.apify.com/sdk/python/
 Project-URL: Source, https://github.com/apify/apify-sdk-python
 Project-URL: Issue tracker, https://github.com/apify/apify-sdk-python/issues
```

### Comparing `apify-1.1.1b1/src/apify.egg-info/SOURCES.txt` & `apify-1.1.2b1/src/apify.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 LICENSE
 README.md
 pyproject.toml
 src/apify/__init__.py
 src/apify/_crypto.py
-src/apify/_types.py
 src/apify/_utils.py
 src/apify/actor.py
 src/apify/config.py
 src/apify/consts.py
 src/apify/event_manager.py
 src/apify/log.py
 src/apify/proxy_configuration.py
```

### Comparing `apify-1.1.1b1/src/apify.egg-info/requires.txt` & `apify-1.1.2b1/src/apify.egg-info/requires.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 aiofiles>=22.1.0
 aioshutil>=1.0
-apify-client>=1.2.0
+apify-client>=1.3.1
+apify-shared>=1.0.0
 colorama>=0.4.6
 cryptography>=39.0.0
 httpx>=0.24.1
 psutil>=5.9.5
 pyee>=9.0.0
 sortedcollections>=2.0.1
 typing-extensions>=4.1.0
```

