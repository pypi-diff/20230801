# Comparing `tmp/aEye-1.1.3.tar.gz` & `tmp/aEye-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aEye-1.1.3.tar", last modified: Tue Aug  1 15:21:15 2023, max compression
+gzip compressed data, was "aEye-1.1.4.tar", last modified: Tue Aug  1 15:28:39 2023, max compression
```

## Comparing `aEye-1.1.3.tar` & `aEye-1.1.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:21:15.144424 aEye-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-01 15:21:04.000000 aEye-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8735 2023-08-01 15:21:15.144424 aEye-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-08-01 15:21:04.000000 aEye-1.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:21:15.144424 aEye-1.1.3/aEye/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-08-01 15:21:04.000000 aEye-1.1.3/aEye/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9359 2023-08-01 15:21:04.000000 aEye-1.1.3/aEye/auxiliary.py
--rw-r--r--   0 runner    (1001) docker     (123)     8677 2023-08-01 15:21:04.000000 aEye-1.1.3/aEye/extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)    19315 2023-08-01 15:21:04.000000 aEye-1.1.3/aEye/labeler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11873 2023-08-01 15:21:04.000000 aEye-1.1.3/aEye/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:21:15.144424 aEye-1.1.3/aEye.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8735 2023-08-01 15:21:15.000000 aEye-1.1.3/aEye.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-08-01 15:21:15.000000 aEye-1.1.3/aEye.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 15:21:15.000000 aEye-1.1.3/aEye.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-01 15:21:15.000000 aEye-1.1.3/aEye.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-01 15:21:15.000000 aEye-1.1.3/aEye.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 15:21:15.144424 aEye-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-08-01 15:21:04.000000 aEye-1.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:21:15.144424 aEye-1.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-08-01 15:21:04.000000 aEye-1.1.3/tests/test_extract_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:28:39.810328 aEye-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-01 15:28:28.000000 aEye-1.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8735 2023-08-01 15:28:39.810328 aEye-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-08-01 15:28:28.000000 aEye-1.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:28:39.810328 aEye-1.1.4/aEye/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-08-01 15:28:28.000000 aEye-1.1.4/aEye/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9183 2023-08-01 15:28:28.000000 aEye-1.1.4/aEye/auxiliary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8677 2023-08-01 15:28:28.000000 aEye-1.1.4/aEye/extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19315 2023-08-01 15:28:28.000000 aEye-1.1.4/aEye/labeler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11873 2023-08-01 15:28:28.000000 aEye-1.1.4/aEye/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:28:39.810328 aEye-1.1.4/aEye.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8735 2023-08-01 15:28:39.000000 aEye-1.1.4/aEye.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-08-01 15:28:39.000000 aEye-1.1.4/aEye.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 15:28:39.000000 aEye-1.1.4/aEye.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-01 15:28:39.000000 aEye-1.1.4/aEye.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-01 15:28:39.000000 aEye-1.1.4/aEye.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 15:28:39.810328 aEye-1.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-08-01 15:28:28.000000 aEye-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:28:39.810328 aEye-1.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-08-01 15:28:28.000000 aEye-1.1.4/tests/test_extract_metadata.py
```

### Comparing `aEye-1.1.3/LICENSE` & `aEye-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aEye-1.1.3/PKG-INFO` & `aEye-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aEye
-Version: 1.1.3
+Version: 1.1.4
 Summary: Extensible Video Processing Framework
 Home-page: https://github.com/DISHDevEx/aEye
 Author-email: devex@dish.com
 License: Dish Wireless
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aEye-1.1.3/README.md` & `aEye-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `aEye-1.1.3/aEye/auxiliary.py` & `aEye-1.1.4/aEye/auxiliary.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,21 +131,25 @@
         """
         video_list = []
 
         if os.path.isdir(path):
             for i in os.listdir(path):
                 new_vid = Video(file=path + i, title=i)
                 new_vid.path = path
+                self._local_path = path
+
                 video_list.append(new_vid)
 
         else:
             dummy = path.replace('/', ' ').strip()
             title = dummy.split(' ')[-1]
             new_vid = Video(file=path, title=title)
             new_vid.path = path
+            self._local_path = path
+
             video_list.append(new_vid)
 
         logging.info(f"successfully load the video files from local path: {path}")
         print(f"Loaded from {path}")
         return video_list
 
     def upload_s3(self, video_list, bucket, prefix='modified/'):
@@ -260,14 +264,7 @@
         Returns
         ----------
 
         """
         self._local_path = path
 
 
-if __name__ == '__main__':
-    aux = Aux()
-    video_list = aux.load_local('/Users/James.Fagan/Documents/Video_Benchmark_Car.mp4')
-    video = video_list[0]
-    print(video)
-    video.extract_metadata()
-    print(video.title, video.path, video.meta_data)
```

### Comparing `aEye-1.1.3/aEye/extractor.py` & `aEye-1.1.4/aEye/extractor.py`

 * *Files identical despite different names*

### Comparing `aEye-1.1.3/aEye/labeler.py` & `aEye-1.1.4/aEye/labeler.py`

 * *Files identical despite different names*

### Comparing `aEye-1.1.3/aEye/video.py` & `aEye-1.1.4/aEye/video.py`

 * *Files identical despite different names*

### Comparing `aEye-1.1.3/aEye.egg-info/PKG-INFO` & `aEye-1.1.4/aEye.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aEye
-Version: 1.1.3
+Version: 1.1.4
 Summary: Extensible Video Processing Framework
 Home-page: https://github.com/DISHDevEx/aEye
 Author-email: devex@dish.com
 License: Dish Wireless
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aEye-1.1.3/setup.py` & `aEye-1.1.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 
 def get_version():
     """
     Checks commandline arguments for a user specified Version number.
     If the --version flag is not given at run time, then the version number is defaulted to
-    v1.1.3, which will later be replaced with a git tag when performing
+    v1.1.4, which will later be replaced with a git tag when performing
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
-    version = 'v1.1.3'
+    version = 'v1.1.4'
     if "--version" in sys.argv:
         try:
             version = sys.argv[3]
             sys.argv.remove(sys.argv[3])
         except IndexError as e:
             print("error:  " + str(e))
             print("supply a version number i.e. --version 1.x.x")
```

### Comparing `aEye-1.1.3/tests/test_extract_metadata.py` & `aEye-1.1.4/tests/test_extract_metadata.py`

 * *Files identical despite different names*

