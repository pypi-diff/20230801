# Comparing `tmp/deafrica_tools-2.0.1.tar.gz` & `tmp/deafrica_tools-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deafrica_tools-2.0.1.tar", max compression
+gzip compressed data, was "deafrica_tools-2.0.2.tar", max compression
```

## Comparing `deafrica_tools-2.0.1.tar` & `deafrica_tools-2.0.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0    11357 2023-06-27 16:22:39.741268 deafrica_tools-2.0.1/LICENSE
--rw-r--r--   0        0        0     3097 2023-06-27 16:22:39.741268 deafrica_tools-2.0.1/README.md
--rw-r--r--   0        0        0      676 2023-06-27 16:22:39.741268 deafrica_tools-2.0.1/deafrica_tools/__init__.py
--rw-r--r--   0        0        0       22 2023-06-27 16:22:39.741268 deafrica_tools-2.0.1/deafrica_tools/app/__init__.py
--rw-r--r--   0        0        0    31449 2023-06-27 16:22:39.741268 deafrica_tools-2.0.1/deafrica_tools/app/animations.py
--rw-r--r--   0        0        0    10984 2023-06-27 16:22:39.745268 deafrica_tools-2.0.1/deafrica_tools/app/changefilmstrips.py
--rw-r--r--   0        0        0    10494 2023-06-27 16:22:39.745268 deafrica_tools-2.0.1/deafrica_tools/app/crophealth.py
--rw-r--r--   0        0        0    20287 2023-06-27 16:22:39.745268 deafrica_tools-2.0.1/deafrica_tools/app/deacoastlines.py
--rw-r--r--   0        0        0    37843 2023-06-27 16:22:39.745268 deafrica_tools-2.0.1/deafrica_tools/app/forestmonitoring.py
--rw-r--r--   0        0        0     8673 2023-06-27 16:22:39.745268 deafrica_tools-2.0.1/deafrica_tools/app/geomedian.py
--rw-r--r--   0        0        0    13383 2023-06-27 16:22:39.745268 deafrica_tools-2.0.1/deafrica_tools/app/imageexport.py
--rw-r--r--   0        0        0    13148 2023-06-27 16:22:39.745268 deafrica_tools-2.0.1/deafrica_tools/app/wetlandsinsighttool.py
--rw-r--r--   0        0        0     9882 2023-06-27 16:22:39.745268 deafrica_tools-2.0.1/deafrica_tools/app/widgetconstructors.py
--rw-r--r--   0        0        0     2043 2023-06-27 16:22:39.745268 deafrica_tools-2.0.1/deafrica_tools/areaofinterest.py
--rw-r--r--   0        0        0    24548 2023-06-27 16:22:39.745268 deafrica_tools-2.0.1/deafrica_tools/bandindices.py
--rw-r--r--   0        0        0    61473 2023-06-27 16:22:39.745268 deafrica_tools-2.0.1/deafrica_tools/classification.py
--rw-r--r--   0        0        0    23515 2023-06-27 16:22:39.745268 deafrica_tools-2.0.1/deafrica_tools/coastal.py
--rw-r--r--   0        0        0     3404 2023-06-27 16:22:39.745268 deafrica_tools-2.0.1/deafrica_tools/dask.py
--rw-r--r--   0        0        0    35752 2023-06-27 16:22:39.745268 deafrica_tools-2.0.1/deafrica_tools/datahandling.py
--rw-r--r--   0        0        0    14369 2023-06-27 16:22:39.745268 deafrica_tools-2.0.1/deafrica_tools/load_era5.py
--rw-r--r--   0        0        0     2793 2023-06-27 16:22:39.745268 deafrica_tools-2.0.1/deafrica_tools/load_isda.py
--rw-r--r--   0        0        0     2027 2023-06-27 16:22:39.745268 deafrica_tools-2.0.1/deafrica_tools/load_soil_moisture.py
--rw-r--r--   0        0        0     1783 2023-06-27 16:22:39.745268 deafrica_tools-2.0.1/deafrica_tools/locales/fr/LC_MESSAGES/deafrica_tools.mo
--rw-r--r--   0        0        0     3315 2023-06-27 16:22:39.745268 deafrica_tools-2.0.1/deafrica_tools/locales/fr/LC_MESSAGES/deafrica_tools.po
--rw-r--r--   0        0        0    50697 2023-06-27 16:22:39.745268 deafrica_tools-2.0.1/deafrica_tools/plotting.py
--rw-r--r--   0        0        0    36957 2023-06-27 16:22:39.749268 deafrica_tools-2.0.1/deafrica_tools/spatial.py
--rw-r--r--   0        0        0    17245 2023-06-27 16:22:39.749268 deafrica_tools-2.0.1/deafrica_tools/temporal.py
--rw-r--r--   0        0        0    25961 2023-06-27 16:22:39.749268 deafrica_tools-2.0.1/deafrica_tools/wetlands.py
--rw-r--r--   0        0        0     3310 2023-06-27 16:22:39.749268 deafrica_tools-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     5577 1970-01-01 00:00:00.000000 deafrica_tools-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-08-01 10:39:16.195908 deafrica_tools-2.0.2/LICENSE
+-rw-r--r--   0        0        0     3097 2023-08-01 10:39:16.195908 deafrica_tools-2.0.2/README.md
+-rw-r--r--   0        0        0      676 2023-08-01 10:39:16.195908 deafrica_tools-2.0.2/deafrica_tools/__init__.py
+-rw-r--r--   0        0        0       22 2023-08-01 10:39:16.195908 deafrica_tools-2.0.2/deafrica_tools/app/__init__.py
+-rw-r--r--   0        0        0    31449 2023-08-01 10:39:16.195908 deafrica_tools-2.0.2/deafrica_tools/app/animations.py
+-rw-r--r--   0        0        0    10984 2023-08-01 10:39:16.195908 deafrica_tools-2.0.2/deafrica_tools/app/changefilmstrips.py
+-rw-r--r--   0        0        0    10494 2023-08-01 10:39:16.195908 deafrica_tools-2.0.2/deafrica_tools/app/crophealth.py
+-rw-r--r--   0        0        0    20287 2023-08-01 10:39:16.195908 deafrica_tools-2.0.2/deafrica_tools/app/deacoastlines.py
+-rw-r--r--   0        0        0    37843 2023-08-01 10:39:16.195908 deafrica_tools-2.0.2/deafrica_tools/app/forestmonitoring.py
+-rw-r--r--   0        0        0     8673 2023-08-01 10:39:16.195908 deafrica_tools-2.0.2/deafrica_tools/app/geomedian.py
+-rw-r--r--   0        0        0    13383 2023-08-01 10:39:16.195908 deafrica_tools-2.0.2/deafrica_tools/app/imageexport.py
+-rw-r--r--   0        0        0    13148 2023-08-01 10:39:16.195908 deafrica_tools-2.0.2/deafrica_tools/app/wetlandsinsighttool.py
+-rw-r--r--   0        0        0     9882 2023-08-01 10:39:16.195908 deafrica_tools-2.0.2/deafrica_tools/app/widgetconstructors.py
+-rw-r--r--   0        0        0     2016 2023-08-01 10:39:16.195908 deafrica_tools-2.0.2/deafrica_tools/areaofinterest.py
+-rw-r--r--   0        0        0    24548 2023-08-01 10:39:16.195908 deafrica_tools-2.0.2/deafrica_tools/bandindices.py
+-rw-r--r--   0        0        0    61473 2023-08-01 10:39:16.195908 deafrica_tools-2.0.2/deafrica_tools/classification.py
+-rw-r--r--   0        0        0    23515 2023-08-01 10:39:16.195908 deafrica_tools-2.0.2/deafrica_tools/coastal.py
+-rw-r--r--   0        0        0     3404 2023-08-01 10:39:16.195908 deafrica_tools-2.0.2/deafrica_tools/dask.py
+-rw-r--r--   0        0        0    35752 2023-08-01 10:39:16.195908 deafrica_tools-2.0.2/deafrica_tools/datahandling.py
+-rw-r--r--   0        0        0    14369 2023-08-01 10:39:16.195908 deafrica_tools-2.0.2/deafrica_tools/load_era5.py
+-rw-r--r--   0        0        0     2793 2023-08-01 10:39:16.195908 deafrica_tools-2.0.2/deafrica_tools/load_isda.py
+-rw-r--r--   0        0        0     2027 2023-08-01 10:39:16.195908 deafrica_tools-2.0.2/deafrica_tools/load_soil_moisture.py
+-rw-r--r--   0        0        0     1783 2023-08-01 10:39:16.195908 deafrica_tools-2.0.2/deafrica_tools/locales/fr/LC_MESSAGES/deafrica_tools.mo
+-rw-r--r--   0        0        0     3315 2023-08-01 10:39:16.195908 deafrica_tools-2.0.2/deafrica_tools/locales/fr/LC_MESSAGES/deafrica_tools.po
+-rw-r--r--   0        0        0    50697 2023-08-01 10:39:16.195908 deafrica_tools-2.0.2/deafrica_tools/plotting.py
+-rw-r--r--   0        0        0    36957 2023-08-01 10:39:16.195908 deafrica_tools-2.0.2/deafrica_tools/spatial.py
+-rw-r--r--   0        0        0    17245 2023-08-01 10:39:16.195908 deafrica_tools-2.0.2/deafrica_tools/temporal.py
+-rw-r--r--   0        0        0    25961 2023-08-01 10:39:16.195908 deafrica_tools-2.0.2/deafrica_tools/wetlands.py
+-rw-r--r--   0        0        0     3310 2023-08-01 10:39:16.199908 deafrica_tools-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5577 1970-01-01 00:00:00.000000 deafrica_tools-2.0.2/PKG-INFO
```

### Comparing `deafrica_tools-2.0.1/LICENSE` & `deafrica_tools-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.1/README.md` & `deafrica_tools-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.1/deafrica_tools/__init__.py` & `deafrica_tools-2.0.2/deafrica_tools/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "2.0.1"
+__version__ = "2.0.2"
 
 __locales__ = __path__[0] + '/locales'
 
 
 def set_lang(lang=None):
     if lang is None:
         import os
```

### Comparing `deafrica_tools-2.0.1/deafrica_tools/app/animations.py` & `deafrica_tools-2.0.2/deafrica_tools/app/animations.py`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.1/deafrica_tools/app/changefilmstrips.py` & `deafrica_tools-2.0.2/deafrica_tools/app/changefilmstrips.py`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.1/deafrica_tools/app/crophealth.py` & `deafrica_tools-2.0.2/deafrica_tools/app/crophealth.py`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.1/deafrica_tools/app/deacoastlines.py` & `deafrica_tools-2.0.2/deafrica_tools/app/deacoastlines.py`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.1/deafrica_tools/app/forestmonitoring.py` & `deafrica_tools-2.0.2/deafrica_tools/app/forestmonitoring.py`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.1/deafrica_tools/app/geomedian.py` & `deafrica_tools-2.0.2/deafrica_tools/app/geomedian.py`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.1/deafrica_tools/app/imageexport.py` & `deafrica_tools-2.0.2/deafrica_tools/app/imageexport.py`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.1/deafrica_tools/app/wetlandsinsighttool.py` & `deafrica_tools-2.0.2/deafrica_tools/app/wetlandsinsighttool.py`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.1/deafrica_tools/app/widgetconstructors.py` & `deafrica_tools-2.0.2/deafrica_tools/app/widgetconstructors.py`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.1/deafrica_tools/areaofinterest.py` & `deafrica_tools-2.0.2/deafrica_tools/areaofinterest.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 """
-Function for defining an area of interest using either a point and buffer or a shapefile file. 
+Function for defining an area of interest using either a point and buffer or a vector file. 
 """
 
 # Import required packages
 
 # Force GeoPandas to use Shapely instead of PyGEOS
 # In a future release, GeoPandas will switch to using Shapely by default.
 import os
 os.environ['USE_PYGEOS'] = '0'
 
 import geopandas as gpd
 from shapely.geometry import box
 from geojson import Feature, Point, FeatureCollection
 
-def define_area(lat=None, lon=None, buffer=None, shapefile_path=None):
+def define_area(lat=None, lon=None, buffer=None, vector_path=None):
     '''
-    Define an area of interest using either a point and buffer or a shapefile.
+    Define an area of interest using either a point and buffer or a vector.
     
     Parameters:
     -----------
     lat : float, optional
         The latitude of the center point of the area of interest.
     lon : float, optional
         The longitude of the center point of the area of interest.
     buffer : float, optional
         The buffer around the center point, in degrees.
-    shapefile_path : str, optional
-        The path to a shapefile defining the area of interest.
+    vector_path : str, optional
+        The path to a vector defining the area of interest.
     
     Returns:
     --------
     feature_collection : dict
         A GeoJSON feature collection representing the area of interest.
     '''
     # Define area using point and buffer
     if lat is not None and lon is not None and buffer is not None:
         lat_range = (lat - buffer, lat + buffer)
         lon_range = (lon - buffer, lon + buffer)
         box_geom = box(min(lon_range), min(lat_range), max(lon_range), max(lat_range))
         aoi = gpd.GeoDataFrame(geometry=[box_geom], crs='EPSG:4326')
     
-    # Define area using shapefile
-    elif shapefile_path is not None:
-        aoi = gpd.read_file(shapefile_path).to_crs("EPSG:4326")
+    # Define area using vector
+    elif vector_path is not None:
+        aoi = gpd.read_file(vector_path).to_crs("EPSG:4326")
     # If neither option is provided, raise an error
     else:
-        raise ValueError("Either lat/lon/buffer or shapefile_path must be provided.")
+        raise ValueError("Either lat/lon/buffer or vector_path must be provided.")
     
     # Convert the GeoDataFrame to a GeoJSON FeatureCollection
     features = [Feature(geometry=row["geometry"], properties=row.drop("geometry").to_dict()) for _, row in aoi.iterrows()]
     feature_collection = FeatureCollection(features)
     
     return feature_collection
```

### Comparing `deafrica_tools-2.0.1/deafrica_tools/bandindices.py` & `deafrica_tools-2.0.2/deafrica_tools/bandindices.py`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.1/deafrica_tools/classification.py` & `deafrica_tools-2.0.2/deafrica_tools/classification.py`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.1/deafrica_tools/coastal.py` & `deafrica_tools-2.0.2/deafrica_tools/coastal.py`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.1/deafrica_tools/dask.py` & `deafrica_tools-2.0.2/deafrica_tools/dask.py`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.1/deafrica_tools/datahandling.py` & `deafrica_tools-2.0.2/deafrica_tools/datahandling.py`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.1/deafrica_tools/load_era5.py` & `deafrica_tools-2.0.2/deafrica_tools/load_era5.py`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.1/deafrica_tools/load_isda.py` & `deafrica_tools-2.0.2/deafrica_tools/load_isda.py`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.1/deafrica_tools/load_soil_moisture.py` & `deafrica_tools-2.0.2/deafrica_tools/load_soil_moisture.py`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.1/deafrica_tools/locales/fr/LC_MESSAGES/deafrica_tools.mo` & `deafrica_tools-2.0.2/deafrica_tools/locales/fr/LC_MESSAGES/deafrica_tools.mo`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.1/deafrica_tools/locales/fr/LC_MESSAGES/deafrica_tools.po` & `deafrica_tools-2.0.2/deafrica_tools/locales/fr/LC_MESSAGES/deafrica_tools.po`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.1/deafrica_tools/plotting.py` & `deafrica_tools-2.0.2/deafrica_tools/plotting.py`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.1/deafrica_tools/spatial.py` & `deafrica_tools-2.0.2/deafrica_tools/spatial.py`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.1/deafrica_tools/temporal.py` & `deafrica_tools-2.0.2/deafrica_tools/temporal.py`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.1/deafrica_tools/wetlands.py` & `deafrica_tools-2.0.2/deafrica_tools/wetlands.py`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.1/pyproject.toml` & `deafrica_tools-2.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # pyproject.toml tells “frontend” build tools like pip and build what “backend” tool to use to create distribution packages for your project.
 
 # Using poetry for dependency management and packaging.
 
 # Package metadata.
 [tool.poetry]
 name = "deafrica-tools"
-version = "2.0.1"
+version = "2.0.2"
 description = "Functions and algorithms for analysing Digital Earth Africa data."
 license = "Apache-2.0"
 authors = ["Digital Earth Africa <systems@digitalearthafrica.org>"]
 readme = "README.md"
 homepage = "https://github.com/digitalearthafrica/deafrica-sandbox-notebooks"
 repository = "https://github.com/digitalearthafrica/deafrica-sandbox-notebooks"
 documentation = "https://docs.digitalearthafrica.org/en/latest/sandbox/notebooks/Tools/index.html"
```

### Comparing `deafrica_tools-2.0.1/PKG-INFO` & `deafrica_tools-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deafrica-tools
-Version: 2.0.1
+Version: 2.0.2
 Summary: Functions and algorithms for analysing Digital Earth Africa data.
 Home-page: https://github.com/digitalearthafrica/deafrica-sandbox-notebooks
 License: Apache-2.0
 Author: Digital Earth Africa
 Author-email: systems@digitalearthafrica.org
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
```

