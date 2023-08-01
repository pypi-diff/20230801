# Comparing `tmp/nonebot_plugin_remake-0.3.1.tar.gz` & `tmp/nonebot_plugin_remake-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_remake-0.3.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_remake-0.3.2.tar", max compression
```

## Comparing `nonebot_plugin_remake-0.3.1.tar` & `nonebot_plugin_remake-0.3.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1063 2023-08-01 18:55:17.171814 nonebot_plugin_remake-0.3.1/LICENSE
--rw-r--r--   0        0        0     1164 2023-08-01 18:55:17.171814 nonebot_plugin_remake-0.3.1/README.md
--rw-r--r--   0        0        0     7728 2023-08-01 18:55:17.171814 nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/__init__.py
--rw-r--r--   0        0        0      679 2023-08-01 18:55:17.171814 nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/age.py
--rw-r--r--   0        0        0      127 2023-08-01 18:55:17.171814 nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/config.py
--rw-r--r--   0        0        0    11874 2023-08-01 18:55:17.171814 nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/drawer.py
--rw-r--r--   0        0        0     3138 2023-08-01 18:55:17.171814 nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/event.py
--rw-r--r--   0        0        0     2596 2023-08-01 18:55:17.171814 nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/life.py
--rw-r--r--   0        0        0     6700 2023-08-01 18:55:17.171814 nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/property.py
--rw-r--r--   0        0        0  1967733 2023-08-01 18:55:17.179814 nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/resources/data/age.json
--rw-r--r--   0        0        0   377196 2023-08-01 18:55:17.179814 nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/resources/data/events.json
--rw-r--r--   0        0        0    29584 2023-08-01 18:55:17.179814 nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/resources/data/talents.json
--rw-r--r--   0        0        0  1895036 2023-08-01 18:55:17.187814 nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/resources/fonts/方正像素12.ttf
--rw-r--r--   0        0        0     9336 2023-08-01 18:55:17.187814 nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/resources/images/bg_summary.png
--rw-r--r--   0        0        0     6810 2023-08-01 18:55:17.187814 nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/resources/images/bg_talent.png
--rw-r--r--   0        0        0     4590 2023-08-01 18:55:17.187814 nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/resources/images/icon_chr.png
--rw-r--r--   0        0        0     1586 2023-08-01 18:55:17.187814 nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/resources/images/icon_int.png
--rw-r--r--   0        0        0      904 2023-08-01 18:55:17.187814 nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/resources/images/icon_mny.png
--rw-r--r--   0        0        0     3319 2023-08-01 18:55:17.187814 nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/resources/images/icon_spr.png
--rw-r--r--   0        0        0     2873 2023-08-01 18:55:17.187814 nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/resources/images/icon_str.png
--rw-r--r--   0        0        0      195 2023-08-01 18:55:17.187814 nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/resources/images/title_left.png
--rw-r--r--   0        0        0      208 2023-08-01 18:55:17.187814 nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/resources/images/title_right.png
--rw-r--r--   0        0        0    86169 2023-08-01 18:55:17.187814 nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/resources/images/titlebar.png
--rw-r--r--   0        0        0     3258 2023-08-01 18:55:17.187814 nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/talent.py
--rw-r--r--   0        0        0      960 2023-08-01 18:55:17.187814 nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/utils.py
--rw-r--r--   0        0        0      691 2023-08-01 18:55:17.191814 nonebot_plugin_remake-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     2064 1970-01-01 00:00:00.000000 nonebot_plugin_remake-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-08-01 19:30:35.693543 nonebot_plugin_remake-0.3.2/LICENSE
+-rw-r--r--   0        0        0     1164 2023-08-01 19:30:35.693543 nonebot_plugin_remake-0.3.2/README.md
+-rw-r--r--   0        0        0     7728 2023-08-01 19:30:35.693543 nonebot_plugin_remake-0.3.2/nonebot_plugin_remake/__init__.py
+-rw-r--r--   0        0        0      679 2023-08-01 19:30:35.693543 nonebot_plugin_remake-0.3.2/nonebot_plugin_remake/age.py
+-rw-r--r--   0        0        0      127 2023-08-01 19:30:35.693543 nonebot_plugin_remake-0.3.2/nonebot_plugin_remake/config.py
+-rw-r--r--   0        0        0    12054 2023-08-01 19:30:35.693543 nonebot_plugin_remake-0.3.2/nonebot_plugin_remake/drawer.py
+-rw-r--r--   0        0        0     3138 2023-08-01 19:30:35.693543 nonebot_plugin_remake-0.3.2/nonebot_plugin_remake/event.py
+-rw-r--r--   0        0        0     2596 2023-08-01 19:30:35.693543 nonebot_plugin_remake-0.3.2/nonebot_plugin_remake/life.py
+-rw-r--r--   0        0        0     6700 2023-08-01 19:30:35.693543 nonebot_plugin_remake-0.3.2/nonebot_plugin_remake/property.py
+-rw-r--r--   0        0        0  1967733 2023-08-01 19:30:35.701543 nonebot_plugin_remake-0.3.2/nonebot_plugin_remake/resources/data/age.json
+-rw-r--r--   0        0        0   377196 2023-08-01 19:30:35.701543 nonebot_plugin_remake-0.3.2/nonebot_plugin_remake/resources/data/events.json
+-rw-r--r--   0        0        0    29584 2023-08-01 19:30:35.701543 nonebot_plugin_remake-0.3.2/nonebot_plugin_remake/resources/data/talents.json
+-rw-r--r--   0        0        0  1895036 2023-08-01 19:30:35.709543 nonebot_plugin_remake-0.3.2/nonebot_plugin_remake/resources/fonts/方正像素12.ttf
+-rw-r--r--   0        0        0     9336 2023-08-01 19:30:35.709543 nonebot_plugin_remake-0.3.2/nonebot_plugin_remake/resources/images/bg_summary.png
+-rw-r--r--   0        0        0     6810 2023-08-01 19:30:35.709543 nonebot_plugin_remake-0.3.2/nonebot_plugin_remake/resources/images/bg_talent.png
+-rw-r--r--   0        0        0     4590 2023-08-01 19:30:35.709543 nonebot_plugin_remake-0.3.2/nonebot_plugin_remake/resources/images/icon_chr.png
+-rw-r--r--   0        0        0     1586 2023-08-01 19:30:35.709543 nonebot_plugin_remake-0.3.2/nonebot_plugin_remake/resources/images/icon_int.png
+-rw-r--r--   0        0        0      904 2023-08-01 19:30:35.709543 nonebot_plugin_remake-0.3.2/nonebot_plugin_remake/resources/images/icon_mny.png
+-rw-r--r--   0        0        0     3319 2023-08-01 19:30:35.709543 nonebot_plugin_remake-0.3.2/nonebot_plugin_remake/resources/images/icon_spr.png
+-rw-r--r--   0        0        0     2873 2023-08-01 19:30:35.709543 nonebot_plugin_remake-0.3.2/nonebot_plugin_remake/resources/images/icon_str.png
+-rw-r--r--   0        0        0      195 2023-08-01 19:30:35.709543 nonebot_plugin_remake-0.3.2/nonebot_plugin_remake/resources/images/title_left.png
+-rw-r--r--   0        0        0      208 2023-08-01 19:30:35.709543 nonebot_plugin_remake-0.3.2/nonebot_plugin_remake/resources/images/title_right.png
+-rw-r--r--   0        0        0    86169 2023-08-01 19:30:35.709543 nonebot_plugin_remake-0.3.2/nonebot_plugin_remake/resources/images/titlebar.png
+-rw-r--r--   0        0        0     3258 2023-08-01 19:30:35.709543 nonebot_plugin_remake-0.3.2/nonebot_plugin_remake/talent.py
+-rw-r--r--   0        0        0      960 2023-08-01 19:30:35.709543 nonebot_plugin_remake-0.3.2/nonebot_plugin_remake/utils.py
+-rw-r--r--   0        0        0      691 2023-08-01 19:30:35.709543 nonebot_plugin_remake-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     2064 1970-01-01 00:00:00.000000 nonebot_plugin_remake-0.3.2/PKG-INFO
```

### Comparing `nonebot_plugin_remake-0.3.1/LICENSE` & `nonebot_plugin_remake-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_remake-0.3.1/README.md` & `nonebot_plugin_remake-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/__init__.py` & `nonebot_plugin_remake-0.3.2/nonebot_plugin_remake/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     homepage="https://github.com/noneplugin/nonebot-plugin-remake",
     config=Config,
     supported_adapters=saa_plugin_meta.supported_adapters,
     extra={
         "unique_name": "remake",
         "example": "@小Q remake",
         "author": "meetwq <meetwq@gmail.com>",
-        "version": "0.3.1",
+        "version": "0.3.2",
     },
 )
 
 remake_config = Config.parse_obj(get_driver().config.dict())
 
 onebot_v11_loaded = False
 if remake_config.remake_send_forword_msg:
```

### Comparing `nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/age.py` & `nonebot_plugin_remake-0.3.2/nonebot_plugin_remake/age.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/drawer.py` & `nonebot_plugin_remake-0.3.2/nonebot_plugin_remake/drawer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from io import BytesIO
 from pathlib import Path
-from typing import List, NamedTuple
+from typing import List, NamedTuple, Optional
 
 from PIL import Image, ImageDraw, ImageFont
 from PIL.Image import Image as IMG
 from PIL.Image import Resampling
 from PIL.ImageFont import FreeTypeFont
 
 from .life import PerAgeProperty, PerAgeResult
@@ -21,14 +21,48 @@
     return ImageFont.truetype(str(font_dir / "方正像素12.ttf"), fontsize)
 
 
 def get_icon(item: str) -> IMG:
     return Image.open(image_dir / f"icon_{item}.png")
 
 
+def break_text(text: str, font: FreeTypeFont, length: int) -> List[str]:
+    lines = []
+    line = ""
+    for word in text:
+        if font.getlength(line + word) > length:
+            lines.append(line)
+            line = ""
+        line += word
+    if line:
+        lines.append(line)
+    return lines
+
+
+def text_to_image(
+    texts: List[str],
+    fontsize: int = 10,
+    fill: str = "black",
+    spacing: int = 4,
+    max_width: Optional[int] = None,
+) -> IMG:
+    font = get_font(fontsize)
+    texts = sum([text.splitlines() for text in texts], [])
+    if max_width:
+        texts = sum([break_text(text, font, max_width) for text in texts], [])
+    max_length = int(max([font.getlength(text) for text in texts]))
+    ascent, descent = font.getmetrics()
+    h = ascent * len(texts) + spacing * (len(texts) - 1) + descent
+    image = Image.new("RGBA", (max_length, h))
+    draw = ImageDraw.Draw(image)
+    text = "\n".join(texts)
+    draw.multiline_text((0, 0), text, font=font, fill=fill, spacing=spacing)
+    return image
+
+
 def draw_init_properties(prop: PerAgeProperty) -> IMG:
     image = Image.new("RGBA", (1250, 84))
     font = get_font(45)
     draw = ImageDraw.Draw(image)
     draw.rounded_rectangle((0, 0, image.width, image.height), 20, "#0A2530")
     x = 0
 
@@ -75,35 +109,20 @@
     draw_property("int", prop.INT)
     draw_property("str", prop.STR)
     draw_property("mny", prop.MNY)
     draw_property("spr", prop.SPR)
     return image
 
 
-def text_to_image(
-    texts: List[str], fontsize: int = 10, fill: str = "black", spacing=4
-) -> IMG:
-    texts = sum([text.splitlines() for text in texts], [])
-    font = get_font(fontsize)
-    max_length = int(max([font.getlength(text) for text in texts]))
-    ascent, descent = font.getmetrics()
-    h = ascent * len(texts) + spacing * (len(texts) - 1) + descent
-    image = Image.new("RGBA", (max_length, h))
-    draw = ImageDraw.Draw(image)
-    text = "\n".join(texts)
-    draw.multiline_text((0, 0), text, font=font, fill=fill, spacing=spacing)
-    return image
-
-
 def draw_age(age: int) -> IMG:
     return text_to_image([f"{age}岁："], fontsize=45, fill="#C3DE5A")
 
 
 def draw_logs(logs: List[str]) -> IMG:
-    return text_to_image(logs, fontsize=45, fill="#F0F2F3", spacing=30)
+    return text_to_image(logs, fontsize=45, fill="#F0F2F3", spacing=30, max_width=1200)
 
 
 def draw_results(results: List[PerAgeResult]) -> IMG:
     class ImageResult(NamedTuple):
         prop: IMG
         age: IMG
         logs: IMG
@@ -286,27 +305,14 @@
     titlebar.paste(
         left, (int((titlebar.width - length) / 2 - left.width - 10), 140), mask=left
     )
     titlebar.paste(right, (int((titlebar.width + length) / 2 + 10), 140), mask=right)
     return titlebar
 
 
-def break_text(text: str, font: FreeTypeFont, length: int) -> List[str]:
-    lines = []
-    line = ""
-    for word in text:
-        if font.getlength(line + word) > length:
-            lines.append(line)
-            line = ""
-        line += word
-    if line:
-        lines.append(line)
-    return lines
-
-
 def draw_talent(talent: Talent) -> IMG:
     bg = Image.open(image_dir / "bg_talent.png")
     font = get_font(45)
     draw = ImageDraw.Draw(bg)
     draw.text((40, 50), talent.name, font=font, fill="white")
     font = get_font(35)
     text = "\n".join(break_text(talent.description, font, 300))
```

### Comparing `nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/event.py` & `nonebot_plugin_remake-0.3.2/nonebot_plugin_remake/event.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/life.py` & `nonebot_plugin_remake-0.3.2/nonebot_plugin_remake/life.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/property.py` & `nonebot_plugin_remake-0.3.2/nonebot_plugin_remake/property.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/resources/data/age.json` & `nonebot_plugin_remake-0.3.2/nonebot_plugin_remake/resources/data/age.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/resources/data/events.json` & `nonebot_plugin_remake-0.3.2/nonebot_plugin_remake/resources/data/events.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/resources/data/talents.json` & `nonebot_plugin_remake-0.3.2/nonebot_plugin_remake/resources/data/talents.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/resources/fonts/方正像素12.ttf` & `nonebot_plugin_remake-0.3.2/nonebot_plugin_remake/resources/fonts/方正像素12.ttf`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/resources/images/bg_summary.png` & `nonebot_plugin_remake-0.3.2/nonebot_plugin_remake/resources/images/bg_summary.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/resources/images/bg_talent.png` & `nonebot_plugin_remake-0.3.2/nonebot_plugin_remake/resources/images/bg_talent.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/resources/images/icon_chr.png` & `nonebot_plugin_remake-0.3.2/nonebot_plugin_remake/resources/images/icon_chr.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/resources/images/icon_int.png` & `nonebot_plugin_remake-0.3.2/nonebot_plugin_remake/resources/images/icon_int.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/resources/images/icon_mny.png` & `nonebot_plugin_remake-0.3.2/nonebot_plugin_remake/resources/images/icon_mny.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/resources/images/icon_spr.png` & `nonebot_plugin_remake-0.3.2/nonebot_plugin_remake/resources/images/icon_spr.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/resources/images/icon_str.png` & `nonebot_plugin_remake-0.3.2/nonebot_plugin_remake/resources/images/icon_str.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/resources/images/titlebar.png` & `nonebot_plugin_remake-0.3.2/nonebot_plugin_remake/resources/images/titlebar.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/talent.py` & `nonebot_plugin_remake-0.3.2/nonebot_plugin_remake/talent.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/utils.py` & `nonebot_plugin_remake-0.3.2/nonebot_plugin_remake/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_remake-0.3.1/pyproject.toml` & `nonebot_plugin_remake-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_remake"
-version = "0.3.1"
+version = "0.3.2"
 description = "适用于 Nonebot2 的人生重开模拟器插件"
 authors = ["meetwq <meetwq@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/noneplugin/nonebot-plugin-remake"
 repository = "https://github.com/noneplugin/nonebot-plugin-remake"
```

### Comparing `nonebot_plugin_remake-0.3.1/PKG-INFO` & `nonebot_plugin_remake-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-remake
-Version: 0.3.1
+Version: 0.3.2
 Summary: 适用于 Nonebot2 的人生重开模拟器插件
 Home-page: https://github.com/noneplugin/nonebot-plugin-remake
 License: MIT
 Author: meetwq
 Author-email: meetwq@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

