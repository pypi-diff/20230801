# Comparing `tmp/aEye-1.1.1.tar.gz` & `tmp/aEye-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aEye-1.1.1.tar", last modified: Tue Jul 25 20:07:47 2023, max compression
+gzip compressed data, was "aEye-1.1.2.tar", last modified: Tue Aug  1 15:14:11 2023, max compression
```

## Comparing `aEye-1.1.1.tar` & `aEye-1.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:07:47.497064 aEye-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-25 20:07:33.000000 aEye-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8735 2023-07-25 20:07:47.497064 aEye-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-07-25 20:07:33.000000 aEye-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:07:47.497064 aEye-1.1.1/aEye/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-25 20:07:33.000000 aEye-1.1.1/aEye/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9093 2023-07-25 20:07:33.000000 aEye-1.1.1/aEye/auxiliary.py
--rw-r--r--   0 runner    (1001) docker     (123)     8677 2023-07-25 20:07:33.000000 aEye-1.1.1/aEye/extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)    19315 2023-07-25 20:07:33.000000 aEye-1.1.1/aEye/labeler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11873 2023-07-25 20:07:33.000000 aEye-1.1.1/aEye/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:07:47.497064 aEye-1.1.1/aEye.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8735 2023-07-25 20:07:47.000000 aEye-1.1.1/aEye.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-25 20:07:47.000000 aEye-1.1.1/aEye.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 20:07:47.000000 aEye-1.1.1/aEye.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-25 20:07:47.000000 aEye-1.1.1/aEye.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-25 20:07:47.000000 aEye-1.1.1/aEye.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 20:07:47.497064 aEye-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-25 20:07:33.000000 aEye-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:07:47.497064 aEye-1.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-25 20:07:33.000000 aEye-1.1.1/tests/test_extract_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:14:11.859348 aEye-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-01 15:13:59.000000 aEye-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8735 2023-08-01 15:14:11.859348 aEye-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-08-01 15:13:59.000000 aEye-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:14:11.859348 aEye-1.1.2/aEye/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-08-01 15:13:59.000000 aEye-1.1.2/aEye/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9359 2023-08-01 15:13:59.000000 aEye-1.1.2/aEye/auxiliary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8677 2023-08-01 15:13:59.000000 aEye-1.1.2/aEye/extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19315 2023-08-01 15:13:59.000000 aEye-1.1.2/aEye/labeler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11873 2023-08-01 15:13:59.000000 aEye-1.1.2/aEye/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:14:11.859348 aEye-1.1.2/aEye.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8735 2023-08-01 15:14:11.000000 aEye-1.1.2/aEye.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-08-01 15:14:11.000000 aEye-1.1.2/aEye.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 15:14:11.000000 aEye-1.1.2/aEye.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-01 15:14:11.000000 aEye-1.1.2/aEye.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-01 15:14:11.000000 aEye-1.1.2/aEye.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 15:14:11.859348 aEye-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-08-01 15:13:59.000000 aEye-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:14:11.859348 aEye-1.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-08-01 15:13:59.000000 aEye-1.1.2/tests/test_extract_metadata.py
```

### Comparing `aEye-1.1.1/LICENSE` & `aEye-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aEye-1.1.1/PKG-INFO` & `aEye-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aEye
-Version: 1.1.1
+Version: 1.1.2
 Summary: Extensible Video Processing Framework
 Home-page: https://github.com/DISHDevEx/aEye
 Author-email: devex@dish.com
 License: Dish Wireless
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aEye-1.1.1/README.md` & `aEye-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `aEye-1.1.1/aEye/auxiliary.py` & `aEye-1.1.2/aEye/auxiliary.py`

 * *Files 6% similar despite different names*

```diff
@@ -130,26 +130,26 @@
             The list of all video files loaded from local bucket.
         """
         video_list = []
 
         if os.path.isdir(path):
             for i in os.listdir(path):
                 new_vid = Video(file=path + i, title=i)
-                new_vid.path = self._temp_folder
+                new_vid.path = path
                 video_list.append(new_vid)
 
         else:
             dummy = path.replace('/', ' ').strip()
             title = dummy.split(' ')[-1]
             new_vid = Video(file=path, title=title)
-            new_vid.path = self._temp_folder
+            new_vid.path = path
             video_list.append(new_vid)
 
         logging.info(f"successfully load the video files from local path: {path}")
-
+        print(f"Loaded from {path}")
         return video_list
 
     def upload_s3(self, video_list, bucket, prefix='modified/'):
         """
         This method will push modified video list to the S3 bucket and delete all video files from local temp folder.
 
         Parameters
@@ -258,7 +258,16 @@
             The path to set
 
         Returns
         ----------
 
         """
         self._local_path = path
+
+
+if __name__ == '__main__':
+    aux = Aux()
+    video_list = aux.load_local('/Users/James.Fagan/Documents/Video_Benchmark_Car.mp4')
+    video = video_list[0]
+    print(video)
+    video.extract_metadata()
+    print(video.title, video.path, video.meta_data)
```

### Comparing `aEye-1.1.1/aEye/extractor.py` & `aEye-1.1.2/aEye/extractor.py`

 * *Files identical despite different names*

### Comparing `aEye-1.1.1/aEye/labeler.py` & `aEye-1.1.2/aEye/labeler.py`

 * *Files identical despite different names*

### Comparing `aEye-1.1.1/aEye/video.py` & `aEye-1.1.2/aEye/video.py`

 * *Files identical despite different names*

### Comparing `aEye-1.1.1/aEye.egg-info/PKG-INFO` & `aEye-1.1.2/aEye.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aEye
-Version: 1.1.1
+Version: 1.1.2
 Summary: Extensible Video Processing Framework
 Home-page: https://github.com/DISHDevEx/aEye
 Author-email: devex@dish.com
 License: Dish Wireless
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aEye-1.1.1/setup.py` & `aEye-1.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 
 def get_version():
     """
     Checks commandline arguments for a user specified Version number.
     If the --version flag is not given at run time, then the version number is defaulted to
-    v1.1.1, which will later be replaced with a git tag when performing
+    v1.1.2, which will later be replaced with a git tag when performing
     version releases.
 
     Returns
     -------
     when the bdist_wheel command is given a version flag and version number, such as:
 
     --version 1.x.x
@@ -36,15 +36,15 @@
     If the --version flag is given, but no version number is supplied, such as:
 
     --version
 
     then an IndexError will be thrown and the build will exit with exit status 1.
 
     """
-    version = 'v1.1.1'
+    version = 'v1.1.2'
     if "--version" in sys.argv:
         try:
             version = sys.argv[3]
             sys.argv.remove(sys.argv[3])
         except IndexError as e:
             print("error:  " + str(e))
             print("supply a version number i.e. --version 1.x.x")
```

### Comparing `aEye-1.1.1/tests/test_extract_metadata.py` & `aEye-1.1.2/tests/test_extract_metadata.py`

 * *Files identical despite different names*

