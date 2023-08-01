# Comparing `tmp/nonebot_plugin_remake-0.3.0.tar.gz` & `tmp/nonebot_plugin_remake-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_remake-0.3.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_remake-0.3.1.tar", max compression
```

## Comparing `nonebot_plugin_remake-0.3.0.tar` & `nonebot_plugin_remake-0.3.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1063 2023-08-01 18:43:54.668067 nonebot_plugin_remake-0.3.0/LICENSE
--rw-r--r--   0        0        0     1164 2023-08-01 18:43:54.668067 nonebot_plugin_remake-0.3.0/README.md
--rw-r--r--   0        0        0     7728 2023-08-01 18:43:54.668067 nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/__init__.py
--rw-r--r--   0        0        0      679 2023-08-01 18:43:54.668067 nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/age.py
--rw-r--r--   0        0        0      127 2023-08-01 18:43:54.668067 nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/config.py
--rw-r--r--   0        0        0    11874 2023-08-01 18:43:54.668067 nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/drawer.py
--rw-r--r--   0        0        0     3138 2023-08-01 18:43:54.668067 nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/event.py
--rw-r--r--   0        0        0     2596 2023-08-01 18:43:54.668067 nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/life.py
--rw-r--r--   0        0        0     6700 2023-08-01 18:43:54.668067 nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/property.py
--rw-r--r--   0        0        0  1967733 2023-08-01 18:43:54.676067 nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/resources/data/age.json
--rw-r--r--   0        0        0   377196 2023-08-01 18:43:54.676067 nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/resources/data/events.json
--rw-r--r--   0        0        0    29584 2023-08-01 18:43:54.676067 nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/resources/data/talents.json
--rw-r--r--   0        0        0  1895036 2023-08-01 18:43:54.684067 nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/resources/fonts/方正像素12.ttf
--rw-r--r--   0        0        0     9336 2023-08-01 18:43:54.684067 nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/resources/images/bg_summary.png
--rw-r--r--   0        0        0     6810 2023-08-01 18:43:54.684067 nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/resources/images/bg_talent.png
--rw-r--r--   0        0        0     4590 2023-08-01 18:43:54.684067 nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/resources/images/icon_chr.png
--rw-r--r--   0        0        0     1586 2023-08-01 18:43:54.684067 nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/resources/images/icon_int.png
--rw-r--r--   0        0        0      904 2023-08-01 18:43:54.684067 nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/resources/images/icon_mny.png
--rw-r--r--   0        0        0     3319 2023-08-01 18:43:54.684067 nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/resources/images/icon_spr.png
--rw-r--r--   0        0        0     2873 2023-08-01 18:43:54.684067 nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/resources/images/icon_str.png
--rw-r--r--   0        0        0      195 2023-08-01 18:43:54.684067 nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/resources/images/title_left.png
--rw-r--r--   0        0        0      208 2023-08-01 18:43:54.684067 nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/resources/images/title_right.png
--rw-r--r--   0        0        0    86169 2023-08-01 18:43:54.684067 nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/resources/images/titlebar.png
--rw-r--r--   0        0        0     3258 2023-08-01 18:43:54.684067 nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/talent.py
--rw-r--r--   0        0        0      960 2023-08-01 18:43:54.684067 nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/utils.py
--rw-r--r--   0        0        0      664 2023-08-01 18:43:54.684067 nonebot_plugin_remake-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2024 1970-01-01 00:00:00.000000 nonebot_plugin_remake-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-08-01 18:55:17.171814 nonebot_plugin_remake-0.3.1/LICENSE
+-rw-r--r--   0        0        0     1164 2023-08-01 18:55:17.171814 nonebot_plugin_remake-0.3.1/README.md
+-rw-r--r--   0        0        0     7728 2023-08-01 18:55:17.171814 nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/__init__.py
+-rw-r--r--   0        0        0      679 2023-08-01 18:55:17.171814 nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/age.py
+-rw-r--r--   0        0        0      127 2023-08-01 18:55:17.171814 nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/config.py
+-rw-r--r--   0        0        0    11874 2023-08-01 18:55:17.171814 nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/drawer.py
+-rw-r--r--   0        0        0     3138 2023-08-01 18:55:17.171814 nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/event.py
+-rw-r--r--   0        0        0     2596 2023-08-01 18:55:17.171814 nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/life.py
+-rw-r--r--   0        0        0     6700 2023-08-01 18:55:17.171814 nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/property.py
+-rw-r--r--   0        0        0  1967733 2023-08-01 18:55:17.179814 nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/resources/data/age.json
+-rw-r--r--   0        0        0   377196 2023-08-01 18:55:17.179814 nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/resources/data/events.json
+-rw-r--r--   0        0        0    29584 2023-08-01 18:55:17.179814 nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/resources/data/talents.json
+-rw-r--r--   0        0        0  1895036 2023-08-01 18:55:17.187814 nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/resources/fonts/方正像素12.ttf
+-rw-r--r--   0        0        0     9336 2023-08-01 18:55:17.187814 nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/resources/images/bg_summary.png
+-rw-r--r--   0        0        0     6810 2023-08-01 18:55:17.187814 nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/resources/images/bg_talent.png
+-rw-r--r--   0        0        0     4590 2023-08-01 18:55:17.187814 nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/resources/images/icon_chr.png
+-rw-r--r--   0        0        0     1586 2023-08-01 18:55:17.187814 nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/resources/images/icon_int.png
+-rw-r--r--   0        0        0      904 2023-08-01 18:55:17.187814 nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/resources/images/icon_mny.png
+-rw-r--r--   0        0        0     3319 2023-08-01 18:55:17.187814 nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/resources/images/icon_spr.png
+-rw-r--r--   0        0        0     2873 2023-08-01 18:55:17.187814 nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/resources/images/icon_str.png
+-rw-r--r--   0        0        0      195 2023-08-01 18:55:17.187814 nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/resources/images/title_left.png
+-rw-r--r--   0        0        0      208 2023-08-01 18:55:17.187814 nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/resources/images/title_right.png
+-rw-r--r--   0        0        0    86169 2023-08-01 18:55:17.187814 nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/resources/images/titlebar.png
+-rw-r--r--   0        0        0     3258 2023-08-01 18:55:17.187814 nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/talent.py
+-rw-r--r--   0        0        0      960 2023-08-01 18:55:17.187814 nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/utils.py
+-rw-r--r--   0        0        0      691 2023-08-01 18:55:17.191814 nonebot_plugin_remake-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2064 1970-01-01 00:00:00.000000 nonebot_plugin_remake-0.3.1/PKG-INFO
```

### Comparing `nonebot_plugin_remake-0.3.0/LICENSE` & `nonebot_plugin_remake-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_remake-0.3.0/README.md` & `nonebot_plugin_remake-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/__init__.py` & `nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/__init__.py`

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
-        "version": "0.3.0",
+        "version": "0.3.1",
     },
 )
 
 remake_config = Config.parse_obj(get_driver().config.dict())
 
 onebot_v11_loaded = False
 if remake_config.remake_send_forword_msg:
```

### Comparing `nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/age.py` & `nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/age.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/drawer.py` & `nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/drawer.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/event.py` & `nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/event.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/life.py` & `nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/life.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/property.py` & `nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/property.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/resources/data/age.json` & `nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/resources/data/age.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/resources/data/events.json` & `nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/resources/data/events.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/resources/data/talents.json` & `nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/resources/data/talents.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/resources/fonts/方正像素12.ttf` & `nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/resources/fonts/方正像素12.ttf`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/resources/images/bg_summary.png` & `nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/resources/images/bg_summary.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/resources/images/bg_talent.png` & `nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/resources/images/bg_talent.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/resources/images/icon_chr.png` & `nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/resources/images/icon_chr.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/resources/images/icon_int.png` & `nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/resources/images/icon_int.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/resources/images/icon_mny.png` & `nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/resources/images/icon_mny.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/resources/images/icon_spr.png` & `nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/resources/images/icon_spr.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/resources/images/icon_str.png` & `nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/resources/images/icon_str.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/resources/images/titlebar.png` & `nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/resources/images/titlebar.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/talent.py` & `nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/talent.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_remake-0.3.0/nonebot_plugin_remake/utils.py` & `nonebot_plugin_remake-0.3.1/nonebot_plugin_remake/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_remake-0.3.0/pyproject.toml` & `nonebot_plugin_remake-0.3.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [tool.poetry]
 name = "nonebot_plugin_remake"
-version = "0.3.0"
+version = "0.3.1"
 description = "适用于 Nonebot2 的人生重开模拟器插件"
 authors = ["meetwq <meetwq@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/noneplugin/nonebot-plugin-remake"
 repository = "https://github.com/noneplugin/nonebot-plugin-remake"
 
 [tool.poetry.dependencies]
 python = "^3.8"
+Pillow = ">=9.2.0,<11.0.0"
 nonebot2 = "^2.0.0"
 nonebot-plugin-send-anything-anywhere = "^0.2.7"
 nonebot-adapter-onebot = { version = "^2.2.0", optional = true }
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.1.0"
```

### Comparing `nonebot_plugin_remake-0.3.0/PKG-INFO` & `nonebot_plugin_remake-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-remake
-Version: 0.3.0
+Version: 0.3.1
 Summary: 适用于 Nonebot2 的人生重开模拟器插件
 Home-page: https://github.com/noneplugin/nonebot-plugin-remake
 License: MIT
 Author: meetwq
 Author-email: meetwq@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: Pillow (>=9.2.0,<11.0.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.2.0,<3.0.0)
 Requires-Dist: nonebot-plugin-send-anything-anywhere (>=0.2.7,<0.3.0)
 Requires-Dist: nonebot2 (>=2.0.0,<3.0.0)
 Project-URL: Repository, https://github.com/noneplugin/nonebot-plugin-remake
 Description-Content-Type: text/markdown
 
 # nonebot-plugin-remake
```

