# Comparing `tmp/rclip-1.4.1.tar.gz` & `tmp/rclip-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rclip-1.4.1.tar", max compression
+gzip compressed data, was "rclip-1.4.2.tar", max compression
```

## Comparing `rclip-1.4.1.tar` & `rclip-1.4.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1074 2021-12-18 09:44:28.707592 rclip-1.4.1/LICENSE
--rw-r--r--   0        0        0     4073 2023-07-21 14:06:16.134178 rclip-1.4.1/README.md
--rw-r--r--   0        0        0     1564 2023-08-01 04:46:58.675533 rclip-1.4.1/pyproject.toml
--rw-r--r--   0        0        0     2940 2023-07-31 14:28:36.693991 rclip-1.4.1/rclip/db.py
--rw-r--r--   0        0        0     5586 2023-07-24 08:17:08.004229 rclip-1.4.1/rclip/main.py
--rw-r--r--   0        0        0     5161 2023-08-01 04:46:19.501263 rclip-1.4.1/rclip/model.py
--rw-r--r--   0        0        0     4551 2023-07-23 16:44:40.439264 rclip-1.4.1/rclip/utils.py
--rw-r--r--   0        0        0     5469 1970-01-01 00:00:00.000000 rclip-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2021-12-18 09:44:28.707592 rclip-1.4.2/LICENSE
+-rw-r--r--   0        0        0     4197 2023-08-01 04:51:20.720004 rclip-1.4.2/README.md
+-rw-r--r--   0        0        0     1564 2023-08-01 04:51:46.762368 rclip-1.4.2/pyproject.toml
+-rw-r--r--   0        0        0     2940 2023-07-31 14:28:36.693991 rclip-1.4.2/rclip/db.py
+-rw-r--r--   0        0        0     5586 2023-07-24 08:17:08.004229 rclip-1.4.2/rclip/main.py
+-rw-r--r--   0        0        0     5161 2023-08-01 04:46:19.501263 rclip-1.4.2/rclip/model.py
+-rw-r--r--   0        0        0     4551 2023-07-23 16:44:40.439264 rclip-1.4.2/rclip/utils.py
+-rw-r--r--   0        0        0     5593 1970-01-01 00:00:00.000000 rclip-1.4.2/PKG-INFO
```

### Comparing `rclip-1.4.1/LICENSE` & `rclip-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rclip-1.4.1/README.md` & `rclip-1.4.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
 [![All Contributors](https://img.shields.io/badge/all_contributors-1-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 [[Blog]](https://mikhalevi.ch/rclip-an-ai-powered-command-line-photo-search-tool/) [[Demo on YouTube]](https://www.youtube.com/watch?v=tAJHXOkHidw) [[Paper]](https://www.thinkmind.org/index.php?view=article&articleid=content_2023_1_20_60011)
 
 <div align="center">
-  <img alt="rclip logo" src="resources/logo-transparent.png" width="600px" />
+  <img alt="rclip logo" src="https://raw.githubusercontent.com/yurijmikhalevich/rclip/main/resources/logo-transparent.png" width="600px" />
 </div>
 
 **rclip** is a command-line photo search tool based on the awesome OpenAI's [CLIP](https://github.com/openai/CLIP) neural network.
 
 ## Installation
 
 Currently, pre-built distributable is available only for Linux x86_64.
@@ -26,15 +26,15 @@
 
 ## Usage
 
 ```bash
 cd photos && rclip "search query"
 ```
 
-<img alt="rclip usage demo" src="resources/rclip-usage.gif" width="640px" />
+<img alt="rclip usage demo" src="https://raw.githubusercontent.com/yurijmikhalevich/rclip/main/resources/rclip-usage.gif" width="640px" />
 
 When you run **rclip** for the first time in a particular directory, it's going to extract features from the photos, and this takes time. How long it takes depends on your CPU and the number of pictures you will search through. It took about a day to process 73 thousand photos on my NAS, which runs an old-ish Intel Celeron J3455.
 
 For a detailed demonstration, watch the video: https://www.youtube.com/watch?v=tAJHXOkHidw.
 
 You can also use another image as a query by passing a file path or even an URL to the image file, and **rclip** will find the images most similar to the one you used as a query. If you are referencing a local image via a relative path, you **must** prefix it with `./`. For example:
```

### Comparing `rclip-1.4.1/pyproject.toml` & `rclip-1.4.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rclip"
-version = "1.4.1"
+version = "1.4.2"
 description = "AI-Powered Command-Line Photo Search Tool"
 authors = ["Yurij Mikhalevich <yurij@mikhalevi.ch>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/yurijmikhalevich/rclip"
 keywords = ["image search", "computer vision", "photography"]
 classifiers = [
```

### Comparing `rclip-1.4.1/rclip/db.py` & `rclip-1.4.2/rclip/db.py`

 * *Files identical despite different names*

### Comparing `rclip-1.4.1/rclip/main.py` & `rclip-1.4.2/rclip/main.py`

 * *Files identical despite different names*

### Comparing `rclip-1.4.1/rclip/model.py` & `rclip-1.4.2/rclip/model.py`

 * *Files identical despite different names*

### Comparing `rclip-1.4.1/rclip/utils.py` & `rclip-1.4.2/rclip/utils.py`

 * *Files identical despite different names*

### Comparing `rclip-1.4.1/PKG-INFO` & `rclip-1.4.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rclip
-Version: 1.4.1
+Version: 1.4.2
 Summary: AI-Powered Command-Line Photo Search Tool
 Home-page: https://github.com/yurijmikhalevich/rclip
 License: MIT
 Keywords: image search,computer vision,photography
 Author: Yurij Mikhalevich
 Author-email: yurij@mikhalevi.ch
 Requires-Python: >=3.8,<3.10
@@ -34,15 +34,15 @@
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
 [![All Contributors](https://img.shields.io/badge/all_contributors-1-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 [[Blog]](https://mikhalevi.ch/rclip-an-ai-powered-command-line-photo-search-tool/) [[Demo on YouTube]](https://www.youtube.com/watch?v=tAJHXOkHidw) [[Paper]](https://www.thinkmind.org/index.php?view=article&articleid=content_2023_1_20_60011)
 
 <div align="center">
-  <img alt="rclip logo" src="resources/logo-transparent.png" width="600px" />
+  <img alt="rclip logo" src="https://raw.githubusercontent.com/yurijmikhalevich/rclip/main/resources/logo-transparent.png" width="600px" />
 </div>
 
 **rclip** is a command-line photo search tool based on the awesome OpenAI's [CLIP](https://github.com/openai/CLIP) neural network.
 
 ## Installation
 
 Currently, pre-built distributable is available only for Linux x86_64.
@@ -58,15 +58,15 @@
 
 ## Usage
 
 ```bash
 cd photos && rclip "search query"
 ```
 
-<img alt="rclip usage demo" src="resources/rclip-usage.gif" width="640px" />
+<img alt="rclip usage demo" src="https://raw.githubusercontent.com/yurijmikhalevich/rclip/main/resources/rclip-usage.gif" width="640px" />
 
 When you run **rclip** for the first time in a particular directory, it's going to extract features from the photos, and this takes time. How long it takes depends on your CPU and the number of pictures you will search through. It took about a day to process 73 thousand photos on my NAS, which runs an old-ish Intel Celeron J3455.
 
 For a detailed demonstration, watch the video: https://www.youtube.com/watch?v=tAJHXOkHidw.
 
 You can also use another image as a query by passing a file path or even an URL to the image file, and **rclip** will find the images most similar to the one you used as a query. If you are referencing a local image via a relative path, you **must** prefix it with `./`. For example:
```

