# Comparing `tmp/f_dpi-0.0.4.tar.gz` & `tmp/f_dpi-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "f_dpi-0.0.4.tar", last modified: Sat Jul  1 06:48:25 2023, max compression
+gzip compressed data, was "f_dpi-0.0.5.tar", last modified: Tue Aug  1 05:13:24 2023, max compression
```

## Comparing `f_dpi-0.0.4.tar` & `f_dpi-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 06:48:25.474054 f_dpi-0.0.4/
--rw-rw-rw-   0        0        0      147 2023-07-01 06:48:25.474054 f_dpi-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0        6 2023-04-17 20:39:54.000000 f_dpi-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-01 06:48:25.460734 f_dpi-0.0.4/f_dpi/
--rw-rw-rw-   0        0        0       62 2023-07-01 06:26:53.000000 f_dpi-0.0.4/f_dpi/__init__.py
--rw-rw-rw-   0        0        0       21 2023-07-01 06:48:02.000000 f_dpi-0.0.4/f_dpi/__version__.py
--rw-rw-rw-   0        0        0     1427 2023-07-01 06:44:42.000000 f_dpi-0.0.4/f_dpi/f_dpi.py
-drwxrwxrwx   0        0        0        0 2023-07-01 06:48:25.473044 f_dpi-0.0.4/f_dpi.egg-info/
--rw-rw-rw-   0        0        0      147 2023-07-01 06:48:25.000000 f_dpi-0.0.4/f_dpi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2023-07-01 06:48:25.000000 f_dpi-0.0.4/f_dpi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 06:48:25.000000 f_dpi-0.0.4/f_dpi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-07-01 06:48:25.000000 f_dpi-0.0.4/f_dpi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-01 06:48:25.000000 f_dpi-0.0.4/f_dpi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-07-01 06:48:25.475054 f_dpi-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      523 2023-07-01 06:48:10.000000 f_dpi-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 05:13:24.317764 f_dpi-0.0.5/
+-rw-rw-rw-   0        0        0      147 2023-08-01 05:13:24.317764 f_dpi-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0        6 2023-04-17 20:39:54.000000 f_dpi-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-08-01 05:13:24.317764 f_dpi-0.0.5/f_dpi/
+-rw-rw-rw-   0        0        0       62 2023-07-01 06:26:53.000000 f_dpi-0.0.5/f_dpi/__init__.py
+-rw-rw-rw-   0        0        0       21 2023-08-01 05:12:16.000000 f_dpi-0.0.5/f_dpi/__version__.py
+-rw-rw-rw-   0        0        0     1438 2023-08-01 05:12:28.000000 f_dpi-0.0.5/f_dpi/f_dpi.py
+drwxrwxrwx   0        0        0        0 2023-08-01 05:13:24.317764 f_dpi-0.0.5/f_dpi.egg-info/
+-rw-rw-rw-   0        0        0      147 2023-08-01 05:13:24.000000 f_dpi-0.0.5/f_dpi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      198 2023-08-01 05:13:24.000000 f_dpi-0.0.5/f_dpi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 05:13:24.000000 f_dpi-0.0.5/f_dpi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-08-01 05:13:24.000000 f_dpi-0.0.5/f_dpi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-08-01 05:13:24.317764 f_dpi-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      402 2023-08-01 05:12:05.000000 f_dpi-0.0.5/setup.py
```

### Comparing `f_dpi-0.0.4/f_dpi/f_dpi.py` & `f_dpi-0.0.5/f_dpi/f_dpi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import cv2
 from PIL import Image, ImageDraw
 import numpy as np
 
 def test():
 	print('test success')
```

