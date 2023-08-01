# Comparing `tmp/rclip-1.4.3.tar.gz` & `tmp/rclip-1.4.4a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rclip-1.4.3.tar", max compression
+gzip compressed data, was "rclip-1.4.4a4.tar", max compression
```

## Comparing `rclip-1.4.3.tar` & `rclip-1.4.4a4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1074 2021-12-18 09:44:28.707592 rclip-1.4.3/LICENSE
--rw-r--r--   0        0        0     4791 2023-08-01 05:05:25.103033 rclip-1.4.3/README.md
--rw-r--r--   0        0        0     1556 2023-08-01 05:16:40.977956 rclip-1.4.3/pyproject.toml
--rw-r--r--   0        0        0     2940 2023-07-31 14:28:36.693991 rclip-1.4.3/rclip/db.py
--rw-r--r--   0        0        0     5586 2023-07-24 08:17:08.004229 rclip-1.4.3/rclip/main.py
--rw-r--r--   0        0        0     5161 2023-08-01 04:46:19.501263 rclip-1.4.3/rclip/model.py
--rw-r--r--   0        0        0     4551 2023-07-23 16:44:40.439264 rclip-1.4.3/rclip/utils.py
--rw-r--r--   0        0        0     6296 1970-01-01 00:00:00.000000 rclip-1.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-08-01 05:57:50.985407 rclip-1.4.4a4/LICENSE
+-rw-r--r--   0        0        0     4791 2023-08-01 05:57:50.985407 rclip-1.4.4a4/README.md
+-rw-r--r--   0        0        0     1558 2023-08-01 05:57:50.989407 rclip-1.4.4a4/pyproject.toml
+-rw-r--r--   0        0        0     2940 2023-08-01 05:57:50.989407 rclip-1.4.4a4/rclip/db.py
+-rw-r--r--   0        0        0     5586 2023-08-01 05:57:50.989407 rclip-1.4.4a4/rclip/main.py
+-rw-r--r--   0        0        0     5161 2023-08-01 05:57:50.989407 rclip-1.4.4a4/rclip/model.py
+-rw-r--r--   0        0        0     4551 2023-08-01 05:57:50.989407 rclip-1.4.4a4/rclip/utils.py
+-rw-r--r--   0        0        0     6298 1970-01-01 00:00:00.000000 rclip-1.4.4a4/PKG-INFO
```

### Comparing `rclip-1.4.3/LICENSE` & `rclip-1.4.4a4/LICENSE`

 * *Files identical despite different names*

### Comparing `rclip-1.4.3/README.md` & `rclip-1.4.4a4/README.md`

 * *Files identical despite different names*

### Comparing `rclip-1.4.3/pyproject.toml` & `rclip-1.4.4a4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rclip"
-version = "1.4.3"
+version = "1.4.4a4"
 description = "AI-Powered Command-Line Photo Search Tool"
 authors = ["Yurij Mikhalevich <yurij@mikhalevi.ch>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/yurijmikhalevich/rclip"
 keywords = ["image search", "computer vision", "photography"]
 classifiers = [
```

### Comparing `rclip-1.4.3/rclip/db.py` & `rclip-1.4.4a4/rclip/db.py`

 * *Files identical despite different names*

### Comparing `rclip-1.4.3/rclip/main.py` & `rclip-1.4.4a4/rclip/main.py`

 * *Files identical despite different names*

### Comparing `rclip-1.4.3/rclip/model.py` & `rclip-1.4.4a4/rclip/model.py`

 * *Files identical despite different names*

### Comparing `rclip-1.4.3/rclip/utils.py` & `rclip-1.4.4a4/rclip/utils.py`

 * *Files identical despite different names*

### Comparing `rclip-1.4.3/PKG-INFO` & `rclip-1.4.4a4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rclip
-Version: 1.4.3
+Version: 1.4.4a4
 Summary: AI-Powered Command-Line Photo Search Tool
 Home-page: https://github.com/yurijmikhalevich/rclip
 License: MIT
 Keywords: image search,computer vision,photography
 Author: Yurij Mikhalevich
 Author-email: yurij@mikhalevi.ch
 Requires-Python: >=3.8,<4.0
```

