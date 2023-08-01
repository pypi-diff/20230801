# Comparing `tmp/openmodule_commands-12.1.1.tar.gz` & `tmp/openmodule_commands-12.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openmodule_commands-12.1.1.tar", last modified: Tue Aug  1 07:43:48 2023, max compression
+gzip compressed data, was "openmodule_commands-12.1.2.tar", last modified: Tue Aug  1 10:20:01 2023, max compression
```

## Comparing `openmodule_commands-12.1.1.tar` & `openmodule_commands-12.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 07:43:48.149462 openmodule_commands-12.1.1/
--rw-r--r--   0 root         (0) root         (0)      302 2023-08-01 07:43:48.000000 openmodule_commands-12.1.1/AUTHORS
--rw-r--r--   0 root         (0) root         (0)     8282 2023-08-01 07:43:48.000000 openmodule_commands-12.1.1/ChangeLog
--rw-r--r--   0 root         (0) root         (0)      618 2023-08-01 07:43:48.149462 openmodule_commands-12.1.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2826 2023-08-01 07:43:35.000000 openmodule_commands-12.1.1/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 07:43:48.149462 openmodule_commands-12.1.1/openmodule_commands.egg-info/
--rw-r--r--   0 root         (0) root         (0)      618 2023-08-01 07:43:48.000000 openmodule_commands-12.1.1/openmodule_commands.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      363 2023-08-01 07:43:48.000000 openmodule_commands-12.1.1/openmodule_commands.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 07:43:48.000000 openmodule_commands-12.1.1/openmodule_commands.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      232 2023-08-01 07:43:48.000000 openmodule_commands-12.1.1/openmodule_commands.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 07:43:48.000000 openmodule_commands-12.1.1/openmodule_commands.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       46 2023-08-01 07:43:48.000000 openmodule_commands-12.1.1/openmodule_commands.egg-info/pbr.json
--rw-r--r--   0 root         (0) root         (0)       20 2023-08-01 07:43:48.000000 openmodule_commands-12.1.1/openmodule_commands.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      850 2023-08-01 07:43:48.149462 openmodule_commands-12.1.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      529 2023-08-01 07:43:35.000000 openmodule_commands-12.1.1/setup.py
--rw-rw-rw-   0 root         (0) root         (0)     8162 2023-08-01 07:43:35.000000 openmodule_commands-12.1.1/translate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 10:20:01.096619 openmodule_commands-12.1.2/
+-rw-r--r--   0 root         (0) root         (0)      302 2023-08-01 10:20:01.000000 openmodule_commands-12.1.2/AUTHORS
+-rw-r--r--   0 root         (0) root         (0)     8267 2023-08-01 10:20:01.000000 openmodule_commands-12.1.2/ChangeLog
+-rw-r--r--   0 root         (0) root         (0)      618 2023-08-01 10:20:01.096619 openmodule_commands-12.1.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2826 2023-08-01 10:19:48.000000 openmodule_commands-12.1.2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 10:20:01.096619 openmodule_commands-12.1.2/openmodule_commands.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      618 2023-08-01 10:20:01.000000 openmodule_commands-12.1.2/openmodule_commands.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      363 2023-08-01 10:20:01.000000 openmodule_commands-12.1.2/openmodule_commands.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 10:20:01.000000 openmodule_commands-12.1.2/openmodule_commands.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      232 2023-08-01 10:20:01.000000 openmodule_commands-12.1.2/openmodule_commands.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 10:20:01.000000 openmodule_commands-12.1.2/openmodule_commands.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       46 2023-08-01 10:20:01.000000 openmodule_commands-12.1.2/openmodule_commands.egg-info/pbr.json
+-rw-r--r--   0 root         (0) root         (0)       20 2023-08-01 10:20:01.000000 openmodule_commands-12.1.2/openmodule_commands.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      850 2023-08-01 10:20:01.096619 openmodule_commands-12.1.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      529 2023-08-01 10:19:48.000000 openmodule_commands-12.1.2/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     8162 2023-08-01 10:19:48.000000 openmodule_commands-12.1.2/translate.py
```

### Comparing `openmodule_commands-12.1.1/ChangeLog` & `openmodule_commands-12.1.2/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 CHANGES
 =======
 
+v12.1.2
+-------
+
+* databox changed to rpc\_no\_blocking -> no exceptions and no waiting added immediate\_callbacks to MockRPCClient
+
 v12.1.1
 -------
 
 * trigger requirements update for changes in settings-models
 * docs and additional assertion in databox upload function
 
 v12.1.0
@@ -229,13 +234,7 @@
 * reduced warnings in the testcases
 * GUID type and rpc server changes to better support all pydantic models, in this case Union Types. DEVICE-891
 * fixes an issue in rpc server logging, and adds more debug log output
 
 v7.0.0
 ------
 
-* # OpenModule \* rpc client resource filter only applies if resource in message \* all zmq messages now use utc timestamps
-
-v6.1.6
-------
-
-* 6.1.6
```

### Comparing `openmodule_commands-12.1.1/PKG-INFO` & `openmodule_commands-12.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmodule_commands
-Version: 12.1.1
+Version: 12.1.2
 Summary: Commands for openmodule services
 Home-page: https://gitlab.com/arivo-public/device-python/openmodule.git
 Author: ARIVO
 Author-email: support@arivo.co
 License: GNU General Public License v2 (GPLv2)
 Keywords: arivo openmodule openmodule_commands commands
 Platform: UNKNOWN
```

### Comparing `openmodule_commands-12.1.1/__init__.py` & `openmodule_commands-12.1.2/__init__.py`

 * *Files identical despite different names*

### Comparing `openmodule_commands-12.1.1/openmodule_commands.egg-info/PKG-INFO` & `openmodule_commands-12.1.2/openmodule_commands.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmodule-commands
-Version: 12.1.1
+Version: 12.1.2
 Summary: Commands for openmodule services
 Home-page: https://gitlab.com/arivo-public/device-python/openmodule.git
 Author: ARIVO
 Author-email: support@arivo.co
 License: GNU General Public License v2 (GPLv2)
 Keywords: arivo openmodule openmodule_commands commands
 Platform: UNKNOWN
```

### Comparing `openmodule_commands-12.1.1/setup.cfg` & `openmodule_commands-12.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `openmodule_commands-12.1.1/setup.py` & `openmodule_commands-12.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `openmodule_commands-12.1.1/translate.py` & `openmodule_commands-12.1.2/translate.py`

 * *Files identical despite different names*

