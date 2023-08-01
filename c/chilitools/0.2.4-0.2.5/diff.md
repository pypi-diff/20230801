# Comparing `tmp/chilitools-0.2.4.tar.gz` & `tmp/chilitools-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chilitools-0.2.4.tar", max compression
+gzip compressed data, was "chilitools-0.2.5.tar", max compression
```

## Comparing `chilitools-0.2.4.tar` & `chilitools-0.2.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     3655 2023-08-01 18:55:06.483874 chilitools-0.2.4/chilitools/__init__.py
--rw-r--r--   0        0        0        0 2022-04-15 01:52:44.257043 chilitools-0.2.4/chilitools/api/__init__.py
--rw-r--r--   0        0        0     7202 2023-07-26 02:58:58.897478 chilitools-0.2.4/chilitools/api/connector.py
--rw-r--r--   0        0        0    21203 2023-07-31 18:36:41.911804 chilitools-0.2.4/chilitools/api/endpoints.py
--rw-r--r--   0        0        0     3728 2023-03-21 14:29:37.670561 chilitools-0.2.4/chilitools/api/mycp.py
--rw-r--r--   0        0        0     3114 2022-09-20 16:25:32.069762 chilitools-0.2.4/chilitools/api/response.py
--rw-r--r--   0        0        0        0 2023-06-20 02:25:18.519289 chilitools-0.2.4/chilitools/grafx/__init__.py
--rw-r--r--   0        0        0        0 2023-06-20 19:59:39.899564 chilitools-0.2.4/chilitools/grafx/api/__init__.py
--rw-r--r--   0        0        0     1610 2023-06-22 21:44:25.944416 chilitools-0.2.4/chilitools/grafx/api/environment.py
--rw-r--r--   0        0        0      513 2023-06-22 22:42:14.136612 chilitools-0.2.4/chilitools/grafx/api/platform.py
--rw-r--r--   0        0        0     2584 2023-07-27 16:52:54.465186 chilitools-0.2.4/chilitools/grafx/auth.py
--rw-r--r--   0        0        0     1941 2023-07-27 16:52:30.339296 chilitools-0.2.4/chilitools/grafx/connector.py
--rw-r--r--   0        0        0     2370 2023-07-27 17:26:37.658495 chilitools-0.2.4/chilitools/grafx/document.py
--rw-r--r--   0        0        0      662 2023-06-22 22:26:48.267393 chilitools-0.2.4/chilitools/grafx/environment.py
--rw-r--r--   0        0        0        0 2023-07-11 20:57:26.204562 chilitools-0.2.4/chilitools/publisher/__init__.py
--rw-r--r--   0        0        0     2263 2023-07-12 15:49:38.021139 chilitools-0.2.4/chilitools/publisher/document.py
--rw-r--r--   0        0        0        0 2022-04-15 01:52:44.257581 chilitools-0.2.4/chilitools/settings/__init__.py
--rw-r--r--   0        0        0      199 2022-04-15 23:48:49.570757 chilitools-0.2.4/chilitools/settings/config.py
--rw-r--r--   0        0        0    17933 2023-07-31 19:18:35.661107 chilitools-0.2.4/chilitools/utilities/ServerMigration.py
--rw-r--r--   0        0        0        0 2022-04-15 01:52:44.257751 chilitools-0.2.4/chilitools/utilities/__init__.py
--rw-r--r--   0        0        0     2104 2022-10-28 20:09:34.951802 chilitools-0.2.4/chilitools/utilities/backoffice.py
--rw-r--r--   0        0        0      602 2022-04-15 23:48:53.626324 chilitools-0.2.4/chilitools/utilities/defaults.py
--rw-r--r--   0        0        0     2903 2023-07-31 18:31:52.474774 chilitools-0.2.4/chilitools/utilities/document.py
--rw-r--r--   0        0        0      897 2022-07-21 19:16:13.652722 chilitools-0.2.4/chilitools/utilities/errors.py
--rw-r--r--   0        0        0     6022 2022-10-28 20:05:22.841538 chilitools-0.2.4/chilitools/utilities/file.py
--rw-r--r--   0        0        0      807 2023-06-20 15:02:52.753030 chilitools-0.2.4/chilitools/utilities/logger.py
--rw-r--r--   0        0        0      509 2022-06-29 19:01:07.878458 chilitools-0.2.4/chilitools/utilities/strings.py
--rw-r--r--   0        0        0     3831 2023-03-21 15:07:48.139637 chilitools-0.2.4/chilitools/utilities/xmltools.py
--rw-r--r--   0        0        0      505 2023-08-01 18:55:21.533000 chilitools-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      698 1970-01-01 00:00:00.000000 chilitools-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     3655 2023-08-01 18:55:06.483874 chilitools-0.2.5/chilitools/__init__.py
+-rw-r--r--   0        0        0        0 2022-04-15 01:52:44.257043 chilitools-0.2.5/chilitools/api/__init__.py
+-rw-r--r--   0        0        0     7202 2023-07-26 02:58:58.897478 chilitools-0.2.5/chilitools/api/connector.py
+-rw-r--r--   0        0        0    21203 2023-07-31 18:36:41.911804 chilitools-0.2.5/chilitools/api/endpoints.py
+-rw-r--r--   0        0        0     3728 2023-03-21 14:29:37.670561 chilitools-0.2.5/chilitools/api/mycp.py
+-rw-r--r--   0        0        0     3114 2022-09-20 16:25:32.069762 chilitools-0.2.5/chilitools/api/response.py
+-rw-r--r--   0        0        0        0 2023-06-20 02:25:18.519289 chilitools-0.2.5/chilitools/grafx/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-20 19:59:39.899564 chilitools-0.2.5/chilitools/grafx/api/__init__.py
+-rw-r--r--   0        0        0     1610 2023-06-22 21:44:25.944416 chilitools-0.2.5/chilitools/grafx/api/environment.py
+-rw-r--r--   0        0        0      513 2023-06-22 22:42:14.136612 chilitools-0.2.5/chilitools/grafx/api/platform.py
+-rw-r--r--   0        0        0     2584 2023-07-27 16:52:54.465186 chilitools-0.2.5/chilitools/grafx/auth.py
+-rw-r--r--   0        0        0     1941 2023-07-27 16:52:30.339296 chilitools-0.2.5/chilitools/grafx/connector.py
+-rw-r--r--   0        0        0     2370 2023-07-27 17:26:37.658495 chilitools-0.2.5/chilitools/grafx/document.py
+-rw-r--r--   0        0        0      662 2023-06-22 22:26:48.267393 chilitools-0.2.5/chilitools/grafx/environment.py
+-rw-r--r--   0        0        0        0 2023-07-11 20:57:26.204562 chilitools-0.2.5/chilitools/publisher/__init__.py
+-rw-r--r--   0        0        0     2263 2023-07-12 15:49:38.021139 chilitools-0.2.5/chilitools/publisher/document.py
+-rw-r--r--   0        0        0        0 2022-04-15 01:52:44.257581 chilitools-0.2.5/chilitools/settings/__init__.py
+-rw-r--r--   0        0        0      199 2022-04-15 23:48:49.570757 chilitools-0.2.5/chilitools/settings/config.py
+-rw-r--r--   0        0        0    17933 2023-08-01 19:22:39.654439 chilitools-0.2.5/chilitools/utilities/ServerMigration.py
+-rw-r--r--   0        0        0        0 2022-04-15 01:52:44.257751 chilitools-0.2.5/chilitools/utilities/__init__.py
+-rw-r--r--   0        0        0     2104 2022-10-28 20:09:34.951802 chilitools-0.2.5/chilitools/utilities/backoffice.py
+-rw-r--r--   0        0        0      602 2022-04-15 23:48:53.626324 chilitools-0.2.5/chilitools/utilities/defaults.py
+-rw-r--r--   0        0        0     2903 2023-08-01 19:20:34.566598 chilitools-0.2.5/chilitools/utilities/document.py
+-rw-r--r--   0        0        0      897 2022-07-21 19:16:13.652722 chilitools-0.2.5/chilitools/utilities/errors.py
+-rw-r--r--   0        0        0     6022 2022-10-28 20:05:22.841538 chilitools-0.2.5/chilitools/utilities/file.py
+-rw-r--r--   0        0        0      807 2023-06-20 15:02:52.753030 chilitools-0.2.5/chilitools/utilities/logger.py
+-rw-r--r--   0        0        0      509 2022-06-29 19:01:07.878458 chilitools-0.2.5/chilitools/utilities/strings.py
+-rw-r--r--   0        0        0     3831 2023-03-21 15:07:48.139637 chilitools-0.2.5/chilitools/utilities/xmltools.py
+-rw-r--r--   0        0        0      505 2023-08-01 19:23:24.154853 chilitools-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      698 1970-01-01 00:00:00.000000 chilitools-0.2.5/PKG-INFO
```

### Comparing `chilitools-0.2.4/chilitools/__init__.py` & `chilitools-0.2.5/chilitools/__init__.py`

 * *Files identical despite different names*

### Comparing `chilitools-0.2.4/chilitools/api/connector.py` & `chilitools-0.2.5/chilitools/api/connector.py`

 * *Files identical despite different names*

### Comparing `chilitools-0.2.4/chilitools/api/endpoints.py` & `chilitools-0.2.5/chilitools/api/endpoints.py`

 * *Files identical despite different names*

### Comparing `chilitools-0.2.4/chilitools/api/mycp.py` & `chilitools-0.2.5/chilitools/api/mycp.py`

 * *Files identical despite different names*

### Comparing `chilitools-0.2.4/chilitools/api/response.py` & `chilitools-0.2.5/chilitools/api/response.py`

 * *Files identical despite different names*

### Comparing `chilitools-0.2.4/chilitools/grafx/api/environment.py` & `chilitools-0.2.5/chilitools/grafx/api/environment.py`

 * *Files identical despite different names*

### Comparing `chilitools-0.2.4/chilitools/grafx/api/platform.py` & `chilitools-0.2.5/chilitools/grafx/api/platform.py`

 * *Files identical despite different names*

### Comparing `chilitools-0.2.4/chilitools/grafx/auth.py` & `chilitools-0.2.5/chilitools/grafx/auth.py`

 * *Files identical despite different names*

### Comparing `chilitools-0.2.4/chilitools/grafx/connector.py` & `chilitools-0.2.5/chilitools/grafx/connector.py`

 * *Files identical despite different names*

### Comparing `chilitools-0.2.4/chilitools/grafx/document.py` & `chilitools-0.2.5/chilitools/grafx/document.py`

 * *Files identical despite different names*

### Comparing `chilitools-0.2.4/chilitools/grafx/environment.py` & `chilitools-0.2.5/chilitools/grafx/environment.py`

 * *Files identical despite different names*

### Comparing `chilitools-0.2.4/chilitools/publisher/document.py` & `chilitools-0.2.5/chilitools/publisher/document.py`

 * *Files identical despite different names*

### Comparing `chilitools-0.2.4/chilitools/utilities/ServerMigration.py` & `chilitools-0.2.5/chilitools/utilities/ServerMigration.py`

 * *Files 0% similar despite different names*

```diff
@@ -231,15 +231,15 @@
 
           fonts = []
           for font in cd.get_fonts():
             fonts.append(font["id"])
 
           assets = cd.get_images()
           images = [image.get("id") for image in assets if image.get("resource_type") == "Assets"]
-          daps = [image.get("id") for image in assets if image.get("resource_type" == "DynamicAssetProviders")]
+          daps = [image.get("id") for image in assets if image.get("resource_type") == "DynamicAssetProviders"]
           barcodes = cd.get_barcode_ids()
 
 
           if fonts:
             self.logger.info(f"Found fonts in document, transferring... (Arial Regular will probably fail)")
             self.transferList(itemList=fonts, resource="Fonts")
           if images:
```

### Comparing `chilitools-0.2.4/chilitools/utilities/backoffice.py` & `chilitools-0.2.5/chilitools/utilities/backoffice.py`

 * *Files identical despite different names*

### Comparing `chilitools-0.2.4/chilitools/utilities/defaults.py` & `chilitools-0.2.5/chilitools/utilities/defaults.py`

 * *Files identical despite different names*

### Comparing `chilitools-0.2.4/chilitools/utilities/document.py` & `chilitools-0.2.5/chilitools/utilities/document.py`

 * *Files identical despite different names*

### Comparing `chilitools-0.2.4/chilitools/utilities/errors.py` & `chilitools-0.2.5/chilitools/utilities/errors.py`

 * *Files identical despite different names*

### Comparing `chilitools-0.2.4/chilitools/utilities/file.py` & `chilitools-0.2.5/chilitools/utilities/file.py`

 * *Files identical despite different names*

### Comparing `chilitools-0.2.4/chilitools/utilities/logger.py` & `chilitools-0.2.5/chilitools/utilities/logger.py`

 * *Files identical despite different names*

### Comparing `chilitools-0.2.4/chilitools/utilities/xmltools.py` & `chilitools-0.2.5/chilitools/utilities/xmltools.py`

 * *Files identical despite different names*

### Comparing `chilitools-0.2.4/PKG-INFO` & `chilitools-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chilitools
-Version: 0.2.4
+Version: 0.2.5
 Summary: A collection of tools for working with CHILI products
 Author: Austin
 Author-email: austin.meier@hotmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

