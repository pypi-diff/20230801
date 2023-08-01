# Comparing `tmp/earthml-0.1.tar.gz` & `tmp/earthml-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "earthml-0.1.tar", last modified: Tue Aug  1 18:57:48 2023, max compression
+gzip compressed data, was "earthml-0.2.tar", last modified: Tue Aug  1 19:07:53 2023, max compression
```

## Comparing `earthml-0.1.tar` & `earthml-0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 akhilchhibber   (501) staff       (20)        0 2023-08-01 18:57:48.867510 earthml-0.1/
--rw-r--r--   0 akhilchhibber   (501) staff       (20)     1070 2023-08-01 18:41:39.000000 earthml-0.1/LICENSE
--rw-r--r--   0 akhilchhibber   (501) staff       (20)      598 2023-08-01 18:57:48.867390 earthml-0.1/PKG-INFO
--rw-r--r--   0 akhilchhibber   (501) staff       (20)     1496 2023-08-01 18:50:13.000000 earthml-0.1/README.md
-drwxr-xr-x   0 akhilchhibber   (501) staff       (20)        0 2023-08-01 18:57:48.866563 earthml-0.1/earthml/
--rw-r--r--   0 akhilchhibber   (501) staff       (20)       33 2023-08-01 18:30:59.000000 earthml-0.1/earthml/__init__.py
--rw-r--r--   0 akhilchhibber   (501) staff       (20)    13831 2023-08-01 18:57:08.000000 earthml-0.1/earthml/geodata_to_geohash.py
-drwxr-xr-x   0 akhilchhibber   (501) staff       (20)        0 2023-08-01 18:57:48.867222 earthml-0.1/earthml.egg-info/
--rw-r--r--   0 akhilchhibber   (501) staff       (20)      598 2023-08-01 18:57:48.000000 earthml-0.1/earthml.egg-info/PKG-INFO
--rw-r--r--   0 akhilchhibber   (501) staff       (20)      230 2023-08-01 18:57:48.000000 earthml-0.1/earthml.egg-info/SOURCES.txt
--rw-r--r--   0 akhilchhibber   (501) staff       (20)        1 2023-08-01 18:57:48.000000 earthml-0.1/earthml.egg-info/dependency_links.txt
--rw-r--r--   0 akhilchhibber   (501) staff       (20)       38 2023-08-01 18:57:48.000000 earthml-0.1/earthml.egg-info/requires.txt
--rw-r--r--   0 akhilchhibber   (501) staff       (20)        8 2023-08-01 18:57:48.000000 earthml-0.1/earthml.egg-info/top_level.txt
--rw-r--r--   0 akhilchhibber   (501) staff       (20)       38 2023-08-01 18:57:48.867549 earthml-0.1/setup.cfg
--rw-r--r--   0 akhilchhibber   (501) staff       (20)      812 2023-08-01 18:45:01.000000 earthml-0.1/setup.py
+drwxr-xr-x   0 akhilchhibber   (501) staff       (20)        0 2023-08-01 19:07:53.237385 earthml-0.2/
+-rw-r--r--   0 akhilchhibber   (501) staff       (20)     1070 2023-08-01 18:41:39.000000 earthml-0.2/LICENSE
+-rw-r--r--   0 akhilchhibber   (501) staff       (20)     2135 2023-08-01 19:07:53.237259 earthml-0.2/PKG-INFO
+-rw-r--r--   0 akhilchhibber   (501) staff       (20)     1496 2023-08-01 18:50:13.000000 earthml-0.2/README.md
+drwxr-xr-x   0 akhilchhibber   (501) staff       (20)        0 2023-08-01 19:07:53.236411 earthml-0.2/earthml/
+-rw-r--r--   0 akhilchhibber   (501) staff       (20)       33 2023-08-01 18:30:59.000000 earthml-0.2/earthml/__init__.py
+-rw-r--r--   0 akhilchhibber   (501) staff       (20)    13831 2023-08-01 18:57:08.000000 earthml-0.2/earthml/geodata_to_geohash.py
+drwxr-xr-x   0 akhilchhibber   (501) staff       (20)        0 2023-08-01 19:07:53.237084 earthml-0.2/earthml.egg-info/
+-rw-r--r--   0 akhilchhibber   (501) staff       (20)     2135 2023-08-01 19:07:53.000000 earthml-0.2/earthml.egg-info/PKG-INFO
+-rw-r--r--   0 akhilchhibber   (501) staff       (20)      230 2023-08-01 19:07:53.000000 earthml-0.2/earthml.egg-info/SOURCES.txt
+-rw-r--r--   0 akhilchhibber   (501) staff       (20)        1 2023-08-01 19:07:53.000000 earthml-0.2/earthml.egg-info/dependency_links.txt
+-rw-r--r--   0 akhilchhibber   (501) staff       (20)       38 2023-08-01 19:07:53.000000 earthml-0.2/earthml.egg-info/requires.txt
+-rw-r--r--   0 akhilchhibber   (501) staff       (20)        8 2023-08-01 19:07:53.000000 earthml-0.2/earthml.egg-info/top_level.txt
+-rw-r--r--   0 akhilchhibber   (501) staff       (20)       38 2023-08-01 19:07:53.237424 earthml-0.2/setup.cfg
+-rw-r--r--   0 akhilchhibber   (501) staff       (20)     1030 2023-08-01 19:07:38.000000 earthml-0.2/setup.py
```

### Comparing `earthml-0.1/LICENSE` & `earthml-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `earthml-0.1/README.md` & `earthml-0.2/README.md`

 * *Files identical despite different names*

### Comparing `earthml-0.1/earthml/geodata_to_geohash.py` & `earthml-0.2/earthml/geodata_to_geohash.py`

 * *Files identical despite different names*

