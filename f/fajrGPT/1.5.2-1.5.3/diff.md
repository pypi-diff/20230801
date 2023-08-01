# Comparing `tmp/fajrGPT-1.5.2.tar.gz` & `tmp/fajrGPT-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fajrGPT-1.5.2.tar", last modified: Mon Jul 31 11:28:08 2023, max compression
+gzip compressed data, was "fajrGPT-1.5.3.tar", last modified: Tue Aug  1 02:31:47 2023, max compression
```

## Comparing `fajrGPT-1.5.2.tar` & `fajrGPT-1.5.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-31 11:28:08.756057 fajrGPT-1.5.2/
--rw-r--r--   0 malek8     (501) staff       (20)     1062 2023-05-15 07:44:33.000000 fajrGPT-1.5.2/LICENSE
--rw-r--r--   0 malek8     (501) staff       (20)     2946 2023-07-31 11:28:08.755885 fajrGPT-1.5.2/PKG-INFO
--rw-r--r--   0 malek8     (501) staff       (20)     2283 2023-06-12 00:59:24.000000 fajrGPT-1.5.2/README.md
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-31 11:28:08.754543 fajrGPT-1.5.2/fajrGPT/
--rw-r--r--   0 malek8     (501) staff       (20)        0 2023-06-12 01:14:16.000000 fajrGPT-1.5.2/fajrGPT/__init__.py
--rw-r--r--   0 malek8     (501) staff       (20)     4095 2023-07-31 02:16:34.000000 fajrGPT-1.5.2/fajrGPT/quran_metadata.py
--rw-r--r--   0 malek8     (501) staff       (20)    22056 2023-07-31 11:25:34.000000 fajrGPT-1.5.2/fajrGPT/wake.py
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-31 11:28:08.755683 fajrGPT-1.5.2/fajrGPT.egg-info/
--rw-r--r--   0 malek8     (501) staff       (20)     2946 2023-07-31 11:28:08.000000 fajrGPT-1.5.2/fajrGPT.egg-info/PKG-INFO
--rw-r--r--   0 malek8     (501) staff       (20)      276 2023-07-31 11:28:08.000000 fajrGPT-1.5.2/fajrGPT.egg-info/SOURCES.txt
--rw-r--r--   0 malek8     (501) staff       (20)        1 2023-07-31 11:28:08.000000 fajrGPT-1.5.2/fajrGPT.egg-info/dependency_links.txt
--rw-r--r--   0 malek8     (501) staff       (20)       46 2023-07-31 11:28:08.000000 fajrGPT-1.5.2/fajrGPT.egg-info/entry_points.txt
--rw-r--r--   0 malek8     (501) staff       (20)       62 2023-07-31 11:28:08.000000 fajrGPT-1.5.2/fajrGPT.egg-info/requires.txt
--rw-r--r--   0 malek8     (501) staff       (20)        8 2023-07-31 11:28:08.000000 fajrGPT-1.5.2/fajrGPT.egg-info/top_level.txt
--rw-r--r--   0 malek8     (501) staff       (20)       38 2023-07-31 11:28:08.756097 fajrGPT-1.5.2/setup.cfg
--rw-r--r--   0 malek8     (501) staff       (20)     1148 2023-07-31 11:27:21.000000 fajrGPT-1.5.2/setup.py
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-08-01 02:31:47.211844 fajrGPT-1.5.3/
+-rw-r--r--   0 malek8     (501) staff       (20)     1062 2023-05-15 07:44:33.000000 fajrGPT-1.5.3/LICENSE
+-rw-r--r--   0 malek8     (501) staff       (20)     2946 2023-08-01 02:31:47.211647 fajrGPT-1.5.3/PKG-INFO
+-rw-r--r--   0 malek8     (501) staff       (20)     2283 2023-06-12 00:59:24.000000 fajrGPT-1.5.3/README.md
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-08-01 02:31:47.207912 fajrGPT-1.5.3/fajrGPT/
+-rw-r--r--   0 malek8     (501) staff       (20)        0 2023-06-12 01:14:16.000000 fajrGPT-1.5.3/fajrGPT/__init__.py
+-rw-r--r--   0 malek8     (501) staff       (20)     4095 2023-07-31 02:16:34.000000 fajrGPT-1.5.3/fajrGPT/quran_metadata.py
+-rw-r--r--   0 malek8     (501) staff       (20)    22056 2023-07-31 11:25:34.000000 fajrGPT-1.5.3/fajrGPT/wake.py
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-08-01 02:31:47.211414 fajrGPT-1.5.3/fajrGPT.egg-info/
+-rw-r--r--   0 malek8     (501) staff       (20)     2946 2023-08-01 02:31:47.000000 fajrGPT-1.5.3/fajrGPT.egg-info/PKG-INFO
+-rw-r--r--   0 malek8     (501) staff       (20)      276 2023-08-01 02:31:47.000000 fajrGPT-1.5.3/fajrGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 malek8     (501) staff       (20)        1 2023-08-01 02:31:47.000000 fajrGPT-1.5.3/fajrGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       46 2023-08-01 02:31:47.000000 fajrGPT-1.5.3/fajrGPT.egg-info/entry_points.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       68 2023-08-01 02:31:47.000000 fajrGPT-1.5.3/fajrGPT.egg-info/requires.txt
+-rw-r--r--   0 malek8     (501) staff       (20)        8 2023-08-01 02:31:47.000000 fajrGPT-1.5.3/fajrGPT.egg-info/top_level.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       38 2023-08-01 02:31:47.211884 fajrGPT-1.5.3/setup.cfg
+-rw-r--r--   0 malek8     (501) staff       (20)     1165 2023-08-01 02:31:08.000000 fajrGPT-1.5.3/setup.py
```

### Comparing `fajrGPT-1.5.2/LICENSE` & `fajrGPT-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fajrGPT-1.5.2/PKG-INFO` & `fajrGPT-1.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fajrGPT
-Version: 1.5.2
+Version: 1.5.3
 Summary: A Python application to assist in waking up for Fajr prayer by providing 3 interactive verses/explanations from the Quran + ChatGPT explanations accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube.
 Home-page: https://github.com/malekinho8/quran-wake-up
 Author: Malek Ibrahim
 Author-email: shmeek8@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fajrGPT-1.5.2/README.md` & `fajrGPT-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `fajrGPT-1.5.2/fajrGPT/quran_metadata.py` & `fajrGPT-1.5.3/fajrGPT/quran_metadata.py`

 * *Files identical despite different names*

### Comparing `fajrGPT-1.5.2/fajrGPT/wake.py` & `fajrGPT-1.5.3/fajrGPT/wake.py`

 * *Files identical despite different names*

### Comparing `fajrGPT-1.5.2/fajrGPT.egg-info/PKG-INFO` & `fajrGPT-1.5.3/fajrGPT.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fajrGPT
-Version: 1.5.2
+Version: 1.5.3
 Summary: A Python application to assist in waking up for Fajr prayer by providing 3 interactive verses/explanations from the Quran + ChatGPT explanations accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube.
 Home-page: https://github.com/malekinho8/quran-wake-up
 Author: Malek Ibrahim
 Author-email: shmeek8@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fajrGPT-1.5.2/setup.py` & `fajrGPT-1.5.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="fajrGPT",
-    version="1.5.2",
+    version="1.5.3",
     author="Malek Ibrahim",
     author_email="shmeek8@gmail.com",
     description=("A Python application to assist in waking up for Fajr prayer "
                  "by providing 3 interactive verses/explanations from the Quran + ChatGPT explanations "
                  "accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube."),
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
@@ -23,14 +23,15 @@
         "click",
         "pygame",
         "pydub",
         "moviepy",
         "openai",
         "tqdm",
         "mutagen",
+        "scipy",
         "TheQuranModule"
     ],
     entry_points={
         'console_scripts': [
             'fajrGPT=fajrGPT.wake:main',
         ],
     },
```

