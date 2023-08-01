# Comparing `tmp/chapyter-0.3.0.tar.gz` & `tmp/chapyter-0.3.1.tar.gz`

## Comparing `chapyter-0.3.0.tar` & `chapyter-0.3.1.tar`

### file list

```diff
@@ -1,33 +1,34 @@
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 chapyter-0.3.0/.prettierignore
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 chapyter-0.3.0/.yarnrc.yml
--rw-r--r--   0        0        0     4169 2020-02-02 00:00:00.000000 chapyter-0.3.0/RELEASE.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 chapyter-0.3.0/babel.config.js
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 chapyter-0.3.0/install.json
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 chapyter-0.3.0/jest.config.js
--rw-r--r--   0        0        0     6340 2020-02-02 00:00:00.000000 chapyter-0.3.0/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 chapyter-0.3.0/setup.py
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 chapyter-0.3.0/tsconfig.json
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 chapyter-0.3.0/tsconfig.test.json
--rw-r--r--   0        0        0   364822 2020-02-02 00:00:00.000000 chapyter-0.3.0/yarn.lock
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 chapyter-0.3.0/chapyter/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 chapyter-0.3.0/chapyter/_version.py
--rw-r--r--   0        0        0    12863 2020-02-02 00:00:00.000000 chapyter-0.3.0/chapyter/magic.py
--rw-r--r--   0        0        0     7308 2020-02-02 00:00:00.000000 chapyter-0.3.0/chapyter/programs.py
--rw-r--r--   0        0        0     5606 2020-02-02 00:00:00.000000 chapyter-0.3.0/chapyter/labextension/package.json
--rw-r--r--   0        0        0     6340 2020-02-02 00:00:00.000000 chapyter-0.3.0/chapyter/labextension/schemas/@shannon-shen/chapyter/package.json.orig
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 chapyter-0.3.0/chapyter/labextension/static/568.630c95d80cb75b8352da.js
--rw-r--r--   0        0        0     4764 2020-02-02 00:00:00.000000 chapyter-0.3.0/chapyter/labextension/static/747.217e756827eb66a6f3d4.js
--rw-r--r--   0        0        0     6961 2020-02-02 00:00:00.000000 chapyter-0.3.0/chapyter/labextension/static/remoteEntry.674ce065681604c8f0d3.js
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 chapyter-0.3.0/chapyter/labextension/static/style.js
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 chapyter-0.3.0/chapyter/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0    12382 2020-02-02 00:00:00.000000 chapyter-0.3.0/examples/01-quick-start.ipynb
--rw-r--r--   0        0        0    12599 2020-02-02 00:00:00.000000 chapyter-0.3.0/examples/02-configure-chapyter.ipynb
--rw-r--r--   0        0        0    10704 2020-02-02 00:00:00.000000 chapyter-0.3.0/src/index.ts
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 chapyter-0.3.0/style/base.css
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 chapyter-0.3.0/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 chapyter-0.3.0/style/index.js
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 chapyter-0.3.0/.gitignore
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 chapyter-0.3.0/LICENSE
--rw-r--r--   0        0        0     6273 2020-02-02 00:00:00.000000 chapyter-0.3.0/README.md
--rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 chapyter-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     9158 2020-02-02 00:00:00.000000 chapyter-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 chapyter-0.3.1/.prettierignore
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 chapyter-0.3.1/.yarnrc.yml
+-rw-r--r--   0        0        0     4169 2020-02-02 00:00:00.000000 chapyter-0.3.1/RELEASE.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 chapyter-0.3.1/babel.config.js
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 chapyter-0.3.1/install.json
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 chapyter-0.3.1/jest.config.js
+-rw-r--r--   0        0        0     6340 2020-02-02 00:00:00.000000 chapyter-0.3.1/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 chapyter-0.3.1/setup.py
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 chapyter-0.3.1/tsconfig.json
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 chapyter-0.3.1/tsconfig.test.json
+-rw-r--r--   0        0        0   364822 2020-02-02 00:00:00.000000 chapyter-0.3.1/yarn.lock
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 chapyter-0.3.1/chapyter/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 chapyter-0.3.1/chapyter/_version.py
+-rw-r--r--   0        0        0    13089 2020-02-02 00:00:00.000000 chapyter-0.3.1/chapyter/magic.py
+-rw-r--r--   0        0        0     7308 2020-02-02 00:00:00.000000 chapyter-0.3.1/chapyter/programs.py
+-rw-r--r--   0        0        0     5606 2020-02-02 00:00:00.000000 chapyter-0.3.1/chapyter/labextension/package.json
+-rw-r--r--   0        0        0     6340 2020-02-02 00:00:00.000000 chapyter-0.3.1/chapyter/labextension/schemas/@shannon-shen/chapyter/package.json.orig
+-rw-r--r--   0        0        0     3339 2020-02-02 00:00:00.000000 chapyter-0.3.1/chapyter/labextension/static/568.963fc68e9aea61cb1c90.js
+-rw-r--r--   0        0        0     4764 2020-02-02 00:00:00.000000 chapyter-0.3.1/chapyter/labextension/static/747.217e756827eb66a6f3d4.js
+-rw-r--r--   0        0        0     6961 2020-02-02 00:00:00.000000 chapyter-0.3.1/chapyter/labextension/static/remoteEntry.fa1a7e093e0f27eb2386.js
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 chapyter-0.3.1/chapyter/labextension/static/style.js
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 chapyter-0.3.1/chapyter/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0    12382 2020-02-02 00:00:00.000000 chapyter-0.3.1/examples/01-quick-start.ipynb
+-rw-r--r--   0        0        0    12599 2020-02-02 00:00:00.000000 chapyter-0.3.1/examples/02-configure-chapyter.ipynb
+-rw-r--r--   0        0        0    12206 2020-02-02 00:00:00.000000 chapyter-0.3.1/src/index.ts
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 chapyter-0.3.1/style/base.css
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 chapyter-0.3.1/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 chapyter-0.3.1/style/index.js
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 chapyter-0.3.1/tests/test_chapyter.py
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 chapyter-0.3.1/.gitignore
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 chapyter-0.3.1/LICENSE
+-rw-r--r--   0        0        0     6273 2020-02-02 00:00:00.000000 chapyter-0.3.1/README.md
+-rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 chapyter-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     9158 2020-02-02 00:00:00.000000 chapyter-0.3.1/PKG-INFO
```

### Comparing `chapyter-0.3.0/RELEASE.md` & `chapyter-0.3.1/RELEASE.md`

 * *Files identical despite different names*

### Comparing `chapyter-0.3.0/jest.config.js` & `chapyter-0.3.1/jest.config.js`

 * *Files identical despite different names*

### Comparing `chapyter-0.3.0/package.json` & `chapyter-0.3.1/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.98%*

 * *Differences: {"'version'": "'0.3.1'"}*

```diff
@@ -182,12 +182,12 @@
         "rules": {
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.3.0",
+    "version": "0.3.1",
     "workspaces": [
         "ui-tests"
     ]
 }
```

### Comparing `chapyter-0.3.0/tsconfig.json` & `chapyter-0.3.1/tsconfig.json`

 * *Files identical despite different names*

### Comparing `chapyter-0.3.0/yarn.lock` & `chapyter-0.3.1/yarn.lock`

 * *Files identical despite different names*

### Comparing `chapyter-0.3.0/chapyter/__init__.py` & `chapyter-0.3.1/chapyter/__init__.py`

 * *Files identical despite different names*

### Comparing `chapyter-0.3.0/chapyter/magic.py` & `chapyter-0.3.1/chapyter/magic.py`

 * *Files 6% similar despite different names*

```diff
@@ -349,28 +349,32 @@
 
         - %chapyter <parameter_name>
           print the current value of the parameter
 
         - %chapyter <parameter_name>=<value>
           set the value of the parameter
         """
+
+        # This code is inspired by the %config magic command in IPython
+        # See the code here: https://github.com/ipython/ipython/blob/6b17e43544316d691376e35e677032a4b00d6eeb/IPython/core/magics/config.py#L36
+
         # remove text after comments
         line = line.strip().split("#")[0].strip()
 
         all_class_configs = self.class_own_traits()
 
         if not line or line.startswith("#"):
             help = self.class_get_help(self)
             # strip leading '--' from cl-args:
             help = re.sub(re.compile(r"^--", re.MULTILINE), "", help)
             print(help)
             return
         elif line in all_class_configs.keys():
             return getattr(self, line)
-        elif "=" in line and line.split("=")[0] in all_class_configs.keys():
+        elif "=" in line and line.split("=")[0].strip() in all_class_configs.keys():
             cfg = Config()
             exec(f"cfg.{self.__class__.__name__}." + line, self.shell.user_ns, locals())
             self.update_config(cfg)
         elif line.startswith("help"):
             print(
                 "The %chapyter magic command supports the following usage:\n"
                 "- %chapyter\n  print all the configurable parameters and its current value\n"
```

### Comparing `chapyter-0.3.0/chapyter/programs.py` & `chapyter-0.3.1/chapyter/programs.py`

 * *Files identical despite different names*

### Comparing `chapyter-0.3.0/chapyter/labextension/package.json` & `chapyter-0.3.1/chapyter/labextension/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9795833333333333%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.fa1a7e093e0f27eb2386.js'}}",*

 * * "'version'": "'0.3.1'"}*

```diff
@@ -105,15 +105,15 @@
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*.json"
     ],
     "homepage": "https://github.com/chapyter/chapyter",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.674ce065681604c8f0d3.js",
+            "load": "static/remoteEntry.fa1a7e093e0f27eb2386.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "chapyter/labextension",
         "schemaDir": "schema"
     },
     "keywords": [
@@ -187,12 +187,12 @@
         "rules": {
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.3.0",
+    "version": "0.3.1",
     "workspaces": [
         "ui-tests"
     ]
 }
```

### Comparing `chapyter-0.3.0/chapyter/labextension/schemas/@shannon-shen/chapyter/package.json.orig` & `chapyter-0.3.1/chapyter/labextension/schemas/@shannon-shen/chapyter/package.json.orig`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.98%*

 * *Differences: {"'version'": "'0.3.1'"}*

```diff
@@ -182,12 +182,12 @@
         "rules": {
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.3.0",
+    "version": "0.3.1",
     "workspaces": [
         "ui-tests"
     ]
 }
```

### Comparing `chapyter-0.3.0/chapyter/labextension/static/568.630c95d80cb75b8352da.js` & `chapyter-0.3.1/chapyter/labextension/static/568.963fc68e9aea61cb1c90.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,111 +1,122 @@
 "use strict";
 (self.webpackChunk_shannon_shen_chapyter = self.webpackChunk_shannon_shen_chapyter || []).push([
     [568], {
         568: (e, t, l) => {
             l.r(t), l.d(t, {
-                default: () => r
+                default: () => h
             });
-            var n = l(861),
-                o = l(882);
-            const d = "jp-chapyter-chat-executing";
+            var o = l(861),
+                d = l(882);
+            const n = "jp-chapyter-chat",
+                a = "jp-chapyter-chat-executing",
+                i = "jp-chapyter-assistance";
 
-            function a(e) {
-                if ((0, o.isCodeCellModel)(e.model)) {
+            function s(e) {
+                if ((0, d.isCodeCellModel)(e.model)) {
                     let t = e.model.getMetadata("ChapyterCell") || null;
                     if (t && "generated" === t.cellType) return !1
                 }
                 return !0
             }
 
-            function i(e, t) {
+            function r(e, t) {
+                for (let l = 0; l < e.widgets.length; l++) {
+                    let o = e.widgets[l];
+                    if (o.model.id === t) return o
+                }
+                return null
+            }
+
+            function c(e, t) {
                 let l = e.activeCellIndex,
-                    o = function(e, t) {
+                    d = function(e, t) {
                         for (let l = 0; l < e.widgets.length; l++)
                             if (e.widgets[l].model.id === t) return l;
                         return -1
                     }(e, t);
-                if (-1 !== o && l !== o)
-                    if (l < o)
-                        for (let t = l; t < o; t++) e.widgets[t].inputHidden || n.NotebookActions.selectBelow(e);
+                if (-1 !== d && l !== d)
+                    if (l < d)
+                        for (let t = l; t < d; t++) e.widgets[t].inputHidden || o.NotebookActions.selectBelow(e);
                     else
-                        for (let t = l; t > o; t--) e.widgets[t].inputHidden || n.NotebookActions.selectAbove(e)
+                        for (let t = l; t > d; t--) e.widgets[t].inputHidden || o.NotebookActions.selectAbove(e)
             }
 
-            function s(e, t = !1) {
+            function u(e, t = !1) {
                 let l = e.model.sharedModel.getSource();
                 return !(!l.startsWith("%chat") && !l.startsWith("%%chat") || l.startsWith("%%chatonly") && t)
             }
-            const r = {
+            const h = {
                 id: "@shannon-shen/chapyter:plugin",
                 description: "A Natural Language-Based Python Program Interpreter",
                 autoStart: !0,
-                requires: [n.INotebookTracker],
+                requires: [o.INotebookTracker],
                 activate: (e, t) => {
-                    n.NotebookActions.executed.connect(((e, l) => {
+                    o.NotebookActions.executed.connect(((e, l) => {
                         if (l.success) {
                             let e = l.cell;
-                            if (s(e, !0) && a(e)) {
+                            if (u(e, !0) && s(e)) {
                                 void 0 === e.model.getMetadata("ChapyterCell") && e.model.setMetadata("ChapyterCell", {
                                     cellType: "original"
                                 });
                                 let l = function(e) {
                                         let t = e.model.sharedModel.getSource().split("\n")[0];
                                         return t.includes("-s") || t.includes("--safe")
                                     }(e),
-                                    o = t.currentWidget;
-                                if (o) {
+                                    d = t.currentWidget;
+                                if (d) {
                                     let t = function(e, t) {
                                         if (t) {
                                             const l = `# Assistant Code for Cell [${t}]:`;
                                             for (let t = 0; t < e.widgets.length; t++) {
-                                                let n = e.widgets[t];
-                                                if ("code" === n.model.type && n.model.sharedModel.getSource().split("\n")[0].startsWith(l)) return n
+                                                let o = e.widgets[t];
+                                                if ("code" === o.model.type && o.model.sharedModel.getSource().split("\n")[0].startsWith(l)) return o
                                             }
                                         }
                                         return null
-                                    }(o.content, e.model.executionCount);
+                                    }(d.content, e.model.executionCount);
                                     t && (t.model.setMetadata("ChapyterCell", {
                                         cellType: "generated",
                                         linkedCellId: e.model.id
-                                    }), console.log(l), l || (i(o.content, t.model.id), n.NotebookActions.run(o.content, o.sessionContext), t.inputHidden = !0), i(o.content, t.model.id), l || n.NotebookActions.selectBelow(o.content), e.model.setMetadata("ChapyterCell", {
+                                    }), console.log(l), l || (c(d.content, t.model.id), o.NotebookActions.run(d.content, d.sessionContext), t.inputHidden = !0), c(d.content, t.model.id), l || o.NotebookActions.selectBelow(d.content), e.model.setMetadata("ChapyterCell", {
                                         cellType: "original",
                                         linkedCellId: t.model.id
-                                    }), e.addClass("jp-chapyter-chat"), e.removeClass(d), t.addClass("jp-chapyter-assistance"))
+                                    }), e.addClass(n), e.removeClass(a), t.addClass(i))
                                 }
                             }
                         }
-                    })), n.NotebookActions.executionScheduled.connect(((e, l) => {
-                        var n;
-                        let o = l.cell;
-                        if (s(o) && a(o)) {
-                            o.toggleClass(d);
-                            let e = null === (n = o.model.getMetadata("ChapyterCell")) || void 0 === n ? void 0 : n.linkedCellId,
+                    })), o.NotebookActions.executionScheduled.connect(((e, l) => {
+                        var o;
+                        let d = l.cell;
+                        if (u(d) && s(d)) {
+                            d.toggleClass(a);
+                            let e = null === (o = d.model.getMetadata("ChapyterCell")) || void 0 === o ? void 0 : o.linkedCellId,
                                 l = t.currentWidget;
                             if (l && e) {
-                                let t = function(e, t) {
-                                    for (let l = 0; l < e.widgets.length; l++) {
-                                        let n = e.widgets[l];
-                                        if (n.model.id === t) return n
-                                    }
-                                    return null
-                                }(l.content, e);
+                                let t = r(l.content, e);
                                 t && (function(e, t) {
                                     const l = e.model.sharedModel,
-                                        n = [];
-                                    e.widgets.forEach(((l, o) => {
-                                        var d;
-                                        l === t && !1 !== l.model.getMetadata("deletable") && (n.push(o), null === (d = e.model) || void 0 === d || d.deletedCells.push(l.model.id))
-                                    })), n.length > 0 && (l.transact((() => {
-                                        n.reverse().forEach((e => {
+                                        o = [];
+                                    e.widgets.forEach(((l, d) => {
+                                        var n;
+                                        l === t && !1 !== l.model.getMetadata("deletable") && (o.push(d), null === (n = e.model) || void 0 === n || n.deletedCells.push(l.model.id))
+                                    })), o.length > 0 && (l.transact((() => {
+                                        o.reverse().forEach((e => {
                                             l.deleteCell(e)
                                         }))
-                                    })), e.activeCellIndex = n[0] - n.length + 1), e.deselectAll()
-                                }(l.content, t), i(l.content, o.model.id))
+                                    })), e.activeCellIndex = o[0] - o.length + 1), e.deselectAll()
+                                }(l.content, t), c(l.content, d.model.id))
                             }
                         }
+                    })), t.widgetAdded.connect(((e, t) => {
+                        t.context.ready.then((() => {
+                            t.content.widgets.forEach((e => {
+                                var l, o, d;
+                                "code" === e.model.type && e.model.getMetadata("ChapyterCell") && ("original" === (null === (l = e.model.getMetadata("ChapyterCell")) || void 0 === l ? void 0 : l.cellType) ? r(t.content, null === (o = e.model.getMetadata("ChapyterCell")) || void 0 === o ? void 0 : o.linkedCellId) ? e.addClass(n) : e.addClass(a) : "generated" === (null === (d = e.model.getMetadata("ChapyterCell")) || void 0 === d ? void 0 : d.cellType) ? e.addClass(i) : console.log(e.model.getMetadata("ChapyterCell")))
+                            }))
+                        }))
                     }))
                 }
             }
         }
     }
 ]);
```

### Comparing `chapyter-0.3.0/chapyter/labextension/static/747.217e756827eb66a6f3d4.js` & `chapyter-0.3.1/chapyter/labextension/static/747.217e756827eb66a6f3d4.js`

 * *Files identical despite different names*

### Comparing `chapyter-0.3.0/chapyter/labextension/static/remoteEntry.674ce065681604c8f0d3.js` & `chapyter-0.3.1/chapyter/labextension/static/remoteEntry.fa1a7e093e0f27eb2386.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -43,18 +43,18 @@
         }), r
     }, E.d = (e, r) => {
         for (var t in r) E.o(r, t) && !E.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, E.f = {}, E.e = e => Promise.all(Object.keys(E.f).reduce(((r, t) => (E.f[t](e, r), r)), [])), E.u = e => e + "." + {
-        568: "630c95d80cb75b8352da",
+        568: "963fc68e9aea61cb1c90",
         747: "217e756827eb66a6f3d4"
     } [e] + ".js?v=" + {
-        568: "630c95d80cb75b8352da",
+        568: "963fc68e9aea61cb1c90",
         747: "217e756827eb66a6f3d4"
     } [e], E.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
@@ -106,15 +106,15 @@
                     var o = a[e] = a[e] || {},
                         u = o[r];
                     (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (o[r] = {
                         get: () => E.e(568).then((() => () => E(568))),
                         from: i,
                         eager: !1
                     })
-                })("@shannon-shen/chapyter", "0.3.0"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("@shannon-shen/chapyter", "0.3.1"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         E.g.importScripts && (e = E.g.location + "");
         var r = E.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
```

### Comparing `chapyter-0.3.0/chapyter/labextension/static/third-party-licenses.json` & `chapyter-0.3.1/chapyter/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `chapyter-0.3.0/examples/01-quick-start.ipynb` & `chapyter-0.3.1/examples/01-quick-start.ipynb`

 * *Files identical despite different names*

### Comparing `chapyter-0.3.0/examples/02-configure-chapyter.ipynb` & `chapyter-0.3.1/examples/02-configure-chapyter.ipynb`

 * *Files identical despite different names*

### Comparing `chapyter-0.3.0/src/index.ts` & `chapyter-0.3.1/src/index.ts`

 * *Files 9% similar despite different names*

```diff
@@ -294,11 +294,43 @@
                */
               selectCellById(notebook.content, chatCell.model.id);
             }
           }
         }
       }
     });
+
+    tracker.widgetAdded.connect((sender, notebookPanel) => {
+      notebookPanel.context.ready.then(() => {
+        notebookPanel.content.widgets.forEach(cell => {
+          switch (cell.model.type) {
+            case 'code': {
+              /**
+               * The logic: 
+               * When we load a notebook, we want to check if a code cell is a chapyter cell.
+               * 1. if it is generated, then we want to add the class CHAPYTER_ASSISTANCE_CELL
+               * 2. if it is original, 
+               *  a. if the linked cell exists, then we want to add the class CHAPYTER_CHAT_CELL
+               *  b. if the linked cell does not exist, then we want to add the class CHAPYTER_CHAT_CELL_EXECUTING
+               */
+              if (cell.model.getMetadata('ChapyterCell')) {
+                if (cell.model.getMetadata('ChapyterCell')?.cellType === 'original') {
+                  if (findCellById(notebookPanel.content, cell.model.getMetadata('ChapyterCell')?.linkedCellId)) {
+                    cell.addClass(CHAPYTER_CHAT_CELL);
+                  } else {
+                    cell.addClass(CHAPYTER_CHAT_CELL_EXECUTING);
+                  }
+                } else if (cell.model.getMetadata('ChapyterCell')?.cellType === 'generated') {
+                  cell.addClass(CHAPYTER_ASSISTANCE_CELL);
+                } else {
+                  console.log(cell.model.getMetadata('ChapyterCell'));
+                }
+              }
+            }
+          }
+        })
+      })
+    });
   }
 };
 
 export default plugin;
```

### Comparing `chapyter-0.3.0/style/base.css` & `chapyter-0.3.1/style/base.css`

 * *Files identical despite different names*

### Comparing `chapyter-0.3.0/.gitignore` & `chapyter-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `chapyter-0.3.0/LICENSE` & `chapyter-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chapyter-0.3.0/README.md` & `chapyter-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `chapyter-0.3.0/pyproject.toml` & `chapyter-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `chapyter-0.3.0/PKG-INFO` & `chapyter-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chapyter
-Version: 0.3.0
+Version: 0.3.1
 Summary: A Natural Language-Based Python Program Interpreter
 Project-URL: Homepage, https://github.com/chapyter/chapyter
 Project-URL: Bug Tracker, https://github.com/chapyter/chapyter/issues
 Project-URL: Repository, https://github.com/chapyter/chapyter.git
 Author-email: chapyter <zejiangshen@gmail.com>
 License: BSD 3-Clause License
```

