# Comparing `tmp/getblocks-2023.5.31.tar.gz` & `tmp/getblocks-2023.7.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getblocks-2023.5.31.tar", last modified: Thu Jun  1 01:14:18 2023, max compression
+gzip compressed data, was "getblocks-2023.7.31.tar", last modified: Tue Aug  1 00:59:58 2023, max compression
```

## Comparing `getblocks-2023.5.31.tar` & `getblocks-2023.7.31.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 01:14:18.826974 getblocks-2023.5.31/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-01 01:14:07.000000 getblocks-2023.5.31/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-06-01 01:14:18.826974 getblocks-2023.5.31/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-06-01 01:14:07.000000 getblocks-2023.5.31/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 01:14:18.826974 getblocks-2023.5.31/getblocks/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-01 01:14:07.000000 getblocks-2023.5.31/getblocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-01 01:14:07.000000 getblocks-2023.5.31/getblocks/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8566 2023-06-01 01:14:07.000000 getblocks-2023.5.31/getblocks/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 01:14:18.826974 getblocks-2023.5.31/getblocks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-06-01 01:14:18.000000 getblocks-2023.5.31/getblocks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-01 01:14:18.000000 getblocks-2023.5.31/getblocks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 01:14:18.000000 getblocks-2023.5.31/getblocks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-01 01:14:18.000000 getblocks-2023.5.31/getblocks.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 01:14:18.000000 getblocks-2023.5.31/getblocks.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-01 01:14:18.000000 getblocks-2023.5.31/getblocks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-01 01:14:18.000000 getblocks-2023.5.31/getblocks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 01:14:18.826974 getblocks-2023.5.31/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-01 01:14:07.000000 getblocks-2023.5.31/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:59:58.726213 getblocks-2023.7.31/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-01 00:59:48.000000 getblocks-2023.7.31/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-08-01 00:59:58.726213 getblocks-2023.7.31/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-08-01 00:59:48.000000 getblocks-2023.7.31/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:59:58.722213 getblocks-2023.7.31/getblocks/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-01 00:59:48.000000 getblocks-2023.7.31/getblocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-08-01 00:59:48.000000 getblocks-2023.7.31/getblocks/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8566 2023-08-01 00:59:48.000000 getblocks-2023.7.31/getblocks/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:59:58.726213 getblocks-2023.7.31/getblocks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-08-01 00:59:58.000000 getblocks-2023.7.31/getblocks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-08-01 00:59:58.000000 getblocks-2023.7.31/getblocks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 00:59:58.000000 getblocks-2023.7.31/getblocks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-01 00:59:58.000000 getblocks-2023.7.31/getblocks.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 00:59:58.000000 getblocks-2023.7.31/getblocks.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-01 00:59:58.000000 getblocks-2023.7.31/getblocks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-01 00:59:58.000000 getblocks-2023.7.31/getblocks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 00:59:58.726213 getblocks-2023.7.31/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-08-01 00:59:48.000000 getblocks-2023.7.31/setup.py
```

### Comparing `getblocks-2023.5.31/LICENSE` & `getblocks-2023.7.31/LICENSE`

 * *Files identical despite different names*

### Comparing `getblocks-2023.5.31/PKG-INFO` & `getblocks-2023.7.31/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getblocks
-Version: 2023.5.31
+Version: 2023.7.31
 Summary: Down to the smallest sector detail!
 Home-page: https://github.com/jblukach/getblocks
 Author: John Lukach
 Author-email: hello@lukach.io
 License: Apache-2.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `getblocks-2023.5.31/README.md` & `getblocks-2023.7.31/README.md`

 * *Files identical despite different names*

### Comparing `getblocks-2023.5.31/getblocks/cli.py` & `getblocks-2023.7.31/getblocks/cli.py`

 * *Files identical despite different names*

### Comparing `getblocks-2023.5.31/getblocks.egg-info/PKG-INFO` & `getblocks-2023.7.31/getblocks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getblocks
-Version: 2023.5.31
+Version: 2023.7.31
 Summary: Down to the smallest sector detail!
 Home-page: https://github.com/jblukach/getblocks
 Author: John Lukach
 Author-email: hello@lukach.io
 License: Apache-2.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `getblocks-2023.5.31/setup.py` & `getblocks-2023.7.31/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     author_email = "hello@lukach.io",
     license = "Apache-2.0",
     packages = [
         "getblocks"
     ],
     install_requires = [
         "blake3",
-        "requests"
+        "requests==2.29.0"
     ],
     zip_safe = False,
     entry_points = {
         "console_scripts": [
             "getblocks=getblocks.cli:main"
         ],
     },
```

