# Comparing `tmp/blob_mounting_helper_utility-1.0.7.tar.gz` & `tmp/blob_mounting_helper_utility-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blob_mounting_helper_utility-1.0.7.tar", last modified: Tue Aug  1 10:52:14 2023, max compression
+gzip compressed data, was "blob_mounting_helper_utility-1.0.8.tar", last modified: Tue Aug  1 13:16:54 2023, max compression
```

## Comparing `blob_mounting_helper_utility-1.0.7.tar` & `blob_mounting_helper_utility-1.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 ivica     (1000) ivica     (1000)        0 2023-08-01 10:52:14.164950 blob_mounting_helper_utility-1.0.7/
--rw-rw-r--   0 ivica     (1000) ivica     (1000)     2559 2023-08-01 10:52:14.164950 blob_mounting_helper_utility-1.0.7/PKG-INFO
--rw-rw-r--   0 ivica     (1000) ivica     (1000)     2029 2023-06-15 13:30:00.000000 blob_mounting_helper_utility-1.0.7/README.md
-drwxrwxr-x   0 ivica     (1000) ivica     (1000)        0 2023-08-01 10:52:14.164950 blob_mounting_helper_utility-1.0.7/blob_mounting_helper_utility/
--rw-rw-r--   0 ivica     (1000) ivica     (1000)       37 2023-06-15 11:11:15.000000 blob_mounting_helper_utility-1.0.7/blob_mounting_helper_utility/__init__.py
--rw-rw-r--   0 ivica     (1000) ivica     (1000)     6264 2023-08-01 10:52:03.000000 blob_mounting_helper_utility-1.0.7/blob_mounting_helper_utility/utils.py
-drwxrwxr-x   0 ivica     (1000) ivica     (1000)        0 2023-08-01 10:52:14.164950 blob_mounting_helper_utility-1.0.7/blob_mounting_helper_utility.egg-info/
--rw-rw-r--   0 ivica     (1000) ivica     (1000)     2559 2023-08-01 10:52:14.000000 blob_mounting_helper_utility-1.0.7/blob_mounting_helper_utility.egg-info/PKG-INFO
--rw-rw-r--   0 ivica     (1000) ivica     (1000)      356 2023-08-01 10:52:14.000000 blob_mounting_helper_utility-1.0.7/blob_mounting_helper_utility.egg-info/SOURCES.txt
--rw-rw-r--   0 ivica     (1000) ivica     (1000)        1 2023-08-01 10:52:14.000000 blob_mounting_helper_utility-1.0.7/blob_mounting_helper_utility.egg-info/dependency_links.txt
--rw-rw-r--   0 ivica     (1000) ivica     (1000)       28 2023-08-01 10:52:14.000000 blob_mounting_helper_utility-1.0.7/blob_mounting_helper_utility.egg-info/requires.txt
--rw-rw-r--   0 ivica     (1000) ivica     (1000)       29 2023-08-01 10:52:14.000000 blob_mounting_helper_utility-1.0.7/blob_mounting_helper_utility.egg-info/top_level.txt
--rw-rw-r--   0 ivica     (1000) ivica     (1000)       38 2023-08-01 10:52:14.164950 blob_mounting_helper_utility-1.0.7/setup.cfg
--rw-rw-r--   0 ivica     (1000) ivica     (1000)     1055 2023-08-01 10:52:11.000000 blob_mounting_helper_utility-1.0.7/setup.py
+drwxrwxr-x   0 ivica     (1000) ivica     (1000)        0 2023-08-01 13:16:54.392139 blob_mounting_helper_utility-1.0.8/
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)     2559 2023-08-01 13:16:54.392139 blob_mounting_helper_utility-1.0.8/PKG-INFO
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)     2029 2023-06-15 13:30:00.000000 blob_mounting_helper_utility-1.0.8/README.md
+drwxrwxr-x   0 ivica     (1000) ivica     (1000)        0 2023-08-01 13:16:54.392139 blob_mounting_helper_utility-1.0.8/blob_mounting_helper_utility/
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)       37 2023-06-15 11:11:15.000000 blob_mounting_helper_utility-1.0.8/blob_mounting_helper_utility/__init__.py
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)     6602 2023-08-01 13:16:37.000000 blob_mounting_helper_utility-1.0.8/blob_mounting_helper_utility/utils.py
+drwxrwxr-x   0 ivica     (1000) ivica     (1000)        0 2023-08-01 13:16:54.392139 blob_mounting_helper_utility-1.0.8/blob_mounting_helper_utility.egg-info/
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)     2559 2023-08-01 13:16:54.000000 blob_mounting_helper_utility-1.0.8/blob_mounting_helper_utility.egg-info/PKG-INFO
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)      356 2023-08-01 13:16:54.000000 blob_mounting_helper_utility-1.0.8/blob_mounting_helper_utility.egg-info/SOURCES.txt
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)        1 2023-08-01 13:16:54.000000 blob_mounting_helper_utility-1.0.8/blob_mounting_helper_utility.egg-info/dependency_links.txt
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)       28 2023-08-01 13:16:54.000000 blob_mounting_helper_utility-1.0.8/blob_mounting_helper_utility.egg-info/requires.txt
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)       29 2023-08-01 13:16:54.000000 blob_mounting_helper_utility-1.0.8/blob_mounting_helper_utility.egg-info/top_level.txt
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)       38 2023-08-01 13:16:54.392139 blob_mounting_helper_utility-1.0.8/setup.cfg
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)     1055 2023-08-01 13:16:48.000000 blob_mounting_helper_utility-1.0.8/setup.py
```

### Comparing `blob_mounting_helper_utility-1.0.7/PKG-INFO` & `blob_mounting_helper_utility-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blob_mounting_helper_utility
-Version: 1.0.7
+Version: 1.0.8
 Summary: Blob mapping utility for easy translation between azure urls and local paths
 Home-page: UNKNOWN
 Author: Ivica Matic
 Author-email: <ivica.matic@spatialdays.com>
 License: UNKNOWN
 Keywords: python,azure,blob,mount
 Platform: UNKNOWN
```

### Comparing `blob_mounting_helper_utility-1.0.7/README.md` & `blob_mounting_helper_utility-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `blob_mounting_helper_utility-1.0.7/blob_mounting_helper_utility/utils.py` & `blob_mounting_helper_utility-1.0.8/blob_mounting_helper_utility/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -116,13 +116,23 @@
         logger.debug(f"Uploaded blob from {file_path}")
 
     def cleanup_files(self) -> None:
         logger.debug("Cleaning up files")
         for file_path in self.downloaded_paths:
             logger.debug(f"Removing downloaded file {file_path}")
             os.remove(file_path)
+            # remove the directory if it is empty
+            try:
+                os.rmdir(os.path.dirname(file_path))
+            except OSError:
+                pass
         for file_path in self.uploaded_paths:
             logger.debug(f"Removing uploaded file {file_path}")
             os.remove(file_path)
+            # remove the directory if it is empty
+            try:
+                os.rmdir(os.path.dirname(file_path))
+            except OSError:
+                pass
         self.downloaded_paths = []
         self.uploaded_paths = []
         logger.debug("Cleaned up files")
```

### Comparing `blob_mounting_helper_utility-1.0.7/blob_mounting_helper_utility.egg-info/PKG-INFO` & `blob_mounting_helper_utility-1.0.8/blob_mounting_helper_utility.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blob-mounting-helper-utility
-Version: 1.0.7
+Version: 1.0.8
 Summary: Blob mapping utility for easy translation between azure urls and local paths
 Home-page: UNKNOWN
 Author: Ivica Matic
 Author-email: <ivica.matic@spatialdays.com>
 License: UNKNOWN
 Keywords: python,azure,blob,mount
 Platform: UNKNOWN
```

### Comparing `blob_mounting_helper_utility-1.0.7/setup.py` & `blob_mounting_helper_utility-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.0.7'
+VERSION = '1.0.8'
 DESCRIPTION = 'Blob mapping utility for easy translation between azure urls and local paths'
 LONG_DESCRIPTION = 'Blob mapping utility for easy translation between azure urls and local paths'
 
 # Setting up
 setup(
     name="blob_mounting_helper_utility",
     version=VERSION,
```

