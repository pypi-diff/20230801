# Comparing `tmp/pygeoops-0.2.0a4.tar.gz` & `tmp/pygeoops-0.3.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygeoops-0.2.0a4.tar", last modified: Thu Jul 27 01:41:15 2023, max compression
+gzip compressed data, was "pygeoops-0.3.0a0.tar", last modified: Tue Aug  1 13:49:37 2023, max compression
```

## Comparing `pygeoops-0.2.0a4.tar` & `pygeoops-0.3.0a0.tar`

### file list

```diff
@@ -1,35 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:41:15.755622 pygeoops-0.2.0a4/
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-27 01:41:05.000000 pygeoops-0.2.0a4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-27 01:41:05.000000 pygeoops-0.2.0a4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-07-27 01:41:15.755622 pygeoops-0.2.0a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-27 01:41:05.000000 pygeoops-0.2.0a4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:41:15.751622 pygeoops-0.2.0a4/pygeoops/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-27 01:41:05.000000 pygeoops-0.2.0a4/pygeoops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11750 2023-07-27 01:41:05.000000 pygeoops-0.2.0a4/pygeoops/_centerline.py
--rw-r--r--   0 runner    (1001) docker     (123)    10746 2023-07-27 01:41:05.000000 pygeoops-0.2.0a4/pygeoops/_general.py
--rw-r--r--   0 runner    (1001) docker     (123)     8595 2023-07-27 01:41:05.000000 pygeoops-0.2.0a4/pygeoops/_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    12042 2023-07-27 01:41:05.000000 pygeoops-0.2.0a4/pygeoops/_simplify.py
--rw-r--r--   0 runner    (1001) docker     (123)     9290 2023-07-27 01:41:05.000000 pygeoops-0.2.0a4/pygeoops/_simplify_lang.py
--rw-r--r--   0 runner    (1001) docker     (123)     5833 2023-07-27 01:41:05.000000 pygeoops-0.2.0a4/pygeoops/_simplify_topo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-07-27 01:41:05.000000 pygeoops-0.2.0a4/pygeoops/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     7639 2023-07-27 01:41:05.000000 pygeoops-0.2.0a4/pygeoops/_view_angles.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-27 01:41:05.000000 pygeoops-0.2.0a4/pygeoops/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:41:15.751622 pygeoops-0.2.0a4/pygeoops.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-07-27 01:41:15.000000 pygeoops-0.2.0a4/pygeoops.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-27 01:41:15.000000 pygeoops-0.2.0a4/pygeoops.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 01:41:15.000000 pygeoops-0.2.0a4/pygeoops.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-27 01:41:15.000000 pygeoops-0.2.0a4/pygeoops.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-27 01:41:15.000000 pygeoops-0.2.0a4/pygeoops.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-07-27 01:41:05.000000 pygeoops-0.2.0a4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-27 01:41:15.755622 pygeoops-0.2.0a4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-27 01:41:05.000000 pygeoops-0.2.0a4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:41:15.755622 pygeoops-0.2.0a4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-07-27 01:41:05.000000 pygeoops-0.2.0a4/tests/test_centerline.py
--rw-r--r--   0 runner    (1001) docker     (123)     8464 2023-07-27 01:41:05.000000 pygeoops-0.2.0a4/tests/test_general.py
--rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-07-27 01:41:05.000000 pygeoops-0.2.0a4/tests/test_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-07-27 01:41:05.000000 pygeoops-0.2.0a4/tests/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    12708 2023-07-27 01:41:05.000000 pygeoops-0.2.0a4/tests/test_simplify.py
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-07-27 01:41:05.000000 pygeoops-0.2.0a4/tests/test_simplify_lang.py
--rw-r--r--   0 runner    (1001) docker     (123)     9019 2023-07-27 01:41:05.000000 pygeoops-0.2.0a4/tests/test_simplify_topo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-07-27 01:41:05.000000 pygeoops-0.2.0a4/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-07-27 01:41:05.000000 pygeoops-0.2.0a4/tests/test_view_angles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:49:37.991353 pygeoops-0.3.0a0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-08-01 13:49:24.000000 pygeoops-0.3.0a0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-01 13:49:24.000000 pygeoops-0.3.0a0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-08-01 13:49:37.991353 pygeoops-0.3.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-08-01 13:49:24.000000 pygeoops-0.3.0a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:49:37.987353 pygeoops-0.3.0a0/pygeoops/
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-08-01 13:49:24.000000 pygeoops-0.3.0a0/pygeoops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11750 2023-08-01 13:49:24.000000 pygeoops-0.3.0a0/pygeoops/_centerline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10195 2023-08-01 13:49:24.000000 pygeoops-0.3.0a0/pygeoops/_difference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12868 2023-08-01 13:49:24.000000 pygeoops-0.3.0a0/pygeoops/_general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8595 2023-08-01 13:49:24.000000 pygeoops-0.3.0a0/pygeoops/_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-08-01 13:49:24.000000 pygeoops-0.3.0a0/pygeoops/_paramvalidation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11979 2023-08-01 13:49:24.000000 pygeoops-0.3.0a0/pygeoops/_simplify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9290 2023-08-01 13:49:24.000000 pygeoops-0.3.0a0/pygeoops/_simplify_lang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5833 2023-08-01 13:49:24.000000 pygeoops-0.3.0a0/pygeoops/_simplify_topo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-08-01 13:49:24.000000 pygeoops-0.3.0a0/pygeoops/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7639 2023-08-01 13:49:24.000000 pygeoops-0.3.0a0/pygeoops/_view_angles.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-01 13:49:24.000000 pygeoops-0.3.0a0/pygeoops/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:49:37.991353 pygeoops-0.3.0a0/pygeoops.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-08-01 13:49:37.000000 pygeoops-0.3.0a0/pygeoops.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-08-01 13:49:37.000000 pygeoops-0.3.0a0/pygeoops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 13:49:37.000000 pygeoops-0.3.0a0/pygeoops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 13:49:37.000000 pygeoops-0.3.0a0/pygeoops.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-01 13:49:37.000000 pygeoops-0.3.0a0/pygeoops.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-08-01 13:49:24.000000 pygeoops-0.3.0a0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-08-01 13:49:37.991353 pygeoops-0.3.0a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-08-01 13:49:24.000000 pygeoops-0.3.0a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:49:37.991353 pygeoops-0.3.0a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-08-01 13:49:24.000000 pygeoops-0.3.0a0/tests/test_centerline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-08-01 13:49:24.000000 pygeoops-0.3.0a0/tests/test_difference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11870 2023-08-01 13:49:24.000000 pygeoops-0.3.0a0/tests/test_general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-08-01 13:49:24.000000 pygeoops-0.3.0a0/tests/test_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-08-01 13:49:24.000000 pygeoops-0.3.0a0/tests/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-08-01 13:49:24.000000 pygeoops-0.3.0a0/tests/test_paramvalidation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-08-01 13:49:24.000000 pygeoops-0.3.0a0/tests/test_shapely.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12922 2023-08-01 13:49:24.000000 pygeoops-0.3.0a0/tests/test_simplify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-08-01 13:49:24.000000 pygeoops-0.3.0a0/tests/test_simplify_lang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9037 2023-08-01 13:49:24.000000 pygeoops-0.3.0a0/tests/test_simplify_topo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-08-01 13:49:24.000000 pygeoops-0.3.0a0/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-08-01 13:49:24.000000 pygeoops-0.3.0a0/tests/test_view_angles.py
```

### Comparing `pygeoops-0.2.0a4/LICENSE.txt` & `pygeoops-0.3.0a0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pygeoops-0.2.0a4/PKG-INFO` & `pygeoops-0.3.0a0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: pygeoops
-Version: 0.2.0a4
+Version: 0.3.0a0
 Summary: Library with some less common or extended spatial functions
 Author-email: Pieter Roggemans <pieter.roggemans@gmail.com>
 Project-URL: Homepage, https://github.com/pygeoops/pygeoops
 Project-URL: Bug Tracker, https://github.com/pygeoops/pygeoops/issues
 Keywords: GIS,cartography,pandas,shapely,geopandas
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: full
 License-File: LICENSE.txt
 
 # PyGeoOps
 
 [![Actions Status](https://github.com/pygeoops/pygeoops/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/pygeoops/pygeoops/actions/workflows/tests.yml?query=workflow%3ATests) 
 [![codecov](https://codecov.io/gh/pygeoops/pygeoops/branch/main/graph/badge.svg?token=4241CY86O2)](https://codecov.io/gh/pygeoops/pygeoops)
 [![PyPI version](https://img.shields.io/pypi/v/pygeoops.svg)](https://pypi.org/project/pygeoops)
```

### Comparing `pygeoops-0.2.0a4/README.md` & `pygeoops-0.3.0a0/README.md`

 * *Files identical despite different names*

### Comparing `pygeoops-0.2.0a4/pygeoops/_centerline.py` & `pygeoops-0.3.0a0/pygeoops/_centerline.py`

 * *Files identical despite different names*

### Comparing `pygeoops-0.2.0a4/pygeoops/_general.py` & `pygeoops-0.3.0a0/pygeoops/_general.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import Optional, Union
+import warnings
 
 from geopandas import GeoSeries
 import numpy as np
 from numpy.typing import NDArray
 import pyproj
 import shapely
 from shapely.geometry.base import BaseGeometry, BaseMultipartGeometry
@@ -82,77 +83,138 @@
     elif result_collection_type == GeometryType.GEOMETRYCOLLECTION:
         return shapely.GeometryCollection(geometries)
     else:
         raise ValueError(f"Unsupported geometry type: {result_collection_type}")
 
 
 def collection_extract(
-    geometry, primitivetype: PrimitiveType
+    geometry,
+    keep_geom_type: Union[int, PrimitiveType, None] = None,
+    primitivetype: Optional[PrimitiveType] = None,
 ) -> Union[BaseGeometry, NDArray[BaseGeometry], None]:
     """
     Extracts the parts from the input geometry/geometries that comply with the
     primitive_type specified and returns them as (Multi)geometry.
 
     Args:
         geometry (geometry, GeoSeries or arraylike): geometry or arraylike.
-        primitivetype (GeometryPrimitiveTypes): the primitive type to extract from the
-            input geometry.
+        keep_geom_type (Union[int, PrimitiveType]): the type of geometries to keep in
+            the output. Either a PrimitiveType or and int with one of the following
+            values: -1: all, 0: points, 1: lines, 2: polygons.
+        primitivetype (PrimitiveType): deprecated, use keep_geom_type.
 
     Raises:
         ValueError: if in_geom is an unsupported geometry type or the primitive
             type is invalid.
 
     Returns:
         Union[BaseGeometry, NDArray[BaseGeometry], None]: geometry or array of
             geometries containing only parts of the primitive type specified.
     """
-    # Extract the polygons from the multipolygon, but store them as multipolygons anyway
+    if primitivetype is not None:
+        warnings.warn(
+            "primitivetype parameter is deprecated, use keep_geom_type. Will be "
+            "removed in a later version.",
+            FutureWarning,
+            stacklevel=2,
+        )
     if geometry is None:
         return None
+    if keep_geom_type is not None and primitivetype is not None:
+        raise ValueError("primitivetype is deprecated, only specify keep_geom_type")
+    if keep_geom_type is None:
+        if primitivetype is not None:
+            keep_geom_type = primitivetype.value - 1
+        else:
+            raise ValueError("keep_geom_type should be specified")
+    elif isinstance(keep_geom_type, PrimitiveType):
+        keep_geom_type = keep_geom_type.value - 1
+    elif isinstance(keep_geom_type, (int, np.integer)):
+        if keep_geom_type not in [-1, 0, 1, 2]:
+            raise ValueError(f"Invalid value for keep_geom_type: {keep_geom_type}")
+    else:
+        raise ValueError(f"Invalid type for keep_geom_type: {type(keep_geom_type)}")
+    assert keep_geom_type is not None
 
     # If input is not arraylike, apply once, otherwise apply to all elements
     if not hasattr(geometry, "__len__"):
-        return _collection_extract(geometry=geometry, primitivetype=primitivetype)
+        return _collection_extract(geometry=geometry, keep_geom_type=keep_geom_type)
     else:
         result = np.array(
             [
-                _collection_extract(geometry=geom, primitivetype=primitivetype)
+                _collection_extract(geometry=geom, keep_geom_type=keep_geom_type)
                 for geom in geometry
             ]
         )
         if isinstance(geometry, GeoSeries):
             result = GeoSeries(result, index=geometry.index, crs=geometry.crs)
         return result
 
 
 def _collection_extract(
-    geometry: Optional[BaseGeometry], primitivetype: PrimitiveType
+    geometry: Optional[BaseGeometry], keep_geom_type: int
 ) -> Optional[BaseGeometry]:
     if geometry is None:
         return None
+    if keep_geom_type == -1:
+        return geometry
 
     if isinstance(geometry, (shapely.MultiPoint, shapely.Point)):
-        if primitivetype == PrimitiveType.POINT:
+        if keep_geom_type == 0:
             return geometry
     elif isinstance(geometry, (shapely.LineString, shapely.MultiLineString)):
-        if primitivetype == PrimitiveType.LINESTRING:
+        if keep_geom_type == 1:
             return geometry
     elif isinstance(geometry, (shapely.MultiPolygon, shapely.Polygon)):
-        if primitivetype == PrimitiveType.POLYGON:
+        if keep_geom_type == 2:
             return geometry
     elif isinstance(geometry, shapely.GeometryCollection):
         returngeoms = [
-            collection_extract(geometry, primitivetype=primitivetype)
+            collection_extract(geometry, keep_geom_type=keep_geom_type)
             for geometry in shapely.GeometryCollection(geometry).geoms
         ]
         if len(returngeoms) > 0:
             return collect(returngeoms)
     else:
         raise ValueError(f"Invalid/unsupported geometry(type): {geometry}")
 
+    return None
+
+
+def empty(dimension: int) -> Optional[BaseGeometry]:
+    """
+    Generate an empty geometry of the type specified.
+
+    Args:
+        dimension (int): Dimension of the empty geometry to return. Possible values:
+            - None: None returned
+            - -1: empty GeometryCollection
+            - 0: empty Point
+            - 1: empty LineString
+            - 2: empty Polygon
+
+    Raises:
+        ValueError: Invalid dimension specified
+
+    Returns:
+        Optional[BaseGeometry]: empty geometry or None.
+    """
+    if dimension is None:
+        return None
+    elif dimension == -1:
+        return shapely.GeometryCollection()
+    elif dimension == 0:
+        return shapely.Point()
+    elif dimension == 1:
+        return shapely.LineString()
+    elif dimension == 2:
+        return shapely.Polygon()
+    else:
+        raise ValueError(f"Invalid dimension specified: {dimension}")
+
 
 def explode(geometry: Optional[BaseGeometry]) -> Optional[NDArray[BaseGeometry]]:
     """
     Dump all (multi)geometries in the input to one list of single geometries.
 
     Args:
         geometry (BaseGeometry, optional): geometry to explode.
```

### Comparing `pygeoops-0.2.0a4/pygeoops/_grid.py` & `pygeoops-0.3.0a0/pygeoops/_grid.py`

 * *Files identical despite different names*

### Comparing `pygeoops-0.2.0a4/pygeoops/_simplify.py` & `pygeoops-0.3.0a0/pygeoops/_simplify.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,14 @@
     import simplification.cutil as simplification
 
     HAS_SIMPLIFICATION = True
 except ImportError:
     HAS_SIMPLIFICATION = False
 
 import pygeoops._general as general
-from pygeoops._general import PrimitiveType
 from pygeoops import _simplify_lang as simplify_lang
 from pygeoops import _simplify_topo as simplify_topo
 
 logger = logging.getLogger(__name__)
 
 
 def simplify(
@@ -240,15 +239,15 @@
             # add original ring
             interiors_simpl.append(interior.coords)
 
     result_poly = shapely.Polygon(exterior_simpl, interiors_simpl)
 
     # Extract only polygons as result + try to make valid
     result_poly = general.collection_extract(
-        shapely.make_valid(result_poly), primitivetype=PrimitiveType.POLYGON
+        shapely.make_valid(result_poly), keep_geom_type=2
     )
 
     # If the result is None and the topology needs to be preserved, return
     # original polygon
     if preserve_topology and result_poly is None:
         return polygon
```

### Comparing `pygeoops-0.2.0a4/pygeoops/_simplify_lang.py` & `pygeoops-0.3.0a0/pygeoops/_simplify_lang.py`

 * *Files identical despite different names*

### Comparing `pygeoops-0.2.0a4/pygeoops/_simplify_topo.py` & `pygeoops-0.3.0a0/pygeoops/_simplify_topo.py`

 * *Files identical despite different names*

### Comparing `pygeoops-0.2.0a4/pygeoops/_types.py` & `pygeoops-0.3.0a0/pygeoops/_types.py`

 * *Files identical despite different names*

### Comparing `pygeoops-0.2.0a4/pygeoops/_view_angles.py` & `pygeoops-0.3.0a0/pygeoops/_view_angles.py`

 * *Files identical despite different names*

### Comparing `pygeoops-0.2.0a4/pygeoops.egg-info/PKG-INFO` & `pygeoops-0.3.0a0/pygeoops.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: pygeoops
-Version: 0.2.0a4
+Version: 0.3.0a0
 Summary: Library with some less common or extended spatial functions
 Author-email: Pieter Roggemans <pieter.roggemans@gmail.com>
 Project-URL: Homepage, https://github.com/pygeoops/pygeoops
 Project-URL: Bug Tracker, https://github.com/pygeoops/pygeoops/issues
 Keywords: GIS,cartography,pandas,shapely,geopandas
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: full
 License-File: LICENSE.txt
 
 # PyGeoOps
 
 [![Actions Status](https://github.com/pygeoops/pygeoops/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/pygeoops/pygeoops/actions/workflows/tests.yml?query=workflow%3ATests) 
 [![codecov](https://codecov.io/gh/pygeoops/pygeoops/branch/main/graph/badge.svg?token=4241CY86O2)](https://codecov.io/gh/pygeoops/pygeoops)
 [![PyPI version](https://img.shields.io/pypi/v/pygeoops.svg)](https://pypi.org/project/pygeoops)
```

### Comparing `pygeoops-0.2.0a4/pygeoops.egg-info/SOURCES.txt` & `pygeoops-0.3.0a0/pygeoops.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -2,29 +2,34 @@
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 pygeoops/__init__.py
 pygeoops/_centerline.py
+pygeoops/_difference.py
 pygeoops/_general.py
 pygeoops/_grid.py
+pygeoops/_paramvalidation.py
 pygeoops/_simplify.py
 pygeoops/_simplify_lang.py
 pygeoops/_simplify_topo.py
 pygeoops/_types.py
 pygeoops/_view_angles.py
 pygeoops/version.txt
 pygeoops.egg-info/PKG-INFO
 pygeoops.egg-info/SOURCES.txt
 pygeoops.egg-info/dependency_links.txt
 pygeoops.egg-info/requires.txt
 pygeoops.egg-info/top_level.txt
 tests/test_centerline.py
+tests/test_difference.py
 tests/test_general.py
 tests/test_grid.py
 tests/test_helper.py
+tests/test_paramvalidation.py
+tests/test_shapely.py
 tests/test_simplify.py
 tests/test_simplify_lang.py
 tests/test_simplify_topo.py
 tests/test_types.py
 tests/test_view_angles.py
```

### Comparing `pygeoops-0.2.0a4/pyproject.toml` & `pygeoops-0.3.0a0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pygeoops"
-version = "0.2.0a4"
+version = "0.3.0a0"
 authors = [
   { name="Pieter Roggemans", email="pieter.roggemans@gmail.com" },
 ]
 description = "Library with some less common or extended spatial functions"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -19,14 +19,18 @@
 dependencies = [
     "geopandas",
     "shapely>1",
     "topojson",
 ]
 keywords = ["GIS", "cartography", "pandas", "shapely", "geopandas"]
 
+[project.optional-dependencies]
+# development dependency groups
+full = ["simplification"]
+
 [project.urls]
 "Homepage" = "https://github.com/pygeoops/pygeoops"
 "Bug Tracker" = "https://github.com/pygeoops/pygeoops/issues"
 
 [tool.black]
 line-length = 88
```

### Comparing `pygeoops-0.2.0a4/tests/test_centerline.py` & `pygeoops-0.3.0a0/tests/test_centerline.py`

 * *Files identical despite different names*

### Comparing `pygeoops-0.2.0a4/tests/test_general.py` & `pygeoops-0.3.0a0/tests/test_general.py`

 * *Files 16% similar despite different names*

```diff
@@ -58,38 +58,110 @@
     # Test arraylike input
     # --------------------
     assert pygeoops.collect(gpd.GeoSeries([point, line, poly])) == geometrycoll
     assert pygeoops.collect(np.array([point, line, poly])) == geometrycoll
 
 
 def test_collection_extract():
+    """
+    Base tests
+    """
     # Test None input
     # ---------------
-    assert pygeoops.collection_extract(None, PrimitiveType.POINT) is None
-    assert pygeoops.collection_extract([None], PrimitiveType.POINT) == [None]
+    assert pygeoops.collection_extract(None, 0) is None
+    assert pygeoops.collection_extract([None], 0) == [None]
 
     # Test dealing with points
     # ------------------------
     point = shapely.Point((0, 0))
     multipoint = shapely.MultiPoint([point, point])
-    assert pygeoops.collection_extract(point, PrimitiveType.POINT) == point
-    assert pygeoops.collection_extract(multipoint, PrimitiveType.POINT) == multipoint
-    assert pygeoops.collection_extract(multipoint, PrimitiveType.POLYGON) is None
+    assert pygeoops.collection_extract(point, 0) == point
+    assert pygeoops.collection_extract(multipoint, 0) == multipoint
+    assert pygeoops.collection_extract(multipoint, 2) is None
 
     # Test dealing with mixed geometries
     # ----------------------------------
     line = shapely.LineString([(0, 0), (0, 1)])
     poly = shapely.Polygon([(0, 0), (0, 1), (0, 0)])
     multipoly = shapely.MultiPolygon([poly, poly])
     geometrycoll = shapely.GeometryCollection([point, line, poly, multipoly])
+    assert pygeoops.collection_extract(geometrycoll, 0) == point
     assert pygeoops.collection_extract(geometrycoll, PrimitiveType.POINT) == point
+    assert pygeoops.collection_extract(geometrycoll, 1) == line
     assert pygeoops.collection_extract(geometrycoll, PrimitiveType.LINESTRING) == line
+    assert pygeoops.collection_extract(geometrycoll, 2) == shapely.GeometryCollection(
+        [poly, multipoly]
+    )
     assert pygeoops.collection_extract(
         geometrycoll, PrimitiveType.POLYGON
     ) == shapely.GeometryCollection([poly, multipoly])
+    assert pygeoops.collection_extract(geometrycoll, -1) == geometrycoll
+
+    # Test dealing with deeper nested geometries
+    # ------------------------------------------
+    assert pygeoops.collection_extract(
+        shapely.GeometryCollection(geometrycoll), -1
+    ) == shapely.GeometryCollection(geometrycoll)
+
+
+def test_collection_extract_backwards_compatibility():
+    """
+    Test if it still works with PrimitiveType parameter
+    """
+    # Test None input
+    # ---------------
+    assert pygeoops.collection_extract(None, primitivetype=PrimitiveType.POINT) is None
+    assert pygeoops.collection_extract([None], primitivetype=PrimitiveType.POINT) == [
+        None
+    ]
+
+    # Test dealing with points
+    # ------------------------
+    point = shapely.Point((0, 0))
+    multipoint = shapely.MultiPoint([point, point])
+    assert (
+        pygeoops.collection_extract(point, primitivetype=PrimitiveType.POINT) == point
+    )
+    assert (
+        pygeoops.collection_extract(multipoint, primitivetype=PrimitiveType.POINT)
+        == multipoint
+    )
+    assert (
+        pygeoops.collection_extract(multipoint, primitivetype=PrimitiveType.POLYGON)
+        is None
+    )
+
+    # Test dealing with mixed geometries
+    # ----------------------------------
+    line = shapely.LineString([(0, 0), (0, 1)])
+    poly = shapely.Polygon([(0, 0), (0, 1), (0, 0)])
+    multipoly = shapely.MultiPolygon([poly, poly])
+    geometrycoll = shapely.GeometryCollection([point, line, poly, multipoly])
+    assert (
+        pygeoops.collection_extract(geometrycoll, primitivetype=PrimitiveType.POINT)
+        == point
+    )
+    assert (
+        pygeoops.collection_extract(
+            geometrycoll, primitivetype=PrimitiveType.LINESTRING
+        )
+        == line
+    )
+    assert pygeoops.collection_extract(
+        geometrycoll, primitivetype=PrimitiveType.POLYGON
+    ) == shapely.GeometryCollection([poly, multipoly])
+
+    # Invalid parameters/combinations
+    # -------------------------------
+    with pytest.raises(
+        ValueError, match="primitivetype is deprecated, only specify keep_geom_type"
+    ):
+        pygeoops.collection_extract(
+            geometrycoll, keep_geom_type=1, primitivetype=PrimitiveType.POINT
+        )
 
 
 @pytest.mark.parametrize("input_type", ["geoseries", "ndarray", "list"])
 def test_collection_extract_geometries(input_type):
     """
     Test collection_extract with several geometries as input.
     """
@@ -108,15 +180,15 @@
         input = gpd.GeoSeries(
             input, index=[index + start_idx for index in range(len(input))]
         )
     elif input_type == "ndarray":
         input = np.array(input)
 
     # Run test
-    result = pygeoops.collection_extract(input, primitivetype=PrimitiveType.POINT)
+    result = pygeoops.collection_extract(input, keep_geom_type=0)
 
     # Check result
     assert result is not None
     if input_type == "geoseries":
         assert isinstance(result, gpd.GeoSeries)
     else:
         assert isinstance(result, np.ndarray)
@@ -124,14 +196,36 @@
     assert result[start_idx + 1] == multipoint
     assert result[start_idx + 2] is None
     assert result[start_idx + 3] is None
     assert result[start_idx + 4] is None
     assert result[start_idx + 5] == point
 
 
+def test_collection_extract_invalid_params():
+    with pytest.raises(ValueError, match="Invalid value for keep_geom_type"):
+        pygeoops.collection_extract(shapely.Point((0, 0)), keep_geom_type=5)
+        pygeoops.collection_extract(shapely.Point((0, 0)), keep_geom_type=-5)
+    with pytest.raises(ValueError, match="keep_geom_type should be specified"):
+        pygeoops.collection_extract(shapely.Point((0, 0)), keep_geom_type=None)
+    with pytest.raises(ValueError, match="Invalid type for keep_geom_type"):
+        pygeoops.collection_extract(shapely.Point((0, 0)), keep_geom_type="invalid")
+
+
+def test_empty():
+    assert pygeoops.empty(None) is None
+    assert pygeoops.empty(-1) == shapely.GeometryCollection()
+    assert pygeoops.empty(0) == shapely.Point()
+    assert pygeoops.empty(1) == shapely.LineString()
+    assert pygeoops.empty(2) == shapely.Polygon()
+
+    with pytest.raises(ValueError, match="Invalid dimension specified"):
+        pygeoops.empty(-2)
+        pygeoops.empty(3)
+
+
 def test_explode():
     # Test dealing with None/empty input
     # ----------------------------------
     assert pygeoops.explode(None) is None
 
     # Test dealing with points
     # ------------------------
```

### Comparing `pygeoops-0.2.0a4/tests/test_grid.py` & `pygeoops-0.3.0a0/tests/test_grid.py`

 * *Files identical despite different names*

### Comparing `pygeoops-0.2.0a4/tests/test_helper.py` & `pygeoops-0.3.0a0/tests/test_helper.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,18 @@
 import shapely
 import shapely.affinity
 import shapely.plotting
 from shapely.geometry.base import BaseGeometry
 
 _data_dir = Path(__file__).parent.resolve() / "data"
 
+RUNS_LOCAL = True
+if "GITHUB_ACTIONS" in os.environ:
+    RUNS_LOCAL = False
+
 
 class TestData:
     crs_epsg = 31370
     point = shapely.Point((0, 0))
     multipoint = shapely.MultiPoint([(0, 0), (10, 10), (20, 20)])
     linestring = shapely.LineString([(0, 0), (10, 10), (20, 20)])
     multilinestring = shapely.MultiLineString(
```

### Comparing `pygeoops-0.2.0a4/tests/test_simplify.py` & `pygeoops-0.3.0a0/tests/test_simplify.py`

 * *Files 2% similar despite different names*

```diff
@@ -273,16 +273,16 @@
         )
 
 
 @pytest.mark.parametrize(
     "algorithm, tolerance", [("lang", 2), ("lang+", 2), ("rdp", 2), ("vw", 15)]
 )
 def test_simplify_keep_points_on(tmp_path, algorithm, tolerance):
-    # Skip test if simplification is not available
-    if algorithm != "lang":
+    # Skip test for algorithms that needs simplification lib when it is not available
+    if algorithm in ["rdp", "vw"]:
         _ = pytest.importorskip("simplification")
 
     # Prepare test data
     poly_input = shapely.Polygon(
         shell=[(0, 0), (0, 10), (5, 12), (10, 10), (10, 0), (5, 0), (0, 0)]
     )
     # Create geometry where we want the points kept
@@ -324,14 +324,18 @@
     assert result == [None]
 
 
 @pytest.mark.parametrize(
     "algorithm, tolerance", [("lang", 10), ("lang+", 10), ("vw", 50)]
 )
 def test_simplify_preservetopology(algorithm, tolerance):
+    # Skip test for algorithms that needs simplification lib when it is not available
+    if algorithm in ["rdp", "vw"]:
+        _ = pytest.importorskip("simplification")
+
     # Test Polygon lookahead -1
     poly = shapely.Polygon(
         shell=[(0, 0), (0, 10), (1, 10), (10, 10), (10, 0), (0, 0)],
         holes=[[(2, 2), (2, 8), (8, 8), (8, 2), (2, 2)]],
     )
 
     # If preserve_topology True, the original polygon is returned
```

### Comparing `pygeoops-0.2.0a4/tests/test_simplify_lang.py` & `pygeoops-0.3.0a0/tests/test_simplify_lang.py`

 * *Files identical despite different names*

### Comparing `pygeoops-0.2.0a4/tests/test_simplify_topo.py` & `pygeoops-0.3.0a0/tests/test_simplify_topo.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 
 from pygeoops import _simplify_topo as simplify_topo
 import test_helper
 
 
 @pytest.mark.parametrize("algorithm", ["rdp", "lang", "lang+"])
 def test_simplify_topo(algorithm):
-    # Skip test if algorithm != "lang" and simplification is not available
-    if algorithm != "lang":
+    # Skip test for algorithms that needs simplification lib when it is not available
+    if algorithm in ["rdp", "vw"]:
         _ = pytest.importorskip("simplification")
 
     # Prepare test data
     poly1 = shapely.Polygon([(10, 10), (0, 10), (0, 0), (10, 0), (10, 10)])
     poly2 = shapely.Polygon([(10, 10), (0, 10), (0, 0), (11, 0), (10, 10)])
     input = [poly1, poly2]
```

### Comparing `pygeoops-0.2.0a4/tests/test_types.py` & `pygeoops-0.3.0a0/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `pygeoops-0.2.0a4/tests/test_view_angles.py` & `pygeoops-0.3.0a0/tests/test_view_angles.py`

 * *Files identical despite different names*

