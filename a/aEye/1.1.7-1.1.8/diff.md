# Comparing `tmp/aEye-1.1.7.tar.gz` & `tmp/aEye-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aEye-1.1.7.tar", last modified: Tue Aug  1 16:53:17 2023, max compression
+gzip compressed data, was "aEye-1.1.8.tar", last modified: Tue Aug  1 17:06:38 2023, max compression
```

## Comparing `aEye-1.1.7.tar` & `aEye-1.1.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:53:17.633826 aEye-1.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-01 16:53:04.000000 aEye-1.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8735 2023-08-01 16:53:17.633826 aEye-1.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-08-01 16:53:04.000000 aEye-1.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:53:17.629826 aEye-1.1.7/aEye/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-08-01 16:53:04.000000 aEye-1.1.7/aEye/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9537 2023-08-01 16:53:04.000000 aEye-1.1.7/aEye/auxiliary.py
--rw-r--r--   0 runner    (1001) docker     (123)     8677 2023-08-01 16:53:04.000000 aEye-1.1.7/aEye/extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)    20072 2023-08-01 16:53:04.000000 aEye-1.1.7/aEye/labeler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11873 2023-08-01 16:53:04.000000 aEye-1.1.7/aEye/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:53:17.633826 aEye-1.1.7/aEye.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8735 2023-08-01 16:53:17.000000 aEye-1.1.7/aEye.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-08-01 16:53:17.000000 aEye-1.1.7/aEye.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 16:53:17.000000 aEye-1.1.7/aEye.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-01 16:53:17.000000 aEye-1.1.7/aEye.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-01 16:53:17.000000 aEye-1.1.7/aEye.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 16:53:17.633826 aEye-1.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-08-01 16:53:04.000000 aEye-1.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:53:17.633826 aEye-1.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-08-01 16:53:04.000000 aEye-1.1.7/tests/test_extract_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:06:38.044994 aEye-1.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-01 17:06:23.000000 aEye-1.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8735 2023-08-01 17:06:38.044994 aEye-1.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-08-01 17:06:23.000000 aEye-1.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:06:38.044994 aEye-1.1.8/aEye/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-08-01 17:06:23.000000 aEye-1.1.8/aEye/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9342 2023-08-01 17:06:23.000000 aEye-1.1.8/aEye/auxiliary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8677 2023-08-01 17:06:23.000000 aEye-1.1.8/aEye/extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20072 2023-08-01 17:06:23.000000 aEye-1.1.8/aEye/labeler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11873 2023-08-01 17:06:23.000000 aEye-1.1.8/aEye/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:06:38.044994 aEye-1.1.8/aEye.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8735 2023-08-01 17:06:38.000000 aEye-1.1.8/aEye.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-08-01 17:06:38.000000 aEye-1.1.8/aEye.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 17:06:38.000000 aEye-1.1.8/aEye.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-01 17:06:38.000000 aEye-1.1.8/aEye.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-01 17:06:38.000000 aEye-1.1.8/aEye.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 17:06:38.044994 aEye-1.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-08-01 17:06:24.000000 aEye-1.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:06:38.044994 aEye-1.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-08-01 17:06:23.000000 aEye-1.1.8/tests/test_extract_metadata.py
```

### Comparing `aEye-1.1.7/LICENSE` & `aEye-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `aEye-1.1.7/PKG-INFO` & `aEye-1.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aEye
-Version: 1.1.7
+Version: 1.1.8
 Summary: Extensible Video Processing Framework
 Home-page: https://github.com/DISHDevEx/aEye
 Author-email: devex@dish.com
 License: Dish Wireless
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aEye-1.1.7/README.md` & `aEye-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `aEye-1.1.7/aEye/auxiliary.py` & `aEye-1.1.8/aEye/auxiliary.py`

 * *Files 6% similar despite different names*

```diff
@@ -164,20 +164,14 @@
             bucket: string
                 The bucket name/path to upload on S3.
 
             prefix: string
                 The subfolder name that the video list will be uploaded to.
 
         """
-
-            # When we request from S3 with the input parameters, the prefix folder will also pop up as a object.
-            # This if-statement is to skip over the folder object since we are only interested in the video files.
-
-
-
         s3 = boto3.client('s3')
         for video in video_list:
             if not self._local_path:
                 path = self._temp_folder + '/' + video.get_output_title()
             else:
                 path = self._local_path #+ '/' + video.get_output_title()
             s3.upload_file(path, bucket, prefix + video.get_output_title())
@@ -215,14 +209,15 @@
         for video in video_list:
             if video.out == '':
                 source = video.get_presigned_url()
             else:
                 source = video.out
             if len(video.complex_filter) > 0:
                 video.create_complex_filter(video)
+            video.get_output_title()
             command = f"{ffmpeg} -y -i {source} {video.get_label()} {path}/{video.get_output_title()}"
             subprocess.run(command, shell=True)
             logging.info(command)
             #print(command)  # REALLY useful for debug
             new_path = video.get_output_title()
             video.reset_label()
             new_video = Video(f'{path}/{video.get_output_title()}', title=f'{video.get_output_title()}')
```

### Comparing `aEye-1.1.7/aEye/extractor.py` & `aEye-1.1.8/aEye/extractor.py`

 * *Files identical despite different names*

### Comparing `aEye-1.1.7/aEye/labeler.py` & `aEye-1.1.8/aEye/labeler.py`

 * *Files identical despite different names*

### Comparing `aEye-1.1.7/aEye/video.py` & `aEye-1.1.8/aEye/video.py`

 * *Files identical despite different names*

### Comparing `aEye-1.1.7/aEye.egg-info/PKG-INFO` & `aEye-1.1.8/aEye.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aEye
-Version: 1.1.7
+Version: 1.1.8
 Summary: Extensible Video Processing Framework
 Home-page: https://github.com/DISHDevEx/aEye
 Author-email: devex@dish.com
 License: Dish Wireless
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aEye-1.1.7/setup.py` & `aEye-1.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 
 def get_version():
     """
     Checks commandline arguments for a user specified Version number.
     If the --version flag is not given at run time, then the version number is defaulted to
-    v1.1.7, which will later be replaced with a git tag when performing
+    v1.1.8, which will later be replaced with a git tag when performing
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
-    version = 'v1.1.7'
+    version = 'v1.1.8'
     if "--version" in sys.argv:
         try:
             version = sys.argv[3]
             sys.argv.remove(sys.argv[3])
         except IndexError as e:
             print("error:  " + str(e))
             print("supply a version number i.e. --version 1.x.x")
```

### Comparing `aEye-1.1.7/tests/test_extract_metadata.py` & `aEye-1.1.8/tests/test_extract_metadata.py`

 * *Files identical despite different names*

