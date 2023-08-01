# Comparing `tmp/MyOverlay-0.1.6.tar.gz` & `tmp/MyOverlay-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MyOverlay-0.1.6.tar", last modified: Tue Aug  1 09:58:11 2023, max compression
+gzip compressed data, was "MyOverlay-0.1.7.tar", last modified: Tue Aug  1 10:02:10 2023, max compression
```

## Comparing `MyOverlay-0.1.6.tar` & `MyOverlay-0.1.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 09:58:11.353589 MyOverlay-0.1.6/
--rw-rw-rw-   0        0        0     1091 2023-08-01 09:37:41.000000 MyOverlay-0.1.6/LICENSE
--rw-rw-rw-   0        0        0      745 2023-08-01 09:58:11.353589 MyOverlay-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0      174 2023-08-01 09:37:33.000000 MyOverlay-0.1.6/README.md
--rw-rw-rw-   0        0        0      649 2023-08-01 09:57:51.000000 MyOverlay-0.1.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-01 09:58:11.353589 MyOverlay-0.1.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-01 09:58:11.327928 MyOverlay-0.1.6/src/
-drwxrwxrwx   0        0        0        0 2023-08-01 09:58:11.336928 MyOverlay-0.1.6/src/MyOverlay/
--rw-rw-rw-   0        0        0      324 2023-08-01 09:55:11.000000 MyOverlay-0.1.6/src/MyOverlay/Overlay.py
--rw-rw-rw-   0        0        0        0 2023-08-01 09:49:30.000000 MyOverlay-0.1.6/src/MyOverlay/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 09:58:11.352588 MyOverlay-0.1.6/src/MyOverlay/funcs/
--rw-rw-rw-   0        0        0     3311 2023-08-01 09:56:48.000000 MyOverlay-0.1.6/src/MyOverlay/funcs/myfunctions.py
-drwxrwxrwx   0        0        0        0 2023-08-01 09:58:11.349593 MyOverlay-0.1.6/src/MyOverlay.egg-info/
--rw-rw-rw-   0        0        0      745 2023-08-01 09:58:11.000000 MyOverlay-0.1.6/src/MyOverlay.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2023-08-01 09:58:11.000000 MyOverlay-0.1.6/src/MyOverlay.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 09:58:11.000000 MyOverlay-0.1.6/src/MyOverlay.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-08-01 09:58:11.000000 MyOverlay-0.1.6/src/MyOverlay.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 10:02:10.640331 MyOverlay-0.1.7/
+-rw-rw-rw-   0        0        0     1091 2023-08-01 09:37:41.000000 MyOverlay-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0      745 2023-08-01 10:02:10.639331 MyOverlay-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0      174 2023-08-01 09:37:33.000000 MyOverlay-0.1.7/README.md
+-rw-rw-rw-   0        0        0      649 2023-08-01 10:02:07.000000 MyOverlay-0.1.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-01 10:02:10.640331 MyOverlay-0.1.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-01 10:02:10.617367 MyOverlay-0.1.7/src/
+drwxrwxrwx   0        0        0        0 2023-08-01 10:02:10.623334 MyOverlay-0.1.7/src/MyOverlay/
+-rw-rw-rw-   0        0        0      324 2023-08-01 09:55:11.000000 MyOverlay-0.1.7/src/MyOverlay/Overlay.py
+-rw-rw-rw-   0        0        0        0 2023-08-01 09:49:30.000000 MyOverlay-0.1.7/src/MyOverlay/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 10:02:10.638331 MyOverlay-0.1.7/src/MyOverlay/funcs/
+-rw-rw-rw-   0        0        0     3311 2023-08-01 10:01:55.000000 MyOverlay-0.1.7/src/MyOverlay/funcs/myfunctions.py
+drwxrwxrwx   0        0        0        0 2023-08-01 10:02:10.638331 MyOverlay-0.1.7/src/MyOverlay.egg-info/
+-rw-rw-rw-   0        0        0      745 2023-08-01 10:02:10.000000 MyOverlay-0.1.7/src/MyOverlay.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2023-08-01 10:02:10.000000 MyOverlay-0.1.7/src/MyOverlay.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 10:02:10.000000 MyOverlay-0.1.7/src/MyOverlay.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-08-01 10:02:10.000000 MyOverlay-0.1.7/src/MyOverlay.egg-info/top_level.txt
```

### Comparing `MyOverlay-0.1.6/LICENSE` & `MyOverlay-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `MyOverlay-0.1.6/PKG-INFO` & `MyOverlay-0.1.7/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MyOverlay
-Version: 0.1.6
+Version: 0.1.7
 Summary: Customized Text Only Screen Overlay
 Author-email: Erik Reimann <erikreimann28@gmail.com>
 Project-URL: Homepage, https://github.com/HerpesHabenderHauptmannHarry/MyOverlay
 Project-URL: Bug Tracker, https://github.com/HerpesHabenderHauptmannHarry/MyOverlay/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `MyOverlay-0.1.6/pyproject.toml` & `MyOverlay-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools>=61.0']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "MyOverlay"
-version = "0.1.6"
+version = "0.1.7"
 authors = [
   { name="Erik Reimann", email="erikreimann28@gmail.com" },
 ]
 description = "Customized Text Only Screen Overlay"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `MyOverlay-0.1.6/src/MyOverlay/funcs/myfunctions.py` & `MyOverlay-0.1.7/src/MyOverlay/funcs/myfunctions.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
     for event in pygame.event.get():
         if event.type == pygame.QUIT:
             OverlayRunning = 0
     font = pygame.font.SysFont('Segoe UI Semibold', 30, False)
     screen.fill(fuchsia)  # Transparent background
     lines = str(text).splitlines()
     for i, l in enumerate(lines):
-        screen.blit(render(l, font), (XPos // 2, PosY // 2 + 30 * i))
+        screen.blit(render(l, font), (PosX // 2, PosY // 2 + 30 * i))
     pygame.display.update()
     
 def KillOverlay():
     pygame.display.quit()
     OverlayRunning = False
     
 def StatusOverlay():
```

### Comparing `MyOverlay-0.1.6/src/MyOverlay.egg-info/PKG-INFO` & `MyOverlay-0.1.7/src/MyOverlay.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MyOverlay
-Version: 0.1.6
+Version: 0.1.7
 Summary: Customized Text Only Screen Overlay
 Author-email: Erik Reimann <erikreimann28@gmail.com>
 Project-URL: Homepage, https://github.com/HerpesHabenderHauptmannHarry/MyOverlay
 Project-URL: Bug Tracker, https://github.com/HerpesHabenderHauptmannHarry/MyOverlay/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

