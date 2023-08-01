# Comparing `tmp/landfall-0.3.4.tar.gz` & `tmp/landfall-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "landfall-0.3.4.tar", last modified: Wed Jul 26 18:24:54 2023, max compression
+gzip compressed data, was "landfall-0.3.5.tar", last modified: Tue Aug  1 14:40:50 2023, max compression
```

## Comparing `landfall-0.3.4.tar` & `landfall-0.3.5.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-07-26 18:24:54.456950 landfall-0.3.4/
--rw-r--r--   0 odosmatthews   (501) staff       (20)     1068 2023-02-28 17:06:52.000000 landfall-0.3.4/LICENSE
--rw-r--r--   0 odosmatthews   (501) staff       (20)     1818 2023-07-26 18:24:54.457063 landfall-0.3.4/PKG-INFO
--rw-r--r--   0 odosmatthews   (501) staff       (20)     1191 2023-07-26 17:59:17.000000 landfall-0.3.4/README.md
--rw-r--r--   0 odosmatthews   (501) staff       (20)      499 2023-02-28 17:09:25.000000 landfall-0.3.4/pyproject.toml
--rw-r--r--   0 odosmatthews   (501) staff       (20)      926 2023-07-26 18:24:54.457994 landfall-0.3.4/setup.cfg
--rw-r--r--   0 odosmatthews   (501) staff       (20)       68 2023-07-25 16:48:54.000000 landfall-0.3.4/setup.py
-drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-07-26 18:24:54.441738 landfall-0.3.4/src/
-drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-07-26 18:24:54.451719 landfall-0.3.4/src/landfall/
--rw-r--r--   0 odosmatthews   (501) staff       (20)      216 2023-07-26 18:24:02.000000 landfall-0.3.4/src/landfall/__init__.py
--rw-r--r--   0 odosmatthews   (501) staff       (20)     1848 2023-03-06 19:27:35.000000 landfall-0.3.4/src/landfall/color.py
--rw-r--r--   0 odosmatthews   (501) staff       (20)      631 2023-03-06 17:06:44.000000 landfall-0.3.4/src/landfall/colorsys.py
--rw-r--r--   0 odosmatthews   (501) staff       (20)      865 2023-07-24 18:54:39.000000 landfall-0.3.4/src/landfall/combos.py
--rw-r--r--   0 odosmatthews   (501) staff       (20)      508 2023-07-25 18:14:06.000000 landfall-0.3.4/src/landfall/context.py
--rw-r--r--   0 odosmatthews   (501) staff       (20)      271 2023-03-06 17:06:44.000000 landfall-0.3.4/src/landfall/distinctipy.py
--rw-r--r--   0 odosmatthews   (501) staff       (20)     3823 2023-07-25 18:27:07.000000 landfall-0.3.4/src/landfall/points.py
--rw-r--r--   0 odosmatthews   (501) staff       (20)     2384 2023-07-26 18:23:23.000000 landfall-0.3.4/src/landfall/polygons.py
-drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-07-26 18:24:54.456480 landfall-0.3.4/src/landfall.egg-info/
--rw-r--r--   0 odosmatthews   (501) staff       (20)     1818 2023-07-26 18:24:54.000000 landfall-0.3.4/src/landfall.egg-info/PKG-INFO
--rw-r--r--   0 odosmatthews   (501) staff       (20)      481 2023-07-26 18:24:54.000000 landfall-0.3.4/src/landfall.egg-info/SOURCES.txt
--rw-r--r--   0 odosmatthews   (501) staff       (20)        1 2023-07-26 18:24:54.000000 landfall-0.3.4/src/landfall.egg-info/dependency_links.txt
--rw-r--r--   0 odosmatthews   (501) staff       (20)        1 2023-02-28 18:06:53.000000 landfall-0.3.4/src/landfall.egg-info/not-zip-safe
--rw-r--r--   0 odosmatthews   (501) staff       (20)      118 2023-07-26 18:24:54.000000 landfall-0.3.4/src/landfall.egg-info/requires.txt
--rw-r--r--   0 odosmatthews   (501) staff       (20)        9 2023-07-26 18:24:54.000000 landfall-0.3.4/src/landfall.egg-info/top_level.txt
-drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-07-26 18:24:54.456743 landfall-0.3.4/tests/
--rw-r--r--   0 odosmatthews   (501) staff       (20)      452 2023-07-25 18:31:53.000000 landfall-0.3.4/tests/test_points.py
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-08-01 14:40:50.516038 landfall-0.3.5/
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     1068 2023-02-28 17:06:52.000000 landfall-0.3.5/LICENSE
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     1818 2023-08-01 14:40:50.516246 landfall-0.3.5/PKG-INFO
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     1191 2023-07-26 17:59:17.000000 landfall-0.3.5/README.md
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      499 2023-02-28 17:09:25.000000 landfall-0.3.5/pyproject.toml
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      926 2023-08-01 14:40:50.517620 landfall-0.3.5/setup.cfg
+-rw-r--r--   0 odosmatthews   (501) staff       (20)       68 2023-07-25 16:48:54.000000 landfall-0.3.5/setup.py
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-08-01 14:40:50.501856 landfall-0.3.5/src/
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-08-01 14:40:50.510743 landfall-0.3.5/src/landfall/
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      216 2023-08-01 14:40:16.000000 landfall-0.3.5/src/landfall/__init__.py
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     1947 2023-07-31 15:01:40.000000 landfall-0.3.5/src/landfall/color.py
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      631 2023-03-06 17:06:44.000000 landfall-0.3.5/src/landfall/colorsys.py
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      865 2023-07-24 18:54:39.000000 landfall-0.3.5/src/landfall/combos.py
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      508 2023-07-25 18:14:06.000000 landfall-0.3.5/src/landfall/context.py
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      321 2023-07-31 15:01:00.000000 landfall-0.3.5/src/landfall/distinctipy.py
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     2307 2023-07-28 16:38:58.000000 landfall-0.3.5/src/landfall/plot.py
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     3837 2023-08-01 14:39:02.000000 landfall-0.3.5/src/landfall/points.py
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     4114 2023-08-01 14:36:49.000000 landfall-0.3.5/src/landfall/polygons.py
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-08-01 14:40:50.515323 landfall-0.3.5/src/landfall.egg-info/
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     1818 2023-08-01 14:40:50.000000 landfall-0.3.5/src/landfall.egg-info/PKG-INFO
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      502 2023-08-01 14:40:50.000000 landfall-0.3.5/src/landfall.egg-info/SOURCES.txt
+-rw-r--r--   0 odosmatthews   (501) staff       (20)        1 2023-08-01 14:40:50.000000 landfall-0.3.5/src/landfall.egg-info/dependency_links.txt
+-rw-r--r--   0 odosmatthews   (501) staff       (20)        1 2023-02-28 18:06:53.000000 landfall-0.3.5/src/landfall.egg-info/not-zip-safe
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      118 2023-08-01 14:40:50.000000 landfall-0.3.5/src/landfall.egg-info/requires.txt
+-rw-r--r--   0 odosmatthews   (501) staff       (20)        9 2023-08-01 14:40:50.000000 landfall-0.3.5/src/landfall.egg-info/top_level.txt
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-08-01 14:40:50.515781 landfall-0.3.5/tests/
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      452 2023-07-25 18:31:53.000000 landfall-0.3.5/tests/test_points.py
```

### Comparing `landfall-0.3.4/LICENSE` & `landfall-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `landfall-0.3.4/PKG-INFO` & `landfall-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: landfall
-Version: 0.3.4
+Version: 0.3.5
 Summary: Easy to use functions to plot geospatial data on maps using staticmaps.
 Author: Odos Matthews
 License: MIT
 Platform: unix
 Platform: linux
 Platform: osx
 Platform: cygwin
```

### Comparing `landfall-0.3.4/README.md` & `landfall-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `landfall-0.3.4/setup.cfg` & `landfall-0.3.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = landfall
-version = 0.3.4
+version = 0.3.5
 description = Easy to use functions to plot geospatial data on maps using staticmaps.
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8
 author = Odos Matthews
 license = MIT
 license_file = LICENSE
 platforms = unix, linux, osx, cygwin, win32
```

### Comparing `landfall-0.3.4/src/landfall/color.py` & `landfall-0.3.5/src/landfall/color.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 """
 Functions for using colors.
 """
 
 import random
-from typing import Sequence, List, Mapping, Union
+from typing import Optional, Sequence, List, Mapping, Union
 
 from staticmaps import Color, parse_color
 
 from .distinctipy import get_distict_colors
 from .colorsys import get_wheel_colors
 
 
-def random_color():
+def random_color(rng: Optional[int] = None):
+    random.seed(rng)
     r = random.randrange(0, 256)
     g = random.randrange(0, 256)
     b = random.randrange(0, 256)
     return Color(r, g, b)
 
 
 def process_colors(
     colors: Sequence,
-    count: int
+    count: int,
+    rng: Optional[int] = None
 ) -> List[Color]:
     if type(colors) is str:
         if colors == 'random':
-            colors = [random_color() for _ in range(count)]
+            colors = [random_color(rng) for _ in range(count)]
         elif colors == 'distinct':
-            colors = convert_colors(get_distict_colors(count))
+            colors = convert_colors(get_distict_colors(count, rng=rng))
         elif colors == 'wheel':
             colors = convert_colors(get_wheel_colors(count))
         else:
             raise ValueError('str must be "random", "distinct", or "wheel"')
     else:
         colors = convert_colors(colors)
     return colors
```

### Comparing `landfall-0.3.4/src/landfall/colorsys.py` & `landfall-0.3.5/src/landfall/colorsys.py`

 * *Files identical despite different names*

### Comparing `landfall-0.3.4/src/landfall/combos.py` & `landfall-0.3.5/src/landfall/combos.py`

 * *Files identical despite different names*

### Comparing `landfall-0.3.4/src/landfall/points.py` & `landfall-0.3.5/src/landfall/points.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """
 Functions for plotting points.
 """
 from typing import Mapping, Optional, Sequence, Tuple, Union
-from itertools import repeat
 
 import staticmaps
 from PIL.Image import Image
 
-from landfall.color import process_colors, process_id_colors
+from landfall.plot import plot_colors, plot_zoom
 
 
 tp = staticmaps.tile_provider_OSM
 
 
 def plot_points(
     latitudes: Sequence,
@@ -29,57 +28,82 @@
     flip_coords=False,
     context: Optional[staticmaps.Context] = None
 ) -> Image:
     if context is None:
         context = staticmaps.Context()
 
     context.set_tile_provider(tile_provider)
+
+    add_points(
+        context=context,
+        latitudes=latitudes,
+        longitudes=longitudes,
+        colors=colors,
+        ids=ids,
+        id_colors=id_colors,
+        point_size=point_size,
+        color=color,
+        flip_coords=flip_coords
+    )
+
+    zoom = plot_zoom(context, window_size, zoom, set_zoom)
+    context.set_zoom(zoom)
+    
+    return context.render_pillow(*window_size) # type: ignore
+
+
+def add_points(
+    context: staticmaps.Context,
+    latitudes: Sequence,
+    longitudes: Optional[Sequence] = None,
+    *,
+    colors: Optional[Union[Sequence, str]] = None,
+    ids: Optional[Sequence] = None,
+    id_colors: Optional[Union[Mapping, str]] = None,
+    point_size=10,
+    color=staticmaps.color.BLUE,
+    flip_coords=False,
+) -> None:
     count = len(latitudes)
 
+    colors = plot_colors(
+        count=count,
+        colors=colors,
+        ids=ids,
+        id_colors=id_colors,
+        color=color
+    )
+
     if longitudes is None:
         latitudes, longitudes = points_to_lats_lons(latitudes)
 
     if flip_coords:
         latitudes, longitudes = longitudes, latitudes
 
-    if colors is not None:
-        colors = process_colors(colors, count)
-    else:
-        colors = list(repeat(color, count))
-
-    if ids is not None and id_colors is not None:
-        colors = process_id_colors(ids, id_colors)
-
     for lat, lon, clr in zip(latitudes, longitudes, colors):
         add_point(context, lat, lon, clr, point_size)
 
-    _, _zoom = context.determine_center_zoom(*window_size)
-    if _zoom is not None:
-        context.set_zoom(_zoom + zoom)
-
-    if set_zoom is not None:
-        context.set_zoom(set_zoom)
-    
-    return context.render_pillow(*window_size) # type: ignore
     
 
 def plot_points_data(
     data: Mapping[str, Sequence],
     latitude_name: str,
     longitude_name: str,
+    *,
     color_name: Optional[str] = None,
-    colors: Optional[str] = None,
     ids_name: Optional[str] = None,
     id_colors: Optional[Union[Mapping, str]] = None,
+    colors: Optional[str] = None,
     tile_provider=tp,
     point_size=10,
     window_size=(500, 400),
     zoom=0,
     color=staticmaps.color.BLUE,
     set_zoom=None,
+    flip_coords=False,
     context: Optional[staticmaps.Context] = None
 ) -> Image:
     lats = data[latitude_name]
     lons = data[longitude_name]
     colors_values = None if color_name is None else data[color_name]
     if colors_values is None and colors is not None:
         colors_values = colors
@@ -93,15 +117,17 @@
         id_colors=id_colors,
         tile_provider=tile_provider,
         point_size=point_size,
         window_size=window_size,
         zoom=zoom,
         color=color,
         set_zoom=set_zoom,
-        context=context)
+        flip_coords=flip_coords,
+        context=context
+    )
 
 
 def points_to_lats_lons(
     points: Sequence[Sequence[float]]
 ) -> Tuple[Sequence[float], Sequence[float]]:
     latitudes, longitudes = zip(*points)
     return latitudes, longitudes
@@ -117,21 +143,8 @@
     lat: float,
     lon: float,
     color: staticmaps.Color = staticmaps.color.BLUE,
     point_size: int = 10
 ) -> None:
     point = staticmaps.create_latlng(lat, lon)
     marker = staticmaps.Marker(point, color=color, size=point_size)
-    context.add_object(marker)
-
-
-def add_points(
-        context: staticmaps.Context,
-        latitudes: Sequence[float],
-        longitudes: Sequence[float],
-        colors: Optional[Sequence[staticmaps.Color]] = None,
-        point_size: int = 10
-) -> None:
-    if colors is None:
-        colors = list(repeat(staticmaps.color.BLUE, len(latitudes)))
-    for lat, lon, clr in zip(latitudes, longitudes, colors):
-        add_point(context, lat, lon, clr, point_size)
+    context.add_object(marker)
```

### Comparing `landfall-0.3.4/src/landfall.egg-info/PKG-INFO` & `landfall-0.3.5/src/landfall.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: landfall
-Version: 0.3.4
+Version: 0.3.5
 Summary: Easy to use functions to plot geospatial data on maps using staticmaps.
 Author: Odos Matthews
 License: MIT
 Platform: unix
 Platform: linux
 Platform: osx
 Platform: cygwin
```

