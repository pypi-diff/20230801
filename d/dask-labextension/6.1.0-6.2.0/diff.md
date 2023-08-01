# Comparing `tmp/dask_labextension-6.1.0.tar.gz` & `tmp/dask_labextension-6.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dask_labextension-6.1.0.tar", last modified: Sun Feb 19 00:30:47 2023, max compression
+gzip compressed data, was "dask_labextension-6.2.0.tar", last modified: Tue Aug  1 20:27:26 2023, max compression
```

## Comparing `dask_labextension-6.1.0.tar` & `dask_labextension-6.2.0.tar`

### file list

```diff
@@ -1,60 +1,62 @@
-drwxrwxr-x   0 ian       (1000) ian       (1000)        0 2023-02-19 00:30:47.771650 dask_labextension-6.1.0/
--rw-rw-r--   0 ian       (1000) ian       (1000)     1532 2023-02-18 16:05:13.000000 dask_labextension-6.1.0/LICENSE
--rw-rw-r--   0 ian       (1000) ian       (1000)      606 2023-02-18 16:05:13.000000 dask_labextension-6.1.0/MANIFEST.in
--rw-rw-r--   0 ian       (1000) ian       (1000)     8062 2023-02-19 00:30:47.771650 dask_labextension-6.1.0/PKG-INFO
--rw-rw-r--   0 ian       (1000) ian       (1000)     7326 2023-02-18 16:05:13.000000 dask_labextension-6.1.0/README.md
-drwxrwxr-x   0 ian       (1000) ian       (1000)        0 2023-02-19 00:30:47.771650 dask_labextension-6.1.0/dask_labextension/
--rw-rw-r--   0 ian       (1000) ian       (1000)     1581 2023-02-18 16:05:13.000000 dask_labextension-6.1.0/dask_labextension/__init__.py
--rw-rw-r--   0 ian       (1000) ian       (1000)      536 2023-02-19 00:30:47.771650 dask_labextension-6.1.0/dask_labextension/_version.py
--rw-rw-r--   0 ian       (1000) ian       (1000)     2893 2023-02-18 16:05:13.000000 dask_labextension-6.1.0/dask_labextension/clusterhandler.py
--rw-rw-r--   0 ian       (1000) ian       (1000)      297 2023-02-18 16:05:13.000000 dask_labextension-6.1.0/dask_labextension/config.py
--rw-rw-r--   0 ian       (1000) ian       (1000)     7539 2023-02-19 00:15:04.000000 dask_labextension-6.1.0/dask_labextension/dashboardhandler.py
-drwxrwxr-x   0 ian       (1000) ian       (1000)        0 2023-02-19 00:30:47.767658 dask_labextension-6.1.0/dask_labextension/labextension/
--rw-rw-r--   0 ian       (1000) ian       (1000)     3605 2023-02-19 00:30:47.000000 dask_labextension-6.1.0/dask_labextension/labextension/package.json
-drwxrwxr-x   0 ian       (1000) ian       (1000)        0 2023-02-19 00:30:47.763666 dask_labextension-6.1.0/dask_labextension/labextension/schemas/
-drwxrwxr-x   0 ian       (1000) ian       (1000)        0 2023-02-19 00:30:47.767658 dask_labextension-6.1.0/dask_labextension/labextension/schemas/dask-labextension/
--rw-rw-r--   0 ian       (1000) ian       (1000)     3489 2023-02-19 00:30:45.000000 dask_labextension-6.1.0/dask_labextension/labextension/schemas/dask-labextension/package.json.orig
--rw-rw-r--   0 ian       (1000) ian       (1000)     2822 2023-02-19 00:30:45.000000 dask_labextension-6.1.0/dask_labextension/labextension/schemas/dask-labextension/plugin.json
-drwxrwxr-x   0 ian       (1000) ian       (1000)        0 2023-02-19 00:30:47.767658 dask_labextension-6.1.0/dask_labextension/labextension/static/
--rw-rw-r--   0 ian       (1000) ian       (1000)     8567 2023-02-19 00:30:47.000000 dask_labextension-6.1.0/dask_labextension/labextension/static/114.6d8f6f4a88afc2816496.js
--rw-rw-r--   0 ian       (1000) ian       (1000)    41509 2023-02-19 00:30:47.000000 dask_labextension-6.1.0/dask_labextension/labextension/static/319.3ff908a63582f9623f31.js
--rw-rw-r--   0 ian       (1000) ian       (1000)     7780 2023-02-19 00:30:47.000000 dask_labextension-6.1.0/dask_labextension/labextension/static/remoteEntry.c559dc887be99a51d44a.js
--rw-rw-r--   0 ian       (1000) ian       (1000)      118 2023-02-19 00:30:45.000000 dask_labextension-6.1.0/dask_labextension/labextension/static/style.js
--rw-rw-r--   0 ian       (1000) ian       (1000)     2590 2023-02-19 00:30:47.000000 dask_labextension-6.1.0/dask_labextension/labextension/static/third-party-licenses.json
--rw-rw-r--   0 ian       (1000) ian       (1000)      361 2023-02-18 16:05:13.000000 dask_labextension-6.1.0/dask_labextension/labextension.yaml
--rw-rw-r--   0 ian       (1000) ian       (1000)     9359 2023-02-18 16:05:13.000000 dask_labextension-6.1.0/dask_labextension/manager.py
-drwxrwxr-x   0 ian       (1000) ian       (1000)        0 2023-02-19 00:30:47.767658 dask_labextension-6.1.0/dask_labextension/tests/
--rw-rw-r--   0 ian       (1000) ian       (1000)     5094 2023-02-18 16:05:13.000000 dask_labextension-6.1.0/dask_labextension/tests/test_manager.py
-drwxrwxr-x   0 ian       (1000) ian       (1000)        0 2023-02-19 00:30:47.767658 dask_labextension-6.1.0/dask_labextension.egg-info/
--rw-rw-r--   0 ian       (1000) ian       (1000)     8062 2023-02-19 00:30:47.000000 dask_labextension-6.1.0/dask_labextension.egg-info/PKG-INFO
--rw-rw-r--   0 ian       (1000) ian       (1000)     1450 2023-02-19 00:30:47.000000 dask_labextension-6.1.0/dask_labextension.egg-info/SOURCES.txt
--rw-rw-r--   0 ian       (1000) ian       (1000)        1 2023-02-19 00:30:47.000000 dask_labextension-6.1.0/dask_labextension.egg-info/dependency_links.txt
--rw-rw-r--   0 ian       (1000) ian       (1000)        1 2023-02-19 00:18:55.000000 dask_labextension-6.1.0/dask_labextension.egg-info/not-zip-safe
--rw-rw-r--   0 ian       (1000) ian       (1000)       87 2023-02-19 00:30:47.000000 dask_labextension-6.1.0/dask_labextension.egg-info/requires.txt
--rw-rw-r--   0 ian       (1000) ian       (1000)       18 2023-02-19 00:30:47.000000 dask_labextension-6.1.0/dask_labextension.egg-info/top_level.txt
--rw-rw-r--   0 ian       (1000) ian       (1000)      195 2023-02-18 16:05:13.000000 dask_labextension-6.1.0/install.json
-drwxrwxr-x   0 ian       (1000) ian       (1000)        0 2023-02-19 00:30:47.763666 dask_labextension-6.1.0/jupyter-config/
-drwxrwxr-x   0 ian       (1000) ian       (1000)        0 2023-02-19 00:30:47.767658 dask_labextension-6.1.0/jupyter-config/jupyter_notebook_config.d/
--rw-rw-r--   0 ian       (1000) ian       (1000)       94 2023-02-18 16:05:13.000000 dask_labextension-6.1.0/jupyter-config/jupyter_notebook_config.d/dask_labextension.json
-drwxrwxr-x   0 ian       (1000) ian       (1000)        0 2023-02-19 00:30:47.767658 dask_labextension-6.1.0/jupyter-config/jupyter_server_config.d/
--rw-rw-r--   0 ian       (1000) ian       (1000)       92 2023-02-18 16:05:13.000000 dask_labextension-6.1.0/jupyter-config/jupyter_server_config.d/dask_labextension.json
--rw-rw-r--   0 ian       (1000) ian       (1000)     3489 2023-02-19 00:28:03.000000 dask_labextension-6.1.0/package.json
--rw-rw-r--   0 ian       (1000) ian       (1000)      157 2023-02-18 16:05:13.000000 dask_labextension-6.1.0/pyproject.toml
-drwxrwxr-x   0 ian       (1000) ian       (1000)        0 2023-02-19 00:30:47.767658 dask_labextension-6.1.0/schema/
--rw-rw-r--   0 ian       (1000) ian       (1000)     2822 2023-02-18 16:05:13.000000 dask_labextension-6.1.0/schema/plugin.json
--rw-rw-r--   0 ian       (1000) ian       (1000)      738 2023-02-19 00:30:47.771650 dask_labextension-6.1.0/setup.cfg
--rw-rw-r--   0 ian       (1000) ian       (1000)     2858 2023-02-18 16:05:13.000000 dask_labextension-6.1.0/setup.py
-drwxrwxr-x   0 ian       (1000) ian       (1000)        0 2023-02-19 00:30:47.771650 dask_labextension-6.1.0/src/
--rw-rw-r--   0 ian       (1000) ian       (1000)    23013 2023-02-18 16:05:13.000000 dask_labextension-6.1.0/src/clusters.tsx
--rw-rw-r--   0 ian       (1000) ian       (1000)    17355 2023-02-18 16:05:13.000000 dask_labextension-6.1.0/src/dashboard.tsx
--rw-rw-r--   0 ian       (1000) ian       (1000)    25346 2023-02-18 16:05:13.000000 dask_labextension-6.1.0/src/index.ts
--rw-rw-r--   0 ian       (1000) ian       (1000)     7137 2023-02-18 16:05:13.000000 dask_labextension-6.1.0/src/scaling.tsx
--rw-rw-r--   0 ian       (1000) ian       (1000)     2657 2023-02-18 16:05:13.000000 dask_labextension-6.1.0/src/sidebar.ts
-drwxrwxr-x   0 ian       (1000) ian       (1000)        0 2023-02-19 00:30:47.771650 dask_labextension-6.1.0/style/
--rw-rw-r--   0 ian       (1000) ian       (1000)      246 2023-02-18 16:05:13.000000 dask_labextension-6.1.0/style/code-dark.svg
--rw-rw-r--   0 ian       (1000) ian       (1000)      246 2023-02-18 16:05:13.000000 dask_labextension-6.1.0/style/code-light.svg
--rw-rw-r--   0 ian       (1000) ian       (1000)     1607 2023-02-18 16:05:13.000000 dask_labextension-6.1.0/style/dask.svg
--rw-rw-r--   0 ian       (1000) ian       (1000)     6941 2023-02-18 16:05:13.000000 dask_labextension-6.1.0/style/index.css
--rw-rw-r--   0 ian       (1000) ian       (1000)       75 2023-02-18 16:05:13.000000 dask_labextension-6.1.0/tsconfig.eslint.json
--rw-rw-r--   0 ian       (1000) ian       (1000)      555 2023-02-19 00:27:41.000000 dask_labextension-6.1.0/tsconfig.json
--rw-rw-r--   0 ian       (1000) ian       (1000)    69015 2023-02-18 16:05:13.000000 dask_labextension-6.1.0/versioneer.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-01 20:27:26.726349 dask_labextension-6.2.0/
+-rw-r--r--   0 james      (501) staff       (20)     1532 2023-08-01 20:08:53.000000 dask_labextension-6.2.0/LICENSE
+-rw-r--r--   0 james      (501) staff       (20)      625 2023-08-01 20:23:30.000000 dask_labextension-6.2.0/MANIFEST.in
+-rw-r--r--   0 james      (501) staff       (20)     8480 2023-08-01 20:27:26.726416 dask_labextension-6.2.0/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)     7744 2023-08-01 20:23:30.000000 dask_labextension-6.2.0/README.md
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-01 20:27:26.726832 dask_labextension-6.2.0/dask_labextension/
+-rw-r--r--   0 james      (501) staff       (20)     1581 2023-08-01 20:09:43.000000 dask_labextension-6.2.0/dask_labextension/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)      536 2023-08-01 20:27:26.726869 dask_labextension-6.2.0/dask_labextension/_version.py
+-rw-r--r--   0 james      (501) staff       (20)     2893 2023-08-01 20:09:43.000000 dask_labextension-6.2.0/dask_labextension/clusterhandler.py
+-rw-r--r--   0 james      (501) staff       (20)      297 2023-08-01 20:08:53.000000 dask_labextension-6.2.0/dask_labextension/config.py
+-rw-r--r--   0 james      (501) staff       (20)     7539 2023-08-01 20:09:43.000000 dask_labextension-6.2.0/dask_labextension/dashboardhandler.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-01 20:27:26.722708 dask_labextension-6.2.0/dask_labextension/labextension/
+-rw-r--r--   0 james      (501) staff       (20)     3639 2023-08-01 20:27:26.000000 dask_labextension-6.2.0/dask_labextension/labextension/package.json
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-01 20:27:26.717866 dask_labextension-6.2.0/dask_labextension/labextension/schemas/
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-01 20:27:26.722957 dask_labextension-6.2.0/dask_labextension/labextension/schemas/dask-labextension/
+-rw-r--r--   0 james      (501) staff       (20)     3523 2023-08-01 20:27:25.000000 dask_labextension-6.2.0/dask_labextension/labextension/schemas/dask-labextension/package.json.orig
+-rw-r--r--   0 james      (501) staff       (20)     2822 2023-08-01 20:27:25.000000 dask_labextension-6.2.0/dask_labextension/labextension/schemas/dask-labextension/plugin.json
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-01 20:27:26.723598 dask_labextension-6.2.0/dask_labextension/labextension/static/
+-rw-r--r--   0 james      (501) staff       (20)     8783 2023-08-01 20:27:26.000000 dask_labextension-6.2.0/dask_labextension/labextension/static/114.f9e3bc980911cf750147.js
+-rw-r--r--   0 james      (501) staff       (20)    43202 2023-08-01 20:27:26.000000 dask_labextension-6.2.0/dask_labextension/labextension/static/224.86c44b816becca807a99.js
+-rw-r--r--   0 james      (501) staff       (20)     7818 2023-08-01 20:27:26.000000 dask_labextension-6.2.0/dask_labextension/labextension/static/remoteEntry.48341a7428463ba2c6bb.js
+-rw-r--r--   0 james      (501) staff       (20)      118 2023-08-01 20:27:25.000000 dask_labextension-6.2.0/dask_labextension/labextension/static/style.js
+-rw-r--r--   0 james      (501) staff       (20)     2590 2023-08-01 20:27:26.000000 dask_labextension-6.2.0/dask_labextension/labextension/static/third-party-licenses.json
+-rw-r--r--   0 james      (501) staff       (20)      361 2023-08-01 20:09:43.000000 dask_labextension-6.2.0/dask_labextension/labextension.yaml
+-rw-r--r--   0 james      (501) staff       (20)     9359 2023-08-01 20:09:43.000000 dask_labextension-6.2.0/dask_labextension/manager.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-01 20:27:26.723714 dask_labextension-6.2.0/dask_labextension/tests/
+-rw-r--r--   0 james      (501) staff       (20)     5094 2023-08-01 20:09:43.000000 dask_labextension-6.2.0/dask_labextension/tests/test_manager.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-01 20:27:26.722579 dask_labextension-6.2.0/dask_labextension.egg-info/
+-rw-r--r--   0 james      (501) staff       (20)     8480 2023-08-01 20:27:26.000000 dask_labextension-6.2.0/dask_labextension.egg-info/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)     1473 2023-08-01 20:27:26.000000 dask_labextension-6.2.0/dask_labextension.egg-info/SOURCES.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2023-08-01 20:27:26.000000 dask_labextension-6.2.0/dask_labextension.egg-info/dependency_links.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2023-08-01 20:27:00.000000 dask_labextension-6.2.0/dask_labextension.egg-info/not-zip-safe
+-rw-r--r--   0 james      (501) staff       (20)       90 2023-08-01 20:27:26.000000 dask_labextension-6.2.0/dask_labextension.egg-info/requires.txt
+-rw-r--r--   0 james      (501) staff       (20)       18 2023-08-01 20:27:26.000000 dask_labextension-6.2.0/dask_labextension.egg-info/top_level.txt
+-rw-r--r--   0 james      (501) staff       (20)      195 2023-08-01 20:09:43.000000 dask_labextension-6.2.0/install.json
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-01 20:27:26.718234 dask_labextension-6.2.0/jupyter-config/
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-01 20:27:26.723840 dask_labextension-6.2.0/jupyter-config/jupyter_notebook_config.d/
+-rw-r--r--   0 james      (501) staff       (20)       94 2023-08-01 20:08:53.000000 dask_labextension-6.2.0/jupyter-config/jupyter_notebook_config.d/dask_labextension.json
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-01 20:27:26.724831 dask_labextension-6.2.0/jupyter-config/jupyter_server_config.d/
+-rw-r--r--   0 james      (501) staff       (20)       92 2023-08-01 20:09:43.000000 dask_labextension-6.2.0/jupyter-config/jupyter_server_config.d/dask_labextension.json
+-rw-r--r--   0 james      (501) staff       (20)     3523 2023-08-01 20:25:35.000000 dask_labextension-6.2.0/package.json
+-rw-r--r--   0 james      (501) staff       (20)      157 2023-08-01 20:09:43.000000 dask_labextension-6.2.0/pyproject.toml
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-01 20:27:26.725031 dask_labextension-6.2.0/schema/
+-rw-r--r--   0 james      (501) staff       (20)     2822 2023-08-01 20:09:43.000000 dask_labextension-6.2.0/schema/plugin.json
+-rw-r--r--   0 james      (501) staff       (20)      738 2023-08-01 20:27:26.726709 dask_labextension-6.2.0/setup.cfg
+-rw-r--r--   0 james      (501) staff       (20)     2861 2023-08-01 20:23:30.000000 dask_labextension-6.2.0/setup.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-01 20:27:26.725773 dask_labextension-6.2.0/src/
+-rw-r--r--   0 james      (501) staff       (20)    23013 2023-08-01 20:09:43.000000 dask_labextension-6.2.0/src/clusters.tsx
+-rw-r--r--   0 james      (501) staff       (20)    17355 2023-08-01 20:09:43.000000 dask_labextension-6.2.0/src/dashboard.tsx
+-rw-r--r--   0 james      (501) staff       (20)    25542 2023-08-01 20:09:43.000000 dask_labextension-6.2.0/src/index.ts
+-rw-r--r--   0 james      (501) staff       (20)     7137 2023-08-01 20:08:53.000000 dask_labextension-6.2.0/src/scaling.tsx
+-rw-r--r--   0 james      (501) staff       (20)     2657 2023-08-01 20:08:53.000000 dask_labextension-6.2.0/src/sidebar.ts
+-rw-r--r--   0 james      (501) staff       (20)       74 2023-08-01 20:09:43.000000 dask_labextension-6.2.0/src/svg.d.ts
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-01 20:27:26.726227 dask_labextension-6.2.0/style/
+-rw-r--r--   0 james      (501) staff       (20)      246 2023-08-01 20:08:53.000000 dask_labextension-6.2.0/style/code-dark.svg
+-rw-r--r--   0 james      (501) staff       (20)      246 2023-08-01 20:08:53.000000 dask_labextension-6.2.0/style/code-light.svg
+-rw-r--r--   0 james      (501) staff       (20)     1607 2023-08-01 20:09:43.000000 dask_labextension-6.2.0/style/dask.svg
+-rw-r--r--   0 james      (501) staff       (20)     6941 2023-08-01 20:09:43.000000 dask_labextension-6.2.0/style/index.css
+-rw-r--r--   0 james      (501) staff       (20)       75 2023-08-01 20:09:43.000000 dask_labextension-6.2.0/tsconfig.eslint.json
+-rw-r--r--   0 james      (501) staff       (20)      555 2023-08-01 20:09:43.000000 dask_labextension-6.2.0/tsconfig.json
+-rw-r--r--   0 james      (501) staff       (20)    69015 2023-08-01 20:09:43.000000 dask_labextension-6.2.0/versioneer.py
+-rw-r--r--   0 james      (501) staff       (20)   214431 2023-08-01 20:23:30.000000 dask_labextension-6.2.0/yarn.lock
```

### Comparing `dask_labextension-6.1.0/LICENSE` & `dask_labextension-6.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dask_labextension-6.1.0/MANIFEST.in` & `dask_labextension-6.2.0/MANIFEST.in`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 include pyproject.toml
 include jupyter-config/dask_labextension.json
 
 include package.json
 include install.json
 include ts*.json
 
+include yarn.lock
+
 graft dask_labextension/labextension
 
 # Javascript files
 graft src
 graft style
 graft schema
 prune **/node_modules
```

### Comparing `dask_labextension-6.1.0/PKG-INFO` & `dask_labextension-6.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: dask_labextension
-Version: 6.1.0
-Summary: A JupyterLab extension for Dask.
-Home-page: https://github.com/dask/dask-labextension
-Author: Ian Rose, Matt Rocklin, Jacob Tomlinson
-License: BSD-3-Clause
-Keywords: dask,Jupyter,JupyterLab,JupyterLab3
-Platform: Linux
-Platform: Mac OS X
-Platform: Windows
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Framework :: Jupyter
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Dask JupyterLab Extension
 
 [![Build Status](https://travis-ci.org/dask/dask-labextension.svg?branch=main)](https://travis-ci.org/dask/dask-labextension) [![Version](https://img.shields.io/npm/v/dask-labextension.svg)](https://www.npmjs.com/package/dask-labextension) [![Downloads](https://img.shields.io/npm/dm/dask-labextension.svg)](https://www.npmjs.com/package/dask-labextension) [![Dependencies](https://img.shields.io/librariesio/release/npm/dask-labextension.svg)](https://libraries.io/npm/dask-labextension)
 
 This package provides a JupyterLab extension to manage Dask clusters,
 as well as embed Dask's dashboard plots directly into JupyterLab panes.
 
@@ -231,26 +209,39 @@
 ```bash
 pip install -e .
 jupyter serverextension enable --sys-prefix dask_labextension
 ```
 
 ## Publishing
 
-This application is distributed as two subpackages.
-
-The JupyterLab frontend part is published to [npm](https://www.npmjs.com/package/dask-labextension),
-and the server-side part to [PyPI](https://pypi.org/project/dask-labextension/).
-
-Releases for both packages are done with the `jlpm` tool, `git` and Travis CI.
+This extension contains a front-end component written in TypeScript
+and a back-end component written in Python.
+The front-end is compiled to Javascript during the build process
+and is distributed as static assets along with the Python package.
 
 _Note: Package versions are not prefixed with the letter `v`. You will need to disable this._
 
 ```console
 $ jlpm config set version-tag-prefix ""
 ```
 
-Making a release
+### Release process
 
-```console
-$ jlpm version [--major|--minor|--patch]  # updates package.json and creates git commit and tag
-$ git push upstream main && git push upstream main --tags  # pushes tags to GitHub which triggers Travis CI to build and deploy
+This requires `node`, `build`, and `twine` to be installed.
+
+```bash
+jlpm version [--major|--minor|--patch]  # updates package.json and creates git commit and tag
+git push upstream main && git push upstream main --tags  # pushes to GitHub
+python -m build .  # Build the package
+twine upload dist/*  # Upload the package to PyPI
+```
+
+### Handling Javascript package version conflicts
+
+Unlike Python, Javascript packages can include more than one version of the same dependency.
+Usually the `yarn` package manager handles this okay, but occasionally you might end up with conflicting versions,
+or with unexpected package bloat.
+You can try to fix this by deduplicating dependencies:
+
+```bash
+jlpm yarn-deduplicate -s fewer
 ```
```

#### html2text {}

```diff
@@ -1,18 +1,8 @@
-Metadata-Version: 2.1 Name: dask_labextension Version: 6.1.0 Summary: A
-JupyterLab extension for Dask. Home-page: https://github.com/dask/dask-
-labextension Author: Ian Rose, Matt Rocklin, Jacob Tomlinson License: BSD-3-
-Clause Keywords: dask,Jupyter,JupyterLab,JupyterLab3 Platform: Linux Platform:
-Mac OS X Platform: Windows Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python Classifier: Programming Language ::
-Python :: 3 Classifier: Programming Language :: Python :: 3.6 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Framework :: Jupyter Requires-Python: >=3.6
-Description-Content-Type: text/markdown License-File: LICENSE # Dask JupyterLab
-Extension [![Build Status](https://travis-ci.org/dask/dask-
+# Dask JupyterLab Extension [![Build Status](https://travis-ci.org/dask/dask-
 labextension.svg?branch=main)](https://travis-ci.org/dask/dask-labextension) [!
 [Version](https://img.shields.io/npm/v/dask-labextension.svg)](https://
 www.npmjs.com/package/dask-labextension) [![Downloads](https://img.shields.io/
 npm/dm/dask-labextension.svg)](https://www.npmjs.com/package/dask-labextension)
 [![Dependencies](https://img.shields.io/librariesio/release/npm/dask-
 labextension.svg)](https://libraries.io/npm/dask-labextension) This package
 provides a JupyterLab extension to manage Dask clusters, as well as embed
@@ -84,17 +74,22 @@
 of the labextension you can run the following in this directory: ```bash jlpm #
 Install npm package dependencies jlpm build # Compile the TypeScript sources to
 Javascript jupyter labextension develop . --overwrite # Install the current
 directory as an extension ``` To rebuild the extension: ```bash jlpm build ```
 You should then be able to refresh the JupyterLab page and it will pick up the
 changes to the extension. To run an editable install of the server extension,
 run ```bash pip install -e . jupyter serverextension enable --sys-prefix
-dask_labextension ``` ## Publishing This application is distributed as two
-subpackages. The JupyterLab frontend part is published to [npm](https://
-www.npmjs.com/package/dask-labextension), and the server-side part to [PyPI]
-(https://pypi.org/project/dask-labextension/). Releases for both packages are
-done with the `jlpm` tool, `git` and Travis CI. _Note: Package versions are not
+dask_labextension ``` ## Publishing This extension contains a front-end
+component written in TypeScript and a back-end component written in Python. The
+front-end is compiled to Javascript during the build process and is distributed
+as static assets along with the Python package. _Note: Package versions are not
 prefixed with the letter `v`. You will need to disable this._ ```console $ jlpm
-config set version-tag-prefix "" ``` Making a release ```console $ jlpm version
-[--major|--minor|--patch] # updates package.json and creates git commit and tag
-$ git push upstream main && git push upstream main --tags # pushes tags to
-GitHub which triggers Travis CI to build and deploy ```
+config set version-tag-prefix "" ``` ### Release process This requires `node`,
+`build`, and `twine` to be installed. ```bash jlpm version [--major|--minor|--
+patch] # updates package.json and creates git commit and tag git push upstream
+main && git push upstream main --tags # pushes to GitHub python -m build . #
+Build the package twine upload dist/* # Upload the package to PyPI ``` ###
+Handling Javascript package version conflicts Unlike Python, Javascript
+packages can include more than one version of the same dependency. Usually the
+`yarn` package manager handles this okay, but occasionally you might end up
+with conflicting versions, or with unexpected package bloat. You can try to fix
+this by deduplicating dependencies: ```bash jlpm yarn-deduplicate -s fewer ```
```

### Comparing `dask_labextension-6.1.0/README.md` & `dask_labextension-6.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: dask_labextension
+Version: 6.2.0
+Summary: A JupyterLab extension for Dask.
+Home-page: https://github.com/dask/dask-labextension
+Author: Ian Rose, Matt Rocklin, Jacob Tomlinson
+License: BSD-3-Clause
+Keywords: dask,Jupyter,JupyterLab,JupyterLab3
+Platform: Linux
+Platform: Mac OS X
+Platform: Windows
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Framework :: Jupyter
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Dask JupyterLab Extension
 
 [![Build Status](https://travis-ci.org/dask/dask-labextension.svg?branch=main)](https://travis-ci.org/dask/dask-labextension) [![Version](https://img.shields.io/npm/v/dask-labextension.svg)](https://www.npmjs.com/package/dask-labextension) [![Downloads](https://img.shields.io/npm/dm/dask-labextension.svg)](https://www.npmjs.com/package/dask-labextension) [![Dependencies](https://img.shields.io/librariesio/release/npm/dask-labextension.svg)](https://libraries.io/npm/dask-labextension)
 
 This package provides a JupyterLab extension to manage Dask clusters,
 as well as embed Dask's dashboard plots directly into JupyterLab panes.
 
@@ -209,26 +231,39 @@
 ```bash
 pip install -e .
 jupyter serverextension enable --sys-prefix dask_labextension
 ```
 
 ## Publishing
 
-This application is distributed as two subpackages.
-
-The JupyterLab frontend part is published to [npm](https://www.npmjs.com/package/dask-labextension),
-and the server-side part to [PyPI](https://pypi.org/project/dask-labextension/).
-
-Releases for both packages are done with the `jlpm` tool, `git` and Travis CI.
+This extension contains a front-end component written in TypeScript
+and a back-end component written in Python.
+The front-end is compiled to Javascript during the build process
+and is distributed as static assets along with the Python package.
 
 _Note: Package versions are not prefixed with the letter `v`. You will need to disable this._
 
 ```console
 $ jlpm config set version-tag-prefix ""
 ```
 
-Making a release
+### Release process
 
-```console
-$ jlpm version [--major|--minor|--patch]  # updates package.json and creates git commit and tag
-$ git push upstream main && git push upstream main --tags  # pushes tags to GitHub which triggers Travis CI to build and deploy
+This requires `node`, `build`, and `twine` to be installed.
+
+```bash
+jlpm version [--major|--minor|--patch]  # updates package.json and creates git commit and tag
+git push upstream main && git push upstream main --tags  # pushes to GitHub
+python -m build .  # Build the package
+twine upload dist/*  # Upload the package to PyPI
+```
+
+### Handling Javascript package version conflicts
+
+Unlike Python, Javascript packages can include more than one version of the same dependency.
+Usually the `yarn` package manager handles this okay, but occasionally you might end up with conflicting versions,
+or with unexpected package bloat.
+You can try to fix this by deduplicating dependencies:
+
+```bash
+jlpm yarn-deduplicate -s fewer
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,18 @@
-# Dask JupyterLab Extension [![Build Status](https://travis-ci.org/dask/dask-
+Metadata-Version: 2.1 Name: dask_labextension Version: 6.2.0 Summary: A
+JupyterLab extension for Dask. Home-page: https://github.com/dask/dask-
+labextension Author: Ian Rose, Matt Rocklin, Jacob Tomlinson License: BSD-3-
+Clause Keywords: dask,Jupyter,JupyterLab,JupyterLab3 Platform: Linux Platform:
+Mac OS X Platform: Windows Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python :: 3.6 Classifier:
+Programming Language :: Python :: 3.7 Classifier: Programming Language ::
+Python :: 3.8 Classifier: Framework :: Jupyter Requires-Python: >=3.6
+Description-Content-Type: text/markdown License-File: LICENSE # Dask JupyterLab
+Extension [![Build Status](https://travis-ci.org/dask/dask-
 labextension.svg?branch=main)](https://travis-ci.org/dask/dask-labextension) [!
 [Version](https://img.shields.io/npm/v/dask-labextension.svg)](https://
 www.npmjs.com/package/dask-labextension) [![Downloads](https://img.shields.io/
 npm/dm/dask-labextension.svg)](https://www.npmjs.com/package/dask-labextension)
 [![Dependencies](https://img.shields.io/librariesio/release/npm/dask-
 labextension.svg)](https://libraries.io/npm/dask-labextension) This package
 provides a JupyterLab extension to manage Dask clusters, as well as embed
@@ -74,17 +84,22 @@
 of the labextension you can run the following in this directory: ```bash jlpm #
 Install npm package dependencies jlpm build # Compile the TypeScript sources to
 Javascript jupyter labextension develop . --overwrite # Install the current
 directory as an extension ``` To rebuild the extension: ```bash jlpm build ```
 You should then be able to refresh the JupyterLab page and it will pick up the
 changes to the extension. To run an editable install of the server extension,
 run ```bash pip install -e . jupyter serverextension enable --sys-prefix
-dask_labextension ``` ## Publishing This application is distributed as two
-subpackages. The JupyterLab frontend part is published to [npm](https://
-www.npmjs.com/package/dask-labextension), and the server-side part to [PyPI]
-(https://pypi.org/project/dask-labextension/). Releases for both packages are
-done with the `jlpm` tool, `git` and Travis CI. _Note: Package versions are not
+dask_labextension ``` ## Publishing This extension contains a front-end
+component written in TypeScript and a back-end component written in Python. The
+front-end is compiled to Javascript during the build process and is distributed
+as static assets along with the Python package. _Note: Package versions are not
 prefixed with the letter `v`. You will need to disable this._ ```console $ jlpm
-config set version-tag-prefix "" ``` Making a release ```console $ jlpm version
-[--major|--minor|--patch] # updates package.json and creates git commit and tag
-$ git push upstream main && git push upstream main --tags # pushes tags to
-GitHub which triggers Travis CI to build and deploy ```
+config set version-tag-prefix "" ``` ### Release process This requires `node`,
+`build`, and `twine` to be installed. ```bash jlpm version [--major|--minor|--
+patch] # updates package.json and creates git commit and tag git push upstream
+main && git push upstream main --tags # pushes to GitHub python -m build . #
+Build the package twine upload dist/* # Upload the package to PyPI ``` ###
+Handling Javascript package version conflicts Unlike Python, Javascript
+packages can include more than one version of the same dependency. Usually the
+`yarn` package manager handles this okay, but occasionally you might end up
+with conflicting versions, or with unexpected package bloat. You can try to fix
+this by deduplicating dependencies: ```bash jlpm yarn-deduplicate -s fewer ```
```

### Comparing `dask_labextension-6.1.0/dask_labextension/__init__.py` & `dask_labextension-6.2.0/dask_labextension/__init__.py`

 * *Files identical despite different names*

### Comparing `dask_labextension-6.1.0/dask_labextension/clusterhandler.py` & `dask_labextension-6.2.0/dask_labextension/clusterhandler.py`

 * *Files identical despite different names*

### Comparing `dask_labextension-6.1.0/dask_labextension/dashboardhandler.py` & `dask_labextension-6.2.0/dask_labextension/dashboardhandler.py`

 * *Files identical despite different names*

### Comparing `dask_labextension-6.1.0/dask_labextension/labextension/package.json` & `dask_labextension-6.2.0/dask_labextension/labextension/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.969720179738562%*

 * *Differences: {"'devDependencies'": "{'yarn-deduplicate': '^5.0.0'}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.48341a7428463ba2c6bb.js'}}",*

 * * "'version'": "'6.2.0'"}*

```diff
@@ -41,26 +41,27 @@
         "eslint-plugin-react": "^7.21.5",
         "mkdirp": "^1.0.3",
         "mocha": "^6.2.0",
         "npm-run-all": "^4.1.5",
         "prettier": "^2.1.1",
         "rimraf": "^3.0.2",
         "typescript": "~4.1.3",
-        "yarn": "1.22.0"
+        "yarn": "1.22.0",
+        "yarn-deduplicate": "^5.0.0"
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "schema/*.json",
         "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/dask/dask-labextension",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.c559dc887be99a51d44a.js"
+            "load": "static/remoteEntry.48341a7428463ba2c6bb.js"
         },
         "extension": true,
         "outputDir": "dask_labextension/labextension",
         "schemaDir": "schema"
     },
     "keywords": [
         "dask",
@@ -97,9 +98,9 @@
         "prettier:check": "prettier --list-different '**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}'",
         "test": "mocha",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
     "types": "lib/index.d.ts",
-    "version": "6.1.0"
+    "version": "6.2.0"
 }
```

### Comparing `dask_labextension-6.1.0/dask_labextension/labextension/schemas/dask-labextension/package.json.orig` & `dask_labextension-6.2.0/dask_labextension/labextension/schemas/dask-labextension/package.json.orig`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9705882352941175%*

 * *Differences: {"'devDependencies'": "{'yarn-deduplicate': '^5.0.0'}", "'version'": "'6.2.0'"}*

```diff
@@ -41,15 +41,16 @@
         "eslint-plugin-react": "^7.21.5",
         "mkdirp": "^1.0.3",
         "mocha": "^6.2.0",
         "npm-run-all": "^4.1.5",
         "prettier": "^2.1.1",
         "rimraf": "^3.0.2",
         "typescript": "~4.1.3",
-        "yarn": "1.22.0"
+        "yarn": "1.22.0",
+        "yarn-deduplicate": "^5.0.0"
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "schema/*.json",
         "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/dask/dask-labextension",
@@ -93,9 +94,9 @@
         "prettier:check": "prettier --list-different '**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}'",
         "test": "mocha",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
     "types": "lib/index.d.ts",
-    "version": "6.1.0"
+    "version": "6.2.0"
 }
```

### Comparing `dask_labextension-6.1.0/dask_labextension/labextension/schemas/dask-labextension/plugin.json` & `dask_labextension-6.2.0/dask_labextension/labextension/schemas/dask-labextension/plugin.json`

 * *Files identical despite different names*

### Comparing `dask_labextension-6.1.0/dask_labextension/labextension/static/114.6d8f6f4a88afc2816496.js` & `dask_labextension-6.2.0/dask_labextension/labextension/static/114.f9e3bc980911cf750147.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -1,75 +1,75 @@
 "use strict";
 (self.webpackChunkdask_labextension = self.webpackChunkdask_labextension || []).push([
     [114], {
-        114: (e, t, n) => {
-            n.r(t), n.d(t, {
+        114: (t, e, n) => {
+            n.r(e), n.d(e, {
                 Debouncer: () => y,
                 Poll: () => f,
                 RateLimiter: () => d,
                 Throttler: () => m
             });
             var i = n(526),
                 r = n(840),
-                o = function(e, t) {
+                o = function(t, e) {
                     return o = Object.setPrototypeOf || {
                         __proto__: []
                     }
-                    instanceof Array && function(e, t) {
-                        e.__proto__ = t
-                    } || function(e, t) {
-                        for (var n in t) Object.prototype.hasOwnProperty.call(t, n) && (e[n] = t[n])
-                    }, o(e, t)
+                    instanceof Array && function(t, e) {
+                        t.__proto__ = e
+                    } || function(t, e) {
+                        for (var n in e) Object.prototype.hasOwnProperty.call(e, n) && (t[n] = e[n])
+                    }, o(t, e)
                 };
 
-            function a(e, t) {
-                if ("function" != typeof t && null !== t) throw new TypeError("Class extends value " + String(t) + " is not a constructor or null");
+            function a(t, e) {
+                if ("function" != typeof e && null !== e) throw new TypeError("Class extends value " + String(e) + " is not a constructor or null");
 
                 function n() {
-                    this.constructor = e
+                    this.constructor = t
                 }
-                o(e, t), e.prototype = null === t ? Object.create(t) : (n.prototype = t.prototype, new n)
+                o(t, e), t.prototype = null === e ? Object.create(e) : (n.prototype = e.prototype, new n)
             }
             var s = function() {
-                return s = Object.assign || function(e) {
-                    for (var t, n = 1, i = arguments.length; n < i; n++)
-                        for (var r in t = arguments[n]) Object.prototype.hasOwnProperty.call(t, r) && (e[r] = t[r]);
-                    return e
+                return s = Object.assign || function(t) {
+                    for (var e, n = 1, i = arguments.length; n < i; n++)
+                        for (var r in e = arguments[n]) Object.prototype.hasOwnProperty.call(e, r) && (t[r] = e[r]);
+                    return t
                 }, s.apply(this, arguments)
             };
 
-            function c(e, t, n, i) {
+            function c(t, e, n, i) {
                 return new(n || (n = Promise))((function(r, o) {
-                    function a(e) {
+                    function a(t) {
                         try {
-                            c(i.next(e))
-                        } catch (e) {
-                            o(e)
+                            c(i.next(t))
+                        } catch (t) {
+                            o(t)
                         }
                     }
 
-                    function s(e) {
+                    function s(t) {
                         try {
-                            c(i.throw(e))
-                        } catch (e) {
-                            o(e)
+                            c(i.throw(t))
+                        } catch (t) {
+                            o(t)
                         }
                     }
 
-                    function c(e) {
-                        var t;
-                        e.done ? r(e.value) : (t = e.value, t instanceof n ? t : new n((function(e) {
-                            e(t)
+                    function c(t) {
+                        var e;
+                        t.done ? r(t.value) : (e = t.value, e instanceof n ? e : new n((function(t) {
+                            t(e)
                         }))).then(a, s)
                     }
-                    c((i = i.apply(e, t || [])).next())
+                    c((i = i.apply(t, e || [])).next())
                 }))
             }
 
-            function u(e, t) {
+            function u(t, e) {
                 var n, i, r, o, a = {
                     label: 0,
                     sent: function() {
                         if (1 & r[0]) throw r[1];
                         return r[1]
                     },
                     trys: [],
@@ -121,17 +121,17 @@
                                         if (r && a.label < r[2]) {
                                             a.label = r[2], a.ops.push(o);
                                             break
                                         }
                                         r[2] && a.ops.pop(), a.trys.pop();
                                         continue
                                 }
-                                o = t.call(e, a)
-                            } catch (e) {
-                                o = [6, e], i = 0
+                                o = e.call(t, a)
+                            } catch (t) {
+                                o = [6, t], i = 0
                             } finally {
                                 n = r = 0
                             }
                             if (5 & o[0]) throw o[1];
                             return {
                                 value: o[0] ? o[1] : void 0,
                                 done: !0
@@ -139,250 +139,248 @@
                         }([o, s])
                     }
                 }
             }
             var l, p = "function" == typeof requestAnimationFrame ? requestAnimationFrame : setImmediate,
                 h = "function" == typeof cancelAnimationFrame ? cancelAnimationFrame : clearImmediate,
                 f = function() {
-                    function e(e) {
-                        var t = this;
-                        this._disposed = new r.Signal(this), this._tick = new i.PromiseDelegate, this._ticked = new r.Signal(this), this._timeout = -1, this._factory = e.factory, this._standby = e.standby || l.DEFAULT_STANDBY, this._state = s(s({}, l.DEFAULT_STATE), {
+                    function t(t) {
+                        var e = this;
+                        this._disposed = new r.Signal(this), this._tick = new i.PromiseDelegate, this._ticked = new r.Signal(this), this._timeout = -1, this._factory = t.factory, this._standby = t.standby || l.DEFAULT_STANDBY, this._state = s(s({}, l.DEFAULT_STATE), {
                             timestamp: (new Date).getTime()
                         });
-                        var n = e.frequency || {},
+                        var n = t.frequency || {},
                             o = Math.max(n.interval || 0, n.max || 0, l.DEFAULT_FREQUENCY.max);
                         this.frequency = s(s(s({}, l.DEFAULT_FREQUENCY), n), {
                             max: o
-                        }), this.name = e.name || l.DEFAULT_NAME, "auto" in e && !e.auto || p((function() {
-                            t.start()
+                        }), this.name = t.name || l.DEFAULT_NAME, "auto" in t && !t.auto || p((function() {
+                            e.start()
                         }))
                     }
-                    return Object.defineProperty(e.prototype, "disposed", {
+                    return Object.defineProperty(t.prototype, "disposed", {
                         get: function() {
                             return this._disposed
                         },
                         enumerable: !0,
                         configurable: !0
-                    }), Object.defineProperty(e.prototype, "frequency", {
+                    }), Object.defineProperty(t.prototype, "frequency", {
                         get: function() {
                             return this._frequency
                         },
-                        set: function(t) {
-                            if (!this.isDisposed && !i.JSONExt.deepEqual(t, this.frequency || {})) {
-                                var n = t.backoff,
-                                    r = t.interval,
-                                    o = t.max;
+                        set: function(e) {
+                            if (!this.isDisposed && !i.JSONExt.deepEqual(e, this.frequency || {})) {
+                                var n = e.backoff,
+                                    r = e.interval,
+                                    o = e.max;
                                 if (r = Math.round(r), o = Math.round(o), "number" == typeof n && n < 1) throw new Error("Poll backoff growth factor must be at least 1");
-                                if ((r < 0 || r > o) && r !== e.NEVER) throw new Error("Poll interval must be between 0 and max");
-                                if (o > e.MAX_INTERVAL && o !== e.NEVER) throw new Error("Max interval must be less than " + e.MAX_INTERVAL);
+                                if ((r < 0 || r > o) && r !== t.NEVER) throw new Error("Poll interval must be between 0 and max");
+                                if (o > t.MAX_INTERVAL && o !== t.NEVER) throw new Error("Max interval must be less than " + t.MAX_INTERVAL);
                                 this._frequency = {
                                     backoff: n,
                                     interval: r,
                                     max: o
                                 }
                             }
                         },
                         enumerable: !0,
                         configurable: !0
-                    }), Object.defineProperty(e.prototype, "isDisposed", {
+                    }), Object.defineProperty(t.prototype, "isDisposed", {
                         get: function() {
                             return "disposed" === this.state.phase
                         },
                         enumerable: !0,
                         configurable: !0
-                    }), Object.defineProperty(e.prototype, "standby", {
+                    }), Object.defineProperty(t.prototype, "standby", {
                         get: function() {
                             return this._standby
                         },
-                        set: function(e) {
-                            this.isDisposed || this.standby === e || (this._standby = e)
+                        set: function(t) {
+                            this.isDisposed || this.standby === t || (this._standby = t)
                         },
                         enumerable: !0,
                         configurable: !0
-                    }), Object.defineProperty(e.prototype, "state", {
+                    }), Object.defineProperty(t.prototype, "state", {
                         get: function() {
                             return this._state
                         },
                         enumerable: !0,
                         configurable: !0
-                    }), Object.defineProperty(e.prototype, "tick", {
+                    }), Object.defineProperty(t.prototype, "tick", {
                         get: function() {
                             return this._tick.promise
                         },
                         enumerable: !0,
                         configurable: !0
-                    }), Object.defineProperty(e.prototype, "ticked", {
+                    }), Object.defineProperty(t.prototype, "ticked", {
                         get: function() {
                             return this._ticked
                         },
                         enumerable: !0,
                         configurable: !0
-                    }), e.prototype.dispose = function() {
+                    }), t.prototype.dispose = function() {
                         this.isDisposed || (this._state = s(s({}, l.DISPOSED_STATE), {
                             timestamp: (new Date).getTime()
-                        }), this._tick.promise.catch((function(e) {})), this._tick.reject(new Error("Poll (" + this.name + ") is disposed.")), this._disposed.emit(void 0), r.Signal.clearData(this))
-                    }, e.prototype.refresh = function() {
+                        }), this._tick.promise.catch((function(t) {})), this._tick.reject(new Error("Poll (" + this.name + ") is disposed.")), this._disposed.emit(void 0), r.Signal.clearData(this))
+                    }, t.prototype.refresh = function() {
                         return this.schedule({
-                            cancel: function(e) {
-                                return "refreshed" === e.phase
+                            cancel: function(t) {
+                                return "refreshed" === t.phase
                             },
-                            interval: e.IMMEDIATE,
+                            interval: t.IMMEDIATE,
                             phase: "refreshed"
                         })
-                    }, e.prototype.schedule = function(t) {
-                        return void 0 === t && (t = {}), c(this, void 0, void 0, (function() {
+                    }, t.prototype.schedule = function(e) {
+                        return void 0 === e && (e = {}), c(this, void 0, void 0, (function() {
                             var n, r, o, a, c, l = this;
                             return u(this, (function(u) {
                                 switch (u.label) {
                                     case 0:
-                                        return this.isDisposed || t.cancel && t.cancel(this.state) ? [2] : (n = this.state, r = this._tick, o = new i.PromiseDelegate, a = s({
+                                        return this.isDisposed || e.cancel && e.cancel(this.state) ? [2] : (n = this.state, r = this._tick, o = new i.PromiseDelegate, a = s({
                                             interval: this.frequency.interval,
                                             payload: null,
                                             phase: "standby",
                                             timestamp: (new Date).getTime()
-                                        }, t), this._state = a, this._tick = o, n.interval === e.IMMEDIATE ? h(this._timeout) : clearTimeout(this._timeout), this._ticked.emit(this.state), r.resolve(this), [4, r.promise]);
+                                        }, e), this._state = a, this._tick = o, n.interval === t.IMMEDIATE ? h(this._timeout) : clearTimeout(this._timeout), this._ticked.emit(this.state), r.resolve(this), [4, r.promise]);
                                     case 1:
                                         return u.sent(), c = function() {
                                             l.isDisposed || l.tick !== o.promise || l._execute()
-                                        }, this._timeout = a.interval === e.IMMEDIATE ? p(c) : a.interval === e.NEVER ? -1 : setTimeout(c, a.interval), [2]
+                                        }, this._timeout = a.interval === t.IMMEDIATE ? p(c) : a.interval === t.NEVER ? -1 : setTimeout(c, a.interval), [2]
                                 }
                             }))
                         }))
-                    }, e.prototype.start = function() {
+                    }, t.prototype.start = function() {
                         return this.schedule({
-                            cancel: function(e) {
-                                var t = e.phase;
-                                return "constructed" !== t && "standby" !== t && "stopped" !== t
+                            cancel: function(t) {
+                                var e = t.phase;
+                                return "constructed" !== e && "standby" !== e && "stopped" !== e
                             },
-                            interval: e.IMMEDIATE,
+                            interval: t.IMMEDIATE,
                             phase: "started"
                         })
-                    }, e.prototype.stop = function() {
+                    }, t.prototype.stop = function() {
                         return this.schedule({
-                            cancel: function(e) {
-                                return "stopped" === e.phase
+                            cancel: function(t) {
+                                return "stopped" === t.phase
                             },
-                            interval: e.NEVER,
+                            interval: t.NEVER,
                             phase: "stopped"
                         })
-                    }, e.prototype._execute = function() {
-                        var e = this,
-                            t = "function" == typeof this.standby ? this.standby() : this.standby;
-                        if (t = "never" !== t && ("when-hidden" === t ? !("undefined" == typeof document || !document || !document.hidden) : t)) this.schedule();
+                    }, t.prototype._execute = function() {
+                        var t = this,
+                            e = "function" == typeof this.standby ? this.standby() : this.standby;
+                        if (e = "never" !== e && ("when-hidden" === e ? !("undefined" == typeof document || !document || !document.hidden) : e)) this.schedule();
                         else {
                             var n = this.tick;
-                            this._factory(this.state).then((function(t) {
-                                e.isDisposed || e.tick !== n || e.schedule({
-                                    payload: t,
-                                    phase: "rejected" === e.state.phase ? "reconnected" : "resolved"
+                            this._factory(this.state).then((function(e) {
+                                t.isDisposed || t.tick !== n || t.schedule({
+                                    payload: e,
+                                    phase: "rejected" === t.state.phase ? "reconnected" : "resolved"
                                 })
-                            })).catch((function(t) {
-                                e.isDisposed || e.tick !== n || e.schedule({
-                                    interval: l.sleep(e.frequency, e.state),
-                                    payload: t,
+                            })).catch((function(e) {
+                                t.isDisposed || t.tick !== n || t.schedule({
+                                    interval: l.sleep(t.frequency, t.state),
+                                    payload: e,
                                     phase: "rejected"
                                 })
                             }))
                         }
-                    }, e
+                    }, t
                 }();
-            ! function(e) {
-                e.IMMEDIATE = 0, e.MAX_INTERVAL = 2147483647, e.NEVER = 1 / 0
+            ! function(t) {
+                t.IMMEDIATE = 0, t.MAX_INTERVAL = 2147483647, t.NEVER = 1 / 0
             }(f || (f = {})),
-            function(e) {
-                e.DEFAULT_BACKOFF = 3, e.DEFAULT_FREQUENCY = {
+            function(t) {
+                t.DEFAULT_BACKOFF = 3, t.DEFAULT_FREQUENCY = {
                     backoff: !0,
                     interval: 1e3,
                     max: 3e4
-                }, e.DEFAULT_NAME = "unknown", e.DEFAULT_STANDBY = "when-hidden", e.DEFAULT_STATE = {
+                }, t.DEFAULT_NAME = "unknown", t.DEFAULT_STANDBY = "when-hidden", t.DEFAULT_STATE = {
                     interval: f.NEVER,
                     payload: null,
                     phase: "constructed",
                     timestamp: new Date(0).getTime()
-                }, e.DISPOSED_STATE = {
+                }, t.DISPOSED_STATE = {
                     interval: f.NEVER,
                     payload: null,
                     phase: "disposed",
                     timestamp: new Date(0).getTime()
-                }, e.sleep = function(t, n) {
-                    var i = t.backoff,
-                        r = t.interval,
-                        o = t.max;
+                }, t.sleep = function(e, n) {
+                    var i = e.backoff,
+                        r = e.interval,
+                        o = e.max;
                     if (r === f.NEVER) return r;
-                    var a = !0 === i ? e.DEFAULT_BACKOFF : !1 === i ? 1 : i,
-                        s = function(e, t) {
-                            return e = Math.ceil(e), t = Math.floor(t), Math.floor(Math.random() * (t - e + 1)) + e
+                    var a = !0 === i ? t.DEFAULT_BACKOFF : !1 === i ? 1 : i,
+                        s = function(t, e) {
+                            return t = Math.ceil(t), e = Math.floor(e), Math.floor(Math.random() * (e - t + 1)) + t
                         }(r, n.interval * a);
                     return Math.min(o, s)
                 }
             }(l || (l = {}));
             var d = function() {
-                    function e(e, t) {
+                    function t(t, e) {
                         var n = this;
-                        void 0 === t && (t = 500), this.payload = null, this.limit = t, this.poll = new f({
+                        void 0 === e && (e = 500), this.args = void 0, this.payload = null, this.limit = e, this.poll = new f({
                             auto: !1,
                             factory: function() {
                                 return c(n, void 0, void 0, (function() {
-                                    return u(this, (function(t) {
-                                        switch (t.label) {
-                                            case 0:
-                                                return [4, e()];
-                                            case 1:
-                                                return [2, t.sent()]
-                                        }
+                                    var e;
+                                    return u(this, (function(n) {
+                                        return e = this.args, this.args = void 0, [2, t.apply(void 0, e)]
                                     }))
                                 }))
                             },
                             frequency: {
                                 backoff: !1,
                                 interval: f.NEVER,
                                 max: f.NEVER
                             },
                             standby: "never"
-                        }), this.payload = new i.PromiseDelegate, this.poll.ticked.connect((function(e, t) {
+                        }), this.payload = new i.PromiseDelegate, this.poll.ticked.connect((function(t, e) {
                             var r = n.payload;
-                            return "resolved" === t.phase ? (n.payload = new i.PromiseDelegate, void r.resolve(t.payload)) : "rejected" === t.phase || "stopped" === t.phase ? (n.payload = new i.PromiseDelegate, r.promise.catch((function(e) {})), void r.reject(t.payload)) : void 0
+                            return "resolved" === e.phase ? (n.payload = new i.PromiseDelegate, void r.resolve(e.payload)) : "rejected" === e.phase || "stopped" === e.phase ? (n.payload = new i.PromiseDelegate, r.promise.catch((function(t) {})), void r.reject(e.payload)) : void 0
                         }), this)
                     }
-                    return Object.defineProperty(e.prototype, "isDisposed", {
+                    return Object.defineProperty(t.prototype, "isDisposed", {
                         get: function() {
                             return null === this.payload
                         },
                         enumerable: !0,
                         configurable: !0
-                    }), e.prototype.dispose = function() {
-                        this.isDisposed || (this.payload = null, this.poll.dispose())
-                    }, e.prototype.stop = function() {
+                    }), t.prototype.dispose = function() {
+                        this.isDisposed || (this.args = void 0, this.payload = null, this.poll.dispose())
+                    }, t.prototype.stop = function() {
                         return c(this, void 0, void 0, (function() {
-                            return u(this, (function(e) {
+                            return u(this, (function(t) {
                                 return [2, this.poll.stop()]
                             }))
                         }))
-                    }, e
+                    }, t
                 }(),
-                y = function(e) {
-                    function t() {
-                        return null !== e && e.apply(this, arguments) || this
+                y = function(t) {
+                    function e() {
+                        return null !== t && t.apply(this, arguments) || this
                     }
-                    return a(t, e), t.prototype.invoke = function() {
-                        return this.poll.schedule({
+                    return a(e, t), e.prototype.invoke = function() {
+                        for (var t = [], e = 0; e < arguments.length; e++) t[e] = arguments[e];
+                        return this.args = t, this.poll.schedule({
                             interval: this.limit,
                             phase: "invoked"
                         }), this.payload.promise
-                    }, t
+                    }, e
                 }(d),
-                m = function(e) {
-                    function t(t, n) {
-                        var i = e.call(this, t, "number" == typeof n ? n : n && n.limit) || this,
-                            r = "leading";
-                        return "number" != typeof n && (r = "edge" in (n = n || {}) ? n.edge : r), i._interval = "trailing" === r ? i.limit : f.IMMEDIATE, i
+                m = function(t) {
+                    function e(e, n) {
+                        var i = t.call(this, e, "number" == typeof n ? n : n && n.limit) || this;
+                        return i._trailing = !1, "number" != typeof n && n && "trailing" === n.edge && (i._trailing = !0), i._interval = i._trailing ? i.limit : f.IMMEDIATE, i
                     }
-                    return a(t, e), t.prototype.invoke = function() {
-                        return "invoked" !== this.poll.state.phase && this.poll.schedule({
+                    return a(e, t), e.prototype.invoke = function() {
+                        for (var t = [], e = 0; e < arguments.length; e++) t[e] = arguments[e];
+                        var n = "invoked" !== this.poll.state.phase;
+                        return (n || this._trailing) && (this.args = t), n && this.poll.schedule({
                             interval: this._interval,
                             phase: "invoked"
                         }), this.payload.promise
-                    }, t
+                    }, e
                 }(d)
         }
     }
 ]);
```

### Comparing `dask_labextension-6.1.0/dask_labextension/labextension/static/319.3ff908a63582f9623f31.js` & `dask_labextension-6.2.0/dask_labextension/labextension/static/224.86c44b816becca807a99.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,32 +1,33 @@
 (self.webpackChunkdask_labextension = self.webpackChunkdask_labextension || []).push([
-    [319], {
-        319: (e, t, n) => {
+    [224], {
+        224: (e, t, n) => {
             "use strict";
             n.r(t), n.d(t, {
-                default: () => W
+                DaskIcon: () => F,
+                default: () => z
             });
-            var s, a = n(866),
-                i = n(510),
-                r = n(468),
-                o = n(705),
-                l = n(598),
-                d = n(397),
-                c = n(767),
-                u = n(918),
-                h = n(840),
-                m = n(886),
-                p = n(258),
-                g = n(591),
+            var s, a = n(638),
+                i = n(303),
+                r = n(745),
+                o = n(543),
+                l = n(535),
+                d = n(299),
+                c = n(548),
+                u = n(127),
+                h = n(918),
+                m = n(840),
+                p = n(344),
+                g = n(139),
                 v = n(526),
                 C = n(358),
-                f = n(431),
+                f = n(832),
                 b = n(271),
                 k = n(456);
-            class _ extends i.MainAreaWidget {
+            class w extends i.MainAreaWidget {
                 constructor() {
                     super({
                         content: new i.IFrame({
                             sandbox: ["allow-scripts", "allow-same-origin"]
                         })
                     }), this._item = null, this._dashboardUrl = "", this._active = !1, this._inactivePanel = s.createInactivePanel(), this.content.node.appendChild(this._inactivePanel), this.addClass("dask-DaskDashboard-widget"), this.update()
                 }
@@ -46,57 +47,57 @@
                     return this._active
                 }
                 set active(e) {
                     e !== this._active && (this._active = e, this.update())
                 }
                 onUpdateRequest() {
                     if (!this.item || !this.dashboardUrl || !this.active) return this.content.url = "", void(this._inactivePanel.style.display = "");
-                    this._inactivePanel.style.display = "none", this.content.url = m.URLExt.join(this.dashboardUrl, this.item.route)
+                    this._inactivePanel.style.display = "none", this.content.url = p.URLExt.join(this.dashboardUrl, this.item.route)
                 }
             }
             class y extends f.Widget {
                 constructor(e) {
                     super();
                     let t = this.layout = new f.PanelLayout;
-                    this._dashboard = new f.Widget, this._serverSettings = p.ServerConnection.makeSettings(), this._input = new w(this._serverSettings, e.linkFinder), t.addWidget(this._input), t.addWidget(this._dashboard), this.addClass("dask-DaskDashboardLauncher"), this._items = e.items || [], this._launchItem = e.launchItem, this._input.urlInfoChanged.connect(this._updateLinks, this)
+                    this._dashboard = new f.Widget, this._serverSettings = g.ServerConnection.makeSettings(), this._input = new _(this._serverSettings, e.linkFinder), t.addWidget(this._input), t.addWidget(this._dashboard), this.addClass("dask-DaskDashboardLauncher"), this._items = e.items || [], this._launchItem = e.launchItem, this._input.urlInfoChanged.connect(this._updateLinks, this)
                 }
                 _updateLinks(e, t) {
                     if (!t.newValue.isActive) return void this.update();
                     const n = s.getDashboardPlots(t.newValue);
                     this._items = n, this.update()
                 }
                 get items() {
                     return this._items
                 }
                 get input() {
                     return this._input
                 }
                 onUpdateRequest() {
-                    this.isVisible && k.render(b.createElement(L, {
+                    this.isVisible && k.render(b.createElement(x, {
                         launchItem: this._launchItem,
                         isEnabled: this.input.urlInfo.isActive,
                         items: this._items
                     }), this._dashboard.node)
                 }
                 onAfterShow() {
                     this.update()
                 }
             }
-            class w extends f.Widget {
+            class _ extends f.Widget {
                 constructor(e, t) {
-                    super(), this._urlChanged = new h.Signal(this), this._urlInfo = {
+                    super(), this._urlChanged = new m.Signal(this), this._urlInfo = {
                         isActive: !1,
                         url: "",
                         plots: {}
                     }, this._browserDashboardCheck = !1, this.addClass("dask-URLInput");
                     const n = this.layout = new f.PanelLayout,
                         s = new f.Widget;
                     if (s.addClass("dask-URLInput-wrapper"), this._input = document.createElement("input"), this._input.placeholder = "DASK DASHBOARD URL", s.node.appendChild(this._input), n.addWidget(s), this._serverSettings = e, t) {
                         const e = new i.ToolbarButton({
-                            icon: g.searchIcon,
+                            icon: r.searchIcon,
                             onClick: async () => {
                                 let e = await t();
                                 e && (this.url = e)
                             },
                             tooltip: "Auto-detect dashboard URL"
                         });
                         n.addWidget(e)
@@ -157,15 +158,15 @@
                             max: 12e4
                         },
                         standby: "when-hidden"
                     }), this._urlChanged.connect((() => this._poll.refresh()), this)
                 }
             }
 
-            function L(e) {
+            function x(e) {
                 if (!e.isEnabled) return b.createElement("div", {
                     className: "dask-DashboardListing-inactive"
                 }, b.createElement("span", {
                     className: "dask-DashboardListing-inactive-title"
                 }, "Dashboard not connected"), b.createElement("span", {
                     className: "dask-DashboardListing-inactive-detail"
                 }, "To connect, paste a dashboard URL in the box above, or create a new Dask cluster with the cluster manager below. If you are still unable to connect, check your network setup."));
@@ -180,25 +181,25 @@
                 }, t.label))));
                 return b.createElement("div", null, b.createElement("ul", {
                     className: "dask-DashboardListing-list"
                 }, t))
             }! function(e) {
                 function t(e, t = "") {
                     if (n(e)) {
-                        t || (t = m.PageConfig.getBaseUrl());
+                        t || (t = p.PageConfig.getBaseUrl());
                         const n = new URL(t);
                         e.startsWith(n.pathname) && (e = e.slice(n.pathname.length)), e = t + e
                     }
-                    return e.endsWith("status") ? e = e.slice(0, -"status".length) : e.endsWith("status/") && (e = e.slice(0, -"status/".length)), e
+                    return e.endsWith("status") ? e = e.slice(0, -6) : e.endsWith("status/") && (e = e.slice(0, -7)), e
                 }
 
                 function n(e) {
                     const {
                         protocol: t
-                    } = m.URLExt.parse(e);
+                    } = p.URLExt.parse(e);
                     return 0 !== e.toLowerCase().indexOf(t) && 0 !== e.indexOf("//")
                 }
                 e.normalizeDashboardUrl = t, e.getDashboardPlots = function(e) {
                     const t = [];
                     for (let n in e.plots) {
                         const s = n.replace("Individual ", ""),
                             a = {
@@ -206,15 +207,15 @@
                                 label: s,
                                 key: s
                             };
                         t.push(a)
                     }
                     return t
                 }, e.testDaskDashboard = async function(e, n, s = !1) {
-                    if (0 === (e = t(e, n.baseUrl)).indexOf(n.baseUrl)) return p.ServerConnection.makeRequest(m.URLExt.join(e, "individual-plots.json"), {}, n).then((async t => {
+                    if (0 === (e = t(e, n.baseUrl)).indexOf(n.baseUrl)) return g.ServerConnection.makeRequest(p.URLExt.join(e, "individual-plots.json"), {}, n).then((async t => {
                         if (200 === t.status) {
                             const n = await t.json();
                             return {
                                 url: e,
                                 isActive: !0,
                                 plots: n
                             }
@@ -225,15 +226,15 @@
                             plots: {}
                         }
                     })).catch((() => ({
                         url: e,
                         isActive: !1,
                         plots: {}
                     })));
-                    if (s) return fetch(m.URLExt.join(e, "individual-plots.json")).then((async t => {
+                    if (s) return fetch(p.URLExt.join(e, "individual-plots.json")).then((async t => {
                         if (200 === t.status) {
                             const n = await t.json();
                             return {
                                 url: e,
                                 isActive: !0,
                                 plots: n
                             }
@@ -244,22 +245,22 @@
                             plots: {}
                         }
                     })).catch((() => ({
                         url: e,
                         isActive: !1,
                         plots: {}
                     })));
-                    const a = await p.ServerConnection.makeRequest(m.URLExt.join(n.baseUrl, "dask", "dashboard-check", encodeURIComponent(e)), {}, n);
+                    const a = await g.ServerConnection.makeRequest(p.URLExt.join(n.baseUrl, "dask", "dashboard-check", encodeURIComponent(e)), {}, n);
                     return await a.json()
                 }, e.createInactivePanel = function() {
                     const e = document.createElement("div");
                     return e.className = "dask-DaskDashboard-inactive", e
                 }, e.isLocal = n
             }(s || (s = {}));
-            var x, I = n(520),
+            var L, I = n(520),
                 E = n(694);
             class D extends b.Component {
                 constructor(e) {
                     let t;
                     super(e);
                     const n = !!e.initialModel.adapt;
                     t = n ? e.initialModel : {
@@ -384,32 +385,32 @@
                             this.onMaximumChanged(e)
                         }
                     }))))
                 }
             }
             class S extends f.Widget {
                 constructor(e) {
-                    super(), this._dragData = null, this._clusters = [], this._activeClusterChanged = new h.Signal(this), this._failedServerChecks = 0, this._hasServer = !1, this._isReady = !0, this.addClass("dask-DaskClusterManager"), this._serverSettings = p.ServerConnection.makeSettings(), this._injectClientCodeForCluster = e.injectClientCodeForCluster, this._getClientCodeForCluster = e.getClientCodeForCluster, this._registry = e.registry, this._launchClusterId = e.launchClusterId, this._setActiveById = t => {
+                    super(), this._dragData = null, this._clusters = [], this._activeClusterChanged = new m.Signal(this), this._failedServerChecks = 0, this._hasServer = !1, this._isReady = !0, this.addClass("dask-DaskClusterManager"), this._serverSettings = g.ServerConnection.makeSettings(), this._injectClientCodeForCluster = e.injectClientCodeForCluster, this._getClientCodeForCluster = e.getClientCodeForCluster, this._registry = e.registry, this._launchClusterId = e.launchClusterId, this._setActiveById = t => {
                         const n = this._clusters.find((e => e.id === t));
                         if (!n) return;
-                        const s = m.URLExt.join(this._serverSettings.baseUrl, "proxy"),
+                        const s = p.URLExt.join(this._serverSettings.baseUrl, "proxy"),
                             a = new URL(s).pathname; - 1 !== n.dashboard_link.indexOf(a) ? e.setDashboardUrl(n.dashboard_link) : e.setDashboardUrl(`dask/dashboard/${n.id}`);
                         const i = this._activeCluster;
                         i && i.id === n.id || (this._activeCluster = n, this._activeClusterChanged.emit({
                             name: "cluster",
                             oldValue: i,
                             newValue: n
                         }), this.update())
                     };
                     const t = this.layout = new f.PanelLayout;
                     this._clusterListing = new f.Widget, this._clusterListing.addClass("dask-ClusterListing");
                     const n = new i.Toolbar,
                         s = new f.Widget;
                     s.node.textContent = "CLUSTERS", s.addClass("dask-DaskClusterManager-label"), n.addItem("label", s), n.addItem("refresh", new i.ToolbarButton({
-                        icon: g.refreshIcon,
+                        icon: r.refreshIcon,
                         onClick: async () => this._updateClusterList(),
                         tooltip: "Refresh Cluster List"
                     })), n.addItem(this._launchClusterId, new i.CommandToolbarButton({
                         commands: this._registry,
                         id: this._launchClusterId
                     })), t.addWidget(n), t.addWidget(this._clusterListing), this._updateClusterList(), this._poll = new C.Poll({
                         factory: async () => {
@@ -511,15 +512,15 @@
                     let n = Math.abs(e.clientX - t.pressX),
                         s = Math.abs(e.clientY - t.pressY);
                     (n >= 5 || s >= 5) && (e.preventDefault(), e.stopPropagation(), this._startDrag(t.index, e.clientX, e.clientY))
                 }
                 async _startDrag(e, t, n) {
                     const s = this._clusters[e],
                         a = this._clusterListing.node.querySelector(`li.dask-ClusterListingItem[data-cluster-id="${s.id}"]`),
-                        i = x.createDragImage(a);
+                        i = L.createDragImage(a);
                     this._drag = new E.Drag({
                         mimeData: new v.MimeData,
                         dragImage: i,
                         supportedActions: "copy",
                         proposedAction: "copy",
                         source: this
                     });
@@ -534,41 +535,41 @@
                     }];
                     return this._drag.mimeData.setData("application/vnd.jupyter.cells", o), document.removeEventListener("mousemove", this, !0), document.removeEventListener("mouseup", this, !0), this._drag.start(t, n).then((e => {
                         this.isDisposed || (this._drag = null, this._dragData = null)
                     }))
                 }
                 async _launchCluster() {
                     this._isReady = !1, this._registry.notifyCommandChanged(this._launchClusterId);
-                    const e = await p.ServerConnection.makeRequest(`${this._serverSettings.baseUrl}dask/clusters`, {
+                    const e = await g.ServerConnection.makeRequest(`${this._serverSettings.baseUrl}dask/clusters`, {
                         method: "PUT"
                     }, this._serverSettings);
                     if (200 !== e.status) {
                         const t = await e.json();
                         throw (0, i.showErrorMessage)("Cluster Start Error", t), this._isReady = !0, this._registry.notifyCommandChanged(this._launchClusterId), t
                     }
                     const t = await e.json();
                     return await this._updateClusterList(), this._isReady = !0, this._registry.notifyCommandChanged(this._launchClusterId), t
                 }
                 async _updateClusterList() {
-                    const e = await p.ServerConnection.makeRequest(`${this._serverSettings.baseUrl}dask/clusters`, {}, this._serverSettings);
+                    const e = await g.ServerConnection.makeRequest(`${this._serverSettings.baseUrl}dask/clusters`, {}, this._serverSettings);
                     if (200 !== e.status) {
                         this._failedServerChecks++;
                         const e = new Error("Failed to list Dask clusters: might the server extension not be installed/enabled?");
                         throw this._hasServer || 5 != this._failedServerChecks || (0, i.showErrorMessage)("Dask Server Error", e), e
                     }
                     this._hasServer = !0;
                     const t = await e.json();
                     if (this._clusters = t, !this._clusters.find((e => e.id === (this._activeCluster && this._activeCluster.id)))) {
                         const e = this._clusters[0] && this._clusters[0].id || "";
                         this._setActiveById(e)
                     }
                     this.update()
                 }
                 async _stopById(e) {
-                    const t = await p.ServerConnection.makeRequest(`${this._serverSettings.baseUrl}dask/clusters/${e}`, {
+                    const t = await g.ServerConnection.makeRequest(`${this._serverSettings.baseUrl}dask/clusters/${e}`, {
                         method: "DELETE"
                     }, this._serverSettings);
                     if (204 !== t.status) {
                         const e = await t.json();
                         throw (0, i.showErrorMessage)("Failed to close cluster", e), e
                     }
                     await this._updateClusterList()
@@ -591,28 +592,28 @@
                             }),
                             buttons: [i.Dialog.cancelButton(), i.Dialog.okButton({
                                 label: "SCALE"
                             })]
                         }).then((n => n.button.accept ? t : e))
                     }(t);
                     if (v.JSONExt.deepEqual(n, t)) return Promise.resolve(t);
-                    const s = await p.ServerConnection.makeRequest(`${this._serverSettings.baseUrl}dask/clusters/${e}`, {
+                    const s = await g.ServerConnection.makeRequest(`${this._serverSettings.baseUrl}dask/clusters/${e}`, {
                         method: "PATCH",
                         body: JSON.stringify(n)
                     }, this._serverSettings);
                     if (200 !== s.status) {
                         const e = await s.json();
                         throw (0, i.showErrorMessage)("Failed to scale cluster", e), e
                     }
                     const a = await s.json();
                     return await this._updateClusterList(), a
                 }
                 _findCluster(e) {
                     const t = Array.from(this.node.querySelectorAll("li.dask-ClusterListingItem"));
-                    return u.ArrayExt.findFirstIndex(t, (t => I.ElementExt.hitTest(t, e.clientX, e.clientY)))
+                    return h.ArrayExt.findFirstIndex(t, (t => I.ElementExt.hitTest(t, e.clientX, e.clientY)))
                 }
             }
 
             function j(e) {
                 let t = e.clusters.map((t => b.createElement(M, {
                     isActive: t.id === e.activeClusterId,
                     key: t.id,
@@ -686,15 +687,15 @@
                     title: `Shutdown ${t.name}`
                 }, "SHUTDOWN")))
             }! function(e) {
                 e.createDragImage = function(e) {
                     const t = e.cloneNode(!0);
                     return t.classList.add("dask-ClusterListingItem-drag"), t
                 }
-            }(x || (x = {}));
+            }(L || (L = {}));
             class U extends f.Widget {
                 constructor(e) {
                     super(), this.addClass("dask-DaskSidebar");
                     let t = this.layout = new f.PanelLayout;
                     this._dashboard = new y({
                         launchItem: e.launchDashboardItem,
                         linkFinder: e.linkFinder
@@ -714,52 +715,57 @@
                 get dashboardLauncher() {
                     return this._dashboard
                 }
                 get clusterManager() {
                     return this._clusters
                 }
             }
-            var A, N = n(379),
-                R = n.n(N),
-                B = n(760);
-            R()(B.Z, {
-                    insert: "head",
-                    singleton: !1
-                }), B.Z.locals,
-                function(e) {
-                    e.launchPanel = "dask:launch-dashboard", e.launchLayout = "dask:launch-layout", e.populateDashboardUrl = "dask:populate-dashboard-url", e.populateAndLaunchLayout = "dask:populate-and-launch-layout", e.injectClientCode = "dask:inject-client-code", e.launchCluster = "dask:launch-cluster", e.stopCluster = "dask:stop-cluster", e.scaleCluster = "dask:scale-cluster", e.toggleAutoStartClient = "dask:toggle-auto-start-client"
-                }(A || (A = {}));
+            var A = n(379),
+                N = n.n(A),
+                R = n(760);
+            N()(R.Z, {
+                insert: "head",
+                singleton: !1
+            }), R.Z.locals;
+            const F = new r.LabIcon({
+                name: "dask:icon",
+                svgstr: '<?xml version="1.0" encoding="utf-8"?>\n\x3c!-- Generator: Adobe Illustrator 26.0.3, SVG Export Plug-In . SVG Version: 6.00 Build 0)  --\x3e\n<svg version="1.1" id="Layer_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" x="0px" y="0px"\n\t viewBox="0 0 512 512" style="enable-background:new 0 0 512 512;" xml:space="preserve">\n<style type="text/css">\n\t.st0{fill:#FFC11E;}\n\t.st1{fill:#04255C;}\n\t.st2{fill:#FC6E6B;}\n\t.st3{fill:#FFFFFF;}\n\t.st4{fill:#EF1161;}\n</style>\n<g>\n\t<path class="st0" d="M143.71,157.61l126.5-72.99c1.25-0.72,2.02-2.05,2.02-3.5l0.01-43.77c0-6.48-2.66-12.9-7.83-16.81\n\t\tc-6.69-5.06-15.28-5.56-22.33-1.48L65.13,121.17c-6.22,3.59-10.06,10.23-10.06,17.41L55,369.18c0,6.47,2.65,12.89,7.81,16.81\n\t\tc6.68,5.07,15.29,5.57,22.35,1.49l37.48-21.62c1.25-0.72,2.02-2.05,2.02-3.5l0.05-171.85C124.71,176.93,131.95,164.4,143.71,157.61\n\t\tz"/>\n\t<path class="st4" d="M446.95,124.53c-3.15-1.82-6.61-2.73-10.06-2.73c-3.45,0-6.9,0.91-10.05,2.73l-176.96,102.1\n\t\tc-6.2,3.58-10.06,10.25-10.06,17.41l-0.07,231.47c0,7.27,3.76,13.78,10.05,17.42c6.3,3.64,13.81,3.64,20.11,0l176.95-102.11\n\t\tc6.2-3.58,10.06-10.25,10.06-17.41L457,141.95C457,134.68,453.24,128.16,446.95,124.53z"/>\n\t<path class="st2" d="M240.95,211.14l116.78-67.38c1.25-0.72,2.02-2.05,2.02-3.5l0.02-50.98c0-6.48-2.66-12.9-7.83-16.81\n\t\tc-6.69-5.06-15.27-5.55-22.33-1.48l-48.43,27.95L152.64,173.1c-6.22,3.59-10.06,10.23-10.06,17.41l-0.05,174.18l-0.02,56.41\n\t\tc0,6.48,2.65,12.89,7.81,16.81c6.69,5.07,15.29,5.57,22.35,1.49l47.2-27.24c1.25-0.72,2.02-2.05,2.02-3.5l0.05-164.64\n\t\tC221.95,230.46,229.19,217.92,240.95,211.14z"/>\n</g>\n</svg>\n'
+            });
+            var B;
+            ! function(e) {
+                e.launchPanel = "dask:launch-dashboard", e.launchLayout = "dask:launch-layout", e.populateDashboardUrl = "dask:populate-dashboard-url", e.populateAndLaunchLayout = "dask:populate-and-launch-layout", e.injectClientCode = "dask:inject-client-code", e.launchCluster = "dask:launch-cluster", e.stopCluster = "dask:stop-cluster", e.scaleCluster = "dask:scale-cluster", e.toggleAutoStartClient = "dask:toggle-auto-start-client"
+            }(B || (B = {}));
             const P = "dask-labextension:plugin",
-                F = {
+                W = {
                     activate: async function(e, t, n, s, a, r, o, l, d) {
                         const c = "dask-dashboard-launcher",
-                            m = async () => {
+                            u = async () => {
                                 const e = $.getCurrentKernel(s, o, n);
                                 return await $.shouldUseKernel(e) ? await $.checkKernel(e) : ""
                             }, p = t => {
                                 const s = $.getCurrentEditor(e, o, n);
                                 s && $.injectClientCode(t, s)
                             }, g = new U({
                                 launchDashboardItem: t => {
-                                    e.commands.execute(A.launchPanel, {
+                                    e.commands.execute(B.launchPanel, {
                                         item: t
                                     })
                                 },
-                                linkFinder: m,
+                                linkFinder: u,
                                 clientCodeInjector: p,
                                 clientCodeGetter: $.getClientCode,
                                 registry: e.commands,
-                                launchClusterId: A.launchCluster
+                                launchClusterId: B.launchCluster
                             });
-                        g.id = c, g.title.iconClass = "dask-DaskLogo jp-SideBar-tabIcon", g.title.caption = "Dask";
+                        g.id = c, g.title.icon = F, g.title.iconClass = "jp-SideBar-tabIcon", g.title.caption = "Dask";
                         const v = new i.WidgetTracker({
                             namespace: "dask-dashboard-launcher"
                         });
                         a.add(g, c), a.restore(v, {
-                            command: A.launchPanel,
+                            command: B.launchPanel,
                             args: e => ({
                                 item: e.item
                             } || {}),
                             name: e => e.item && e.item.route || ""
                         }), s.add(g, "left", {
                             rank: 200
                         });
@@ -793,172 +799,172 @@
                             if (!e) return;
                             const t = g.clusterManager.activeCluster;
                             return t && await $.shouldUseKernel(e.kernel) ? $.createClientForKernel(t, e.kernel) : void 0
                         }, b = [o, n], k = async e => {
                             if (e.session && e.session.kernel && "restarting" === e.session.kernel.status) return f(e.session)
                         }, y = (e, t) => {
                             t.sessionContext.statusChanged.connect(k)
-                        }, w = () => {
+                        }, _ = () => {
                             b.forEach((e => {
                                 e.forEach((async e => {
                                     const t = e.sessionContext.session;
                                     if (t && await $.shouldUseKernel(t.kernel)) return f(t)
                                 }))
                             }))
                         };
-                        let L, x = !1,
+                        let x, L = !1,
                             I = !1,
                             E = !1;
                         Promise.all([l.load(P), d.fetch(c)]).then((async e => {
                             const t = e[0];
                             if (!t) return void console.warn("Unable to retrieve dask-labextension settings");
                             const n = e[1],
                                 s = n ? n.url : "",
                                 a = n ? n.cluster : "",
                                 i = g.dashboardLauncher.input.urlInfo.effectiveUrl || g.dashboardLauncher.input.urlInfo.url;
                             g.dashboardLauncher.input.url = s && !i ? s : t.get("defaultURL").composite;
                             const r = () => {
-                                x = t.get("autoStartClient").composite, h.Signal.clearData(y), h.Signal.clearData(k), h.Signal.clearData(w), x && (b.forEach((e => {
+                                L = t.get("autoStartClient").composite, m.Signal.clearData(y), m.Signal.clearData(k), m.Signal.clearData(_), L && (b.forEach((e => {
                                     e.widgetAdded.connect(y)
                                 })), b.forEach((e => {
                                     e.forEach((async e => {
                                         await f(e.sessionContext.session), e.sessionContext.statusChanged.connect(k)
                                     }))
-                                })), g.clusterManager.activeClusterChanged.connect(w)), E = t.get("browserDashboardCheck").composite, g.dashboardLauncher.input.browserDashboardCheck = E, I = t.get("hideClusterManager").composite, g.clusterManager.setHidden(I), L = t.get("defaultLayout").composite
+                                })), g.clusterManager.activeClusterChanged.connect(_)), E = t.get("browserDashboardCheck").composite, g.dashboardLauncher.input.browserDashboardCheck = E, I = t.get("hideClusterManager").composite, g.clusterManager.setHidden(I), x = t.get("defaultLayout").composite
                             };
                             r(), t.changed.connect(r), a && (await g.clusterManager.refresh(), g.clusterManager.setActiveCluster(a))
-                        })), e.commands.addCommand(A.launchPanel, {
+                        })), e.commands.addCommand(B.launchPanel, {
                             label: e => `Launch Dask ${e.item.label||""} Dashboard`,
                             caption: "Launch a Dask dashboard",
                             execute: e => {
                                 const t = g.dashboardLauncher.input.urlInfo,
                                     n = t.effectiveUrl || t.url,
                                     a = t.isActive,
                                     i = e.item,
                                     r = null == e ? void 0 : e.options,
                                     o = v.find((e => !(!e || !e.item || e.item.route !== i.route)));
                                 if (o) return o.isAttached || s.add(o, "main", r), void s.activateById(o.id);
-                                const l = new _;
-                                return l.dashboardUrl = n, l.item = i, l.active = a, l.id = "dask-dashboard-" + $.id++, l.title.label = `${i.label}`, l.title.icon = "dask-DaskLogo", s.add(l, "main", r), v.add(l), l
+                                const l = new w;
+                                return l.dashboardUrl = n, l.item = i, l.active = a, l.id = "dask-dashboard-" + $.id++, l.title.label = `${i.label}`, l.title.icon = F, s.add(l, "main", r), v.add(l), l
                             }
                         });
                         const D = e => (e.startsWith("/") && (e = e.slice(1)), e.startsWith("individual-") || (e = "individual-" + e), e);
-                        e.commands.addCommand(A.launchLayout, {
+                        e.commands.addCommand(B.launchLayout, {
                             label: "Launch Dask Dashboard Layout",
                             caption: "Launch a pre-configured Dask Dashboard Layout",
                             isEnabled: () => g.dashboardLauncher.input.urlInfo.isActive,
                             execute: async () => {
                                 const t = g.dashboardLauncher.items,
                                     n = [];
-                                for (let e of Object.keys(L)) n.push([L[e].ref || null, e]);
-                                const s = (0, u.topologicSort)(n).filter((e => e)),
+                                for (let e of Object.keys(x)) n.push([x[e].ref || null, e]);
+                                const s = (0, h.topologicSort)(n).filter((e => e)),
                                     a = e.shell.currentWidget;
                                 for (let n of s) {
-                                    const s = L[n],
+                                    const s = x[n],
                                         a = t.find((e => D(e.route) === D(n)));
                                     if (!a) {
                                         console.warn(`Non-existent dashboard found in Dask layout spec ${n}`);
                                         continue
                                     }
                                     const i = {
                                         mode: s.mode
                                     };
                                     if (s.ref) {
                                         const e = v.find((e => !(!e || !e.item || D(e.item.route) !== D(s.ref))));
                                         e ? i.ref = e.id : (console.warn(`Non-existent dashboard found in Dask layout spec ${s.ref}`), i.ref = null)
                                     } else i.ref = null;
-                                    await e.commands.execute(A.launchPanel, {
+                                    await e.commands.execute(B.launchPanel, {
                                         item: a,
                                         options: i
                                     })
                                 }
                                 e.shell.activateById(a.id)
                             }
-                        }), e.commands.addCommand(A.populateDashboardUrl, {
+                        }), e.commands.addCommand(B.populateDashboardUrl, {
                             label: "Populate Dask Dashboard URL",
                             caption: "Attempt to populate the URL for an active Dask cluster",
                             execute: async e => {
-                                let t = e.url || await m();
+                                let t = e.url || await u();
                                 return t && (g.dashboardLauncher.input.url = t), t
                             }
-                        }), e.commands.addCommand(A.populateAndLaunchLayout, {
+                        }), e.commands.addCommand(B.populateAndLaunchLayout, {
                             label: "Populate Dask Dashboard URL and launch the default layout",
                             caption: "Attempt to populate the URL for an active Dask cluster and then launch the default layout",
                             execute: async t => {
-                                await e.commands.execute(A.populateDashboardUrl, t) && await e.commands.execute(A.launchLayout)
+                                await e.commands.execute(B.populateDashboardUrl, t) && await e.commands.execute(B.launchLayout)
                             }
-                        }), e.commands.addCommand(A.injectClientCode, {
+                        }), e.commands.addCommand(B.injectClientCode, {
                             label: "Inject Dask Client Connection Code",
                             execute: () => {
                                 const t = $.clusterFromClick(e, g.clusterManager);
                                 t && p(t)
                             }
-                        }), e.commands.addCommand(A.launchCluster, {
+                        }), e.commands.addCommand(B.launchCluster, {
                             label: e => e.isPalette ? "Launch New Cluster" : "NEW",
                             execute: () => g.clusterManager.start(),
                             iconClass: e => e.isPalette ? "" : "jp-AddIcon jp-Icon jp-Icon-16",
                             isEnabled: () => g.clusterManager.isReady,
                             caption: () => g.clusterManager.isReady ? "Start New Dask Cluster" : "Cluster starting..."
-                        }), e.commands.addCommand(A.stopCluster, {
+                        }), e.commands.addCommand(B.stopCluster, {
                             label: "Shutdown Cluster",
                             execute: () => {
                                 const t = $.clusterFromClick(e, g.clusterManager);
                                 if (t) return g.clusterManager.stop(t.id)
                             }
-                        }), e.commands.addCommand(A.scaleCluster, {
+                        }), e.commands.addCommand(B.scaleCluster, {
                             label: "Scale Cluster…",
                             execute: () => {
                                 const t = $.clusterFromClick(e, g.clusterManager);
                                 if (t) return g.clusterManager.scale(t.id)
                             }
-                        }), e.commands.addCommand(A.toggleAutoStartClient, {
+                        }), e.commands.addCommand(B.toggleAutoStartClient, {
                             label: "Auto-Start Dask",
-                            isToggled: () => x,
+                            isToggled: () => L,
                             execute: async () => {
-                                const e = !x,
+                                const e = !L,
                                     t = "autoStartClient";
                                 return l.set(P, t, e).catch((e => {
                                     console.error(`Failed to set ${P}:${t} - ${e.message}`)
                                 }))
                             }
                         }), r.fileMenu.addGroup([{
-                            command: A.launchLayout
+                            command: B.launchLayout
                         }], 50), r.settingsMenu.addGroup([{
-                            command: A.toggleAutoStartClient
-                        }]), [A.launchCluster, A.launchLayout, A.toggleAutoStartClient].forEach((e => {
+                            command: B.toggleAutoStartClient
+                        }]), [B.launchCluster, B.launchLayout, B.toggleAutoStartClient].forEach((e => {
                             t.addItem({
                                 category: "Dask",
                                 command: e,
                                 args: {
                                     isPalette: !0
                                 }
                             })
                         })), e.contextMenu.addItem({
-                            command: A.injectClientCode,
+                            command: B.injectClientCode,
                             selector: ".dask-ClusterListingItem",
                             rank: 10
                         }), e.contextMenu.addItem({
-                            command: A.stopCluster,
+                            command: B.stopCluster,
                             selector: ".dask-ClusterListingItem",
                             rank: 3
                         }), e.contextMenu.addItem({
-                            command: A.scaleCluster,
+                            command: B.scaleCluster,
                             selector: ".dask-ClusterListingItem",
                             rank: 2
                         }), e.contextMenu.addItem({
-                            command: A.launchCluster,
+                            command: B.launchCluster,
                             selector: ".dask-ClusterListing-list",
                             rank: 1
                         })
                     },
                     id: P,
-                    requires: [i.ICommandPalette, r.IConsoleTracker, a.ILabShell, a.ILayoutRestorer, o.IMainMenu, c.INotebookTracker, l.ISettingRegistry, d.IStateDB],
+                    requires: [i.ICommandPalette, o.IConsoleTracker, a.ILabShell, a.ILayoutRestorer, l.IMainMenu, u.INotebookTracker, d.ISettingRegistry, c.IStateDB],
                     autoStart: !0
                 },
-                W = F;
+                z = W;
             var $;
             ! function(e) {
                 function t(e) {
                     return `from dask.distributed import Client\n\nclient = Client("${e.scheduler_address}")\nclient`
                 }
                 e.id = 0, e.shouldUseKernel = async function(e) {
                     if (!e) return !1;
@@ -994,23 +1000,23 @@
                 }, e.getClientCode = t, e.getCurrentKernel = function(e, t, n) {
                     var s, a, i, r;
                     let o, l = e.currentWidget;
                     return l && t.has(l) ? o = null === (s = l.sessionContext.session) || void 0 === s ? void 0 : s.kernel : l && n.has(l) ? o = null === (a = l.sessionContext.session) || void 0 === a ? void 0 : a.kernel : t.currentWidget ? o = null === (i = t.currentWidget.sessionContext.session) || void 0 === i ? void 0 : i.kernel : n.currentWidget && (o = null === (r = n.currentWidget.sessionContext.session) || void 0 === r ? void 0 : r.kernel), o
                 }, e.getCurrentEditor = function(e, t, n) {
                     let s, a = e.shell.currentWidget;
                     if (a && t.has(a)) {
-                        c.NotebookActions.insertAbove(a.content);
+                        u.NotebookActions.insertAbove(a.content);
                         const e = a.content.activeCell;
                         s = e && e.editor
                     } else if (a && n.has(a)) {
                         const e = a.console.promptCell;
                         s = e && e.editor
                     } else if (t.currentWidget) {
                         const e = t.currentWidget;
-                        c.NotebookActions.insertAbove(e.content);
+                        u.NotebookActions.insertAbove(e.content);
                         const n = e.content.activeCell;
                         s = n && n.editor
                     } else if (n.currentWidget) {
                         const e = n.currentWidget.console.promptCell;
                         s = e && e.editor
                     }
                     return s
```

### Comparing `dask_labextension-6.1.0/dask_labextension/labextension/static/remoteEntry.c559dc887be99a51d44a.js` & `dask_labextension-6.2.0/dask_labextension/labextension/static/remoteEntry.48341a7428463ba2c6bb.js`

 * *Files 13% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, a, i, l, u, s, d, f, p, c, h, v, m, b, g = {
-            803: (e, r, t) => {
+    var e, r, t, n, o, a, i, l, u, s, d, f, c, p, h, b, v, m, g, y = {
+            391: (e, r, t) => {
                 var n = {
-                        "./index": () => Promise.all([t.e(60), t.e(319)]).then((() => () => t(319))),
-                        "./extension": () => Promise.all([t.e(60), t.e(319)]).then((() => () => t(319)))
+                        "./index": () => Promise.all([t.e(60), t.e(224)]).then((() => () => t(224))),
+                        "./extension": () => Promise.all([t.e(60), t.e(224)]).then((() => () => t(224)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     a = (e, r) => {
                         if (t.S) {
                             var n = "default",
@@ -20,115 +20,116 @@
                     };
                 t.d(r, {
                     get: () => o,
                     init: () => a
                 })
             }
         },
-        y = {};
+        w = {};
 
-    function w(e) {
-        var r = y[e];
+    function j(e) {
+        var r = w[e];
         if (void 0 !== r) return r.exports;
-        var t = y[e] = {
+        var t = w[e] = {
             id: e,
             exports: {}
         };
-        return g[e](t, t.exports, w), t.exports
+        return y[e](t, t.exports, j), t.exports
     }
-    w.m = g, w.c = y, w.n = e => {
+    j.m = y, j.c = w, j.n = e => {
         var r = e && e.__esModule ? () => e.default : () => e;
-        return w.d(r, {
+        return j.d(r, {
             a: r
         }), r
-    }, w.d = (e, r) => {
-        for (var t in r) w.o(r, t) && !w.o(e, t) && Object.defineProperty(e, t, {
+    }, j.d = (e, r) => {
+        for (var t in r) j.o(r, t) && !j.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
-    }, w.f = {}, w.e = e => Promise.all(Object.keys(w.f).reduce(((r, t) => (w.f[t](e, r), r)), [])), w.u = e => e + "." + {
-        60: "ae13c83df156626ac632",
-        114: "6d8f6f4a88afc2816496",
-        319: "3ff908a63582f9623f31"
+    }, j.f = {}, j.e = e => Promise.all(Object.keys(j.f).reduce(((r, t) => (j.f[t](e, r), r)), [])), j.u = e => e + "." + {
+        60: "6b27874877fba88bc953",
+        114: "f9e3bc980911cf750147",
+        224: "86c44b816becca807a99"
     } [e] + ".js?v=" + {
-        60: "ae13c83df156626ac632",
-        114: "6d8f6f4a88afc2816496",
-        319: "3ff908a63582f9623f31"
-    } [e], w.g = function() {
+        60: "6b27874877fba88bc953",
+        114: "f9e3bc980911cf750147",
+        224: "86c44b816becca807a99"
+    } [e], j.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), w.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "dask-labextension:", w.l = (t, n, o, a) => {
+    }(), j.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "dask-labextension:", j.l = (t, n, o, a) => {
         if (e[t]) e[t].push(n);
         else {
             var i, l;
             if (void 0 !== o)
                 for (var u = document.getElementsByTagName("script"), s = 0; s < u.length; s++) {
                     var d = u[s];
                     if (d.getAttribute("src") == t || d.getAttribute("data-webpack") == r + o) {
                         i = d;
                         break
                     }
                 }
-            i || (l = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, w.nc && i.setAttribute("nonce", w.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
+            i || (l = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, j.nc && i.setAttribute("nonce", j.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
             var f = (r, n) => {
-                    i.onerror = i.onload = null, clearTimeout(p);
+                    i.onerror = i.onload = null, clearTimeout(c);
                     var o = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
                 },
-                p = setTimeout(f.bind(null, void 0, {
+                c = setTimeout(f.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
             i.onerror = f.bind(null, i.onerror), i.onload = f.bind(null, i.onload), l && document.head.appendChild(i)
         }
-    }, w.r = e => {
+    }, j.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
     }, (() => {
-        w.S = {};
+        j.S = {};
         var e = {},
             r = {};
-        w.I = (t, n) => {
+        j.I = (t, n) => {
             n || (n = []);
             var o = r[t];
             if (o || (o = r[t] = {}), !(n.indexOf(o) >= 0)) {
                 if (n.push(o), e[t]) return e[t];
-                w.o(w.S, t) || (w.S[t] = {});
-                var a = w.S[t],
+                j.o(j.S, t) || (j.S[t] = {});
+                var a = j.S[t],
                     i = "dask-labextension",
                     l = (e, r, t, n) => {
                         var o = a[e] = a[e] || {},
                             l = o[r];
                         (!l || !l.loaded && (!n != !l.eager ? n : i > l.from)) && (o[r] = {
                             get: t,
                             from: i,
                             eager: !!n
                         })
                     },
                     u = [];
-                return "default" === t && (l("@lumino/polling", "1.10.0", (() => Promise.all([w.e(114), w.e(60)]).then((() => () => w(114))))), l("dask-labextension", "6.1.0", (() => Promise.all([w.e(60), w.e(319)]).then((() => () => w(319)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                return "default" === t && (l("@lumino/polling", "1.11.4", (() => Promise.all([j.e(114), j.e(60)]).then((() => () => j(114))))), l("dask-labextension", "6.2.0", (() => Promise.all([j.e(60), j.e(224)]).then((() => () => j(224)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
-        w.g.importScripts && (e = w.g.location + "");
-        var r = w.g.document;
+        j.g.importScripts && (e = j.g.location + "");
+        var r = j.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
             var t = r.getElementsByTagName("script");
-            t.length && (e = t[t.length - 1].src)
+            if (t.length)
+                for (var n = t.length - 1; n > -1 && !e;) e = t[n--].src
         }
         if (!e) throw new Error("Automatic publicPath is not supported in this browser");
-        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), w.p = e
+        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), j.p = e
     })(), t = e => {
         var r = e => e.split(".").map((e => +e == e ? +e : e)),
             t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
             n = t[1] ? r(t[1]) : [];
         return t[2] && (n.length++, n.push.apply(n, r(t[2]))), t[3] && (n.push([]), n.push.apply(n, r(t[3]))), n
     }, n = (e, r) => {
         e = t(e), r = t(r);
@@ -186,113 +187,115 @@
                     u = !1, l--
                 } else {
                     if (l <= n || d < f != o) return !1;
                     u = !1
                 } else "s" != f && "n" != f && (u = !1, l--)
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
-        var t = w.S[e];
-        if (!t || !w.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
+        var t = j.S[e];
+        if (!t || !j.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, l = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
     }, u = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", s = (e, r, t, n) => {
         var o = l(e, t);
-        return a(n, o) || "undefined" != typeof console && console.warn && console.warn(u(e, t, o, n)), f(e[t][o])
+        return a(n, o) || f(u(e, t, o, n)), c(e[t][o])
     }, d = (e, r, t) => {
         var o = e[r];
         return (r = Object.keys(o).reduce(((e, r) => !a(t, r) || e && !n(e, r) ? e : r), 0)) && o[r]
-    }, f = e => (e.loaded = 1, e.get()), c = (p = e => function(r, t, n, o) {
-        var a = w.I(r);
-        return a && a.then ? a.then(e.bind(e, r, w.S[r], t, n, o)) : e(r, w.S[r], t, n, o)
-    })(((e, r, t, n) => (i(e, t), s(r, 0, t, n)))), h = p(((e, r, t, n, o) => {
-        var a = r && w.o(r, t) && d(r, t, n);
-        return a ? f(a) : o()
+    }, f = e => {
+        "undefined" != typeof console && console.warn && console.warn(e)
+    }, c = e => (e.loaded = 1, e.get()), h = (p = e => function(r, t, n, o) {
+        var a = j.I(r);
+        return a && a.then ? a.then(e.bind(e, r, j.S[r], t, n, o)) : e(r, j.S[r], t, n, o)
+    })(((e, r, t, n) => (i(e, t), s(r, 0, t, n)))), b = p(((e, r, t, n, o) => {
+        var a = r && j.o(r, t) && d(r, t, n);
+        return a ? c(a) : o()
     })), v = {}, m = {
-        526: () => c("default", "@lumino/coreutils", [1, 1, 11, 0]),
-        840: () => c("default", "@lumino/signaling", [1, 1, 10, 0]),
-        258: () => c("default", "@jupyterlab/services", [1, 6, 6, 1]),
-        271: () => c("default", "react", [1, 17, 0, 1]),
-        358: () => h("default", "@lumino/polling", [1, 1, 0, 4], (() => w.e(114).then((() => () => w(114))))),
-        397: () => c("default", "@jupyterlab/statedb", [1, 3, 6, 1]),
-        431: () => c("default", "@lumino/widgets", [1, 1, 37, 1]),
-        456: () => c("default", "react-dom", [1, 17, 0, 1]),
-        468: () => c("default", "@jupyterlab/console", [1, 3, 6, 1]),
-        510: () => c("default", "@jupyterlab/apputils", [1, 3, 6, 1]),
-        520: () => c("default", "@lumino/domutils", [1, 1, 8, 0]),
-        591: () => c("default", "@jupyterlab/ui-components", [1, 3, 6, 1]),
-        598: () => c("default", "@jupyterlab/settingregistry", [1, 3, 6, 1]),
-        694: () => c("default", "@lumino/dragdrop", [1, 1, 13, 0]),
-        705: () => c("default", "@jupyterlab/mainmenu", [1, 3, 6, 1]),
-        767: () => c("default", "@jupyterlab/notebook", [1, 3, 6, 1]),
-        866: () => c("default", "@jupyterlab/application", [1, 3, 6, 1]),
-        886: () => c("default", "@jupyterlab/coreutils", [1, 5, 6, 1]),
-        918: () => c("default", "@lumino/algorithm", [1, 1, 9, 0])
-    }, b = {
+        526: () => h("default", "@lumino/coreutils", [1, 1, 11, 0]),
+        840: () => h("default", "@lumino/signaling", [1, 1, 10, 0]),
+        127: () => h("default", "@jupyterlab/notebook", [1, 3, 6, 5]),
+        139: () => h("default", "@jupyterlab/services", [1, 6, 6, 5]),
+        271: () => h("default", "react", [1, 17, 0, 1]),
+        299: () => h("default", "@jupyterlab/settingregistry", [1, 3, 6, 5]),
+        303: () => h("default", "@jupyterlab/apputils", [1, 3, 6, 5]),
+        344: () => h("default", "@jupyterlab/coreutils", [1, 5, 6, 5]),
+        358: () => b("default", "@lumino/polling", [1, 1, 0, 4], (() => j.e(114).then((() => () => j(114))))),
+        456: () => h("default", "react-dom", [1, 17, 0, 1]),
+        520: () => h("default", "@lumino/domutils", [1, 1, 8, 0]),
+        535: () => h("default", "@jupyterlab/mainmenu", [1, 3, 6, 5]),
+        543: () => h("default", "@jupyterlab/console", [1, 3, 6, 5]),
+        548: () => h("default", "@jupyterlab/statedb", [1, 3, 6, 5]),
+        638: () => h("default", "@jupyterlab/application", [1, 3, 6, 5]),
+        694: () => h("default", "@lumino/dragdrop", [1, 1, 13, 0]),
+        745: () => h("default", "@jupyterlab/ui-components", [1, 3, 6, 5]),
+        832: () => h("default", "@lumino/widgets", [1, 1, 37, 2]),
+        918: () => h("default", "@lumino/algorithm", [1, 1, 9, 0])
+    }, g = {
         60: [526, 840],
-        319: [258, 271, 358, 397, 431, 456, 468, 510, 520, 591, 598, 694, 705, 767, 866, 886, 918]
-    }, w.f.consumes = (e, r) => {
-        w.o(b, e) && b[e].forEach((e => {
-            if (w.o(v, e)) return r.push(v[e]);
+        224: [127, 139, 271, 299, 303, 344, 358, 456, 520, 535, 543, 548, 638, 694, 745, 832, 918]
+    }, j.f.consumes = (e, r) => {
+        j.o(g, e) && g[e].forEach((e => {
+            if (j.o(v, e)) return r.push(v[e]);
             var t = r => {
-                    v[e] = 0, w.m[e] = t => {
-                        delete w.c[e], t.exports = r()
+                    v[e] = 0, j.m[e] = t => {
+                        delete j.c[e], t.exports = r()
                     }
                 },
                 n = r => {
-                    delete v[e], w.m[e] = t => {
-                        throw delete w.c[e], r
+                    delete v[e], j.m[e] = t => {
+                        throw delete j.c[e], r
                     }
                 };
             try {
                 var o = m[e]();
                 o.then ? r.push(v[e] = o.then(t).catch(n)) : t(o)
             } catch (e) {
                 n(e)
             }
         }))
     }, (() => {
         var e = {
             754: 0
         };
-        w.f.j = (r, t) => {
-            var n = w.o(e, r) ? e[r] : void 0;
+        j.f.j = (r, t) => {
+            var n = j.o(e, r) ? e[r] : void 0;
             if (0 !== n)
                 if (n) t.push(n[2]);
                 else if (60 != r) {
                 var o = new Promise(((t, o) => n = e[r] = [t, o]));
                 t.push(n[2] = o);
-                var a = w.p + w.u(r),
+                var a = j.p + j.u(r),
                     i = new Error;
-                w.l(a, (t => {
-                    if (w.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
+                j.l(a, (t => {
+                    if (j.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
                         var o = t && ("load" === t.type ? "missing" : t.type),
                             a = t && t.target && t.target.src;
                         i.message = "Loading chunk " + r + " failed.\n(" + o + ": " + a + ")", i.name = "ChunkLoadError", i.type = o, i.request = a, n[1](i)
                     }
                 }), "chunk-" + r, r)
             } else e[r] = 0
         };
         var r = (r, t) => {
                 var n, o, [a, i, l] = t,
                     u = 0;
                 if (a.some((r => 0 !== e[r]))) {
-                    for (n in i) w.o(i, n) && (w.m[n] = i[n]);
-                    l && l(w)
+                    for (n in i) j.o(i, n) && (j.m[n] = i[n]);
+                    l && l(j)
                 }
-                for (r && r(t); u < a.length; u++) o = a[u], w.o(e, o) && e[o] && e[o][0](), e[o] = 0
+                for (r && r(t); u < a.length; u++) o = a[u], j.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
             t = self.webpackChunkdask_labextension = self.webpackChunkdask_labextension || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
-    })(), w.nc = void 0;
-    var j = w(803);
-    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["dask-labextension"] = j
+    })(), j.nc = void 0;
+    var k = j(391);
+    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["dask-labextension"] = k
 })();
```

### Comparing `dask_labextension-6.1.0/dask_labextension/labextension/static/third-party-licenses.json` & `dask_labextension-6.2.0/dask_labextension/labextension/static/third-party-licenses.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666667%*

 * *Differences: {"'packages'": "{0: {'versionInfo': '1.11.4'}}"}*

```diff
@@ -1,14 +1,14 @@
 {
     "packages": [
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@lumino/polling",
-            "versionInfo": "1.10.0"
+            "versionInfo": "1.11.4"
         },
         {
             "extractedText": "Copyright JS Foundation and other contributors\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n'Software'), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY\nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,\nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE\nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "css-loader",
             "versionInfo": "5.2.7"
         },
```

### Comparing `dask_labextension-6.1.0/dask_labextension/manager.py` & `dask_labextension-6.2.0/dask_labextension/manager.py`

 * *Files identical despite different names*

### Comparing `dask_labextension-6.1.0/dask_labextension/tests/test_manager.py` & `dask_labextension-6.2.0/dask_labextension/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `dask_labextension-6.1.0/dask_labextension.egg-info/PKG-INFO` & `dask_labextension-6.2.0/dask_labextension.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-labextension
-Version: 6.1.0
+Version: 6.2.0
 Summary: A JupyterLab extension for Dask.
 Home-page: https://github.com/dask/dask-labextension
 Author: Ian Rose, Matt Rocklin, Jacob Tomlinson
 License: BSD-3-Clause
 Keywords: dask,Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
 Platform: Mac OS X
@@ -231,26 +231,39 @@
 ```bash
 pip install -e .
 jupyter serverextension enable --sys-prefix dask_labextension
 ```
 
 ## Publishing
 
-This application is distributed as two subpackages.
-
-The JupyterLab frontend part is published to [npm](https://www.npmjs.com/package/dask-labextension),
-and the server-side part to [PyPI](https://pypi.org/project/dask-labextension/).
-
-Releases for both packages are done with the `jlpm` tool, `git` and Travis CI.
+This extension contains a front-end component written in TypeScript
+and a back-end component written in Python.
+The front-end is compiled to Javascript during the build process
+and is distributed as static assets along with the Python package.
 
 _Note: Package versions are not prefixed with the letter `v`. You will need to disable this._
 
 ```console
 $ jlpm config set version-tag-prefix ""
 ```
 
-Making a release
+### Release process
 
-```console
-$ jlpm version [--major|--minor|--patch]  # updates package.json and creates git commit and tag
-$ git push upstream main && git push upstream main --tags  # pushes tags to GitHub which triggers Travis CI to build and deploy
+This requires `node`, `build`, and `twine` to be installed.
+
+```bash
+jlpm version [--major|--minor|--patch]  # updates package.json and creates git commit and tag
+git push upstream main && git push upstream main --tags  # pushes to GitHub
+python -m build .  # Build the package
+twine upload dist/*  # Upload the package to PyPI
+```
+
+### Handling Javascript package version conflicts
+
+Unlike Python, Javascript packages can include more than one version of the same dependency.
+Usually the `yarn` package manager handles this okay, but occasionally you might end up with conflicting versions,
+or with unexpected package bloat.
+You can try to fix this by deduplicating dependencies:
+
+```bash
+jlpm yarn-deduplicate -s fewer
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dask-labextension Version: 6.1.0 Summary: A
+Metadata-Version: 2.1 Name: dask-labextension Version: 6.2.0 Summary: A
 JupyterLab extension for Dask. Home-page: https://github.com/dask/dask-
 labextension Author: Ian Rose, Matt Rocklin, Jacob Tomlinson License: BSD-3-
 Clause Keywords: dask,Jupyter,JupyterLab,JupyterLab3 Platform: Linux Platform:
 Mac OS X Platform: Windows Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.6 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
@@ -84,17 +84,22 @@
 of the labextension you can run the following in this directory: ```bash jlpm #
 Install npm package dependencies jlpm build # Compile the TypeScript sources to
 Javascript jupyter labextension develop . --overwrite # Install the current
 directory as an extension ``` To rebuild the extension: ```bash jlpm build ```
 You should then be able to refresh the JupyterLab page and it will pick up the
 changes to the extension. To run an editable install of the server extension,
 run ```bash pip install -e . jupyter serverextension enable --sys-prefix
-dask_labextension ``` ## Publishing This application is distributed as two
-subpackages. The JupyterLab frontend part is published to [npm](https://
-www.npmjs.com/package/dask-labextension), and the server-side part to [PyPI]
-(https://pypi.org/project/dask-labextension/). Releases for both packages are
-done with the `jlpm` tool, `git` and Travis CI. _Note: Package versions are not
+dask_labextension ``` ## Publishing This extension contains a front-end
+component written in TypeScript and a back-end component written in Python. The
+front-end is compiled to Javascript during the build process and is distributed
+as static assets along with the Python package. _Note: Package versions are not
 prefixed with the letter `v`. You will need to disable this._ ```console $ jlpm
-config set version-tag-prefix "" ``` Making a release ```console $ jlpm version
-[--major|--minor|--patch] # updates package.json and creates git commit and tag
-$ git push upstream main && git push upstream main --tags # pushes tags to
-GitHub which triggers Travis CI to build and deploy ```
+config set version-tag-prefix "" ``` ### Release process This requires `node`,
+`build`, and `twine` to be installed. ```bash jlpm version [--major|--minor|--
+patch] # updates package.json and creates git commit and tag git push upstream
+main && git push upstream main --tags # pushes to GitHub python -m build . #
+Build the package twine upload dist/* # Upload the package to PyPI ``` ###
+Handling Javascript package version conflicts Unlike Python, Javascript
+packages can include more than one version of the same dependency. Usually the
+`yarn` package manager handles this okay, but occasionally you might end up
+with conflicting versions, or with unexpected package bloat. You can try to fix
+this by deduplicating dependencies: ```bash jlpm yarn-deduplicate -s fewer ```
```

### Comparing `dask_labextension-6.1.0/dask_labextension.egg-info/SOURCES.txt` & `dask_labextension-6.2.0/dask_labextension.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 package.json
 pyproject.toml
 setup.cfg
 setup.py
 tsconfig.eslint.json
 tsconfig.json
 versioneer.py
+yarn.lock
 dask_labextension/__init__.py
 dask_labextension/_version.py
 dask_labextension/clusterhandler.py
 dask_labextension/config.py
 dask_labextension/dashboardhandler.py
 dask_labextension/labextension.yaml
 dask_labextension/manager.py
@@ -21,25 +22,26 @@
 dask_labextension.egg-info/dependency_links.txt
 dask_labextension.egg-info/not-zip-safe
 dask_labextension.egg-info/requires.txt
 dask_labextension.egg-info/top_level.txt
 dask_labextension/labextension/package.json
 dask_labextension/labextension/schemas/dask-labextension/package.json.orig
 dask_labextension/labextension/schemas/dask-labextension/plugin.json
-dask_labextension/labextension/static/114.6d8f6f4a88afc2816496.js
-dask_labextension/labextension/static/319.3ff908a63582f9623f31.js
-dask_labextension/labextension/static/remoteEntry.c559dc887be99a51d44a.js
+dask_labextension/labextension/static/114.f9e3bc980911cf750147.js
+dask_labextension/labextension/static/224.86c44b816becca807a99.js
+dask_labextension/labextension/static/remoteEntry.48341a7428463ba2c6bb.js
 dask_labextension/labextension/static/style.js
 dask_labextension/labextension/static/third-party-licenses.json
 dask_labextension/tests/test_manager.py
 jupyter-config/jupyter_notebook_config.d/dask_labextension.json
 jupyter-config/jupyter_server_config.d/dask_labextension.json
 schema/plugin.json
 src/clusters.tsx
 src/dashboard.tsx
 src/index.ts
 src/scaling.tsx
 src/sidebar.ts
+src/svg.d.ts
 style/code-dark.svg
 style/code-light.svg
 style/dask.svg
 style/index.css
```

### Comparing `dask_labextension-6.1.0/package.json` & `dask_labextension-6.2.0/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9705882352941175%*

 * *Differences: {"'devDependencies'": "{'yarn-deduplicate': '^5.0.0'}", "'version'": "'6.2.0'"}*

```diff
@@ -41,15 +41,16 @@
         "eslint-plugin-react": "^7.21.5",
         "mkdirp": "^1.0.3",
         "mocha": "^6.2.0",
         "npm-run-all": "^4.1.5",
         "prettier": "^2.1.1",
         "rimraf": "^3.0.2",
         "typescript": "~4.1.3",
-        "yarn": "1.22.0"
+        "yarn": "1.22.0",
+        "yarn-deduplicate": "^5.0.0"
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "schema/*.json",
         "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/dask/dask-labextension",
@@ -93,9 +94,9 @@
         "prettier:check": "prettier --list-different '**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}'",
         "test": "mocha",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
     "types": "lib/index.d.ts",
-    "version": "6.1.0"
+    "version": "6.2.0"
 }
```

### Comparing `dask_labextension-6.1.0/schema/plugin.json` & `dask_labextension-6.2.0/schema/plugin.json`

 * *Files identical despite different names*

### Comparing `dask_labextension-6.1.0/setup.cfg` & `dask_labextension-6.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `dask_labextension-6.1.0/setup.py` & `dask_labextension-6.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     long_description_content_type="text/markdown",
     cmdclass=cmdclass,
     packages=setuptools.find_packages(),
     install_requires=[
         "bokeh >=1.0.0,!=2.0.0",
         "distributed>=1.24.1",
         "jupyter-server-proxy>=1.3.2",
-        "jupyterlab>=3.0.0",
+        "jupyterlab>=3.0.0,<4",
     ],
     zip_safe=False,
     include_package_data=True,
     python_requires=">=3.6",
     license="BSD-3-Clause",
     platforms="Linux, Mac OS X, Windows",
     keywords=["dask", "Jupyter", "JupyterLab", "JupyterLab3"],
```

### Comparing `dask_labextension-6.1.0/src/clusters.tsx` & `dask_labextension-6.2.0/src/clusters.tsx`

 * *Files identical despite different names*

### Comparing `dask_labextension-6.1.0/src/dashboard.tsx` & `dask_labextension-6.2.0/src/dashboard.tsx`

 * *Files identical despite different names*

### Comparing `dask_labextension-6.1.0/src/index.ts` & `dask_labextension-6.2.0/src/index.ts`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,16 @@
   ISessionContext,
   IWidgetTracker,
   WidgetTracker
 } from '@jupyterlab/apputils';
 
 import { CodeEditor } from '@jupyterlab/codeeditor';
 
+import { LabIcon } from '@jupyterlab/ui-components';
+
 import { ConsolePanel, IConsoleTracker } from '@jupyterlab/console';
 
 import { DocumentRegistry } from '@jupyterlab/docregistry';
 
 import { IMainMenu } from '@jupyterlab/mainmenu';
 
 import { ISettingRegistry } from '@jupyterlab/settingregistry';
@@ -40,14 +42,21 @@
 
 import { DaskDashboard, IDashboardItem } from './dashboard';
 
 import { DaskSidebar } from './sidebar';
 
 import '../style/index.css';
 
+import DaskSvgStr from '../style/dask.svg';
+
+export const DaskIcon = new LabIcon({
+  name: 'dask:icon',
+  svgstr: DaskSvgStr
+});
+
 namespace CommandIDs {
   /**
    * Launch a dask dashboard panel in an iframe.
    */
   export const launchPanel = 'dask:launch-dashboard';
 
   /**
@@ -171,15 +180,16 @@
     linkFinder,
     clientCodeInjector,
     clientCodeGetter: Private.getClientCode,
     registry: app.commands,
     launchClusterId: CommandIDs.launchCluster
   });
   sidebar.id = id;
-  sidebar.title.iconClass = 'dask-DaskLogo jp-SideBar-tabIcon';
+  sidebar.title.icon = DaskIcon;
+  sidebar.title.iconClass = 'jp-SideBar-tabIcon';
   sidebar.title.caption = 'Dask';
 
   // An instance tracker which is used for state restoration.
   const tracker = new WidgetTracker<DaskDashboard>({
     namespace: 'dask-dashboard-launcher'
   });
 
@@ -427,15 +437,15 @@
       // Otherwise create the new dashboard widget.
       const dashboard = new DaskDashboard();
       dashboard.dashboardUrl = dashboardUrl;
       dashboard.item = dashboardItem;
       dashboard.active = active;
       dashboard.id = `dask-dashboard-${Private.id++}`;
       dashboard.title.label = `${dashboardItem.label}`;
-      dashboard.title.icon = 'dask-DaskLogo';
+      dashboard.title.icon = DaskIcon;
 
       labShell.add(dashboard, 'main', addOptions);
       void tracker.add(dashboard); // no need to wait on this
       return dashboard;
     }
   });
```

### Comparing `dask_labextension-6.1.0/src/scaling.tsx` & `dask_labextension-6.2.0/src/scaling.tsx`

 * *Files identical despite different names*

### Comparing `dask_labextension-6.1.0/src/sidebar.ts` & `dask_labextension-6.2.0/src/sidebar.ts`

 * *Files identical despite different names*

### Comparing `dask_labextension-6.1.0/style/dask.svg` & `dask_labextension-6.2.0/style/dask.svg`

 * *Files identical despite different names*

### Comparing `dask_labextension-6.1.0/style/index.css` & `dask_labextension-6.2.0/style/index.css`

 * *Files identical despite different names*

### Comparing `dask_labextension-6.1.0/tsconfig.json` & `dask_labextension-6.2.0/tsconfig.json`

 * *Files identical despite different names*

### Comparing `dask_labextension-6.1.0/versioneer.py` & `dask_labextension-6.2.0/versioneer.py`

 * *Files identical despite different names*

