# Comparing `tmp/MyOverlay-0.1.8.tar.gz` & `tmp/MyOverlay-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MyOverlay-0.1.8.tar", last modified: Tue Aug  1 11:15:32 2023, max compression
+gzip compressed data, was "MyOverlay-0.1.9.tar", last modified: Tue Aug  1 11:17:22 2023, max compression
```

## Comparing `MyOverlay-0.1.8.tar` & `MyOverlay-0.1.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 11:15:32.524672 MyOverlay-0.1.8/
--rw-rw-rw-   0        0        0     1091 2023-08-01 09:37:41.000000 MyOverlay-0.1.8/LICENSE
--rw-rw-rw-   0        0        0      745 2023-08-01 11:15:32.524672 MyOverlay-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0      174 2023-08-01 09:37:33.000000 MyOverlay-0.1.8/README.md
--rw-rw-rw-   0        0        0      649 2023-08-01 11:15:15.000000 MyOverlay-0.1.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-01 11:15:32.525671 MyOverlay-0.1.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-01 11:15:32.491639 MyOverlay-0.1.8/src/
-drwxrwxrwx   0        0        0        0 2023-08-01 11:15:32.506643 MyOverlay-0.1.8/src/MyOverlay/
--rw-rw-rw-   0        0        0      324 2023-08-01 09:55:11.000000 MyOverlay-0.1.8/src/MyOverlay/Overlay.py
--rw-rw-rw-   0        0        0        0 2023-08-01 09:49:30.000000 MyOverlay-0.1.8/src/MyOverlay/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 11:15:32.523672 MyOverlay-0.1.8/src/MyOverlay/funcs/
--rw-rw-rw-   0        0        0     3334 2023-08-01 11:14:56.000000 MyOverlay-0.1.8/src/MyOverlay/funcs/myfunctions.py
-drwxrwxrwx   0        0        0        0 2023-08-01 11:15:32.522683 MyOverlay-0.1.8/src/MyOverlay.egg-info/
--rw-rw-rw-   0        0        0      745 2023-08-01 11:15:32.000000 MyOverlay-0.1.8/src/MyOverlay.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2023-08-01 11:15:32.000000 MyOverlay-0.1.8/src/MyOverlay.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 11:15:32.000000 MyOverlay-0.1.8/src/MyOverlay.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-08-01 11:15:32.000000 MyOverlay-0.1.8/src/MyOverlay.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 11:17:22.496540 MyOverlay-0.1.9/
+-rw-rw-rw-   0        0        0     1091 2023-08-01 09:37:41.000000 MyOverlay-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0      745 2023-08-01 11:17:22.496540 MyOverlay-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      174 2023-08-01 09:37:33.000000 MyOverlay-0.1.9/README.md
+-rw-rw-rw-   0        0        0      649 2023-08-01 11:17:07.000000 MyOverlay-0.1.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-01 11:17:22.496540 MyOverlay-0.1.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-01 11:17:22.467539 MyOverlay-0.1.9/src/
+drwxrwxrwx   0        0        0        0 2023-08-01 11:17:22.475539 MyOverlay-0.1.9/src/MyOverlay/
+-rw-rw-rw-   0        0        0      324 2023-08-01 09:55:11.000000 MyOverlay-0.1.9/src/MyOverlay/Overlay.py
+-rw-rw-rw-   0        0        0        0 2023-08-01 09:49:30.000000 MyOverlay-0.1.9/src/MyOverlay/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 11:17:22.494542 MyOverlay-0.1.9/src/MyOverlay/funcs/
+-rw-rw-rw-   0        0        0     3347 2023-08-01 11:17:01.000000 MyOverlay-0.1.9/src/MyOverlay/funcs/myfunctions.py
+drwxrwxrwx   0        0        0        0 2023-08-01 11:17:22.491540 MyOverlay-0.1.9/src/MyOverlay.egg-info/
+-rw-rw-rw-   0        0        0      745 2023-08-01 11:17:22.000000 MyOverlay-0.1.9/src/MyOverlay.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2023-08-01 11:17:22.000000 MyOverlay-0.1.9/src/MyOverlay.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 11:17:22.000000 MyOverlay-0.1.9/src/MyOverlay.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-08-01 11:17:22.000000 MyOverlay-0.1.9/src/MyOverlay.egg-info/top_level.txt
```

### Comparing `MyOverlay-0.1.8/LICENSE` & `MyOverlay-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `MyOverlay-0.1.8/PKG-INFO` & `MyOverlay-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MyOverlay
-Version: 0.1.8
+Version: 0.1.9
 Summary: Customized Text Only Screen Overlay
 Author-email: Erik Reimann <erikreimann28@gmail.com>
 Project-URL: Homepage, https://github.com/HerpesHabenderHauptmannHarry/MyOverlay
 Project-URL: Bug Tracker, https://github.com/HerpesHabenderHauptmannHarry/MyOverlay/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `MyOverlay-0.1.8/pyproject.toml` & `MyOverlay-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools>=61.0']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "MyOverlay"
-version = "0.1.8"
+version = "0.1.9"
 authors = [
   { name="Erik Reimann", email="erikreimann28@gmail.com" },
 ]
 description = "Customized Text Only Screen Overlay"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `MyOverlay-0.1.8/src/MyOverlay/funcs/myfunctions.py` & `MyOverlay-0.1.9/src/MyOverlay/funcs/myfunctions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from win32api import GetSystemMetrics
 import pygame
 import win32api
 import win32con
 import win32gui
 import ctypes
+import time
 
 OverlayRunning = False
 white = (255, 255, 255)
 black = (0, 0, 0)
 fuchsia = (255, 0, 128)
 GWL_EXSTYLE = -20
 WS_EX_APPWINDOW = 0x00040000
```

### Comparing `MyOverlay-0.1.8/src/MyOverlay.egg-info/PKG-INFO` & `MyOverlay-0.1.9/src/MyOverlay.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MyOverlay
-Version: 0.1.8
+Version: 0.1.9
 Summary: Customized Text Only Screen Overlay
 Author-email: Erik Reimann <erikreimann28@gmail.com>
 Project-URL: Homepage, https://github.com/HerpesHabenderHauptmannHarry/MyOverlay
 Project-URL: Bug Tracker, https://github.com/HerpesHabenderHauptmannHarry/MyOverlay/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

