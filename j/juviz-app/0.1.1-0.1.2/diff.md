# Comparing `tmp/juviz-app-0.1.1.tar.gz` & `tmp/juviz-app-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "juviz-app-0.1.1.tar", last modified: Wed Jul 26 11:14:22 2023, max compression
+gzip compressed data, was "juviz-app-0.1.2.tar", last modified: Tue Aug  1 15:46:08 2023, max compression
```

## Comparing `juviz-app-0.1.1.tar` & `juviz-app-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:14:22.479249 juviz-app-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-07-26 11:14:12.000000 juviz-app-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-26 11:14:22.479249 juviz-app-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-26 11:14:12.000000 juviz-app-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:14:22.479249 juviz-app-0.1.1/juviz/
--rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-07-26 11:14:12.000000 juviz-app-0.1.1/juviz/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:14:22.479249 juviz-app-0.1.1/juviz/assets/
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-26 11:14:12.000000 juviz-app-0.1.1/juviz/assets/FZJ_Logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-26 11:14:12.000000 juviz-app-0.1.1/juviz/assets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:14:22.479249 juviz-app-0.1.1/juviz/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-26 11:14:12.000000 juviz-app-0.1.1/juviz/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-07-26 11:14:12.000000 juviz-app-0.1.1/juviz/widgets/juviz_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:14:22.479249 juviz-app-0.1.1/juviz_app.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-26 11:14:22.000000 juviz-app-0.1.1/juviz_app.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-26 11:14:22.000000 juviz-app-0.1.1/juviz_app.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 11:14:22.000000 juviz-app-0.1.1/juviz_app.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-26 11:14:22.000000 juviz-app-0.1.1/juviz_app.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-26 11:14:22.000000 juviz-app-0.1.1/juviz_app.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-26 11:14:22.479249 juviz-app-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 11:14:12.000000 juviz-app-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:46:08.857059 juviz-app-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-08-01 15:45:57.000000 juviz-app-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-08-01 15:46:08.857059 juviz-app-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-01 15:45:57.000000 juviz-app-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:46:08.857059 juviz-app-0.1.2/juviz/
+-rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-08-01 15:45:57.000000 juviz-app-0.1.2/juviz/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:46:08.857059 juviz-app-0.1.2/juviz/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-08-01 15:45:57.000000 juviz-app-0.1.2/juviz/assets/FZJ_Logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-08-01 15:45:57.000000 juviz-app-0.1.2/juviz/assets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:46:08.857059 juviz-app-0.1.2/juviz/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-08-01 15:45:57.000000 juviz-app-0.1.2/juviz/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4689 2023-08-01 15:45:57.000000 juviz-app-0.1.2/juviz/widgets/juviz_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:46:08.857059 juviz-app-0.1.2/juviz_app.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-08-01 15:46:08.000000 juviz-app-0.1.2/juviz_app.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-08-01 15:46:08.000000 juviz-app-0.1.2/juviz_app.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 15:46:08.000000 juviz-app-0.1.2/juviz_app.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-01 15:46:08.000000 juviz-app-0.1.2/juviz_app.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-01 15:46:08.000000 juviz-app-0.1.2/juviz_app.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-08-01 15:46:08.857059 juviz-app-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 15:45:57.000000 juviz-app-0.1.2/setup.py
```

### Comparing `juviz-app-0.1.1/LICENSE` & `juviz-app-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `juviz-app-0.1.1/PKG-INFO` & `juviz-app-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: juviz-app
-Version: 0.1.1
+Version: 0.1.2
 Summary: Default trame App for JuViz
 Author: Jonathan Windgassen
 Author-email: j.windgassen@fz-juelich.de
 License: BSD License
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Environment :: Web Environment
```

### Comparing `juviz-app-0.1.1/juviz/__init__.py` & `juviz-app-0.1.2/juviz/__init__.py`

 * *Files identical despite different names*

### Comparing `juviz-app-0.1.1/juviz/assets/FZJ_Logo.svg` & `juviz-app-0.1.2/juviz/assets/FZJ_Logo.svg`

 * *Files identical despite different names*

### Comparing `juviz-app-0.1.1/juviz/widgets/__init__.py` & `juviz-app-0.1.2/juviz/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `juviz-app-0.1.1/juviz/widgets/juviz_controller.py` & `juviz-app-0.1.2/juviz/widgets/juviz_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from aiohttp.web import Application, Request, StreamResponse, HTTPOk, HTTPBadRequest
+from aiohttp.web import Request, StreamResponse, HTTPOk, HTTPBadRequest
+from wslink.protocol import AbstractWebApp
 from paraview import servermanager  # noqa
 
 from trame.widgets import html, vuetify
 
 NAME = "juviz-controller"
 ICON = "mdi-eye-settings"
 ICON_STYLE = {}
@@ -50,19 +51,19 @@
 
     ctrl.connect_to_server = connect
     ctrl.disconnect_from_server = disconnect
     ctrl.open_catalyst = open_catalyst
     ctrl.close_catalyst = close_catalyst
 
     @ctrl.add("on_server_bind")
-    def add_routes(aiohttp_server: Application):
-        # Define Handler for the JuViz Route
-        async def handle(request: Request) -> StreamResponse:
-            global _catalyst_connection
+    def add_routes(aiohttp_server: AbstractWebApp):
+        print("Creating JuViz Endpoint")
 
+        # Define Handler for the JuViz Route
+        async def handle_post(request: Request) -> StreamResponse:
             data: dict = await request.json()
             print(f"Received JuViz Request: {data = }")
             action = data["action"].lower()
 
             if action == "connect":
                 connect(data["url"], int(data.get("port", 11111)))
             elif action == "disconnect":
@@ -71,15 +72,16 @@
                 open_catalyst()
             elif action == "close_catalyst":
                 close_catalyst()
 
             return HTTPOk()
 
         # Create route
-        aiohttp_server.router.add_post("/juviz", handle)
+        # ToDo: Only works for aiohttp backend
+        aiohttp_server.app.router.add_post("/juviz", handle_post)
 
 
 def create_panel(server):
     state, ctrl = server.state, server.controller
 
     # Wrapper to get the values from the state
     def _connect():
```

### Comparing `juviz-app-0.1.1/juviz_app.egg-info/PKG-INFO` & `juviz-app-0.1.2/juviz_app.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: juviz-app
-Version: 0.1.1
+Version: 0.1.2
 Summary: Default trame App for JuViz
 Author: Jonathan Windgassen
 Author-email: j.windgassen@fz-juelich.de
 License: BSD License
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Environment :: Web Environment
```

### Comparing `juviz-app-0.1.1/setup.cfg` & `juviz-app-0.1.2/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = juviz-app
-version = 0.1.1
+version = 0.1.2
 description = Default trame App for JuViz
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Jonathan Windgassen
 author_email = j.windgassen@fz-juelich.de
 license = BSD License
 classifiers = 
@@ -23,15 +23,16 @@
 	Application
 	Framework
 
 [options]
 packages = find:
 include_package_data = True
 install_requires = 
-	pv_visualizer
+	pv-visualizer
+	wslink>=1.11.1
 
 [options.package_data]
 juviz.assets = *.svg
 
 [semantic_release]
 version_pattern = setup.cfg:version = (\d+\.\d+\.\d+)
```

