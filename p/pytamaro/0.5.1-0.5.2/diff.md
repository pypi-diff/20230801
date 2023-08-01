# Comparing `tmp/pytamaro-0.5.1.tar.gz` & `tmp/pytamaro-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytamaro-0.5.1.tar", max compression
+gzip compressed data, was "pytamaro-0.5.2.tar", max compression
```

## Comparing `pytamaro-0.5.1.tar` & `pytamaro-0.5.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1103 2022-03-04 16:39:39.043278 pytamaro-0.5.1/LICENSE
--rw-r--r--   0        0        0      818 2023-06-03 07:06:56.646268 pytamaro-0.5.1/pyproject.toml
--rw-r--r--   0        0        0      472 2023-06-03 07:06:56.651499 pytamaro-0.5.1/pytamaro/__init__.py
--rw-r--r--   0        0        0     3659 2023-02-27 12:54:43.437950 pytamaro-0.5.1/pytamaro/checks.py
--rw-r--r--   0        0        0      962 2023-02-27 12:54:43.438236 pytamaro-0.5.1/pytamaro/color.py
--rw-r--r--   0        0        0     4641 2023-02-27 12:54:43.438488 pytamaro-0.5.1/pytamaro/color_functions.py
--rw-r--r--   0        0        0      799 2023-02-27 12:54:43.438694 pytamaro-0.5.1/pytamaro/color_names.py
--rw-r--r--   0        0        0      456 2023-02-27 12:54:43.439015 pytamaro-0.5.1/pytamaro/de/__init__.py
--rw-r--r--   0        0        0     3948 2023-02-27 12:54:43.439329 pytamaro-0.5.1/pytamaro/de/color.py
--rw-r--r--   0        0        0     1093 2022-03-04 16:39:39.049297 pytamaro-0.5.1/pytamaro/de/color_names.py
--rw-r--r--   0        0        0      445 2023-02-27 12:54:43.439701 pytamaro-0.5.1/pytamaro/de/graphic.py
--rw-r--r--   0        0        0     3211 2023-05-29 08:23:29.417046 pytamaro-0.5.1/pytamaro/de/io.py
--rw-r--r--   0        0        0     4206 2023-02-27 12:54:43.440314 pytamaro-0.5.1/pytamaro/de/operations.py
--rw-r--r--   0        0        0      119 2023-02-27 12:54:43.440547 pytamaro-0.5.1/pytamaro/de/point.py
--rw-r--r--   0        0        0     1364 2023-02-27 12:54:43.440806 pytamaro-0.5.1/pytamaro/de/point_names.py
--rw-r--r--   0        0        0     4626 2023-02-27 12:54:43.441003 pytamaro-0.5.1/pytamaro/de/primitives.py
--rw-r--r--   0        0        0     2643 2023-02-27 12:54:43.441184 pytamaro-0.5.1/pytamaro/debug.py
--rw-r--r--   0        0        0     8147 2023-06-02 09:48:23.048575 pytamaro-0.5.1/pytamaro/graphic.py
--rw-r--r--   0        0        0     9313 2023-06-03 06:56:26.725254 pytamaro-0.5.1/pytamaro/io.py
--rw-r--r--   0        0        0      457 2023-02-27 12:54:43.441979 pytamaro-0.5.1/pytamaro/it/__init__.py
--rw-r--r--   0        0        0     3370 2023-02-27 12:54:43.442282 pytamaro-0.5.1/pytamaro/it/color.py
--rw-r--r--   0        0        0      923 2022-11-30 08:45:09.899740 pytamaro-0.5.1/pytamaro/it/color_names.py
--rw-r--r--   0        0        0      459 2023-02-27 12:54:43.442558 pytamaro-0.5.1/pytamaro/it/graphic.py
--rw-r--r--   0        0        0     2949 2023-05-29 08:23:29.417817 pytamaro-0.5.1/pytamaro/it/io.py
--rw-r--r--   0        0        0     4512 2023-02-27 12:54:43.442887 pytamaro-0.5.1/pytamaro/it/operations.py
--rw-r--r--   0        0        0      111 2023-02-27 12:54:43.443014 pytamaro-0.5.1/pytamaro/it/point.py
--rw-r--r--   0        0        0     1626 2023-02-27 12:54:43.443240 pytamaro-0.5.1/pytamaro/it/point_names.py
--rw-r--r--   0        0        0     4636 2023-02-27 12:54:43.443425 pytamaro-0.5.1/pytamaro/it/primitives.py
--rw-r--r--   0        0        0     5786 2023-02-27 12:54:43.443621 pytamaro-0.5.1/pytamaro/localization.py
--rw-r--r--   0        0        0     5834 2023-02-27 12:54:43.443786 pytamaro-0.5.1/pytamaro/operations.py
--rw-r--r--   0        0        0     1900 2023-02-27 12:54:43.443994 pytamaro-0.5.1/pytamaro/point.py
--rw-r--r--   0        0        0     1233 2023-02-27 12:54:43.444184 pytamaro-0.5.1/pytamaro/point_names.py
--rw-r--r--   0        0        0     4997 2023-02-27 12:54:43.444392 pytamaro-0.5.1/pytamaro/primitives.py
--rw-r--r--   0        0        0        0 2022-10-31 08:45:16.764275 pytamaro-0.5.1/pytamaro/py.typed
--rw-r--r--   0        0        0     1032 2023-05-29 08:23:29.418250 pytamaro-0.5.1/pytamaro/utils.py
--rw-r--r--   0        0        0      539 1970-01-01 00:00:00.000000 pytamaro-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1103 2022-03-04 16:39:39.043278 pytamaro-0.5.2/LICENSE
+-rw-r--r--   0        0        0      887 2023-08-01 09:10:46.945046 pytamaro-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0      472 2023-08-01 09:10:46.950104 pytamaro-0.5.2/pytamaro/__init__.py
+-rw-r--r--   0        0        0     3659 2023-02-27 12:54:43.437950 pytamaro-0.5.2/pytamaro/checks.py
+-rw-r--r--   0        0        0      962 2023-02-27 12:54:43.438236 pytamaro-0.5.2/pytamaro/color.py
+-rw-r--r--   0        0        0     4641 2023-02-27 12:54:43.438488 pytamaro-0.5.2/pytamaro/color_functions.py
+-rw-r--r--   0        0        0      799 2023-02-27 12:54:43.438694 pytamaro-0.5.2/pytamaro/color_names.py
+-rw-r--r--   0        0        0      456 2023-02-27 12:54:43.439015 pytamaro-0.5.2/pytamaro/de/__init__.py
+-rw-r--r--   0        0        0     3948 2023-02-27 12:54:43.439329 pytamaro-0.5.2/pytamaro/de/color.py
+-rw-r--r--   0        0        0     1093 2022-03-04 16:39:39.049297 pytamaro-0.5.2/pytamaro/de/color_names.py
+-rw-r--r--   0        0        0      445 2023-02-27 12:54:43.439701 pytamaro-0.5.2/pytamaro/de/graphic.py
+-rw-r--r--   0        0        0     3211 2023-05-29 08:23:29.417046 pytamaro-0.5.2/pytamaro/de/io.py
+-rw-r--r--   0        0        0     4206 2023-02-27 12:54:43.440314 pytamaro-0.5.2/pytamaro/de/operations.py
+-rw-r--r--   0        0        0      119 2023-02-27 12:54:43.440547 pytamaro-0.5.2/pytamaro/de/point.py
+-rw-r--r--   0        0        0     1364 2023-02-27 12:54:43.440806 pytamaro-0.5.2/pytamaro/de/point_names.py
+-rw-r--r--   0        0        0     4626 2023-02-27 12:54:43.441003 pytamaro-0.5.2/pytamaro/de/primitives.py
+-rw-r--r--   0        0        0     2643 2023-02-27 12:54:43.441184 pytamaro-0.5.2/pytamaro/debug.py
+-rw-r--r--   0        0        0     8157 2023-07-26 12:01:25.982000 pytamaro-0.5.2/pytamaro/graphic.py
+-rw-r--r--   0        0        0     9529 2023-08-01 09:04:29.004332 pytamaro-0.5.2/pytamaro/io.py
+-rw-r--r--   0        0        0      457 2023-02-27 12:54:43.441979 pytamaro-0.5.2/pytamaro/it/__init__.py
+-rw-r--r--   0        0        0     3370 2023-02-27 12:54:43.442282 pytamaro-0.5.2/pytamaro/it/color.py
+-rw-r--r--   0        0        0      923 2022-11-30 08:45:09.899740 pytamaro-0.5.2/pytamaro/it/color_names.py
+-rw-r--r--   0        0        0      459 2023-02-27 12:54:43.442558 pytamaro-0.5.2/pytamaro/it/graphic.py
+-rw-r--r--   0        0        0     2949 2023-05-29 08:23:29.417817 pytamaro-0.5.2/pytamaro/it/io.py
+-rw-r--r--   0        0        0     4512 2023-02-27 12:54:43.442887 pytamaro-0.5.2/pytamaro/it/operations.py
+-rw-r--r--   0        0        0      111 2023-02-27 12:54:43.443014 pytamaro-0.5.2/pytamaro/it/point.py
+-rw-r--r--   0        0        0     1626 2023-02-27 12:54:43.443240 pytamaro-0.5.2/pytamaro/it/point_names.py
+-rw-r--r--   0        0        0     4636 2023-02-27 12:54:43.443425 pytamaro-0.5.2/pytamaro/it/primitives.py
+-rw-r--r--   0        0        0     5786 2023-02-27 12:54:43.443621 pytamaro-0.5.2/pytamaro/localization.py
+-rw-r--r--   0        0        0     5834 2023-02-27 12:54:43.443786 pytamaro-0.5.2/pytamaro/operations.py
+-rw-r--r--   0        0        0     1900 2023-02-27 12:54:43.443994 pytamaro-0.5.2/pytamaro/point.py
+-rw-r--r--   0        0        0     1233 2023-02-27 12:54:43.444184 pytamaro-0.5.2/pytamaro/point_names.py
+-rw-r--r--   0        0        0     4997 2023-02-27 12:54:43.444392 pytamaro-0.5.2/pytamaro/primitives.py
+-rw-r--r--   0        0        0        0 2022-10-31 08:45:16.764275 pytamaro-0.5.2/pytamaro/py.typed
+-rw-r--r--   0        0        0     1032 2023-05-29 08:23:29.418250 pytamaro-0.5.2/pytamaro/utils.py
+-rw-r--r--   0        0        0      544 1970-01-01 00:00:00.000000 pytamaro-0.5.2/PKG-INFO
```

### Comparing `pytamaro-0.5.1/LICENSE` & `pytamaro-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytamaro-0.5.1/pyproject.toml` & `pytamaro-0.5.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 [tool.poetry]
 name = "pytamaro"
-version = "0.5.1"
+version = "0.5.2"
 description = "Educational library for teaching problem decompositon using graphics"
 authors = ["Luca Chiodini <luca@chiodini.org>"]
 
 [tool.poetry.dependencies]
-python = ">=3.8"
+python = ">=3.8,<4.0"
 Pillow = "^9.0.0"
 skia-python = "^87.4"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.5"
 pytest-watch = "^4.2.0"
 pytest-cov = "^3.0.0"
 pylint = "^2.12.2"
 pycodestyle = "^2.8.0"
 Sphinx = "^5.2.3"
 sphinx-rtd-theme = "^1.0.0"
 pyright = "^0.0.13"
 
+[tool.poetry.group.dev.dependencies]
+sphinx-toolbox = "^3.5.0"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pyright]
 include = ["pytamaro", "tests"]
```

### Comparing `pytamaro-0.5.1/pytamaro/checks.py` & `pytamaro-0.5.2/pytamaro/checks.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.5.1/pytamaro/color.py` & `pytamaro-0.5.2/pytamaro/color.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.5.1/pytamaro/color_functions.py` & `pytamaro-0.5.2/pytamaro/color_functions.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.5.1/pytamaro/color_names.py` & `pytamaro-0.5.2/pytamaro/color_names.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.5.1/pytamaro/de/color.py` & `pytamaro-0.5.2/pytamaro/de/color.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.5.1/pytamaro/de/color_names.py` & `pytamaro-0.5.2/pytamaro/de/color_names.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.5.1/pytamaro/de/io.py` & `pytamaro-0.5.2/pytamaro/de/io.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.5.1/pytamaro/de/operations.py` & `pytamaro-0.5.2/pytamaro/de/operations.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.5.1/pytamaro/de/point_names.py` & `pytamaro-0.5.2/pytamaro/de/point_names.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.5.1/pytamaro/de/primitives.py` & `pytamaro-0.5.2/pytamaro/de/primitives.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.5.1/pytamaro/debug.py` & `pytamaro-0.5.2/pytamaro/debug.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.5.1/pytamaro/graphic.py` & `pytamaro-0.5.2/pytamaro/graphic.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
 class CircularSector(Primitive):
     """
     A circular sector (with an angle between 0 and 360).
     Its pinning position is the center of the circle from which it is taken.
     """
     def __init__(self, radius: float, angle: float, color: Color):
         if angle == 360:
-            path = Path.Circle(0, 0, radius)
+            path = Path.Circle(radius, radius, radius)
         else:
             diameter = 2 * radius
             path = Path()
             path.moveTo(radius, radius)
             path.arcTo(Rect.MakeWH(diameter, diameter), 0, -angle, False)
             path.close()
         super().__init__(path, color)
```

### Comparing `pytamaro-0.5.1/pytamaro/io.py` & `pytamaro-0.5.2/pytamaro/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Functions for output (show or save) of graphics.
 """
 
 import base64
 import io
 import os
 import re
-from pathlib import Path
 import subprocess
 import sys
+from pathlib import Path
 from tempfile import NamedTemporaryFile
 from typing import List
 
 from PIL import Image as PILImageMod
 from PIL.Image import Image as PILImage
 from skia import Canvas, FILEWStream, Image, Rect, Surface, SVGCanvas, kPNG
 
@@ -62,21 +62,26 @@
     """
     size = graphic.size()
     stream = FILEWStream(filename)
     canvas = SVGCanvas.Make(Rect.MakeSize(size), stream)
     _draw_to_canvas(canvas, graphic)
     del canvas
     stream.flush()
+    stream.fsync()
     # Manually add shape-rendering="crispEdges" to the SVG file.
     # We don't use the XML parser from the standard library because,
     # among other aspects, it does not properly maintain the doctype.
+    # We also manually add `fill="none"` to the root `svg` element to ensure
+    # that renderers always use a transparent background.
     with open(filename, "r", encoding="utf-8") as file:
         content = file.read()
     # `svg` tag may be self-closing
-    new_content = re.sub("<svg(.*?)(/?)>", r'<svg\1 shape-rendering="crispEdges"\2>', content)
+    new_content = re.sub("<svg(.*?)(/?)>",
+                         r'<svg\1 shape-rendering="crispEdges" fill="none"\2>',
+                         content)
     with open(filename, "w", encoding="utf-8") as file:
         file.write(new_content)
 
 
 def graphic_to_image(graphic: Graphic) -> Image:
     """
     Renders a graphic into a Skia image.
```

### Comparing `pytamaro-0.5.1/pytamaro/it/color.py` & `pytamaro-0.5.2/pytamaro/it/color.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.5.1/pytamaro/it/color_names.py` & `pytamaro-0.5.2/pytamaro/it/color_names.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.5.1/pytamaro/it/io.py` & `pytamaro-0.5.2/pytamaro/it/io.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.5.1/pytamaro/it/operations.py` & `pytamaro-0.5.2/pytamaro/it/operations.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.5.1/pytamaro/it/point_names.py` & `pytamaro-0.5.2/pytamaro/it/point_names.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.5.1/pytamaro/it/primitives.py` & `pytamaro-0.5.2/pytamaro/it/primitives.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.5.1/pytamaro/localization.py` & `pytamaro-0.5.2/pytamaro/localization.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.5.1/pytamaro/operations.py` & `pytamaro-0.5.2/pytamaro/operations.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.5.1/pytamaro/point.py` & `pytamaro-0.5.2/pytamaro/point.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.5.1/pytamaro/point_names.py` & `pytamaro-0.5.2/pytamaro/point_names.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.5.1/pytamaro/primitives.py` & `pytamaro-0.5.2/pytamaro/primitives.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.5.1/pytamaro/utils.py` & `pytamaro-0.5.2/pytamaro/utils.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.5.1/PKG-INFO` & `pytamaro-0.5.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: pytamaro
-Version: 0.5.1
+Version: 0.5.2
 Summary: Educational library for teaching problem decompositon using graphics
 Author: Luca Chiodini
 Author-email: luca@chiodini.org
-Requires-Python: >=3.8
+Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Pillow (>=9.0.0,<10.0.0)
 Requires-Dist: skia-python (>=87.4,<88.0)
```

