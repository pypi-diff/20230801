# Comparing `tmp/sourmash_plugin_venn-0.3.tar.gz` & `tmp/sourmash_plugin_venn-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sourmash_plugin_venn-0.3.tar", last modified: Sun Jul 30 10:35:07 2023, max compression
+gzip compressed data, was "sourmash_plugin_venn-0.4.tar", last modified: Tue Aug  1 14:24:58 2023, max compression
```

## Comparing `sourmash_plugin_venn-0.3.tar` & `sourmash_plugin_venn-0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 t          (502) staff       (20)        0 2023-07-30 10:35:07.121432 sourmash_plugin_venn-0.3/
--rw-r--r--   0 t          (502) staff       (20)     1540 2023-07-24 20:57:14.000000 sourmash_plugin_venn-0.3/LICENSE
--rw-r--r--   0 t          (502) staff       (20)     1093 2023-07-30 10:35:07.121286 sourmash_plugin_venn-0.3/PKG-INFO
--rw-r--r--   0 t          (502) staff       (20)      896 2023-07-30 10:32:56.000000 sourmash_plugin_venn-0.3/README.md
--rw-r--r--   0 t          (502) staff       (20)      381 2023-07-30 10:32:14.000000 sourmash_plugin_venn-0.3/pyproject.toml
--rw-r--r--   0 t          (502) staff       (20)       38 2023-07-30 10:35:07.121723 sourmash_plugin_venn-0.3/setup.cfg
-drwxr-xr-x   0 t          (502) staff       (20)        0 2023-07-30 10:35:07.116501 sourmash_plugin_venn-0.3/src/
-drwxr-xr-x   0 t          (502) staff       (20)        0 2023-07-30 10:35:07.118886 sourmash_plugin_venn-0.3/src/sourmash_plugin_venn.egg-info/
--rw-r--r--   0 t          (502) staff       (20)     1093 2023-07-30 10:35:07.000000 sourmash_plugin_venn-0.3/src/sourmash_plugin_venn.egg-info/PKG-INFO
--rw-r--r--   0 t          (502) staff       (20)      380 2023-07-30 10:35:07.000000 sourmash_plugin_venn-0.3/src/sourmash_plugin_venn.egg-info/SOURCES.txt
--rw-r--r--   0 t          (502) staff       (20)        1 2023-07-30 10:35:07.000000 sourmash_plugin_venn-0.3/src/sourmash_plugin_venn.egg-info/dependency_links.txt
--rw-r--r--   0 t          (502) staff       (20)       68 2023-07-30 10:35:07.000000 sourmash_plugin_venn-0.3/src/sourmash_plugin_venn.egg-info/entry_points.txt
--rw-r--r--   0 t          (502) staff       (20)       46 2023-07-30 10:35:07.000000 sourmash_plugin_venn-0.3/src/sourmash_plugin_venn.egg-info/requires.txt
--rw-r--r--   0 t          (502) staff       (20)       21 2023-07-30 10:35:07.000000 sourmash_plugin_venn-0.3/src/sourmash_plugin_venn.egg-info/top_level.txt
--rw-r--r--   0 t          (502) staff       (20)     3189 2023-07-30 10:27:30.000000 sourmash_plugin_venn-0.3/src/sourmash_plugin_venn.py
-drwxr-xr-x   0 t          (502) staff       (20)        0 2023-07-30 10:35:07.120251 sourmash_plugin_venn-0.3/tests/
--rw-r--r--   0 t          (502) staff       (20)      446 2023-07-24 20:57:14.000000 sourmash_plugin_venn-0.3/tests/test_sourmash_plugin.py
+drwxr-xr-x   0 t          (502) staff       (20)        0 2023-08-01 14:24:58.519613 sourmash_plugin_venn-0.4/
+-rw-r--r--   0 t          (502) staff       (20)     1540 2023-07-24 20:57:14.000000 sourmash_plugin_venn-0.4/LICENSE
+-rw-r--r--   0 t          (502) staff       (20)     1224 2023-08-01 14:24:58.519462 sourmash_plugin_venn-0.4/PKG-INFO
+-rw-r--r--   0 t          (502) staff       (20)     1027 2023-08-01 14:23:47.000000 sourmash_plugin_venn-0.4/README.md
+-rw-r--r--   0 t          (502) staff       (20)      376 2023-08-01 14:23:52.000000 sourmash_plugin_venn-0.4/pyproject.toml
+-rw-r--r--   0 t          (502) staff       (20)       38 2023-08-01 14:24:58.519671 sourmash_plugin_venn-0.4/setup.cfg
+drwxr-xr-x   0 t          (502) staff       (20)        0 2023-08-01 14:24:58.518092 sourmash_plugin_venn-0.4/src/
+drwxr-xr-x   0 t          (502) staff       (20)        0 2023-08-01 14:24:58.518975 sourmash_plugin_venn-0.4/src/sourmash_plugin_venn.egg-info/
+-rw-r--r--   0 t          (502) staff       (20)     1224 2023-08-01 14:24:58.000000 sourmash_plugin_venn-0.4/src/sourmash_plugin_venn.egg-info/PKG-INFO
+-rw-r--r--   0 t          (502) staff       (20)      378 2023-08-01 14:24:58.000000 sourmash_plugin_venn-0.4/src/sourmash_plugin_venn.egg-info/SOURCES.txt
+-rw-r--r--   0 t          (502) staff       (20)        1 2023-08-01 14:24:58.000000 sourmash_plugin_venn-0.4/src/sourmash_plugin_venn.egg-info/dependency_links.txt
+-rw-r--r--   0 t          (502) staff       (20)       63 2023-08-01 14:24:58.000000 sourmash_plugin_venn-0.4/src/sourmash_plugin_venn.egg-info/entry_points.txt
+-rw-r--r--   0 t          (502) staff       (20)       46 2023-08-01 14:24:58.000000 sourmash_plugin_venn-0.4/src/sourmash_plugin_venn.egg-info/requires.txt
+-rw-r--r--   0 t          (502) staff       (20)       21 2023-08-01 14:24:58.000000 sourmash_plugin_venn-0.4/src/sourmash_plugin_venn.egg-info/top_level.txt
+-rw-r--r--   0 t          (502) staff       (20)     3748 2023-08-01 14:23:47.000000 sourmash_plugin_venn-0.4/src/sourmash_plugin_venn.py
+drwxr-xr-x   0 t          (502) staff       (20)        0 2023-08-01 14:24:58.519123 sourmash_plugin_venn-0.4/tests/
+-rw-r--r--   0 t          (502) staff       (20)     1389 2023-08-01 14:23:47.000000 sourmash_plugin_venn-0.4/tests/test_sourmash_venn.py
```

### Comparing `sourmash_plugin_venn-0.3/LICENSE` & `sourmash_plugin_venn-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_venn-0.3/PKG-INFO` & `sourmash_plugin_venn-0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: sourmash_plugin_venn
-Version: 0.3
+Version: 0.4
 Summary: sourmash plugin to build venn diagrams.
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # sourmash_plugin_venn: generate a simple Venn diagram for two sourmash sketches
 
 Generate Venn diagrams showing overlaps between two
 [sourmash sketches](https://sourmash.readthedocs.io/) of DNA or
 protein sequences:
 
 ![simple Venn diagram](doc/simple.png)
 
-## Execution
+## Examples
 
 ```
 sourmash scripts venn examples/a.sig.gz examples/b.sig.gz -o a-b.png
 
 sourmash scripts venn examples/a.sig.gz examples/b.sig.gz -o a-b.png --name1 A --name2 B
 
 sourmash scripts venn examples/a.sig.gz examples/b.sig.gz examples/c.sig.gz -o a-b-c.png 
@@ -28,15 +28,26 @@
 
 ## Installation
 
 ```
 pip install sourmash_plugin_venn
 ```
 
-## Generating a release
+## Dev docs
+
+`venn` is developed at https://github.com/sourmash-bio/sourmash_plugin_venn.
+
+### Testing
+
+Run:
+```
+pytest tests
+```
+
+### Generating a release
 
 Bump version number in `pyproject.toml` and push.
 
 Make a new release on github.
 
 Then pull, and:
```

### Comparing `sourmash_plugin_venn-0.3/README.md` & `sourmash_plugin_venn-0.4/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 Generate Venn diagrams showing overlaps between two
 [sourmash sketches](https://sourmash.readthedocs.io/) of DNA or
 protein sequences:
 
 ![simple Venn diagram](doc/simple.png)
 
-## Execution
+## Examples
 
 ```
 sourmash scripts venn examples/a.sig.gz examples/b.sig.gz -o a-b.png
 
 sourmash scripts venn examples/a.sig.gz examples/b.sig.gz -o a-b.png --name1 A --name2 B
 
 sourmash scripts venn examples/a.sig.gz examples/b.sig.gz examples/c.sig.gz -o a-b-c.png 
@@ -20,15 +20,26 @@
 
 ## Installation
 
 ```
 pip install sourmash_plugin_venn
 ```
 
-## Generating a release
+## Dev docs
+
+`venn` is developed at https://github.com/sourmash-bio/sourmash_plugin_venn.
+
+### Testing
+
+Run:
+```
+pytest tests
+```
+
+### Generating a release
 
 Bump version number in `pyproject.toml` and push.
 
 Make a new release on github.
 
 Then pull, and:
```

### Comparing `sourmash_plugin_venn-0.3/src/sourmash_plugin_venn.egg-info/PKG-INFO` & `sourmash_plugin_venn-0.4/src/sourmash_plugin_venn.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: sourmash-plugin-venn
-Version: 0.3
+Version: 0.4
 Summary: sourmash plugin to build venn diagrams.
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # sourmash_plugin_venn: generate a simple Venn diagram for two sourmash sketches
 
 Generate Venn diagrams showing overlaps between two
 [sourmash sketches](https://sourmash.readthedocs.io/) of DNA or
 protein sequences:
 
 ![simple Venn diagram](doc/simple.png)
 
-## Execution
+## Examples
 
 ```
 sourmash scripts venn examples/a.sig.gz examples/b.sig.gz -o a-b.png
 
 sourmash scripts venn examples/a.sig.gz examples/b.sig.gz -o a-b.png --name1 A --name2 B
 
 sourmash scripts venn examples/a.sig.gz examples/b.sig.gz examples/c.sig.gz -o a-b-c.png 
@@ -28,15 +28,26 @@
 
 ## Installation
 
 ```
 pip install sourmash_plugin_venn
 ```
 
-## Generating a release
+## Dev docs
+
+`venn` is developed at https://github.com/sourmash-bio/sourmash_plugin_venn.
+
+### Testing
+
+Run:
+```
+pytest tests
+```
+
+### Generating a release
 
 Bump version number in `pyproject.toml` and push.
 
 Make a new release on github.
 
 Then pull, and:
```

