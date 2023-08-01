# Comparing `tmp/blob_mounting_helper_utility-1.0.5.tar.gz` & `tmp/blob_mounting_helper_utility-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blob_mounting_helper_utility-1.0.5.tar", last modified: Tue Aug  1 10:44:40 2023, max compression
+gzip compressed data, was "blob_mounting_helper_utility-1.0.6.tar", last modified: Tue Aug  1 10:47:11 2023, max compression
```

## Comparing `blob_mounting_helper_utility-1.0.5.tar` & `blob_mounting_helper_utility-1.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 ivica     (1000) ivica     (1000)        0 2023-08-01 10:44:40.047699 blob_mounting_helper_utility-1.0.5/
--rw-rw-r--   0 ivica     (1000) ivica     (1000)     2559 2023-08-01 10:44:40.043699 blob_mounting_helper_utility-1.0.5/PKG-INFO
--rw-rw-r--   0 ivica     (1000) ivica     (1000)     2029 2023-06-15 13:30:00.000000 blob_mounting_helper_utility-1.0.5/README.md
-drwxrwxr-x   0 ivica     (1000) ivica     (1000)        0 2023-08-01 10:44:40.043699 blob_mounting_helper_utility-1.0.5/blob_mounting_helper_utility/
--rw-rw-r--   0 ivica     (1000) ivica     (1000)       37 2023-06-15 11:11:15.000000 blob_mounting_helper_utility-1.0.5/blob_mounting_helper_utility/__init__.py
--rw-rw-r--   0 ivica     (1000) ivica     (1000)     6328 2023-08-01 10:44:30.000000 blob_mounting_helper_utility-1.0.5/blob_mounting_helper_utility/utils.py
-drwxrwxr-x   0 ivica     (1000) ivica     (1000)        0 2023-08-01 10:44:40.043699 blob_mounting_helper_utility-1.0.5/blob_mounting_helper_utility.egg-info/
--rw-rw-r--   0 ivica     (1000) ivica     (1000)     2559 2023-08-01 10:44:40.000000 blob_mounting_helper_utility-1.0.5/blob_mounting_helper_utility.egg-info/PKG-INFO
--rw-rw-r--   0 ivica     (1000) ivica     (1000)      356 2023-08-01 10:44:40.000000 blob_mounting_helper_utility-1.0.5/blob_mounting_helper_utility.egg-info/SOURCES.txt
--rw-rw-r--   0 ivica     (1000) ivica     (1000)        1 2023-08-01 10:44:40.000000 blob_mounting_helper_utility-1.0.5/blob_mounting_helper_utility.egg-info/dependency_links.txt
--rw-rw-r--   0 ivica     (1000) ivica     (1000)       28 2023-08-01 10:44:40.000000 blob_mounting_helper_utility-1.0.5/blob_mounting_helper_utility.egg-info/requires.txt
--rw-rw-r--   0 ivica     (1000) ivica     (1000)       29 2023-08-01 10:44:40.000000 blob_mounting_helper_utility-1.0.5/blob_mounting_helper_utility.egg-info/top_level.txt
--rw-rw-r--   0 ivica     (1000) ivica     (1000)       38 2023-08-01 10:44:40.047699 blob_mounting_helper_utility-1.0.5/setup.cfg
--rw-rw-r--   0 ivica     (1000) ivica     (1000)     1055 2023-08-01 10:44:39.000000 blob_mounting_helper_utility-1.0.5/setup.py
+drwxrwxr-x   0 ivica     (1000) ivica     (1000)        0 2023-08-01 10:47:11.846619 blob_mounting_helper_utility-1.0.6/
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)     2559 2023-08-01 10:47:11.846619 blob_mounting_helper_utility-1.0.6/PKG-INFO
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)     2029 2023-06-15 13:30:00.000000 blob_mounting_helper_utility-1.0.6/README.md
+drwxrwxr-x   0 ivica     (1000) ivica     (1000)        0 2023-08-01 10:47:11.842620 blob_mounting_helper_utility-1.0.6/blob_mounting_helper_utility/
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)       37 2023-06-15 11:11:15.000000 blob_mounting_helper_utility-1.0.6/blob_mounting_helper_utility/__init__.py
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)     6281 2023-08-01 10:47:03.000000 blob_mounting_helper_utility-1.0.6/blob_mounting_helper_utility/utils.py
+drwxrwxr-x   0 ivica     (1000) ivica     (1000)        0 2023-08-01 10:47:11.846619 blob_mounting_helper_utility-1.0.6/blob_mounting_helper_utility.egg-info/
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)     2559 2023-08-01 10:47:11.000000 blob_mounting_helper_utility-1.0.6/blob_mounting_helper_utility.egg-info/PKG-INFO
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)      356 2023-08-01 10:47:11.000000 blob_mounting_helper_utility-1.0.6/blob_mounting_helper_utility.egg-info/SOURCES.txt
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)        1 2023-08-01 10:47:11.000000 blob_mounting_helper_utility-1.0.6/blob_mounting_helper_utility.egg-info/dependency_links.txt
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)       28 2023-08-01 10:47:11.000000 blob_mounting_helper_utility-1.0.6/blob_mounting_helper_utility.egg-info/requires.txt
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)       29 2023-08-01 10:47:11.000000 blob_mounting_helper_utility-1.0.6/blob_mounting_helper_utility.egg-info/top_level.txt
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)       38 2023-08-01 10:47:11.846619 blob_mounting_helper_utility-1.0.6/setup.cfg
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)     1055 2023-08-01 10:47:10.000000 blob_mounting_helper_utility-1.0.6/setup.py
```

### Comparing `blob_mounting_helper_utility-1.0.5/PKG-INFO` & `blob_mounting_helper_utility-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blob_mounting_helper_utility
-Version: 1.0.5
+Version: 1.0.6
 Summary: Blob mapping utility for easy translation between azure urls and local paths
 Home-page: UNKNOWN
 Author: Ivica Matic
 Author-email: <ivica.matic@spatialdays.com>
 License: UNKNOWN
 Keywords: python,azure,blob,mount
 Platform: UNKNOWN
```

### Comparing `blob_mounting_helper_utility-1.0.5/README.md` & `blob_mounting_helper_utility-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `blob_mounting_helper_utility-1.0.5/blob_mounting_helper_utility/utils.py` & `blob_mounting_helper_utility-1.0.6/blob_mounting_helper_utility/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,18 +104,17 @@
             self.downloaded_paths.append(download_file_path)
         else:
             logger.debug(f"Blob already downloaded to {download_file_path}")
 
     def upload_blob(self, file_path: str) -> None:
         logger.debug(f"Uploading blob from {file_path}")
         blob_client = BlobClient.from_blob_url(self.get_url_from_mounted_filepath(file_path),
-                                               credential=self.azure_storage_account_key,
-                                               overwrite=True)
+                                               credential=self.azure_storage_account_key)
         with open(file_path, "rb") as data:
-            blob_client.upload_blob(data)
+            blob_client.upload_blob(data, overwrite=True)
         if file_path not in self.uploaded_paths:
             self.uploaded_paths.append(file_path)
         logger.debug(f"Uploaded blob from {file_path}")
 
     def cleanup_files(self) -> None:
         logger.debug("Cleaning up files")
         for file_path in self.downloaded_paths:
```

### Comparing `blob_mounting_helper_utility-1.0.5/blob_mounting_helper_utility.egg-info/PKG-INFO` & `blob_mounting_helper_utility-1.0.6/blob_mounting_helper_utility.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blob-mounting-helper-utility
-Version: 1.0.5
+Version: 1.0.6
 Summary: Blob mapping utility for easy translation between azure urls and local paths
 Home-page: UNKNOWN
 Author: Ivica Matic
 Author-email: <ivica.matic@spatialdays.com>
 License: UNKNOWN
 Keywords: python,azure,blob,mount
 Platform: UNKNOWN
```

### Comparing `blob_mounting_helper_utility-1.0.5/setup.py` & `blob_mounting_helper_utility-1.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.0.5'
+VERSION = '1.0.6'
 DESCRIPTION = 'Blob mapping utility for easy translation between azure urls and local paths'
 LONG_DESCRIPTION = 'Blob mapping utility for easy translation between azure urls and local paths'
 
 # Setting up
 setup(
     name="blob_mounting_helper_utility",
     version=VERSION,
```

