# Comparing `tmp/sourmash_plugin_commonhash-0.2.1.tar.gz` & `tmp/sourmash_plugin_commonhash-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sourmash_plugin_commonhash-0.2.1.tar", last modified: Mon Jul 31 13:43:54 2023, max compression
+gzip compressed data, was "sourmash_plugin_commonhash-0.3.tar", last modified: Tue Aug  1 14:21:59 2023, max compression
```

## Comparing `sourmash_plugin_commonhash-0.2.1.tar` & `sourmash_plugin_commonhash-0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 t          (502) staff       (20)        0 2023-07-31 13:43:54.455639 sourmash_plugin_commonhash-0.2.1/
--rw-r--r--   0 t          (502) staff       (20)     1540 2023-07-30 11:12:12.000000 sourmash_plugin_commonhash-0.2.1/LICENSE
--rw-r--r--   0 t          (502) staff       (20)     1693 2023-07-31 13:43:54.455493 sourmash_plugin_commonhash-0.2.1/PKG-INFO
--rw-r--r--   0 t          (502) staff       (20)     1459 2023-07-31 13:42:35.000000 sourmash_plugin_commonhash-0.2.1/README.md
--rw-r--r--   0 t          (502) staff       (20)      398 2023-07-31 13:42:53.000000 sourmash_plugin_commonhash-0.2.1/pyproject.toml
--rw-r--r--   0 t          (502) staff       (20)       38 2023-07-31 13:43:54.455684 sourmash_plugin_commonhash-0.2.1/setup.cfg
-drwxr-xr-x   0 t          (502) staff       (20)        0 2023-07-31 13:43:54.454034 sourmash_plugin_commonhash-0.2.1/src/
-drwxr-xr-x   0 t          (502) staff       (20)        0 2023-07-31 13:43:54.455048 sourmash_plugin_commonhash-0.2.1/src/sourmash_plugin_commonhash.egg-info/
--rw-r--r--   0 t          (502) staff       (20)     1693 2023-07-31 13:43:54.000000 sourmash_plugin_commonhash-0.2.1/src/sourmash_plugin_commonhash.egg-info/PKG-INFO
--rw-r--r--   0 t          (502) staff       (20)      422 2023-07-31 13:43:54.000000 sourmash_plugin_commonhash-0.2.1/src/sourmash_plugin_commonhash.egg-info/SOURCES.txt
--rw-r--r--   0 t          (502) staff       (20)        1 2023-07-31 13:43:54.000000 sourmash_plugin_commonhash-0.2.1/src/sourmash_plugin_commonhash.egg-info/dependency_links.txt
--rw-r--r--   0 t          (502) staff       (20)       81 2023-07-31 13:43:54.000000 sourmash_plugin_commonhash-0.2.1/src/sourmash_plugin_commonhash.egg-info/entry_points.txt
--rw-r--r--   0 t          (502) staff       (20)       19 2023-07-31 13:43:54.000000 sourmash_plugin_commonhash-0.2.1/src/sourmash_plugin_commonhash.egg-info/requires.txt
--rw-r--r--   0 t          (502) staff       (20)       27 2023-07-31 13:43:54.000000 sourmash_plugin_commonhash-0.2.1/src/sourmash_plugin_commonhash.egg-info/top_level.txt
--rw-r--r--   0 t          (502) staff       (20)     3705 2023-07-31 12:31:46.000000 sourmash_plugin_commonhash-0.2.1/src/sourmash_plugin_commonhash.py
-drwxr-xr-x   0 t          (502) staff       (20)        0 2023-07-31 13:43:54.455168 sourmash_plugin_commonhash-0.2.1/tests/
--rw-r--r--   0 t          (502) staff       (20)      446 2023-07-30 11:12:12.000000 sourmash_plugin_commonhash-0.2.1/tests/test_sourmash_plugin.py
+drwxr-xr-x   0 t          (502) staff       (20)        0 2023-08-01 14:21:59.946273 sourmash_plugin_commonhash-0.3/
+-rw-r--r--   0 t          (502) staff       (20)     1540 2023-07-30 11:12:12.000000 sourmash_plugin_commonhash-0.3/LICENSE
+-rw-r--r--   0 t          (502) staff       (20)     1692 2023-08-01 14:21:59.946112 sourmash_plugin_commonhash-0.3/PKG-INFO
+-rw-r--r--   0 t          (502) staff       (20)     1460 2023-08-01 14:20:31.000000 sourmash_plugin_commonhash-0.3/README.md
+-rw-r--r--   0 t          (502) staff       (20)      396 2023-08-01 14:20:52.000000 sourmash_plugin_commonhash-0.3/pyproject.toml
+-rw-r--r--   0 t          (502) staff       (20)       38 2023-08-01 14:21:59.946318 sourmash_plugin_commonhash-0.3/setup.cfg
+drwxr-xr-x   0 t          (502) staff       (20)        0 2023-08-01 14:21:59.944473 sourmash_plugin_commonhash-0.3/src/
+drwxr-xr-x   0 t          (502) staff       (20)        0 2023-08-01 14:21:59.945502 sourmash_plugin_commonhash-0.3/src/sourmash_plugin_commonhash.egg-info/
+-rw-r--r--   0 t          (502) staff       (20)     1692 2023-08-01 14:21:59.000000 sourmash_plugin_commonhash-0.3/src/sourmash_plugin_commonhash.egg-info/PKG-INFO
+-rw-r--r--   0 t          (502) staff       (20)      426 2023-08-01 14:21:59.000000 sourmash_plugin_commonhash-0.3/src/sourmash_plugin_commonhash.egg-info/SOURCES.txt
+-rw-r--r--   0 t          (502) staff       (20)        1 2023-08-01 14:21:59.000000 sourmash_plugin_commonhash-0.3/src/sourmash_plugin_commonhash.egg-info/dependency_links.txt
+-rw-r--r--   0 t          (502) staff       (20)       81 2023-08-01 14:21:59.000000 sourmash_plugin_commonhash-0.3/src/sourmash_plugin_commonhash.egg-info/entry_points.txt
+-rw-r--r--   0 t          (502) staff       (20)       19 2023-08-01 14:21:59.000000 sourmash_plugin_commonhash-0.3/src/sourmash_plugin_commonhash.egg-info/requires.txt
+-rw-r--r--   0 t          (502) staff       (20)       27 2023-08-01 14:21:59.000000 sourmash_plugin_commonhash-0.3/src/sourmash_plugin_commonhash.egg-info/top_level.txt
+-rw-r--r--   0 t          (502) staff       (20)     3706 2023-08-01 14:20:31.000000 sourmash_plugin_commonhash-0.3/src/sourmash_plugin_commonhash.py
+drwxr-xr-x   0 t          (502) staff       (20)        0 2023-08-01 14:21:59.945627 sourmash_plugin_commonhash-0.3/tests/
+-rw-r--r--   0 t          (502) staff       (20)     1288 2023-08-01 14:20:04.000000 sourmash_plugin_commonhash-0.3/tests/test_sourmash_commonhash.py
```

### Comparing `sourmash_plugin_commonhash-0.2.1/LICENSE` & `sourmash_plugin_commonhash-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_commonhash-0.2.1/PKG-INFO` & `sourmash_plugin_commonhash-0.3/src/sourmash_plugin_commonhash.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: sourmash_plugin_commonhash
-Version: 0.2.1
+Name: sourmash-plugin-commonhash
+Version: 0.3
 Summary: sourmash plugin to calculate common hashes across multiple sketches.
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # sourmash_plugin_commonhash
 
@@ -33,15 +33,15 @@
 commonhash will output one filtered sketch for _each_ input sketch.
 You can then use the various `sourmash sig` commands to union these
 sketches, extract individual ones, etc.
 
 ### Example
 
 ```
-sourmash scripts commonhash example/*.sig.gz -o commonhash.zip
+sourmash scripts commonhash examples/*.sig.gz -o commonhash.zip
 ```
 
 should yield:
 
 ```
 ...
```

### Comparing `sourmash_plugin_commonhash-0.2.1/README.md` & `sourmash_plugin_commonhash-0.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 commonhash will output one filtered sketch for _each_ input sketch.
 You can then use the various `sourmash sig` commands to union these
 sketches, extract individual ones, etc.
 
 ### Example
 
 ```
-sourmash scripts commonhash example/*.sig.gz -o commonhash.zip
+sourmash scripts commonhash examples/*.sig.gz -o commonhash.zip
 ```
 
 should yield:
 
 ```
 ...
```

### Comparing `sourmash_plugin_commonhash-0.2.1/src/sourmash_plugin_commonhash.egg-info/PKG-INFO` & `sourmash_plugin_commonhash-0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: sourmash-plugin-commonhash
-Version: 0.2.1
+Name: sourmash_plugin_commonhash
+Version: 0.3
 Summary: sourmash plugin to calculate common hashes across multiple sketches.
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # sourmash_plugin_commonhash
 
@@ -33,15 +33,15 @@
 commonhash will output one filtered sketch for _each_ input sketch.
 You can then use the various `sourmash sig` commands to union these
 sketches, extract individual ones, etc.
 
 ### Example
 
 ```
-sourmash scripts commonhash example/*.sig.gz -o commonhash.zip
+sourmash scripts commonhash examples/*.sig.gz -o commonhash.zip
 ```
 
 should yield:
 
 ```
 ...
```

### Comparing `sourmash_plugin_commonhash-0.2.1/src/sourmash_plugin_commonhash.py` & `sourmash_plugin_commonhash-0.3/src/sourmash_plugin_commonhash.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""
+"""\
 filter hashes by min occurrence across sketches
 
 Reduce 'noise' in Jaccard comparisons of sequencing data by removing
 hashes that are present in only a few sketches.
 
 'commonhash' supports the full range of sourmash sketch output formats [1].
```

