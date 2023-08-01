# Comparing `tmp/paucode-0.2.tar.gz` & `tmp/paucode-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paucode-0.2.tar", last modified: Fri Jul 28 18:16:40 2023, max compression
+gzip compressed data, was "paucode-0.3.tar", last modified: Tue Aug  1 03:44:54 2023, max compression
```

## Comparing `paucode-0.2.tar` & `paucode-0.3.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxr-x   0 choque    (1000) choque    (1000)        0 2023-07-28 18:16:40.685483 paucode-0.2/
--rw-rw-r--   0 choque    (1000) choque    (1000)     1065 2023-07-24 04:26:30.000000 paucode-0.2/LICENSE
--rw-rw-r--   0 choque    (1000) choque    (1000)      635 2023-07-28 18:16:40.685483 paucode-0.2/PKG-INFO
--rw-rw-r--   0 choque    (1000) choque    (1000)      313 2023-07-24 04:27:02.000000 paucode-0.2/README.md
-drwxrwxr-x   0 choque    (1000) choque    (1000)        0 2023-07-28 18:16:40.685483 paucode-0.2/paucode/
--rw-rw-r--   0 choque    (1000) choque    (1000)       46 2023-07-28 18:11:14.000000 paucode-0.2/paucode/__init__.py
--rw-rw-r--   0 choque    (1000) choque    (1000)        0 2023-07-24 04:26:30.000000 paucode-0.2/paucode/ds.py
--rw-rw-r--   0 choque    (1000) choque    (1000)      587 2023-07-28 17:51:54.000000 paucode-0.2/paucode/eco.py
--rw-rw-r--   0 choque    (1000) choque    (1000)     4505 2023-07-28 17:45:38.000000 paucode-0.2/paucode/ing.py
--rw-rw-r--   0 choque    (1000) choque    (1000)     1077 2023-07-24 04:26:30.000000 paucode-0.2/paucode/tsp.py
-drwxrwxr-x   0 choque    (1000) choque    (1000)        0 2023-07-28 18:16:40.685483 paucode-0.2/paucode.egg-info/
--rw-rw-r--   0 choque    (1000) choque    (1000)      635 2023-07-28 18:16:40.000000 paucode-0.2/paucode.egg-info/PKG-INFO
--rw-rw-r--   0 choque    (1000) choque    (1000)      229 2023-07-28 18:16:40.000000 paucode-0.2/paucode.egg-info/SOURCES.txt
--rw-rw-r--   0 choque    (1000) choque    (1000)        1 2023-07-28 18:16:40.000000 paucode-0.2/paucode.egg-info/dependency_links.txt
--rw-rw-r--   0 choque    (1000) choque    (1000)        8 2023-07-28 18:16:40.000000 paucode-0.2/paucode.egg-info/top_level.txt
--rw-rw-r--   0 choque    (1000) choque    (1000)       38 2023-07-28 18:16:40.685483 paucode-0.2/setup.cfg
--rw-rw-r--   0 choque    (1000) choque    (1000)      528 2023-07-28 18:11:01.000000 paucode-0.2/setup.py
+drwxrwxr-x   0 choque    (1000) choque    (1000)        0 2023-08-01 03:44:54.974254 paucode-0.3/
+-rw-rw-r--   0 choque    (1000) choque    (1000)     1065 2023-07-24 04:26:30.000000 paucode-0.3/LICENSE
+-rw-rw-r--   0 choque    (1000) choque    (1000)      635 2023-08-01 03:44:54.974254 paucode-0.3/PKG-INFO
+-rw-rw-r--   0 choque    (1000) choque    (1000)      313 2023-07-24 04:27:02.000000 paucode-0.3/README.md
+drwxrwxr-x   0 choque    (1000) choque    (1000)        0 2023-08-01 03:44:54.974254 paucode-0.3/paucode/
+-rw-rw-r--   0 choque    (1000) choque    (1000)       46 2023-07-28 18:11:14.000000 paucode-0.3/paucode/__init__.py
+-rw-rw-r--   0 choque    (1000) choque    (1000)        0 2023-07-24 04:26:30.000000 paucode-0.3/paucode/ds.py
+-rw-rw-r--   0 choque    (1000) choque    (1000)      587 2023-07-28 17:51:54.000000 paucode-0.3/paucode/eco.py
+-rw-rw-r--   0 choque    (1000) choque    (1000)     4505 2023-07-28 17:45:38.000000 paucode-0.3/paucode/ing.py
+-rw-rw-r--   0 choque    (1000) choque    (1000)     1077 2023-07-24 04:26:30.000000 paucode-0.3/paucode/tsp.py
+drwxrwxr-x   0 choque    (1000) choque    (1000)        0 2023-08-01 03:44:54.974254 paucode-0.3/paucode.egg-info/
+-rw-rw-r--   0 choque    (1000) choque    (1000)      635 2023-08-01 03:44:54.000000 paucode-0.3/paucode.egg-info/PKG-INFO
+-rw-rw-r--   0 choque    (1000) choque    (1000)      259 2023-08-01 03:44:54.000000 paucode-0.3/paucode.egg-info/SOURCES.txt
+-rw-rw-r--   0 choque    (1000) choque    (1000)        1 2023-08-01 03:44:54.000000 paucode-0.3/paucode.egg-info/dependency_links.txt
+-rw-rw-r--   0 choque    (1000) choque    (1000)       17 2023-08-01 03:44:54.000000 paucode-0.3/paucode.egg-info/requires.txt
+-rw-rw-r--   0 choque    (1000) choque    (1000)        8 2023-08-01 03:44:54.000000 paucode-0.3/paucode.egg-info/top_level.txt
+-rw-rw-r--   0 choque    (1000) choque    (1000)       38 2023-08-01 03:44:54.974254 paucode-0.3/setup.cfg
+-rw-rw-r--   0 choque    (1000) choque    (1000)      656 2023-08-01 03:43:22.000000 paucode-0.3/setup.py
```

### Comparing `paucode-0.2/LICENSE` & `paucode-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `paucode-0.2/PKG-INFO` & `paucode-0.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paucode
-Version: 0.2
+Version: 0.3
 Summary: funciones de ayuda en trabajo como economista
 Download-URL: https://github.com/paucode1/paucode
 Author: Javier Choque Paucar
 Author-email: choquepaucarj.social@gmail.com
 License: MIT
 Keywords: example
 Description-Content-Type: text/markdown
```

### Comparing `paucode-0.2/paucode/eco.py` & `paucode-0.3/paucode/eco.py`

 * *Files identical despite different names*

### Comparing `paucode-0.2/paucode/ing.py` & `paucode-0.3/paucode/ing.py`

 * *Files identical despite different names*

### Comparing `paucode-0.2/paucode/tsp.py` & `paucode-0.3/paucode/tsp.py`

 * *Files identical despite different names*

### Comparing `paucode-0.2/paucode.egg-info/PKG-INFO` & `paucode-0.3/paucode.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paucode
-Version: 0.2
+Version: 0.3
 Summary: funciones de ayuda en trabajo como economista
 Download-URL: https://github.com/paucode1/paucode
 Author: Javier Choque Paucar
 Author-email: choquepaucarj.social@gmail.com
 License: MIT
 Keywords: example
 Description-Content-Type: text/markdown
```

