# Comparing `tmp/jupyterlab_vim-4.0.0.tar.gz` & `tmp/jupyterlab_vim-4.0.1.tar.gz`

## Comparing `jupyterlab_vim-4.0.0.tar` & `jupyterlab_vim-4.0.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.0/.eslintignore
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.0/.prettierignore
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.0/.prettierrc
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.0/.yarnrc.yml
--rw-r--r--   0        0        0     5690 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.0/CHANGELOG.md
--rw-r--r--   0        0        0     3923 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.0/RELEASE.md
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.0/install.json
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.0/installing.md
--rw-r--r--   0        0        0     2584 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.0/modify-keybinds.md
--rw-r--r--   0        0        0     6647 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.0/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.0/setup.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.0/tsconfig.json
--rw-r--r--   0        0        0   212877 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.0/yarn.lock
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.0/jupyterlab_vim/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.0/jupyterlab_vim/_version.py
--rw-r--r--   0        0        0     5921 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.0/jupyterlab_vim/labextension/package.json
--rw-r--r--   0        0        0     6647 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.0/jupyterlab_vim/labextension/schemas/@axlair/jupyterlab_vim/package.json.orig
--rw-r--r--   0        0        0    10856 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.0/jupyterlab_vim/labextension/schemas/@axlair/jupyterlab_vim/plugin.json
--rw-r--r--   0        0        0   130333 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.0/jupyterlab_vim/labextension/static/252.e0500116419ca3a355d1.js
--rw-r--r--   0        0        0    10172 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.0/jupyterlab_vim/labextension/static/353.8b609c372dc07b2baac6.js
--rw-r--r--   0        0        0     4399 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.0/jupyterlab_vim/labextension/static/747.a573445024188eae7034.js
--rw-r--r--   0        0        0     7577 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.0/jupyterlab_vim/labextension/static/remoteEntry.a73b7957e55f8d1b9f75.js
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.0/jupyterlab_vim/labextension/static/style.js
--rw-r--r--   0        0        0     7505 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.0/jupyterlab_vim/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0    10856 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.0/schema/plugin.json
--rw-r--r--   0        0        0    11763 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.0/src/codemirrorCommands.ts
--rw-r--r--   0        0        0     6297 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.0/src/index.ts
--rw-r--r--   0        0        0     8187 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.0/src/labCommands.ts
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.0/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.0/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.0/style/index.js
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.0/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.0/LICENSE
--rw-r--r--   0        0        0     6383 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.0/README.md
--rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.0/pyproject.toml
--rw-r--r--   0        0        0     8705 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.0/PKG-INFO
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.1/.eslintignore
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.1/.prettierignore
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.1/.prettierrc
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.1/.yarnrc.yml
+-rw-r--r--   0        0        0     7179 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.1/CHANGELOG.md
+-rw-r--r--   0        0        0     3923 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.1/RELEASE.md
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.1/install.json
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.1/installing.md
+-rw-r--r--   0        0        0     2584 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.1/modify-keybinds.md
+-rw-r--r--   0        0        0     6647 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.1/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.1/setup.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.1/tsconfig.json
+-rw-r--r--   0        0        0   212877 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.1/yarn.lock
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.1/jupyterlab_vim/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.1/jupyterlab_vim/_version.py
+-rw-r--r--   0        0        0     5921 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.1/jupyterlab_vim/labextension/package.json
+-rw-r--r--   0        0        0     6647 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.1/jupyterlab_vim/labextension/schemas/@axlair/jupyterlab_vim/package.json.orig
+-rw-r--r--   0        0        0    10856 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.1/jupyterlab_vim/labextension/schemas/@axlair/jupyterlab_vim/plugin.json
+-rw-r--r--   0        0        0   130333 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.1/jupyterlab_vim/labextension/static/252.e0500116419ca3a355d1.js
+-rw-r--r--   0        0        0    10218 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.1/jupyterlab_vim/labextension/static/353.9c6b79c5ee878d215a0a.js
+-rw-r--r--   0        0        0     4399 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.1/jupyterlab_vim/labextension/static/747.a573445024188eae7034.js
+-rw-r--r--   0        0        0     7577 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.1/jupyterlab_vim/labextension/static/remoteEntry.ddb05f98b2e0f61dea44.js
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.1/jupyterlab_vim/labextension/static/style.js
+-rw-r--r--   0        0        0     7505 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.1/jupyterlab_vim/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0    10856 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.1/schema/plugin.json
+-rw-r--r--   0        0        0    11871 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.1/src/codemirrorCommands.ts
+-rw-r--r--   0        0        0     6297 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.1/src/index.ts
+-rw-r--r--   0        0        0     8187 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.1/src/labCommands.ts
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.1/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.1/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.1/style/index.js
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.1/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.1/LICENSE
+-rw-r--r--   0        0        0     6383 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.1/README.md
+-rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.1/pyproject.toml
+-rw-r--r--   0        0        0     8705 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.1/PKG-INFO
```

### Comparing `jupyterlab_vim-4.0.0/CHANGELOG.md` & `jupyterlab_vim-4.0.1/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,36 @@
 # Changelog
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 4.0.1
+
+([Full Changelog](https://github.com/jupyterlab-contrib/jupyterlab-vim/compare/v4.0.0...9aa55aad927c578d91e51f351bb5bcf987d03c46))
+
+### Enhancements made
+
+- build: don't require package.json for python import [#93](https://github.com/jupyterlab-contrib/jupyterlab-vim/pull/93) ([@ianhi](https://github.com/ianhi))
+
+### Bugs fixed
+
+- Fix for attempting to update editor when there was none [#95](https://github.com/jupyterlab-contrib/jupyterlab-vim/pull/95) ([@krassowski](https://github.com/krassowski))
+
+### Maintenance and upkeep improvements
+
+- style: lint [#96](https://github.com/jupyterlab-contrib/jupyterlab-vim/pull/96) ([@ianhi](https://github.com/ianhi))
+- build: don't require package.json for python import [#93](https://github.com/jupyterlab-contrib/jupyterlab-vim/pull/93) ([@ianhi](https://github.com/ianhi))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/jupyterlab-contrib/jupyterlab-vim/graphs/contributors?from=2023-07-31&to=2023-08-01&type=c))
+
+[@github-actions](https://github.com/search?q=repo%3Ajupyterlab-contrib%2Fjupyterlab-vim+involves%3Agithub-actions+updated%3A2023-07-31..2023-08-01&type=Issues) | [@ianhi](https://github.com/search?q=repo%3Ajupyterlab-contrib%2Fjupyterlab-vim+involves%3Aianhi+updated%3A2023-07-31..2023-08-01&type=Issues) | [@krassowski](https://github.com/search?q=repo%3Ajupyterlab-contrib%2Fjupyterlab-vim+involves%3Akrassowski+updated%3A2023-07-31..2023-08-01&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 4.0.0
 
 ([Full Changelog](https://github.com/jupyterlab-contrib/jupyterlab-vim/compare/1.1.0...718d294cbbab1010ffaf35c79773e3abc5d98a6c))
 
 ### Enhancements made
 
 - Add support for vim mode in Text Editor [#90](https://github.com/jupyterlab-contrib/jupyterlab-vim/pull/90) ([@krassowski](https://github.com/krassowski))
@@ -29,16 +54,14 @@
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/jupyterlab-contrib/jupyterlab-vim/graphs/contributors?from=2022-03-12&to=2023-07-31&type=c))
 
 [@alexveden](https://github.com/search?q=repo%3Ajupyterlab-contrib%2Fjupyterlab-vim+involves%3Aalexveden+updated%3A2022-03-12..2023-07-31&type=Issues) | [@asford](https://github.com/search?q=repo%3Ajupyterlab-contrib%2Fjupyterlab-vim+involves%3Aasford+updated%3A2022-03-12..2023-07-31&type=Issues) | [@github-actions](https://github.com/search?q=repo%3Ajupyterlab-contrib%2Fjupyterlab-vim+involves%3Agithub-actions+updated%3A2022-03-12..2023-07-31&type=Issues) | [@ianhi](https://github.com/search?q=repo%3Ajupyterlab-contrib%2Fjupyterlab-vim+involves%3Aianhi+updated%3A2022-03-12..2023-07-31&type=Issues) | [@krassowski](https://github.com/search?q=repo%3Ajupyterlab-contrib%2Fjupyterlab-vim+involves%3Akrassowski+updated%3A2022-03-12..2023-07-31&type=Issues) | [@peytondmurray](https://github.com/search?q=repo%3Ajupyterlab-contrib%2Fjupyterlab-vim+involves%3Apeytondmurray+updated%3A2022-03-12..2023-07-31&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 # History
 
 ## 0.17.0 / 2023-07-30
 
 - Support JupyterLab 4.0 (#85, thanks @krassowski)
 
 ## 0.16.0 / 2023-03-12
```

### Comparing `jupyterlab_vim-4.0.0/RELEASE.md` & `jupyterlab_vim-4.0.1/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_vim-4.0.0/modify-keybinds.md` & `jupyterlab_vim-4.0.1/modify-keybinds.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_vim-4.0.0/package.json` & `jupyterlab_vim-4.0.1/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'4.0.1'"}*

```diff
@@ -187,9 +187,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "4.0.0"
+    "version": "4.0.1"
 }
```

### Comparing `jupyterlab_vim-4.0.0/tsconfig.json` & `jupyterlab_vim-4.0.1/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_vim-4.0.0/yarn.lock` & `jupyterlab_vim-4.0.1/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_vim-4.0.0/jupyterlab_vim/labextension/package.json` & `jupyterlab_vim-4.0.1/jupyterlab_vim/labextension/package.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9787326388888888%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.ddb05f98b2e0f61dea44.js'}}",*

 * * "'version'": "'4.0.1'"}*

```diff
@@ -117,15 +117,15 @@
         "schema/**/*.{json,}",
         "style/index.js"
     ],
     "homepage": "https://github.com/jupyterlab-contrib/jupyterlab-vim",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.a73b7957e55f8d1b9f75.js",
+            "load": "static/remoteEntry.ddb05f98b2e0f61dea44.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "jupyterlab_vim/labextension",
         "schemaDir": "schema"
     },
     "keywords": [
@@ -192,9 +192,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "4.0.0"
+    "version": "4.0.1"
 }
```

### Comparing `jupyterlab_vim-4.0.0/jupyterlab_vim/labextension/schemas/@axlair/jupyterlab_vim/package.json.orig` & `jupyterlab_vim-4.0.1/jupyterlab_vim/labextension/schemas/@axlair/jupyterlab_vim/package.json.orig`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'4.0.1'"}*

```diff
@@ -187,9 +187,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "4.0.0"
+    "version": "4.0.1"
 }
```

### Comparing `jupyterlab_vim-4.0.0/jupyterlab_vim/labextension/schemas/@axlair/jupyterlab_vim/plugin.json` & `jupyterlab_vim-4.0.1/jupyterlab_vim/labextension/schemas/@axlair/jupyterlab_vim/plugin.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_vim-4.0.0/jupyterlab_vim/labextension/static/252.e0500116419ca3a355d1.js` & `jupyterlab_vim-4.0.1/jupyterlab_vim/labextension/static/252.e0500116419ca3a355d1.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_vim-4.0.0/jupyterlab_vim/labextension/static/353.8b609c372dc07b2baac6.js` & `jupyterlab_vim-4.0.1/jupyterlab_vim/labextension/static/353.9c6b79c5ee878d215a0a.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -19,15 +19,15 @@
                 }) {
                     this._lastActiveEditor = null, this.enabled = e, this.userKeybindings = null != t ? t : []
                 }
                 async onActiveEditorChanged(e, t) {
                     t && (await t.content.ready, this.modifyEditor(t.content.editor))
                 }
                 updateLastActive() {
-                    this.modifyEditor(this._lastActiveEditor)
+                    this._lastActiveEditor && this.modifyEditor(this._lastActiveEditor)
                 }
                 modifyEditor(e) {
                     const t = e;
                     if (!t) throw Error("Editor not available");
                     this._lastActiveEditor = t;
                     const o = t.editor;
                     if (this.enabled) {
@@ -66,15 +66,15 @@
                         enabled: t
                     }), this._lastActiveCell = null, this._commands = e
                 }
                 onActiveCellChanged(e, t) {
                     this.modifyCell(t).catch(console.error)
                 }
                 updateLastActive() {
-                    this.modifyCell(this._lastActiveCell)
+                    this._lastActiveCell && this.modifyCell(this._lastActiveCell)
                 }
                 async modifyCell(e) {
                     e && (this._lastActiveCell = e, await e.ready, e.isDisposed ? console.warn("Cell was already disposed, cannot setup vim mode") : this.modifyEditor(e.editor) && this._modifyEdgeNavigation(e))
                 }
                 _modifyEdgeNavigation(e) {
                     const t = (o, n, i, l) => {
                         const d = n;
```

### Comparing `jupyterlab_vim-4.0.0/jupyterlab_vim/labextension/static/747.a573445024188eae7034.js` & `jupyterlab_vim-4.0.1/jupyterlab_vim/labextension/static/747.a573445024188eae7034.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_vim-4.0.0/jupyterlab_vim/labextension/static/remoteEntry.a73b7957e55f8d1b9f75.js` & `jupyterlab_vim-4.0.1/jupyterlab_vim/labextension/static/remoteEntry.ddb05f98b2e0f61dea44.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -44,21 +44,21 @@
     }, j.d = (e, r) => {
         for (var t in r) j.o(r, t) && !j.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, j.f = {}, j.e = e => Promise.all(Object.keys(j.f).reduce(((r, t) => (j.f[t](e, r), r)), [])), j.u = e => e + "." + {
         252: "e0500116419ca3a355d1",
-        353: "8b609c372dc07b2baac6",
+        353: "9c6b79c5ee878d215a0a",
         598: "ad606b2bbb9816d73182",
         747: "a573445024188eae7034",
         818: "53acaa7ded124a9243cd"
     } [e] + ".js?v=" + {
         252: "e0500116419ca3a355d1",
-        353: "8b609c372dc07b2baac6",
+        353: "9c6b79c5ee878d215a0a",
         598: "ad606b2bbb9816d73182",
         747: "a573445024188eae7034",
         818: "53acaa7ded124a9243cd"
     } [e], j.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
@@ -113,15 +113,15 @@
                         (!l || !l.loaded && (!a != !l.eager ? a : i > l.from)) && (o[r] = {
                             get: t,
                             from: i,
                             eager: !!a
                         })
                     },
                     u = [];
-                return "default" === t && (l("@axlair/jupyterlab_vim", "4.0.0", (() => Promise.all([j.e(598), j.e(353)]).then((() => () => j(353))))), l("@replit/codemirror-vim", "6.0.14", (() => Promise.all([j.e(252), j.e(598), j.e(818)]).then((() => () => j(252)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                return "default" === t && (l("@axlair/jupyterlab_vim", "4.0.1", (() => Promise.all([j.e(598), j.e(353)]).then((() => () => j(353))))), l("@replit/codemirror-vim", "6.0.14", (() => Promise.all([j.e(252), j.e(598), j.e(818)]).then((() => () => j(252)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         j.g.importScripts && (e = j.g.location + "");
         var r = j.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
```

### Comparing `jupyterlab_vim-4.0.0/jupyterlab_vim/labextension/static/third-party-licenses.json` & `jupyterlab_vim-4.0.1/jupyterlab_vim/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_vim-4.0.0/schema/plugin.json` & `jupyterlab_vim-4.0.1/schema/plugin.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_vim-4.0.0/src/codemirrorCommands.ts` & `jupyterlab_vim-4.0.1/src/codemirrorCommands.ts`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,17 @@
       return;
     }
     await activeEditor.content.ready;
     this.modifyEditor(activeEditor.content.editor);
   }
 
   updateLastActive() {
+    if (!this._lastActiveEditor) {
+      return;
+    }
     this.modifyEditor(this._lastActiveEditor);
   }
 
   modifyEditor(editor: CodeEditor.IEditor | null): boolean {
     // JupyterLab 4.0 only supports CodeMirror editors
     const mirrorEditor = editor as CodeMirrorEditor | null;
 
@@ -157,14 +160,17 @@
     tracker: INotebookTracker,
     activeCell: Cell<ICellModel> | null
   ): void {
     this.modifyCell(activeCell).catch(console.error);
   }
 
   updateLastActive() {
+    if (!this._lastActiveCell) {
+      return;
+    }
     this.modifyCell(this._lastActiveCell);
   }
 
   async modifyCell(activeCell: Cell<ICellModel> | null): Promise<void> {
     if (!activeCell) {
       return;
     }
```

### Comparing `jupyterlab_vim-4.0.0/src/index.ts` & `jupyterlab_vim-4.0.1/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_vim-4.0.0/src/labCommands.ts` & `jupyterlab_vim-4.0.1/src/labCommands.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_vim-4.0.0/.gitignore` & `jupyterlab_vim-4.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_vim-4.0.0/LICENSE` & `jupyterlab_vim-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_vim-4.0.0/README.md` & `jupyterlab_vim-4.0.1/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_vim-4.0.0/pyproject.toml` & `jupyterlab_vim-4.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_vim-4.0.0/PKG-INFO` & `jupyterlab_vim-4.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab_vim
-Version: 4.0.0
+Version: 4.0.1
 Summary: Code cell vim bindings
 Project-URL: Homepage, https://github.com/jupyterlab-contrib/jupyterlab-vim
 Project-URL: Bug Tracker, https://github.com/jupyterlab-contrib/jupyterlab-vim/issues
 Project-URL: Repository, https://github.com/jupyterlab-contrib/jupyterlab-vim.git
 Author: Axel Fahy
 License: MIT License
```

