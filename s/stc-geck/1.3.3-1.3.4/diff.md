# Comparing `tmp/stc-geck-1.3.3.tar.gz` & `tmp/stc-geck-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stc-geck-1.3.3.tar", last modified: Sun Jul 23 16:44:26 2023, max compression
+gzip compressed data, was "stc-geck-1.3.4.tar", last modified: Tue Aug  1 14:43:04 2023, max compression
```

## Comparing `stc-geck-1.3.3.tar` & `stc-geck-1.3.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-23 16:44:26.322884 stc-geck-1.3.3/
--rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 stc-geck-1.3.3/MANIFEST.in
--rw-r--r--   0 pasha      (501) staff       (20)     1033 2023-07-23 16:44:26.321935 stc-geck-1.3.3/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)      688 2023-07-22 19:34:42.000000 stc-geck-1.3.3/README.md
--rw-r--r--   0 pasha      (501) staff       (20)      600 2023-07-23 16:43:55.000000 stc-geck-1.3.3/pyproject.toml
--rw-r--r--   0 pasha      (501) staff       (20)      161 2023-07-20 13:58:38.000000 stc-geck-1.3.3/requirements.txt
--rw-r--r--   0 pasha      (501) staff       (20)       38 2023-07-23 16:44:26.323155 stc-geck-1.3.3/setup.cfg
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-23 16:44:26.315554 stc-geck-1.3.3/stc_geck/
--rw-r--r--   0 pasha      (501) staff       (20)        0 2023-07-19 19:56:31.000000 stc-geck-1.3.3/stc_geck/__init__.py
--rw-r--r--   0 pasha      (501) staff       (20)      923 2023-07-06 11:45:56.000000 stc-geck-1.3.3/stc_geck/advices.py
--rw-r--r--   0 pasha      (501) staff       (20)     7346 2023-07-23 16:43:55.000000 stc-geck-1.3.3/stc_geck/cli.py
--rw-r--r--   0 pasha      (501) staff       (20)     7231 2023-07-23 16:43:55.000000 stc-geck-1.3.3/stc_geck/client.py
--rw-r--r--   0 pasha      (501) staff       (20)     1877 2023-07-22 08:16:03.000000 stc-geck-1.3.3/stc_geck/utils.py
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-23 16:44:26.320711 stc-geck-1.3.3/stc_geck.egg-info/
--rw-r--r--   0 pasha      (501) staff       (20)     1033 2023-07-23 16:44:26.000000 stc-geck-1.3.3/stc_geck.egg-info/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)      341 2023-07-23 16:44:26.000000 stc-geck-1.3.3/stc_geck.egg-info/SOURCES.txt
--rw-r--r--   0 pasha      (501) staff       (20)        1 2023-07-23 16:44:26.000000 stc-geck-1.3.3/stc_geck.egg-info/dependency_links.txt
--rw-r--r--   0 pasha      (501) staff       (20)       43 2023-07-23 16:44:26.000000 stc-geck-1.3.3/stc_geck.egg-info/entry_points.txt
--rw-r--r--   0 pasha      (501) staff       (20)      162 2023-07-23 16:44:26.000000 stc-geck-1.3.3/stc_geck.egg-info/requires.txt
--rw-r--r--   0 pasha      (501) staff       (20)        9 2023-07-23 16:44:26.000000 stc-geck-1.3.3/stc_geck.egg-info/top_level.txt
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-01 14:43:04.371915 stc-geck-1.3.4/
+-rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 stc-geck-1.3.4/MANIFEST.in
+-rw-r--r--   0 pasha      (501) staff       (20)     7330 2023-08-01 14:43:04.371614 stc-geck-1.3.4/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)     6985 2023-07-23 19:18:57.000000 stc-geck-1.3.4/README.md
+-rw-r--r--   0 pasha      (501) staff       (20)      600 2023-08-01 14:41:13.000000 stc-geck-1.3.4/pyproject.toml
+-rw-r--r--   0 pasha      (501) staff       (20)      161 2023-07-30 14:20:06.000000 stc-geck-1.3.4/requirements.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       38 2023-08-01 14:43:04.372036 stc-geck-1.3.4/setup.cfg
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-01 14:43:04.368168 stc-geck-1.3.4/stc_geck/
+-rw-r--r--   0 pasha      (501) staff       (20)        0 2023-07-19 19:56:31.000000 stc-geck-1.3.4/stc_geck/__init__.py
+-rw-r--r--   0 pasha      (501) staff       (20)      923 2023-07-06 11:45:56.000000 stc-geck-1.3.4/stc_geck/advices.py
+-rw-r--r--   0 pasha      (501) staff       (20)     7346 2023-07-23 18:24:49.000000 stc-geck-1.3.4/stc_geck/cli.py
+-rw-r--r--   0 pasha      (501) staff       (20)     7231 2023-07-23 18:24:49.000000 stc-geck-1.3.4/stc_geck/client.py
+-rw-r--r--   0 pasha      (501) staff       (20)     1877 2023-07-22 08:16:03.000000 stc-geck-1.3.4/stc_geck/utils.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-01 14:43:04.371119 stc-geck-1.3.4/stc_geck.egg-info/
+-rw-r--r--   0 pasha      (501) staff       (20)     7330 2023-08-01 14:43:04.000000 stc-geck-1.3.4/stc_geck.egg-info/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)      341 2023-08-01 14:43:04.000000 stc-geck-1.3.4/stc_geck.egg-info/SOURCES.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        1 2023-08-01 14:43:04.000000 stc-geck-1.3.4/stc_geck.egg-info/dependency_links.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       43 2023-08-01 14:43:04.000000 stc-geck-1.3.4/stc_geck.egg-info/entry_points.txt
+-rw-r--r--   0 pasha      (501) staff       (20)      162 2023-08-01 14:43:04.000000 stc-geck-1.3.4/stc_geck.egg-info/requires.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        9 2023-08-01 14:43:04.000000 stc-geck-1.3.4/stc_geck.egg-info/top_level.txt
```

### Comparing `stc-geck-1.3.3/pyproject.toml` & `stc-geck-1.3.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools<65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "stc-geck"
-version = "1.3.3"
+version = "1.3.4"
 authors = [{ name = "Interdimensional Walker" }]
 description = "GECK (Garden Of Eden Creation Kit) is a toolkit for setting up and maintaning STC"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3.8",
 ]
```

### Comparing `stc-geck-1.3.3/stc_geck/advices.py` & `stc-geck-1.3.4/stc_geck/advices.py`

 * *Files identical despite different names*

### Comparing `stc-geck-1.3.3/stc_geck/cli.py` & `stc-geck-1.3.4/stc_geck/cli.py`

 * *Files identical despite different names*

### Comparing `stc-geck-1.3.3/stc_geck/client.py` & `stc-geck-1.3.4/stc_geck/client.py`

 * *Files identical despite different names*

### Comparing `stc-geck-1.3.3/stc_geck/utils.py` & `stc-geck-1.3.4/stc_geck/utils.py`

 * *Files identical despite different names*

