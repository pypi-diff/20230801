# Comparing `tmp/f_yolov8-0.0.5.tar.gz` & `tmp/f_yolov8-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "f_yolov8-0.0.5.tar", last modified: Tue Aug  1 05:25:29 2023, max compression
+gzip compressed data, was "f_yolov8-0.0.6.tar", last modified: Tue Aug  1 05:35:40 2023, max compression
```

## Comparing `f_yolov8-0.0.5.tar` & `f_yolov8-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 05:25:29.512240 f_yolov8-0.0.5/
--rw-rw-rw-   0        0        0      150 2023-08-01 05:25:29.512240 f_yolov8-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0        6 2023-04-17 20:39:54.000000 f_yolov8-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-08-01 05:25:29.500198 f_yolov8-0.0.5/f_yolov8/
--rw-rw-rw-   0        0        0       65 2023-07-04 01:40:15.000000 f_yolov8-0.0.5/f_yolov8/__init__.py
--rw-rw-rw-   0        0        0       21 2023-08-01 05:24:13.000000 f_yolov8-0.0.5/f_yolov8/__version__.py
--rw-rw-rw-   0        0        0     8555 2023-07-04 01:38:13.000000 f_yolov8-0.0.5/f_yolov8/f_yolov8.py
-drwxrwxrwx   0        0        0        0 2023-08-01 05:25:29.511240 f_yolov8-0.0.5/f_yolov8.egg-info/
--rw-rw-rw-   0        0        0      150 2023-08-01 05:25:29.000000 f_yolov8-0.0.5/f_yolov8.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      222 2023-08-01 05:25:29.000000 f_yolov8-0.0.5/f_yolov8.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 05:25:29.000000 f_yolov8-0.0.5/f_yolov8.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-08-01 05:25:29.000000 f_yolov8-0.0.5/f_yolov8.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-08-01 05:25:29.513242 f_yolov8-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      403 2023-08-01 05:24:46.000000 f_yolov8-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 05:35:40.375999 f_yolov8-0.0.6/
+-rw-rw-rw-   0        0        0      150 2023-08-01 05:35:40.375999 f_yolov8-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0        6 2023-04-17 20:39:54.000000 f_yolov8-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-08-01 05:35:40.360372 f_yolov8-0.0.6/f_yolov8/
+-rw-rw-rw-   0        0        0       65 2023-07-04 01:40:15.000000 f_yolov8-0.0.6/f_yolov8/__init__.py
+-rw-rw-rw-   0        0        0       21 2023-08-01 05:34:41.000000 f_yolov8-0.0.6/f_yolov8/__version__.py
+-rw-rw-rw-   0        0        0     8545 2023-08-01 05:29:35.000000 f_yolov8-0.0.6/f_yolov8/f_yolov8.py
+drwxrwxrwx   0        0        0        0 2023-08-01 05:35:40.375999 f_yolov8-0.0.6/f_yolov8.egg-info/
+-rw-rw-rw-   0        0        0      150 2023-08-01 05:35:40.000000 f_yolov8-0.0.6/f_yolov8.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2023-08-01 05:35:40.000000 f_yolov8-0.0.6/f_yolov8.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 05:35:40.000000 f_yolov8-0.0.6/f_yolov8.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-08-01 05:35:40.000000 f_yolov8-0.0.6/f_yolov8.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-08-01 05:35:40.375999 f_yolov8-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      403 2023-08-01 05:34:48.000000 f_yolov8-0.0.6/setup.py
```

### Comparing `f_yolov8-0.0.5/f_yolov8/f_yolov8.py` & `f_yolov8-0.0.6/f_yolov8/f_yolov8.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from ultralytics.yolo.utils.plotting import Annotator, colors
-from ultralytics.yolo.data.augment import LetterBox
+from ultralytics.utils.plotting import Annotator, colors
+from ultralytics.data.augment import LetterBox
 import copy
 import cv2
 from PIL import Image, ImageDraw
 import numpy as np
 import torch
 
 from PIL import ImageFont
```

