# Comparing `tmp/cellmaps_imagedownloader-0.1.0a6.tar.gz` & `tmp/cellmaps_imagedownloader-0.1.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cellmaps_imagedownloader-0.1.0a6.tar", last modified: Mon Jul 17 19:13:47 2023, max compression
+gzip compressed data, was "dist/cellmaps_imagedownloader-0.1.0a7.tar", last modified: Tue Aug  1 20:07:35 2023, max compression
```

## Comparing `cellmaps_imagedownloader-0.1.0a6.tar` & `cellmaps_imagedownloader-0.1.0a7.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-17 19:13:47.116332 cellmaps_imagedownloader-0.1.0a6/
--rw-r--r--   0 churas     (504) staff       (20)      266 2023-07-17 19:13:09.000000 cellmaps_imagedownloader-0.1.0a6/AUTHORS.rst
--rw-r--r--   0 churas     (504) staff       (20)     3731 2023-05-03 22:51:16.000000 cellmaps_imagedownloader-0.1.0a6/CONTRIBUTING.rst
--rw-r--r--   0 churas     (504) staff       (20)       89 2023-05-11 22:14:34.000000 cellmaps_imagedownloader-0.1.0a6/HISTORY.rst
--rw-r--r--   0 churas     (504) staff       (20)     1102 2023-02-15 23:31:37.000000 cellmaps_imagedownloader-0.1.0a6/LICENSE
--rw-r--r--   0 churas     (504) staff       (20)      262 2023-02-15 23:31:37.000000 cellmaps_imagedownloader-0.1.0a6/MANIFEST.in
--rw-r--r--   0 churas     (504) staff       (20)     5242 2023-07-17 19:13:47.116462 cellmaps_imagedownloader-0.1.0a6/PKG-INFO
--rw-r--r--   0 churas     (504) staff       (20)     3281 2023-06-07 18:23:11.000000 cellmaps_imagedownloader-0.1.0a6/README.rst
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-17 19:13:47.102169 cellmaps_imagedownloader-0.1.0a6/cellmaps_imagedownloader/
--rw-r--r--   0 churas     (504) staff       (20)      354 2023-07-17 19:13:09.000000 cellmaps_imagedownloader-0.1.0a6/cellmaps_imagedownloader/__init__.py
--rw-r--r--   0 churas     (504) staff       (20)    11048 2023-07-17 19:13:31.000000 cellmaps_imagedownloader-0.1.0a6/cellmaps_imagedownloader/cellmaps_imagedownloadercmd.py
--rw-r--r--   0 churas     (504) staff       (20)      145 2023-05-03 22:51:16.000000 cellmaps_imagedownloader-0.1.0a6/cellmaps_imagedownloader/exceptions.py
--rw-r--r--   0 churas     (504) staff       (20)    16811 2023-07-17 19:13:31.000000 cellmaps_imagedownloader-0.1.0a6/cellmaps_imagedownloader/gene.py
--rw-r--r--   0 churas     (504) staff       (20)     7244 2023-07-17 19:13:31.000000 cellmaps_imagedownloader-0.1.0a6/cellmaps_imagedownloader/proteinatlas.py
--rw-r--r--   0 churas     (504) staff       (20)    29631 2023-07-17 19:13:31.000000 cellmaps_imagedownloader-0.1.0a6/cellmaps_imagedownloader/runner.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-17 19:13:47.104744 cellmaps_imagedownloader-0.1.0a6/cellmaps_imagedownloader.egg-info/
--rw-r--r--   0 churas     (504) staff       (20)     5242 2023-07-17 19:13:47.000000 cellmaps_imagedownloader-0.1.0a6/cellmaps_imagedownloader.egg-info/PKG-INFO
--rw-r--r--   0 churas     (504) staff       (20)     1517 2023-07-17 19:13:47.000000 cellmaps_imagedownloader-0.1.0a6/cellmaps_imagedownloader.egg-info/SOURCES.txt
--rw-r--r--   0 churas     (504) staff       (20)        1 2023-07-17 19:13:47.000000 cellmaps_imagedownloader-0.1.0a6/cellmaps_imagedownloader.egg-info/dependency_links.txt
--rw-r--r--   0 churas     (504) staff       (20)        1 2023-07-17 19:13:47.000000 cellmaps_imagedownloader-0.1.0a6/cellmaps_imagedownloader.egg-info/not-zip-safe
--rw-r--r--   0 churas     (504) staff       (20)       36 2023-07-17 19:13:47.000000 cellmaps_imagedownloader-0.1.0a6/cellmaps_imagedownloader.egg-info/requires.txt
--rw-r--r--   0 churas     (504) staff       (20)       25 2023-07-17 19:13:47.000000 cellmaps_imagedownloader-0.1.0a6/cellmaps_imagedownloader.egg-info/top_level.txt
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-17 19:13:47.110537 cellmaps_imagedownloader-0.1.0a6/docs/
--rw-r--r--   0 churas     (504) staff       (20)      625 2023-05-03 22:57:03.000000 cellmaps_imagedownloader-0.1.0a6/docs/Makefile
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-17 19:13:47.096461 cellmaps_imagedownloader-0.1.0a6/docs/_build/
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-17 19:13:47.096598 cellmaps_imagedownloader-0.1.0a6/docs/_build/html/
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-17 19:13:47.111593 cellmaps_imagedownloader-0.1.0a6/docs/_build/html/_static/
--rw-r--r--   0 churas     (504) staff       (20)      286 2023-05-02 22:49:28.000000 cellmaps_imagedownloader-0.1.0a6/docs/_build/html/_static/file.png
--rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_imagedownloader-0.1.0a6/docs/_build/html/_static/minus.png
--rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_imagedownloader-0.1.0a6/docs/_build/html/_static/plus.png
--rw-r--r--   0 churas     (504) staff       (20)       28 2023-02-15 23:31:37.000000 cellmaps_imagedownloader-0.1.0a6/docs/authors.rst
--rw-r--r--   0 churas     (504) staff       (20)     1027 2023-05-03 22:58:28.000000 cellmaps_imagedownloader-0.1.0a6/docs/cellmaps_imagedownloader.rst
--rwxr-xr-x   0 churas     (504) staff       (20)     6214 2023-05-22 22:22:34.000000 cellmaps_imagedownloader-0.1.0a6/docs/conf.py
--rw-r--r--   0 churas     (504) staff       (20)       33 2023-02-15 23:31:37.000000 cellmaps_imagedownloader-0.1.0a6/docs/contributing.rst
--rw-r--r--   0 churas     (504) staff       (20)      174 2023-02-15 23:31:37.000000 cellmaps_imagedownloader-0.1.0a6/docs/devbranches.rst
--rw-r--r--   0 churas     (504) staff       (20)      292 2023-05-03 22:57:03.000000 cellmaps_imagedownloader-0.1.0a6/docs/developer.rst
--rw-r--r--   0 churas     (504) staff       (20)       28 2023-02-15 23:31:37.000000 cellmaps_imagedownloader-0.1.0a6/docs/history.rst
--rw-r--r--   0 churas     (504) staff       (20)      243 2023-05-22 21:38:15.000000 cellmaps_imagedownloader-0.1.0a6/docs/index.rst
--rw-r--r--   0 churas     (504) staff       (20)     1254 2023-05-03 22:57:03.000000 cellmaps_imagedownloader-0.1.0a6/docs/installation.rst
--rw-r--r--   0 churas     (504) staff       (20)      472 2023-05-03 22:57:03.000000 cellmaps_imagedownloader-0.1.0a6/docs/integrationtesting.rst
--rw-r--r--   0 churas     (504) staff       (20)      817 2023-02-15 23:31:37.000000 cellmaps_imagedownloader-0.1.0a6/docs/make.bat
--rw-r--r--   0 churas     (504) staff       (20)       83 2023-05-22 23:09:36.000000 cellmaps_imagedownloader-0.1.0a6/docs/modules.rst
--rw-r--r--   0 churas     (504) staff       (20)     4424 2023-05-03 22:57:03.000000 cellmaps_imagedownloader-0.1.0a6/docs/newrelease.rst
--rw-r--r--   0 churas     (504) staff       (20)      794 2023-05-03 22:57:03.000000 cellmaps_imagedownloader-0.1.0a6/docs/pypircfile.rst
--rw-r--r--   0 churas     (504) staff       (20)      739 2023-05-03 22:57:03.000000 cellmaps_imagedownloader-0.1.0a6/docs/usage.rst
--rw-r--r--   0 churas     (504) staff       (20)      817 2023-02-15 23:31:37.000000 cellmaps_imagedownloader-0.1.0a6/docs/versioningscheme.rst
--rw-r--r--   0 churas     (504) staff       (20)      407 2023-07-17 19:13:47.117022 cellmaps_imagedownloader-0.1.0a6/setup.cfg
--rw-r--r--   0 churas     (504) staff       (20)     2242 2023-07-17 19:13:09.000000 cellmaps_imagedownloader-0.1.0a6/setup.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-17 19:13:47.115487 cellmaps_imagedownloader-0.1.0a6/tests/
--rw-r--r--   0 churas     (504) staff       (20)       79 2023-05-03 22:51:16.000000 cellmaps_imagedownloader-0.1.0a6/tests/__init__.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-17 19:13:47.116033 cellmaps_imagedownloader-0.1.0a6/tests/data/
--rw-r--r--   0 churas     (504) staff       (20)      166 2023-05-22 20:49:48.000000 cellmaps_imagedownloader-0.1.0a6/tests/data/test_single_sample.tsv
--rw-r--r--   0 churas     (504) staff       (20)      122 2023-05-22 20:51:02.000000 cellmaps_imagedownloader-0.1.0a6/tests/data/test_single_unique.tsv
--rw-r--r--   0 churas     (504) staff       (20)     1429 2023-06-14 20:42:24.000000 cellmaps_imagedownloader-0.1.0a6/tests/test_cellmaps_imagedownloadercmd.py
--rw-r--r--   0 churas     (504) staff       (20)    26236 2023-07-17 19:13:31.000000 cellmaps_imagedownloader-0.1.0a6/tests/test_cellmapsimagedownloader.py
--rw-r--r--   0 churas     (504) staff       (20)      896 2023-07-17 19:13:31.000000 cellmaps_imagedownloader-0.1.0a6/tests/test_genenodegenerator.py
--rw-r--r--   0 churas     (504) staff       (20)     2739 2023-06-14 20:42:15.000000 cellmaps_imagedownloader-0.1.0a6/tests/test_genequery.py
--rw-r--r--   0 churas     (504) staff       (20)     4286 2023-07-17 19:13:31.000000 cellmaps_imagedownloader-0.1.0a6/tests/test_imagedownloadtuplegenerator.py
--rw-r--r--   0 churas     (504) staff       (20)    20366 2023-07-17 19:13:31.000000 cellmaps_imagedownloader-0.1.0a6/tests/test_imagegenenodegenerator.py
--rw-r--r--   0 churas     (504) staff       (20)      817 2023-05-03 22:57:03.000000 cellmaps_imagedownloader-0.1.0a6/tests/test_integration_cellmaps_downloader.py
--rw-r--r--   0 churas     (504) staff       (20)     1018 2023-06-14 20:38:55.000000 cellmaps_imagedownloader-0.1.0a6/tests/test_multiprocessimagedownloader.py
--rw-r--r--   0 churas     (504) staff       (20)     2447 2023-07-17 19:13:31.000000 cellmaps_imagedownloader-0.1.0a6/tests/test_proteinatlasimageurlreader.py
--rw-r--r--   0 churas     (504) staff       (20)     3639 2023-07-17 19:13:31.000000 cellmaps_imagedownloader-0.1.0a6/tests/test_proteinatlasreader.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-01 20:07:35.281376 cellmaps_imagedownloader-0.1.0a7/
+-rw-r--r--   0 churas     (504) staff       (20)      266 2023-07-17 19:13:09.000000 cellmaps_imagedownloader-0.1.0a7/AUTHORS.rst
+-rw-r--r--   0 churas     (504) staff       (20)     3731 2023-05-03 22:51:16.000000 cellmaps_imagedownloader-0.1.0a7/CONTRIBUTING.rst
+-rw-r--r--   0 churas     (504) staff       (20)       89 2023-05-11 22:14:34.000000 cellmaps_imagedownloader-0.1.0a7/HISTORY.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1102 2023-02-15 23:31:37.000000 cellmaps_imagedownloader-0.1.0a7/LICENSE
+-rw-r--r--   0 churas     (504) staff       (20)      262 2023-02-15 23:31:37.000000 cellmaps_imagedownloader-0.1.0a7/MANIFEST.in
+-rw-r--r--   0 churas     (504) staff       (20)     5422 2023-08-01 20:07:35.281506 cellmaps_imagedownloader-0.1.0a7/PKG-INFO
+-rw-r--r--   0 churas     (504) staff       (20)     3453 2023-08-01 19:06:46.000000 cellmaps_imagedownloader-0.1.0a7/README.rst
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-01 20:07:35.269744 cellmaps_imagedownloader-0.1.0a7/cellmaps_imagedownloader/
+-rw-r--r--   0 churas     (504) staff       (20)      354 2023-08-01 20:07:18.000000 cellmaps_imagedownloader-0.1.0a7/cellmaps_imagedownloader/__init__.py
+-rw-r--r--   0 churas     (504) staff       (20)    11032 2023-08-01 20:07:18.000000 cellmaps_imagedownloader-0.1.0a7/cellmaps_imagedownloader/cellmaps_imagedownloadercmd.py
+-rw-r--r--   0 churas     (504) staff       (20)      145 2023-05-03 22:51:16.000000 cellmaps_imagedownloader-0.1.0a7/cellmaps_imagedownloader/exceptions.py
+-rw-r--r--   0 churas     (504) staff       (20)    16811 2023-07-17 19:13:31.000000 cellmaps_imagedownloader-0.1.0a7/cellmaps_imagedownloader/gene.py
+-rw-r--r--   0 churas     (504) staff       (20)     7444 2023-08-01 20:07:18.000000 cellmaps_imagedownloader-0.1.0a7/cellmaps_imagedownloader/proteinatlas.py
+-rw-r--r--   0 churas     (504) staff       (20)    29631 2023-07-17 19:13:31.000000 cellmaps_imagedownloader-0.1.0a7/cellmaps_imagedownloader/runner.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-01 20:07:35.271942 cellmaps_imagedownloader-0.1.0a7/cellmaps_imagedownloader.egg-info/
+-rw-r--r--   0 churas     (504) staff       (20)     5422 2023-08-01 20:07:35.000000 cellmaps_imagedownloader-0.1.0a7/cellmaps_imagedownloader.egg-info/PKG-INFO
+-rw-r--r--   0 churas     (504) staff       (20)     1517 2023-08-01 20:07:35.000000 cellmaps_imagedownloader-0.1.0a7/cellmaps_imagedownloader.egg-info/SOURCES.txt
+-rw-r--r--   0 churas     (504) staff       (20)        1 2023-08-01 20:07:35.000000 cellmaps_imagedownloader-0.1.0a7/cellmaps_imagedownloader.egg-info/dependency_links.txt
+-rw-r--r--   0 churas     (504) staff       (20)        1 2023-08-01 20:07:35.000000 cellmaps_imagedownloader-0.1.0a7/cellmaps_imagedownloader.egg-info/not-zip-safe
+-rw-r--r--   0 churas     (504) staff       (20)       36 2023-08-01 20:07:35.000000 cellmaps_imagedownloader-0.1.0a7/cellmaps_imagedownloader.egg-info/requires.txt
+-rw-r--r--   0 churas     (504) staff       (20)       25 2023-08-01 20:07:35.000000 cellmaps_imagedownloader-0.1.0a7/cellmaps_imagedownloader.egg-info/top_level.txt
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-01 20:07:35.277532 cellmaps_imagedownloader-0.1.0a7/docs/
+-rw-r--r--   0 churas     (504) staff       (20)      625 2023-05-03 22:57:03.000000 cellmaps_imagedownloader-0.1.0a7/docs/Makefile
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-01 20:07:35.264085 cellmaps_imagedownloader-0.1.0a7/docs/_build/
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-01 20:07:35.264156 cellmaps_imagedownloader-0.1.0a7/docs/_build/html/
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-01 20:07:35.278408 cellmaps_imagedownloader-0.1.0a7/docs/_build/html/_static/
+-rw-r--r--   0 churas     (504) staff       (20)      286 2023-05-02 22:49:28.000000 cellmaps_imagedownloader-0.1.0a7/docs/_build/html/_static/file.png
+-rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_imagedownloader-0.1.0a7/docs/_build/html/_static/minus.png
+-rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_imagedownloader-0.1.0a7/docs/_build/html/_static/plus.png
+-rw-r--r--   0 churas     (504) staff       (20)       28 2023-02-15 23:31:37.000000 cellmaps_imagedownloader-0.1.0a7/docs/authors.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1027 2023-05-03 22:58:28.000000 cellmaps_imagedownloader-0.1.0a7/docs/cellmaps_imagedownloader.rst
+-rwxr-xr-x   0 churas     (504) staff       (20)     6214 2023-05-22 22:22:34.000000 cellmaps_imagedownloader-0.1.0a7/docs/conf.py
+-rw-r--r--   0 churas     (504) staff       (20)       33 2023-02-15 23:31:37.000000 cellmaps_imagedownloader-0.1.0a7/docs/contributing.rst
+-rw-r--r--   0 churas     (504) staff       (20)      174 2023-02-15 23:31:37.000000 cellmaps_imagedownloader-0.1.0a7/docs/devbranches.rst
+-rw-r--r--   0 churas     (504) staff       (20)      292 2023-05-03 22:57:03.000000 cellmaps_imagedownloader-0.1.0a7/docs/developer.rst
+-rw-r--r--   0 churas     (504) staff       (20)       28 2023-02-15 23:31:37.000000 cellmaps_imagedownloader-0.1.0a7/docs/history.rst
+-rw-r--r--   0 churas     (504) staff       (20)      819 2023-08-01 19:06:46.000000 cellmaps_imagedownloader-0.1.0a7/docs/index.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1254 2023-05-03 22:57:03.000000 cellmaps_imagedownloader-0.1.0a7/docs/installation.rst
+-rw-r--r--   0 churas     (504) staff       (20)      472 2023-05-03 22:57:03.000000 cellmaps_imagedownloader-0.1.0a7/docs/integrationtesting.rst
+-rw-r--r--   0 churas     (504) staff       (20)      817 2023-02-15 23:31:37.000000 cellmaps_imagedownloader-0.1.0a7/docs/make.bat
+-rw-r--r--   0 churas     (504) staff       (20)       83 2023-05-22 23:09:36.000000 cellmaps_imagedownloader-0.1.0a7/docs/modules.rst
+-rw-r--r--   0 churas     (504) staff       (20)     4424 2023-05-03 22:57:03.000000 cellmaps_imagedownloader-0.1.0a7/docs/newrelease.rst
+-rw-r--r--   0 churas     (504) staff       (20)      794 2023-05-03 22:57:03.000000 cellmaps_imagedownloader-0.1.0a7/docs/pypircfile.rst
+-rw-r--r--   0 churas     (504) staff       (20)      739 2023-05-03 22:57:03.000000 cellmaps_imagedownloader-0.1.0a7/docs/usage.rst
+-rw-r--r--   0 churas     (504) staff       (20)      817 2023-02-15 23:31:37.000000 cellmaps_imagedownloader-0.1.0a7/docs/versioningscheme.rst
+-rw-r--r--   0 churas     (504) staff       (20)      407 2023-08-01 20:07:35.281952 cellmaps_imagedownloader-0.1.0a7/setup.cfg
+-rw-r--r--   0 churas     (504) staff       (20)     2242 2023-07-17 19:13:09.000000 cellmaps_imagedownloader-0.1.0a7/setup.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-01 20:07:35.280790 cellmaps_imagedownloader-0.1.0a7/tests/
+-rw-r--r--   0 churas     (504) staff       (20)       79 2023-05-03 22:51:16.000000 cellmaps_imagedownloader-0.1.0a7/tests/__init__.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-01 20:07:35.281190 cellmaps_imagedownloader-0.1.0a7/tests/data/
+-rw-r--r--   0 churas     (504) staff       (20)      166 2023-05-22 20:49:48.000000 cellmaps_imagedownloader-0.1.0a7/tests/data/test_single_sample.tsv
+-rw-r--r--   0 churas     (504) staff       (20)      122 2023-05-22 20:51:02.000000 cellmaps_imagedownloader-0.1.0a7/tests/data/test_single_unique.tsv
+-rw-r--r--   0 churas     (504) staff       (20)     1429 2023-06-14 20:42:24.000000 cellmaps_imagedownloader-0.1.0a7/tests/test_cellmaps_imagedownloadercmd.py
+-rw-r--r--   0 churas     (504) staff       (20)    26236 2023-07-17 19:13:31.000000 cellmaps_imagedownloader-0.1.0a7/tests/test_cellmapsimagedownloader.py
+-rw-r--r--   0 churas     (504) staff       (20)      896 2023-07-17 19:13:31.000000 cellmaps_imagedownloader-0.1.0a7/tests/test_genenodegenerator.py
+-rw-r--r--   0 churas     (504) staff       (20)     2739 2023-06-14 20:42:15.000000 cellmaps_imagedownloader-0.1.0a7/tests/test_genequery.py
+-rw-r--r--   0 churas     (504) staff       (20)     4286 2023-07-17 19:13:31.000000 cellmaps_imagedownloader-0.1.0a7/tests/test_imagedownloadtuplegenerator.py
+-rw-r--r--   0 churas     (504) staff       (20)    20366 2023-07-17 19:13:31.000000 cellmaps_imagedownloader-0.1.0a7/tests/test_imagegenenodegenerator.py
+-rw-r--r--   0 churas     (504) staff       (20)      817 2023-05-03 22:57:03.000000 cellmaps_imagedownloader-0.1.0a7/tests/test_integration_cellmaps_downloader.py
+-rw-r--r--   0 churas     (504) staff       (20)     1018 2023-06-14 20:38:55.000000 cellmaps_imagedownloader-0.1.0a7/tests/test_multiprocessimagedownloader.py
+-rw-r--r--   0 churas     (504) staff       (20)     2431 2023-08-01 20:07:18.000000 cellmaps_imagedownloader-0.1.0a7/tests/test_proteinatlasimageurlreader.py
+-rw-r--r--   0 churas     (504) staff       (20)     3639 2023-07-17 19:13:31.000000 cellmaps_imagedownloader-0.1.0a7/tests/test_proteinatlasreader.py
```

### Comparing `cellmaps_imagedownloader-0.1.0a6/CONTRIBUTING.rst` & `cellmaps_imagedownloader-0.1.0a7/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_imagedownloader-0.1.0a6/LICENSE` & `cellmaps_imagedownloader-0.1.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `cellmaps_imagedownloader-0.1.0a6/PKG-INFO` & `cellmaps_imagedownloader-0.1.0a7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
 Name: cellmaps_imagedownloader
-Version: 0.1.0a6
+Version: 0.1.0a7
 Summary: A tool to download specified image data from the Human Protein Atlas website using CSV file
 Home-page: https://github.com/idekerlab/cellmaps_imagedownloader
 Author: Ideker Lab CM4AI team
 Author-email: tools@cm4ai.org
 License: MIT license
-Description: =========================
-        cellmaps_imagedownloader
-        =========================
+Description: =============================================
+        Cell Maps ImmunoFluorescent Image Downloader
+        =============================================
         
         
         .. image:: https://img.shields.io/pypi/v/cellmaps_imagedownloader.svg
                 :target: https://pypi.python.org/pypi/cellmaps_imagedownloader
         
         .. image:: https://app.travis-ci.com/idekerlab/cellmaps_imagedownloader.svg?branch=main
             :target: https://app.travis-ci.com/idekerlab/cellmaps_imagedownloader
         
-        .. image:: https://readthedocs.org/projects/cellmaps-downloader/badge/?version=latest
+        .. image:: https://readthedocs.org/projects/cellmaps-imagedownloader/badge/?version=latest
                 :target: https://cellmaps-imagedownloader.readthedocs.io/en/latest/?badge=latest
                 :alt: Documentation Status
         
         
-        Downloads IF data needed for CM4AI MuSIC pipeline
+        Downloads ImmunoFluorescent image data from `Human Protein Atlas <https://www.proteinatlas.org/>`__
+        used by `Cell Maps for AI (CM4AI) <https://cm4ai.org>`__
         
         
         * Free software: MIT license
         * Documentation: https://cellmaps-imagedownloader.readthedocs.io.
         
         
         Dependencies
```

### Comparing `cellmaps_imagedownloader-0.1.0a6/README.rst` & `cellmaps_imagedownloader-0.1.0a7/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,25 @@
-=========================
-cellmaps_imagedownloader
-=========================
+=============================================
+Cell Maps ImmunoFluorescent Image Downloader
+=============================================
 
 
 .. image:: https://img.shields.io/pypi/v/cellmaps_imagedownloader.svg
         :target: https://pypi.python.org/pypi/cellmaps_imagedownloader
 
 .. image:: https://app.travis-ci.com/idekerlab/cellmaps_imagedownloader.svg?branch=main
     :target: https://app.travis-ci.com/idekerlab/cellmaps_imagedownloader
 
-.. image:: https://readthedocs.org/projects/cellmaps-downloader/badge/?version=latest
+.. image:: https://readthedocs.org/projects/cellmaps-imagedownloader/badge/?version=latest
         :target: https://cellmaps-imagedownloader.readthedocs.io/en/latest/?badge=latest
         :alt: Documentation Status
 
 
-Downloads IF data needed for CM4AI MuSIC pipeline
+Downloads ImmunoFluorescent image data from `Human Protein Atlas <https://www.proteinatlas.org/>`__
+used by `Cell Maps for AI (CM4AI) <https://cm4ai.org>`__
 
 
 * Free software: MIT license
 * Documentation: https://cellmaps-imagedownloader.readthedocs.io.
 
 
 Dependencies
```

### Comparing `cellmaps_imagedownloader-0.1.0a6/cellmaps_imagedownloader/cellmaps_imagedownloadercmd.py` & `cellmaps_imagedownloader-0.1.0a7/cellmaps_imagedownloader/cellmaps_imagedownloadercmd.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,15 +54,15 @@
                         help='Path to file containing provenance '
                              'information about input files in JSON format. '
                              'This is required and not including will output '
                              'and error message with example of file')
     parser.add_argument('--image_url', default='https://images.proteinatlas.org',
                         help='Base URL for downloading IF images')
     parser.add_argument('--proteinatlasxml',
-                        default='https://www.proteinatlas.org/download/proteinatlas.xml.gz',
+                        default=ProteinAtlasReader.DEFAULT_PROTEINATLAS_URL,
                         help='URL or path to proteinatlas.xml or proteinatlas.xml.gz file '
                              'used to look for images not found in the standard location '
                              'on HPA')
     parser.add_argument('--fake_images', action='store_true',
                         help='If set, 1st image of each color is downloaded '
                              'and subsequent images are just copies of those '
                              'images')
```

### Comparing `cellmaps_imagedownloader-0.1.0a6/cellmaps_imagedownloader/gene.py` & `cellmaps_imagedownloader-0.1.0a7/cellmaps_imagedownloader/gene.py`

 * *Files identical despite different names*

### Comparing `cellmaps_imagedownloader-0.1.0a6/cellmaps_imagedownloader/proteinatlas.py` & `cellmaps_imagedownloader-0.1.0a7/cellmaps_imagedownloader/proteinatlas.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,25 +14,30 @@
 
 
 class ProteinAtlasReader(object):
     """
     Returns contents of proteinatlas.xml file one
     line at a time
     """
+
+    DEFAULT_PROTEINATLAS_URL = 'https://www.proteinatlas.org/download/proteinatlas.xml.gz'
+
     def __init__(self, outdir=None,
                  proteinatlas=None):
         """
         Constructor
 
         :param outdir: Path to directory where results can be written to
         :type outdir: str
         :param proteinatlas: URL or path to proteinatlas.xml| proteinatlas.xml.gz file
         :type proteinatlas: str
         """
         self._outdir = outdir
+        if proteinatlas is None:
+            self._proteinatlas = ProteinAtlasReader.DEFAULT_PROTEINATLAS_URL
         self._proteinatlas = proteinatlas
 
     def readline(self):
         """
         Generator that returns next line of proteinatlas data
         set via constructor
 
@@ -123,15 +128,15 @@
     def _get_image_id(self, image_url):
         """
 
         :param image_url:
         :return:
         """
         antibody_and_id = '/'.join(image_url.split('/')[-2:])
-        return antibody_and_id[:antibody_and_id.index('_blue')+1]
+        return '_'.join(antibody_and_id.split('_')[0:3]) + '_'
 
     def get_next_image_id_and_url(self):
         """
 
         :return: (image id, image_url)
         :rtype: tuple
         """
```

### Comparing `cellmaps_imagedownloader-0.1.0a6/cellmaps_imagedownloader/runner.py` & `cellmaps_imagedownloader-0.1.0a7/cellmaps_imagedownloader/runner.py`

 * *Files identical despite different names*

### Comparing `cellmaps_imagedownloader-0.1.0a6/cellmaps_imagedownloader.egg-info/PKG-INFO` & `cellmaps_imagedownloader-0.1.0a7/cellmaps_imagedownloader.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
 Name: cellmaps-imagedownloader
-Version: 0.1.0a6
+Version: 0.1.0a7
 Summary: A tool to download specified image data from the Human Protein Atlas website using CSV file
 Home-page: https://github.com/idekerlab/cellmaps_imagedownloader
 Author: Ideker Lab CM4AI team
 Author-email: tools@cm4ai.org
 License: MIT license
-Description: =========================
-        cellmaps_imagedownloader
-        =========================
+Description: =============================================
+        Cell Maps ImmunoFluorescent Image Downloader
+        =============================================
         
         
         .. image:: https://img.shields.io/pypi/v/cellmaps_imagedownloader.svg
                 :target: https://pypi.python.org/pypi/cellmaps_imagedownloader
         
         .. image:: https://app.travis-ci.com/idekerlab/cellmaps_imagedownloader.svg?branch=main
             :target: https://app.travis-ci.com/idekerlab/cellmaps_imagedownloader
         
-        .. image:: https://readthedocs.org/projects/cellmaps-downloader/badge/?version=latest
+        .. image:: https://readthedocs.org/projects/cellmaps-imagedownloader/badge/?version=latest
                 :target: https://cellmaps-imagedownloader.readthedocs.io/en/latest/?badge=latest
                 :alt: Documentation Status
         
         
-        Downloads IF data needed for CM4AI MuSIC pipeline
+        Downloads ImmunoFluorescent image data from `Human Protein Atlas <https://www.proteinatlas.org/>`__
+        used by `Cell Maps for AI (CM4AI) <https://cm4ai.org>`__
         
         
         * Free software: MIT license
         * Documentation: https://cellmaps-imagedownloader.readthedocs.io.
         
         
         Dependencies
```

### Comparing `cellmaps_imagedownloader-0.1.0a6/cellmaps_imagedownloader.egg-info/SOURCES.txt` & `cellmaps_imagedownloader-0.1.0a7/cellmaps_imagedownloader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellmaps_imagedownloader-0.1.0a6/docs/Makefile` & `cellmaps_imagedownloader-0.1.0a7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cellmaps_imagedownloader-0.1.0a6/docs/cellmaps_imagedownloader.rst` & `cellmaps_imagedownloader-0.1.0a7/docs/cellmaps_imagedownloader.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_imagedownloader-0.1.0a6/docs/conf.py` & `cellmaps_imagedownloader-0.1.0a7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cellmaps_imagedownloader-0.1.0a6/docs/installation.rst` & `cellmaps_imagedownloader-0.1.0a7/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_imagedownloader-0.1.0a6/docs/make.bat` & `cellmaps_imagedownloader-0.1.0a7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cellmaps_imagedownloader-0.1.0a6/docs/newrelease.rst` & `cellmaps_imagedownloader-0.1.0a7/docs/newrelease.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_imagedownloader-0.1.0a6/docs/pypircfile.rst` & `cellmaps_imagedownloader-0.1.0a7/docs/pypircfile.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_imagedownloader-0.1.0a6/docs/usage.rst` & `cellmaps_imagedownloader-0.1.0a7/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_imagedownloader-0.1.0a6/docs/versioningscheme.rst` & `cellmaps_imagedownloader-0.1.0a7/docs/versioningscheme.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_imagedownloader-0.1.0a6/setup.py` & `cellmaps_imagedownloader-0.1.0a7/setup.py`

 * *Files identical despite different names*

### Comparing `cellmaps_imagedownloader-0.1.0a6/tests/test_cellmaps_imagedownloadercmd.py` & `cellmaps_imagedownloader-0.1.0a7/tests/test_cellmaps_imagedownloadercmd.py`

 * *Files identical despite different names*

### Comparing `cellmaps_imagedownloader-0.1.0a6/tests/test_cellmapsimagedownloader.py` & `cellmaps_imagedownloader-0.1.0a7/tests/test_cellmapsimagedownloader.py`

 * *Files identical despite different names*

### Comparing `cellmaps_imagedownloader-0.1.0a6/tests/test_genenodegenerator.py` & `cellmaps_imagedownloader-0.1.0a7/tests/test_genenodegenerator.py`

 * *Files identical despite different names*

### Comparing `cellmaps_imagedownloader-0.1.0a6/tests/test_genequery.py` & `cellmaps_imagedownloader-0.1.0a7/tests/test_genequery.py`

 * *Files identical despite different names*

### Comparing `cellmaps_imagedownloader-0.1.0a6/tests/test_imagedownloadtuplegenerator.py` & `cellmaps_imagedownloader-0.1.0a7/tests/test_imagedownloadtuplegenerator.py`

 * *Files identical despite different names*

### Comparing `cellmaps_imagedownloader-0.1.0a6/tests/test_imagegenenodegenerator.py` & `cellmaps_imagedownloader-0.1.0a7/tests/test_imagegenenodegenerator.py`

 * *Files identical despite different names*

### Comparing `cellmaps_imagedownloader-0.1.0a6/tests/test_integration_cellmaps_downloader.py` & `cellmaps_imagedownloader-0.1.0a7/tests/test_integration_cellmaps_downloader.py`

 * *Files identical despite different names*

### Comparing `cellmaps_imagedownloader-0.1.0a6/tests/test_multiprocessimagedownloader.py` & `cellmaps_imagedownloader-0.1.0a7/tests/test_multiprocessimagedownloader.py`

 * *Files identical despite different names*

### Comparing `cellmaps_imagedownloader-0.1.0a6/tests/test_proteinatlasimageurlreader.py` & `cellmaps_imagedownloader-0.1.0a7/tests/test_proteinatlasimageurlreader.py`

 * *Files 8% similar despite different names*

```diff
@@ -136,18 +136,17 @@
 00000870: 2f34 3130 392f 3138 3332 5f43 315f 325f  /4109/1832_C1_2_
 00000880: 626c 7565 5f27 0a20 2020 2020 2020 2020  blue_'.         
 00000890: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000008a0: 2027 7265 645f 6772 6565 6e2e 6a70 6727   'red_green.jpg'
 000008b0: 292c 2072 6573 5b30 5d29 0a20 2020 2020  ), res[0]).     
 000008c0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
 000008d0: 7561 6c28 2827 3431 3039 2f31 3834 335f  ual(('4109/1843_
-000008e0: 4232 5f31 375f 6372 3561 6639 3731 6132  B2_17_cr5af971a2
-000008f0: 3633 3836 345f 272c 0a20 2020 2020 2020  63864_',.       
-00000900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000910: 2020 2027 6874 7470 3a2f 2f69 6d61 6765     'http://image
-00000920: 732e 7072 6f74 6569 6e61 746c 6173 2e6f  s.proteinatlas.o
-00000930: 7267 2f34 3130 392f 3138 3433 5f42 325f  rg/4109/1843_B2_
-00000940: 3137 5f27 0a20 2020 2020 2020 2020 2020  17_'.           
-00000950: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00000960: 6372 3561 6639 3731 6132 3633 3836 345f  cr5af971a263864_
-00000970: 626c 7565 5f72 6564 5f67 7265 656e 2e6a  blue_red_green.j
-00000980: 7067 2729 2c20 7265 735b 315d 290a 0a    pg'), res[1])..
+000008e0: 4232 5f31 375f 272c 0a20 2020 2020 2020  B2_17_',.       
+000008f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000900: 2020 2027 6874 7470 3a2f 2f69 6d61 6765     'http://image
+00000910: 732e 7072 6f74 6569 6e61 746c 6173 2e6f  s.proteinatlas.o
+00000920: 7267 2f34 3130 392f 3138 3433 5f42 325f  rg/4109/1843_B2_
+00000930: 3137 5f27 0a20 2020 2020 2020 2020 2020  17_'.           
+00000940: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00000950: 6372 3561 6639 3731 6132 3633 3836 345f  cr5af971a263864_
+00000960: 626c 7565 5f72 6564 5f67 7265 656e 2e6a  blue_red_green.j
+00000970: 7067 2729 2c20 7265 735b 315d 290a 0a    pg'), res[1])..
```

### Comparing `cellmaps_imagedownloader-0.1.0a6/tests/test_proteinatlasreader.py` & `cellmaps_imagedownloader-0.1.0a7/tests/test_proteinatlasreader.py`

 * *Files identical despite different names*

