# Comparing `tmp/earthml-0.2.tar.gz` & `tmp/earthml-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "earthml-0.2.tar", last modified: Tue Aug  1 19:07:53 2023, max compression
+gzip compressed data, was "earthml-0.3.tar", last modified: Tue Aug  1 19:45:55 2023, max compression
```

## Comparing `earthml-0.2.tar` & `earthml-0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 akhilchhibber   (501) staff       (20)        0 2023-08-01 19:07:53.237385 earthml-0.2/
--rw-r--r--   0 akhilchhibber   (501) staff       (20)     1070 2023-08-01 18:41:39.000000 earthml-0.2/LICENSE
--rw-r--r--   0 akhilchhibber   (501) staff       (20)     2135 2023-08-01 19:07:53.237259 earthml-0.2/PKG-INFO
--rw-r--r--   0 akhilchhibber   (501) staff       (20)     1496 2023-08-01 18:50:13.000000 earthml-0.2/README.md
-drwxr-xr-x   0 akhilchhibber   (501) staff       (20)        0 2023-08-01 19:07:53.236411 earthml-0.2/earthml/
--rw-r--r--   0 akhilchhibber   (501) staff       (20)       33 2023-08-01 18:30:59.000000 earthml-0.2/earthml/__init__.py
--rw-r--r--   0 akhilchhibber   (501) staff       (20)    13831 2023-08-01 18:57:08.000000 earthml-0.2/earthml/geodata_to_geohash.py
-drwxr-xr-x   0 akhilchhibber   (501) staff       (20)        0 2023-08-01 19:07:53.237084 earthml-0.2/earthml.egg-info/
--rw-r--r--   0 akhilchhibber   (501) staff       (20)     2135 2023-08-01 19:07:53.000000 earthml-0.2/earthml.egg-info/PKG-INFO
--rw-r--r--   0 akhilchhibber   (501) staff       (20)      230 2023-08-01 19:07:53.000000 earthml-0.2/earthml.egg-info/SOURCES.txt
--rw-r--r--   0 akhilchhibber   (501) staff       (20)        1 2023-08-01 19:07:53.000000 earthml-0.2/earthml.egg-info/dependency_links.txt
--rw-r--r--   0 akhilchhibber   (501) staff       (20)       38 2023-08-01 19:07:53.000000 earthml-0.2/earthml.egg-info/requires.txt
--rw-r--r--   0 akhilchhibber   (501) staff       (20)        8 2023-08-01 19:07:53.000000 earthml-0.2/earthml.egg-info/top_level.txt
--rw-r--r--   0 akhilchhibber   (501) staff       (20)       38 2023-08-01 19:07:53.237424 earthml-0.2/setup.cfg
--rw-r--r--   0 akhilchhibber   (501) staff       (20)     1030 2023-08-01 19:07:38.000000 earthml-0.2/setup.py
+drwxr-xr-x   0 akhilchhibber   (501) staff       (20)        0 2023-08-01 19:45:55.147952 earthml-0.3/
+-rw-r--r--   0 akhilchhibber   (501) staff       (20)     1070 2023-08-01 18:41:39.000000 earthml-0.3/LICENSE
+-rw-r--r--   0 akhilchhibber   (501) staff       (20)     2019 2023-08-01 19:45:55.147839 earthml-0.3/PKG-INFO
+-rw-r--r--   0 akhilchhibber   (501) staff       (20)     1379 2023-08-01 19:45:18.000000 earthml-0.3/README.md
+drwxr-xr-x   0 akhilchhibber   (501) staff       (20)        0 2023-08-01 19:45:55.147008 earthml-0.3/earthml/
+-rw-r--r--   0 akhilchhibber   (501) staff       (20)       33 2023-08-01 18:30:59.000000 earthml-0.3/earthml/__init__.py
+-rw-r--r--   0 akhilchhibber   (501) staff       (20)    13831 2023-08-01 18:57:08.000000 earthml-0.3/earthml/geodata_to_geohash.py
+drwxr-xr-x   0 akhilchhibber   (501) staff       (20)        0 2023-08-01 19:45:55.147678 earthml-0.3/earthml.egg-info/
+-rw-r--r--   0 akhilchhibber   (501) staff       (20)     2019 2023-08-01 19:45:55.000000 earthml-0.3/earthml.egg-info/PKG-INFO
+-rw-r--r--   0 akhilchhibber   (501) staff       (20)      230 2023-08-01 19:45:55.000000 earthml-0.3/earthml.egg-info/SOURCES.txt
+-rw-r--r--   0 akhilchhibber   (501) staff       (20)        1 2023-08-01 19:45:55.000000 earthml-0.3/earthml.egg-info/dependency_links.txt
+-rw-r--r--   0 akhilchhibber   (501) staff       (20)       38 2023-08-01 19:45:55.000000 earthml-0.3/earthml.egg-info/requires.txt
+-rw-r--r--   0 akhilchhibber   (501) staff       (20)        8 2023-08-01 19:45:55.000000 earthml-0.3/earthml.egg-info/top_level.txt
+-rw-r--r--   0 akhilchhibber   (501) staff       (20)       38 2023-08-01 19:45:55.147990 earthml-0.3/setup.cfg
+-rw-r--r--   0 akhilchhibber   (501) staff       (20)     1030 2023-08-01 19:45:18.000000 earthml-0.3/setup.py
```

### Comparing `earthml-0.2/LICENSE` & `earthml-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `earthml-0.2/PKG-INFO` & `earthml-0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: earthml
-Version: 0.2
+Version: 0.3
 Summary: A library to Perform different possible operations on Geo-Spatial Dataset
 Home-page: https://github.com/akhilchibber
 Author: Akhil Chhibber
 Author-email: akhil.chibber@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: GIS
@@ -67,10 +67,7 @@
 
 
 
 
 
 # Note
 This README provides a brief overview of the library, explains its goal, highlights key features, and provides simple installation and usage instructions.
-
-Would you like me to make any modifications or provide additional details? Let me know how you'd like to proceed!
-
```

### Comparing `earthml-0.2/README.md` & `earthml-0.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -49,11 +49,8 @@
 
 
 
 
 
 
 # Note
-This README provides a brief overview of the library, explains its goal, highlights key features, and provides simple installation and usage instructions.
-
-Would you like me to make any modifications or provide additional details? Let me know how you'd like to proceed!
-
+This README provides a brief overview of the library, explains its goal, highlights key features, and provides simple installation and usage instructions.
```

### Comparing `earthml-0.2/earthml/geodata_to_geohash.py` & `earthml-0.3/earthml/geodata_to_geohash.py`

 * *Files identical despite different names*

### Comparing `earthml-0.2/earthml.egg-info/PKG-INFO` & `earthml-0.3/earthml.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: earthml
-Version: 0.2
+Version: 0.3
 Summary: A library to Perform different possible operations on Geo-Spatial Dataset
 Home-page: https://github.com/akhilchibber
 Author: Akhil Chhibber
 Author-email: akhil.chibber@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: GIS
@@ -67,10 +67,7 @@
 
 
 
 
 
 # Note
 This README provides a brief overview of the library, explains its goal, highlights key features, and provides simple installation and usage instructions.
-
-Would you like me to make any modifications or provide additional details? Let me know how you'd like to proceed!
-
```

### Comparing `earthml-0.2/setup.py` & `earthml-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the content of the README.md file
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='earthml',
-    version='0.2',
+    version='0.3',
     packages=find_packages(),
     install_requires=[
         'fiona',
         'rasterio',
         'pygeohash',
         'Pillow',
         'laspy',
```

