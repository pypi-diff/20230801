# Comparing `tmp/jupyter_viz_extension-0.2.4.tar.gz` & `tmp/jupyter_viz_extension-0.3.0.tar.gz`

## Comparing `jupyter_viz_extension-0.2.4.tar` & `jupyter_viz_extension-0.3.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/.yarnrc.yml
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/CHANGELOG.md
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/install.json
--rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/setup.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/tsconfig.json
--rw-r--r--   0        0        0   231366 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/yarn.lock
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/jupyter-config/nb-config/jupyter_viz_extension.json
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/jupyter-config/server-config/jupyter_viz_extension.json
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/jupyter_viz_extension/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/jupyter_viz_extension/_version.py
--rw-r--r--   0        0        0     3567 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/jupyter_viz_extension/trame_model.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/jupyter_viz_extension/handlers/__init__.py
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/jupyter_viz_extension/handlers/cmd.py
--rw-r--r--   0        0        0     2158 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/jupyter_viz_extension/handlers/paraview.py
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/jupyter_viz_extension/handlers/trame.py
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/jupyter_viz_extension/handlers/user.py
--rw-r--r--   0        0        0     5374 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/jupyter_viz_extension/labextension/package.json
--rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/jupyter_viz_extension/labextension/schemas/jupyter-viz-extension/package.json.orig
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/jupyter_viz_extension/labextension/schemas/jupyter-viz-extension/plugin.json
--rw-r--r--   0        0        0    10694 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/jupyter_viz_extension/labextension/static/187.f44cc496302e8c70c5db.js
--rw-r--r--   0        0        0     5702 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/jupyter_viz_extension/labextension/static/747.e893f2b2bb7591fde94c.js
--rw-r--r--   0        0        0     6415 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/jupyter_viz_extension/labextension/static/759.31e0c66cf5e4357de249.js
--rw-r--r--   0        0        0    10694 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/jupyter_viz_extension/labextension/static/893.b4c09f80424627b87fe3.js
--rw-r--r--   0        0        0     7280 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/jupyter_viz_extension/labextension/static/remoteEntry.f31b28d3ff5c024fc221.js
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/jupyter_viz_extension/labextension/static/style.js
--rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/jupyter_viz_extension/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/jupyter_viz_extension/share/launch_paraview.in
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/schema/plugin.json
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/src/components.tsx
--rw-r--r--   0        0        0     3570 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/src/dialogs.tsx
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/src/handler.ts
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/src/index.tsx
--rw-r--r--   0        0        0     2680 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/src/paraview.tsx
--rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/src/trame.tsx
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/style/base.css
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/style/collapsible.css
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/style/index.js
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/.gitignore
--rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/LICENSE
--rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/README.md
--rw-r--r--   0        0        0     2548 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     6098 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.3.0/.yarnrc.yml
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.3.0/install.json
+-rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.3.0/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.3.0/setup.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.3.0/tsconfig.json
+-rw-r--r--   0        0        0   231366 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.3.0/yarn.lock
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.3.0/jupyter-config/nb-config/jupyter_viz_extension.json
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.3.0/jupyter-config/server-config/jupyter_viz_extension.json
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.3.0/jupyter_viz_extension/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.3.0/jupyter_viz_extension/_version.py
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.3.0/jupyter_viz_extension/cmd.py
+-rw-r--r--   0        0        0     8031 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.3.0/jupyter_viz_extension/model.py
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.3.0/jupyter_viz_extension/handlers/__init__.py
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.3.0/jupyter_viz_extension/handlers/paraview.py
+-rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.3.0/jupyter_viz_extension/handlers/trame.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.3.0/jupyter_viz_extension/handlers/user.py
+-rw-r--r--   0        0        0     5374 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.3.0/jupyter_viz_extension/labextension/package.json
+-rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.3.0/jupyter_viz_extension/labextension/schemas/jupyter-viz-extension/package.json.orig
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.3.0/jupyter_viz_extension/labextension/schemas/jupyter-viz-extension/plugin.json
+-rw-r--r--   0        0        0    10694 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.3.0/jupyter_viz_extension/labextension/static/187.f44cc496302e8c70c5db.js
+-rw-r--r--   0        0        0     6021 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.3.0/jupyter_viz_extension/labextension/static/747.d9a674d94c3c348fe532.js
+-rw-r--r--   0        0        0     8737 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.3.0/jupyter_viz_extension/labextension/static/759.5604a063656a1e46357d.js
+-rw-r--r--   0        0        0    10694 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.3.0/jupyter_viz_extension/labextension/static/893.b4c09f80424627b87fe3.js
+-rw-r--r--   0        0        0     7280 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.3.0/jupyter_viz_extension/labextension/static/remoteEntry.644577cc87d67f92cf64.js
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.3.0/jupyter_viz_extension/labextension/static/style.js
+-rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.3.0/jupyter_viz_extension/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.3.0/jupyter_viz_extension/share/launch_paraview.in
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.3.0/schema/plugin.json
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.3.0/src/components.tsx
+-rw-r--r--   0        0        0     5170 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.3.0/src/dialogs.tsx
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.3.0/src/handler.ts
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.3.0/src/index.tsx
+-rw-r--r--   0        0        0     2644 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.3.0/src/paraview.tsx
+-rw-r--r--   0        0        0     5694 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.3.0/src/trame.tsx
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.3.0/style/base.css
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.3.0/style/collapsible.css
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.3.0/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.3.0/style/index.js
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.3.0/README.md
+-rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6137 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.3.0/PKG-INFO
```

### Comparing `jupyter_viz_extension-0.2.4/package.json` & `jupyter_viz_extension-0.3.0/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'0.3.0'"}*

```diff
@@ -178,9 +178,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.2.4"
+    "version": "0.3.0"
 }
```

### Comparing `jupyter_viz_extension-0.2.4/tsconfig.json` & `jupyter_viz_extension-0.3.0/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.4/yarn.lock` & `jupyter_viz_extension-0.3.0/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.4/jupyter_viz_extension/__init__.py` & `jupyter_viz_extension-0.3.0/jupyter_viz_extension/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,13 @@
+from jupyter_server.serverapp import ServerApp
+from jupyter_server.utils import url_path_join
+
 from ._version import __version__
 from .handlers import setup_handlers
+from .model import Model
 
 
 def _jupyter_labextension_paths():
     return [{
         "src": "labextension",
         "dest": "jupyter-viz-extension"
     }]
@@ -11,16 +15,18 @@
 
 def _jupyter_server_extension_points():
     return [{
         "module": "jupyter_viz_extension"
     }]
 
 
-def _load_jupyter_server_extension(server_app):
-    setup_handlers(server_app.web_app)
+def _load_jupyter_server_extension(server_app: ServerApp):
+    model = Model(server_app.log, server_app.base_url)
+    setup_handlers(server_app.web_app, model)
+
     name = "jupyter_viz_extension"
     server_app.log.info(f"Registered {name} server extension")
 
 
 # For backward compatibility with notebook server
 load_jupyter_server_extension = _load_jupyter_server_extension
```

### Comparing `jupyter_viz_extension-0.2.4/jupyter_viz_extension/handlers/cmd.py` & `jupyter_viz_extension-0.3.0/jupyter_viz_extension/cmd.py`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.4/jupyter_viz_extension/handlers/trame.py` & `jupyter_viz_extension-0.3.0/jupyter_viz_extension/handlers/paraview.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 import json
 from jupyter_server.base.handlers import APIHandler
 from tornado.web import authenticated
 
-from ..trame_model import TrameModel
+from ..model import Model
 
 
-class TrameHandler(APIHandler):
+class ParaViewHandler(APIHandler):
+    _model: Model
+
+    def initialize(self, model):
+        self._model = model
+
     @authenticated
     async def get(self):
-        await self.finish(json.dumps([
-            app.dump() for app in TrameModel.instance(self.log).apps.values()
-        ]))
-    
+        await self.finish(json.dumps(
+            [server.dump() for server in self._model.servers]
+        ))
+        
     @authenticated
     async def post(self):
-        app_name = self.get_argument("app_name", "juviz")
-        self.log.info(f"Launching new trame instance {app_name!r}")
-
         try:
-            instance = await TrameModel.instance(self.log).launch_trame(app_name)
+            return_code, message = await self._model.launch_paraview(json.loads(self.request.body))
             self.set_status(200)
-            await self.finish(instance.dump())
+            await self.finish({"returnCode": return_code, "message": message})
             
         except Exception as e:
             self.log.error(str(e))
             self.set_status(400)
             await self.finish(str(e))
```

### Comparing `jupyter_viz_extension-0.2.4/jupyter_viz_extension/handlers/user.py` & `jupyter_viz_extension-0.3.0/jupyter_viz_extension/handlers/user.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
+import os
 import asyncio
 from jupyter_server.base.handlers import APIHandler
 from tornado.web import authenticated
-from .cmd import output
+from ..cmd import output
 
 
 async def _get_accounts():
     _, out = await output("jutil", "user", "projects", "--format='json'")
     return [group["unixgroup"] for group in json.loads(out)] if out else []
 
 
@@ -23,11 +24,12 @@
             _get_partitions()
         )
 
         self.log.debug(f"User: {username!r} - Accounts: {accounts!r} - Partitions: {partitions!r}")
 
         await self.finish({
             "user": username,
+            "home": os.path.expanduser("~"),
             "accounts": accounts,
             "partitions": partitions
         })
```

### Comparing `jupyter_viz_extension-0.2.4/jupyter_viz_extension/labextension/package.json` & `jupyter_viz_extension-0.3.0/jupyter_viz_extension/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9788194444444445%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.644577cc87d67f92cf64.js'}}",*

 * * "'version'": "'0.3.0'"}*

```diff
@@ -106,15 +106,15 @@
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*.json"
     ],
     "homepage": "https://github.com/github_username/jupyter-viz-extension",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.f31b28d3ff5c024fc221.js",
+            "load": "static/remoteEntry.644577cc87d67f92cf64.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "jupyter_viz_extension"
                 },
@@ -183,9 +183,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.2.4"
+    "version": "0.3.0"
 }
```

### Comparing `jupyter_viz_extension-0.2.4/jupyter_viz_extension/labextension/schemas/jupyter-viz-extension/package.json.orig` & `jupyter_viz_extension-0.3.0/jupyter_viz_extension/labextension/schemas/jupyter-viz-extension/package.json.orig`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'0.3.0'"}*

```diff
@@ -178,9 +178,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.2.4"
+    "version": "0.3.0"
 }
```

### Comparing `jupyter_viz_extension-0.2.4/jupyter_viz_extension/labextension/static/187.f44cc496302e8c70c5db.js` & `jupyter_viz_extension-0.3.0/jupyter_viz_extension/labextension/static/187.f44cc496302e8c70c5db.js`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.4/jupyter_viz_extension/labextension/static/747.e893f2b2bb7591fde94c.js` & `jupyter_viz_extension-0.3.0/jupyter_viz_extension/labextension/static/747.d9a674d94c3c348fe532.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -7,15 +7,15 @@
             });
             var o = t(645),
                 r = t.n(o),
                 i = t(243),
                 a = r()((function(n) {
                     return n[1]
                 }));
-            a.i(i.Z), a.push([n.id, ".juviz-sidepanel {\n  background: var(--jp-layout-color3);\n}\n\n.juviz-sidepanel-segment {\n  background: var(--jp-layout-color0);\n  color: var(--jp-content-font-color0);\n  padding: 10px;\n}\n\n.instance-list {\n  display: flex;\n  flex-direction: column;\n  row-gap: 10px;\n}\n\n.instance-list li {\n  border: var(--jp-layout-color4) solid 2px;\n  padding: 5px;\n  display: flex;\n  flex-direction: row;\n}\n\n.launch-button {\n  background: green;\n  color: white;\n  border: 0 solid green;\n  float: right;\n  padding: 4px 8px;\n}\n\n.form-input {\n  margin-bottom: 12px;\n}\n\n.open-button {\n  width: 30%;\n  border: 0;\n  padding: 0;\n  background: var(--jp-layout-color2);\n  flex-shrink: 0;\n}\n\n.open-button:hover {\n  background-color: var(--jp-layout-color3);\n}\n\n.open-button:active {\n  color: white;\n  background-color: var(--jp-layout-color4);\n}", ""]);
+            a.i(i.Z), a.push([n.id, ".juviz-sidepanel {\n  background: var(--jp-layout-color3);\n}\n\n.juviz-sidepanel-segment {\n  background: var(--jp-layout-color0);\n  color: var(--jp-content-font-color0);\n  padding: 10px;\n}\n\n.instance-list {\n  display: flex;\n  flex-direction: column;\n  row-gap: 10px;\n}\n\n.instance-list li {\n  padding: 5px;\n  display: flex;\n  flex-direction: row;\n}\n\n.launch-button {\n  background: green;\n  color: white;\n  border: 0 solid green;\n  float: right;\n  padding: 4px 8px;\n}\n\n.form-input {\n  margin-bottom: 12px;\n}\n\n.open-button {\n  width: 30%;\n  border: 0;\n  padding: 0;\n  margin: 0 5px;\n  background: var(--jp-layout-color2);\n  flex-shrink: 0;\n}\n\n.open-button:hover {\n  background-color: var(--jp-layout-color3);\n}\n\n.open-button:active {\n  color: white;\n  background-color: var(--jp-layout-color4);\n}\n\n.connect-button {\n  width: calc(100% - 20px);\n  height: 20px;\n  border: 0;\n  padding: 0;\n  margin: 10px 10px 0;\n  background: green;\n  color: white;\n}\n\n\n.disconnect-button {\n  width: calc(100% - 20px);\n  height: 20px;\n  border: 0;\n  padding: 0;\n  margin: 10px 10px 0;\n  background: var(--jp-layout-color4);\n  color: white;\n}", ""]);
             const c = a
         },
         243: (n, e, t) => {
             t.d(e, {
                 Z: () => i
             });
             var o = t(645),
@@ -79,22 +79,22 @@
             function c(n, e) {
                 for (var t = {}, o = [], r = 0; r < n.length; r++) {
                     var c = n[r],
                         l = e.base ? c[0] + e.base : c[0],
                         s = t[l] || 0,
                         d = "".concat(l, " ").concat(s);
                     t[l] = s + 1;
-                    var u = a(d),
-                        p = {
+                    var p = a(d),
+                        u = {
                             css: c[1],
                             media: c[2],
                             sourceMap: c[3]
-                        }; - 1 !== u ? (i[u].references++, i[u].updater(p)) : i.push({
+                        }; - 1 !== p ? (i[p].references++, i[p].updater(u)) : i.push({
                         identifier: d,
-                        updater: g(p, e),
+                        updater: v(u, e),
                         references: 1
                     }), o.push(d)
                 }
                 return o
             }
 
             function l(n) {
@@ -114,43 +114,43 @@
                 }
                 return e
             }
             var s, d = (s = [], function(n, e) {
                 return s[n] = e, s.filter(Boolean).join("\n")
             });
 
-            function u(n, e, t, o) {
+            function p(n, e, t, o) {
                 var r = t ? "" : o.media ? "@media ".concat(o.media, " {").concat(o.css, "}") : o.css;
                 if (n.styleSheet) n.styleSheet.cssText = d(e, r);
                 else {
                     var i = document.createTextNode(r),
                         a = n.childNodes;
                     a[e] && n.removeChild(a[e]), a.length ? n.insertBefore(i, a[e]) : n.appendChild(i)
                 }
             }
 
-            function p(n, e, t) {
+            function u(n, e, t) {
                 var o = t.css,
                     r = t.media,
                     i = t.sourceMap;
                 if (r ? n.setAttribute("media", r) : n.removeAttribute("media"), i && "undefined" != typeof btoa && (o += "\n/*# sourceMappingURL=data:application/json;base64,".concat(btoa(unescape(encodeURIComponent(JSON.stringify(i)))), " */")), n.styleSheet) n.styleSheet.cssText = o;
                 else {
                     for (; n.firstChild;) n.removeChild(n.firstChild);
                     n.appendChild(document.createTextNode(o))
                 }
             }
             var f = null,
-                v = 0;
+                g = 0;
 
-            function g(n, e) {
+            function v(n, e) {
                 var t, o, r;
                 if (e.singleton) {
-                    var i = v++;
-                    t = f || (f = l(e)), o = u.bind(null, t, i, !1), r = u.bind(null, t, i, !0)
-                } else t = l(e), o = p.bind(null, t, e), r = function() {
+                    var i = g++;
+                    t = f || (f = l(e)), o = p.bind(null, t, i, !1), r = p.bind(null, t, i, !0)
+                } else t = l(e), o = u.bind(null, t, e), r = function() {
                     ! function(n) {
                         if (null === n.parentNode) return !1;
                         n.parentNode.removeChild(n)
                     }(t)
                 };
                 return o(n),
                     function(e) {
```

### Comparing `jupyter_viz_extension-0.2.4/jupyter_viz_extension/labextension/static/759.31e0c66cf5e4357de249.js` & `jupyter_viz_extension-0.3.0/jupyter_viz_extension/labextension/static/759.5604a063656a1e46357d.js`

 * *Files 22% similar despite different names*

#### js-beautify {}

```diff
@@ -1,23 +1,23 @@
 "use strict";
 (self.webpackChunkjupyter_viz_extension = self.webpackChunkjupyter_viz_extension || []).push([
     [759], {
         759: (e, t, n) => {
             n.r(t), n.d(t, {
-                default: () => S
+                default: () => N
             });
             var a = n(303),
                 s = n(832),
                 i = n(271),
                 o = n.n(i),
-                r = n(628),
-                c = n.n(r),
+                c = n(628),
+                r = n.n(c),
                 l = n(344),
                 p = n(139);
-            async function u(e, t = {}) {
+            async function m(e, t = {}) {
                 const n = p.ServerConnection.makeSettings(),
                     a = l.URLExt.join(n.baseUrl, "jupyter-viz-extension", e);
                 let s;
                 try {
                     s = await p.ServerConnection.makeRequest(a, t, n)
                 } catch (e) {
                     throw new p.ServerConnection.NetworkError(e)
@@ -28,125 +28,142 @@
                 } catch (e) {
                     console.log("Not a JSON response body.", s)
                 }
                 if (!s.ok) throw new p.ServerConnection.ResponseError(s, i.message || i);
                 return i
             }
 
-            function m(e, t) {
+            function d(e, t) {
                 const n = document.createElement("label");
                 return n.htmlFor = e, n.textContent = t, n
             }
 
-            function d(e, t) {
+            function h(e, t) {
                 const n = document.createElement("select");
                 n.id = e;
                 for (const e of t) {
                     const t = document.createElement("option");
                     t.value = e, t.textContent = e, n.appendChild(t)
                 }
                 return n
             }
 
-            function h(e, t, n, a = []) {
+            function u(e, t, n, a = []) {
                 const s = document.createElement("input");
                 s.type = t, s.id = e, s.value = n, s.classList.add("form-input");
                 for (const [e, t] of a) s.setAttribute(e, t);
                 return s
             }
             class E extends s.Widget {
                 constructor() {
                     super(), this.fetchUserData = async () => {
-                        const e = await u("user");
+                        const e = await m("user");
                         for (const t of e.accounts) {
                             const e = document.createElement("option");
                             e.value = t, e.textContent = t, this._accountElement.appendChild(e)
                         }
                         for (const t of e.partitions) {
                             const e = document.createElement("option");
                             e.value = t, e.textContent = t, this._partitionElement.appendChild(e)
                         }
                     };
                     const e = document.createElement("div");
-                    e.appendChild(m("account", "Account: ")), e.appendChild(this._accountElement = d("account", [])), this.node.appendChild(e);
+                    e.appendChild(d("name", "Name: ")), e.appendChild(this._nameElement = u("name", "text", "ParaView Server")), this.node.appendChild(e);
                     const t = document.createElement("div");
-                    t.appendChild(m("partition", "Partition: ")), t.appendChild(this._partitionElement = d("partition", [])), this.node.appendChild(t);
+                    t.appendChild(d("account", "Account: ")), t.appendChild(this._accountElement = h("account", [])), this.node.appendChild(t);
                     const n = document.createElement("div");
-                    n.appendChild(m("nodes", "Nodes: ")), n.appendChild(this._nodesElement = h("nodes", "number", "4", [
+                    n.appendChild(d("partition", "Partition: ")), n.appendChild(this._partitionElement = h("partition", [])), this.node.appendChild(n);
+                    const a = document.createElement("div");
+                    a.appendChild(d("nodes", "Nodes: ")), a.appendChild(this._nodesElement = u("nodes", "number", "4", [
                         ["min", "1"],
                         ["max", "32"],
                         ["step", "1"]
-                    ])), this.node.appendChild(n);
-                    const a = document.createElement("div");
-                    a.appendChild(m("time", "Time: ")), a.appendChild(this._timeElement = h("time", "text", "02:00:00")), this.node.appendChild(a), this.fetchUserData()
+                    ])), this.node.appendChild(a);
+                    const s = document.createElement("div");
+                    s.appendChild(d("time", "Time: ")), s.appendChild(this._timeElement = u("time", "text", "02:00:00")), this.node.appendChild(s), this.fetchUserData()
                 }
                 getValue() {
                     return {
+                        name: this._nameElement.value,
                         account: this._accountElement.value,
                         partition: this._partitionElement.value,
                         nodes: Number(this._nodesElement.value),
                         timeLimit: this._timeElement.value
                     }
                 }
             }
-            class v extends i.Component {
+            class v extends s.Widget {
+                constructor(e, t) {
+                    super(), this.fetchUserData = async () => {
+                        const e = await m("user");
+                        this._dataDirElement.value = e.home
+                    };
+                    const n = document.createElement("div");
+                    n.appendChild(d("name", "Name: ")), n.appendChild(this._nameElement = u("name", "text", `${e} Instance ${t+1}`)), this.node.appendChild(n);
+                    const a = document.createElement("div");
+                    a.appendChild(d("dataDir", "Data Directory: ")), a.appendChild(this._dataDirElement = u("dataDir", "text", "")), this.node.appendChild(a), this.fetchUserData()
+                }
+                getValue() {
+                    return {
+                        name: this._nameElement.value,
+                        dataDirectory: this._dataDirElement.value
+                    }
+                }
+            }
+            class g extends i.Component {
                 render() {
                     return i.createElement("div", null, i.createElement("span", {
                         style: {
                             fontWeight: "bold"
                         }
                     }, this.props.label, ": "), i.createElement("span", null, this.props.value))
                 }
             }
-            class g extends i.Component {
+            class b extends i.Component {
                 constructor(e) {
                     super(e)
                 }
                 render() {
-                    var e;
-                    const t = i.createElement(i.Fragment, null, i.createElement(v, {
+                    const e = i.createElement(i.Fragment, null, i.createElement("b", null, this.props.name), i.createElement(g, {
                         label: "Nodes",
                         value: this.props.nodes.toString()
-                    }), i.createElement(v, {
+                    }), i.createElement(g, {
                         label: "Status",
                         value: this.props.state
-                    }), i.createElement(v, {
+                    }), i.createElement(g, {
                         label: "Time",
                         value: `${this.props.timeUsed} / ${this.props.timeLimit}`
                     }));
-                    return i.createElement(i.Fragment, null, i.createElement(c(), {
-                        trigger: t
-                    }, i.createElement(v, {
+                    return i.createElement(i.Fragment, null, i.createElement(r(), {
+                        trigger: e
+                    }, i.createElement(g, {
                         label: "Project",
                         value: this.props.account
-                    }), i.createElement(v, {
+                    }), i.createElement(g, {
                         label: "Partition",
                         value: this.props.partition
-                    }), i.createElement(v, {
+                    }), i.createElement(g, {
                         label: "Nodes",
                         value: this.props.nodes.toString()
-                    }), i.createElement(v, {
-                        label: "Port for Connection",
-                        value: null !== (e = this.props.url) && void 0 !== e ? e : ""
                     })))
                 }
             }
             class C extends i.Component {
                 constructor() {
                     super({}), this.fetchData = async () => {
                         this.setState({
-                            instances: await u("paraview")
+                            instances: await m("paraview")
                         })
                     }, this.newInstance = async () => {
                         const e = await (0, a.showDialog)({
                             title: "Launch a new ParaView instance",
                             body: new E
                         });
                         console.log(e.value);
-                        const t = await u("paraview", {
+                        const t = await m("paraview", {
                             method: "POST",
                             body: JSON.stringify(e.value)
                         });
                         await Promise.all([(0, a.showErrorMessage)(0 === t.returnCode ? "Success" : "Error", t.message), this.fetchData()])
                     }, this.state = {
                         instances: []
                     }
@@ -157,95 +174,167 @@
                 render() {
                     return i.createElement(i.Fragment, null, i.createElement("h3", null, "Running ParaView backends:", i.createElement("button", {
                         className: "launch-button",
                         onClick: this.newInstance
                     }, "Launch")), i.createElement("div", {
                         id: "paraview-instances",
                         className: "instance-list"
-                    }, this.state.instances.map((e => i.createElement(g, Object.assign({}, e))))))
+                    }, this.state.instances.map((e => i.createElement(b, Object.assign({}, e))))))
                 }
             }
-            class b extends i.Component {
+            class w extends i.Component {
                 constructor(e) {
                     super(e), this.openInstance = () => {
-                        const e = p.ServerConnection.makeSettings(),
-                            t = l.URLExt.join(e.baseUrl, "proxy", String(this.props.port), "index.html");
-                        window.open(t, "_blank", "noreferrer")
+                        const e = l.URLExt.join(this.props.base_url, "index.html");
+                        window.open(e, "_blank", "noreferrer")
+                    }, this.connect = async () => {
+                        const e = await m("paraview"),
+                            t = await a.InputDialog.getItem({
+                                title: "Select ParaView Server to connect to",
+                                items: e.map((e => e.name)),
+                                current: 0,
+                                editable: !1
+                            });
+                        if (!t.value || 0 === t.value.length) return;
+                        console.log(`Connecting instance '${this.props.name}' to Server '${t.value}'`);
+                        const n = await m(l.URLExt.join("trame", "connect"), {
+                            method: "POST",
+                            body: JSON.stringify({
+                                appName: this.props.appName,
+                                instanceName: this.props.name,
+                                serverName: t.value
+                            })
+                        });
+                        this.setState({
+                            connection: [t.value, n.url]
+                        })
+                    }, this.disconnect = async () => {
+                        await m(l.URLExt.join("trame", "disconnect"), {
+                            method: "POST",
+                            body: JSON.stringify({
+                                appName: this.props.appName,
+                                instanceName: this.props.name
+                            })
+                        }), this.setState({
+                            connection: void 0
+                        })
+                    }, this.state = {
+                        connection: void 0
                     }
                 }
                 render() {
+                    const e = i.createElement(i.Fragment, null, i.createElement("b", null, this.props.name)),
+                        t = this.state.connection ? i.createElement("div", {
+                            style: {
+                                marginTop: "10px"
+                            }
+                        }, "Connected to ParaView Server ", i.createElement("span", {
+                            style: {
+                                fontWeight: "bold"
+                            }
+                        }, this.state.connection[0]), " on ", i.createElement("span", {
+                            style: {
+                                fontWeight: "bold"
+                            }
+                        }, this.state.connection[1], ":11111"), i.createElement("button", {
+                            className: "disconnect-button",
+                            onClick: this.disconnect
+                        }, "Disconnect")) : i.createElement("button", {
+                            className: "connect-button",
+                            onClick: this.connect
+                        }, "Connect");
                     return i.createElement("li", null, i.createElement("div", {
                         style: {
                             flexGrow: 1
                         }
-                    }, i.createElement(v, {
+                    }, i.createElement(r(), {
+                        trigger: e
+                    }, i.createElement(g, {
+                        label: "Data Directory",
+                        value: `${this.props.dataDirectory}`
+                    }), i.createElement(g, {
                         label: "Port",
                         value: `${this.props.port}`
-                    }), i.createElement(v, {
+                    }), i.createElement(g, {
+                        label: "Base URL",
+                        value: `${this.props.base_url}`
+                    }), i.createElement(g, {
                         label: "Log File",
                         value: this.props.log
-                    })), i.createElement("button", {
+                    }), t)), i.createElement("button", {
                         className: "open-button",
                         onClick: this.openInstance
                     }, "Open"))
                 }
             }
-            class w extends i.Component {
+            class y extends i.Component {
                 constructor(e) {
                     super(e), this.launchInstance = async () => {
-                        console.log("Launching trame app " + this.props.name);
-                        const e = await u("trame", {
+                        const e = await (0, a.showDialog)({
+                            title: "Launch a new ParaView instance",
+                            body: new v(this.props.displayName, this.state.instances.length)
+                        });
+                        console.log("Launching trame app:", e.value);
+                        const t = await m("trame", {
                             method: "POST",
                             body: JSON.stringify({
-                                app_name: this.props.name
+                                appName: this.props.name,
+                                ...e.value
                             })
                         });
                         this.setState({
-                            instances: [...this.state.instances, e]
-                        }), await (0, a.showErrorMessage)("Success", `Launched new trame instance on port ${e.port}`)
+                            instances: [...this.state.instances, t]
+                        }), await (0, a.showErrorMessage)("Success", `Launched new trame instance on port ${t.port}`)
                     }, this.state = {
                         instances: this.props.instances
                     }
                 }
                 render() {
-                    const e = i.createElement("div", null, i.createElement("b", null, " ", this.props.name, " "), i.createElement("br", null), "Running Instances: ", this.state.instances.length);
-                    return i.createElement(i.Fragment, null, i.createElement(c(), {
+                    const e = i.createElement("div", null, i.createElement("b", null, " ", this.props.displayName, " "), i.createElement("br", null), "Running Instances: ", this.state.instances.length);
+                    return i.createElement(i.Fragment, null, i.createElement(r(), {
                         trigger: e
-                    }, i.createElement(v, {
+                    }, i.createElement(g, {
                         label: "Path",
                         value: this.props.path
-                    }), i.createElement("h4", null, "Instances:", i.createElement("button", {
+                    }), i.createElement("div", {
+                        style: {
+                            height: "40px",
+                            margin: "10px 0 0 0"
+                        }
+                    }, i.createElement("button", {
                         className: "launch-button",
                         onClick: this.launchInstance
                     }, "Launch")), i.createElement("div", {
                         className: "instance-list"
-                    }, this.state.instances.map((e => i.createElement(b, Object.assign({}, e)))))))
+                    }, this.state.instances.map((e => i.createElement(w, Object.assign({}, e, {
+                        appName: this.props.name
+                    })))))))
                 }
             }
             class f extends i.Component {
                 constructor() {
                     super({}), this.fetchData = async () => {
                         this.setState({
-                            instances: await u("trame")
+                            instances: await m("trame")
                         })
                     }, this.state = {
                         instances: []
                     }
                 }
                 async componentDidMount() {
                     await this.fetchData()
                 }
                 render() {
                     return i.createElement(i.Fragment, null, i.createElement("h3", null, "trame Apps:"), i.createElement("div", {
                         id: "trame-instances",
                         className: "instance-list"
-                    }, this.state.instances.map((e => i.createElement(w, Object.assign({}, e))))))
+                    }, this.state.instances.map((e => i.createElement(y, Object.assign({}, e))))))
                 }
             }
-            const S = {
+            const N = {
                 id: "juviz-extension",
                 autoStart: !0,
                 activate: e => {
                     const t = new s.SplitPanel;
                     t.orientation = "vertical", t.id = "juviz-sidepanel", t.title.iconClass = "jp-ExtensionIcon jp-SideBar-tabIcon", t.title.caption = "JuWiz";
                     const n = a.ReactWidget.create(o().createElement(C, null));
                     n.addClass("juviz-sidepanel-segment"), t.addWidget(n);
```

### Comparing `jupyter_viz_extension-0.2.4/jupyter_viz_extension/labextension/static/893.b4c09f80424627b87fe3.js` & `jupyter_viz_extension-0.3.0/jupyter_viz_extension/labextension/static/893.b4c09f80424627b87fe3.js`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.4/jupyter_viz_extension/labextension/static/remoteEntry.f31b28d3ff5c024fc221.js` & `jupyter_viz_extension-0.3.0/jupyter_viz_extension/labextension/static/remoteEntry.644577cc87d67f92cf64.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, a, i, u, l, s, d, f, p, c, h, v, b, g, m, y = {
+    var e, r, t, n, o, a, i, u, l, s, f, d, c, p, h, v, b, g, m, y = {
             299: (e, r, t) => {
                 var n = {
                         "./index": () => Promise.all([t.e(271), t.e(759)]).then((() => () => t(759))),
                         "./extension": () => Promise.all([t.e(271), t.e(759)]).then((() => () => t(759))),
                         "./style": () => t.e(747).then((() => () => t(747)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
@@ -45,53 +45,53 @@
         for (var t in r) j.o(r, t) && !j.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, j.f = {}, j.e = e => Promise.all(Object.keys(j.f).reduce(((r, t) => (j.f[t](e, r), r)), [])), j.u = e => e + "." + {
         187: "f44cc496302e8c70c5db",
         271: "624d1e1a34fcab02d699",
-        747: "e893f2b2bb7591fde94c",
-        759: "31e0c66cf5e4357de249",
+        747: "d9a674d94c3c348fe532",
+        759: "5604a063656a1e46357d",
         893: "b4c09f80424627b87fe3"
     } [e] + ".js?v=" + {
         187: "f44cc496302e8c70c5db",
         271: "624d1e1a34fcab02d699",
-        747: "e893f2b2bb7591fde94c",
-        759: "31e0c66cf5e4357de249",
+        747: "d9a674d94c3c348fe532",
+        759: "5604a063656a1e46357d",
         893: "b4c09f80424627b87fe3"
     } [e], j.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), j.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "jupyter-viz-extension:", j.l = (t, n, o, a) => {
         if (e[t]) e[t].push(n);
         else {
             var i, u;
             if (void 0 !== o)
                 for (var l = document.getElementsByTagName("script"), s = 0; s < l.length; s++) {
-                    var d = l[s];
-                    if (d.getAttribute("src") == t || d.getAttribute("data-webpack") == r + o) {
-                        i = d;
+                    var f = l[s];
+                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + o) {
+                        i = f;
                         break
                     }
                 }
             i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, j.nc && i.setAttribute("nonce", j.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
-            var f = (r, n) => {
-                    i.onerror = i.onload = null, clearTimeout(p);
+            var d = (r, n) => {
+                    i.onerror = i.onload = null, clearTimeout(c);
                     var o = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
                 },
-                p = setTimeout(f.bind(null, void 0, {
+                c = setTimeout(d.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = f.bind(null, i.onerror), i.onload = f.bind(null, i.onload), u && document.head.appendChild(i)
+            i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), u && document.head.appendChild(i)
         }
     }, j.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -113,15 +113,15 @@
                         (!u || !u.loaded && (!n != !u.eager ? n : i > u.from)) && (o[r] = {
                             get: t,
                             from: i,
                             eager: !!n
                         })
                     },
                     l = [];
-                return "default" === t && (u("jupyter-viz-extension", "0.2.4", (() => Promise.all([j.e(271), j.e(759)]).then((() => () => j(759))))), u("react-collapsible", "2.10.0", (() => Promise.all([j.e(271), j.e(893)]).then((() => () => j(893)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                return "default" === t && (u("jupyter-viz-extension", "0.3.0", (() => Promise.all([j.e(271), j.e(759)]).then((() => () => j(759))))), u("react-collapsible", "2.10.0", (() => Promise.all([j.e(271), j.e(893)]).then((() => () => j(893)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         j.g.importScripts && (e = j.g.location + "");
         var r = j.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -171,63 +171,63 @@
     }, a = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 o = n < 0;
             o && (n = -n - 1);
             for (var i = 0, u = 1, l = !0;; u++, i++) {
-                var s, d, f = u < e.length ? (typeof e[u])[0] : "";
-                if (i >= r.length || "o" == (d = (typeof(s = r[i]))[0])) return !l || ("u" == f ? u > n && !o : "" == f != o);
-                if ("u" == d) {
-                    if (!l || "u" != f) return !1
+                var s, f, d = u < e.length ? (typeof e[u])[0] : "";
+                if (i >= r.length || "o" == (f = (typeof(s = r[i]))[0])) return !l || ("u" == d ? u > n && !o : "" == d != o);
+                if ("u" == f) {
+                    if (!l || "u" != d) return !1
                 } else if (l)
-                    if (f == d)
+                    if (d == f)
                         if (u <= n) {
                             if (s != e[u]) return !1
                         } else {
                             if (o ? s > e[u] : s < e[u]) return !1;
                             s != e[u] && (l = !1)
                         }
-                else if ("s" != f && "n" != f) {
+                else if ("s" != d && "n" != d) {
                     if (o || u <= n) return !1;
                     l = !1, u--
                 } else {
-                    if (u <= n || d < f != o) return !1;
+                    if (u <= n || f < d != o) return !1;
                     l = !1
-                } else "s" != f && "n" != f && (l = !1, u--)
+                } else "s" != d && "n" != d && (l = !1, u--)
             }
         }
-        var p = [],
-            c = p.pop.bind(p);
+        var c = [],
+            p = c.pop.bind(c);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
-            p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? a(h, r) : !c())
+            c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? a(h, r) : !p())
         }
-        return !!c()
+        return !!p()
     }, i = (e, r) => {
         var t = j.S[e];
         if (!t || !j.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
     }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", s = (e, r, t, n) => {
         var o = u(e, t);
-        return a(n, o) || f(l(e, t, o, n)), p(e[t][o])
-    }, d = (e, r, t) => {
+        return a(n, o) || d(l(e, t, o, n)), c(e[t][o])
+    }, f = (e, r, t) => {
         var o = e[r];
         return (r = Object.keys(o).reduce(((e, r) => !a(t, r) || e && !n(e, r) ? e : r), 0)) && o[r]
-    }, f = e => {
+    }, d = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, p = e => (e.loaded = 1, e.get()), h = (c = e => function(r, t, n, o) {
+    }, c = e => (e.loaded = 1, e.get()), h = (p = e => function(r, t, n, o) {
         var a = j.I(r);
         return a && a.then ? a.then(e.bind(e, r, j.S[r], t, n, o)) : e(r, j.S[r], t, n, o)
-    })(((e, r, t, n) => (i(e, t), s(r, 0, t, n)))), v = c(((e, r, t, n, o) => {
-        var a = r && j.o(r, t) && d(r, t, n);
-        return a ? p(a) : o()
+    })(((e, r, t, n) => (i(e, t), s(r, 0, t, n)))), v = p(((e, r, t, n, o) => {
+        var a = r && j.o(r, t) && f(r, t, n);
+        return a ? c(a) : o()
     })), b = {}, g = {
         271: () => h("default", "react", [1, 17, 0, 1]),
         139: () => h("default", "@jupyterlab/services", [1, 6, 6, 5]),
         303: () => h("default", "@jupyterlab/apputils", [1, 3, 6, 5]),
         344: () => h("default", "@jupyterlab/coreutils", [1, 5, 6, 5]),
         628: () => v("default", "react-collapsible", [1, 2, 10, 0], (() => j.e(187).then((() => () => j(893))))),
         832: () => h("default", "@lumino/widgets", [1, 1, 37, 2])
```

### Comparing `jupyter_viz_extension-0.2.4/jupyter_viz_extension/labextension/static/third-party-licenses.json` & `jupyter_viz_extension-0.3.0/jupyter_viz_extension/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.4/jupyter_viz_extension/share/launch_paraview.in` & `jupyter_viz_extension-0.3.0/jupyter_viz_extension/share/launch_paraview.in`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/bin/bash
 #SBATCH --account={{ account }}
-#SBATCH --job-name="juviz-pvserver"
+#SBATCH --job-name={{ name }}
 #SBATCH --output=pvserver.out
 #SBATCH --error=pvserver.err
 #SBATCH --nodes={{ nodes }}
 #SBATCH --time={{ timeLimit }}
 
 # change this only with caution and with respect to "--displays="
 #SBATCH --partition={{ partition }}
```

### Comparing `jupyter_viz_extension-0.2.4/src/handler.ts` & `jupyter_viz_extension-0.3.0/src/handler.ts`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.4/src/index.tsx` & `jupyter_viz_extension-0.3.0/src/index.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.4/src/paraview.tsx` & `jupyter_viz_extension-0.3.0/src/paraview.tsx`

 * *Files 2% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 
 import { requestAPI } from './handler';
 import { ParaViewLauncherDialog } from './dialogs';
 import { Info, Empty, InstanceList } from './components';
 
 
 export type ParaViewLaunchOptions = {
+  name: string;
   account: string;
   partition: string;
   nodes: number;
   timeLimit: string;
 };
 
-type ParaViewInstanceOptions = ParaViewLaunchOptions & {
+export type ParaViewInstanceOptions = ParaViewLaunchOptions & {
   state: string;
   timeUsed: string;
-  url?: string;
 };
 
 type ParaViewReturnStatus = {
   returnCode: number;
   message: string;
 }
 
@@ -30,27 +30,27 @@
   constructor(props: ParaViewInstanceOptions) {
     super(props);
   }
 
   render() {
     const label = (
       <>
+        <b>{this.props.name}</b>
         <Info label='Nodes' value={this.props.nodes.toString()} />
         <Info label='Status' value={this.props.state} />
         <Info label='Time' value={`${this.props.timeUsed} / ${this.props.timeLimit}`} />
       </>
     );
 
     return (
       <>
         <Collapsible trigger={label}>
           <Info label='Project' value={this.props.account} />
           <Info label='Partition' value={this.props.partition} />
           <Info label='Nodes' value={this.props.nodes.toString()} />
-          <Info label='Port for Connection' value={this.props.url ?? ''} />
         </Collapsible>
       </>
     );
   }
 }
```

### Comparing `jupyter_viz_extension-0.2.4/style/collapsible.css` & `jupyter_viz_extension-0.3.0/style/collapsible.css`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.4/.gitignore` & `jupyter_viz_extension-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.4/LICENSE` & `jupyter_viz_extension-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.4/README.md` & `jupyter_viz_extension-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.4/pyproject.toml` & `jupyter_viz_extension-0.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,16 @@
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
-    "jupyter_server>=1.21,<3"
+    "jupyter-server>=1.21,<3",
+    "jupyter-server-proxy>=3"
 ]
 dynamic = ["version", "description", "authors", "urls", "keywords"]
 
 [tool.hatch.version]
 source = "nodejs"
 
 [tool.hatch.metadata.hooks.nodejs]
```

### Comparing `jupyter_viz_extension-0.2.4/PKG-INFO` & `jupyter_viz_extension-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter_viz_extension
-Version: 0.2.4
+Version: 0.3.0
 Summary: A JupyterLab extension.
 Project-URL: Homepage, https://github.com/github_username/jupyter-viz-extension
 Project-URL: Bug Tracker, https://github.com/github_username/jupyter-viz-extension/issues
 Project-URL: Repository, https://github.com/github_username/jupyter-viz-extension.git
 Author-email: Jonathan Windgassen <j.windgassen@fz-juelich.de>
 License: BSD 3-Clause License
         
@@ -46,14 +46,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
+Requires-Dist: jupyter-server-proxy>=3
 Requires-Dist: jupyter-server<3,>=1.21
 Description-Content-Type: text/markdown
 
 # jupyter_viz_extension
 
 [![Github Actions Status](https://github.com/jwindgassen/jupyter_viz_extension/workflows/Build/badge.svg)](https://github.com/jwindgassen/jupyter_viz_extension/actions/workflows/build.yml)
 A JupyterLab extension.
```

