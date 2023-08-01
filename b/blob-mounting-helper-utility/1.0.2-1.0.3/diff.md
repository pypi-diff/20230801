# Comparing `tmp/blob_mounting_helper_utility-1.0.2.tar.gz` & `tmp/blob_mounting_helper_utility-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blob_mounting_helper_utility-1.0.2.tar", last modified: Thu Jun 15 13:31:53 2023, max compression
+gzip compressed data, was "blob_mounting_helper_utility-1.0.3.tar", last modified: Tue Aug  1 10:11:56 2023, max compression
```

## Comparing `blob_mounting_helper_utility-1.0.2.tar` & `blob_mounting_helper_utility-1.0.3.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxr-x   0 ivica     (1000) ivica     (1000)        0 2023-06-15 13:31:53.730013 blob_mounting_helper_utility-1.0.2/
--rw-rw-r--   0 ivica     (1000) ivica     (1000)     3018 2023-06-15 13:31:53.730013 blob_mounting_helper_utility-1.0.2/PKG-INFO
--rw-rw-r--   0 ivica     (1000) ivica     (1000)     2029 2023-06-15 13:30:00.000000 blob_mounting_helper_utility-1.0.2/README.md
-drwxrwxr-x   0 ivica     (1000) ivica     (1000)        0 2023-06-15 13:31:53.726013 blob_mounting_helper_utility-1.0.2/blob_mounting_helper_utility/
--rw-rw-r--   0 ivica     (1000) ivica     (1000)       37 2023-06-15 11:11:15.000000 blob_mounting_helper_utility-1.0.2/blob_mounting_helper_utility/__init__.py
--rw-rw-r--   0 ivica     (1000) ivica     (1000)     4230 2023-06-15 10:51:13.000000 blob_mounting_helper_utility-1.0.2/blob_mounting_helper_utility/utils.py
-drwxrwxr-x   0 ivica     (1000) ivica     (1000)        0 2023-06-15 13:31:53.726013 blob_mounting_helper_utility-1.0.2/blob_mounting_helper_utility.egg-info/
--rw-rw-r--   0 ivica     (1000) ivica     (1000)     3018 2023-06-15 13:31:53.000000 blob_mounting_helper_utility-1.0.2/blob_mounting_helper_utility.egg-info/PKG-INFO
--rw-rw-r--   0 ivica     (1000) ivica     (1000)      305 2023-06-15 13:31:53.000000 blob_mounting_helper_utility-1.0.2/blob_mounting_helper_utility.egg-info/SOURCES.txt
--rw-rw-r--   0 ivica     (1000) ivica     (1000)        1 2023-06-15 13:31:53.000000 blob_mounting_helper_utility-1.0.2/blob_mounting_helper_utility.egg-info/dependency_links.txt
--rw-rw-r--   0 ivica     (1000) ivica     (1000)       29 2023-06-15 13:31:53.000000 blob_mounting_helper_utility-1.0.2/blob_mounting_helper_utility.egg-info/top_level.txt
--rw-rw-r--   0 ivica     (1000) ivica     (1000)       38 2023-06-15 13:31:53.730013 blob_mounting_helper_utility-1.0.2/setup.cfg
--rw-rw-r--   0 ivica     (1000) ivica     (1000)     1028 2023-06-15 13:30:20.000000 blob_mounting_helper_utility-1.0.2/setup.py
+drwxrwxr-x   0 ivica     (1000) ivica     (1000)        0 2023-08-01 10:11:56.230518 blob_mounting_helper_utility-1.0.3/
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)     2559 2023-08-01 10:11:56.230518 blob_mounting_helper_utility-1.0.3/PKG-INFO
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)     2029 2023-06-15 13:30:00.000000 blob_mounting_helper_utility-1.0.3/README.md
+drwxrwxr-x   0 ivica     (1000) ivica     (1000)        0 2023-08-01 10:11:56.230518 blob_mounting_helper_utility-1.0.3/blob_mounting_helper_utility/
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)       37 2023-06-15 11:11:15.000000 blob_mounting_helper_utility-1.0.3/blob_mounting_helper_utility/__init__.py
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)     5617 2023-08-01 10:09:16.000000 blob_mounting_helper_utility-1.0.3/blob_mounting_helper_utility/utils.py
+drwxrwxr-x   0 ivica     (1000) ivica     (1000)        0 2023-08-01 10:11:56.230518 blob_mounting_helper_utility-1.0.3/blob_mounting_helper_utility.egg-info/
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)     2559 2023-08-01 10:11:56.000000 blob_mounting_helper_utility-1.0.3/blob_mounting_helper_utility.egg-info/PKG-INFO
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)      356 2023-08-01 10:11:56.000000 blob_mounting_helper_utility-1.0.3/blob_mounting_helper_utility.egg-info/SOURCES.txt
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)        1 2023-08-01 10:11:56.000000 blob_mounting_helper_utility-1.0.3/blob_mounting_helper_utility.egg-info/dependency_links.txt
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)       28 2023-08-01 10:11:56.000000 blob_mounting_helper_utility-1.0.3/blob_mounting_helper_utility.egg-info/requires.txt
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)       29 2023-08-01 10:11:56.000000 blob_mounting_helper_utility-1.0.3/blob_mounting_helper_utility.egg-info/top_level.txt
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)       38 2023-08-01 10:11:56.230518 blob_mounting_helper_utility-1.0.3/setup.cfg
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)     1055 2023-08-01 10:11:51.000000 blob_mounting_helper_utility-1.0.3/setup.py
```

### Comparing `blob_mounting_helper_utility-1.0.2/PKG-INFO` & `blob_mounting_helper_utility-1.0.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,72 +1,74 @@
 Metadata-Version: 2.1
 Name: blob_mounting_helper_utility
-Version: 1.0.2
+Version: 1.0.3
 Summary: Blob mapping utility for easy translation between azure urls and local paths
 Home-page: UNKNOWN
 Author: Ivica Matic
 Author-email: <ivica.matic@spatialdays.com>
 License: UNKNOWN
-Description: 
-        # Blob mapping utility
-        
-        When your code needs to access many mapped blobs as a mounted folder, the utility to make translation between blob urls and filepaths easier was made.
-        It can be configured using the configuration json file.
-        
-        Configuration file example:
-        
-        ``` json
-        {
-          "blob_mounting_configurations": [
-            {
-              "storage_account_name": "examplestagingstrgacc",
-              "storage_account_url": "https://examplestagingstrgacc.blob.core.windows.net/",
-              "container_name": "heightstore-example1-raw",
-              "mount_point": "/mnt/heightstore-example1-raw"
-            },
-            {
-              "storage_account_name": "examplestagingstrgacc",
-              "storage_account_url": "https://examplestagingstrgacc.blob.core.windows.net/",
-              "container_name": "heightstore-example2-raw",
-              "mount_point": "/mnt/heightstore-example2-raw"
-            },
-            {
-              "storage_account_name": "examplestagingstrgacc",
-              "storage_account_url": "https://examplestagingstrgacc.blob.core.windows.net/",
-              "container_name": "heightstore-example3-raw",
-              "mount_point": "/mnt/heightstore-example3-raw"
-            },
-            {
-              "storage_account_name": "examplestagingstrgacc",
-              "storage_account_url": "https://examplestagingstrgacc.blob.core.windows.net/",
-              "container_name": "example-container-raw",
-              "mount_point": "/mnt/example-container-raw"
-            }
-          ]
-        }
-        ```
-        
-        ## How to use
-        
-        ```python
-        from blob_mounting_helper_utility import BlobMappingUtility
-        json_config_file = "blob_mapping_config.json"
-        
-        # read the file into a dictionary
-        with open(json_config_file) as json_file:
-            config = json.load(json_file)["blob_mounting_configurations"]
-        
-        # create the utility object
-        blob_mapping_utility = BlobMappingUtility(config)
-        
-        filepath1 = "/mnt/example-container-raw/cool_picture.png
-        blob_url = blob_mapping_utility.get_url_from_mounted_filepath(filepath1) # -> https://examplestagingstrgacc.blob.core.windows.net/example-container-raw/cool_picture.png
-        
-        filepath2 = get_mounted_filepath_from_url(blob_url) # -> /mnt/example-container-raw/cool_picture.png
-        ```
 Keywords: python,azure,blob,mount
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Description-Content-Type: text/markdown
+
+
+# Blob mapping utility
+
+When your code needs to access many mapped blobs as a mounted folder, the utility to make translation between blob urls and filepaths easier was made.
+It can be configured using the configuration json file.
+
+Configuration file example:
+
+``` json
+{
+  "blob_mounting_configurations": [
+    {
+      "storage_account_name": "examplestagingstrgacc",
+      "storage_account_url": "https://examplestagingstrgacc.blob.core.windows.net/",
+      "container_name": "heightstore-example1-raw",
+      "mount_point": "/mnt/heightstore-example1-raw"
+    },
+    {
+      "storage_account_name": "examplestagingstrgacc",
+      "storage_account_url": "https://examplestagingstrgacc.blob.core.windows.net/",
+      "container_name": "heightstore-example2-raw",
+      "mount_point": "/mnt/heightstore-example2-raw"
+    },
+    {
+      "storage_account_name": "examplestagingstrgacc",
+      "storage_account_url": "https://examplestagingstrgacc.blob.core.windows.net/",
+      "container_name": "heightstore-example3-raw",
+      "mount_point": "/mnt/heightstore-example3-raw"
+    },
+    {
+      "storage_account_name": "examplestagingstrgacc",
+      "storage_account_url": "https://examplestagingstrgacc.blob.core.windows.net/",
+      "container_name": "example-container-raw",
+      "mount_point": "/mnt/example-container-raw"
+    }
+  ]
+}
+```
+
+## How to use
+
+```python
+from blob_mounting_helper_utility import BlobMappingUtility
+json_config_file = "blob_mapping_config.json"
+
+# read the file into a dictionary
+with open(json_config_file) as json_file:
+    config = json.load(json_file)["blob_mounting_configurations"]
+
+# create the utility object
+blob_mapping_utility = BlobMappingUtility(config)
+
+filepath1 = "/mnt/example-container-raw/cool_picture.png
+blob_url = blob_mapping_utility.get_url_from_mounted_filepath(filepath1) # -> https://examplestagingstrgacc.blob.core.windows.net/example-container-raw/cool_picture.png
+
+filepath2 = get_mounted_filepath_from_url(blob_url) # -> /mnt/example-container-raw/cool_picture.png
+```
+
```

### Comparing `blob_mounting_helper_utility-1.0.2/README.md` & `blob_mounting_helper_utility-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `blob_mounting_helper_utility-1.0.2/blob_mounting_helper_utility.egg-info/PKG-INFO` & `blob_mounting_helper_utility-1.0.3/blob_mounting_helper_utility.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,72 +1,74 @@
 Metadata-Version: 2.1
 Name: blob-mounting-helper-utility
-Version: 1.0.2
+Version: 1.0.3
 Summary: Blob mapping utility for easy translation between azure urls and local paths
 Home-page: UNKNOWN
 Author: Ivica Matic
 Author-email: <ivica.matic@spatialdays.com>
 License: UNKNOWN
-Description: 
-        # Blob mapping utility
-        
-        When your code needs to access many mapped blobs as a mounted folder, the utility to make translation between blob urls and filepaths easier was made.
-        It can be configured using the configuration json file.
-        
-        Configuration file example:
-        
-        ``` json
-        {
-          "blob_mounting_configurations": [
-            {
-              "storage_account_name": "examplestagingstrgacc",
-              "storage_account_url": "https://examplestagingstrgacc.blob.core.windows.net/",
-              "container_name": "heightstore-example1-raw",
-              "mount_point": "/mnt/heightstore-example1-raw"
-            },
-            {
-              "storage_account_name": "examplestagingstrgacc",
-              "storage_account_url": "https://examplestagingstrgacc.blob.core.windows.net/",
-              "container_name": "heightstore-example2-raw",
-              "mount_point": "/mnt/heightstore-example2-raw"
-            },
-            {
-              "storage_account_name": "examplestagingstrgacc",
-              "storage_account_url": "https://examplestagingstrgacc.blob.core.windows.net/",
-              "container_name": "heightstore-example3-raw",
-              "mount_point": "/mnt/heightstore-example3-raw"
-            },
-            {
-              "storage_account_name": "examplestagingstrgacc",
-              "storage_account_url": "https://examplestagingstrgacc.blob.core.windows.net/",
-              "container_name": "example-container-raw",
-              "mount_point": "/mnt/example-container-raw"
-            }
-          ]
-        }
-        ```
-        
-        ## How to use
-        
-        ```python
-        from blob_mounting_helper_utility import BlobMappingUtility
-        json_config_file = "blob_mapping_config.json"
-        
-        # read the file into a dictionary
-        with open(json_config_file) as json_file:
-            config = json.load(json_file)["blob_mounting_configurations"]
-        
-        # create the utility object
-        blob_mapping_utility = BlobMappingUtility(config)
-        
-        filepath1 = "/mnt/example-container-raw/cool_picture.png
-        blob_url = blob_mapping_utility.get_url_from_mounted_filepath(filepath1) # -> https://examplestagingstrgacc.blob.core.windows.net/example-container-raw/cool_picture.png
-        
-        filepath2 = get_mounted_filepath_from_url(blob_url) # -> /mnt/example-container-raw/cool_picture.png
-        ```
 Keywords: python,azure,blob,mount
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Description-Content-Type: text/markdown
+
+
+# Blob mapping utility
+
+When your code needs to access many mapped blobs as a mounted folder, the utility to make translation between blob urls and filepaths easier was made.
+It can be configured using the configuration json file.
+
+Configuration file example:
+
+``` json
+{
+  "blob_mounting_configurations": [
+    {
+      "storage_account_name": "examplestagingstrgacc",
+      "storage_account_url": "https://examplestagingstrgacc.blob.core.windows.net/",
+      "container_name": "heightstore-example1-raw",
+      "mount_point": "/mnt/heightstore-example1-raw"
+    },
+    {
+      "storage_account_name": "examplestagingstrgacc",
+      "storage_account_url": "https://examplestagingstrgacc.blob.core.windows.net/",
+      "container_name": "heightstore-example2-raw",
+      "mount_point": "/mnt/heightstore-example2-raw"
+    },
+    {
+      "storage_account_name": "examplestagingstrgacc",
+      "storage_account_url": "https://examplestagingstrgacc.blob.core.windows.net/",
+      "container_name": "heightstore-example3-raw",
+      "mount_point": "/mnt/heightstore-example3-raw"
+    },
+    {
+      "storage_account_name": "examplestagingstrgacc",
+      "storage_account_url": "https://examplestagingstrgacc.blob.core.windows.net/",
+      "container_name": "example-container-raw",
+      "mount_point": "/mnt/example-container-raw"
+    }
+  ]
+}
+```
+
+## How to use
+
+```python
+from blob_mounting_helper_utility import BlobMappingUtility
+json_config_file = "blob_mapping_config.json"
+
+# read the file into a dictionary
+with open(json_config_file) as json_file:
+    config = json.load(json_file)["blob_mounting_configurations"]
+
+# create the utility object
+blob_mapping_utility = BlobMappingUtility(config)
+
+filepath1 = "/mnt/example-container-raw/cool_picture.png
+blob_url = blob_mapping_utility.get_url_from_mounted_filepath(filepath1) # -> https://examplestagingstrgacc.blob.core.windows.net/example-container-raw/cool_picture.png
+
+filepath2 = get_mounted_filepath_from_url(blob_url) # -> /mnt/example-container-raw/cool_picture.png
+```
+
```

### Comparing `blob_mounting_helper_utility-1.0.2/setup.py` & `blob_mounting_helper_utility-1.0.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,29 +3,29 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.0.2'
+VERSION = '1.0.3'
 DESCRIPTION = 'Blob mapping utility for easy translation between azure urls and local paths'
 LONG_DESCRIPTION = 'Blob mapping utility for easy translation between azure urls and local paths'
 
 # Setting up
 setup(
     name="blob_mounting_helper_utility",
     version=VERSION,
     author="Ivica Matic",
     author_email="<ivica.matic@spatialdays.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
-    install_requires=[''],
+    install_requires=['azure-storage-blob==12.17.0'],
     keywords=['python', 'azure', 'blob', 'mount'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
     ]
```

