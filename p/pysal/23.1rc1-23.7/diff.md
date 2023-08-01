# Comparing `tmp/pysal-23.1rc1.tar.gz` & `tmp/pysal-23.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysal-23.1rc1.tar", last modified: Fri Jan 27 21:21:13 2023, max compression
+gzip compressed data, was "pysal-23.7.tar", last modified: Tue Aug  1 02:39:33 2023, max compression
```

## Comparing `pysal-23.1rc1.tar` & `pysal-23.7.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 21:21:13.831461 pysal-23.1rc1/
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-01-27 21:20:36.000000 pysal-23.1rc1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-01-27 21:20:36.000000 pysal-23.1rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13893 2023-01-27 21:21:13.831461 pysal-23.1rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12966 2023-01-27 21:20:36.000000 pysal-23.1rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 21:21:13.831461 pysal-23.1rc1/pysal/
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-01-27 21:20:36.000000 pysal-23.1rc1/pysal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-01-27 21:21:13.831461 pysal-23.1rc1/pysal/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-01-27 21:20:36.000000 pysal-23.1rc1/pysal/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 21:21:13.831461 pysal-23.1rc1/pysal/explore/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-27 21:20:36.000000 pysal-23.1rc1/pysal/explore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 21:21:13.831461 pysal-23.1rc1/pysal/explore/esda/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-01-27 21:20:36.000000 pysal-23.1rc1/pysal/explore/esda/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 21:21:13.831461 pysal-23.1rc1/pysal/explore/giddy/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-01-27 21:20:36.000000 pysal-23.1rc1/pysal/explore/giddy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 21:21:13.831461 pysal-23.1rc1/pysal/explore/inequality/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-01-27 21:20:36.000000 pysal-23.1rc1/pysal/explore/inequality/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 21:21:13.831461 pysal-23.1rc1/pysal/explore/momepy/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-01-27 21:20:36.000000 pysal-23.1rc1/pysal/explore/momepy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 21:21:13.831461 pysal-23.1rc1/pysal/explore/pointpats/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-01-27 21:20:36.000000 pysal-23.1rc1/pysal/explore/pointpats/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 21:21:13.831461 pysal-23.1rc1/pysal/explore/segregation/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-01-27 21:20:36.000000 pysal-23.1rc1/pysal/explore/segregation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 21:21:13.831461 pysal-23.1rc1/pysal/explore/spaghetti/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-01-27 21:20:36.000000 pysal-23.1rc1/pysal/explore/spaghetti/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-01-27 21:20:36.000000 pysal-23.1rc1/pysal/frozen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 21:21:13.831461 pysal-23.1rc1/pysal/lib/
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-01-27 21:20:36.000000 pysal-23.1rc1/pysal/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-01-27 21:20:36.000000 pysal-23.1rc1/pysal/lib/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 21:21:13.831461 pysal-23.1rc1/pysal/lib/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-01-27 21:20:36.000000 pysal-23.1rc1/pysal/lib/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 21:21:13.831461 pysal-23.1rc1/pysal/model/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-01-27 21:20:36.000000 pysal-23.1rc1/pysal/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 21:21:13.831461 pysal-23.1rc1/pysal/model/access/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-01-27 21:20:36.000000 pysal-23.1rc1/pysal/model/access/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 21:21:13.831461 pysal-23.1rc1/pysal/model/mgwr/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-01-27 21:20:36.000000 pysal-23.1rc1/pysal/model/mgwr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 21:21:13.831461 pysal-23.1rc1/pysal/model/spglm/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-01-27 21:20:36.000000 pysal-23.1rc1/pysal/model/spglm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 21:21:13.831461 pysal-23.1rc1/pysal/model/spint/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-01-27 21:20:36.000000 pysal-23.1rc1/pysal/model/spint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 21:21:13.831461 pysal-23.1rc1/pysal/model/spopt/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-27 21:20:36.000000 pysal-23.1rc1/pysal/model/spopt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 21:21:13.831461 pysal-23.1rc1/pysal/model/spreg/
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-01-27 21:20:36.000000 pysal-23.1rc1/pysal/model/spreg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 21:21:13.831461 pysal-23.1rc1/pysal/model/spvcm/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-01-27 21:20:36.000000 pysal-23.1rc1/pysal/model/spvcm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 21:21:13.831461 pysal-23.1rc1/pysal/model/tobler/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-27 21:20:36.000000 pysal-23.1rc1/pysal/model/tobler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 21:21:13.831461 pysal-23.1rc1/pysal/viz/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-01-27 21:20:36.000000 pysal-23.1rc1/pysal/viz/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 21:21:13.831461 pysal-23.1rc1/pysal/viz/mapclassify/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-01-27 21:20:36.000000 pysal-23.1rc1/pysal/viz/mapclassify/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 21:21:13.831461 pysal-23.1rc1/pysal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13893 2023-01-27 21:21:13.000000 pysal-23.1rc1/pysal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-01-27 21:21:13.000000 pysal-23.1rc1/pysal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-27 21:21:13.000000 pysal-23.1rc1/pysal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-01-27 21:21:13.000000 pysal-23.1rc1/pysal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-01-27 21:21:13.000000 pysal-23.1rc1/pysal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-01-27 21:20:36.000000 pysal-23.1rc1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-01-27 21:20:36.000000 pysal-23.1rc1/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-01-27 21:20:36.000000 pysal-23.1rc1/requirements_docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-01-27 21:20:36.000000 pysal-23.1rc1/requirements_plus.txt
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-01-27 21:21:13.831461 pysal-23.1rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-01-27 21:20:36.000000 pysal-23.1rc1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    78254 2023-01-27 21:20:36.000000 pysal-23.1rc1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:39:33.516480 pysal-23.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-08-01 02:38:59.000000 pysal-23.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-01 02:38:59.000000 pysal-23.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13890 2023-08-01 02:39:33.516480 pysal-23.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12966 2023-08-01 02:38:59.000000 pysal-23.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:39:33.516480 pysal-23.7/pysal/
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-08-01 02:38:59.000000 pysal-23.7/pysal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-08-01 02:39:33.516480 pysal-23.7/pysal/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-08-01 02:38:59.000000 pysal-23.7/pysal/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:39:33.508479 pysal-23.7/pysal/explore/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-08-01 02:38:59.000000 pysal-23.7/pysal/explore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:39:33.508479 pysal-23.7/pysal/explore/esda/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-08-01 02:38:59.000000 pysal-23.7/pysal/explore/esda/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:39:33.512479 pysal-23.7/pysal/explore/giddy/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-08-01 02:38:59.000000 pysal-23.7/pysal/explore/giddy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:39:33.512479 pysal-23.7/pysal/explore/inequality/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-08-01 02:38:59.000000 pysal-23.7/pysal/explore/inequality/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:39:33.512479 pysal-23.7/pysal/explore/momepy/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-01 02:38:59.000000 pysal-23.7/pysal/explore/momepy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:39:33.512479 pysal-23.7/pysal/explore/pointpats/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-08-01 02:38:59.000000 pysal-23.7/pysal/explore/pointpats/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:39:33.512479 pysal-23.7/pysal/explore/segregation/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-08-01 02:38:59.000000 pysal-23.7/pysal/explore/segregation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:39:33.512479 pysal-23.7/pysal/explore/spaghetti/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-08-01 02:38:59.000000 pysal-23.7/pysal/explore/spaghetti/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-08-01 02:38:59.000000 pysal-23.7/pysal/frozen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:39:33.512479 pysal-23.7/pysal/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-08-01 02:38:59.000000 pysal-23.7/pysal/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-08-01 02:38:59.000000 pysal-23.7/pysal/lib/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:39:33.512479 pysal-23.7/pysal/lib/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-08-01 02:38:59.000000 pysal-23.7/pysal/lib/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:39:33.512479 pysal-23.7/pysal/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-08-01 02:38:59.000000 pysal-23.7/pysal/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:39:33.512479 pysal-23.7/pysal/model/access/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-08-01 02:38:59.000000 pysal-23.7/pysal/model/access/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:39:33.512479 pysal-23.7/pysal/model/mgwr/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-08-01 02:38:59.000000 pysal-23.7/pysal/model/mgwr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:39:33.512479 pysal-23.7/pysal/model/spglm/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-01 02:38:59.000000 pysal-23.7/pysal/model/spglm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:39:33.512479 pysal-23.7/pysal/model/spint/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-08-01 02:38:59.000000 pysal-23.7/pysal/model/spint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:39:33.512479 pysal-23.7/pysal/model/spopt/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-01 02:38:59.000000 pysal-23.7/pysal/model/spopt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:39:33.512479 pysal-23.7/pysal/model/spreg/
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-08-01 02:38:59.000000 pysal-23.7/pysal/model/spreg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:39:33.512479 pysal-23.7/pysal/model/spvcm/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-08-01 02:38:59.000000 pysal-23.7/pysal/model/spvcm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:39:33.512479 pysal-23.7/pysal/model/tobler/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-08-01 02:38:59.000000 pysal-23.7/pysal/model/tobler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:39:33.516480 pysal-23.7/pysal/viz/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-01 02:38:59.000000 pysal-23.7/pysal/viz/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:39:33.516480 pysal-23.7/pysal/viz/mapclassify/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-08-01 02:38:59.000000 pysal-23.7/pysal/viz/mapclassify/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:39:33.508479 pysal-23.7/pysal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13890 2023-08-01 02:39:33.000000 pysal-23.7/pysal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-08-01 02:39:33.000000 pysal-23.7/pysal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 02:39:33.000000 pysal-23.7/pysal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-08-01 02:39:33.000000 pysal-23.7/pysal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-01 02:39:33.000000 pysal-23.7/pysal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-08-01 02:38:59.000000 pysal-23.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-08-01 02:38:59.000000 pysal-23.7/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-08-01 02:38:59.000000 pysal-23.7/requirements_docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-08-01 02:38:59.000000 pysal-23.7/requirements_plus.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-08-01 02:39:33.516480 pysal-23.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-08-01 02:38:59.000000 pysal-23.7/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78254 2023-08-01 02:38:59.000000 pysal-23.7/versioneer.py
```

### Comparing `pysal-23.1rc1/LICENSE.txt` & `pysal-23.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pysal-23.1rc1/PKG-INFO` & `pysal-23.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysal
-Version: 23.1rc1
+Version: 23.7
 Summary: A library of spatial analysis functions.
 Home-page: http://pysal.org
 Download-URL: https://pypi.python.org/pypi/pysal
 Maintainer: PySAL Developers
 Maintainer-email: pysal-dev@googlegroups.com
 License: BSD
 Keywords: spatial statistics
```

### Comparing `pysal-23.1rc1/README.md` & `pysal-23.7/README.md`

 * *Files identical despite different names*

### Comparing `pysal-23.1rc1/pysal/__init__.py` & `pysal-23.7/pysal/__init__.py`

 * *Files identical despite different names*

### Comparing `pysal-23.1rc1/pysal/base.py` & `pysal-23.7/pysal/base.py`

 * *Files identical despite different names*

### Comparing `pysal-23.1rc1/pysal/explore/esda/__init__.py` & `pysal-23.7/pysal/explore/esda/__init__.py`

 * *Files identical despite different names*

### Comparing `pysal-23.1rc1/pysal/lib/__init__.py` & `pysal-23.7/pysal/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `pysal-23.1rc1/pysal/lib/common.py` & `pysal-23.7/pysal/lib/common.py`

 * *Files identical despite different names*

### Comparing `pysal-23.1rc1/pysal/model/spreg/__init__.py` & `pysal-23.7/pysal/model/spreg/__init__.py`

 * *Files identical despite different names*

### Comparing `pysal-23.1rc1/pysal.egg-info/PKG-INFO` & `pysal-23.7/pysal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysal
-Version: 23.1rc1
+Version: 23.7
 Summary: A library of spatial analysis functions.
 Home-page: http://pysal.org
 Download-URL: https://pypi.python.org/pypi/pysal
 Maintainer: PySAL Developers
 Maintainer-email: pysal-dev@googlegroups.com
 License: BSD
 Keywords: spatial statistics
```

### Comparing `pysal-23.1rc1/pysal.egg-info/SOURCES.txt` & `pysal-23.7/pysal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pysal-23.1rc1/pysal.egg-info/requires.txt` & `pysal-23.7/pysal.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pysal-23.1rc1/setup.py` & `pysal-23.7/setup.py`

 * *Files identical despite different names*

### Comparing `pysal-23.1rc1/versioneer.py` & `pysal-23.7/versioneer.py`

 * *Files identical despite different names*

