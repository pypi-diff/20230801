# Comparing `tmp/paucode-0.3.tar.gz` & `tmp/paucode-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paucode-0.3.tar", last modified: Tue Aug  1 03:44:54 2023, max compression
+gzip compressed data, was "paucode-0.4.tar", last modified: Tue Aug  1 04:15:22 2023, max compression
```

## Comparing `paucode-0.3.tar` & `paucode-0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 choque    (1000) choque    (1000)        0 2023-08-01 03:44:54.974254 paucode-0.3/
--rw-rw-r--   0 choque    (1000) choque    (1000)     1065 2023-07-24 04:26:30.000000 paucode-0.3/LICENSE
--rw-rw-r--   0 choque    (1000) choque    (1000)      635 2023-08-01 03:44:54.974254 paucode-0.3/PKG-INFO
--rw-rw-r--   0 choque    (1000) choque    (1000)      313 2023-07-24 04:27:02.000000 paucode-0.3/README.md
-drwxrwxr-x   0 choque    (1000) choque    (1000)        0 2023-08-01 03:44:54.974254 paucode-0.3/paucode/
--rw-rw-r--   0 choque    (1000) choque    (1000)       46 2023-07-28 18:11:14.000000 paucode-0.3/paucode/__init__.py
--rw-rw-r--   0 choque    (1000) choque    (1000)        0 2023-07-24 04:26:30.000000 paucode-0.3/paucode/ds.py
--rw-rw-r--   0 choque    (1000) choque    (1000)      587 2023-07-28 17:51:54.000000 paucode-0.3/paucode/eco.py
--rw-rw-r--   0 choque    (1000) choque    (1000)     4505 2023-07-28 17:45:38.000000 paucode-0.3/paucode/ing.py
--rw-rw-r--   0 choque    (1000) choque    (1000)     1077 2023-07-24 04:26:30.000000 paucode-0.3/paucode/tsp.py
-drwxrwxr-x   0 choque    (1000) choque    (1000)        0 2023-08-01 03:44:54.974254 paucode-0.3/paucode.egg-info/
--rw-rw-r--   0 choque    (1000) choque    (1000)      635 2023-08-01 03:44:54.000000 paucode-0.3/paucode.egg-info/PKG-INFO
--rw-rw-r--   0 choque    (1000) choque    (1000)      259 2023-08-01 03:44:54.000000 paucode-0.3/paucode.egg-info/SOURCES.txt
--rw-rw-r--   0 choque    (1000) choque    (1000)        1 2023-08-01 03:44:54.000000 paucode-0.3/paucode.egg-info/dependency_links.txt
--rw-rw-r--   0 choque    (1000) choque    (1000)       17 2023-08-01 03:44:54.000000 paucode-0.3/paucode.egg-info/requires.txt
--rw-rw-r--   0 choque    (1000) choque    (1000)        8 2023-08-01 03:44:54.000000 paucode-0.3/paucode.egg-info/top_level.txt
--rw-rw-r--   0 choque    (1000) choque    (1000)       38 2023-08-01 03:44:54.974254 paucode-0.3/setup.cfg
--rw-rw-r--   0 choque    (1000) choque    (1000)      656 2023-08-01 03:43:22.000000 paucode-0.3/setup.py
+drwxrwxr-x   0 choque    (1000) choque    (1000)        0 2023-08-01 04:15:22.663305 paucode-0.4/
+-rw-rw-r--   0 choque    (1000) choque    (1000)     1065 2023-07-24 04:26:30.000000 paucode-0.4/LICENSE
+-rw-rw-r--   0 choque    (1000) choque    (1000)      575 2023-08-01 04:15:22.663305 paucode-0.4/PKG-INFO
+-rw-rw-r--   0 choque    (1000) choque    (1000)      253 2023-08-01 04:09:07.000000 paucode-0.4/README.md
+drwxrwxr-x   0 choque    (1000) choque    (1000)        0 2023-08-01 04:15:22.663305 paucode-0.4/paucode/
+-rw-rw-r--   0 choque    (1000) choque    (1000)       46 2023-07-28 18:11:14.000000 paucode-0.4/paucode/__init__.py
+-rw-rw-r--   0 choque    (1000) choque    (1000)        0 2023-07-24 04:26:30.000000 paucode-0.4/paucode/ds.py
+-rw-rw-r--   0 choque    (1000) choque    (1000)      587 2023-07-28 17:51:54.000000 paucode-0.4/paucode/eco.py
+-rw-rw-r--   0 choque    (1000) choque    (1000)     4505 2023-07-28 17:45:38.000000 paucode-0.4/paucode/ing.py
+-rw-rw-r--   0 choque    (1000) choque    (1000)     1077 2023-07-24 04:26:30.000000 paucode-0.4/paucode/tsp.py
+drwxrwxr-x   0 choque    (1000) choque    (1000)        0 2023-08-01 04:15:22.663305 paucode-0.4/paucode.egg-info/
+-rw-rw-r--   0 choque    (1000) choque    (1000)      575 2023-08-01 04:15:22.000000 paucode-0.4/paucode.egg-info/PKG-INFO
+-rw-rw-r--   0 choque    (1000) choque    (1000)      259 2023-08-01 04:15:22.000000 paucode-0.4/paucode.egg-info/SOURCES.txt
+-rw-rw-r--   0 choque    (1000) choque    (1000)        1 2023-08-01 04:15:22.000000 paucode-0.4/paucode.egg-info/dependency_links.txt
+-rw-rw-r--   0 choque    (1000) choque    (1000)       17 2023-08-01 04:15:22.000000 paucode-0.4/paucode.egg-info/requires.txt
+-rw-rw-r--   0 choque    (1000) choque    (1000)        8 2023-08-01 04:15:22.000000 paucode-0.4/paucode.egg-info/top_level.txt
+-rw-rw-r--   0 choque    (1000) choque    (1000)       38 2023-08-01 04:15:22.663305 paucode-0.4/setup.cfg
+-rw-rw-r--   0 choque    (1000) choque    (1000)      652 2023-08-01 04:13:55.000000 paucode-0.4/setup.py
```

### Comparing `paucode-0.3/LICENSE` & `paucode-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `paucode-0.3/paucode/eco.py` & `paucode-0.4/paucode/eco.py`

 * *Files identical despite different names*

### Comparing `paucode-0.3/paucode/ing.py` & `paucode-0.4/paucode/ing.py`

 * *Files identical despite different names*

### Comparing `paucode-0.3/paucode/tsp.py` & `paucode-0.4/paucode/tsp.py`

 * *Files identical despite different names*

### Comparing `paucode-0.3/setup.py` & `paucode-0.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 readme = open("./README.md", "r")
 
 setup(
     name="paucode",
-    packages=find_packages(),
-    version="0.03",
+    packages=["paucode"],
+    version="0.04",
     description="funciones de ayuda en trabajo como economista",
     long_description=readme.read(),
     long_description_content_type="text/markdown",
     author="Javier Choque Paucar",
     author_email="choquepaucarj.social@gmail.com",
     download_url="https://github.com/paucode1/paucode",
     keywords=["example"],
```

