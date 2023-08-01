# Comparing `tmp/rclip-1.4.4a4.tar.gz` & `tmp/rclip-1.4.4a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rclip-1.4.4a4.tar", max compression
+gzip compressed data, was "rclip-1.4.4a5.tar", max compression
```

## Comparing `rclip-1.4.4a4.tar` & `rclip-1.4.4a5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1074 2023-08-01 05:57:50.985407 rclip-1.4.4a4/LICENSE
--rw-r--r--   0        0        0     4791 2023-08-01 05:57:50.985407 rclip-1.4.4a4/README.md
--rw-r--r--   0        0        0     1558 2023-08-01 05:57:50.989407 rclip-1.4.4a4/pyproject.toml
--rw-r--r--   0        0        0     2940 2023-08-01 05:57:50.989407 rclip-1.4.4a4/rclip/db.py
--rw-r--r--   0        0        0     5586 2023-08-01 05:57:50.989407 rclip-1.4.4a4/rclip/main.py
--rw-r--r--   0        0        0     5161 2023-08-01 05:57:50.989407 rclip-1.4.4a4/rclip/model.py
--rw-r--r--   0        0        0     4551 2023-08-01 05:57:50.989407 rclip-1.4.4a4/rclip/utils.py
--rw-r--r--   0        0        0     6298 1970-01-01 00:00:00.000000 rclip-1.4.4a4/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-08-01 06:15:21.672181 rclip-1.4.4a5/LICENSE
+-rw-r--r--   0        0        0     5055 2023-08-01 06:15:21.672181 rclip-1.4.4a5/README.md
+-rw-r--r--   0        0        0     1558 2023-08-01 06:15:21.672181 rclip-1.4.4a5/pyproject.toml
+-rw-r--r--   0        0        0     2940 2023-08-01 06:15:21.672181 rclip-1.4.4a5/rclip/db.py
+-rw-r--r--   0        0        0     5586 2023-08-01 06:15:21.672181 rclip-1.4.4a5/rclip/main.py
+-rw-r--r--   0        0        0     5161 2023-08-01 06:15:21.672181 rclip-1.4.4a5/rclip/model.py
+-rw-r--r--   0        0        0     4551 2023-08-01 06:15:21.672181 rclip-1.4.4a5/rclip/utils.py
+-rw-r--r--   0        0        0     6562 1970-01-01 00:00:00.000000 rclip-1.4.4a5/PKG-INFO
```

### Comparing `rclip-1.4.4a4/LICENSE` & `rclip-1.4.4a5/LICENSE`

 * *Files identical despite different names*

### Comparing `rclip-1.4.4a4/README.md` & `rclip-1.4.4a5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -9,24 +9,36 @@
   <img alt="rclip logo" src="https://raw.githubusercontent.com/yurijmikhalevich/rclip/main/resources/logo-transparent.png" width="600px" />
 </div>
 
 **rclip** is a command-line photo search tool based on the awesome OpenAI's [CLIP](https://github.com/openai/CLIP) neural network.
 
 ## Installation
 
-Currently, pre-built distributable is available only for Linux x86_64.
-
-1. Download the AppImage from the latest [release](https://github.com/yurijmikhalevich/rclip/releases).
-
-2. Execute the following commands:
-
-```bash
-chmod +x <downloaded AppImage filename>
-sudo mv <downloaded AppImage filename> /usr/local/bin/rclip
-```
+<details>
+  <summary><strong>Using <code>pip</code> (macOS/Windows/Linux/etc.)</strong></summary>
+  
+  ```bash
+  pip install rclip
+  ```
+</details>
+
+<details>
+  <summary><strong>Linux x86_64 (self-containing binary)</strong></summary>
+  
+  On Linux x86_64, you can install **rclip** as a self-containing binary.
+
+  1. Download the AppImage from the latest [release](https://github.com/yurijmikhalevich/rclip/releases).
+
+  2. Execute the following commands:
+
+  ```bash
+  chmod +x <downloaded AppImage filename>
+  sudo mv <downloaded AppImage filename> /usr/local/bin/rclip
+  ```
+</details>
 
 ## Usage
 
 ```bash
 cd photos && rclip "search query"
 ```
```

### Comparing `rclip-1.4.4a4/pyproject.toml` & `rclip-1.4.4a5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rclip"
-version = "1.4.4a4"
+version = "1.4.4a5"
 description = "AI-Powered Command-Line Photo Search Tool"
 authors = ["Yurij Mikhalevich <yurij@mikhalevi.ch>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/yurijmikhalevich/rclip"
 keywords = ["image search", "computer vision", "photography"]
 classifiers = [
```

### Comparing `rclip-1.4.4a4/rclip/db.py` & `rclip-1.4.4a5/rclip/db.py`

 * *Files identical despite different names*

### Comparing `rclip-1.4.4a4/rclip/main.py` & `rclip-1.4.4a5/rclip/main.py`

 * *Files identical despite different names*

### Comparing `rclip-1.4.4a4/rclip/model.py` & `rclip-1.4.4a5/rclip/model.py`

 * *Files identical despite different names*

### Comparing `rclip-1.4.4a4/rclip/utils.py` & `rclip-1.4.4a5/rclip/utils.py`

 * *Files identical despite different names*

### Comparing `rclip-1.4.4a4/PKG-INFO` & `rclip-1.4.4a5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rclip
-Version: 1.4.4a4
+Version: 1.4.4a5
 Summary: AI-Powered Command-Line Photo Search Tool
 Home-page: https://github.com/yurijmikhalevich/rclip
 License: MIT
 Keywords: image search,computer vision,photography
 Author: Yurij Mikhalevich
 Author-email: yurij@mikhalevi.ch
 Requires-Python: >=3.8,<4.0
@@ -43,24 +43,36 @@
   <img alt="rclip logo" src="https://raw.githubusercontent.com/yurijmikhalevich/rclip/main/resources/logo-transparent.png" width="600px" />
 </div>
 
 **rclip** is a command-line photo search tool based on the awesome OpenAI's [CLIP](https://github.com/openai/CLIP) neural network.
 
 ## Installation
 
-Currently, pre-built distributable is available only for Linux x86_64.
-
-1. Download the AppImage from the latest [release](https://github.com/yurijmikhalevich/rclip/releases).
-
-2. Execute the following commands:
-
-```bash
-chmod +x <downloaded AppImage filename>
-sudo mv <downloaded AppImage filename> /usr/local/bin/rclip
-```
+<details>
+  <summary><strong>Using <code>pip</code> (macOS/Windows/Linux/etc.)</strong></summary>
+  
+  ```bash
+  pip install rclip
+  ```
+</details>
+
+<details>
+  <summary><strong>Linux x86_64 (self-containing binary)</strong></summary>
+  
+  On Linux x86_64, you can install **rclip** as a self-containing binary.
+
+  1. Download the AppImage from the latest [release](https://github.com/yurijmikhalevich/rclip/releases).
+
+  2. Execute the following commands:
+
+  ```bash
+  chmod +x <downloaded AppImage filename>
+  sudo mv <downloaded AppImage filename> /usr/local/bin/rclip
+  ```
+</details>
 
 ## Usage
 
 ```bash
 cd photos && rclip "search query"
 ```
```

