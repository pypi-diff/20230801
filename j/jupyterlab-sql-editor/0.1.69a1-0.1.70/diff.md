# Comparing `tmp/jupyterlab_sql_editor-0.1.69a1.tar.gz` & `tmp/jupyterlab_sql_editor-0.1.70.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterlab_sql_editor-0.1.69a1.tar", last modified: Fri Jul  7 16:21:05 2023, max compression
+gzip compressed data, was "jupyterlab_sql_editor-0.1.70.tar", last modified: Tue Aug  1 17:19:35 2023, max compression
```

## Comparing `jupyterlab_sql_editor-0.1.69a1.tar` & `jupyterlab_sql_editor-0.1.70.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-07 16:21:05.205593 jupyterlab_sql_editor-0.1.69a1/
--rw-r--r--   0 vsts      (1001) docker     (123)     1074 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (123)      472 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (123)     8199 2023-07-07 16:21:05.201593 jupyterlab_sql_editor-0.1.69a1/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     6928 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)     1905 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/RELEASE.md
--rw-r--r--   0 vsts      (1001) docker     (123)      203 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/install.json
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-07 16:21:05.193592 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/
--rw-r--r--   0 vsts      (1001) docker     (123)      261 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      471 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/_version.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-07 16:21:05.197593 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython/
--rw-r--r--   0 vsts      (1001) docker     (123)     3125 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython/SparkSchemaWidget.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8098 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython/balls_line.gif
--rw-r--r--   0 vsts      (1001) docker     (123)     4960 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython/common.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8623 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython/spark_streaming_query.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7828 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython/sparkdf.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-07 16:21:05.197593 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython_magic/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython_magic/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-07 16:21:05.197593 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython_magic/common/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython_magic/common/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4621 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython_magic/common/base.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9263 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython_magic/common/export.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-07 16:21:05.197593 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython_magic/sparksql/
--rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython_magic/sparksql/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1768 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython_magic/sparksql/main.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4722 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython_magic/sparksql/spark_export.py
--rw-r--r--   0 vsts      (1001) docker     (123)    10866 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython_magic/sparksql/sparksql.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-07 16:21:05.197593 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython_magic/trino/
--rw-r--r--   0 vsts      (1001) docker     (123)       99 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython_magic/trino/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1750 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython_magic/trino/main.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5389 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython_magic/trino/parser.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7418 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython_magic/trino/parser_test.py
--rw-r--r--   0 vsts      (1001) docker     (123)    35548 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython_magic/trino/parsetab.py
--rw-r--r--   0 vsts      (1001) docker     (123)    10359 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython_magic/trino/trino.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3539 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython_magic/trino/trino_export.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-07 16:21:05.197593 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/labextension/
--rw-r--r--   0 vsts      (1001) docker     (123)    21048 2023-07-07 16:20:38.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/labextension/build_log.json
--rw-r--r--   0 vsts      (1001) docker     (123)     4037 2023-07-07 16:20:39.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/labextension/package.json
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-07 16:21:05.189592 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/labextension/schemas/
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-07 16:21:05.197593 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/labextension/schemas/jupyterlab-sql-editor/
--rw-r--r--   0 vsts      (1001) docker     (123)     3895 2023-07-07 16:20:38.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/labextension/schemas/jupyterlab-sql-editor/package.json.orig
--rw-r--r--   0 vsts      (1001) docker     (123)     1159 2023-07-07 16:20:38.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/labextension/schemas/jupyterlab-sql-editor/plugin.json
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-07 16:21:05.201593 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/labextension/static/
--rw-r--r--   0 vsts      (1001) docker     (123)    23411 2023-07-07 16:20:39.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/labextension/static/lib_index_js.67b6c3715f795c58c5d6.js
--rw-r--r--   0 vsts      (1001) docker     (123)    31873 2023-07-07 16:20:39.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/labextension/static/lib_index_js.67b6c3715f795c58c5d6.js.map
--rw-r--r--   0 vsts      (1001) docker     (123)    29620 2023-07-07 16:20:39.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/labextension/static/remoteEntry.7a5c41927a28f0d15d2b.js
--rw-r--r--   0 vsts      (1001) docker     (123)    28468 2023-07-07 16:20:39.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/labextension/static/remoteEntry.7a5c41927a28f0d15d2b.js.map
--rw-r--r--   0 vsts      (1001) docker     (123)      164 2023-07-07 16:20:38.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/labextension/static/style.js
--rw-r--r--   0 vsts      (1001) docker     (123)     4266 2023-07-07 16:20:39.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/labextension/static/style_index_js.7a9353dfa84524daa532.js
--rw-r--r--   0 vsts      (1001) docker     (123)     1437 2023-07-07 16:20:39.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/labextension/static/style_index_js.7a9353dfa84524daa532.js.map
--rw-r--r--   0 vsts      (1001) docker     (123)    12072 2023-07-07 16:20:39.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.8ab7ecce559b1f364311.js
--rw-r--r--   0 vsts      (1001) docker     (123)    13811 2023-07-07 16:20:39.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.8ab7ecce559b1f364311.js.map
--rw-r--r--   0 vsts      (1001) docker     (123)   361933 2023-07-07 16:20:39.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/labextension/static/vendors-node_modules_sql-formatter_lib_index_js.1955e937c0ff0f3413ea.js
--rw-r--r--   0 vsts      (1001) docker     (123)   485462 2023-07-07 16:20:39.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/labextension/static/vendors-node_modules_sql-formatter_lib_index_js.1955e937c0ff0f3413ea.js.map
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-07 16:21:05.193592 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     8199 2023-07-07 16:21:05.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     3163 2023-07-07 16:21:05.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-07 16:21:05.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)      357 2023-07-07 16:21:05.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-07 16:19:31.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       78 2023-07-07 16:21:05.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       22 2023-07-07 16:21:05.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor.egg-info/top_level.txt
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-07 16:21:05.201593 jupyterlab_sql_editor-0.1.69a1/overrides/
--rw-r--r--   0 vsts      (1001) docker     (123)      676 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/overrides/sparksql-lsp.json
--rw-r--r--   0 vsts      (1001) docker     (123)       91 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/overrides/syntax_highlighting.json
--rw-r--r--   0 vsts      (1001) docker     (123)      671 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/overrides/trino-lsp.json
--rw-r--r--   0 vsts      (1001) docker     (123)     3895 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/package.json
--rw-r--r--   0 vsts      (1001) docker     (123)      619 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/pyproject.toml
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-07 16:21:05.201593 jupyterlab_sql_editor-0.1.69a1/schema/
--rw-r--r--   0 vsts      (1001) docker     (123)     1159 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/schema/plugin.json
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-07-07 16:21:05.205593 jupyterlab_sql_editor-0.1.69a1/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     3960 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-07 16:21:05.201593 jupyterlab_sql_editor-0.1.69a1/src/
--rw-r--r--   0 vsts      (1001) docker     (123)      362 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/src/constants.ts
--rw-r--r--   0 vsts      (1001) docker     (123)     8368 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/src/formatter.ts
--rw-r--r--   0 vsts      (1001) docker     (123)     6249 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/src/index.ts
--rw-r--r--   0 vsts      (1001) docker     (123)     3429 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/src/utils.ts
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-07 16:21:05.201593 jupyterlab_sql_editor-0.1.69a1/style/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/style/base.css
--rw-r--r--   0 vsts      (1001) docker     (123)       25 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/style/index.css
--rw-r--r--   0 vsts      (1001) docker     (123)       21 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/style/index.js
--rw-r--r--   0 vsts      (1001) docker     (123)      554 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/tsconfig.json
--rw-r--r--   0 vsts      (1001) docker     (123)   228103 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/yarn.lock
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 17:19:35.430406 jupyterlab_sql_editor-0.1.70/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1074 2023-08-01 17:17:13.000000 jupyterlab_sql_editor-0.1.70/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (123)      472 2023-08-01 17:17:13.000000 jupyterlab_sql_editor-0.1.70/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (123)     8197 2023-08-01 17:19:35.430406 jupyterlab_sql_editor-0.1.70/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     6928 2023-08-01 17:17:13.000000 jupyterlab_sql_editor-0.1.70/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)     1905 2023-08-01 17:17:13.000000 jupyterlab_sql_editor-0.1.70/RELEASE.md
+-rw-r--r--   0 vsts      (1001) docker     (123)      203 2023-08-01 17:17:13.000000 jupyterlab_sql_editor-0.1.70/install.json
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 17:19:35.422406 jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/
+-rw-r--r--   0 vsts      (1001) docker     (123)      261 2023-08-01 17:17:13.000000 jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      471 2023-08-01 17:17:13.000000 jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/_version.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 17:19:35.426406 jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/ipython/
+-rw-r--r--   0 vsts      (1001) docker     (123)     3125 2023-08-01 17:17:13.000000 jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/ipython/SparkSchemaWidget.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-08-01 17:17:13.000000 jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/ipython/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8098 2023-08-01 17:17:13.000000 jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/ipython/balls_line.gif
+-rw-r--r--   0 vsts      (1001) docker     (123)     4960 2023-08-01 17:17:13.000000 jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/ipython/common.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8623 2023-08-01 17:17:13.000000 jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/ipython/spark_streaming_query.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6895 2023-08-01 17:17:13.000000 jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/ipython/sparkdf.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 17:19:35.426406 jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/ipython_magic/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-08-01 17:17:13.000000 jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/ipython_magic/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 17:19:35.426406 jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/ipython_magic/common/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-08-01 17:17:13.000000 jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/ipython_magic/common/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4621 2023-08-01 17:17:13.000000 jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/ipython_magic/common/base.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9263 2023-08-01 17:17:13.000000 jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/ipython_magic/common/export.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 17:19:35.426406 jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/ipython_magic/sparksql/
+-rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-08-01 17:17:13.000000 jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/ipython_magic/sparksql/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1768 2023-08-01 17:17:13.000000 jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/ipython_magic/sparksql/main.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4722 2023-08-01 17:17:13.000000 jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/ipython_magic/sparksql/spark_export.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11138 2023-08-01 17:17:13.000000 jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/ipython_magic/sparksql/sparksql.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 17:19:35.426406 jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/ipython_magic/trino/
+-rw-r--r--   0 vsts      (1001) docker     (123)       99 2023-08-01 17:17:13.000000 jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/ipython_magic/trino/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1750 2023-08-01 17:17:13.000000 jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/ipython_magic/trino/main.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5389 2023-08-01 17:17:13.000000 jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/ipython_magic/trino/parser.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7418 2023-08-01 17:17:13.000000 jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/ipython_magic/trino/parser_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    35548 2023-08-01 17:17:13.000000 jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/ipython_magic/trino/parsetab.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    10544 2023-08-01 17:17:13.000000 jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/ipython_magic/trino/trino.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3539 2023-08-01 17:17:13.000000 jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/ipython_magic/trino/trino_export.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 17:19:35.426406 jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/labextension/
+-rw-r--r--   0 vsts      (1001) docker     (123)    21041 2023-08-01 17:19:10.000000 jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/labextension/build_log.json
+-rw-r--r--   0 vsts      (1001) docker     (123)     4031 2023-08-01 17:19:11.000000 jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/labextension/package.json
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 17:19:35.422406 jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/labextension/schemas/
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 17:19:35.426406 jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/labextension/schemas/jupyterlab-sql-editor/
+-rw-r--r--   0 vsts      (1001) docker     (123)     3889 2023-08-01 17:19:10.000000 jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/labextension/schemas/jupyterlab-sql-editor/package.json.orig
+-rw-r--r--   0 vsts      (1001) docker     (123)     1159 2023-08-01 17:19:10.000000 jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/labextension/schemas/jupyterlab-sql-editor/plugin.json
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 17:19:35.430406 jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/labextension/static/
+-rw-r--r--   0 vsts      (1001) docker     (123)    23425 2023-08-01 17:19:11.000000 jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/labextension/static/lib_index_js.4c0329159cbdd7702e52.js
+-rw-r--r--   0 vsts      (1001) docker     (123)    31876 2023-08-01 17:19:11.000000 jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/labextension/static/lib_index_js.4c0329159cbdd7702e52.js.map
+-rw-r--r--   0 vsts      (1001) docker     (123)    29614 2023-08-01 17:19:11.000000 jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/labextension/static/remoteEntry.5141fb70facd63fa9a6c.js
+-rw-r--r--   0 vsts      (1001) docker     (123)    28462 2023-08-01 17:19:11.000000 jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/labextension/static/remoteEntry.5141fb70facd63fa9a6c.js.map
+-rw-r--r--   0 vsts      (1001) docker     (123)      164 2023-08-01 17:19:10.000000 jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/labextension/static/style.js
+-rw-r--r--   0 vsts      (1001) docker     (123)     4266 2023-08-01 17:19:11.000000 jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/labextension/static/style_index_js.7a9353dfa84524daa532.js
+-rw-r--r--   0 vsts      (1001) docker     (123)     1437 2023-08-01 17:19:11.000000 jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/labextension/static/style_index_js.7a9353dfa84524daa532.js.map
+-rw-r--r--   0 vsts      (1001) docker     (123)    12072 2023-08-01 17:19:11.000000 jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.8ab7ecce559b1f364311.js
+-rw-r--r--   0 vsts      (1001) docker     (123)    13811 2023-08-01 17:19:11.000000 jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.8ab7ecce559b1f364311.js.map
+-rw-r--r--   0 vsts      (1001) docker     (123)   361933 2023-08-01 17:19:11.000000 jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/labextension/static/vendors-node_modules_sql-formatter_lib_index_js.1955e937c0ff0f3413ea.js
+-rw-r--r--   0 vsts      (1001) docker     (123)   485462 2023-08-01 17:19:11.000000 jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/labextension/static/vendors-node_modules_sql-formatter_lib_index_js.1955e937c0ff0f3413ea.js.map
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 17:19:35.426406 jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     8197 2023-08-01 17:19:35.000000 jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     3163 2023-08-01 17:19:35.000000 jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-08-01 17:19:35.000000 jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)      357 2023-08-01 17:19:35.000000 jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-08-01 17:18:02.000000 jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       78 2023-08-01 17:19:35.000000 jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       22 2023-08-01 17:19:35.000000 jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 17:19:35.430406 jupyterlab_sql_editor-0.1.70/overrides/
+-rw-r--r--   0 vsts      (1001) docker     (123)      677 2023-08-01 17:17:13.000000 jupyterlab_sql_editor-0.1.70/overrides/sparksql-lsp.json
+-rw-r--r--   0 vsts      (1001) docker     (123)       91 2023-08-01 17:17:13.000000 jupyterlab_sql_editor-0.1.70/overrides/syntax_highlighting.json
+-rw-r--r--   0 vsts      (1001) docker     (123)      672 2023-08-01 17:17:13.000000 jupyterlab_sql_editor-0.1.70/overrides/trino-lsp.json
+-rw-r--r--   0 vsts      (1001) docker     (123)     3889 2023-08-01 17:17:13.000000 jupyterlab_sql_editor-0.1.70/package.json
+-rw-r--r--   0 vsts      (1001) docker     (123)      619 2023-08-01 17:17:13.000000 jupyterlab_sql_editor-0.1.70/pyproject.toml
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 17:19:35.430406 jupyterlab_sql_editor-0.1.70/schema/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1159 2023-08-01 17:17:13.000000 jupyterlab_sql_editor-0.1.70/schema/plugin.json
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-08-01 17:19:35.434406 jupyterlab_sql_editor-0.1.70/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     3960 2023-08-01 17:17:13.000000 jupyterlab_sql_editor-0.1.70/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 17:19:35.430406 jupyterlab_sql_editor-0.1.70/src/
+-rw-r--r--   0 vsts      (1001) docker     (123)      362 2023-08-01 17:17:13.000000 jupyterlab_sql_editor-0.1.70/src/constants.ts
+-rw-r--r--   0 vsts      (1001) docker     (123)     8369 2023-08-01 17:17:13.000000 jupyterlab_sql_editor-0.1.70/src/formatter.ts
+-rw-r--r--   0 vsts      (1001) docker     (123)     6250 2023-08-01 17:17:13.000000 jupyterlab_sql_editor-0.1.70/src/index.ts
+-rw-r--r--   0 vsts      (1001) docker     (123)     3430 2023-08-01 17:17:13.000000 jupyterlab_sql_editor-0.1.70/src/utils.ts
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 17:19:35.430406 jupyterlab_sql_editor-0.1.70/style/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-08-01 17:17:13.000000 jupyterlab_sql_editor-0.1.70/style/base.css
+-rw-r--r--   0 vsts      (1001) docker     (123)       25 2023-08-01 17:17:13.000000 jupyterlab_sql_editor-0.1.70/style/index.css
+-rw-r--r--   0 vsts      (1001) docker     (123)       21 2023-08-01 17:17:13.000000 jupyterlab_sql_editor-0.1.70/style/index.js
+-rw-r--r--   0 vsts      (1001) docker     (123)      554 2023-08-01 17:17:13.000000 jupyterlab_sql_editor-0.1.70/tsconfig.json
+-rw-r--r--   0 vsts      (1001) docker     (123)   228150 2023-08-01 17:17:13.000000 jupyterlab_sql_editor-0.1.70/yarn.lock
```

### Comparing `jupyterlab_sql_editor-0.1.69a1/LICENSE` & `jupyterlab_sql_editor-0.1.70/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.69a1/PKG-INFO` & `jupyterlab_sql_editor-0.1.70/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab_sql_editor
-Version: 0.1.69a1
+Version: 0.1.70
 Summary: SQL editor support for formatting, syntax highlighting and code completion of SQL in cell magic, line magic, python string and file editor.
 Home-page: https://github.com/CybercentreCanada/jupyterlab-sql-editor
 Author: cccs-jc
 Author-email: contact@cyber.gc.ca
 License: MIT License (MIT)
 Keywords: sql,Jupyter,JupyterLab,JupyterLab3,jupyter,jupyterlab-extension,spark,trino,dataframe,cccs,canada
 Platform: Linux
```

### Comparing `jupyterlab_sql_editor-0.1.69a1/README.md` & `jupyterlab_sql_editor-0.1.70/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.69a1/RELEASE.md` & `jupyterlab_sql_editor-0.1.70/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython/SparkSchemaWidget.py` & `jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/ipython/SparkSchemaWidget.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython/balls_line.gif` & `jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/ipython/balls_line.gif`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython/common.py` & `jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/ipython/common.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython/spark_streaming_query.py` & `jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/ipython/spark_streaming_query.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython/sparkdf.py` & `jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/ipython/sparkdf.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,60 +47,41 @@
 
 
 def display_spark_df(df, output, limit, truncate, show_nonprinting, args):
     """
     Execute the query of the dataframe and time the execution.
     """
     displays = []
-    start = time()
-    has_more_data = False
     if output == "grid":
-        has_more_data, pdf = to_pandas(df, limit, truncate, show_nonprinting)
+        pdf = to_pandas(df, limit, truncate, show_nonprinting)
         displays.append(render_grid(pdf, limit))
     elif output == "aggrid":
-        has_more_data, pdf = to_pandas(df, limit, truncate, show_nonprinting)
+        pdf = to_pandas(df, limit, truncate, show_nonprinting)
         displays.append(render_ag_grid(pdf))
     elif output == "json":
         json_array = []
         warnings = []
         results = df.toJSON().map(lambda j: json.loads(j)).take(limit)
-        if len(results) > limit:
-            has_more_data = True
         # cast unsafe ints to str for display
         for row in results:
             json_array.append(sanitize_results(row, warnings))
         # add warnings to displays
         for warning in warnings:
             displays.append(warning)
         if show_nonprinting:
             recursive_escape(json_array)
         displays.append(JSON(json_array, expanded=args.expand))
     elif output == "html":
-        has_more_data, html_text = to_html(df, limit, truncate, show_nonprinting)
+        html_text = to_html(df, limit, truncate, show_nonprinting)
         displays.append(HTML(html_text))
     elif output == "text":
         text = df._jdf.showString(limit, truncate, False)
         displays.append(PlainText(data=text))
-    elif limit <= 0 or output == "skip" or output == "none":
-        displays.append("Query execution skipped")
-        return []
-    elif output == "schema":
-        df.printSchema()
-        return []
-    else:
-        displays.append(PlainText(data=f"Invalid output option {output}, valid options are grid, json, html, text"))
-    end = time()
-    elapsed = end - start
-    if has_more_data:
-        message = "only showing top %d %s\n" % (
-            limit,
-            "row" if limit == 1 else "rows",
-        )
-        displays.append(PlainText(data=message))
-    displays.append(PlainText(data=f"Execution time: {elapsed:.2f} seconds"))
+    elif output == "skip" or output == "none":
+        displays.append(PlainText(data="Display of results skipped"))
     return displays
 
 
 def display_link():
     """
     Display a link in notebook so a user can open the spark UI's details.
     """
@@ -190,32 +171,28 @@
     Execute the query unerlying the dataframe and creates an html representation of the results.
     Code inspired from spark's dataframe.py
     """
     sock_info = df._jdf.getRowsToPython(max_num_rows, truncate)
     rows = list(_load_from_socket(sock_info, BatchedSerializer(PickleSerializer())))
     columns = rows[0]
     row_data = rows[1:]
-    has_more_data = len(row_data) > max_num_rows
     row_data = row_data[:max_num_rows]
     html = rows_to_html(columns, row_data, show_nonprinting)
-    if has_more_data:
-        html += "only showing top %d %s\n" % (max_num_rows, "row" if max_num_rows == 1 else "rows")
-    return has_more_data, html
+    return html
 
 
 def to_pandas(df, max_num_rows, truncate, show_nonprinting):
     """
     Execute the query unerlying the dataframe and creates a pandas dataframe with the results.
     Code inspired from spark's dataframe.py
     """
     sock_info = df._jdf.getRowsToPython(max_num_rows, truncate)
     rows = list(_load_from_socket(sock_info, BatchedSerializer(PickleSerializer())))
     head = rows[0]
     row_data = rows[1:]
-    has_more_data = len(row_data) > max_num_rows
     row_data = row_data[:max_num_rows]
     pdf = pd.DataFrame(columns=head)
     for i, row in enumerate(row_data):
         if show_nonprinting:
             row = [escape_control_chars(str(v)) for v in row]
         pdf.loc[i] = row
-    return has_more_data, pdf
+    return pdf
```

### Comparing `jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython_magic/common/base.py` & `jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/ipython_magic/common/base.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython_magic/common/export.py` & `jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/ipython_magic/common/export.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython_magic/sparksql/main.py` & `jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/ipython_magic/sparksql/main.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython_magic/sparksql/spark_export.py` & `jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/ipython_magic/sparksql/spark_export.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython_magic/sparksql/sparksql.py` & `jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/ipython_magic/sparksql/sparksql.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,15 +114,15 @@
         streaming_mode = args.streaming_mode.lower()
 
         truncate = 256
         if args.truncate and args.truncate > 0:
             truncate = args.truncate
 
         limit = args.limit
-        if limit is None:
+        if limit is None or limit <= 0:
             limit = self.limit
 
         if output not in VALID_OUTPUTS:
             print(f"Invalid output option {args.output}. The valid options are {VALID_OUTPUTS}.")
             return
 
         self.spark = self.get_instantiated_spark_session()
@@ -150,26 +150,30 @@
         # statements like INSERT INTO, USE SCHEMA, CREATE TABLE, DROP TABLE
         # execute immediatly, they do not require us to perform a .show(), .collect()
         # we detect these use case by checking for an empty list of columns (no return schema)
         # we treat these use cases differently than a SELECT that returns rows of data
         start = time()
         try:
             df = self.spark.sql(sql)
+            if output == "schema":
+                df.printSchema()
+                return
             results = self.spark.createDataFrame(df.take(limit + 1), schema=df.schema)
         except PYSPARK_ERROR_TYPES as exc:
             if args.lean_exceptions:
                 self.print_pyspark_error(exc)
                 return
             else:
                 raise exc
         end = time()
-        if len(results.columns) == 0:
-            elapsed = end - start
-            print(f"Execution time: {elapsed:.2f} seconds")
-            return
+        print(f"Execution time: {end - start:.2f} seconds")
+
+        # The text output already has it's own message coming from Spark
+        if results.count() > limit and not (output == "skip" or output == "none" or output == "text"):
+            print(f"Only showing top {limit} {'row' if limit == 1 else 'rows'}")
 
         if args.cache or args.eager:
             load_type = "eager" if args.eager else "lazy"
             print(f"Cached dataframe with {load_type} load")
             results = results.cache()
             if args.eager:
                 results.count()
```

### Comparing `jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython_magic/trino/main.py` & `jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/ipython_magic/trino/main.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython_magic/trino/parser.py` & `jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/ipython_magic/trino/parser.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython_magic/trino/parser_test.py` & `jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/ipython_magic/trino/parser_test.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython_magic/trino/parsetab.py` & `jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/ipython_magic/trino/parsetab.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython_magic/trino/trino.py` & `jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/ipython_magic/trino/trino.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 import os
+from time import time
 
 import pandas as pd
 import trino
 from IPython.core.magic import line_cell_magic, magics_class, needs_local_scope
 from IPython.core.magic_arguments import argument, magic_arguments, parse_argstring
 from IPython.display import HTML, JSON, display
 from traitlets import Bool, Instance, Int, Unicode, Union
@@ -114,30 +115,26 @@
             catalog = self.catalog
 
         schema = args.schema
         if not schema:
             schema = self.schema
 
         limit = args.limit
-        if limit is None:
+        if limit is None or limit <= 0:
             limit = self.limit
 
         catalog_array = self.get_catalog_array()
         if self.check_refresh(args.refresh.lower(), output_file, catalog_array):
             return
 
         output = args.output.lower()
         if output not in VALID_OUTPUTS:
             print(f"Invalid output option {args.output}. The valid options are {VALID_OUTPUTS}.")
             return
 
-        if limit <= 0 or output == "skip" or output == "none":
-            print("Query execution skipped")
-            return
-
         sql = self.get_sql_statement(cell, args.sql, args.jinja)
         if not sql:
             return
 
         if output == "sql":
             return self.display_sql(sql)
         elif not args.raw:
@@ -150,20 +147,23 @@
             user=self.user,
             catalog=catalog,
             schema=schema,
             http_scheme=self.httpScheme,
             verify=self.verify,
         )
         self.cur = self.conn.cursor()
+        start = time()
         self.cur.execute(sql)
         results = self.cur.fetchmany(limit + 1)
         columns = list(map(lambda d: d[0], self.cur.description))
+        end = time()
+        print(f"Execution time: {end - start:.2f} seconds")
 
-        if len(results) > limit:
-            print("Only showing top %d row(s)" % limit)
+        if len(results) > limit and not (output == "skip" or output == "none"):
+            print(f"Only showing top {limit} {'row' if limit == 1 else 'rows'}")
             results = results[:limit]
 
         results = list(map(lambda row: [self.format_cell(v, output, truncate) for v in row], results[:limit]))
 
         if args.dataframe:
             print(f"Saved results to pandas dataframe named `{args.dataframe}`")
             pdf = pd.DataFrame.from_records(results, columns=columns)
@@ -208,14 +208,16 @@
                 ),
             )
         elif output == "html":
             html = rows_to_html(columns, results, show_nonprinting)
             display(HTML(make_tag("table", False, html)))
         elif output == "text":
             print(self.render_text(results, columns))
+        elif output == "skip" or output == "none":
+            display("Display of results skipped")
 
     def check_refresh(self, refresh_arg, output_file, catalog_array):
         if refresh_arg == "all":
             update_database_schema(self.cur, output_file, catalog_array)
             return True
         if refresh_arg != "none":
             print(f"Invalid refresh option given {refresh_arg}. Valid refresh options are [all|local|none]")
```

### Comparing `jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython_magic/trino/trino_export.py` & `jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/ipython_magic/trino/trino_export.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/labextension/build_log.json` & `jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/labextension/build_log.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999835127149943%*

 * *Differences: {'0': "{'plugins': {1: {'_options': {'shared': {'jupyterlab-sql-editor': {'version': '0.1.70'}, "*

 * *      "'@jupyter-lsp/jupyterlab-lsp': OrderedDict([('singleton', True), ('import', False)]), "*

 * *      "delete: ['@krassowski/jupyterlab-lsp']}}}}}"}*

```diff
@@ -117,14 +117,18 @@
                             "_JUPYTERLAB",
                             "jupyterlab-sql-editor"
                         ],
                         "type": "var"
                     },
                     "name": "jupyterlab-sql-editor",
                     "shared": {
+                        "@jupyter-lsp/jupyterlab-lsp": {
+                            "import": false,
+                            "singleton": true
+                        },
                         "@jupyter/ydoc": {
                             "import": false,
                             "requiredVersion": "^0.2.0",
                             "singleton": true
                         },
                         "@jupyterlab/application": {
                             "import": false,
@@ -533,18 +537,14 @@
                             "import": false,
                             "requiredVersion": "^3.6.1"
                         },
                         "@jupyterlab/vega5-extension": {
                             "import": false,
                             "requiredVersion": "^3.6.1"
                         },
-                        "@krassowski/jupyterlab-lsp": {
-                            "import": false,
-                            "singleton": true
-                        },
                         "@lumino/algorithm": {
                             "import": false,
                             "requiredVersion": "^1.9.0",
                             "singleton": true
                         },
                         "@lumino/application": {
                             "import": false,
@@ -602,15 +602,15 @@
                             "singleton": true
                         },
                         "@types/codemirror": {},
                         "codemirror": {},
                         "jupyterlab-sql-editor": {
                             "import": "/home/vsts/work/1/s/lib/index.js",
                             "singleton": true,
-                            "version": "0.1.69-alpha.1"
+                            "version": "0.1.70"
                         },
                         "npm-run-all": {},
                         "react": {
                             "import": false,
                             "requiredVersion": "^17.0.1",
                             "singleton": true
                         },
```

### Comparing `jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/labextension/package.json` & `jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9691558441558441%*

 * *Differences: {"'dependencies'": "{'@jupyter-lsp/jupyterlab-lsp': '^4.2.0', delete: "*

 * *                   "['@krassowski/jupyterlab-lsp']}",*

 * * "'devDependencies'": "{'@jupyterlab/builder': '^3.6.5'}",*

 * * "'jupyterlab'": "{'sharedPackages': {replace: OrderedDict([('@jupyter-lsp/jupyterlab-lsp', "*

 * *                 "OrderedDict([('bundled', False), ('singleton', True)]))])}, '_build': {'load': "*

 * *                 "'static/remoteEntry.5141fb70facd63fa9a6c.js'}}",*

 * * "'version'": "'0.1.70'"}*

```diff
@@ -3,32 +3,32 @@
         "email": "contact@cyber.gc.ca",
         "name": "cccs-jc"
     },
     "bugs": {
         "url": "https://github.com/CybercentreCanada/jupyterlab-sql-editor/issues"
     },
     "dependencies": {
+        "@jupyter-lsp/jupyterlab-lsp": "^4.2.0",
         "@jupyterlab/application": "3.6.1",
         "@jupyterlab/apputils": "3.6.1",
         "@jupyterlab/cells": "3.6.1",
         "@jupyterlab/codemirror": "3.6.1",
         "@jupyterlab/docmanager": "3.6.1",
         "@jupyterlab/fileeditor": "3.6.1",
         "@jupyterlab/logconsole": "3.6.1",
         "@jupyterlab/notebook": "3.6.1",
         "@jupyterlab/settingregistry": "3.6.1",
-        "@krassowski/jupyterlab-lsp": "^3.10.2",
         "@types/codemirror": "^5.60.5",
         "codemirror": "~5.61.0",
         "npm-run-all": "^4.1.5",
         "sql-formatter": "6.1.2"
     },
     "description": "SQL editor support for formatting, syntax highlighting and code completion of SQL in cell magic, line magic, python string and file editor.",
     "devDependencies": {
-        "@jupyterlab/builder": "3.6.1",
+        "@jupyterlab/builder": "^3.6.5",
         "@types/node": "~18.11.9",
         "@typescript-eslint/eslint-plugin": "^4.8.1",
         "@typescript-eslint/parser": "^4.8.1",
         "eslint": "^7.14.0",
         "eslint-config-prettier": "^6.15.0",
         "eslint-plugin-prettier": "^3.1.4",
         "npm-run-all": "^4.1.5",
@@ -41,22 +41,22 @@
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*.json"
     ],
     "homepage": "https://github.com/CybercentreCanada/jupyterlab-sql-editor",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.7a5c41927a28f0d15d2b.js",
+            "load": "static/remoteEntry.5141fb70facd63fa9a6c.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "jupyterlab_sql_editor/labextension",
         "schemaDir": "schema",
         "sharedPackages": {
-            "@krassowski/jupyterlab-lsp": {
+            "@jupyter-lsp/jupyterlab-lsp": {
                 "bundled": false,
                 "singleton": true
             }
         }
     },
     "keywords": [
         "jupyter",
@@ -109,9 +109,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.69-alpha.1"
+    "version": "0.1.70"
 }
```

### Comparing `jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/labextension/schemas/jupyterlab-sql-editor/package.json.orig` & `jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/labextension/schemas/jupyterlab-sql-editor/package.json.orig`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9689574314574314%*

 * *Differences: {"'dependencies'": "{'@jupyter-lsp/jupyterlab-lsp': '^4.2.0', delete: "*

 * *                   "['@krassowski/jupyterlab-lsp']}",*

 * * "'devDependencies'": "{'@jupyterlab/builder': '^3.6.5'}",*

 * * "'jupyterlab'": "{'sharedPackages': {replace: OrderedDict([('@jupyter-lsp/jupyterlab-lsp', "*

 * *                 "OrderedDict([('bundled', False), ('singleton', True)]))])}}",*

 * * "'version'": "'0.1.70'"}*

```diff
@@ -3,32 +3,32 @@
         "email": "contact@cyber.gc.ca",
         "name": "cccs-jc"
     },
     "bugs": {
         "url": "https://github.com/CybercentreCanada/jupyterlab-sql-editor/issues"
     },
     "dependencies": {
+        "@jupyter-lsp/jupyterlab-lsp": "^4.2.0",
         "@jupyterlab/application": "3.6.1",
         "@jupyterlab/apputils": "3.6.1",
         "@jupyterlab/cells": "3.6.1",
         "@jupyterlab/codemirror": "3.6.1",
         "@jupyterlab/docmanager": "3.6.1",
         "@jupyterlab/fileeditor": "3.6.1",
         "@jupyterlab/logconsole": "3.6.1",
         "@jupyterlab/notebook": "3.6.1",
         "@jupyterlab/settingregistry": "3.6.1",
-        "@krassowski/jupyterlab-lsp": "^3.10.2",
         "@types/codemirror": "^5.60.5",
         "codemirror": "~5.61.0",
         "npm-run-all": "^4.1.5",
         "sql-formatter": "6.1.2"
     },
     "description": "SQL editor support for formatting, syntax highlighting and code completion of SQL in cell magic, line magic, python string and file editor.",
     "devDependencies": {
-        "@jupyterlab/builder": "3.6.1",
+        "@jupyterlab/builder": "^3.6.5",
         "@types/node": "~18.11.9",
         "@typescript-eslint/eslint-plugin": "^4.8.1",
         "@typescript-eslint/parser": "^4.8.1",
         "eslint": "^7.14.0",
         "eslint-config-prettier": "^6.15.0",
         "eslint-plugin-prettier": "^3.1.4",
         "npm-run-all": "^4.1.5",
@@ -43,15 +43,15 @@
     ],
     "homepage": "https://github.com/CybercentreCanada/jupyterlab-sql-editor",
     "jupyterlab": {
         "extension": true,
         "outputDir": "jupyterlab_sql_editor/labextension",
         "schemaDir": "schema",
         "sharedPackages": {
-            "@krassowski/jupyterlab-lsp": {
+            "@jupyter-lsp/jupyterlab-lsp": {
                 "bundled": false,
                 "singleton": true
             }
         }
     },
     "keywords": [
         "jupyter",
@@ -104,9 +104,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.69-alpha.1"
+    "version": "0.1.70"
 }
```

### Comparing `jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/labextension/schemas/jupyterlab-sql-editor/plugin.json` & `jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/labextension/schemas/jupyterlab-sql-editor/plugin.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/labextension/static/lib_index_js.67b6c3715f795c58c5d6.js` & `jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/labextension/static/lib_index_js.4c0329159cbdd7702e52.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -269,17 +269,17 @@
                     /* harmony export */
                 });
                 /* harmony import */
                 var _jupyterlab_settingregistry__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__( /*! @jupyterlab/settingregistry */ "webpack/sharing/consume/default/@jupyterlab/settingregistry");
                 /* harmony import */
                 var _jupyterlab_settingregistry__WEBPACK_IMPORTED_MODULE_0___default = /*#__PURE__*/ __webpack_require__.n(_jupyterlab_settingregistry__WEBPACK_IMPORTED_MODULE_0__);
                 /* harmony import */
-                var _krassowski_jupyterlab_lsp__WEBPACK_IMPORTED_MODULE_1__ = __webpack_require__( /*! @krassowski/jupyterlab-lsp */ "webpack/sharing/consume/default/@krassowski/jupyterlab-lsp");
+                var _jupyter_lsp_jupyterlab_lsp__WEBPACK_IMPORTED_MODULE_1__ = __webpack_require__( /*! @jupyter-lsp/jupyterlab-lsp */ "webpack/sharing/consume/default/@jupyter-lsp/jupyterlab-lsp");
                 /* harmony import */
-                var _krassowski_jupyterlab_lsp__WEBPACK_IMPORTED_MODULE_1___default = /*#__PURE__*/ __webpack_require__.n(_krassowski_jupyterlab_lsp__WEBPACK_IMPORTED_MODULE_1__);
+                var _jupyter_lsp_jupyterlab_lsp__WEBPACK_IMPORTED_MODULE_1___default = /*#__PURE__*/ __webpack_require__.n(_jupyter_lsp_jupyterlab_lsp__WEBPACK_IMPORTED_MODULE_1__);
                 /* harmony import */
                 var _jupyterlab_codemirror__WEBPACK_IMPORTED_MODULE_2__ = __webpack_require__( /*! @jupyterlab/codemirror */ "webpack/sharing/consume/default/@jupyterlab/codemirror");
                 /* harmony import */
                 var _jupyterlab_codemirror__WEBPACK_IMPORTED_MODULE_2___default = /*#__PURE__*/ __webpack_require__.n(_jupyterlab_codemirror__WEBPACK_IMPORTED_MODULE_2__);
                 /* harmony import */
                 var _jupyterlab_notebook__WEBPACK_IMPORTED_MODULE_3__ = __webpack_require__( /*! @jupyterlab/notebook */ "webpack/sharing/consume/default/@jupyterlab/notebook");
                 /* harmony import */
@@ -361,15 +361,15 @@
                  */
                 const plugin = {
                     id: 'jupyterlab-sql-editor:plugin',
                     autoStart: true,
                     optional: [],
                     requires: [
                         _jupyterlab_codemirror__WEBPACK_IMPORTED_MODULE_2__.ICodeMirror,
-                        _krassowski_jupyterlab_lsp__WEBPACK_IMPORTED_MODULE_1__.ILSPCodeExtractorsManager,
+                        _jupyter_lsp_jupyterlab_lsp__WEBPACK_IMPORTED_MODULE_1__.ILSPCodeExtractorsManager,
                         _jupyterlab_settingregistry__WEBPACK_IMPORTED_MODULE_0__.ISettingRegistry,
                         _jupyterlab_fileeditor__WEBPACK_IMPORTED_MODULE_4__.IEditorTracker,
                         _jupyterlab_notebook__WEBPACK_IMPORTED_MODULE_3__.INotebookTracker
                     ],
                     activate: (app, codeMirror, lspExtractorsMgr, settingRegistry, editorTracker, tracker) => {
                         console.log('JupyterLab extension jupyterlab-sql-editor is activated!');
                         const sqlFormatter = new _formatter__WEBPACK_IMPORTED_MODULE_6__.SqlFormatter(4, false, 'upper');
@@ -449,17 +449,17 @@
                     /* harmony export */
                     registerCodeMirrorFor: () => ( /* binding */ registerCodeMirrorFor),
                     /* harmony export */
                     sqlCodeMirrorModesFor: () => ( /* binding */ sqlCodeMirrorModesFor)
                     /* harmony export */
                 });
                 /* harmony import */
-                var _krassowski_jupyterlab_lsp__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__( /*! @krassowski/jupyterlab-lsp */ "webpack/sharing/consume/default/@krassowski/jupyterlab-lsp");
+                var _jupyter_lsp_jupyterlab_lsp__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__( /*! @jupyter-lsp/jupyterlab-lsp */ "webpack/sharing/consume/default/@jupyter-lsp/jupyterlab-lsp");
                 /* harmony import */
-                var _krassowski_jupyterlab_lsp__WEBPACK_IMPORTED_MODULE_0___default = /*#__PURE__*/ __webpack_require__.n(_krassowski_jupyterlab_lsp__WEBPACK_IMPORTED_MODULE_0__);
+                var _jupyter_lsp_jupyterlab_lsp__WEBPACK_IMPORTED_MODULE_0___default = /*#__PURE__*/ __webpack_require__.n(_jupyter_lsp_jupyterlab_lsp__WEBPACK_IMPORTED_MODULE_0__);
 
                 function line_magic(language) {
                     return `%${language}`;
                 }
 
                 function cell_magic(language) {
                     return `%%${language}`;
@@ -511,35 +511,35 @@
                         close: '__A MARKER THAT WILL NEVER BE MATCHED__',
                         parseDelimiters: false,
                         mode: sqlMode
                     }];
                 }
 
                 function lineMagicExtractor(language) {
-                    return new _krassowski_jupyterlab_lsp__WEBPACK_IMPORTED_MODULE_0__.RegExpForeignCodeExtractor({
+                    return new _jupyter_lsp_jupyterlab_lsp__WEBPACK_IMPORTED_MODULE_0__.RegExpForeignCodeExtractor({
                         language: language,
                         pattern: `${BEGIN}${line_magic(language)}${COMMANDS}([^\n]*)`,
                         foreign_capture_groups: [1],
                         is_standalone: true,
                         file_extension: language
                     });
                 }
 
                 function cellMagicExtractor(language) {
-                    return new _krassowski_jupyterlab_lsp__WEBPACK_IMPORTED_MODULE_0__.RegExpForeignCodeExtractor({
+                    return new _jupyter_lsp_jupyterlab_lsp__WEBPACK_IMPORTED_MODULE_0__.RegExpForeignCodeExtractor({
                         language: language,
                         pattern: `${BEGIN}${cell_magic(language)}${COMMANDS}\n([^]*)`,
                         foreign_capture_groups: [1],
                         is_standalone: true,
                         file_extension: language
                     });
                 }
 
                 function markerExtractor(language) {
-                    return new _krassowski_jupyterlab_lsp__WEBPACK_IMPORTED_MODULE_0__.RegExpForeignCodeExtractor({
+                    return new _jupyter_lsp_jupyterlab_lsp__WEBPACK_IMPORTED_MODULE_0__.RegExpForeignCodeExtractor({
                         language: language,
                         pattern: `${start(language)}.*?\n([^]*?)${end(language)}`,
                         foreign_capture_groups: [1],
                         is_standalone: true,
                         file_extension: language
                     });
                 }
@@ -564,8 +564,8 @@
 
 
                 /***/
             })
 
     }
 ]);
-//# sourceMappingURL=lib_index_js.67b6c3715f795c58c5d6.js.map
+//# sourceMappingURL=lib_index_js.4c0329159cbdd7702e52.js.map
```

### Comparing `jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/labextension/static/lib_index_js.67b6c3715f795c58c5d6.js.map` & `jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/labextension/static/lib_index_js.4c0329159cbdd7702e52.js.map`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7959183673469388%*

 * *Differences: {"'file'": "'lib_index_js.4c0329159cbdd7702e52.js'",*

 * * "'mappings'": "';;;;;;;;;;;;;AAAO,IAAU,SAAS,CAMzB;AAND,WAAiB,SAAS;IACX,2BAAiB,GAAG,uBAAuB,CAAC;IAC5C,wBAAc,GAAG,GAAG,2BAAiB,cAAc,CAAC;IACpD,iCAAuB,GAAG,GAAG,2BAAiB,kBAAkB,CAAC;IACjE,0BAAgB,GAAG,GAAG,2BAAiB,EAAE,CAAC;IAC1C,0BAAgB,GAAG,GAAG,0BAAgB,SAAS,CAAC;AAC/D,CAAC,EANgB,SAAS,KAAT,SAAS,QAMzB;;;;;;;;;;;;;;;;;;;;;;ACHuD;AACjB;AAEC;AAEsB;AAIvD,MAAM,YAAY;IAKvB,YACE,cAAsB,EACtB,aAAsB,EACtB,iBAA8B;QAE9B,IAAI,CAAC,cAAc,GAAG,cAAc,CAAC;QACrC,IAAI,CAAC,aAAa,GAAG, […]*

```diff
@@ -1,19 +1,19 @@
 {
-    "file": "lib_index_js.67b6c3715f795c58c5d6.js",
-    "mappings": "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",
+    "file": "lib_index_js.4c0329159cbdd7702e52.js",
+    "mappings": "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",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://jupyterlab-sql-editor/./src/constants.ts",
         "webpack://jupyterlab-sql-editor/./src/formatter.ts",
         "webpack://jupyterlab-sql-editor/./src/index.ts",
         "webpack://jupyterlab-sql-editor/./src/utils.ts"
     ],
     "sourcesContent": [
         "export namespace Constants {\n  export const SHORT_PLUGIN_NAME = 'jupyterlab-sql-editor';\n  export const FORMAT_COMMAND = `${SHORT_PLUGIN_NAME}:format_cell`;\n  export const FORMAT_COMMAND_DOCUMENT = `${SHORT_PLUGIN_NAME}:format_document`;\n  export const LONG_PLUGIN_NAME = `${SHORT_PLUGIN_NAME}`;\n  export const SETTINGS_SECTION = `${LONG_PLUGIN_NAME}:plugin`;\n}\n",
-        "import { Cell, CodeCell } from '@jupyterlab/cells';\nimport { INotebookTracker, Notebook } from '@jupyterlab/notebook';\nimport { IEditorTracker } from '@jupyterlab/fileeditor';\nimport { showErrorMessage } from '@jupyterlab/apputils';\nimport { format } from 'sql-formatter';\nimport { RegExpForeignCodeExtractor } from '@krassowski/jupyterlab-lsp';\nimport { Constants } from './constants';\nimport { JupyterFrontEnd } from '@jupyterlab/application';\nimport { cellMagicExtractor, markerExtractor } from './utils';\nimport { ICodeMirror } from '@jupyterlab/codemirror';\nimport { KeywordCase } from 'sql-formatter';\n\nexport class SqlFormatter {\n  private formatTabWidth: number;\n  private formatUseTabs: boolean;\n  private formatKeywordCase: KeywordCase;\n\n  constructor(\n    formatTabWidth: number,\n    formatUseTabs: boolean,\n    formatKeywordCase: KeywordCase\n  ) {\n    this.formatTabWidth = formatTabWidth;\n    this.formatUseTabs = formatUseTabs;\n    this.formatKeywordCase = formatKeywordCase;\n  }\n\n  format(text: string | null): string {\n    const formatted = format(text || '', {\n      language: 'spark', // Defaults to \"sql\" (see the above list of supported dialects)\n      tabWidth: this.formatTabWidth, // Defaults to two spaces. Ignored if useTabs is true\n      useTabs: this.formatUseTabs, // Defaults to false\n      keywordCase: this.formatKeywordCase, // Defaults to false (not safe to use when SQL dialect has case-sensitive identifiers)\n      linesBetweenQueries: 2 // Defaults to 1\n    });\n    return formatted;\n  }\n}\n\nclass JupyterlabNotebookCodeFormatter {\n  private notebookTracker: INotebookTracker;\n  private working: boolean;\n  private extractors: RegExpForeignCodeExtractor[];\n  private codeMirror: ICodeMirror;\n  private sqlFormatter: SqlFormatter;\n  constructor(\n    notebookTracker: INotebookTracker,\n    codeMirror: ICodeMirror,\n    sqlFormatter: SqlFormatter\n  ) {\n    this.working = false;\n    this.notebookTracker = notebookTracker;\n    this.extractors = [];\n    this.extractors.push(cellMagicExtractor('sparksql'));\n    this.extractors.push(cellMagicExtractor('trino'));\n    this.extractors.push(markerExtractor('sparksql'));\n    this.extractors.push(markerExtractor('trino'));\n    this.codeMirror = codeMirror;\n    this.sqlFormatter = sqlFormatter;\n  }\n\n  setFormatter(sqlFormatter: SqlFormatter) {\n    this.sqlFormatter = sqlFormatter;\n  }\n\n  public async formatAction() {\n    return this.formatCells(true);\n  }\n\n  public async formatSelectedCodeCells(notebook?: Notebook) {\n    return this.formatCells(true, notebook);\n  }\n\n  private getCodeCells(selectedOnly = true, notebook?: Notebook): CodeCell[] {\n    if (!this.notebookTracker.currentWidget) {\n      return [];\n    }\n    const codeCells: CodeCell[] = [];\n    notebook = notebook || this.notebookTracker.currentWidget.content;\n    notebook.widgets.forEach((cell: Cell) => {\n      if (cell.model.type === 'code') {\n        if (!selectedOnly || notebook?.isSelectedOrActive(cell)) {\n          codeCells.push(cell as CodeCell);\n        }\n      }\n    });\n    return codeCells;\n  }\n\n  private tryReplacing(\n    cellText: string,\n    extractor: RegExpForeignCodeExtractor\n  ): string | null {\n    const extracted = extractor.extract_foreign_code(cellText);\n    if (\n      extracted &&\n      extracted.length > 0 &&\n      extracted[0].foreign_code &&\n      extracted[0].range\n    ) {\n      const sqlText = extracted[0].foreign_code;\n      const formattedSql = this.sqlFormatter.format(sqlText) + '\\n';\n      const doc = new this.codeMirror.CodeMirror.Doc(cellText, 'sql', 0, '\\n');\n      const startPos = new this.codeMirror.CodeMirror.Pos(\n        extracted[0].range.start.line,\n        extracted[0].range.start.column\n      );\n      const endPos = new this.codeMirror.CodeMirror.Pos(\n        extracted[0].range.end.line,\n        extracted[0].range.end.column\n      );\n      doc.replaceRange(formattedSql, startPos, endPos);\n      return doc.getValue();\n    }\n    return null;\n  }\n\n  private async formatCells(selectedOnly: boolean, notebook?: Notebook) {\n    if (this.working || !this.applicable()) {\n      return;\n    }\n    try {\n      this.working = true;\n      const selectedCells = this.getCodeCells(selectedOnly, notebook);\n      if (selectedCells.length > 0) {\n        const currentTexts = selectedCells.map(cell => cell.model.value.text);\n        const formattedTexts = currentTexts.map(cellText => {\n          const formatted = this.extractors\n            .map(extractor => this.tryReplacing(cellText, extractor))\n            .find(formatted => formatted);\n          return formatted || '';\n        });\n        for (let i = 0; i < selectedCells.length; ++i) {\n          const cell = selectedCells[i];\n          const currentText = currentTexts[i];\n          const formattedText = formattedTexts[i];\n          if (cell.model.value.text === currentText) {\n            cell.model.value.text = formattedText;\n          }\n        }\n      }\n    } catch (error) {\n      await showErrorMessage('Jupyterlab Code Formatter Error', error);\n    } finally {\n      this.working = false;\n    }\n  }\n\n  applicable() {\n    const selectedCells = this.getCodeCells();\n    if (selectedCells.length > 0) {\n      const currentTexts = selectedCells.map(cell => cell.model.value.text);\n      let numSqlCells = 0;\n      currentTexts.forEach(cellText => {\n        const found = this.extractors.find(extractor =>\n          extractor.has_foreign_code(cellText)\n        );\n        if (found) {\n          numSqlCells++;\n        }\n      });\n      // eslint-disable-next-line eqeqeq\n      return numSqlCells == selectedCells.length;\n    }\n    return false;\n  }\n}\n\nclass JupyterlabFileEditorCodeFormatter {\n  private editorTracker: IEditorTracker;\n  private working: boolean;\n  private sqlFormatter: SqlFormatter;\n  constructor(editorTracker: IEditorTracker, sqlFormatter: SqlFormatter) {\n    this.working = false;\n    this.editorTracker = editorTracker;\n    this.sqlFormatter = sqlFormatter;\n  }\n\n  setFormatter(sqlFormatter: SqlFormatter) {\n    this.sqlFormatter = sqlFormatter;\n  }\n\n  formatAction() {\n    if (this.working) {\n      return;\n    }\n    const editorWidget = this.editorTracker.currentWidget;\n    if (editorWidget) {\n      try {\n        this.working = true;\n        const editor = editorWidget.content.editor;\n        const code = editor?.model.value.text;\n        const formatted = this.sqlFormatter.format(code);\n        editorWidget.content.editor.model.value.text = formatted;\n      } finally {\n        this.working = false;\n      }\n    }\n  }\n}\n\nexport class JupyterLabCodeFormatter {\n  private app: JupyterFrontEnd;\n  private tracker: INotebookTracker;\n  private editorTracker: IEditorTracker;\n  private notebookCodeFormatter: JupyterlabNotebookCodeFormatter;\n  private fileEditorCodeFormatter: JupyterlabFileEditorCodeFormatter;\n  constructor(\n    app: JupyterFrontEnd,\n    tracker: INotebookTracker,\n    editorTracker: IEditorTracker,\n    codeMirror: ICodeMirror,\n    sqlFormatter: SqlFormatter\n  ) {\n    this.app = app;\n    this.tracker = tracker;\n    this.editorTracker = editorTracker;\n    this.notebookCodeFormatter = new JupyterlabNotebookCodeFormatter(\n      this.tracker,\n      codeMirror,\n      sqlFormatter\n    );\n    this.fileEditorCodeFormatter = new JupyterlabFileEditorCodeFormatter(\n      this.editorTracker,\n      sqlFormatter\n    );\n    this.setupCommands();\n    this.setupContextMenu();\n  }\n\n  setFormatter(sqlFormatter: SqlFormatter) {\n    this.notebookCodeFormatter.setFormatter(sqlFormatter);\n    this.fileEditorCodeFormatter.setFormatter(sqlFormatter);\n  }\n\n  private setupContextMenu() {\n    this.app.contextMenu.addItem({\n      command: Constants.FORMAT_COMMAND,\n      selector: '.jp-CodeCell'\n    });\n    this.app.contextMenu.addItem({\n      command: Constants.FORMAT_COMMAND_DOCUMENT,\n      selector: '.jp-FileEditor'\n    });\n  }\n\n  private setupCommands() {\n    this.app.commands.addCommand(Constants.FORMAT_COMMAND, {\n      execute: async () => {\n        await this.notebookCodeFormatter.formatSelectedCodeCells();\n      },\n      isVisible: () => {\n        return this.notebookCodeFormatter.applicable();\n      },\n      label: 'Format Sql Cell'\n    });\n    this.app.commands.addCommand(Constants.FORMAT_COMMAND_DOCUMENT, {\n      execute: async () => {\n        await this.fileEditorCodeFormatter.formatAction();\n      },\n      label: 'Format Sql Document'\n    });\n  }\n}\n",
-        "import {\n  JupyterFrontEnd,\n  JupyterFrontEndPlugin\n} from '@jupyterlab/application';\nimport { ISettingRegistry } from '@jupyterlab/settingregistry';\nimport { ILSPCodeExtractorsManager } from '@krassowski/jupyterlab-lsp';\nimport { ICodeMirror } from '@jupyterlab/codemirror'\nimport { INotebookTracker } from '@jupyterlab/notebook';\nimport { IEditorTracker } from '@jupyterlab/fileeditor';\nimport {\n  JupyterLabCodeFormatter as SqlCodeFormatter,\n  SqlFormatter\n} from './formatter';\nimport {\n  cellMagicExtractor,\n  markerExtractor,\n  lineMagicExtractor,\n  sqlCodeMirrorModesFor,\n  registerCodeMirrorFor\n} from './utils';\nimport { Constants } from './constants';\nimport { KeywordCase } from 'sql-formatter';\n\n/*\nResults in\n\nLINE_MAGIC_EXTRACT\n(?:^|\\n)%sparksql(?: |-c|--cache|-e|--eager|-[a-z] [0-9a-zA-Z/._]+|--[a-zA-Z]+ [0-9a-zA-Z/._]+)*([^\\n]*)\n\nCELL_MAGIC_EXTRACT\n(?:^|\\n)%%sparksql(?: |-c|--cache|-e|--eager|-[a-z] [0-9a-zA-Z/._]+|--[a-zA-Z]+ [0-9a-zA-Z/._]+)*\\n([^]*)\n*/\n\n/**\n * Code taken from https://github.com/jupyterlab/jupyterlab/blob/master/packages/codemirror/src/codemirror-ipython.ts\n * Modified to support embedded sql syntax\n */\nfunction codeMirrorWithSqlSyntaxHighlightSupport(c: ICodeMirror) {\n  /**\n   * Define an IPython codemirror mode.\n   *\n   * It is a slightly altered Python Mode with a `?` operator.\n   */\n  c.CodeMirror.defineMode(\n    'ipython',\n    (config: CodeMirror.EditorConfiguration, modeOptions?: any) => {\n      const pythonConf: any = {};\n      for (const prop in modeOptions) {\n        if (modeOptions.hasOwnProperty(prop)) {\n          pythonConf[prop] = modeOptions[prop];\n        }\n      }\n      pythonConf.name = 'python';\n      pythonConf.singleOperators = new RegExp('^[\\\\+\\\\-\\\\*/%&|@\\\\^~<>!\\\\?]');\n      pythonConf.identifiers = new RegExp(\n        '^[_A-Za-z\\u00A1-\\uFFFF][_A-Za-z0-9\\u00A1-\\uFFFF]*'\n      );\n      //return c.CodeMirror.getMode(config, pythonConf);\n\n      // Instead of returning this mode we multiplex it with SQL\n      const pythonMode = c.CodeMirror.getMode(config, pythonConf);\n\n      // get a mode for SQL\n      const sqlMode = c.CodeMirror.getMode(config, 'sql');\n\n      // multiplex python with SQL and return it\n      const multiplexedModes = sqlCodeMirrorModesFor(\n        'sparksql',\n        sqlMode\n      ).concat(sqlCodeMirrorModesFor('trino', sqlMode));\n\n      return c.CodeMirror.multiplexingMode(pythonMode, ...multiplexedModes);\n    }\n    // Original code has a third argument. Not sure why we don't..\n    // https://github.com/jupyterlab/jupyterlab/blob/master/packages/codemirror/src/codemirror-ipython.ts\n    // ,\n    // 'python'\n  );\n\n  registerCodeMirrorFor(c, 'sparksql');\n  registerCodeMirrorFor(c, 'trino');\n\n  // The following is already done by default implementation so not redoing here\n  // c.CodeMirror.defineMIME('text/x-ipython', 'ipython');\n  // c.CodeMirror.modeInfo.push({\n  //   ext: [],\n  //   mime: 'text/x-ipython',\n  //   mode: 'ipython',\n  //   name: 'ipython'\n  // });\n}\n\n/**\n * Initialization data for the jupyterlab_jc extension.\n */\nconst plugin: JupyterFrontEndPlugin<void> = {\n  id: 'jupyterlab-sql-editor:plugin',\n  autoStart: true,\n  optional: [],\n  requires: [\n    ICodeMirror,\n    ILSPCodeExtractorsManager,\n    ISettingRegistry,\n    IEditorTracker,\n    INotebookTracker\n  ],\n  activate: (\n    app: JupyterFrontEnd,\n    codeMirror: ICodeMirror,\n    lspExtractorsMgr: ILSPCodeExtractorsManager,\n    settingRegistry: ISettingRegistry,\n    editorTracker: IEditorTracker,\n    tracker: INotebookTracker\n  ) => {\n    console.log('JupyterLab extension jupyterlab-sql-editor is activated!');\n\n    const sqlFormatter = new SqlFormatter(4, false, 'upper');\n    const sqlCodeFormatter = new SqlCodeFormatter(\n      app,\n      tracker,\n      editorTracker,\n      codeMirror,\n      sqlFormatter\n    );\n    console.log('jupyterlab-sql-editor SQL code formatter registered');\n\n    /**\n     * Load the settings for this extension\n     *\n     * @param setting Extension settings\n     */\n    function loadSetting(settings: ISettingRegistry.ISettings): void {\n      // Read the settings and convert to the correct type\n      const formatTabwidth = settings.get('formatTabWidth').composite as number;\n      const formatUseTabs = settings.get('formatUseTabs').composite as boolean;\n      const formatKeywordCase = settings.get('formatKeywordCase')\n        .composite as KeywordCase;\n      const sqlFormatter = new SqlFormatter(\n        formatTabwidth,\n        formatUseTabs,\n        formatKeywordCase\n      );\n      sqlCodeFormatter.setFormatter(sqlFormatter);\n    }\n\n    // Wait for the application to be restored and\n    // for the settings for this plugin to be loaded\n    Promise.all([\n      app.restored,\n      settingRegistry.load(Constants.SETTINGS_SECTION)\n    ])\n      .then(([, settings]) => {\n        // Read the settings\n        loadSetting(settings);\n        // Listen for your plugin setting changes using Signal\n        settings.changed.connect(loadSetting);\n      })\n      .catch(reason => {\n        console.error(\n          `Something went wrong when reading the settings.\\n${reason}`\n        );\n      });\n\n    // JupyterLab uses the CodeMirror library to syntax highlight code\n    // within the cells. Register a multiplex CodeMirror capable of\n    // highlightin SQL which is embedded in a IPython magic or within\n    // a python string (delimited by markers)\n    codeMirrorWithSqlSyntaxHighlightSupport(codeMirror);\n    console.log(\n      'jupyterlab-sql-editor code mirror for syntax highlighting registered'\n    );\n\n    // JupyterLab-LSP relies on extractors to pull the SQL out of the cell\n    // and into a virtual document which is then passed to the sql-language-server\n    // for code completion evaluation\n    lspExtractorsMgr.register(markerExtractor('sparksql'), 'python');\n    lspExtractorsMgr.register(lineMagicExtractor('sparksql'), 'python');\n    lspExtractorsMgr.register(cellMagicExtractor('sparksql'), 'python');\n    lspExtractorsMgr.register(markerExtractor('trino'), 'python');\n    lspExtractorsMgr.register(lineMagicExtractor('trino'), 'python');\n    lspExtractorsMgr.register(cellMagicExtractor('trino'), 'python');\n    console.log('jupyterlab-sql-editor LSP extractors registered');\n  }\n};\n\nexport default plugin;\n",
-        "import { RegExpForeignCodeExtractor } from '@krassowski/jupyterlab-lsp';\nimport { Mode } from 'codemirror';\nimport { ICodeMirror } from '@jupyterlab/codemirror';\n\nfunction line_magic(language: string) {\n  return `%${language}`;\n}\nfunction cell_magic(language: string) {\n  return `%%${language}`;\n}\nfunction start(language: string) {\n  return `--start-${language}`;\n}\nfunction end(language: string) {\n  return `--end-${language}`;\n}\n\n// sparksql magic accepts options in the long form\n// --dataframe df\n// or in the short form\n// -d df\n// some options do not require any values, they act more as a flag\nconst FLAG_OPTS = [\n    '-c', '--cache', //          Cache dataframe\n    '-e', '--eager',  //          Cache dataframe with eager load\n    '-s', '--show-nonprinting',\n    '-x', '--raw',\n    '-j', '--jinja',\n    '-b', '--dbt',\n].join('|')\nconst SPACE = ' ';\nconst OPTION_VALUE = `[0-9a-zA-Z/\\._]+`;\nconst SHORT_OPTS = `-[a-z] ${OPTION_VALUE}`;\nconst LONG_OPTS = `--[_a-zA-Z]+ ${OPTION_VALUE}`;\nconst COMMANDS = `(?:${SPACE}|${FLAG_OPTS}|${SHORT_OPTS}|${LONG_OPTS})*`;\nconst BEGIN = `(?:^|\\n)`;\n\nexport function sqlCodeMirrorModesFor(\n  language: string,\n  sqlMode: Mode<unknown>\n) {\n  return [\n    {\n      open: `${start(language)}`,\n      close: `${end(language)}`,\n      // parseDelimiters is set to true which considers\n      // the marker as part of the SQL statement\n      // it is thus syntax highlighted as a comment\n      parseDelimiters: true,\n      mode: sqlMode\n    },\n    {\n      open: RegExp(`${line_magic(language)}${COMMANDS}`) as unknown as string,\n      close: '\\n', // Line magic: Stop at end of line (blank line)\n      parseDelimiters: false,\n      mode: sqlMode\n    },\n    {\n      open: RegExp(`${cell_magic(language)}${COMMANDS}`) as unknown as string,\n      close: '__A MARKER THAT WILL NEVER BE MATCHED__', // Cell magic: capture chars till the end of the cell\n      parseDelimiters: false,\n      mode: sqlMode\n    }\n  ];\n}\n\nexport function lineMagicExtractor(\n  language: string\n): RegExpForeignCodeExtractor {\n  return new RegExpForeignCodeExtractor({\n    language: language,\n    pattern: `${BEGIN}${line_magic(language)}${COMMANDS}([^\\n]*)`,\n    foreign_capture_groups: [1],\n    is_standalone: true,\n    file_extension: language\n  });\n}\n\nexport function cellMagicExtractor(\n  language: string\n): RegExpForeignCodeExtractor {\n  return new RegExpForeignCodeExtractor({\n    language: language,\n    pattern: `${BEGIN}${cell_magic(language)}${COMMANDS}\\n([^]*)`,\n    foreign_capture_groups: [1],\n    is_standalone: true,\n    file_extension: language\n  });\n}\n\nexport function markerExtractor(language: string): RegExpForeignCodeExtractor {\n  return new RegExpForeignCodeExtractor({\n    language: language,\n    pattern: `${start(language)}.*?\\n([^]*?)${end(language)}`,\n    foreign_capture_groups: [1],\n    is_standalone: true,\n    file_extension: language\n  });\n}\n\n/**\n * Register text editor based on file type.\n * @param c\n * @param language\n */\nexport function registerCodeMirrorFor(c: ICodeMirror, language: string) {\n  c.CodeMirror.defineMode(\n    language,\n    (config: CodeMirror.EditorConfiguration, modeOptions?: any) => {\n      const mode = c.CodeMirror.getMode(config, 'sql');\n      return mode;\n    }\n  );\n  c.CodeMirror.defineMIME(`text/x-${language}`, language);\n  c.CodeMirror.modeInfo.push({\n    ext: [language],\n    mime: `text/x-${language}`,\n    mode: language,\n    name: language\n  });\n}\n"
+        "import { Cell, CodeCell } from '@jupyterlab/cells';\nimport { INotebookTracker, Notebook } from '@jupyterlab/notebook';\nimport { IEditorTracker } from '@jupyterlab/fileeditor';\nimport { showErrorMessage } from '@jupyterlab/apputils';\nimport { format } from 'sql-formatter';\nimport { RegExpForeignCodeExtractor } from '@jupyter-lsp/jupyterlab-lsp';\nimport { Constants } from './constants';\nimport { JupyterFrontEnd } from '@jupyterlab/application';\nimport { cellMagicExtractor, markerExtractor } from './utils';\nimport { ICodeMirror } from '@jupyterlab/codemirror';\nimport { KeywordCase } from 'sql-formatter';\n\nexport class SqlFormatter {\n  private formatTabWidth: number;\n  private formatUseTabs: boolean;\n  private formatKeywordCase: KeywordCase;\n\n  constructor(\n    formatTabWidth: number,\n    formatUseTabs: boolean,\n    formatKeywordCase: KeywordCase\n  ) {\n    this.formatTabWidth = formatTabWidth;\n    this.formatUseTabs = formatUseTabs;\n    this.formatKeywordCase = formatKeywordCase;\n  }\n\n  format(text: string | null): string {\n    const formatted = format(text || '', {\n      language: 'spark', // Defaults to \"sql\" (see the above list of supported dialects)\n      tabWidth: this.formatTabWidth, // Defaults to two spaces. Ignored if useTabs is true\n      useTabs: this.formatUseTabs, // Defaults to false\n      keywordCase: this.formatKeywordCase, // Defaults to false (not safe to use when SQL dialect has case-sensitive identifiers)\n      linesBetweenQueries: 2 // Defaults to 1\n    });\n    return formatted;\n  }\n}\n\nclass JupyterlabNotebookCodeFormatter {\n  private notebookTracker: INotebookTracker;\n  private working: boolean;\n  private extractors: RegExpForeignCodeExtractor[];\n  private codeMirror: ICodeMirror;\n  private sqlFormatter: SqlFormatter;\n  constructor(\n    notebookTracker: INotebookTracker,\n    codeMirror: ICodeMirror,\n    sqlFormatter: SqlFormatter\n  ) {\n    this.working = false;\n    this.notebookTracker = notebookTracker;\n    this.extractors = [];\n    this.extractors.push(cellMagicExtractor('sparksql'));\n    this.extractors.push(cellMagicExtractor('trino'));\n    this.extractors.push(markerExtractor('sparksql'));\n    this.extractors.push(markerExtractor('trino'));\n    this.codeMirror = codeMirror;\n    this.sqlFormatter = sqlFormatter;\n  }\n\n  setFormatter(sqlFormatter: SqlFormatter) {\n    this.sqlFormatter = sqlFormatter;\n  }\n\n  public async formatAction() {\n    return this.formatCells(true);\n  }\n\n  public async formatSelectedCodeCells(notebook?: Notebook) {\n    return this.formatCells(true, notebook);\n  }\n\n  private getCodeCells(selectedOnly = true, notebook?: Notebook): CodeCell[] {\n    if (!this.notebookTracker.currentWidget) {\n      return [];\n    }\n    const codeCells: CodeCell[] = [];\n    notebook = notebook || this.notebookTracker.currentWidget.content;\n    notebook.widgets.forEach((cell: Cell) => {\n      if (cell.model.type === 'code') {\n        if (!selectedOnly || notebook?.isSelectedOrActive(cell)) {\n          codeCells.push(cell as CodeCell);\n        }\n      }\n    });\n    return codeCells;\n  }\n\n  private tryReplacing(\n    cellText: string,\n    extractor: RegExpForeignCodeExtractor\n  ): string | null {\n    const extracted = extractor.extract_foreign_code(cellText);\n    if (\n      extracted &&\n      extracted.length > 0 &&\n      extracted[0].foreign_code &&\n      extracted[0].range\n    ) {\n      const sqlText = extracted[0].foreign_code;\n      const formattedSql = this.sqlFormatter.format(sqlText) + '\\n';\n      const doc = new this.codeMirror.CodeMirror.Doc(cellText, 'sql', 0, '\\n');\n      const startPos = new this.codeMirror.CodeMirror.Pos(\n        extracted[0].range.start.line,\n        extracted[0].range.start.column\n      );\n      const endPos = new this.codeMirror.CodeMirror.Pos(\n        extracted[0].range.end.line,\n        extracted[0].range.end.column\n      );\n      doc.replaceRange(formattedSql, startPos, endPos);\n      return doc.getValue();\n    }\n    return null;\n  }\n\n  private async formatCells(selectedOnly: boolean, notebook?: Notebook) {\n    if (this.working || !this.applicable()) {\n      return;\n    }\n    try {\n      this.working = true;\n      const selectedCells = this.getCodeCells(selectedOnly, notebook);\n      if (selectedCells.length > 0) {\n        const currentTexts = selectedCells.map(cell => cell.model.value.text);\n        const formattedTexts = currentTexts.map(cellText => {\n          const formatted = this.extractors\n            .map(extractor => this.tryReplacing(cellText, extractor))\n            .find(formatted => formatted);\n          return formatted || '';\n        });\n        for (let i = 0; i < selectedCells.length; ++i) {\n          const cell = selectedCells[i];\n          const currentText = currentTexts[i];\n          const formattedText = formattedTexts[i];\n          if (cell.model.value.text === currentText) {\n            cell.model.value.text = formattedText;\n          }\n        }\n      }\n    } catch (error) {\n      await showErrorMessage('Jupyterlab Code Formatter Error', error);\n    } finally {\n      this.working = false;\n    }\n  }\n\n  applicable() {\n    const selectedCells = this.getCodeCells();\n    if (selectedCells.length > 0) {\n      const currentTexts = selectedCells.map(cell => cell.model.value.text);\n      let numSqlCells = 0;\n      currentTexts.forEach(cellText => {\n        const found = this.extractors.find(extractor =>\n          extractor.has_foreign_code(cellText)\n        );\n        if (found) {\n          numSqlCells++;\n        }\n      });\n      // eslint-disable-next-line eqeqeq\n      return numSqlCells == selectedCells.length;\n    }\n    return false;\n  }\n}\n\nclass JupyterlabFileEditorCodeFormatter {\n  private editorTracker: IEditorTracker;\n  private working: boolean;\n  private sqlFormatter: SqlFormatter;\n  constructor(editorTracker: IEditorTracker, sqlFormatter: SqlFormatter) {\n    this.working = false;\n    this.editorTracker = editorTracker;\n    this.sqlFormatter = sqlFormatter;\n  }\n\n  setFormatter(sqlFormatter: SqlFormatter) {\n    this.sqlFormatter = sqlFormatter;\n  }\n\n  formatAction() {\n    if (this.working) {\n      return;\n    }\n    const editorWidget = this.editorTracker.currentWidget;\n    if (editorWidget) {\n      try {\n        this.working = true;\n        const editor = editorWidget.content.editor;\n        const code = editor?.model.value.text;\n        const formatted = this.sqlFormatter.format(code);\n        editorWidget.content.editor.model.value.text = formatted;\n      } finally {\n        this.working = false;\n      }\n    }\n  }\n}\n\nexport class JupyterLabCodeFormatter {\n  private app: JupyterFrontEnd;\n  private tracker: INotebookTracker;\n  private editorTracker: IEditorTracker;\n  private notebookCodeFormatter: JupyterlabNotebookCodeFormatter;\n  private fileEditorCodeFormatter: JupyterlabFileEditorCodeFormatter;\n  constructor(\n    app: JupyterFrontEnd,\n    tracker: INotebookTracker,\n    editorTracker: IEditorTracker,\n    codeMirror: ICodeMirror,\n    sqlFormatter: SqlFormatter\n  ) {\n    this.app = app;\n    this.tracker = tracker;\n    this.editorTracker = editorTracker;\n    this.notebookCodeFormatter = new JupyterlabNotebookCodeFormatter(\n      this.tracker,\n      codeMirror,\n      sqlFormatter\n    );\n    this.fileEditorCodeFormatter = new JupyterlabFileEditorCodeFormatter(\n      this.editorTracker,\n      sqlFormatter\n    );\n    this.setupCommands();\n    this.setupContextMenu();\n  }\n\n  setFormatter(sqlFormatter: SqlFormatter) {\n    this.notebookCodeFormatter.setFormatter(sqlFormatter);\n    this.fileEditorCodeFormatter.setFormatter(sqlFormatter);\n  }\n\n  private setupContextMenu() {\n    this.app.contextMenu.addItem({\n      command: Constants.FORMAT_COMMAND,\n      selector: '.jp-CodeCell'\n    });\n    this.app.contextMenu.addItem({\n      command: Constants.FORMAT_COMMAND_DOCUMENT,\n      selector: '.jp-FileEditor'\n    });\n  }\n\n  private setupCommands() {\n    this.app.commands.addCommand(Constants.FORMAT_COMMAND, {\n      execute: async () => {\n        await this.notebookCodeFormatter.formatSelectedCodeCells();\n      },\n      isVisible: () => {\n        return this.notebookCodeFormatter.applicable();\n      },\n      label: 'Format Sql Cell'\n    });\n    this.app.commands.addCommand(Constants.FORMAT_COMMAND_DOCUMENT, {\n      execute: async () => {\n        await this.fileEditorCodeFormatter.formatAction();\n      },\n      label: 'Format Sql Document'\n    });\n  }\n}\n",
+        "import {\n  JupyterFrontEnd,\n  JupyterFrontEndPlugin\n} from '@jupyterlab/application';\nimport { ISettingRegistry } from '@jupyterlab/settingregistry';\nimport { ILSPCodeExtractorsManager } from '@jupyter-lsp/jupyterlab-lsp';\nimport { ICodeMirror } from '@jupyterlab/codemirror'\nimport { INotebookTracker } from '@jupyterlab/notebook';\nimport { IEditorTracker } from '@jupyterlab/fileeditor';\nimport {\n  JupyterLabCodeFormatter as SqlCodeFormatter,\n  SqlFormatter\n} from './formatter';\nimport {\n  cellMagicExtractor,\n  markerExtractor,\n  lineMagicExtractor,\n  sqlCodeMirrorModesFor,\n  registerCodeMirrorFor\n} from './utils';\nimport { Constants } from './constants';\nimport { KeywordCase } from 'sql-formatter';\n\n/*\nResults in\n\nLINE_MAGIC_EXTRACT\n(?:^|\\n)%sparksql(?: |-c|--cache|-e|--eager|-[a-z] [0-9a-zA-Z/._]+|--[a-zA-Z]+ [0-9a-zA-Z/._]+)*([^\\n]*)\n\nCELL_MAGIC_EXTRACT\n(?:^|\\n)%%sparksql(?: |-c|--cache|-e|--eager|-[a-z] [0-9a-zA-Z/._]+|--[a-zA-Z]+ [0-9a-zA-Z/._]+)*\\n([^]*)\n*/\n\n/**\n * Code taken from https://github.com/jupyterlab/jupyterlab/blob/master/packages/codemirror/src/codemirror-ipython.ts\n * Modified to support embedded sql syntax\n */\nfunction codeMirrorWithSqlSyntaxHighlightSupport(c: ICodeMirror) {\n  /**\n   * Define an IPython codemirror mode.\n   *\n   * It is a slightly altered Python Mode with a `?` operator.\n   */\n  c.CodeMirror.defineMode(\n    'ipython',\n    (config: CodeMirror.EditorConfiguration, modeOptions?: any) => {\n      const pythonConf: any = {};\n      for (const prop in modeOptions) {\n        if (modeOptions.hasOwnProperty(prop)) {\n          pythonConf[prop] = modeOptions[prop];\n        }\n      }\n      pythonConf.name = 'python';\n      pythonConf.singleOperators = new RegExp('^[\\\\+\\\\-\\\\*/%&|@\\\\^~<>!\\\\?]');\n      pythonConf.identifiers = new RegExp(\n        '^[_A-Za-z\\u00A1-\\uFFFF][_A-Za-z0-9\\u00A1-\\uFFFF]*'\n      );\n      //return c.CodeMirror.getMode(config, pythonConf);\n\n      // Instead of returning this mode we multiplex it with SQL\n      const pythonMode = c.CodeMirror.getMode(config, pythonConf);\n\n      // get a mode for SQL\n      const sqlMode = c.CodeMirror.getMode(config, 'sql');\n\n      // multiplex python with SQL and return it\n      const multiplexedModes = sqlCodeMirrorModesFor(\n        'sparksql',\n        sqlMode\n      ).concat(sqlCodeMirrorModesFor('trino', sqlMode));\n\n      return c.CodeMirror.multiplexingMode(pythonMode, ...multiplexedModes);\n    }\n    // Original code has a third argument. Not sure why we don't..\n    // https://github.com/jupyterlab/jupyterlab/blob/master/packages/codemirror/src/codemirror-ipython.ts\n    // ,\n    // 'python'\n  );\n\n  registerCodeMirrorFor(c, 'sparksql');\n  registerCodeMirrorFor(c, 'trino');\n\n  // The following is already done by default implementation so not redoing here\n  // c.CodeMirror.defineMIME('text/x-ipython', 'ipython');\n  // c.CodeMirror.modeInfo.push({\n  //   ext: [],\n  //   mime: 'text/x-ipython',\n  //   mode: 'ipython',\n  //   name: 'ipython'\n  // });\n}\n\n/**\n * Initialization data for the jupyterlab_jc extension.\n */\nconst plugin: JupyterFrontEndPlugin<void> = {\n  id: 'jupyterlab-sql-editor:plugin',\n  autoStart: true,\n  optional: [],\n  requires: [\n    ICodeMirror,\n    ILSPCodeExtractorsManager,\n    ISettingRegistry,\n    IEditorTracker,\n    INotebookTracker\n  ],\n  activate: (\n    app: JupyterFrontEnd,\n    codeMirror: ICodeMirror,\n    lspExtractorsMgr: ILSPCodeExtractorsManager,\n    settingRegistry: ISettingRegistry,\n    editorTracker: IEditorTracker,\n    tracker: INotebookTracker\n  ) => {\n    console.log('JupyterLab extension jupyterlab-sql-editor is activated!');\n\n    const sqlFormatter = new SqlFormatter(4, false, 'upper');\n    const sqlCodeFormatter = new SqlCodeFormatter(\n      app,\n      tracker,\n      editorTracker,\n      codeMirror,\n      sqlFormatter\n    );\n    console.log('jupyterlab-sql-editor SQL code formatter registered');\n\n    /**\n     * Load the settings for this extension\n     *\n     * @param setting Extension settings\n     */\n    function loadSetting(settings: ISettingRegistry.ISettings): void {\n      // Read the settings and convert to the correct type\n      const formatTabwidth = settings.get('formatTabWidth').composite as number;\n      const formatUseTabs = settings.get('formatUseTabs').composite as boolean;\n      const formatKeywordCase = settings.get('formatKeywordCase')\n        .composite as KeywordCase;\n      const sqlFormatter = new SqlFormatter(\n        formatTabwidth,\n        formatUseTabs,\n        formatKeywordCase\n      );\n      sqlCodeFormatter.setFormatter(sqlFormatter);\n    }\n\n    // Wait for the application to be restored and\n    // for the settings for this plugin to be loaded\n    Promise.all([\n      app.restored,\n      settingRegistry.load(Constants.SETTINGS_SECTION)\n    ])\n      .then(([, settings]) => {\n        // Read the settings\n        loadSetting(settings);\n        // Listen for your plugin setting changes using Signal\n        settings.changed.connect(loadSetting);\n      })\n      .catch(reason => {\n        console.error(\n          `Something went wrong when reading the settings.\\n${reason}`\n        );\n      });\n\n    // JupyterLab uses the CodeMirror library to syntax highlight code\n    // within the cells. Register a multiplex CodeMirror capable of\n    // highlightin SQL which is embedded in a IPython magic or within\n    // a python string (delimited by markers)\n    codeMirrorWithSqlSyntaxHighlightSupport(codeMirror);\n    console.log(\n      'jupyterlab-sql-editor code mirror for syntax highlighting registered'\n    );\n\n    // JupyterLab-LSP relies on extractors to pull the SQL out of the cell\n    // and into a virtual document which is then passed to the sql-language-server\n    // for code completion evaluation\n    lspExtractorsMgr.register(markerExtractor('sparksql'), 'python');\n    lspExtractorsMgr.register(lineMagicExtractor('sparksql'), 'python');\n    lspExtractorsMgr.register(cellMagicExtractor('sparksql'), 'python');\n    lspExtractorsMgr.register(markerExtractor('trino'), 'python');\n    lspExtractorsMgr.register(lineMagicExtractor('trino'), 'python');\n    lspExtractorsMgr.register(cellMagicExtractor('trino'), 'python');\n    console.log('jupyterlab-sql-editor LSP extractors registered');\n  }\n};\n\nexport default plugin;\n",
+        "import { RegExpForeignCodeExtractor } from '@jupyter-lsp/jupyterlab-lsp';\nimport { Mode } from 'codemirror';\nimport { ICodeMirror } from '@jupyterlab/codemirror';\n\nfunction line_magic(language: string) {\n  return `%${language}`;\n}\nfunction cell_magic(language: string) {\n  return `%%${language}`;\n}\nfunction start(language: string) {\n  return `--start-${language}`;\n}\nfunction end(language: string) {\n  return `--end-${language}`;\n}\n\n// sparksql magic accepts options in the long form\n// --dataframe df\n// or in the short form\n// -d df\n// some options do not require any values, they act more as a flag\nconst FLAG_OPTS = [\n    '-c', '--cache', //          Cache dataframe\n    '-e', '--eager',  //          Cache dataframe with eager load\n    '-s', '--show-nonprinting',\n    '-x', '--raw',\n    '-j', '--jinja',\n    '-b', '--dbt',\n].join('|')\nconst SPACE = ' ';\nconst OPTION_VALUE = `[0-9a-zA-Z/\\._]+`;\nconst SHORT_OPTS = `-[a-z] ${OPTION_VALUE}`;\nconst LONG_OPTS = `--[_a-zA-Z]+ ${OPTION_VALUE}`;\nconst COMMANDS = `(?:${SPACE}|${FLAG_OPTS}|${SHORT_OPTS}|${LONG_OPTS})*`;\nconst BEGIN = `(?:^|\\n)`;\n\nexport function sqlCodeMirrorModesFor(\n  language: string,\n  sqlMode: Mode<unknown>\n) {\n  return [\n    {\n      open: `${start(language)}`,\n      close: `${end(language)}`,\n      // parseDelimiters is set to true which considers\n      // the marker as part of the SQL statement\n      // it is thus syntax highlighted as a comment\n      parseDelimiters: true,\n      mode: sqlMode\n    },\n    {\n      open: RegExp(`${line_magic(language)}${COMMANDS}`) as unknown as string,\n      close: '\\n', // Line magic: Stop at end of line (blank line)\n      parseDelimiters: false,\n      mode: sqlMode\n    },\n    {\n      open: RegExp(`${cell_magic(language)}${COMMANDS}`) as unknown as string,\n      close: '__A MARKER THAT WILL NEVER BE MATCHED__', // Cell magic: capture chars till the end of the cell\n      parseDelimiters: false,\n      mode: sqlMode\n    }\n  ];\n}\n\nexport function lineMagicExtractor(\n  language: string\n): RegExpForeignCodeExtractor {\n  return new RegExpForeignCodeExtractor({\n    language: language,\n    pattern: `${BEGIN}${line_magic(language)}${COMMANDS}([^\\n]*)`,\n    foreign_capture_groups: [1],\n    is_standalone: true,\n    file_extension: language\n  });\n}\n\nexport function cellMagicExtractor(\n  language: string\n): RegExpForeignCodeExtractor {\n  return new RegExpForeignCodeExtractor({\n    language: language,\n    pattern: `${BEGIN}${cell_magic(language)}${COMMANDS}\\n([^]*)`,\n    foreign_capture_groups: [1],\n    is_standalone: true,\n    file_extension: language\n  });\n}\n\nexport function markerExtractor(language: string): RegExpForeignCodeExtractor {\n  return new RegExpForeignCodeExtractor({\n    language: language,\n    pattern: `${start(language)}.*?\\n([^]*?)${end(language)}`,\n    foreign_capture_groups: [1],\n    is_standalone: true,\n    file_extension: language\n  });\n}\n\n/**\n * Register text editor based on file type.\n * @param c\n * @param language\n */\nexport function registerCodeMirrorFor(c: ICodeMirror, language: string) {\n  c.CodeMirror.defineMode(\n    language,\n    (config: CodeMirror.EditorConfiguration, modeOptions?: any) => {\n      const mode = c.CodeMirror.getMode(config, 'sql');\n      return mode;\n    }\n  );\n  c.CodeMirror.defineMIME(`text/x-${language}`, language);\n  c.CodeMirror.modeInfo.push({\n    ext: [language],\n    mime: `text/x-${language}`,\n    mode: language,\n    name: language\n  });\n}\n"
     ],
     "version": 3
 }
```

### Comparing `jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/labextension/static/remoteEntry.7a5c41927a28f0d15d2b.js` & `jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/labextension/static/remoteEntry.5141fb70facd63fa9a6c.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -182,15 +182,15 @@
     (() => {
         /******/ // This function allow to reference async chunks
         /******/
         __webpack_require__.u = (chunkId) => {
             /******/ // return url for filenames based on template
             /******/
             return "" + chunkId + "." + {
-                "lib_index_js": "67b6c3715f795c58c5d6",
+                "lib_index_js": "4c0329159cbdd7702e52",
                 "vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1": "8ab7ecce559b1f364311",
                 "style_index_js": "7a9353dfa84524daa532",
                 "vendors-node_modules_sql-formatter_lib_index_js": "1955e937c0ff0f3413ea"
             } [chunkId] + ".js";
             /******/
         };
         /******/
@@ -428,15 +428,15 @@
             /******/
             var promises = [];
             /******/
             switch (name) {
                 /******/
                 case "default": {
                     /******/
-                    register("jupyterlab-sql-editor", "0.1.69-alpha.1", () => (__webpack_require__.e("lib_index_js").then(() => (() => (__webpack_require__( /*! ./lib/index.js */ "./lib/index.js"))))));
+                    register("jupyterlab-sql-editor", "0.1.70", () => (__webpack_require__.e("lib_index_js").then(() => (() => (__webpack_require__( /*! ./lib/index.js */ "./lib/index.js"))))));
                     /******/
                     register("sql-formatter", "6.1.2", () => (__webpack_require__.e("vendors-node_modules_sql-formatter_lib_index_js").then(() => (() => (__webpack_require__( /*! ./node_modules/sql-formatter/lib/index.js */ "./node_modules/sql-formatter/lib/index.js"))))));
                     /******/
                 }
                 /******/
                 break;
                 /******/
@@ -833,15 +833,15 @@
         /******/
         var installedModules = {};
         /******/
         var moduleToHandlerMapping = {
             /******/
             "webpack/sharing/consume/default/@jupyterlab/settingregistry": () => (loadSingletonVersionCheck("default", "@jupyterlab/settingregistry", [1, 3, 6, 1])),
             /******/
-            "webpack/sharing/consume/default/@krassowski/jupyterlab-lsp": () => (loadSingletonVersionCheck("default", "@krassowski/jupyterlab-lsp", [1, 3, 10, 2])),
+            "webpack/sharing/consume/default/@jupyter-lsp/jupyterlab-lsp": () => (loadSingletonVersionCheck("default", "@jupyter-lsp/jupyterlab-lsp", [1, 4, 2, 0])),
             /******/
             "webpack/sharing/consume/default/@jupyterlab/codemirror": () => (loadSingletonVersionCheck("default", "@jupyterlab/codemirror", [1, 3, 6, 1])),
             /******/
             "webpack/sharing/consume/default/@jupyterlab/notebook": () => (loadSingletonVersionCheck("default", "@jupyterlab/notebook", [1, 3, 6, 1])),
             /******/
             "webpack/sharing/consume/default/@jupyterlab/fileeditor": () => (loadSingletonVersionCheck("default", "@jupyterlab/fileeditor", [1, 3, 6, 1])),
             /******/
@@ -854,15 +854,15 @@
         /******/
         var chunkMapping = {
             /******/
             "lib_index_js": [
                 /******/
                 "webpack/sharing/consume/default/@jupyterlab/settingregistry",
                 /******/
-                "webpack/sharing/consume/default/@krassowski/jupyterlab-lsp",
+                "webpack/sharing/consume/default/@jupyter-lsp/jupyterlab-lsp",
                 /******/
                 "webpack/sharing/consume/default/@jupyterlab/codemirror",
                 /******/
                 "webpack/sharing/consume/default/@jupyterlab/notebook",
                 /******/
                 "webpack/sharing/consume/default/@jupyterlab/fileeditor",
                 /******/
@@ -1099,8 +1099,8 @@
     /******/
     var __webpack_exports__ = __webpack_require__("webpack/container/entry/jupyterlab-sql-editor");
     /******/
     (_JUPYTERLAB = typeof _JUPYTERLAB === "undefined" ? {} : _JUPYTERLAB)["jupyterlab-sql-editor"] = __webpack_exports__;
     /******/
     /******/
 })();
-//# sourceMappingURL=remoteEntry.7a5c41927a28f0d15d2b.js.map
+//# sourceMappingURL=remoteEntry.5141fb70facd63fa9a6c.js.map
```

### Comparing `jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/labextension/static/remoteEntry.7a5c41927a28f0d15d2b.js.map` & `jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/labextension/static/remoteEntry.5141fb70facd63fa9a6c.js.map`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9081632653061226%*

 * *Differences: {"'file'": "'remoteEntry.5141fb70facd63fa9a6c.js'",*

 * * "'sourcesContent'": "{insert: [(5, '// This function allow to reference async "*

 * *                     'chunks\\n__webpack_require__.u = (chunkId) => {\\n\\t// return url for '*

 * *                     'filenames based on template\\n\\treturn "" + chunkId + "." + '*

 * *                     '{"lib_index_js":"4c0329159cbdd7702e52","vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1":"8ab7ecce559b1f364311","style_index […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "file": "remoteEntry.7a5c41927a28f0d15d2b.js",
+    "file": "remoteEntry.5141fb70facd63fa9a6c.js",
     "mappings": ";;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCpCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC;WACjF;WACA;WACA;;;;;WCPA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;;;;;WCRA;WACA;WACA;WACA,8BAA8B,qRAAqR;WACnT;;;;;WCJA;WACA;WACA;WACA;WACA,GAAG;WACH;WACA;WACA,CAAC;;;;;WCPD;;;;;WCAA;WACA;WACA;WACA;WACA,uBAAuB,4BAA4B;WACnD;WACA;WACA;WACA,iBAAiB,oBAAoB;WACrC;WACA,mGAAmG,YAAY;WAC/G;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,mEAAmE,iCAAiC;WACpG;WACA;WACA;WACA;;;;;WCxCA;WACA;WACA;WACA,uDAAuD,iBAAiB;WACxE;WACA,gDAAgD,aAAa;WAC7D;;;;;WCNA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,oJAAoJ;WACpJ;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,IAAI,aAAa;WACjB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WC9CA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WClBA;WACA;WACA,WAAW,6BAA6B,iBAAiB,GAAG,qEAAqE;WACjI;WACA;WACA;WACA,qCAAqC,aAAa,EAAE,wDAAwD,2BAA2B,4BAA4B,2BAA2B,+CAA+C,mCAAmC;WAChR;WACA;WACA;WACA,qBAAqB,8BAA8B,SAAS,sDAAsD,gBAAgB,eAAe,KAAK,6DAA6D,SAAS,SAAS,QAAQ,eAAe,KAAK,eAAe,qGAAqG,WAAW,aAAa;WAC7Y;WACA;WACA;WACA,gBAAgB,8BAA8B,qBAAqB,YAAY,sBAAsB,SAAS,iDAAiD,6FAA6F,WAAW,uBAAuB,2BAA2B,wBAAwB,KAAK,oCAAoC,oBAAoB,wBAAwB,oBAAoB,SAAS,KAAK,yBAAyB,KAAK,gCAAgC,yBAAyB,QAAQ,eAAe,KAAK,eAAe,4DAA4D;WACtoB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,CAAC;;WAED;WACA;WACA;WACA,CAAC;WACD;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN,KAAK,WAAW;WAChB,GAAG;WACH;WACA;;;;;WCtLA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA,iCAAiC;;WAEjC;WACA;WACA;WACA,KAAK;WACL,eAAe;WACf;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM,qBAAqB;WAC3B;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;WACA;WACA;;;;;WCrFA;;;;;UEAA;UACA;UACA;UACA",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://jupyterlab-sql-editor/webpack/container-entry",
         "webpack://jupyterlab-sql-editor/webpack/bootstrap",
         "webpack://jupyterlab-sql-editor/webpack/runtime/compat get default export",
@@ -25,22 +25,22 @@
     ],
     "sourcesContent": [
         "var moduleMap = {\n\t\"./index\": () => {\n\t\treturn __webpack_require__.e(\"lib_index_js\").then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./extension\": () => {\n\t\treturn __webpack_require__.e(\"lib_index_js\").then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./style\": () => {\n\t\treturn Promise.all([__webpack_require__.e(\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\"), __webpack_require__.e(\"style_index_js\")]).then(() => (() => ((__webpack_require__(/*! ./style/index.js */ \"./style/index.js\")))));\n\t}\n};\nvar get = (module, getScope) => {\n\t__webpack_require__.R = getScope;\n\tgetScope = (\n\t\t__webpack_require__.o(moduleMap, module)\n\t\t\t? moduleMap[module]()\n\t\t\t: Promise.resolve().then(() => {\n\t\t\t\tthrow new Error('Module \"' + module + '\" does not exist in container.');\n\t\t\t})\n\t);\n\t__webpack_require__.R = undefined;\n\treturn getScope;\n};\nvar init = (shareScope, initScope) => {\n\tif (!__webpack_require__.S) return;\n\tvar name = \"default\"\n\tvar oldScope = __webpack_require__.S[name];\n\tif(oldScope && oldScope !== shareScope) throw new Error(\"Container initialization failed as it has already been initialized with a different share scope\");\n\t__webpack_require__.S[name] = shareScope;\n\treturn __webpack_require__.I(name, initScope);\n};\n\n// This exports getters to disallow modifications\n__webpack_require__.d(exports, {\n\tget: () => (get),\n\tinit: () => (init)\n});",
         "// The module cache\nvar __webpack_module_cache__ = {};\n\n// The require function\nfunction __webpack_require__(moduleId) {\n\t// Check if module is in cache\n\tvar cachedModule = __webpack_module_cache__[moduleId];\n\tif (cachedModule !== undefined) {\n\t\treturn cachedModule.exports;\n\t}\n\t// Create a new module (and put it into the cache)\n\tvar module = __webpack_module_cache__[moduleId] = {\n\t\tid: moduleId,\n\t\t// no module.loaded needed\n\t\texports: {}\n\t};\n\n\t// Execute the module function\n\t__webpack_modules__[moduleId](module, module.exports, __webpack_require__);\n\n\t// Return the exports of the module\n\treturn module.exports;\n}\n\n// expose the modules object (__webpack_modules__)\n__webpack_require__.m = __webpack_modules__;\n\n// expose the module cache\n__webpack_require__.c = __webpack_module_cache__;\n\n",
         "// getDefaultExport function for compatibility with non-harmony modules\n__webpack_require__.n = (module) => {\n\tvar getter = module && module.__esModule ?\n\t\t() => (module['default']) :\n\t\t() => (module);\n\t__webpack_require__.d(getter, { a: getter });\n\treturn getter;\n};",
         "// define getter functions for harmony exports\n__webpack_require__.d = (exports, definition) => {\n\tfor(var key in definition) {\n\t\tif(__webpack_require__.o(definition, key) && !__webpack_require__.o(exports, key)) {\n\t\t\tObject.defineProperty(exports, key, { enumerable: true, get: definition[key] });\n\t\t}\n\t}\n};",
         "__webpack_require__.f = {};\n// This file contains only the entry chunk.\n// The chunk loading function for additional chunks\n__webpack_require__.e = (chunkId) => {\n\treturn Promise.all(Object.keys(__webpack_require__.f).reduce((promises, key) => {\n\t\t__webpack_require__.f[key](chunkId, promises);\n\t\treturn promises;\n\t}, []));\n};",
-        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"lib_index_js\":\"67b6c3715f795c58c5d6\",\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\":\"8ab7ecce559b1f364311\",\"style_index_js\":\"7a9353dfa84524daa532\",\"vendors-node_modules_sql-formatter_lib_index_js\":\"1955e937c0ff0f3413ea\"}[chunkId] + \".js\";\n};",
+        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"lib_index_js\":\"4c0329159cbdd7702e52\",\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\":\"8ab7ecce559b1f364311\",\"style_index_js\":\"7a9353dfa84524daa532\",\"vendors-node_modules_sql-formatter_lib_index_js\":\"1955e937c0ff0f3413ea\"}[chunkId] + \".js\";\n};",
         "__webpack_require__.g = (function() {\n\tif (typeof globalThis === 'object') return globalThis;\n\ttry {\n\t\treturn this || new Function('return this')();\n\t} catch (e) {\n\t\tif (typeof window === 'object') return window;\n\t}\n})();",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
         "var inProgress = {};\nvar dataWebpackPrefix = \"jupyterlab-sql-editor:\";\n// loadScript function to load a script via script tag\n__webpack_require__.l = (url, done, key, chunkId) => {\n\tif(inProgress[url]) { inProgress[url].push(done); return; }\n\tvar script, needAttach;\n\tif(key !== undefined) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tfor(var i = 0; i < scripts.length; i++) {\n\t\t\tvar s = scripts[i];\n\t\t\tif(s.getAttribute(\"src\") == url || s.getAttribute(\"data-webpack\") == dataWebpackPrefix + key) { script = s; break; }\n\t\t}\n\t}\n\tif(!script) {\n\t\tneedAttach = true;\n\t\tscript = document.createElement('script');\n\n\t\tscript.charset = 'utf-8';\n\t\tscript.timeout = 120;\n\t\tif (__webpack_require__.nc) {\n\t\t\tscript.setAttribute(\"nonce\", __webpack_require__.nc);\n\t\t}\n\t\tscript.setAttribute(\"data-webpack\", dataWebpackPrefix + key);\n\t\tscript.src = url;\n\t}\n\tinProgress[url] = [done];\n\tvar onScriptComplete = (prev, event) => {\n\t\t// avoid mem leaks in IE.\n\t\tscript.onerror = script.onload = null;\n\t\tclearTimeout(timeout);\n\t\tvar doneFns = inProgress[url];\n\t\tdelete inProgress[url];\n\t\tscript.parentNode && script.parentNode.removeChild(script);\n\t\tdoneFns && doneFns.forEach((fn) => (fn(event)));\n\t\tif(prev) return prev(event);\n\t}\n\tvar timeout = setTimeout(onScriptComplete.bind(null, undefined, { type: 'timeout', target: script }), 120000);\n\tscript.onerror = onScriptComplete.bind(null, script.onerror);\n\tscript.onload = onScriptComplete.bind(null, script.onload);\n\tneedAttach && document.head.appendChild(script);\n};",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
-        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => {\n\t\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n\t};\n\tvar uniqueName = \"jupyterlab-sql-editor\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"jupyterlab-sql-editor\", \"0.1.69-alpha.1\", () => (__webpack_require__.e(\"lib_index_js\").then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t\tregister(\"sql-formatter\", \"6.1.2\", () => (__webpack_require__.e(\"vendors-node_modules_sql-formatter_lib_index_js\").then(() => (() => (__webpack_require__(/*! ./node_modules/sql-formatter/lib/index.js */ \"./node_modules/sql-formatter/lib/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
+        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => {\n\t\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n\t};\n\tvar uniqueName = \"jupyterlab-sql-editor\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"jupyterlab-sql-editor\", \"0.1.70\", () => (__webpack_require__.e(\"lib_index_js\").then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t\tregister(\"sql-formatter\", \"6.1.2\", () => (__webpack_require__.e(\"vendors-node_modules_sql-formatter_lib_index_js\").then(() => (() => (__webpack_require__(/*! ./node_modules/sql-formatter/lib/index.js */ \"./node_modules/sql-formatter/lib/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
         "var scriptUrl;\nif (__webpack_require__.g.importScripts) scriptUrl = __webpack_require__.g.location + \"\";\nvar document = __webpack_require__.g.document;\nif (!scriptUrl && document) {\n\tif (document.currentScript)\n\t\tscriptUrl = document.currentScript.src;\n\tif (!scriptUrl) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tif(scripts.length) {\n\t\t\tvar i = scripts.length - 1;\n\t\t\twhile (i > -1 && !scriptUrl) scriptUrl = scripts[i--].src;\n\t\t}\n\t}\n}\n// When supporting browsers where an automatic publicPath is not supported you must specify an output.publicPath manually via configuration\n// or pass an empty string (\"\") and set the __webpack_public_path__ variable from your code to use your own logic.\nif (!scriptUrl) throw new Error(\"Automatic publicPath is not supported in this browser\");\nscriptUrl = scriptUrl.replace(/#.*$/, \"\").replace(/\\?.*$/, \"\").replace(/\\/[^\\/]+$/, \"/\");\n__webpack_require__.p = scriptUrl;",
-        "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warn = (msg) => {\n\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\twarn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/@jupyterlab/settingregistry\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/settingregistry\", [1,3,6,1])),\n\t\"webpack/sharing/consume/default/@krassowski/jupyterlab-lsp\": () => (loadSingletonVersionCheck(\"default\", \"@krassowski/jupyterlab-lsp\", [1,3,10,2])),\n\t\"webpack/sharing/consume/default/@jupyterlab/codemirror\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/codemirror\", [1,3,6,1])),\n\t\"webpack/sharing/consume/default/@jupyterlab/notebook\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/notebook\", [1,3,6,1])),\n\t\"webpack/sharing/consume/default/@jupyterlab/fileeditor\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/fileeditor\", [1,3,6,1])),\n\t\"webpack/sharing/consume/default/@jupyterlab/apputils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/apputils\", [1,3,6,1])),\n\t\"webpack/sharing/consume/default/sql-formatter/sql-formatter\": () => (loadStrictVersionCheckFallback(\"default\", \"sql-formatter\", [4,6,1,2], () => (__webpack_require__.e(\"vendors-node_modules_sql-formatter_lib_index_js\").then(() => (() => (__webpack_require__(/*! sql-formatter */ \"./node_modules/sql-formatter/lib/index.js\")))))))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"lib_index_js\": [\n\t\t\"webpack/sharing/consume/default/@jupyterlab/settingregistry\",\n\t\t\"webpack/sharing/consume/default/@krassowski/jupyterlab-lsp\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/codemirror\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/notebook\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/fileeditor\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/apputils\",\n\t\t\"webpack/sharing/consume/default/sql-formatter/sql-formatter\"\n\t]\n};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t});\n\t}\n}",
+        "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warn = (msg) => {\n\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\twarn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/@jupyterlab/settingregistry\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/settingregistry\", [1,3,6,1])),\n\t\"webpack/sharing/consume/default/@jupyter-lsp/jupyterlab-lsp\": () => (loadSingletonVersionCheck(\"default\", \"@jupyter-lsp/jupyterlab-lsp\", [1,4,2,0])),\n\t\"webpack/sharing/consume/default/@jupyterlab/codemirror\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/codemirror\", [1,3,6,1])),\n\t\"webpack/sharing/consume/default/@jupyterlab/notebook\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/notebook\", [1,3,6,1])),\n\t\"webpack/sharing/consume/default/@jupyterlab/fileeditor\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/fileeditor\", [1,3,6,1])),\n\t\"webpack/sharing/consume/default/@jupyterlab/apputils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/apputils\", [1,3,6,1])),\n\t\"webpack/sharing/consume/default/sql-formatter/sql-formatter\": () => (loadStrictVersionCheckFallback(\"default\", \"sql-formatter\", [4,6,1,2], () => (__webpack_require__.e(\"vendors-node_modules_sql-formatter_lib_index_js\").then(() => (() => (__webpack_require__(/*! sql-formatter */ \"./node_modules/sql-formatter/lib/index.js\")))))))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"lib_index_js\": [\n\t\t\"webpack/sharing/consume/default/@jupyterlab/settingregistry\",\n\t\t\"webpack/sharing/consume/default/@jupyter-lsp/jupyterlab-lsp\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/codemirror\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/notebook\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/fileeditor\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/apputils\",\n\t\t\"webpack/sharing/consume/default/sql-formatter/sql-formatter\"\n\t]\n};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t});\n\t}\n}",
         "// no baseURI\n\n// object to store loaded and loading chunks\n// undefined = chunk not loaded, null = chunk preloaded/prefetched\n// [resolve, reject, Promise] = chunk loading, 0 = chunk loaded\nvar installedChunks = {\n\t\"jupyterlab-sql-editor\": 0\n};\n\n__webpack_require__.f.j = (chunkId, promises) => {\n\t\t// JSONP chunk loading for javascript\n\t\tvar installedChunkData = __webpack_require__.o(installedChunks, chunkId) ? installedChunks[chunkId] : undefined;\n\t\tif(installedChunkData !== 0) { // 0 means \"already installed\".\n\n\t\t\t// a Promise means \"currently loading\".\n\t\t\tif(installedChunkData) {\n\t\t\t\tpromises.push(installedChunkData[2]);\n\t\t\t} else {\n\t\t\t\tif(true) { // all chunks have JS\n\t\t\t\t\t// setup Promise in chunk cache\n\t\t\t\t\tvar promise = new Promise((resolve, reject) => (installedChunkData = installedChunks[chunkId] = [resolve, reject]));\n\t\t\t\t\tpromises.push(installedChunkData[2] = promise);\n\n\t\t\t\t\t// start chunk loading\n\t\t\t\t\tvar url = __webpack_require__.p + __webpack_require__.u(chunkId);\n\t\t\t\t\t// create error before stack unwound to get useful stacktrace later\n\t\t\t\t\tvar error = new Error();\n\t\t\t\t\tvar loadingEnded = (event) => {\n\t\t\t\t\t\tif(__webpack_require__.o(installedChunks, chunkId)) {\n\t\t\t\t\t\t\tinstalledChunkData = installedChunks[chunkId];\n\t\t\t\t\t\t\tif(installedChunkData !== 0) installedChunks[chunkId] = undefined;\n\t\t\t\t\t\t\tif(installedChunkData) {\n\t\t\t\t\t\t\t\tvar errorType = event && (event.type === 'load' ? 'missing' : event.type);\n\t\t\t\t\t\t\t\tvar realSrc = event && event.target && event.target.src;\n\t\t\t\t\t\t\t\terror.message = 'Loading chunk ' + chunkId + ' failed.\\n(' + errorType + ': ' + realSrc + ')';\n\t\t\t\t\t\t\t\terror.name = 'ChunkLoadError';\n\t\t\t\t\t\t\t\terror.type = errorType;\n\t\t\t\t\t\t\t\terror.request = realSrc;\n\t\t\t\t\t\t\t\tinstalledChunkData[1](error);\n\t\t\t\t\t\t\t}\n\t\t\t\t\t\t}\n\t\t\t\t\t};\n\t\t\t\t\t__webpack_require__.l(url, loadingEnded, \"chunk-\" + chunkId, chunkId);\n\t\t\t\t}\n\t\t\t}\n\t\t}\n};\n\n// no prefetching\n\n// no preloaded\n\n// no HMR\n\n// no HMR manifest\n\n// no on chunks loaded\n\n// install a JSONP callback for chunk loading\nvar webpackJsonpCallback = (parentChunkLoadingFunction, data) => {\n\tvar [chunkIds, moreModules, runtime] = data;\n\t// add \"moreModules\" to the modules object,\n\t// then flag all \"chunkIds\" as loaded and fire callback\n\tvar moduleId, chunkId, i = 0;\n\tif(chunkIds.some((id) => (installedChunks[id] !== 0))) {\n\t\tfor(moduleId in moreModules) {\n\t\t\tif(__webpack_require__.o(moreModules, moduleId)) {\n\t\t\t\t__webpack_require__.m[moduleId] = moreModules[moduleId];\n\t\t\t}\n\t\t}\n\t\tif(runtime) var result = runtime(__webpack_require__);\n\t}\n\tif(parentChunkLoadingFunction) parentChunkLoadingFunction(data);\n\tfor(;i < chunkIds.length; i++) {\n\t\tchunkId = chunkIds[i];\n\t\tif(__webpack_require__.o(installedChunks, chunkId) && installedChunks[chunkId]) {\n\t\t\tinstalledChunks[chunkId][0]();\n\t\t}\n\t\tinstalledChunks[chunkId] = 0;\n\t}\n\n}\n\nvar chunkLoadingGlobal = self[\"webpackChunkjupyterlab_sql_editor\"] = self[\"webpackChunkjupyterlab_sql_editor\"] || [];\nchunkLoadingGlobal.forEach(webpackJsonpCallback.bind(null, 0));\nchunkLoadingGlobal.push = webpackJsonpCallback.bind(null, chunkLoadingGlobal.push.bind(chunkLoadingGlobal));",
         "__webpack_require__.nc = undefined;",
         "",
         "// module cache are used so entry inlining is disabled\n// startup\n// Load entry module and return exports\nvar __webpack_exports__ = __webpack_require__(\"webpack/container/entry/jupyterlab-sql-editor\");\n",
         ""
     ],
     "version": 3
```

### Comparing `jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/labextension/static/style_index_js.7a9353dfa84524daa532.js` & `jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/labextension/static/style_index_js.7a9353dfa84524daa532.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/labextension/static/style_index_js.7a9353dfa84524daa532.js.map` & `jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/labextension/static/style_index_js.7a9353dfa84524daa532.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.8ab7ecce559b1f364311.js` & `jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.8ab7ecce559b1f364311.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.8ab7ecce559b1f364311.js.map` & `jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.8ab7ecce559b1f364311.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/labextension/static/vendors-node_modules_sql-formatter_lib_index_js.1955e937c0ff0f3413ea.js` & `jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/labextension/static/vendors-node_modules_sql-formatter_lib_index_js.1955e937c0ff0f3413ea.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/labextension/static/vendors-node_modules_sql-formatter_lib_index_js.1955e937c0ff0f3413ea.js.map` & `jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor/labextension/static/vendors-node_modules_sql-formatter_lib_index_js.1955e937c0ff0f3413ea.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor.egg-info/PKG-INFO` & `jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab-sql-editor
-Version: 0.1.69a1
+Version: 0.1.70
 Summary: SQL editor support for formatting, syntax highlighting and code completion of SQL in cell magic, line magic, python string and file editor.
 Home-page: https://github.com/CybercentreCanada/jupyterlab-sql-editor
 Author: cccs-jc
 Author-email: contact@cyber.gc.ca
 License: MIT License (MIT)
 Keywords: sql,Jupyter,JupyterLab,JupyterLab3,jupyter,jupyterlab-extension,spark,trino,dataframe,cccs,canada
 Platform: Linux
```

### Comparing `jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor.egg-info/SOURCES.txt` & `jupyterlab_sql_editor-0.1.70/jupyterlab_sql_editor.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -38,18 +38,18 @@
 jupyterlab_sql_editor/ipython_magic/trino/parsetab.py
 jupyterlab_sql_editor/ipython_magic/trino/trino.py
 jupyterlab_sql_editor/ipython_magic/trino/trino_export.py
 jupyterlab_sql_editor/labextension/build_log.json
 jupyterlab_sql_editor/labextension/package.json
 jupyterlab_sql_editor/labextension/schemas/jupyterlab-sql-editor/package.json.orig
 jupyterlab_sql_editor/labextension/schemas/jupyterlab-sql-editor/plugin.json
-jupyterlab_sql_editor/labextension/static/lib_index_js.67b6c3715f795c58c5d6.js
-jupyterlab_sql_editor/labextension/static/lib_index_js.67b6c3715f795c58c5d6.js.map
-jupyterlab_sql_editor/labextension/static/remoteEntry.7a5c41927a28f0d15d2b.js
-jupyterlab_sql_editor/labextension/static/remoteEntry.7a5c41927a28f0d15d2b.js.map
+jupyterlab_sql_editor/labextension/static/lib_index_js.4c0329159cbdd7702e52.js
+jupyterlab_sql_editor/labextension/static/lib_index_js.4c0329159cbdd7702e52.js.map
+jupyterlab_sql_editor/labextension/static/remoteEntry.5141fb70facd63fa9a6c.js
+jupyterlab_sql_editor/labextension/static/remoteEntry.5141fb70facd63fa9a6c.js.map
 jupyterlab_sql_editor/labextension/static/style.js
 jupyterlab_sql_editor/labextension/static/style_index_js.7a9353dfa84524daa532.js
 jupyterlab_sql_editor/labextension/static/style_index_js.7a9353dfa84524daa532.js.map
 jupyterlab_sql_editor/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.8ab7ecce559b1f364311.js
 jupyterlab_sql_editor/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.8ab7ecce559b1f364311.js.map
 jupyterlab_sql_editor/labextension/static/vendors-node_modules_sql-formatter_lib_index_js.1955e937c0ff0f3413ea.js
 jupyterlab_sql_editor/labextension/static/vendors-node_modules_sql-formatter_lib_index_js.1955e937c0ff0f3413ea.js.map
```

### Comparing `jupyterlab_sql_editor-0.1.69a1/overrides/sparksql-lsp.json` & `jupyterlab_sql_editor-0.1.70/overrides/sparksql-lsp.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Differences: {'replace': "OrderedDict([('@jupyter-lsp/jupyterlab-lsp:plugin', OrderedDict([('language_servers', "*

 * *            "OrderedDict([('sparksql-language-server', OrderedDict([('serverSettings', "*

 * *            "OrderedDict([('sqlLanguageServer', OrderedDict([('connections', "*

 * *            "[OrderedDict([('name', 'pyspark-conf'), ('adapter', 'json'), ('filename', "*

 * *            "'/home/jovyan/.local/sparkdb.schema.json'), ('jupyterLabMode', True)])])]))]))]))])), "*

 * *            "('extra_node_roots', [])]))])"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "@krassowski/jupyterlab-lsp:plugin": {
+    "@jupyter-lsp/jupyterlab-lsp:plugin": {
         "extra_node_roots": [],
         "language_servers": {
             "sparksql-language-server": {
                 "serverSettings": {
                     "sqlLanguageServer": {
                         "connections": [
                             {
```

### Comparing `jupyterlab_sql_editor-0.1.69a1/overrides/trino-lsp.json` & `jupyterlab_sql_editor-0.1.70/overrides/trino-lsp.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Differences: {'replace': "OrderedDict([('@jupyter-lsp/jupyterlab-lsp:plugin', OrderedDict([('language_servers', "*

 * *            "OrderedDict([('trino-language-server', OrderedDict([('serverSettings', "*

 * *            "OrderedDict([('sqlLanguageServer', OrderedDict([('connections', "*

 * *            "[OrderedDict([('name', 'trino-conf'), ('adapter', 'json'), ('filename', "*

 * *            "'/home/jovyan/.local/trinodb.schema.json'), ('jupyterLabMode', True)])])]))]))]))])), "*

 * *            "('extra_node_roots', [])]))])"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "@krassowski/jupyterlab-lsp:plugin": {
+    "@jupyter-lsp/jupyterlab-lsp:plugin": {
         "extra_node_roots": [],
         "language_servers": {
             "trino-language-server": {
                 "serverSettings": {
                     "sqlLanguageServer": {
                         "connections": [
                             {
```

### Comparing `jupyterlab_sql_editor-0.1.69a1/package.json` & `jupyterlab_sql_editor-0.1.70/package.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9689574314574314%*

 * *Differences: {"'dependencies'": "{'@jupyter-lsp/jupyterlab-lsp': '^4.2.0', delete: "*

 * *                   "['@krassowski/jupyterlab-lsp']}",*

 * * "'devDependencies'": "{'@jupyterlab/builder': '^3.6.5'}",*

 * * "'jupyterlab'": "{'sharedPackages': {replace: OrderedDict([('@jupyter-lsp/jupyterlab-lsp', "*

 * *                 "OrderedDict([('bundled', False), ('singleton', True)]))])}}",*

 * * "'version'": "'0.1.70'"}*

```diff
@@ -3,32 +3,32 @@
         "email": "contact@cyber.gc.ca",
         "name": "cccs-jc"
     },
     "bugs": {
         "url": "https://github.com/CybercentreCanada/jupyterlab-sql-editor/issues"
     },
     "dependencies": {
+        "@jupyter-lsp/jupyterlab-lsp": "^4.2.0",
         "@jupyterlab/application": "3.6.1",
         "@jupyterlab/apputils": "3.6.1",
         "@jupyterlab/cells": "3.6.1",
         "@jupyterlab/codemirror": "3.6.1",
         "@jupyterlab/docmanager": "3.6.1",
         "@jupyterlab/fileeditor": "3.6.1",
         "@jupyterlab/logconsole": "3.6.1",
         "@jupyterlab/notebook": "3.6.1",
         "@jupyterlab/settingregistry": "3.6.1",
-        "@krassowski/jupyterlab-lsp": "^3.10.2",
         "@types/codemirror": "^5.60.5",
         "codemirror": "~5.61.0",
         "npm-run-all": "^4.1.5",
         "sql-formatter": "6.1.2"
     },
     "description": "SQL editor support for formatting, syntax highlighting and code completion of SQL in cell magic, line magic, python string and file editor.",
     "devDependencies": {
-        "@jupyterlab/builder": "3.6.1",
+        "@jupyterlab/builder": "^3.6.5",
         "@types/node": "~18.11.9",
         "@typescript-eslint/eslint-plugin": "^4.8.1",
         "@typescript-eslint/parser": "^4.8.1",
         "eslint": "^7.14.0",
         "eslint-config-prettier": "^6.15.0",
         "eslint-plugin-prettier": "^3.1.4",
         "npm-run-all": "^4.1.5",
@@ -43,15 +43,15 @@
     ],
     "homepage": "https://github.com/CybercentreCanada/jupyterlab-sql-editor",
     "jupyterlab": {
         "extension": true,
         "outputDir": "jupyterlab_sql_editor/labextension",
         "schemaDir": "schema",
         "sharedPackages": {
-            "@krassowski/jupyterlab-lsp": {
+            "@jupyter-lsp/jupyterlab-lsp": {
                 "bundled": false,
                 "singleton": true
             }
         }
     },
     "keywords": [
         "jupyter",
@@ -104,9 +104,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.69-alpha.1"
+    "version": "0.1.70"
 }
```

### Comparing `jupyterlab_sql_editor-0.1.69a1/pyproject.toml` & `jupyterlab_sql_editor-0.1.70/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.69a1/schema/plugin.json` & `jupyterlab_sql_editor-0.1.70/schema/plugin.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.69a1/setup.py` & `jupyterlab_sql_editor-0.1.70/setup.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.69a1/src/formatter.ts` & `jupyterlab_sql_editor-0.1.70/src/formatter.ts`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import { Cell, CodeCell } from '@jupyterlab/cells';
 import { INotebookTracker, Notebook } from '@jupyterlab/notebook';
 import { IEditorTracker } from '@jupyterlab/fileeditor';
 import { showErrorMessage } from '@jupyterlab/apputils';
 import { format } from 'sql-formatter';
-import { RegExpForeignCodeExtractor } from '@krassowski/jupyterlab-lsp';
+import { RegExpForeignCodeExtractor } from '@jupyter-lsp/jupyterlab-lsp';
 import { Constants } from './constants';
 import { JupyterFrontEnd } from '@jupyterlab/application';
 import { cellMagicExtractor, markerExtractor } from './utils';
 import { ICodeMirror } from '@jupyterlab/codemirror';
 import { KeywordCase } from 'sql-formatter';
 
 export class SqlFormatter {
```

### Comparing `jupyterlab_sql_editor-0.1.69a1/src/index.ts` & `jupyterlab_sql_editor-0.1.70/src/index.ts`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import {
   JupyterFrontEnd,
   JupyterFrontEndPlugin
 } from '@jupyterlab/application';
 import { ISettingRegistry } from '@jupyterlab/settingregistry';
-import { ILSPCodeExtractorsManager } from '@krassowski/jupyterlab-lsp';
+import { ILSPCodeExtractorsManager } from '@jupyter-lsp/jupyterlab-lsp';
 import { ICodeMirror } from '@jupyterlab/codemirror'
 import { INotebookTracker } from '@jupyterlab/notebook';
 import { IEditorTracker } from '@jupyterlab/fileeditor';
 import {
   JupyterLabCodeFormatter as SqlCodeFormatter,
   SqlFormatter
 } from './formatter';
```

### Comparing `jupyterlab_sql_editor-0.1.69a1/src/utils.ts` & `jupyterlab_sql_editor-0.1.70/src/utils.ts`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import { RegExpForeignCodeExtractor } from '@krassowski/jupyterlab-lsp';
+import { RegExpForeignCodeExtractor } from '@jupyter-lsp/jupyterlab-lsp';
 import { Mode } from 'codemirror';
 import { ICodeMirror } from '@jupyterlab/codemirror';
 
 function line_magic(language: string) {
   return `%${language}`;
 }
 function cell_magic(language: string) {
```

### Comparing `jupyterlab_sql_editor-0.1.69a1/tsconfig.json` & `jupyterlab_sql_editor-0.1.70/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.69a1/yarn.lock` & `jupyterlab_sql_editor-0.1.70/yarn.lock`

 * *Files 0% similar despite different names*

```diff
@@ -229,14 +229,91 @@
 "@juggle/resize-observer@npm:^3.3.1":
   version: 3.4.0
   resolution: "@juggle/resize-observer@npm:3.4.0"
   checksum: 2505028c05cc2e17639fcad06218b1c4b60f932a4ebb4b41ab546ef8c157031ae377e3f560903801f6d01706dbefd4943b6c4704bf19ed86dfa1c62f1473a570
   languageName: node
   linkType: hard
 
+"@jupyter-lsp/code-jumpers@npm:~1.2.0":
+  version: 1.2.0
+  resolution: "@jupyter-lsp/code-jumpers@npm:1.2.0"
+  peerDependencies:
+    "@jupyterlab/apputils": ^3.1.0
+    "@jupyterlab/codeeditor": ^3.1.0
+    "@jupyterlab/coreutils": ^5.1.0
+    "@jupyterlab/docmanager": ^3.1.0
+    "@jupyterlab/docregistry": ^3.1.0
+    "@jupyterlab/fileeditor": ^3.1.0
+    "@jupyterlab/notebook": ^3.1.0
+    "@jupyterlab/observables": ^4.1.0
+    "@jupyterlab/translation": ^3.1.0
+  checksum: 36ff90ba97d2db260f938190c8a7c011af5da48ddc774c52b310fafd551fde9b6950251395d8c1b6ac664f72fd758b4028553a2604f8b7aef964bbe66fc9e0a1
+  languageName: node
+  linkType: hard
+
+"@jupyter-lsp/completion-theme@npm:^3.0.0, @jupyter-lsp/completion-theme@npm:~3.3.0":
+  version: 3.3.0
+  resolution: "@jupyter-lsp/completion-theme@npm:3.3.0"
+  checksum: f1ee073a6b39c8a8113d4700bd5677d8bfc7b17b2c2679c0c81231f4124498d61ad49a075096d2519cfa156cad6712d0bcf66db6c494c119dd818ab38df5a0c0
+  languageName: node
+  linkType: hard
+
+"@jupyter-lsp/jupyterlab-lsp@npm:^4.2.0":
+  version: 4.2.0
+  resolution: "@jupyter-lsp/jupyterlab-lsp@npm:4.2.0"
+  dependencies:
+    "@jupyter-lsp/code-jumpers": ~1.2.0
+    "@jupyter-lsp/completion-theme": ~3.3.0
+    "@jupyter-lsp/theme-material": ~2.1.1
+    "@jupyter-lsp/theme-vscode": ~2.1.1
+    lodash.mergewith: ^4.6.1
+    lsp-ws-connection: ~0.7.0
+  peerDependencies:
+    "@jupyterlab/application": ^3.3.0
+    "@jupyterlab/apputils": ^3.3.0
+    "@jupyterlab/cells": ^3.3.0
+    "@jupyterlab/codeeditor": ^3.3.0
+    "@jupyterlab/codemirror": ^3.3.0
+    "@jupyterlab/completer": ^3.3.0
+    "@jupyterlab/coreutils": ^5.3.0
+    "@jupyterlab/docmanager": ^3.3.0
+    "@jupyterlab/docregistry": ^3.3.0
+    "@jupyterlab/fileeditor": ^3.3.0
+    "@jupyterlab/notebook": ^3.3.0
+    "@jupyterlab/rendermime": ^3.3.0
+    "@jupyterlab/services": ^6.3.0
+    "@jupyterlab/statusbar": ^3.3.0
+    "@jupyterlab/tooltip": ^3.3.0
+    "@jupyterlab/ui-components": ^3.3.0
+    "@lumino/algorithm": "*"
+    "@lumino/widgets": ^1.16.1
+    codemirror: "*"
+    react: "*"
+  checksum: 4a9f0be881e70765e419f3614265ebadb8f8c85b3b76132c8a106429db31f3dbdf8140367f148c76cb915e13f8c29fbbdbe69c99b8870d88b41343062cd868b8
+  languageName: node
+  linkType: hard
+
+"@jupyter-lsp/theme-material@npm:~2.1.1":
+  version: 2.1.1
+  resolution: "@jupyter-lsp/theme-material@npm:2.1.1"
+  dependencies:
+    "@jupyter-lsp/completion-theme": ^3.0.0
+  checksum: ca1105065aa044b966086be3c3cf562f889abd357e4e39159b3681ab18a7b42d3f6f3109d4e5b7d834cdd619f2cd090d10afaeccc4ec5cd8124aba58abd272b0
+  languageName: node
+  linkType: hard
+
+"@jupyter-lsp/theme-vscode@npm:~2.1.1":
+  version: 2.1.1
+  resolution: "@jupyter-lsp/theme-vscode@npm:2.1.1"
+  dependencies:
+    "@jupyter-lsp/completion-theme": ^3.0.0
+  checksum: 83fd83c853a2ae4b6d9460b47714766a11af1c234ff14e1fae7fe78b6c5575f33ee14d0afb60cd619b5a92865d712d2eeb5dcd48b2add8522bd8d03b2367de15
+  languageName: node
+  linkType: hard
+
 "@jupyter/ydoc@npm:~0.2.0, @jupyter/ydoc@npm:~0.2.3":
   version: 0.2.4
   resolution: "@jupyter/ydoc@npm:0.2.4"
   dependencies:
     "@jupyterlab/nbformat": ^3.0.0 || ^4.0.0-alpha.15
     "@lumino/coreutils": ^1.11.0 || ^2.0.0-alpha.6
     "@lumino/disposable": ^1.10.0 || ^2.0.0-alpha.6
@@ -347,30 +424,30 @@
     "@jupyterlab/rendermime-interfaces": ^3.6.3
     "@lumino/disposable": ^1.10.0
     "@lumino/signaling": ^1.10.0
   checksum: af8f518d824e87307c568c3ebc610864f2fc31c97e4742ac8c8285e7ac0e6f1e305d3e80eee5e17b34c52275f5fd4e5f5a765ca52f47e2099fa7e0d5cce3e20b
   languageName: node
   linkType: hard
 
-"@jupyterlab/builder@npm:3.6.1":
-  version: 3.6.1
-  resolution: "@jupyterlab/builder@npm:3.6.1"
+"@jupyterlab/builder@npm:^3.6.5":
+  version: 3.6.5
+  resolution: "@jupyterlab/builder@npm:3.6.5"
   dependencies:
     "@lumino/algorithm": ^1.9.0
-    "@lumino/application": ^1.31.3
+    "@lumino/application": ^1.31.4
     "@lumino/commands": ^1.19.0
     "@lumino/coreutils": ^1.11.0
     "@lumino/disposable": ^1.10.0
     "@lumino/domutils": ^1.8.0
     "@lumino/dragdrop": ^1.13.0
     "@lumino/messaging": ^1.10.0
     "@lumino/properties": ^1.8.0
     "@lumino/signaling": ^1.10.0
     "@lumino/virtualdom": ^1.14.0
-    "@lumino/widgets": ^1.37.1
+    "@lumino/widgets": ^1.37.2
     ajv: ^6.12.3
     commander: ~6.0.0
     css-loader: ^5.0.1
     duplicate-package-checker-webpack-plugin: ^3.0.0
     file-loader: ~6.0.0
     fs-extra: ^9.0.1
     glob: ~7.1.6
@@ -388,15 +465,15 @@
     url-loader: ~4.1.0
     webpack: ^5.41.1
     webpack-cli: ^4.1.0
     webpack-merge: ^5.1.2
     worker-loader: ^3.0.2
   bin:
     build-labextension: lib/build-labextension.js
-  checksum: aaf9a42d3a2c1e46cdb8d6abd1552ec9e77c4e1df693d747cf342417dd4ddbea5948850f972a806930efade34918a4828bace47aeeb2bbba29c6d3291880a0d7
+  checksum: 51ffb8a6422d9dfc0d087c68a833bc0bd26204f0a3d642b2ac5aa8c012b2db9336e82e6dfc2c921db4ef1024677c1cae96eb401ab8a53f1400d75a546730a36f
   languageName: node
   linkType: hard
 
 "@jupyterlab/cells@npm:3.6.1":
   version: 3.6.1
   resolution: "@jupyterlab/cells@npm:3.6.1"
   dependencies:
@@ -907,106 +984,29 @@
     typestyle: ^2.0.4
   peerDependencies:
     react: ^17.0.1
   checksum: 0809b6b83c1fca0f65cde6d395c18682366760c16a7b133d01abe487b665c3f01979ee082a676bc479ecb8c0b112d8032de8f0ad0ad2d6ec82fe114f04534b6b
   languageName: node
   linkType: hard
 
-"@krassowski/code-jumpers@npm:~1.2.0":
-  version: 1.2.0
-  resolution: "@krassowski/code-jumpers@npm:1.2.0"
-  peerDependencies:
-    "@jupyterlab/apputils": ^3.1.0
-    "@jupyterlab/codeeditor": ^3.1.0
-    "@jupyterlab/coreutils": ^5.1.0
-    "@jupyterlab/docmanager": ^3.1.0
-    "@jupyterlab/docregistry": ^3.1.0
-    "@jupyterlab/fileeditor": ^3.1.0
-    "@jupyterlab/notebook": ^3.1.0
-    "@jupyterlab/observables": ^4.1.0
-    "@jupyterlab/translation": ^3.1.0
-  checksum: 621eab97524cb63d7f38ba760b2f5d9eede74968ec1df91522512115786b5bd2adc04d9b0cce790362cb6020dd2c9b5a481a0102e0e4681107b4450423cb6bfe
-  languageName: node
-  linkType: hard
-
-"@krassowski/completion-theme@npm:^3.0.0, @krassowski/completion-theme@npm:~3.3.1":
-  version: 3.3.1
-  resolution: "@krassowski/completion-theme@npm:3.3.1"
-  checksum: 82738a3d9dc27c24f7b8f9c073839c7e7e75abb6a5413a2169ac43612f1ed1f6bcbfa353e7b97233cf54fb531aedf50b6ebbec85274afbda0b0521bc0d69582e
-  languageName: node
-  linkType: hard
-
-"@krassowski/jupyterlab-lsp@npm:^3.10.2":
-  version: 3.10.2
-  resolution: "@krassowski/jupyterlab-lsp@npm:3.10.2"
-  dependencies:
-    "@krassowski/code-jumpers": ~1.2.0
-    "@krassowski/completion-theme": ~3.3.1
-    "@krassowski/theme-material": ~2.1.1
-    "@krassowski/theme-vscode": ~2.1.1
-    lodash.mergewith: ^4.6.1
-    lsp-ws-connection: ~0.7.0
-  peerDependencies:
-    "@jupyterlab/application": ^3.1.0
-    "@jupyterlab/apputils": ^3.1.0
-    "@jupyterlab/cells": ^3.1.0
-    "@jupyterlab/codeeditor": ^3.1.0
-    "@jupyterlab/codemirror": ^3.1.0
-    "@jupyterlab/completer": ^3.1.0
-    "@jupyterlab/coreutils": ^5.1.0
-    "@jupyterlab/docmanager": ^3.1.0
-    "@jupyterlab/docregistry": ^3.1.0
-    "@jupyterlab/fileeditor": ^3.1.0
-    "@jupyterlab/notebook": ^3.1.0
-    "@jupyterlab/rendermime": ^3.1.0
-    "@jupyterlab/services": ^6.1.0
-    "@jupyterlab/statusbar": ^3.1.0
-    "@jupyterlab/tooltip": ^3.1.0
-    "@jupyterlab/ui-components": ^3.1.0
-    "@lumino/algorithm": "*"
-    "@lumino/widgets": ^1.16.1
-    codemirror: "*"
-    react: "*"
-  checksum: 602342e2745bcf5046cc26c81a2644c979ea36ef6c94842a2374dbb90e851f589b97bf5b7b1f4346f008a91f70067fe1e855bad29f4d136a023e9ec79b62ceeb
-  languageName: node
-  linkType: hard
-
-"@krassowski/theme-material@npm:~2.1.1":
-  version: 2.1.1
-  resolution: "@krassowski/theme-material@npm:2.1.1"
-  dependencies:
-    "@krassowski/completion-theme": ^3.0.0
-  checksum: cd419feaba5ec807949d55ba558476d8bcc96280bab372f54ec42f77d5fc1cc41499fc20ed956549851c3d32c4e4617323b0327737d67b27e1a6147e1108caf7
-  languageName: node
-  linkType: hard
-
-"@krassowski/theme-vscode@npm:~2.1.1":
-  version: 2.1.1
-  resolution: "@krassowski/theme-vscode@npm:2.1.1"
-  dependencies:
-    "@krassowski/completion-theme": ^3.0.0
-  checksum: 867335065ebaa9da9290ce7ce5f73152cb88278d5ec8de02aa809f6535bb523a8f55f54ebc27170062514428341484f9ad0dcb11b1d8eddaafb13f2613961a6b
-  languageName: node
-  linkType: hard
-
 "@lumino/algorithm@npm:^1.9.0, @lumino/algorithm@npm:^1.9.2":
   version: 1.9.2
   resolution: "@lumino/algorithm@npm:1.9.2"
   checksum: a89e7c63504236119634858e271db1cc649684d30ced5a6ebe2788af7c0837f1e05a6fd3047d8525eb756c42ce137f76b3688f75fd3ef915b71cd4f213dfbb96
   languageName: node
   linkType: hard
 
 "@lumino/algorithm@npm:^2.0.0":
   version: 2.0.0
   resolution: "@lumino/algorithm@npm:2.0.0"
   checksum: 663edf536e94397b449c6a2643a735e602fbb396dec86b56ad1193a768dce27c6e7da5ad0384aa90086ea44cbb64dde3f9d565e9fd81858f1eb0c6b4253f3b94
   languageName: node
   linkType: hard
 
-"@lumino/application@npm:^1.31.3":
+"@lumino/application@npm:^1.31.3, @lumino/application@npm:^1.31.4":
   version: 1.31.4
   resolution: "@lumino/application@npm:1.31.4"
   dependencies:
     "@lumino/commands": ^1.21.1
     "@lumino/coreutils": ^1.12.1
     "@lumino/widgets": ^1.37.2
   checksum: 0aa814bf55cef2f54ad730240693d27503b787a834d6d713323973d60b5fa5aae4e3fdf2556e8a2d24d5bf60880add851b84a4b9ac1899ef13daeeecf13d17e7
@@ -3885,25 +3885,25 @@
   languageName: node
   linkType: hard
 
 "jupyterlab-sql-editor@workspace:.":
   version: 0.0.0-use.local
   resolution: "jupyterlab-sql-editor@workspace:."
   dependencies:
+    "@jupyter-lsp/jupyterlab-lsp": ^4.2.0
     "@jupyterlab/application": 3.6.1
     "@jupyterlab/apputils": 3.6.1
-    "@jupyterlab/builder": 3.6.1
+    "@jupyterlab/builder": ^3.6.5
     "@jupyterlab/cells": 3.6.1
     "@jupyterlab/codemirror": 3.6.1
     "@jupyterlab/docmanager": 3.6.1
     "@jupyterlab/fileeditor": 3.6.1
     "@jupyterlab/logconsole": 3.6.1
     "@jupyterlab/notebook": 3.6.1
     "@jupyterlab/settingregistry": 3.6.1
-    "@krassowski/jupyterlab-lsp": ^3.10.2
     "@types/codemirror": ^5.60.5
     "@types/node": ~18.11.9
     "@typescript-eslint/eslint-plugin": ^4.8.1
     "@typescript-eslint/parser": ^4.8.1
     codemirror: ~5.61.0
     eslint: ^7.14.0
     eslint-config-prettier: ^6.15.0
@@ -5330,19 +5330,19 @@
     ajv: ^6.12.5
     ajv-keywords: ^3.5.2
   checksum: 39683edfe3beff018cdb1ae4fa296fc55cea13a080aa2b4d9351895cd64b22ba4d87e2e548c2a2ac1bc76e60980670adb0f413a58104479f1a0c12e5663cb8ca
   languageName: node
   linkType: hard
 
 "semver@npm:2 || 3 || 4 || 5, semver@npm:^5.4.1, semver@npm:^5.5.0":
-  version: 5.7.1
-  resolution: "semver@npm:5.7.1"
+  version: 5.7.2
+  resolution: "semver@npm:5.7.2"
   bin:
-    semver: ./bin/semver
-  checksum: 57fd0acfd0bac382ee87cd52cd0aaa5af086a7dc8d60379dfe65fea491fb2489b6016400813930ecd61fd0952dae75c115287a1b16c234b1550887117744dfaf
+    semver: bin/semver
+  checksum: fb4ab5e0dd1c22ce0c937ea390b4a822147a9c53dbd2a9a0132f12fe382902beef4fbf12cf51bb955248d8d15874ce8cd89532569756384f994309825f10b686
   languageName: node
   linkType: hard
 
 "semver@npm:^6.0.0":
   version: 6.3.0
   resolution: "semver@npm:6.3.0"
   bin:
@@ -6425,17 +6425,17 @@
   version: 2.0.1
   resolution: "wildcard@npm:2.0.1"
   checksum: e0c60a12a219e4b12065d1199802d81c27b841ed6ad6d9d28240980c73ceec6f856771d575af367cbec2982d9ae7838759168b551776577f155044f5a5ba843c
   languageName: node
   linkType: hard
 
 "word-wrap@npm:^1.2.3":
-  version: 1.2.3
-  resolution: "word-wrap@npm:1.2.3"
-  checksum: 30b48f91fcf12106ed3186ae4fa86a6a1842416df425be7b60485de14bec665a54a68e4b5156647dec3a70f25e84d270ca8bc8cd23182ed095f5c7206a938c1f
+  version: 1.2.4
+  resolution: "word-wrap@npm:1.2.4"
+  checksum: 8f1f2e0a397c0e074ca225ba9f67baa23f99293bc064e31355d426ae91b8b3f6b5f6c1fc9ae5e9141178bb362d563f55e62fd8d5c31f2a77e3ade56cb3e35bd1
   languageName: node
   linkType: hard
 
 "worker-loader@npm:^3.0.2":
   version: 3.0.8
   resolution: "worker-loader@npm:3.0.8"
   dependencies:
```

