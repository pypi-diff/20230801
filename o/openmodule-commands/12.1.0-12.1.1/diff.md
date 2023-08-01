# Comparing `tmp/openmodule_commands-12.1.0.tar.gz` & `tmp/openmodule_commands-12.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openmodule_commands-12.1.0.tar", last modified: Thu Jul 27 09:13:13 2023, max compression
+gzip compressed data, was "openmodule_commands-12.1.1.tar", last modified: Tue Aug  1 07:43:48 2023, max compression
```

## Comparing `openmodule_commands-12.1.0.tar` & `openmodule_commands-12.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 09:13:13.077448 openmodule_commands-12.1.0/
--rw-r--r--   0 root         (0) root         (0)      338 2023-07-27 09:13:12.000000 openmodule_commands-12.1.0/AUTHORS
--rw-r--r--   0 root         (0) root         (0)     8268 2023-07-27 09:13:12.000000 openmodule_commands-12.1.0/ChangeLog
--rw-r--r--   0 root         (0) root         (0)      618 2023-07-27 09:13:13.077448 openmodule_commands-12.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2826 2023-06-29 09:50:19.000000 openmodule_commands-12.1.0/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 09:13:13.077448 openmodule_commands-12.1.0/openmodule_commands.egg-info/
--rw-r--r--   0 root         (0) root         (0)      618 2023-07-27 09:13:12.000000 openmodule_commands-12.1.0/openmodule_commands.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      363 2023-07-27 09:13:13.000000 openmodule_commands-12.1.0/openmodule_commands.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 09:13:12.000000 openmodule_commands-12.1.0/openmodule_commands.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      232 2023-07-27 09:13:12.000000 openmodule_commands-12.1.0/openmodule_commands.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 09:13:12.000000 openmodule_commands-12.1.0/openmodule_commands.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       46 2023-07-27 09:13:12.000000 openmodule_commands-12.1.0/openmodule_commands.egg-info/pbr.json
--rw-r--r--   0 root         (0) root         (0)       20 2023-07-27 09:13:12.000000 openmodule_commands-12.1.0/openmodule_commands.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      850 2023-07-27 09:13:13.077448 openmodule_commands-12.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      529 2023-06-29 09:50:19.000000 openmodule_commands-12.1.0/setup.py
--rw-rw-rw-   0 root         (0) root         (0)     8162 2023-06-29 09:50:19.000000 openmodule_commands-12.1.0/translate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 07:43:48.149462 openmodule_commands-12.1.1/
+-rw-r--r--   0 root         (0) root         (0)      302 2023-08-01 07:43:48.000000 openmodule_commands-12.1.1/AUTHORS
+-rw-r--r--   0 root         (0) root         (0)     8282 2023-08-01 07:43:48.000000 openmodule_commands-12.1.1/ChangeLog
+-rw-r--r--   0 root         (0) root         (0)      618 2023-08-01 07:43:48.149462 openmodule_commands-12.1.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2826 2023-08-01 07:43:35.000000 openmodule_commands-12.1.1/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 07:43:48.149462 openmodule_commands-12.1.1/openmodule_commands.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      618 2023-08-01 07:43:48.000000 openmodule_commands-12.1.1/openmodule_commands.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      363 2023-08-01 07:43:48.000000 openmodule_commands-12.1.1/openmodule_commands.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 07:43:48.000000 openmodule_commands-12.1.1/openmodule_commands.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      232 2023-08-01 07:43:48.000000 openmodule_commands-12.1.1/openmodule_commands.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 07:43:48.000000 openmodule_commands-12.1.1/openmodule_commands.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       46 2023-08-01 07:43:48.000000 openmodule_commands-12.1.1/openmodule_commands.egg-info/pbr.json
+-rw-r--r--   0 root         (0) root         (0)       20 2023-08-01 07:43:48.000000 openmodule_commands-12.1.1/openmodule_commands.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      850 2023-08-01 07:43:48.149462 openmodule_commands-12.1.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      529 2023-08-01 07:43:35.000000 openmodule_commands-12.1.1/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     8162 2023-08-01 07:43:35.000000 openmodule_commands-12.1.1/translate.py
```

### Comparing `openmodule_commands-12.1.0/ChangeLog` & `openmodule_commands-12.1.1/ChangeLog`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 CHANGES
 =======
 
+v12.1.1
+-------
+
+* trigger requirements update for changes in settings-models
+* docs and additional assertion in databox upload function
+
 v12.1.0
 -------
 
 * additional test cases for export\_iterator
 * first version of export iterator
 
 v12.0.0
@@ -229,13 +235,7 @@
 
 * # OpenModule \* rpc client resource filter only applies if resource in message \* all zmq messages now use utc timestamps
 
 v6.1.6
 ------
 
 * 6.1.6
-
-v6.1.5
-------
-
-* bug fix test cases
-* added default zmq.LINGER for context to be more compatible with OMv1 socket creation
```

### Comparing `openmodule_commands-12.1.0/PKG-INFO` & `openmodule_commands-12.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmodule_commands
-Version: 12.1.0
+Version: 12.1.1
 Summary: Commands for openmodule services
 Home-page: https://gitlab.com/arivo-public/device-python/openmodule.git
 Author: ARIVO
 Author-email: support@arivo.co
 License: GNU General Public License v2 (GPLv2)
 Keywords: arivo openmodule openmodule_commands commands
 Platform: UNKNOWN
```

### Comparing `openmodule_commands-12.1.0/__init__.py` & `openmodule_commands-12.1.1/__init__.py`

 * *Files identical despite different names*

### Comparing `openmodule_commands-12.1.0/openmodule_commands.egg-info/PKG-INFO` & `openmodule_commands-12.1.1/openmodule_commands.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmodule-commands
-Version: 12.1.0
+Version: 12.1.1
 Summary: Commands for openmodule services
 Home-page: https://gitlab.com/arivo-public/device-python/openmodule.git
 Author: ARIVO
 Author-email: support@arivo.co
 License: GNU General Public License v2 (GPLv2)
 Keywords: arivo openmodule openmodule_commands commands
 Platform: UNKNOWN
```

### Comparing `openmodule_commands-12.1.0/setup.cfg` & `openmodule_commands-12.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `openmodule_commands-12.1.0/setup.py` & `openmodule_commands-12.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `openmodule_commands-12.1.0/translate.py` & `openmodule_commands-12.1.1/translate.py`

 * *Files identical despite different names*

