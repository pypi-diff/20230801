# Comparing `tmp/pytessng-0.1.7.tar.gz` & `tmp/pytessng-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pytessng-0.1.7.tar", last modified: Mon Jul 31 10:18:07 2023, max compression
+gzip compressed data, was "dist\pytessng-0.1.8.tar", last modified: Tue Aug  1 01:24:32 2023, max compression
```

## Comparing `pytessng-0.1.7.tar` & `pytessng-0.1.8.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 10:18:07.000000 pytessng-0.1.7/
--rw-rw-rw-   0        0        0     1067 2022-10-20 09:37:40.000000 pytessng-0.1.7/LICENSE
--rw-rw-rw-   0        0        0      496 2023-07-31 10:18:07.000000 pytessng-0.1.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-31 10:18:07.000000 pytessng-0.1.7/pytessng/
--rw-rw-rw-   0        0        0    11774 2023-07-31 10:16:30.000000 pytessng-0.1.7/pytessng/DockWidget.py
--rw-rw-rw-   0        0        0    10752 2023-05-11 02:45:30.000000 pytessng-0.1.7/pytessng/GKlib.dll
--rw-rw-rw-   0        0        0  2892800 2022-12-23 03:33:45.000000 pytessng-0.1.7/pytessng/libcrypto-1_1-x64.dll
--rw-rw-rw-   0        0        0  2892800 2022-12-23 03:33:45.000000 pytessng-0.1.7/pytessng/libcrypto-1_1-x64_28.dll
--rw-rw-rw-   0        0        0  3433984 2023-03-01 09:43:29.000000 pytessng-0.1.7/pytessng/libcrypto-1_1-x64_35.dll
--rw-rw-rw-   0        0        0  2518016 2022-10-27 03:37:06.000000 pytessng-0.1.7/pytessng/libprotobuf.dll
--rw-rw-rw-   0        0        0      716 2023-06-21 10:44:15.000000 pytessng-0.1.7/pytessng/main.py
--rw-rw-rw-   0        0        0   455680 2023-05-11 02:52:50.000000 pytessng-0.1.7/pytessng/metis.dll
--rw-rw-rw-   0        0        0      701 2023-04-23 03:05:58.000000 pytessng-0.1.7/pytessng/MyNet.py
--rw-rw-rw-   0        0        0     1534 2023-06-21 10:47:15.000000 pytessng-0.1.7/pytessng/MyPlugin.py
--rw-rw-rw-   0        0        0  3209216 2023-07-10 03:01:09.000000 pytessng-0.1.7/pytessng/TessCluster.dll
--rw-rw-rw-   0        0        0   413696 2023-07-26 15:03:42.000000 pytessng-0.1.7/pytessng/TessInterfaces.dll
--rw-rw-rw-   0        0        0  1446400 2023-07-27 01:41:04.000000 pytessng-0.1.7/pytessng/Tessng.pyd
--rw-rw-rw-   0        0        0    72636 2023-06-27 07:08:31.000000 pytessng-0.1.7/pytessng/Tessng.pyi
--rw-rw-rw-   0        0        0   155648 2023-07-26 15:03:34.000000 pytessng-0.1.7/pytessng/TessSupport.dll
--rw-rw-rw-   0        0        0    13425 2023-07-31 10:16:30.000000 pytessng-0.1.7/pytessng/TESS_API_EXAMPLE.py
--rw-rw-rw-   0        0        0  1320960 2023-07-26 15:04:34.000000 pytessng-0.1.7/pytessng/TESS_DB.dll
--rw-rw-rw-   0        0        0  2080768 2023-07-26 15:04:48.000000 pytessng-0.1.7/pytessng/TESS_NET.dll
--rw-rw-rw-   0        0        0  1082368 2023-07-27 01:32:58.000000 pytessng-0.1.7/pytessng/TESS_SIMU.dll
--rw-rw-rw-   0        0        0  3245056 2023-07-26 15:06:36.000000 pytessng-0.1.7/pytessng/TESS_WIN.dll
-drwxrwxrwx   0        0        0        0 2023-07-31 10:18:07.000000 pytessng-0.1.7/pytessng/utils/
--rw-rw-rw-   0        0        0    24535 2023-07-31 03:25:54.000000 pytessng-0.1.7/pytessng/utils/functions.py
--rw-rw-rw-   0        0        0        0 2023-03-13 03:59:50.000000 pytessng-0.1.7/pytessng/utils/__init__.py
--rw-rw-rw-   0        0        0      194 2023-03-13 03:59:50.000000 pytessng-0.1.7/pytessng/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 10:18:07.000000 pytessng-0.1.7/pytessng.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-31 10:18:07.000000 pytessng-0.1.7/pytessng.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      496 2023-07-31 10:18:07.000000 pytessng-0.1.7/pytessng.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       55 2023-07-31 10:18:07.000000 pytessng-0.1.7/pytessng.egg-info/requires.txt
--rw-rw-rw-   0        0        0      737 2023-07-31 10:18:07.000000 pytessng-0.1.7/pytessng.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        9 2023-07-31 10:18:07.000000 pytessng-0.1.7/pytessng.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       54 2022-10-20 06:33:19.000000 pytessng-0.1.7/README.md
--rw-rw-rw-   0        0        0       42 2023-07-31 10:18:07.000000 pytessng-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      847 2023-07-31 10:17:30.000000 pytessng-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:24:32.000000 pytessng-0.1.8/
+-rw-rw-rw-   0        0        0     1067 2022-10-20 09:37:40.000000 pytessng-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0      496 2023-08-01 01:24:32.000000 pytessng-0.1.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-01 01:24:32.000000 pytessng-0.1.8/pytessng/
+-rw-rw-rw-   0        0        0    11774 2023-07-31 10:16:30.000000 pytessng-0.1.8/pytessng/DockWidget.py
+-rw-rw-rw-   0        0        0    10752 2023-05-11 02:45:30.000000 pytessng-0.1.8/pytessng/GKlib.dll
+-rw-rw-rw-   0        0        0  2892800 2022-12-23 03:33:45.000000 pytessng-0.1.8/pytessng/libcrypto-1_1-x64.dll
+-rw-rw-rw-   0        0        0  2892800 2022-12-23 03:33:45.000000 pytessng-0.1.8/pytessng/libcrypto-1_1-x64_28.dll
+-rw-rw-rw-   0        0        0  3433984 2023-03-01 09:43:29.000000 pytessng-0.1.8/pytessng/libcrypto-1_1-x64_35.dll
+-rw-rw-rw-   0        0        0  2518016 2022-10-27 03:37:06.000000 pytessng-0.1.8/pytessng/libprotobuf.dll
+-rw-rw-rw-   0        0        0      716 2023-06-21 10:44:15.000000 pytessng-0.1.8/pytessng/main.py
+-rw-rw-rw-   0        0        0   455680 2023-05-11 02:52:50.000000 pytessng-0.1.8/pytessng/metis.dll
+-rw-rw-rw-   0        0        0      701 2023-04-23 03:05:58.000000 pytessng-0.1.8/pytessng/MyNet.py
+-rw-rw-rw-   0        0        0     1534 2023-06-21 10:47:15.000000 pytessng-0.1.8/pytessng/MyPlugin.py
+-rw-rw-rw-   0        0        0  3209216 2023-07-10 03:01:09.000000 pytessng-0.1.8/pytessng/TessCluster.dll
+-rw-rw-rw-   0        0        0   413696 2023-07-26 15:03:42.000000 pytessng-0.1.8/pytessng/TessInterfaces.dll
+-rw-rw-rw-   0        0        0  1446400 2023-07-27 01:41:04.000000 pytessng-0.1.8/pytessng/Tessng.pyd
+-rw-rw-rw-   0        0        0    72636 2023-06-27 07:08:31.000000 pytessng-0.1.8/pytessng/Tessng.pyi
+-rw-rw-rw-   0        0        0   155648 2023-07-26 15:03:34.000000 pytessng-0.1.8/pytessng/TessSupport.dll
+-rw-rw-rw-   0        0        0    13425 2023-07-31 10:16:30.000000 pytessng-0.1.8/pytessng/TESS_API_EXAMPLE.py
+-rw-rw-rw-   0        0        0  1320960 2023-07-26 15:04:34.000000 pytessng-0.1.8/pytessng/TESS_DB.dll
+-rw-rw-rw-   0        0        0  2080768 2023-07-26 15:04:48.000000 pytessng-0.1.8/pytessng/TESS_NET.dll
+-rw-rw-rw-   0        0        0  1082368 2023-07-27 01:32:58.000000 pytessng-0.1.8/pytessng/TESS_SIMU.dll
+-rw-rw-rw-   0        0        0  3245056 2023-07-26 15:06:36.000000 pytessng-0.1.8/pytessng/TESS_WIN.dll
+drwxrwxrwx   0        0        0        0 2023-08-01 01:24:32.000000 pytessng-0.1.8/pytessng/utils/
+-rw-rw-rw-   0        0        0    24535 2023-07-31 03:25:54.000000 pytessng-0.1.8/pytessng/utils/functions.py
+-rw-rw-rw-   0        0        0        0 2023-03-13 03:59:50.000000 pytessng-0.1.8/pytessng/utils/__init__.py
+-rw-rw-rw-   0        0        0      194 2023-03-13 03:59:50.000000 pytessng-0.1.8/pytessng/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:24:32.000000 pytessng-0.1.8/pytessng.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-08-01 01:24:32.000000 pytessng-0.1.8/pytessng.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      496 2023-08-01 01:24:32.000000 pytessng-0.1.8/pytessng.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       55 2023-08-01 01:24:32.000000 pytessng-0.1.8/pytessng.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      737 2023-08-01 01:24:32.000000 pytessng-0.1.8/pytessng.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        9 2023-08-01 01:24:32.000000 pytessng-0.1.8/pytessng.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       54 2022-10-20 06:33:19.000000 pytessng-0.1.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-01 01:24:32.000000 pytessng-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      847 2023-08-01 01:24:09.000000 pytessng-0.1.8/setup.py
```

### Comparing `pytessng-0.1.7/LICENSE` & `pytessng-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pytessng-0.1.7/pytessng/DockWidget.py` & `pytessng-0.1.8/pytessng/DockWidget.py`

 * *Files identical despite different names*

### Comparing `pytessng-0.1.7/pytessng/GKlib.dll` & `pytessng-0.1.8/pytessng/GKlib.dll`

 * *Files identical despite different names*

### Comparing `pytessng-0.1.7/pytessng/libcrypto-1_1-x64.dll` & `pytessng-0.1.8/pytessng/libcrypto-1_1-x64.dll`

 * *Files identical despite different names*

### Comparing `pytessng-0.1.7/pytessng/libcrypto-1_1-x64_28.dll` & `pytessng-0.1.8/pytessng/libcrypto-1_1-x64_28.dll`

 * *Files identical despite different names*

### Comparing `pytessng-0.1.7/pytessng/libcrypto-1_1-x64_35.dll` & `pytessng-0.1.8/pytessng/libcrypto-1_1-x64_35.dll`

 * *Files identical despite different names*

### Comparing `pytessng-0.1.7/pytessng/libprotobuf.dll` & `pytessng-0.1.8/pytessng/libprotobuf.dll`

 * *Files identical despite different names*

### Comparing `pytessng-0.1.7/pytessng/main.py` & `pytessng-0.1.8/pytessng/main.py`

 * *Files identical despite different names*

### Comparing `pytessng-0.1.7/pytessng/metis.dll` & `pytessng-0.1.8/pytessng/metis.dll`

 * *Files identical despite different names*

### Comparing `pytessng-0.1.7/pytessng/MyNet.py` & `pytessng-0.1.8/pytessng/MyNet.py`

 * *Files identical despite different names*

### Comparing `pytessng-0.1.7/pytessng/MyPlugin.py` & `pytessng-0.1.8/pytessng/MyPlugin.py`

 * *Files identical despite different names*

### Comparing `pytessng-0.1.7/pytessng/TessCluster.dll` & `pytessng-0.1.8/pytessng/TessCluster.dll`

 * *Files identical despite different names*

### Comparing `pytessng-0.1.7/pytessng/TessInterfaces.dll` & `pytessng-0.1.8/pytessng/TessInterfaces.dll`

 * *Files identical despite different names*

### Comparing `pytessng-0.1.7/pytessng/Tessng.pyi` & `pytessng-0.1.8/pytessng/Tessng.pyi`

 * *Files identical despite different names*

### Comparing `pytessng-0.1.7/pytessng/TessSupport.dll` & `pytessng-0.1.8/pytessng/TessSupport.dll`

 * *Files identical despite different names*

### Comparing `pytessng-0.1.7/pytessng/TESS_API_EXAMPLE.py` & `pytessng-0.1.8/pytessng/TESS_API_EXAMPLE.py`

 * *Files identical despite different names*

### Comparing `pytessng-0.1.7/pytessng/TESS_DB.dll` & `pytessng-0.1.8/pytessng/TESS_DB.dll`

 * *Files identical despite different names*

### Comparing `pytessng-0.1.7/pytessng/TESS_NET.dll` & `pytessng-0.1.8/pytessng/TESS_NET.dll`

 * *Files identical despite different names*

### Comparing `pytessng-0.1.7/pytessng/TESS_SIMU.dll` & `pytessng-0.1.8/pytessng/TESS_SIMU.dll`

 * *Files identical despite different names*

### Comparing `pytessng-0.1.7/pytessng/TESS_WIN.dll` & `pytessng-0.1.8/pytessng/TESS_WIN.dll`

 * *Files identical despite different names*

### Comparing `pytessng-0.1.7/pytessng/utils/functions.py` & `pytessng-0.1.8/pytessng/utils/functions.py`

 * *Files identical despite different names*

### Comparing `pytessng-0.1.7/pytessng.egg-info/SOURCES.txt` & `pytessng-0.1.8/pytessng.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytessng-0.1.7/setup.py` & `pytessng-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pytessng",
-    version="0.1.7",
+    version="0.1.8",
     author="yang",
     author_email="17315487709@163.com",
     description="tessng with python3.6",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     install_requires=[
-        'opendrive2tessng==0.1.5',
+        'opendrive2tessng==0.1.6',
         'tessng2other',
         'PySide2==5.15.2.1',
     ],
     python_requires='>=3.6, <3.8',
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
```

