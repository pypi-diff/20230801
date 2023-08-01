# Comparing `tmp/MyOverlay-0.1.5.tar.gz` & `tmp/MyOverlay-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MyOverlay-0.1.5.tar", last modified: Tue Aug  1 09:47:02 2023, max compression
+gzip compressed data, was "MyOverlay-0.1.6.tar", last modified: Tue Aug  1 09:58:11 2023, max compression
```

## Comparing `MyOverlay-0.1.5.tar` & `MyOverlay-0.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 09:47:02.558841 MyOverlay-0.1.5/
--rw-rw-rw-   0        0        0     1091 2023-08-01 09:37:41.000000 MyOverlay-0.1.5/LICENSE
--rw-rw-rw-   0        0        0      745 2023-08-01 09:47:02.557840 MyOverlay-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      174 2023-08-01 09:37:33.000000 MyOverlay-0.1.5/README.md
--rw-rw-rw-   0        0        0      649 2023-08-01 09:43:00.000000 MyOverlay-0.1.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-01 09:47:02.558841 MyOverlay-0.1.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-01 09:47:02.541840 MyOverlay-0.1.5/src/
-drwxrwxrwx   0        0        0        0 2023-08-01 09:47:02.545841 MyOverlay-0.1.5/src/MyOverlay/
--rw-rw-rw-   0        0        0      332 2023-08-01 07:54:17.000000 MyOverlay-0.1.5/src/MyOverlay/Overlay.py
--rw-rw-rw-   0        0        0        0 2023-07-31 14:05:46.000000 MyOverlay-0.1.5/src/MyOverlay/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 09:47:02.556840 MyOverlay-0.1.5/src/MyOverlay/funcs/
--rw-rw-rw-   0        0        0     3293 2023-08-01 07:53:45.000000 MyOverlay-0.1.5/src/MyOverlay/funcs/myfunctions.py
-drwxrwxrwx   0        0        0        0 2023-08-01 09:47:02.555841 MyOverlay-0.1.5/src/MyOverlay.egg-info/
--rw-rw-rw-   0        0        0      745 2023-08-01 09:47:02.000000 MyOverlay-0.1.5/src/MyOverlay.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2023-08-01 09:47:02.000000 MyOverlay-0.1.5/src/MyOverlay.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 09:47:02.000000 MyOverlay-0.1.5/src/MyOverlay.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-08-01 09:47:02.000000 MyOverlay-0.1.5/src/MyOverlay.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 09:58:11.353589 MyOverlay-0.1.6/
+-rw-rw-rw-   0        0        0     1091 2023-08-01 09:37:41.000000 MyOverlay-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0      745 2023-08-01 09:58:11.353589 MyOverlay-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      174 2023-08-01 09:37:33.000000 MyOverlay-0.1.6/README.md
+-rw-rw-rw-   0        0        0      649 2023-08-01 09:57:51.000000 MyOverlay-0.1.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-01 09:58:11.353589 MyOverlay-0.1.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-01 09:58:11.327928 MyOverlay-0.1.6/src/
+drwxrwxrwx   0        0        0        0 2023-08-01 09:58:11.336928 MyOverlay-0.1.6/src/MyOverlay/
+-rw-rw-rw-   0        0        0      324 2023-08-01 09:55:11.000000 MyOverlay-0.1.6/src/MyOverlay/Overlay.py
+-rw-rw-rw-   0        0        0        0 2023-08-01 09:49:30.000000 MyOverlay-0.1.6/src/MyOverlay/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 09:58:11.352588 MyOverlay-0.1.6/src/MyOverlay/funcs/
+-rw-rw-rw-   0        0        0     3311 2023-08-01 09:56:48.000000 MyOverlay-0.1.6/src/MyOverlay/funcs/myfunctions.py
+drwxrwxrwx   0        0        0        0 2023-08-01 09:58:11.349593 MyOverlay-0.1.6/src/MyOverlay.egg-info/
+-rw-rw-rw-   0        0        0      745 2023-08-01 09:58:11.000000 MyOverlay-0.1.6/src/MyOverlay.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2023-08-01 09:58:11.000000 MyOverlay-0.1.6/src/MyOverlay.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 09:58:11.000000 MyOverlay-0.1.6/src/MyOverlay.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-08-01 09:58:11.000000 MyOverlay-0.1.6/src/MyOverlay.egg-info/top_level.txt
```

### Comparing `MyOverlay-0.1.5/LICENSE` & `MyOverlay-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `MyOverlay-0.1.5/PKG-INFO` & `MyOverlay-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MyOverlay
-Version: 0.1.5
+Version: 0.1.6
 Summary: Customized Text Only Screen Overlay
 Author-email: Erik Reimann <erikreimann28@gmail.com>
 Project-URL: Homepage, https://github.com/HerpesHabenderHauptmannHarry/MyOverlay
 Project-URL: Bug Tracker, https://github.com/HerpesHabenderHauptmannHarry/MyOverlay/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `MyOverlay-0.1.5/pyproject.toml` & `MyOverlay-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools>=61.0']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "MyOverlay"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   { name="Erik Reimann", email="erikreimann28@gmail.com" },
 ]
 description = "Customized Text Only Screen Overlay"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `MyOverlay-0.1.5/src/MyOverlay/funcs/myfunctions.py` & `MyOverlay-0.1.6/src/MyOverlay/funcs/myfunctions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from win32api import GetSystemMetrics
 import pygame
 import win32api
 import win32con
 import win32gui
 import ctypes
 
-OverlayRunning = 0
+OverlayRunning = False
 white = (255, 255, 255)
 black = (0, 0, 0)
 fuchsia = (255, 0, 128)
 GWL_EXSTYLE = -20
 WS_EX_APPWINDOW = 0x00040000
 WS_EX_TOOLWINDOW = 0x00000080
 
@@ -56,15 +56,15 @@
 
 def StartOverlay():
     global OverlayRunning
     if not OverlayRunning:
         global text
         global textRect
         global screen
-        OverlayRunning = 1
+        OverlayRunning = True
         screen_width = GetSystemMetrics(win32con.SM_CXSCREEN)
         screen_height = GetSystemMetrics(win32con.SM_CYSCREEN)
         pygame.init()
         screen = pygame.display.set_mode((screen_width, screen_height), pygame.NOFRAME)  # For borderless, use pygame.NOFRAME
 
         hwnd = pygame.display.get_wm_info()["window"]
 
@@ -79,17 +79,17 @@
                                                       win32con.GWL_EXSTYLE) | win32con.WS_EX_LAYERED | win32con.WS_EX_TOPMOST)
         win32gui.SetLayeredWindowAttributes(hwnd, win32api.RGB(*fuchsia), 0, win32con.LWA_COLORKEY)
         
         screen.fill(fuchsia)
         pygame.display.update()
 
         win32gui.SetWindowPos(hwnd, win32con.HWND_TOPMOST, 0, 0, screen_width, screen_height, 0)
-        return 1
+        return True
     else:
-        return 0
+        return False
 
 
 
 
 def settext(text: str, PosX: int, PosY: int):
     global OverlayRunning
     for event in pygame.event.get():
@@ -100,11 +100,11 @@
     lines = str(text).splitlines()
     for i, l in enumerate(lines):
         screen.blit(render(l, font), (XPos // 2, PosY // 2 + 30 * i))
     pygame.display.update()
     
 def KillOverlay():
     pygame.display.quit()
-    OverlayRunning = 0
+    OverlayRunning = False
     
 def StatusOverlay():
     return OverlayRunning
```

### Comparing `MyOverlay-0.1.5/src/MyOverlay.egg-info/PKG-INFO` & `MyOverlay-0.1.6/src/MyOverlay.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MyOverlay
-Version: 0.1.5
+Version: 0.1.6
 Summary: Customized Text Only Screen Overlay
 Author-email: Erik Reimann <erikreimann28@gmail.com>
 Project-URL: Homepage, https://github.com/HerpesHabenderHauptmannHarry/MyOverlay
 Project-URL: Bug Tracker, https://github.com/HerpesHabenderHauptmannHarry/MyOverlay/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

