# Comparing `tmp/mdast_cli-2023.7.2.tar.gz` & `tmp/mdast_cli-2023.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdast_cli-2023.7.2.tar", last modified: Mon Jul 10 23:46:09 2023, max compression
+gzip compressed data, was "mdast_cli-2023.8.1.tar", last modified: Tue Aug  1 13:51:31 2023, max compression
```

## Comparing `mdast_cli-2023.7.2.tar` & `mdast_cli-2023.8.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 23:46:09.502159 mdast_cli-2023.7.2/
--rw-r--r--   0 runner    (1001) docker     (122)    28412 2023-07-10 23:46:09.502159 mdast_cli-2023.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    28048 2023-07-10 23:45:51.000000 mdast_cli-2023.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 23:46:09.494159 mdast_cli-2023.7.2/mdast_cli/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-10 23:45:51.000000 mdast_cli-2023.7.2/mdast_cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 23:46:09.498159 mdast_cli-2023.7.2/mdast_cli/distribution_systems/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-10 23:45:51.000000 mdast_cli-2023.7.2/mdast_cli/distribution_systems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3656 2023-07-10 23:45:51.000000 mdast_cli-2023.7.2/mdast_cli/distribution_systems/app_center.py
--rw-r--r--   0 runner    (1001) docker     (122)     3292 2023-07-10 23:45:51.000000 mdast_cli-2023.7.2/mdast_cli/distribution_systems/appgallery.py
--rw-r--r--   0 runner    (1001) docker     (122)     7136 2023-07-10 23:45:51.000000 mdast_cli-2023.7.2/mdast_cli/distribution_systems/appstore.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 23:46:09.498159 mdast_cli-2023.7.2/mdast_cli/distribution_systems/appstore_client/
--rwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 23:45:51.000000 mdast_cli-2023.7.2/mdast_cli/distribution_systems/appstore_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 23:46:09.498159 mdast_cli-2023.7.2/mdast_cli/distribution_systems/appstore_client/schemas/
--rwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 23:45:51.000000 mdast_cli-2023.7.2/mdast_cli/distribution_systems/appstore_client/schemas/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     7464 2023-07-10 23:45:51.000000 mdast_cli-2023.7.2/mdast_cli/distribution_systems/appstore_client/schemas/store_authenticate_req.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    99797 2023-07-10 23:45:51.000000 mdast_cli-2023.7.2/mdast_cli/distribution_systems/appstore_client/schemas/store_authenticate_resp.py
--rw-r--r--   0 runner    (1001) docker     (122)    27325 2023-07-10 23:45:51.000000 mdast_cli-2023.7.2/mdast_cli/distribution_systems/appstore_client/schemas/store_buyproduct_req.py
--rw-r--r--   0 runner    (1001) docker     (122)   217008 2023-07-10 23:45:51.000000 mdast_cli-2023.7.2/mdast_cli/distribution_systems/appstore_client/schemas/store_buyproduct_resp.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     5001 2023-07-10 23:45:51.000000 mdast_cli-2023.7.2/mdast_cli/distribution_systems/appstore_client/schemas/store_download_req.py
--rwxr-xr-x   0 runner    (1001) docker     (122)   150706 2023-07-10 23:45:51.000000 mdast_cli-2023.7.2/mdast_cli/distribution_systems/appstore_client/schemas/store_download_resp.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     5628 2023-07-10 23:45:51.000000 mdast_cli-2023.7.2/mdast_cli/distribution_systems/appstore_client/store.py
--rw-r--r--   0 runner    (1001) docker     (122)     3133 2023-07-10 23:45:51.000000 mdast_cli-2023.7.2/mdast_cli/distribution_systems/firebase.py
--rw-r--r--   0 runner    (1001) docker     (122)     5093 2023-07-10 23:45:51.000000 mdast_cli-2023.7.2/mdast_cli/distribution_systems/google_play.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 23:46:09.502159 mdast_cli-2023.7.2/mdast_cli/distribution_systems/gpapi/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-10 23:45:51.000000 mdast_cli-2023.7.2/mdast_cli/distribution_systems/gpapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9033 2023-07-10 23:45:51.000000 mdast_cli-2023.7.2/mdast_cli/distribution_systems/gpapi/config.py
--rw-r--r--   0 runner    (1001) docker     (122)   305712 2023-07-10 23:45:51.000000 mdast_cli-2023.7.2/mdast_cli/distribution_systems/gpapi/device.properties
--rw-r--r--   0 runner    (1001) docker     (122)    15572 2023-07-10 23:45:51.000000 mdast_cli-2023.7.2/mdast_cli/distribution_systems/gpapi/googleplay.py
--rw-r--r--   0 runner    (1001) docker     (122)    65347 2023-07-10 23:45:51.000000 mdast_cli-2023.7.2/mdast_cli/distribution_systems/gpapi/googleplay_pb2.py
--rw-r--r--   0 runner    (1001) docker     (122)      457 2023-07-10 23:45:51.000000 mdast_cli-2023.7.2/mdast_cli/distribution_systems/gpapi/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     3380 2023-07-10 23:45:51.000000 mdast_cli-2023.7.2/mdast_cli/distribution_systems/nexus.py
--rw-r--r--   0 runner    (1001) docker     (122)     2632 2023-07-10 23:45:51.000000 mdast_cli-2023.7.2/mdast_cli/distribution_systems/nexus2.py
--rw-r--r--   0 runner    (1001) docker     (122)     2622 2023-07-10 23:45:51.000000 mdast_cli-2023.7.2/mdast_cli/distribution_systems/rustore.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 23:46:09.502159 mdast_cli-2023.7.2/mdast_cli/helpers/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-10 23:45:51.000000 mdast_cli-2023.7.2/mdast_cli/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      623 2023-07-10 23:45:51.000000 mdast_cli-2023.7.2/mdast_cli/helpers/const.py
--rw-r--r--   0 runner    (1001) docker     (122)      395 2023-07-10 23:45:51.000000 mdast_cli-2023.7.2/mdast_cli/helpers/helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)    36537 2023-07-10 23:45:51.000000 mdast_cli-2023.7.2/mdast_cli/mdast_scan.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 23:46:09.498159 mdast_cli-2023.7.2/mdast_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    28412 2023-07-10 23:46:09.000000 mdast_cli-2023.7.2/mdast_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1806 2023-07-10 23:46:09.000000 mdast_cli-2023.7.2/mdast_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-10 23:46:09.000000 mdast_cli-2023.7.2/mdast_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-07-10 23:46:09.000000 mdast_cli-2023.7.2/mdast_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      521 2023-07-10 23:46:09.000000 mdast_cli-2023.7.2/mdast_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-10 23:46:09.000000 mdast_cli-2023.7.2/mdast_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 23:46:09.502159 mdast_cli-2023.7.2/mdast_cli_core/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-10 23:45:51.000000 mdast_cli-2023.7.2/mdast_cli_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2144 2023-07-10 23:45:51.000000 mdast_cli-2023.7.2/mdast_cli_core/api.py
--rw-r--r--   0 runner    (1001) docker     (122)    24046 2023-07-10 23:45:51.000000 mdast_cli-2023.7.2/mdast_cli_core/base.py
--rw-r--r--   0 runner    (1001) docker     (122)      560 2023-07-10 23:45:51.000000 mdast_cli-2023.7.2/mdast_cli_core/token.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-10 23:46:09.502159 mdast_cli-2023.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1651 2023-07-10 23:45:51.000000 mdast_cli-2023.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 13:51:31.185495 mdast_cli-2023.8.1/
+-rw-r--r--   0 runner    (1001) docker     (122)    28412 2023-08-01 13:51:31.185495 mdast_cli-2023.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    28048 2023-08-01 13:51:08.000000 mdast_cli-2023.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 13:51:31.177495 mdast_cli-2023.8.1/mdast_cli/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-01 13:51:08.000000 mdast_cli-2023.8.1/mdast_cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 13:51:31.181495 mdast_cli-2023.8.1/mdast_cli/distribution_systems/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-01 13:51:08.000000 mdast_cli-2023.8.1/mdast_cli/distribution_systems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3656 2023-08-01 13:51:08.000000 mdast_cli-2023.8.1/mdast_cli/distribution_systems/app_center.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3292 2023-08-01 13:51:08.000000 mdast_cli-2023.8.1/mdast_cli/distribution_systems/appgallery.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7136 2023-08-01 13:51:08.000000 mdast_cli-2023.8.1/mdast_cli/distribution_systems/appstore.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 13:51:31.181495 mdast_cli-2023.8.1/mdast_cli/distribution_systems/appstore_client/
+-rwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 13:51:08.000000 mdast_cli-2023.8.1/mdast_cli/distribution_systems/appstore_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 13:51:31.181495 mdast_cli-2023.8.1/mdast_cli/distribution_systems/appstore_client/schemas/
+-rwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 13:51:08.000000 mdast_cli-2023.8.1/mdast_cli/distribution_systems/appstore_client/schemas/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     7464 2023-08-01 13:51:08.000000 mdast_cli-2023.8.1/mdast_cli/distribution_systems/appstore_client/schemas/store_authenticate_req.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    99797 2023-08-01 13:51:08.000000 mdast_cli-2023.8.1/mdast_cli/distribution_systems/appstore_client/schemas/store_authenticate_resp.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27325 2023-08-01 13:51:08.000000 mdast_cli-2023.8.1/mdast_cli/distribution_systems/appstore_client/schemas/store_buyproduct_req.py
+-rw-r--r--   0 runner    (1001) docker     (122)   217008 2023-08-01 13:51:08.000000 mdast_cli-2023.8.1/mdast_cli/distribution_systems/appstore_client/schemas/store_buyproduct_resp.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5001 2023-08-01 13:51:08.000000 mdast_cli-2023.8.1/mdast_cli/distribution_systems/appstore_client/schemas/store_download_req.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)   150706 2023-08-01 13:51:08.000000 mdast_cli-2023.8.1/mdast_cli/distribution_systems/appstore_client/schemas/store_download_resp.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5628 2023-08-01 13:51:08.000000 mdast_cli-2023.8.1/mdast_cli/distribution_systems/appstore_client/store.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3133 2023-08-01 13:51:08.000000 mdast_cli-2023.8.1/mdast_cli/distribution_systems/firebase.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5093 2023-08-01 13:51:08.000000 mdast_cli-2023.8.1/mdast_cli/distribution_systems/google_play.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 13:51:31.185495 mdast_cli-2023.8.1/mdast_cli/distribution_systems/gpapi/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-01 13:51:08.000000 mdast_cli-2023.8.1/mdast_cli/distribution_systems/gpapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9033 2023-08-01 13:51:08.000000 mdast_cli-2023.8.1/mdast_cli/distribution_systems/gpapi/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)   305712 2023-08-01 13:51:08.000000 mdast_cli-2023.8.1/mdast_cli/distribution_systems/gpapi/device.properties
+-rw-r--r--   0 runner    (1001) docker     (122)    15572 2023-08-01 13:51:08.000000 mdast_cli-2023.8.1/mdast_cli/distribution_systems/gpapi/googleplay.py
+-rw-r--r--   0 runner    (1001) docker     (122)    65347 2023-08-01 13:51:08.000000 mdast_cli-2023.8.1/mdast_cli/distribution_systems/gpapi/googleplay_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)      457 2023-08-01 13:51:08.000000 mdast_cli-2023.8.1/mdast_cli/distribution_systems/gpapi/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3380 2023-08-01 13:51:08.000000 mdast_cli-2023.8.1/mdast_cli/distribution_systems/nexus.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2632 2023-08-01 13:51:08.000000 mdast_cli-2023.8.1/mdast_cli/distribution_systems/nexus2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2622 2023-08-01 13:51:08.000000 mdast_cli-2023.8.1/mdast_cli/distribution_systems/rustore.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 13:51:31.185495 mdast_cli-2023.8.1/mdast_cli/helpers/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-01 13:51:08.000000 mdast_cli-2023.8.1/mdast_cli/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      623 2023-08-01 13:51:08.000000 mdast_cli-2023.8.1/mdast_cli/helpers/const.py
+-rw-r--r--   0 runner    (1001) docker     (122)      395 2023-08-01 13:51:08.000000 mdast_cli-2023.8.1/mdast_cli/helpers/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36794 2023-08-01 13:51:08.000000 mdast_cli-2023.8.1/mdast_cli/mdast_scan.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 13:51:31.181495 mdast_cli-2023.8.1/mdast_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    28412 2023-08-01 13:51:31.000000 mdast_cli-2023.8.1/mdast_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1806 2023-08-01 13:51:31.000000 mdast_cli-2023.8.1/mdast_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-01 13:51:31.000000 mdast_cli-2023.8.1/mdast_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-08-01 13:51:31.000000 mdast_cli-2023.8.1/mdast_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      521 2023-08-01 13:51:31.000000 mdast_cli-2023.8.1/mdast_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-08-01 13:51:31.000000 mdast_cli-2023.8.1/mdast_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 13:51:31.185495 mdast_cli-2023.8.1/mdast_cli_core/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-01 13:51:08.000000 mdast_cli-2023.8.1/mdast_cli_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2144 2023-08-01 13:51:08.000000 mdast_cli-2023.8.1/mdast_cli_core/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24046 2023-08-01 13:51:08.000000 mdast_cli-2023.8.1/mdast_cli_core/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)      560 2023-08-01 13:51:08.000000 mdast_cli-2023.8.1/mdast_cli_core/token.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-08-01 13:51:31.185495 mdast_cli-2023.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1651 2023-08-01 13:51:08.000000 mdast_cli-2023.8.1/setup.py
```

### Comparing `mdast_cli-2023.7.2/PKG-INFO` & `mdast_cli-2023.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdast_cli
-Version: 2023.7.2
+Version: 2023.8.1
 Summary: Dynamic-Mobile-Security
 Home-page: https://github.com/Dynamic-Mobile-Security/mdast-cli
 Author: Dynamic-Mobile-Security
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Description-Content-Type: text/markdown
```

### Comparing `mdast_cli-2023.7.2/README.md` & `mdast_cli-2023.8.1/README.md`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.7.2/mdast_cli/distribution_systems/app_center.py` & `mdast_cli-2023.8.1/mdast_cli/distribution_systems/app_center.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.7.2/mdast_cli/distribution_systems/appgallery.py` & `mdast_cli-2023.8.1/mdast_cli/distribution_systems/appgallery.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.7.2/mdast_cli/distribution_systems/appstore.py` & `mdast_cli-2023.8.1/mdast_cli/distribution_systems/appstore.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.7.2/mdast_cli/distribution_systems/appstore_client/schemas/store_authenticate_req.py` & `mdast_cli-2023.8.1/mdast_cli/distribution_systems/appstore_client/schemas/store_authenticate_req.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.7.2/mdast_cli/distribution_systems/appstore_client/schemas/store_authenticate_resp.py` & `mdast_cli-2023.8.1/mdast_cli/distribution_systems/appstore_client/schemas/store_authenticate_resp.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.7.2/mdast_cli/distribution_systems/appstore_client/schemas/store_buyproduct_req.py` & `mdast_cli-2023.8.1/mdast_cli/distribution_systems/appstore_client/schemas/store_buyproduct_req.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.7.2/mdast_cli/distribution_systems/appstore_client/schemas/store_buyproduct_resp.py` & `mdast_cli-2023.8.1/mdast_cli/distribution_systems/appstore_client/schemas/store_buyproduct_resp.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.7.2/mdast_cli/distribution_systems/appstore_client/schemas/store_download_req.py` & `mdast_cli-2023.8.1/mdast_cli/distribution_systems/appstore_client/schemas/store_download_req.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.7.2/mdast_cli/distribution_systems/appstore_client/schemas/store_download_resp.py` & `mdast_cli-2023.8.1/mdast_cli/distribution_systems/appstore_client/schemas/store_download_resp.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.7.2/mdast_cli/distribution_systems/appstore_client/store.py` & `mdast_cli-2023.8.1/mdast_cli/distribution_systems/appstore_client/store.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.7.2/mdast_cli/distribution_systems/firebase.py` & `mdast_cli-2023.8.1/mdast_cli/distribution_systems/firebase.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.7.2/mdast_cli/distribution_systems/google_play.py` & `mdast_cli-2023.8.1/mdast_cli/distribution_systems/google_play.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.7.2/mdast_cli/distribution_systems/gpapi/config.py` & `mdast_cli-2023.8.1/mdast_cli/distribution_systems/gpapi/config.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.7.2/mdast_cli/distribution_systems/gpapi/device.properties` & `mdast_cli-2023.8.1/mdast_cli/distribution_systems/gpapi/device.properties`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.7.2/mdast_cli/distribution_systems/gpapi/googleplay.py` & `mdast_cli-2023.8.1/mdast_cli/distribution_systems/gpapi/googleplay.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.7.2/mdast_cli/distribution_systems/gpapi/googleplay_pb2.py` & `mdast_cli-2023.8.1/mdast_cli/distribution_systems/gpapi/googleplay_pb2.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.7.2/mdast_cli/distribution_systems/nexus.py` & `mdast_cli-2023.8.1/mdast_cli/distribution_systems/nexus.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.7.2/mdast_cli/distribution_systems/nexus2.py` & `mdast_cli-2023.8.1/mdast_cli/distribution_systems/nexus2.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.7.2/mdast_cli/distribution_systems/rustore.py` & `mdast_cli-2023.8.1/mdast_cli/distribution_systems/rustore.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.7.2/mdast_cli/helpers/const.py` & `mdast_cli-2023.8.1/mdast_cli/helpers/const.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.7.2/mdast_cli/mdast_scan.py` & `mdast_cli-2023.8.1/mdast_cli/mdast_scan.py`

 * *Files 1% similar despite different names*

```diff
@@ -421,14 +421,18 @@
         get_testcase_resp = mdast.get_testcase(testcase_id)
         if get_testcase_resp.status_code == 200:
             architecture = get_testcase_resp.json()['architecture']['id']
         else:
             logger.warning("Testcase with this id does not exist or you use old version of system. Trying to use "
                            "architecture from command line params.")
 
+    if sum(e['architecture'] == architecture_type['id'] and e['state'] == 3 for e in mdast.get_engines().json()) == 0:
+        logger.error(f"Cannot create scan - Cannot find active engine for architecture {architecture_type['name']}")
+        sys.exit(1)
+
     if testcase_id:
         logger.info(f'Autoscan(Stingray) with test case id: '
                     f'{testcase_id}, profile id: {profile_id} and file: {app_file}, architecture id is {architecture}')
     elif appium_script_path:
         logger.info(f'Autoscan(Appium) with  profile id: {profile_id} and file: {app_file},'
                     f' architecture id is {architecture}')
     else:
```

### Comparing `mdast_cli-2023.7.2/mdast_cli.egg-info/PKG-INFO` & `mdast_cli-2023.8.1/mdast_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdast-cli
-Version: 2023.7.2
+Version: 2023.8.1
 Summary: Dynamic-Mobile-Security
 Home-page: https://github.com/Dynamic-Mobile-Security/mdast-cli
 Author: Dynamic-Mobile-Security
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Description-Content-Type: text/markdown
```

### Comparing `mdast_cli-2023.7.2/mdast_cli.egg-info/SOURCES.txt` & `mdast_cli-2023.8.1/mdast_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.7.2/mdast_cli.egg-info/requires.txt` & `mdast_cli-2023.8.1/mdast_cli.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.7.2/mdast_cli_core/api.py` & `mdast_cli-2023.8.1/mdast_cli_core/api.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.7.2/mdast_cli_core/base.py` & `mdast_cli-2023.8.1/mdast_cli_core/base.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.7.2/mdast_cli_core/token.py` & `mdast_cli-2023.8.1/mdast_cli_core/token.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.7.2/setup.py` & `mdast_cli-2023.8.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="mdast_cli",
 
 
-    version='2023.07.02',
+    version='2023.08.01',
 
 
 
     author="Dynamic-Mobile-Security",
     description="Dynamic-Mobile-Security",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

