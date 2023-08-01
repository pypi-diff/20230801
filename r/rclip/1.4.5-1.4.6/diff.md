# Comparing `tmp/rclip-1.4.5.tar.gz` & `tmp/rclip-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rclip-1.4.5.tar", max compression
+gzip compressed data, was "rclip-1.4.6.tar", max compression
```

## Comparing `rclip-1.4.5.tar` & `rclip-1.4.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1074 2023-08-01 07:09:38.251811 rclip-1.4.5/LICENSE
--rw-r--r--   0        0        0     5023 2023-08-01 07:09:38.251811 rclip-1.4.5/README.md
--rw-r--r--   0        0        0     1556 2023-08-01 07:09:38.251811 rclip-1.4.5/pyproject.toml
--rw-r--r--   0        0        0     2940 2023-08-01 07:09:38.251811 rclip-1.4.5/rclip/db.py
--rw-r--r--   0        0        0     5586 2023-08-01 07:09:38.251811 rclip-1.4.5/rclip/main.py
--rw-r--r--   0        0        0     5161 2023-08-01 07:09:38.251811 rclip-1.4.5/rclip/model.py
--rw-r--r--   0        0        0     4551 2023-08-01 07:09:38.251811 rclip-1.4.5/rclip/utils.py
--rw-r--r--   0        0        0     6528 1970-01-01 00:00:00.000000 rclip-1.4.5/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-08-01 09:22:23.983865 rclip-1.4.6/LICENSE
+-rw-r--r--   0        0        0     5023 2023-08-01 09:22:23.983865 rclip-1.4.6/README.md
+-rw-r--r--   0        0        0     1557 2023-08-01 09:22:23.983865 rclip-1.4.6/pyproject.toml
+-rw-r--r--   0        0        0     2940 2023-08-01 09:22:23.983865 rclip-1.4.6/rclip/db.py
+-rw-r--r--   0        0        0     5586 2023-08-01 09:22:23.983865 rclip-1.4.6/rclip/main.py
+-rw-r--r--   0        0        0     5161 2023-08-01 09:22:23.983865 rclip-1.4.6/rclip/model.py
+-rw-r--r--   0        0        0     4551 2023-08-01 09:22:23.983865 rclip-1.4.6/rclip/utils.py
+-rw-r--r--   0        0        0     6529 1970-01-01 00:00:00.000000 rclip-1.4.6/PKG-INFO
```

### Comparing `rclip-1.4.5/LICENSE` & `rclip-1.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `rclip-1.4.5/README.md` & `rclip-1.4.6/README.md`

 * *Files identical despite different names*

### Comparing `rclip-1.4.5/pyproject.toml` & `rclip-1.4.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rclip"
-version = "1.4.5"
+version = "1.4.6"
 description = "AI-Powered Command-Line Photo Search Tool"
 authors = ["Yurij Mikhalevich <yurij@mikhalevi.ch>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/yurijmikhalevich/rclip"
 keywords = ["image search", "computer vision", "photography"]
 classifiers = [
@@ -16,15 +16,15 @@
   "Topic :: Scientific/Engineering :: Image Recognition",
   "Topic :: Utilities",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 open_clip_torch = "^2.20.0"
-pillow = "^9.0.1"
+pillow = "^10.0.0"
 requests = "~=2.26"
 torch = [
   { version = "==2.0.1", source = "pypi", markers = "sys_platform != 'linux'" },
   { version = "==2.0.1+cpu", source = "pytorch-cpu", markers = "sys_platform == 'linux'" }
 ]
 torchvision = [
   { version = "==0.15.2", source = "pypi", markers = "sys_platform != 'linux'" },
```

### Comparing `rclip-1.4.5/rclip/db.py` & `rclip-1.4.6/rclip/db.py`

 * *Files identical despite different names*

### Comparing `rclip-1.4.5/rclip/main.py` & `rclip-1.4.6/rclip/main.py`

 * *Files identical despite different names*

### Comparing `rclip-1.4.5/rclip/model.py` & `rclip-1.4.6/rclip/model.py`

 * *Files identical despite different names*

### Comparing `rclip-1.4.5/rclip/utils.py` & `rclip-1.4.6/rclip/utils.py`

 * *Files identical despite different names*

### Comparing `rclip-1.4.5/PKG-INFO` & `rclip-1.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rclip
-Version: 1.4.5
+Version: 1.4.6
 Summary: AI-Powered Command-Line Photo Search Tool
 Home-page: https://github.com/yurijmikhalevich/rclip
 License: MIT
 Keywords: image search,computer vision,photography
 Author: Yurij Mikhalevich
 Author-email: yurij@mikhalevi.ch
 Requires-Python: >=3.8,<4.0
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Classifier: Topic :: Utilities
 Requires-Dist: open_clip_torch (>=2.20.0,<3.0.0)
-Requires-Dist: pillow (>=9.0.1,<10.0.0)
+Requires-Dist: pillow (>=10.0.0,<11.0.0)
 Requires-Dist: requests (>=2.26,<3.0)
 Requires-Dist: torch (==2.0.1) ; sys_platform != "linux"
 Requires-Dist: torch (==2.0.1+cpu) ; sys_platform == "linux"
 Requires-Dist: torchvision (==0.15.2) ; sys_platform != "linux"
 Requires-Dist: torchvision (==0.15.2+cpu) ; sys_platform == "linux"
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Project-URL: Repository, https://github.com/yurijmikhalevich/rclip
```

