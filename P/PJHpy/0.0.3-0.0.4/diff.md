# Comparing `tmp/PJHpy-0.0.3.tar.gz` & `tmp/PJHpy-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PJHpy-0.0.3.tar", last modified: Tue Aug  1 04:33:04 2023, max compression
+gzip compressed data, was "PJHpy-0.0.4.tar", last modified: Tue Aug  1 04:59:50 2023, max compression
```

## Comparing `PJHpy-0.0.3.tar` & `PJHpy-0.0.4.tar`

### file list

```diff
@@ -1,11 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 04:33:04.486259 PJHpy-0.0.3/
--rw-rw-rw-   0        0        0     1081 2023-08-01 03:30:09.000000 PJHpy-0.0.3/LICENSE
-drwxrwxrwx   0        0        0        0 2023-08-01 04:33:04.480228 PJHpy-0.0.3/PJHpy.egg-info/
--rw-rw-rw-   0        0        0      413 2023-08-01 04:33:04.000000 PJHpy-0.0.3/PJHpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      142 2023-08-01 04:33:04.000000 PJHpy-0.0.3/PJHpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 04:33:04.000000 PJHpy-0.0.3/PJHpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 04:33:04.000000 PJHpy-0.0.3/PJHpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      413 2023-08-01 04:33:04.485219 PJHpy-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       77 2023-08-01 03:59:28.000000 PJHpy-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-08-01 04:33:04.486259 PJHpy-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1284 2023-08-01 04:32:11.000000 PJHpy-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 04:59:50.924517 PJHpy-0.0.4/
+-rw-rw-rw-   0        0        0     1081 2023-08-01 03:30:09.000000 PJHpy-0.0.4/LICENSE
+drwxrwxrwx   0        0        0        0 2023-08-01 04:59:50.924517 PJHpy-0.0.4/PJHpy/
+-rw-rw-rw-   0        0        0      162 2023-08-01 04:56:39.000000 PJHpy-0.0.4/PJHpy/__init__.py
+-rw-rw-rw-   0        0        0    14641 2023-07-31 03:17:57.000000 PJHpy-0.0.4/PJHpy/mypython.py
+drwxrwxrwx   0        0        0        0 2023-08-01 04:59:50.924517 PJHpy-0.0.4/PJHpy.egg-info/
+-rw-rw-rw-   0        0        0      413 2023-08-01 04:59:50.000000 PJHpy-0.0.4/PJHpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2023-08-01 04:59:50.000000 PJHpy-0.0.4/PJHpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 04:59:50.000000 PJHpy-0.0.4/PJHpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-08-01 04:59:50.000000 PJHpy-0.0.4/PJHpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      413 2023-08-01 04:59:50.924517 PJHpy-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       77 2023-08-01 03:59:28.000000 PJHpy-0.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-01 04:59:50.924517 PJHpy-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1284 2023-08-01 04:59:10.000000 PJHpy-0.0.4/setup.py
```

### Comparing `PJHpy-0.0.3/LICENSE` & `PJHpy-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `PJHpy-0.0.3/setup.py` & `PJHpy-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import setuptools
 
 setuptools.setup(
     # 项目的名称
     name="PJHpy",
     # 项目的版本
-    version="0.0.3",
+    version="0.0.4",
     # 项目的作者
     author="PJH",
     # 作者的邮箱
     author_email="super-upan@outlook.com",
     # 项目描述
     description="简单代码上传测试",
     # 项目的长描述
```

