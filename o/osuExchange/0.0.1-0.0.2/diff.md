# Comparing `tmp/osuExchange-0.0.1.tar.gz` & `tmp/osuExchange-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osuExchange-0.0.1.tar", last modified: Sat Jul 29 01:27:15 2023, max compression
+gzip compressed data, was "osuExchange-0.0.2.tar", last modified: Mon Jul 31 22:57:24 2023, max compression
```

## Comparing `osuExchange-0.0.1.tar` & `osuExchange-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 t_        (1000) t_        (1000)        0 2023-07-29 01:27:15.410514 osuExchange-0.0.1/
--rw-r--r--   0 t_        (1000) t_        (1000)      831 2023-07-29 01:27:15.410514 osuExchange-0.0.1/PKG-INFO
--rw-r--r--   0 t_        (1000) t_        (1000)      583 2023-07-23 17:42:53.000000 osuExchange-0.0.1/README.md
-drwxr-xr-x   0 t_        (1000) t_        (1000)        0 2023-07-29 01:27:15.407181 osuExchange-0.0.1/osuExchange/
--rw-r--r--   0 t_        (1000) t_        (1000)      166 2023-07-29 00:24:28.000000 osuExchange-0.0.1/osuExchange/__init__.py
--rw-r--r--   0 t_        (1000) t_        (1000)     1320 2023-07-29 01:23:40.000000 osuExchange-0.0.1/osuExchange/api.py
--rw-r--r--   0 t_        (1000) t_        (1000)     4353 2023-07-15 03:35:17.000000 osuExchange-0.0.1/osuExchange/auth.py
--rw-r--r--   0 t_        (1000) t_        (1000)     7836 2023-07-29 00:25:40.000000 osuExchange-0.0.1/osuExchange/beatmaps.py
--rw-r--r--   0 t_        (1000) t_        (1000)      749 2023-07-15 03:35:16.000000 osuExchange-0.0.1/osuExchange/client.py
--rw-r--r--   0 t_        (1000) t_        (1000)     3399 2023-07-29 00:24:28.000000 osuExchange-0.0.1/osuExchange/scores.py
--rw-r--r--   0 t_        (1000) t_        (1000)      753 2023-07-29 01:14:28.000000 osuExchange-0.0.1/osuExchange/seasonalbg.py
--rw-r--r--   0 t_        (1000) t_        (1000)      221 2023-07-14 21:26:15.000000 osuExchange-0.0.1/osuExchange/typing.py
--rw-r--r--   0 t_        (1000) t_        (1000)     6833 2023-07-15 18:41:10.000000 osuExchange-0.0.1/osuExchange/users.py
--rw-r--r--   0 t_        (1000) t_        (1000)      671 2023-07-15 03:35:17.000000 osuExchange-0.0.1/osuExchange/util.py
-drwxr-xr-x   0 t_        (1000) t_        (1000)        0 2023-07-29 01:27:15.410514 osuExchange-0.0.1/osuExchange.egg-info/
--rw-r--r--   0 t_        (1000) t_        (1000)      831 2023-07-29 01:27:15.000000 osuExchange-0.0.1/osuExchange.egg-info/PKG-INFO
--rw-r--r--   0 t_        (1000) t_        (1000)      418 2023-07-29 01:27:15.000000 osuExchange-0.0.1/osuExchange.egg-info/SOURCES.txt
--rw-r--r--   0 t_        (1000) t_        (1000)        1 2023-07-29 01:27:15.000000 osuExchange-0.0.1/osuExchange.egg-info/dependency_links.txt
--rw-r--r--   0 t_        (1000) t_        (1000)        9 2023-07-29 01:27:15.000000 osuExchange-0.0.1/osuExchange.egg-info/requires.txt
--rw-r--r--   0 t_        (1000) t_        (1000)       12 2023-07-29 01:27:15.000000 osuExchange-0.0.1/osuExchange.egg-info/top_level.txt
--rw-r--r--   0 t_        (1000) t_        (1000)      293 2023-07-29 01:14:03.000000 osuExchange-0.0.1/pyproject.toml
--rw-r--r--   0 t_        (1000) t_        (1000)       38 2023-07-29 01:27:15.410514 osuExchange-0.0.1/setup.cfg
+drwxr-xr-x   0 t_        (1000) t_        (1000)        0 2023-07-31 22:57:24.312741 osuExchange-0.0.2/
+-rw-r--r--   0 t_        (1000) t_        (1000)      831 2023-07-31 22:57:24.312741 osuExchange-0.0.2/PKG-INFO
+-rw-r--r--   0 t_        (1000) t_        (1000)      583 2023-07-23 17:42:53.000000 osuExchange-0.0.2/README.md
+drwxr-xr-x   0 t_        (1000) t_        (1000)        0 2023-07-31 22:57:24.312741 osuExchange-0.0.2/osuExchange/
+-rw-r--r--   0 t_        (1000) t_        (1000)      166 2023-07-29 00:24:28.000000 osuExchange-0.0.2/osuExchange/__init__.py
+-rw-r--r--   0 t_        (1000) t_        (1000)     1320 2023-07-29 01:23:40.000000 osuExchange-0.0.2/osuExchange/api.py
+-rw-r--r--   0 t_        (1000) t_        (1000)     4353 2023-07-15 03:35:17.000000 osuExchange-0.0.2/osuExchange/auth.py
+-rw-r--r--   0 t_        (1000) t_        (1000)     7836 2023-07-29 00:25:40.000000 osuExchange-0.0.2/osuExchange/beatmaps.py
+-rw-r--r--   0 t_        (1000) t_        (1000)     2712 2023-07-29 01:32:24.000000 osuExchange-0.0.2/osuExchange/client.py
+-rw-r--r--   0 t_        (1000) t_        (1000)     3399 2023-07-29 00:24:28.000000 osuExchange-0.0.2/osuExchange/scores.py
+-rw-r--r--   0 t_        (1000) t_        (1000)      753 2023-07-29 01:14:28.000000 osuExchange-0.0.2/osuExchange/seasonalbg.py
+-rw-r--r--   0 t_        (1000) t_        (1000)      221 2023-07-14 21:26:15.000000 osuExchange-0.0.2/osuExchange/typing.py
+-rw-r--r--   0 t_        (1000) t_        (1000)     6833 2023-07-15 18:41:10.000000 osuExchange-0.0.2/osuExchange/users.py
+-rw-r--r--   0 t_        (1000) t_        (1000)      671 2023-07-15 03:35:17.000000 osuExchange-0.0.2/osuExchange/util.py
+drwxr-xr-x   0 t_        (1000) t_        (1000)        0 2023-07-31 22:57:24.312741 osuExchange-0.0.2/osuExchange.egg-info/
+-rw-r--r--   0 t_        (1000) t_        (1000)      831 2023-07-31 22:57:24.000000 osuExchange-0.0.2/osuExchange.egg-info/PKG-INFO
+-rw-r--r--   0 t_        (1000) t_        (1000)      418 2023-07-31 22:57:24.000000 osuExchange-0.0.2/osuExchange.egg-info/SOURCES.txt
+-rw-r--r--   0 t_        (1000) t_        (1000)        1 2023-07-31 22:57:24.000000 osuExchange-0.0.2/osuExchange.egg-info/dependency_links.txt
+-rw-r--r--   0 t_        (1000) t_        (1000)        9 2023-07-31 22:57:24.000000 osuExchange-0.0.2/osuExchange.egg-info/requires.txt
+-rw-r--r--   0 t_        (1000) t_        (1000)       12 2023-07-31 22:57:24.000000 osuExchange-0.0.2/osuExchange.egg-info/top_level.txt
+-rw-r--r--   0 t_        (1000) t_        (1000)      293 2023-07-31 22:57:12.000000 osuExchange-0.0.2/pyproject.toml
+-rw-r--r--   0 t_        (1000) t_        (1000)       38 2023-07-31 22:57:24.312741 osuExchange-0.0.2/setup.cfg
```

### Comparing `osuExchange-0.0.1/PKG-INFO` & `osuExchange-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osuExchange
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simple osu!APIv2 wrapper for Python
 Author: trustytrojan, alittlerocket
 Project-URL: Homepage, https://github.com/alittlerocket/osuExchange
 Description-Content-Type: text/markdown
 
 # osuExchange
```

### Comparing `osuExchange-0.0.1/README.md` & `osuExchange-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `osuExchange-0.0.1/osuExchange/api.py` & `osuExchange-0.0.2/osuExchange/api.py`

 * *Files identical despite different names*

### Comparing `osuExchange-0.0.1/osuExchange/auth.py` & `osuExchange-0.0.2/osuExchange/auth.py`

 * *Files identical despite different names*

### Comparing `osuExchange-0.0.1/osuExchange/beatmaps.py` & `osuExchange-0.0.2/osuExchange/beatmaps.py`

 * *Files identical despite different names*

### Comparing `osuExchange-0.0.1/osuExchange/scores.py` & `osuExchange-0.0.2/osuExchange/scores.py`

 * *Files identical despite different names*

### Comparing `osuExchange-0.0.1/osuExchange/seasonalbg.py` & `osuExchange-0.0.2/osuExchange/seasonalbg.py`

 * *Files identical despite different names*

### Comparing `osuExchange-0.0.1/osuExchange/users.py` & `osuExchange-0.0.2/osuExchange/users.py`

 * *Files identical despite different names*

### Comparing `osuExchange-0.0.1/osuExchange/util.py` & `osuExchange-0.0.2/osuExchange/util.py`

 * *Files identical despite different names*

### Comparing `osuExchange-0.0.1/osuExchange.egg-info/PKG-INFO` & `osuExchange-0.0.2/osuExchange.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osuExchange
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simple osu!APIv2 wrapper for Python
 Author: trustytrojan, alittlerocket
 Project-URL: Homepage, https://github.com/alittlerocket/osuExchange
 Description-Content-Type: text/markdown
 
 # osuExchange
```

