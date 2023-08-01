# Comparing `tmp/nonebot_plugin_pjsk-0.2.3.tar.gz` & `tmp/nonebot_plugin_pjsk-0.2.3.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_pjsk-0.2.3.tar", last modified: Tue Aug  1 12:36:54 2023, max compression
+gzip compressed data, was "nonebot_plugin_pjsk-0.2.3.post1.tar", last modified: Tue Aug  1 15:30:59 2023, max compression
```

## Comparing `nonebot_plugin_pjsk-0.2.3.tar` & `nonebot_plugin_pjsk-0.2.3.post1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1070 2023-08-01 12:36:31.066187 nonebot_plugin_pjsk-0.2.3/LICENSE
--rw-r--r--   0        0        0     4076 2023-08-01 12:36:31.066187 nonebot_plugin_pjsk-0.2.3/README.md
--rw-r--r--   0        0        0      889 2023-08-01 12:36:31.142187 nonebot_plugin_pjsk-0.2.3/nonebot_plugin_pjsk/__init__.py
--rw-r--r--   0        0        0     8436 2023-08-01 12:36:31.142187 nonebot_plugin_pjsk-0.2.3/nonebot_plugin_pjsk/__main__.py
--rw-r--r--   0        0        0     1163 2023-08-01 12:36:31.142187 nonebot_plugin_pjsk-0.2.3/nonebot_plugin_pjsk/config.py
--rw-r--r--   0        0        0    11101 2023-08-01 12:36:31.142187 nonebot_plugin_pjsk-0.2.3/nonebot_plugin_pjsk/draw.py
--rw-r--r--   0        0        0     4002 2023-08-01 12:36:31.142187 nonebot_plugin_pjsk-0.2.3/nonebot_plugin_pjsk/resource.py
--rw-r--r--   0        0        0     2351 2023-08-01 12:36:31.142187 nonebot_plugin_pjsk-0.2.3/nonebot_plugin_pjsk/utils.py
--rw-r--r--   0        0        0     1787 2023-08-01 12:36:54.346318 nonebot_plugin_pjsk-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     5067 1970-01-01 00:00:00.000000 nonebot_plugin_pjsk-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-08-01 15:30:39.668224 nonebot_plugin_pjsk-0.2.3.post1/LICENSE
+-rw-r--r--   0        0        0     4076 2023-08-01 15:30:39.668224 nonebot_plugin_pjsk-0.2.3.post1/README.md
+-rw-r--r--   0        0        0      889 2023-08-01 15:30:39.744227 nonebot_plugin_pjsk-0.2.3.post1/nonebot_plugin_pjsk/__init__.py
+-rw-r--r--   0        0        0     8436 2023-08-01 15:30:39.744227 nonebot_plugin_pjsk-0.2.3.post1/nonebot_plugin_pjsk/__main__.py
+-rw-r--r--   0        0        0     1163 2023-08-01 15:30:39.744227 nonebot_plugin_pjsk-0.2.3.post1/nonebot_plugin_pjsk/config.py
+-rw-r--r--   0        0        0    11099 2023-08-01 15:30:39.744227 nonebot_plugin_pjsk-0.2.3.post1/nonebot_plugin_pjsk/draw.py
+-rw-r--r--   0        0        0     4002 2023-08-01 15:30:39.744227 nonebot_plugin_pjsk-0.2.3.post1/nonebot_plugin_pjsk/resource.py
+-rw-r--r--   0        0        0     2351 2023-08-01 15:30:39.744227 nonebot_plugin_pjsk-0.2.3.post1/nonebot_plugin_pjsk/utils.py
+-rw-r--r--   0        0        0     1793 2023-08-01 15:30:59.033798 nonebot_plugin_pjsk-0.2.3.post1/pyproject.toml
+-rw-r--r--   0        0        0     5073 1970-01-01 00:00:00.000000 nonebot_plugin_pjsk-0.2.3.post1/PKG-INFO
```

### Comparing `nonebot_plugin_pjsk-0.2.3/LICENSE` & `nonebot_plugin_pjsk-0.2.3.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pjsk-0.2.3/README.md` & `nonebot_plugin_pjsk-0.2.3.post1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pjsk-0.2.3/nonebot_plugin_pjsk/__init__.py` & `nonebot_plugin_pjsk-0.2.3.post1/nonebot_plugin_pjsk/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pjsk-0.2.3/nonebot_plugin_pjsk/__main__.py` & `nonebot_plugin_pjsk-0.2.3.post1/nonebot_plugin_pjsk/__main__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pjsk-0.2.3/nonebot_plugin_pjsk/config.py` & `nonebot_plugin_pjsk-0.2.3.post1/nonebot_plugin_pjsk/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pjsk-0.2.3/nonebot_plugin_pjsk/draw.py` & `nonebot_plugin_pjsk-0.2.3.post1/nonebot_plugin_pjsk/draw.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,16 +54,16 @@
 DEFAULT_FONT_WEIGHT = 700
 DEFAULT_STROKE_WIDTH = 9
 DEFAULT_LINE_SPACING = 1.3
 
 CANVAS_SIZE = (296, 256)
 MAX_TEXT_IMAGE_SIZE = 2048
 
-ONE_DARK_BLACK = "282c34"
-ONE_DARK_WHITE = "abb2bf"
+ONE_DARK_BLACK = "#282c34"
+ONE_DARK_WHITE = "#abb2bf"
 
 
 class TextTooLargeError(ValueError):
     pass
 
 
 def ensure_font() -> Font:
@@ -319,26 +319,26 @@
                 else " "
             )
             for x in text.splitlines()
         )
     ]
     size = text_size_multiline(wrapped, font_size, font, line_spacing)
 
-    canvas = Canvas(width, size[1] + padding * 2, Color.from_hex(ONE_DARK_BLACK))
+    canvas = Canvas(width, size[1] + padding * 2, hex_to_color(ONE_DARK_BLACK))
     draw_text_multiline(
         canvas,
         wrapped,
         padding,
         padding,
         0,
         0,
         400,
         font_size,
         font,
-        Paint(Color.from_hex(ONE_DARK_WHITE)),
+        Paint(hex_to_color(ONE_DARK_WHITE)),
         line_spacing,
     )
 
     return canvas.to_image()
 
 
 @overload
```

### Comparing `nonebot_plugin_pjsk-0.2.3/nonebot_plugin_pjsk/resource.py` & `nonebot_plugin_pjsk-0.2.3.post1/nonebot_plugin_pjsk/resource.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pjsk-0.2.3/nonebot_plugin_pjsk/utils.py` & `nonebot_plugin_pjsk-0.2.3.post1/nonebot_plugin_pjsk/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pjsk-0.2.3/pyproject.toml` & `nonebot_plugin_pjsk-0.2.3.post1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-pjsk"
-version = "0.2.3"
+version = "0.2.3.post1"
 description = "Project Sekai Sticker Creator for NoneBot2."
 authors = [
     { name = "Agnes_Digital", email = "Z735803792@163.com" },
     { name = "student_2333", email = "lgc2333@126.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0",
```

### Comparing `nonebot_plugin_pjsk-0.2.3/PKG-INFO` & `nonebot_plugin_pjsk-0.2.3.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-pjsk
-Version: 0.2.3
+Version: 0.2.3.post1
 Summary: Project Sekai Sticker Creator for NoneBot2.
 Keywords: pjsk nonebot2 plugin
 Home-page: https://github.com/Agnes4m/nonebot_plugin_pjsk
 Author-Email: Agnes_Digital <Z735803792@163.com>, student_2333 <lgc2333@126.com>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,10 +1,11 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-pjsk Version: 0.2.3 Summary: Project
-Sekai Sticker Creator for NoneBot2. Keywords: pjsk nonebot2 plugin Home-page:
-https://github.com/Agnes4m/nonebot_plugin_pjsk Author-Email: Agnes_Digital
+Metadata-Version: 2.1 Name: nonebot-plugin-pjsk Version: 0.2.3.post1 Summary:
+Project Sekai Sticker Creator for NoneBot2. Keywords: pjsk nonebot2 plugin
+Home-page: https://github.com/Agnes4m/nonebot_plugin_pjsk Author-Email:
+Agnes_Digital
 163.com>, student_2333
 126.com> License: MIT Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Operating System :: OS Independent Project-URL:
 Homepage, https://github.com/Agnes4m/nonebot_plugin_pjsk Requires-Python:
```

