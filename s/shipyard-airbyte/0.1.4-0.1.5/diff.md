# Comparing `tmp/shipyard_airbyte-0.1.4.tar.gz` & `tmp/shipyard_airbyte-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_airbyte-0.1.4.tar", max compression
+gzip compressed data, was "shipyard_airbyte-0.1.5.tar", max compression
```

## Comparing `shipyard_airbyte-0.1.4.tar` & `shipyard_airbyte-0.1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      931 2023-04-18 15:33:24.337867 shipyard_airbyte-0.1.4/README.md
--rw-r--r--   0        0        0      660 2023-05-16 16:06:52.024288 shipyard_airbyte-0.1.4/pyproject.toml
--rw-r--r--   0        0        0       34 2023-04-18 15:33:24.339180 shipyard_airbyte-0.1.4/shipyard_airbyte/__init__.py
--rw-r--r--   0        0        0     4658 2023-05-15 22:33:53.992063 shipyard_airbyte-0.1.4/shipyard_airbyte/airbyte.py
--rw-r--r--   0        0        0      403 2023-05-10 22:55:38.724312 shipyard_airbyte-0.1.4/shipyard_airbyte/cli/authtest.py
--rw-r--r--   0        0        0     1196 2023-04-18 15:33:24.339946 shipyard_airbyte-0.1.4/shipyard_airbyte/cli/cli_determine_sync_status.py
--rw-r--r--   0        0        0     1094 2023-04-18 15:33:24.340255 shipyard_airbyte-0.1.4/shipyard_airbyte/cli/cli_trigger_sync.py
--rw-r--r--   0        0        0     1613 1970-01-01 00:00:00.000000 shipyard_airbyte-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      931 2023-05-12 18:48:21.820323 shipyard_airbyte-0.1.5/README.md
+-rw-r--r--   0        0        0      661 2023-08-01 12:44:58.152827 shipyard_airbyte-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0       34 2023-05-12 18:48:21.820731 shipyard_airbyte-0.1.5/shipyard_airbyte/__init__.py
+-rw-r--r--   0        0        0     4994 2023-07-31 23:59:07.142813 shipyard_airbyte-0.1.5/shipyard_airbyte/airbyte.py
+-rw-r--r--   0        0        0      304 2023-07-28 00:25:41.242346 shipyard_airbyte-0.1.5/shipyard_airbyte/cli/authtest.py
+-rw-r--r--   0        0        0     1212 2023-07-31 23:59:07.143404 shipyard_airbyte-0.1.5/shipyard_airbyte/cli/cli_determine_sync_status.py
+-rw-r--r--   0        0        0     2234 2023-07-31 23:59:07.143906 shipyard_airbyte-0.1.5/shipyard_airbyte/cli/cli_trigger_sync.py
+-rw-r--r--   0        0        0     1613 1970-01-01 00:00:00.000000 shipyard_airbyte-0.1.5/PKG-INFO
```

### Comparing `shipyard_airbyte-0.1.4/README.md` & `shipyard_airbyte-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `shipyard_airbyte-0.1.4/pyproject.toml` & `shipyard_airbyte-0.1.5/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "shipyard-airbyte"
-version = "0.1.4"
+version = "0.1.5"
 description = "A local client to work with Airbyte Cloud"
 authors = ["wrp801 <wespoulsen@gmail.com>"]
 license = "Apache License 2.0"
 readme = "README.md"
 packages = [{include = "shipyard_airbyte"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 requests = "2.28.0"
 pytest = "^7.2.2"
-shipyard-templates = "0.1.1"
+shipyard-templates = "0.2.0"
 shipyard-bp-utils = "^0.1.0"
 
 [tool.poetry.group.dev.dependencies]
 shipyard-bp-utils = {path = "../shipyard-bp-utils", develop = true}
-shipyard-templates = {path = "../../shipyard-templates", develop = true}
+#shipyard-templates = {path = "../../shipyard-templates", develop = true}
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `shipyard_airbyte-0.1.4/shipyard_airbyte/airbyte.py` & `shipyard_airbyte-0.1.5/shipyard_airbyte/airbyte.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,16 +68,23 @@
         url = 'https://api.airbyte.com/v1/jobs'
         job_url = f"{url}/{job_id}"
         headers = {
             'accept': 'application/json',
             'authorization': f'Bearer {self.access_token}',
             'User-Agent': 'Shipyard User 1.0'
         }
-        job_response = requests.get(job_url, headers=headers).json()
-        return job_response
+        try:
+            job_response = requests.get(job_url, headers=headers).json()
+            job_response.raise_for_status()
+        except Exception as error:
+            self.logger.error(
+                f"Error occurred when attempting to fetch sync status. Check to see that the job id and api token are valid. Error: {error}")
+            sys.exit(self.EXIT_CODE_BAD_REQUEST)
+        else:
+            return job_response
 
     def determine_sync_status(self, job_response: dict) -> int:
         """ Provides logging and handling based off of the status. Intended to be used by the Shipyard Application only
 
         Args:
             job_response: The response from the get_sync_status()
```

### Comparing `shipyard_airbyte-0.1.4/shipyard_airbyte/cli/cli_determine_sync_status.py` & `shipyard_airbyte-0.1.5/shipyard_airbyte/cli/cli_determine_sync_status.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     client = AirbyteClient(api_token)
     base_folder_name = shipyard.logs.determine_base_artifact_folder(
         'airbyte')
     artifact_subfolder_paths = shipyard.logs.determine_artifact_subfolders(
         base_folder_name)
     shipyard.logs.create_artifacts_folders(artifact_subfolder_paths)
     # check if a job id was provided, otherwise look for it in the artifact folders
-    if job_id is None:
+    if job_id is None or job_id == '':
         response = shipyard.logs.read_pickle_file(
             artifact_subfolder_paths, 'sync_response')
         job_id = response
     job_status = client.get_sync_status(job_id=job_id)
     sync_status = client.determine_sync_status(job_status)
     sys.exit(sync_status)
```

### Comparing `shipyard_airbyte-0.1.4/PKG-INFO` & `shipyard_airbyte-0.1.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: shipyard-airbyte
-Version: 0.1.4
+Version: 0.1.5
 Summary: A local client to work with Airbyte Cloud
 License: Apache-2.0
 Author: wrp801
 Author-email: wespoulsen@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pytest (>=7.2.2,<8.0.0)
 Requires-Dist: requests (==2.28.0)
 Requires-Dist: shipyard-bp-utils (>=0.1.0,<0.2.0)
-Requires-Dist: shipyard-templates (==0.1.1)
+Requires-Dist: shipyard-templates (==0.2.0)
 Description-Content-Type: text/markdown
 
 # shipyard-airbyte
 
 ## Description 
 A local client to trigger Airbyte syncs and check statuses of past jobs
```

