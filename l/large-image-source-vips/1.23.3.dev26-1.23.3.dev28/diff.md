# Comparing `tmp/large-image-source-vips-1.23.3.dev26.tar.gz` & `tmp/large-image-source-vips-1.23.3.dev28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "large-image-source-vips-1.23.3.dev26.tar", last modified: Mon Jul 31 15:03:49 2023, max compression
+gzip compressed data, was "large-image-source-vips-1.23.3.dev28.tar", last modified: Tue Aug  1 17:18:46 2023, max compression
```

## Comparing `large-image-source-vips-1.23.3.dev26.tar` & `large-image-source-vips-1.23.3.dev28.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-31 15:03:49.204716 large-image-source-vips-1.23.3.dev26/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2023-07-31 15:03:48.000000 large-image-source-vips-1.23.3.dev26/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      920 2023-07-31 15:03:49.204716 large-image-source-vips-1.23.3.dev26/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8267 2023-07-31 15:03:48.000000 large-image-source-vips-1.23.3.dev26/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-31 15:03:49.204716 large-image-source-vips-1.23.3.dev26/large_image_source_vips/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24064 2023-07-31 15:02:05.000000 large-image-source-vips-1.23.3.dev26/large_image_source_vips/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      374 2023-07-31 15:02:05.000000 large-image-source-vips-1.23.3.dev26/large_image_source_vips/girder_source.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-31 15:03:49.204716 large-image-source-vips-1.23.3.dev26/large_image_source_vips.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      920 2023-07-31 15:03:49.000000 large-image-source-vips-1.23.3.dev26/large_image_source_vips.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      388 2023-07-31 15:03:49.000000 large-image-source-vips-1.23.3.dev26/large_image_source_vips.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-07-31 15:03:49.000000 large-image-source-vips-1.23.3.dev26/large_image_source_vips.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      166 2023-07-31 15:03:49.000000 large-image-source-vips-1.23.3.dev26/large_image_source_vips.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      126 2023-07-31 15:03:49.000000 large-image-source-vips-1.23.3.dev26/large_image_source_vips.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2023-07-31 15:03:49.000000 large-image-source-vips-1.23.3.dev26/large_image_source_vips.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-07-31 15:03:49.204716 large-image-source-vips-1.23.3.dev26/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2590 2023-07-31 15:02:05.000000 large-image-source-vips-1.23.3.dev26/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-01 17:18:46.877385 large-image-source-vips-1.23.3.dev28/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2023-08-01 17:18:46.000000 large-image-source-vips-1.23.3.dev28/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      920 2023-08-01 17:18:46.877385 large-image-source-vips-1.23.3.dev28/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8267 2023-08-01 17:18:46.000000 large-image-source-vips-1.23.3.dev28/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-01 17:18:46.877385 large-image-source-vips-1.23.3.dev28/large_image_source_vips/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24064 2023-08-01 17:17:02.000000 large-image-source-vips-1.23.3.dev28/large_image_source_vips/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      374 2023-08-01 17:17:02.000000 large-image-source-vips-1.23.3.dev28/large_image_source_vips/girder_source.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-01 17:18:46.877385 large-image-source-vips-1.23.3.dev28/large_image_source_vips.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      920 2023-08-01 17:18:46.000000 large-image-source-vips-1.23.3.dev28/large_image_source_vips.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      388 2023-08-01 17:18:46.000000 large-image-source-vips-1.23.3.dev28/large_image_source_vips.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-01 17:18:46.000000 large-image-source-vips-1.23.3.dev28/large_image_source_vips.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      166 2023-08-01 17:18:46.000000 large-image-source-vips-1.23.3.dev28/large_image_source_vips.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      126 2023-08-01 17:18:46.000000 large-image-source-vips-1.23.3.dev28/large_image_source_vips.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2023-08-01 17:18:46.000000 large-image-source-vips-1.23.3.dev28/large_image_source_vips.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-08-01 17:18:46.877385 large-image-source-vips-1.23.3.dev28/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2590 2023-08-01 17:17:02.000000 large-image-source-vips-1.23.3.dev28/setup.py
```

### Comparing `large-image-source-vips-1.23.3.dev26/LICENSE` & `large-image-source-vips-1.23.3.dev28/LICENSE`

 * *Files identical despite different names*

### Comparing `large-image-source-vips-1.23.3.dev26/PKG-INFO` & `large-image-source-vips-1.23.3.dev28/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-vips
-Version: 1.23.3.dev26
+Version: 1.23.3.dev28
 Summary: A libvips tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `large-image-source-vips-1.23.3.dev26/README.rst` & `large-image-source-vips-1.23.3.dev28/README.rst`

 * *Files identical despite different names*

### Comparing `large-image-source-vips-1.23.3.dev26/large_image_source_vips/__init__.py` & `large-image-source-vips-1.23.3.dev28/large_image_source_vips/__init__.py`

 * *Files identical despite different names*

### Comparing `large-image-source-vips-1.23.3.dev26/large_image_source_vips.egg-info/PKG-INFO` & `large-image-source-vips-1.23.3.dev28/large_image_source_vips.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-vips
-Version: 1.23.3.dev26
+Version: 1.23.3.dev28
 Summary: A libvips tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `large-image-source-vips-1.23.3.dev26/setup.py` & `large-image-source-vips-1.23.3.dev28/setup.py`

 * *Files identical despite different names*

