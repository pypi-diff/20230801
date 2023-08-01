# Comparing `tmp/lincot-1.0.2b3.tar.gz` & `tmp/lincot-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lincot-1.0.2b3.tar", last modified: Thu Jun 22 05:23:06 2023, max compression
+gzip compressed data, was "lincot-1.0.3.tar", last modified: Tue Aug  1 21:20:05 2023, max compression
```

## Comparing `lincot-1.0.2b3.tar` & `lincot-1.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 05:23:06.432346 lincot-1.0.2b3/
--rw-r--r--   0 runner    (1001) docker     (122)      557 2023-06-22 05:22:55.000000 lincot-1.0.2b3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-06-22 05:22:55.000000 lincot-1.0.2b3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     4198 2023-06-22 05:23:06.432346 lincot-1.0.2b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2764 2023-06-22 05:22:55.000000 lincot-1.0.2b3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 05:23:06.432346 lincot-1.0.2b3/lincot/
--rw-r--r--   0 runner    (1001) docker     (122)     1331 2023-06-22 05:22:55.000000 lincot-1.0.2b3/lincot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2500 2023-06-22 05:22:55.000000 lincot-1.0.2b3/lincot/classes.py
--rw-r--r--   0 runner    (1001) docker     (122)      960 2023-06-22 05:22:55.000000 lincot-1.0.2b3/lincot/commands.py
--rw-r--r--   0 runner    (1001) docker     (122)      962 2023-06-22 05:22:55.000000 lincot-1.0.2b3/lincot/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     4483 2023-06-22 05:22:55.000000 lincot-1.0.2b3/lincot/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 05:23:06.432346 lincot-1.0.2b3/lincot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4198 2023-06-22 05:23:06.000000 lincot-1.0.2b3/lincot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      327 2023-06-22 05:23:06.000000 lincot-1.0.2b3/lincot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-22 05:23:06.000000 lincot-1.0.2b3/lincot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       48 2023-06-22 05:23:06.000000 lincot-1.0.2b3/lincot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      113 2023-06-22 05:23:06.000000 lincot-1.0.2b3/lincot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-06-22 05:23:06.000000 lincot-1.0.2b3/lincot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1571 2023-06-22 05:23:06.432346 lincot-1.0.2b3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      769 2023-06-22 05:22:55.000000 lincot-1.0.2b3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 21:20:05.648942 lincot-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (122)      557 2023-08-01 21:19:55.000000 lincot-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-08-01 21:19:55.000000 lincot-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     4196 2023-08-01 21:20:05.648942 lincot-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2764 2023-08-01 21:19:55.000000 lincot-1.0.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 21:20:05.644942 lincot-1.0.3/lincot/
+-rw-r--r--   0 runner    (1001) docker     (122)     1325 2023-08-01 21:19:55.000000 lincot-1.0.3/lincot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2500 2023-08-01 21:19:55.000000 lincot-1.0.3/lincot/classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)      960 2023-08-01 21:19:55.000000 lincot-1.0.3/lincot/commands.py
+-rw-r--r--   0 runner    (1001) docker     (122)      962 2023-08-01 21:19:55.000000 lincot-1.0.3/lincot/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4483 2023-08-01 21:19:55.000000 lincot-1.0.3/lincot/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 21:20:05.648942 lincot-1.0.3/lincot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4196 2023-08-01 21:20:05.000000 lincot-1.0.3/lincot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      327 2023-08-01 21:20:05.000000 lincot-1.0.3/lincot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-01 21:20:05.000000 lincot-1.0.3/lincot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       48 2023-08-01 21:20:05.000000 lincot-1.0.3/lincot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      113 2023-08-01 21:20:05.000000 lincot-1.0.3/lincot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-08-01 21:20:05.000000 lincot-1.0.3/lincot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1589 2023-08-01 21:20:05.648942 lincot-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      769 2023-08-01 21:19:55.000000 lincot-1.0.3/setup.py
```

### Comparing `lincot-1.0.2b3/LICENSE` & `lincot-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lincot-1.0.2b3/PKG-INFO` & `lincot-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lincot
-Version: 1.0.2b3
+Version: 1.0.3
 Summary: LINCOT: Linux GPS to TAK Gateway.
 Home-page: https://github.com/snstac/lincot
 Maintainer: Greg Albrecht <oss@undef.net>
 Maintainer-email: oss@undef.net
 License: Apache 2.0
 Project-URL: CI: GitHub Actions, https://github.com/snstac/lincot/actions
 Project-URL: GitHub: issues, https://github.com/snstac/lincot/issues
```

### Comparing `lincot-1.0.2b3/README.rst` & `lincot-1.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `lincot-1.0.2b3/lincot/__init__.py` & `lincot-1.0.3/lincot/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 #
 
 """LINCOT: Linux GPS to TAK Gateway.
 
 :source: <https://github.com/snstac/lincot>
 """
 
-__version__ = "1.0.2-beta3"
+__version__ = "1.0.3"
 __author__ = "Greg Albrecht <gba@snstac.com>"
 __copyright__ = "Copyright 2023 Sensors & Signals LLC"
 __license__ = "Apache License, Version 2.0"
 
 
 # Python 3.6 test/build work-around:
 try:
```

### Comparing `lincot-1.0.2b3/lincot/classes.py` & `lincot-1.0.3/lincot/classes.py`

 * *Files identical despite different names*

### Comparing `lincot-1.0.2b3/lincot/commands.py` & `lincot-1.0.3/lincot/commands.py`

 * *Files identical despite different names*

### Comparing `lincot-1.0.2b3/lincot/constants.py` & `lincot-1.0.3/lincot/constants.py`

 * *Files identical despite different names*

### Comparing `lincot-1.0.2b3/lincot/functions.py` & `lincot-1.0.3/lincot/functions.py`

 * *Files identical despite different names*

### Comparing `lincot-1.0.2b3/lincot.egg-info/PKG-INFO` & `lincot-1.0.3/lincot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lincot
-Version: 1.0.2b3
+Version: 1.0.3
 Summary: LINCOT: Linux GPS to TAK Gateway.
 Home-page: https://github.com/snstac/lincot
 Maintainer: Greg Albrecht <oss@undef.net>
 Maintainer-email: oss@undef.net
 License: Apache 2.0
 Project-URL: CI: GitHub Actions, https://github.com/snstac/lincot/actions
 Project-URL: GitHub: issues, https://github.com/snstac/lincot/issues
```

### Comparing `lincot-1.0.2b3/setup.cfg` & `lincot-1.0.3/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 	TAK Server
 
 [options.entry_points]
 console_scripts = 
 	lincot = lincot.commands:main
 
 [options]
+packages = lincot
 python_requires = >=3.6, <4
 install_requires = 
 	pytak >= 5.4.0
 
 [options.extras_require]
 with_takproto = takproto >= 2.0.0
 test =
```

### Comparing `lincot-1.0.2b3/setup.py` & `lincot-1.0.3/setup.py`

 * *Files identical despite different names*

