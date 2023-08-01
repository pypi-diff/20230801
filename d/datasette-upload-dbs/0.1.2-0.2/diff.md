# Comparing `tmp/datasette-upload-dbs-0.1.2.tar.gz` & `tmp/datasette-upload-dbs-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasette-upload-dbs-0.1.2.tar", last modified: Fri Sep  9 15:59:50 2022, max compression
+gzip compressed data, was "datasette-upload-dbs-0.2.tar", last modified: Tue Aug  1 17:13:55 2023, max compression
```

## Comparing `datasette-upload-dbs-0.1.2.tar` & `datasette-upload-dbs-0.2.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 15:59:50.009556 datasette-upload-dbs-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-09-09 15:59:31.000000 datasette-upload-dbs-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3505 2022-09-09 15:59:50.009556 datasette-upload-dbs-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2840 2022-09-09 15:59:31.000000 datasette-upload-dbs-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 15:59:50.005556 datasette-upload-dbs-0.1.2/datasette_upload_dbs/
--rw-r--r--   0 runner    (1001) docker     (121)     3880 2022-09-09 15:59:31.000000 datasette-upload-dbs-0.1.2/datasette_upload_dbs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 15:59:50.009556 datasette-upload-dbs-0.1.2/datasette_upload_dbs/templates/
--rw-r--r--   0 runner    (1001) docker     (121)     4712 2022-09-09 15:59:31.000000 datasette-upload-dbs-0.1.2/datasette_upload_dbs/templates/upload_dbs.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 15:59:50.009556 datasette-upload-dbs-0.1.2/datasette_upload_dbs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3505 2022-09-09 15:59:49.000000 datasette-upload-dbs-0.1.2/datasette_upload_dbs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      372 2022-09-09 15:59:50.000000 datasette-upload-dbs-0.1.2/datasette_upload_dbs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-09 15:59:49.000000 datasette-upload-dbs-0.1.2/datasette_upload_dbs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-09-09 15:59:49.000000 datasette-upload-dbs-0.1.2/datasette_upload_dbs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-09-09 15:59:49.000000 datasette-upload-dbs-0.1.2/datasette_upload_dbs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-09-09 15:59:49.000000 datasette-upload-dbs-0.1.2/datasette_upload_dbs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-09 15:59:50.009556 datasette-upload-dbs-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1278 2022-09-09 15:59:31.000000 datasette-upload-dbs-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:13:55.074122 datasette-upload-dbs-0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-01 17:13:40.000000 datasette-upload-dbs-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-08-01 17:13:55.074122 datasette-upload-dbs-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-08-01 17:13:40.000000 datasette-upload-dbs-0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:13:55.070122 datasette-upload-dbs-0.2/datasette_upload_dbs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-08-01 17:13:40.000000 datasette-upload-dbs-0.2/datasette_upload_dbs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:13:55.074122 datasette-upload-dbs-0.2/datasette_upload_dbs/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-08-01 17:13:40.000000 datasette-upload-dbs-0.2/datasette_upload_dbs/templates/upload_dbs.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:13:55.074122 datasette-upload-dbs-0.2/datasette_upload_dbs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-08-01 17:13:55.000000 datasette-upload-dbs-0.2/datasette_upload_dbs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-08-01 17:13:55.000000 datasette-upload-dbs-0.2/datasette_upload_dbs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 17:13:55.000000 datasette-upload-dbs-0.2/datasette_upload_dbs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-01 17:13:55.000000 datasette-upload-dbs-0.2/datasette_upload_dbs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-01 17:13:55.000000 datasette-upload-dbs-0.2/datasette_upload_dbs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-01 17:13:55.000000 datasette-upload-dbs-0.2/datasette_upload_dbs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 17:13:55.074122 datasette-upload-dbs-0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-08-01 17:13:40.000000 datasette-upload-dbs-0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:13:55.074122 datasette-upload-dbs-0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-08-01 17:13:40.000000 datasette-upload-dbs-0.2/tests/test_upload_dbs.py
```

### Comparing `datasette-upload-dbs-0.1.2/LICENSE` & `datasette-upload-dbs-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `datasette-upload-dbs-0.1.2/PKG-INFO` & `datasette-upload-dbs-0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-upload-dbs
-Version: 0.1.2
+Version: 0.2
 Summary: Upload SQLite database files to Datasette
 Home-page: https://github.com/simonw/datasette-upload-dbs
 Author: Simon Willison
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/simonw/datasette-upload-dbs/issues
 Project-URL: CI, https://github.com/simonw/datasette-upload-dbs/actions
 Project-URL: Changelog, https://github.com/simonw/datasette-upload-dbs/releases
@@ -57,14 +57,20 @@
 ```
 You can use `"."` for the current folder when the server starts, or `"uploads"` for a folder relative to that folder. The folder will be created on startup if it does not already exist.
 
 Then start Datasette like this:
 
     datasette -m metadata.yml
 
+The plugin defaults to loading all databases in the configured directory.
+
+You can disable this by adding the following setting:
+```
+"skip_startup_scan": true
+```
 ## Usage
 
 Only users with the `upload-dbs` permission will be able to upload files. The `root` user has this permission by default - other users can be granted access using permission plugins, see the [Permissions](https://docs.datasette.io/en/stable/authentication.html#permissions) documentation for details.
 
 To start Datasette as the root user, run this:
 
     datasette -m metadata.yml --root
```

### Comparing `datasette-upload-dbs-0.1.2/README.md` & `datasette-upload-dbs-0.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -40,14 +40,20 @@
 ```
 You can use `"."` for the current folder when the server starts, or `"uploads"` for a folder relative to that folder. The folder will be created on startup if it does not already exist.
 
 Then start Datasette like this:
 
     datasette -m metadata.yml
 
+The plugin defaults to loading all databases in the configured directory.
+
+You can disable this by adding the following setting:
+```
+"skip_startup_scan": true
+```
 ## Usage
 
 Only users with the `upload-dbs` permission will be able to upload files. The `root` user has this permission by default - other users can be granted access using permission plugins, see the [Permissions](https://docs.datasette.io/en/stable/authentication.html#permissions) documentation for details.
 
 To start Datasette as the root user, run this:
 
     datasette -m metadata.yml --root
```

### Comparing `datasette-upload-dbs-0.1.2/datasette_upload_dbs/__init__.py` & `datasette-upload-dbs-0.2/datasette_upload_dbs/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,20 +37,25 @@
 
     return inner
 
 
 @hookimpl
 def startup(datasette):
     # Load any databases located in the directory folder
-    directory = _configured(datasette)
+    config = datasette.plugin_config("datasette-upload-dbs") or {}
+    if config.get("skip_startup_scan"):
+        return
+    directory = config.get("directory")
     if not directory:
         return
     path = pathlib.Path(directory)
     database_files = path.glob("*.db")
     for file_path in database_files:
+        # Needs to set is_mutable=True here because the default was False
+        # in Datasette versions up to and including 0.62
         datasette.add_database(
             Database(datasette, path=str(file_path), is_mutable=True),
         )
 
 
 def _configured(datasette):
     return (datasette.plugin_config("datasette-upload-dbs") or {}).get("directory")
```

### Comparing `datasette-upload-dbs-0.1.2/datasette_upload_dbs/templates/upload_dbs.html` & `datasette-upload-dbs-0.2/datasette_upload_dbs/templates/upload_dbs.html`

 * *Files identical despite different names*

### Comparing `datasette-upload-dbs-0.1.2/datasette_upload_dbs.egg-info/PKG-INFO` & `datasette-upload-dbs-0.2/datasette_upload_dbs.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-upload-dbs
-Version: 0.1.2
+Version: 0.2
 Summary: Upload SQLite database files to Datasette
 Home-page: https://github.com/simonw/datasette-upload-dbs
 Author: Simon Willison
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/simonw/datasette-upload-dbs/issues
 Project-URL: CI, https://github.com/simonw/datasette-upload-dbs/actions
 Project-URL: Changelog, https://github.com/simonw/datasette-upload-dbs/releases
@@ -57,14 +57,20 @@
 ```
 You can use `"."` for the current folder when the server starts, or `"uploads"` for a folder relative to that folder. The folder will be created on startup if it does not already exist.
 
 Then start Datasette like this:
 
     datasette -m metadata.yml
 
+The plugin defaults to loading all databases in the configured directory.
+
+You can disable this by adding the following setting:
+```
+"skip_startup_scan": true
+```
 ## Usage
 
 Only users with the `upload-dbs` permission will be able to upload files. The `root` user has this permission by default - other users can be granted access using permission plugins, see the [Permissions](https://docs.datasette.io/en/stable/authentication.html#permissions) documentation for details.
 
 To start Datasette as the root user, run this:
 
     datasette -m metadata.yml --root
```

### Comparing `datasette-upload-dbs-0.1.2/setup.py` & `datasette-upload-dbs-0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import os
 
-VERSION = "0.1.2"
+VERSION = "0.2"
 
 
 def get_long_description():
     with open(
         os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"),
         encoding="utf8",
     ) as fp:
```

