# Comparing `tmp/f_yolov8-0.0.3.tar.gz` & `tmp/f_yolov8-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "f_yolov8-0.0.3.tar", last modified: Tue Jul  4 01:45:52 2023, max compression
+gzip compressed data, was "f_yolov8-0.0.5.tar", last modified: Tue Aug  1 05:25:29 2023, max compression
```

## Comparing `f_yolov8-0.0.3.tar` & `f_yolov8-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 01:45:52.142068 f_yolov8-0.0.3/
--rw-rw-rw-   0        0        0      150 2023-07-04 01:45:52.143069 f_yolov8-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0        6 2023-04-17 20:39:54.000000 f_yolov8-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-04 01:45:52.130068 f_yolov8-0.0.3/f_yolov8/
--rw-rw-rw-   0        0        0       65 2023-07-04 01:40:15.000000 f_yolov8-0.0.3/f_yolov8/__init__.py
--rw-rw-rw-   0        0        0       21 2023-07-04 01:45:18.000000 f_yolov8-0.0.3/f_yolov8/__version__.py
--rw-rw-rw-   0        0        0     8555 2023-07-04 01:38:13.000000 f_yolov8-0.0.3/f_yolov8/f_yolov8.py
-drwxrwxrwx   0        0        0        0 2023-07-04 01:45:52.141069 f_yolov8-0.0.3/f_yolov8.egg-info/
--rw-rw-rw-   0        0        0      150 2023-07-04 01:45:52.000000 f_yolov8-0.0.3/f_yolov8.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-07-04 01:45:52.000000 f_yolov8-0.0.3/f_yolov8.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 01:45:52.000000 f_yolov8-0.0.3/f_yolov8.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2023-07-04 01:45:52.000000 f_yolov8-0.0.3/f_yolov8.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-04 01:45:52.000000 f_yolov8-0.0.3/f_yolov8.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-07-04 01:45:52.144069 f_yolov8-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      526 2023-07-04 01:45:28.000000 f_yolov8-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 05:25:29.512240 f_yolov8-0.0.5/
+-rw-rw-rw-   0        0        0      150 2023-08-01 05:25:29.512240 f_yolov8-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0        6 2023-04-17 20:39:54.000000 f_yolov8-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-08-01 05:25:29.500198 f_yolov8-0.0.5/f_yolov8/
+-rw-rw-rw-   0        0        0       65 2023-07-04 01:40:15.000000 f_yolov8-0.0.5/f_yolov8/__init__.py
+-rw-rw-rw-   0        0        0       21 2023-08-01 05:24:13.000000 f_yolov8-0.0.5/f_yolov8/__version__.py
+-rw-rw-rw-   0        0        0     8555 2023-07-04 01:38:13.000000 f_yolov8-0.0.5/f_yolov8/f_yolov8.py
+drwxrwxrwx   0        0        0        0 2023-08-01 05:25:29.511240 f_yolov8-0.0.5/f_yolov8.egg-info/
+-rw-rw-rw-   0        0        0      150 2023-08-01 05:25:29.000000 f_yolov8-0.0.5/f_yolov8.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2023-08-01 05:25:29.000000 f_yolov8-0.0.5/f_yolov8.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 05:25:29.000000 f_yolov8-0.0.5/f_yolov8.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-08-01 05:25:29.000000 f_yolov8-0.0.5/f_yolov8.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-08-01 05:25:29.513242 f_yolov8-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      403 2023-08-01 05:24:46.000000 f_yolov8-0.0.5/setup.py
```

### Comparing `f_yolov8-0.0.3/f_yolov8/f_yolov8.py` & `f_yolov8-0.0.5/f_yolov8/f_yolov8.py`

 * *Files identical despite different names*

