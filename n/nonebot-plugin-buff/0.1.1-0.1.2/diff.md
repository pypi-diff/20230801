# Comparing `tmp/nonebot_plugin_buff-0.1.1.tar.gz` & `tmp/nonebot_plugin_buff-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_buff-0.1.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_buff-0.1.2.tar", max compression
```

## Comparing `nonebot_plugin_buff-0.1.1.tar` & `nonebot_plugin_buff-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      699 2023-08-01 03:10:13.023639 nonebot_plugin_buff-0.1.1/README.md
--rw-r--r--   0        0        0     5805 2023-08-01 03:10:13.023639 nonebot_plugin_buff-0.1.1/nonebot_plugin_buff/__init__.py
--rw-r--r--   0        0        0      114 2023-08-01 03:10:13.023639 nonebot_plugin_buff-0.1.1/nonebot_plugin_buff/config.py
--rw-r--r--   0        0        0   500057 2023-08-01 03:10:13.023639 nonebot_plugin_buff-0.1.1/nonebot_plugin_buff/data.txt
--rw-r--r--   0        0        0      436 2023-08-01 03:10:13.027639 nonebot_plugin_buff-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1350 1970-01-01 00:00:00.000000 nonebot_plugin_buff-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      699 2023-08-01 03:49:06.772918 nonebot_plugin_buff-0.1.2/README.md
+-rw-r--r--   0        0        0     5805 2023-08-01 03:49:06.772918 nonebot_plugin_buff-0.1.2/nonebot_plugin_buff/__init__.py
+-rw-r--r--   0        0        0      114 2023-08-01 03:49:06.772918 nonebot_plugin_buff-0.1.2/nonebot_plugin_buff/config.py
+-rw-r--r--   0        0        0   500057 2023-08-01 03:49:06.776919 nonebot_plugin_buff-0.1.2/nonebot_plugin_buff/data.txt
+-rw-r--r--   0        0        0      433 2023-08-01 03:49:06.776919 nonebot_plugin_buff-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1348 1970-01-01 00:00:00.000000 nonebot_plugin_buff-0.1.2/PKG-INFO
```

### Comparing `nonebot_plugin_buff-0.1.1/README.md` & `nonebot_plugin_buff-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_buff-0.1.1/nonebot_plugin_buff/__init__.py` & `nonebot_plugin_buff-0.1.2/nonebot_plugin_buff/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_buff-0.1.1/nonebot_plugin_buff/data.txt` & `nonebot_plugin_buff-0.1.2/nonebot_plugin_buff/data.txt`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_buff-0.1.1/PKG-INFO` & `nonebot_plugin_buff-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-buff
-Version: 0.1.1
+Version: 0.1.2
 Summary: 实时爬取BUFF饰品价格
 License: MIT
 Author: Sydrr0
 Author-email: 2562312527@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: bs4 (>=0.0.1,<0.0.2)
+Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Requires-Dist: nonebot2 (>=2.0.1,<3.0.0)
-Requires-Dist: requests (>=2.31.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # 欢迎使用 nonebot_plugin_buff
 ![image](https://usercontent.githubfast.com/avatars/u/129657153?v=4)
 ![tip](https://badgen.net/badge/python/3.8+/orange?i)  ![tip](https://badgen.net/badge/windows/10+/green?i)  ![tip](https://badgen.net/badge/ubuntu/20.04+/pink?i) 
 
 ## 使用方法
```

