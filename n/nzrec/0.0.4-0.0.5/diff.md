# Comparing `tmp/nzrec-0.0.4.tar.gz` & `tmp/nzrec-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nzrec-0.0.4.tar", last modified: Wed Jan 18 07:48:23 2023, max compression
+gzip compressed data, was "nzrec-0.0.5.tar", last modified: Tue Aug  1 21:56:31 2023, max compression
```

## Comparing `nzrec-0.0.4.tar` & `nzrec-0.0.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-01-18 07:48:23.320602 nzrec-0.0.4/
--rw-rw-r--   0 mike      (1000) mike      (1000)    11357 2022-11-29 06:51:00.000000 nzrec-0.0.4/LICENSE
--rw-rw-r--   0 mike      (1000) mike      (1000)      551 2023-01-18 07:48:23.320602 nzrec-0.0.4/PKG-INFO
--rw-rw-r--   0 mike      (1000) mike      (1000)      191 2022-11-29 06:53:40.000000 nzrec-0.0.4/README.rst
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-01-18 07:48:23.320602 nzrec-0.0.4/nzrec/
--rw-rw-r--   0 mike      (1000) mike      (1000)       38 2023-01-17 21:29:21.000000 nzrec-0.0.4/nzrec/__init__.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-01-18 07:48:23.320602 nzrec-0.0.4/nzrec/datasets/
--rw-rw-r--   0 mike      (1000) mike      (1000)      906 2022-11-29 06:52:17.000000 nzrec-0.0.4/nzrec/datasets/__init__.py
--rw-rw-r--   0 mike      (1000) mike      (1000)    10238 2023-01-18 07:46:56.000000 nzrec-0.0.4/nzrec/main.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     6078 2023-01-15 04:04:45.000000 nzrec-0.0.4/nzrec/rec_cleaning.py
--rw-rw-r--   0 mike      (1000) mike      (1000)    11907 2023-01-17 00:59:37.000000 nzrec-0.0.4/nzrec/shp_to_blt.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-01-18 07:48:23.320602 nzrec-0.0.4/nzrec/tests/
--rw-rw-r--   0 mike      (1000) mike      (1000)      208 2022-11-29 06:52:17.000000 nzrec-0.0.4/nzrec/tests/__init__.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     1476 2022-11-29 06:52:17.000000 nzrec-0.0.4/nzrec/tests/create_test_data.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     5563 2022-11-29 06:52:17.000000 nzrec-0.0.4/nzrec/tests/test_hdf5tools.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     8156 2023-01-18 07:45:45.000000 nzrec-0.0.4/nzrec/utils.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-01-18 07:48:23.320602 nzrec-0.0.4/nzrec.egg-info/
--rw-rw-r--   0 mike      (1000) mike      (1000)      551 2023-01-18 07:48:23.000000 nzrec-0.0.4/nzrec.egg-info/PKG-INFO
--rw-rw-r--   0 mike      (1000) mike      (1000)      398 2023-01-18 07:48:23.000000 nzrec-0.0.4/nzrec.egg-info/SOURCES.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)        1 2023-01-18 07:48:23.000000 nzrec-0.0.4/nzrec.egg-info/dependency_links.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)       59 2023-01-18 07:48:23.000000 nzrec-0.0.4/nzrec.egg-info/requires.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)        6 2023-01-18 07:48:23.000000 nzrec-0.0.4/nzrec.egg-info/top_level.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)      104 2022-11-29 06:52:17.000000 nzrec-0.0.4/pyproject.toml
--rw-rw-r--   0 mike      (1000) mike      (1000)       67 2023-01-18 07:48:23.320602 nzrec-0.0.4/setup.cfg
--rw-rw-r--   0 mike      (1000) mike      (1000)     7262 2023-01-18 07:48:06.000000 nzrec-0.0.4/setup.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-08-01 21:56:31.668190 nzrec-0.0.5/
+-rw-rw-r--   0 mike      (1000) mike      (1000)    11357 2023-07-11 01:17:04.000000 nzrec-0.0.5/LICENSE
+-rw-rw-r--   0 mike      (1000) mike      (1000)      551 2023-08-01 21:56:31.668190 nzrec-0.0.5/PKG-INFO
+-rw-rw-r--   0 mike      (1000) mike      (1000)      191 2023-07-11 01:17:04.000000 nzrec-0.0.5/README.rst
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-08-01 21:56:31.664190 nzrec-0.0.5/nzrec/
+-rw-rw-r--   0 mike      (1000) mike      (1000)       38 2023-07-11 01:17:04.000000 nzrec-0.0.5/nzrec/__init__.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-08-01 21:56:31.668190 nzrec-0.0.5/nzrec/datasets/
+-rw-rw-r--   0 mike      (1000) mike      (1000)      906 2023-07-11 01:17:04.000000 nzrec-0.0.5/nzrec/datasets/__init__.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)    10084 2023-08-01 21:55:22.000000 nzrec-0.0.5/nzrec/main.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     6078 2023-07-11 01:17:04.000000 nzrec-0.0.5/nzrec/rec_cleaning.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)    11907 2023-07-11 01:17:04.000000 nzrec-0.0.5/nzrec/shp_to_blt.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-08-01 21:56:31.668190 nzrec-0.0.5/nzrec/tests/
+-rw-rw-r--   0 mike      (1000) mike      (1000)      208 2023-07-11 01:17:04.000000 nzrec-0.0.5/nzrec/tests/__init__.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     1476 2023-07-11 01:17:04.000000 nzrec-0.0.5/nzrec/tests/create_test_data.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     5563 2023-07-11 01:17:04.000000 nzrec-0.0.5/nzrec/tests/test_hdf5tools.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     8206 2023-08-01 20:09:48.000000 nzrec-0.0.5/nzrec/utils.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-08-01 21:56:31.668190 nzrec-0.0.5/nzrec.egg-info/
+-rw-rw-r--   0 mike      (1000) mike      (1000)      551 2023-08-01 21:56:31.000000 nzrec-0.0.5/nzrec.egg-info/PKG-INFO
+-rw-rw-r--   0 mike      (1000) mike      (1000)      398 2023-08-01 21:56:31.000000 nzrec-0.0.5/nzrec.egg-info/SOURCES.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)        1 2023-08-01 21:56:31.000000 nzrec-0.0.5/nzrec.egg-info/dependency_links.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)       59 2023-08-01 21:56:31.000000 nzrec-0.0.5/nzrec.egg-info/requires.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)        6 2023-08-01 21:56:31.000000 nzrec-0.0.5/nzrec.egg-info/top_level.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)      104 2023-07-11 01:17:04.000000 nzrec-0.0.5/pyproject.toml
+-rw-rw-r--   0 mike      (1000) mike      (1000)       67 2023-08-01 21:56:31.668190 nzrec-0.0.5/setup.cfg
+-rw-rw-r--   0 mike      (1000) mike      (1000)     7262 2023-08-01 21:55:43.000000 nzrec-0.0.5/setup.py
```

### Comparing `nzrec-0.0.4/LICENSE` & `nzrec-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nzrec-0.0.4/PKG-INFO` & `nzrec-0.0.5/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nzrec
-Version: 0.0.4
+Version: 0.0.5
 Summary: NZ REC delineation tool
 Home-page: https://github.com/mullenkamp/nzrec
 Author: Mike Kittridge
 Author-email: mullenkamp1@gmail.com
 License: Apache
 Keywords: rivers
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `nzrec-0.0.4/nzrec/datasets/__init__.py` & `nzrec-0.0.5/nzrec/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `nzrec-0.0.4/nzrec/main.py` & `nzrec-0.0.5/nzrec/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import shapely
 import geopandas as gpd
 from scipy.spatial import KDTree
 import zstandard as zstd
 import orjson
 import pathlib
 import booklet
+from copy import copy
 
 # import utils
 from . import utils
 
 #####################################################
 ### Parameters
 
@@ -353,36 +354,32 @@
 
 
 
 #####################################################
 ### Combo functions
 
 
-
 def between(objs):
     """
 
     """
     ## Checks
     bool_way = all([isinstance(obj, Way) for obj in objs])
     bool_catch = all([isinstance(obj, Catchment) for obj in objs])
 
     new_list = []
     if bool_way or bool_catch:
 
         for obj in objs:
-            diff_options = {len(obj.ways.difference(o.ways)): i for i, o in enumerate(objs) if obj.id != o.id}
-            min_diff_len = min(diff_options)
-            if min_diff_len > 0:
-                next_up_way_pos = diff_options[min_diff_len]
-                diff_ways = obj.ways.difference(objs[next_up_way_pos].ways)
-                new_way_obj = Way(obj._water)
+            new_way_obj = copy(obj)
+            subsets = [o for o in objs if new_way_obj.ways.issuperset(o.ways) and (new_way_obj.id != o.id)]
+
+            for subset in subsets:
+                diff_ways = new_way_obj.ways.difference(subset.ways)
                 new_way_obj.ways = diff_ways
-            else:
-                new_way_obj = obj
 
             if bool_catch:
                 new_list.append(new_way_obj.catchments())
             else:
                 new_list.append(new_way_obj)
     else:
         raise TypeError('Input objs must be all either Way or Cathcment objects.')
```

### Comparing `nzrec-0.0.4/nzrec/rec_cleaning.py` & `nzrec-0.0.5/nzrec/rec_cleaning.py`

 * *Files identical despite different names*

### Comparing `nzrec-0.0.4/nzrec/shp_to_blt.py` & `nzrec-0.0.5/nzrec/shp_to_blt.py`

 * *Files identical despite different names*

### Comparing `nzrec-0.0.4/nzrec/tests/create_test_data.py` & `nzrec-0.0.5/nzrec/tests/create_test_data.py`

 * *Files identical despite different names*

### Comparing `nzrec-0.0.4/nzrec/tests/test_hdf5tools.py` & `nzrec-0.0.5/nzrec/tests/test_hdf5tools.py`

 * *Files identical despite different names*

### Comparing `nzrec-0.0.4/nzrec/utils.py` & `nzrec-0.0.5/nzrec/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,14 +126,17 @@
 
     for way_id in base_ways0:
         nodes = way[int(way_id)]
         if node_id != nodes[-1]:
             way_down = way_id
             break
 
+    if way_down == -1:
+        way_down = way_id
+
     return way_down
 
 
 def make_kdtree(coords):
     """
 
     """
```

### Comparing `nzrec-0.0.4/nzrec.egg-info/PKG-INFO` & `nzrec-0.0.5/nzrec.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nzrec
-Version: 0.0.4
+Version: 0.0.5
 Summary: NZ REC delineation tool
 Home-page: https://github.com/mullenkamp/nzrec
 Author: Mike Kittridge
 Author-email: mullenkamp1@gmail.com
 License: Apache
 Keywords: rivers
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `nzrec-0.0.4/setup.py` & `nzrec-0.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 # General parameters
 name = 'nzrec'
 main_package = 'nzrec'
 # datasets = 'datasets'
-version = '0.0.4'
+version = '0.0.5'
 descrip = 'NZ REC delineation tool'
 
 # The below code is for readthedocs. To have sphinx/readthedocs interact with
 # the contained package, readthedocs needs to build the package. But the dependencies
 # should be installed via the conda yml env file rather than during the package build.
 if os.environ.get('READTHEDOCS', False) == 'True':
     INSTALL_REQUIRES = []
```

