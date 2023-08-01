# Comparing `tmp/heatfall-0.0.1.tar.gz` & `tmp/heatfall-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heatfall-0.0.1.tar", last modified: Tue Aug  1 16:54:12 2023, max compression
+gzip compressed data, was "heatfall-0.0.2.tar", last modified: Tue Aug  1 18:42:27 2023, max compression
```

## Comparing `heatfall-0.0.1.tar` & `heatfall-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-08-01 16:54:12.858980 heatfall-0.0.1/
--rw-r--r--   0 odosmatthews   (501) staff       (20)     1068 2023-08-01 14:52:25.000000 heatfall-0.0.1/LICENSE
--rw-r--r--   0 odosmatthews   (501) staff       (20)     2062 2023-08-01 16:54:12.859129 heatfall-0.0.1/PKG-INFO
--rw-r--r--   0 odosmatthews   (501) staff       (20)     1431 2023-08-01 16:49:40.000000 heatfall-0.0.1/README.md
--rw-r--r--   0 odosmatthews   (501) staff       (20)      499 2023-08-01 14:52:21.000000 heatfall-0.0.1/pyproject.toml
--rw-r--r--   0 odosmatthews   (501) staff       (20)      958 2023-08-01 16:54:12.860525 heatfall-0.0.1/setup.cfg
--rw-r--r--   0 odosmatthews   (501) staff       (20)       68 2023-08-01 14:43:18.000000 heatfall-0.0.1/setup.py
-drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-08-01 16:54:12.832945 heatfall-0.0.1/src/
-drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-08-01 16:54:12.850282 heatfall-0.0.1/src/heatfall/
--rw-r--r--   0 odosmatthews   (501) staff       (20)       63 2023-08-01 16:53:03.000000 heatfall-0.0.1/src/heatfall/__init__.py
--rw-r--r--   0 odosmatthews   (501) staff       (20)     5964 2023-07-21 17:24:03.000000 heatfall-0.0.1/src/heatfall/heat.py
-drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-08-01 16:54:12.858651 heatfall-0.0.1/src/heatfall.egg-info/
--rw-r--r--   0 odosmatthews   (501) staff       (20)     2062 2023-08-01 16:54:12.000000 heatfall-0.0.1/src/heatfall.egg-info/PKG-INFO
--rw-r--r--   0 odosmatthews   (501) staff       (20)      311 2023-08-01 16:54:12.000000 heatfall-0.0.1/src/heatfall.egg-info/SOURCES.txt
--rw-r--r--   0 odosmatthews   (501) staff       (20)        1 2023-08-01 16:54:12.000000 heatfall-0.0.1/src/heatfall.egg-info/dependency_links.txt
--rw-r--r--   0 odosmatthews   (501) staff       (20)        1 2023-08-01 16:54:12.000000 heatfall-0.0.1/src/heatfall.egg-info/not-zip-safe
--rw-r--r--   0 odosmatthews   (501) staff       (20)      144 2023-08-01 16:54:12.000000 heatfall-0.0.1/src/heatfall.egg-info/requires.txt
--rw-r--r--   0 odosmatthews   (501) staff       (20)        9 2023-08-01 16:54:12.000000 heatfall-0.0.1/src/heatfall.egg-info/top_level.txt
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-08-01 18:42:27.889318 heatfall-0.0.2/
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     1068 2023-08-01 14:52:25.000000 heatfall-0.0.2/LICENSE
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     2072 2023-08-01 18:42:27.889459 heatfall-0.0.2/PKG-INFO
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     1440 2023-08-01 18:41:12.000000 heatfall-0.0.2/README.md
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      499 2023-08-01 14:52:21.000000 heatfall-0.0.2/pyproject.toml
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      968 2023-08-01 18:42:27.890544 heatfall-0.0.2/setup.cfg
+-rw-r--r--   0 odosmatthews   (501) staff       (20)       68 2023-08-01 14:43:18.000000 heatfall-0.0.2/setup.py
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-08-01 18:42:27.879739 heatfall-0.0.2/src/
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-08-01 18:42:27.882591 heatfall-0.0.2/src/heatfall/
+-rw-r--r--   0 odosmatthews   (501) staff       (20)       66 2023-08-01 18:38:37.000000 heatfall-0.0.2/src/heatfall/__init__.py
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     5964 2023-07-21 17:24:03.000000 heatfall-0.0.2/src/heatfall/heat.py
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-08-01 18:42:27.889093 heatfall-0.0.2/src/heatfall.egg-info/
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     2072 2023-08-01 18:42:27.000000 heatfall-0.0.2/src/heatfall.egg-info/PKG-INFO
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      311 2023-08-01 18:42:27.000000 heatfall-0.0.2/src/heatfall.egg-info/SOURCES.txt
+-rw-r--r--   0 odosmatthews   (501) staff       (20)        1 2023-08-01 18:42:27.000000 heatfall-0.0.2/src/heatfall.egg-info/dependency_links.txt
+-rw-r--r--   0 odosmatthews   (501) staff       (20)        1 2023-08-01 16:54:12.000000 heatfall-0.0.2/src/heatfall.egg-info/not-zip-safe
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      152 2023-08-01 18:42:27.000000 heatfall-0.0.2/src/heatfall.egg-info/requires.txt
+-rw-r--r--   0 odosmatthews   (501) staff       (20)        9 2023-08-01 18:42:27.000000 heatfall-0.0.2/src/heatfall.egg-info/top_level.txt
```

### Comparing `heatfall-0.0.1/LICENSE` & `heatfall-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `heatfall-0.0.1/PKG-INFO` & `heatfall-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: heatfall
-Version: 0.0.1
-Summary: Easy to use functions to plot heatmaps of geospatial data using staticmaps.
+Version: 0.0.2
+Summary: Easy to use functions to plot heat maps of geospatial data using staticmaps.
 Author: Odos Matthews
 License: MIT
 Platform: unix
 Platform: linux
 Platform: osx
 Platform: cygwin
 Platform: win32
@@ -37,20 +37,20 @@
 ```sh
 # PyPI
 pip install heatfall
 ```
 
 ## Dependencies
 - [py-staticmaps - A python module to create static map images (PNG, SVG) with markers, geodesic lines, etc.](https://github.com/flopp/py-staticmaps)
-- [PyGeodesy - A pure Python implementation of geodesy tools for various ellipsoidal and spherical earth models using precision trigonometric, vector-based, exact, elliptic, iterative and approximate methods for geodetic (lat-/longitude), geocentric (ECEF cartesian) and certain triaxial ellipsoidal coordinates.] (https://github.com/mrJean1/PyGeodesy)
+- [PyGeodesy - A pure Python implementation of geodesy tools for various ellipsoidal and spherical earth models using precision trigonometric, vector-based, exact, elliptic, iterative and approximate methods for geodetic (lat-/longitude), geocentric (ECEF cartesian) and certain triaxial ellipsoidal coordinates.](https://github.com/mrJean1/PyGeodesy)
 
 ## Example
 ```sh
 import heatfall
 
 
 lats = [27.88, 27.92, 27.94]
 lons = [-82.49, -82.49, -82.46]
 
-heatfall.plot_heat(lats, lons)
+heatfall.plot_heat_hashes(lats, lons, 4)
 ```
 ![](https://raw.githubusercontent.com/eddiethedean/heatfall/main/docs/example_map.png)
```

### Comparing `heatfall-0.0.1/README.md` & `heatfall-0.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -16,20 +16,20 @@
 ```sh
 # PyPI
 pip install heatfall
 ```
 
 ## Dependencies
 - [py-staticmaps - A python module to create static map images (PNG, SVG) with markers, geodesic lines, etc.](https://github.com/flopp/py-staticmaps)
-- [PyGeodesy - A pure Python implementation of geodesy tools for various ellipsoidal and spherical earth models using precision trigonometric, vector-based, exact, elliptic, iterative and approximate methods for geodetic (lat-/longitude), geocentric (ECEF cartesian) and certain triaxial ellipsoidal coordinates.] (https://github.com/mrJean1/PyGeodesy)
+- [PyGeodesy - A pure Python implementation of geodesy tools for various ellipsoidal and spherical earth models using precision trigonometric, vector-based, exact, elliptic, iterative and approximate methods for geodetic (lat-/longitude), geocentric (ECEF cartesian) and certain triaxial ellipsoidal coordinates.](https://github.com/mrJean1/PyGeodesy)
 
 ## Example
 ```sh
 import heatfall
 
 
 lats = [27.88, 27.92, 27.94]
 lons = [-82.49, -82.49, -82.46]
 
-heatfall.plot_heat(lats, lons)
+heatfall.plot_heat_hashes(lats, lons, 4)
 ```
 ![](https://raw.githubusercontent.com/eddiethedean/heatfall/main/docs/example_map.png)
```

### Comparing `heatfall-0.0.1/setup.cfg` & `heatfall-0.0.2/setup.cfg`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = heatfall
-version = 0.0.1
-description = Easy to use functions to plot heatmaps of geospatial data using staticmaps.
+version = 0.0.2
+description = Easy to use functions to plot heat maps of geospatial data using staticmaps.
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8
 author = Odos Matthews
 license = MIT
 license_file = LICENSE
 platforms = unix, linux, osx, cygwin, win32
 classifiers = 
@@ -20,14 +20,15 @@
 	heatfall
 install_requires = 
 	range_key_dict
 	geodude
 	py-staticmaps
 	Pillow<=9.5.0
 	more_itertools
+	tinytim
 python_requires = >=3.8
 package_dir = 
 	=src
 zip_safe = no
 
 [options.extras_require]
 testing =
```

### Comparing `heatfall-0.0.1/src/heatfall/heat.py` & `heatfall-0.0.2/src/heatfall/heat.py`

 * *Files identical despite different names*

### Comparing `heatfall-0.0.1/src/heatfall.egg-info/PKG-INFO` & `heatfall-0.0.2/src/heatfall.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: heatfall
-Version: 0.0.1
-Summary: Easy to use functions to plot heatmaps of geospatial data using staticmaps.
+Version: 0.0.2
+Summary: Easy to use functions to plot heat maps of geospatial data using staticmaps.
 Author: Odos Matthews
 License: MIT
 Platform: unix
 Platform: linux
 Platform: osx
 Platform: cygwin
 Platform: win32
@@ -37,20 +37,20 @@
 ```sh
 # PyPI
 pip install heatfall
 ```
 
 ## Dependencies
 - [py-staticmaps - A python module to create static map images (PNG, SVG) with markers, geodesic lines, etc.](https://github.com/flopp/py-staticmaps)
-- [PyGeodesy - A pure Python implementation of geodesy tools for various ellipsoidal and spherical earth models using precision trigonometric, vector-based, exact, elliptic, iterative and approximate methods for geodetic (lat-/longitude), geocentric (ECEF cartesian) and certain triaxial ellipsoidal coordinates.] (https://github.com/mrJean1/PyGeodesy)
+- [PyGeodesy - A pure Python implementation of geodesy tools for various ellipsoidal and spherical earth models using precision trigonometric, vector-based, exact, elliptic, iterative and approximate methods for geodetic (lat-/longitude), geocentric (ECEF cartesian) and certain triaxial ellipsoidal coordinates.](https://github.com/mrJean1/PyGeodesy)
 
 ## Example
 ```sh
 import heatfall
 
 
 lats = [27.88, 27.92, 27.94]
 lons = [-82.49, -82.49, -82.46]
 
-heatfall.plot_heat(lats, lons)
+heatfall.plot_heat_hashes(lats, lons, 4)
 ```
 ![](https://raw.githubusercontent.com/eddiethedean/heatfall/main/docs/example_map.png)
```

