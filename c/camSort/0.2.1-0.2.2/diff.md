# Comparing `tmp/camSort-0.2.1.tar.gz` & `tmp/camSort-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/camSort-0.2.1.tar", last modified: Tue Aug  1 08:34:20 2023, max compression
+gzip compressed data, was "dist/camSort-0.2.2.tar", last modified: Tue Aug  1 08:38:52 2023, max compression
```

## Comparing `camSort-0.2.1.tar` & `camSort-0.2.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-08-01 08:34:20.000000 camSort-0.2.1/
--rw-r--r--   0 macbook    (501) staff       (20)     2461 2023-08-01 08:34:20.000000 camSort-0.2.1/PKG-INFO
--rw-r--r--   0 macbook    (501) staff       (20)     1529 2023-08-01 07:52:20.000000 camSort-0.2.1/README.md
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-08-01 08:34:20.000000 camSort-0.2.1/camSort/
--rw-r--r--   0 macbook    (501) staff       (20)       14 2023-08-01 08:09:51.000000 camSort-0.2.1/camSort/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)   234571 2023-08-01 07:17:43.000000 camSort-0.2.1/camSort/camSort.c
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-08-01 08:34:20.000000 camSort-0.2.1/camSort.egg-info/
--rw-r--r--   0 macbook    (501) staff       (20)     2461 2023-08-01 08:34:20.000000 camSort-0.2.1/camSort.egg-info/PKG-INFO
--rw-r--r--   0 macbook    (501) staff       (20)      180 2023-08-01 08:34:20.000000 camSort-0.2.1/camSort.egg-info/SOURCES.txt
--rw-r--r--   0 macbook    (501) staff       (20)        1 2023-08-01 08:34:20.000000 camSort-0.2.1/camSort.egg-info/dependency_links.txt
--rw-r--r--   0 macbook    (501) staff       (20)        8 2023-08-01 08:34:20.000000 camSort-0.2.1/camSort.egg-info/top_level.txt
--rw-r--r--   0 macbook    (501) staff       (20)       38 2023-08-01 08:34:20.000000 camSort-0.2.1/setup.cfg
--rw-r--r--   0 macbook    (501) staff       (20)     1040 2023-08-01 08:34:11.000000 camSort-0.2.1/setup.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-08-01 08:38:52.000000 camSort-0.2.2/
+-rw-r--r--   0 macbook    (501) staff       (20)     2461 2023-08-01 08:38:52.000000 camSort-0.2.2/PKG-INFO
+-rw-r--r--   0 macbook    (501) staff       (20)     1529 2023-08-01 07:52:20.000000 camSort-0.2.2/README.md
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-08-01 08:38:52.000000 camSort-0.2.2/camSort/
+-rw-r--r--   0 macbook    (501) staff       (20)       14 2023-08-01 08:09:51.000000 camSort-0.2.2/camSort/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)   234571 2023-08-01 07:17:43.000000 camSort-0.2.2/camSort/camSort.c
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-08-01 08:38:52.000000 camSort-0.2.2/camSort.egg-info/
+-rw-r--r--   0 macbook    (501) staff       (20)     2461 2023-08-01 08:38:52.000000 camSort-0.2.2/camSort.egg-info/PKG-INFO
+-rw-r--r--   0 macbook    (501) staff       (20)      180 2023-08-01 08:38:52.000000 camSort-0.2.2/camSort.egg-info/SOURCES.txt
+-rw-r--r--   0 macbook    (501) staff       (20)        1 2023-08-01 08:38:52.000000 camSort-0.2.2/camSort.egg-info/dependency_links.txt
+-rw-r--r--   0 macbook    (501) staff       (20)        8 2023-08-01 08:38:52.000000 camSort-0.2.2/camSort.egg-info/top_level.txt
+-rw-r--r--   0 macbook    (501) staff       (20)       38 2023-08-01 08:38:52.000000 camSort-0.2.2/setup.cfg
+-rw-r--r--   0 macbook    (501) staff       (20)     1040 2023-08-01 08:38:18.000000 camSort-0.2.2/setup.py
```

### Comparing `camSort-0.2.1/PKG-INFO` & `camSort-0.2.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: camSort
-Version: 0.2.1
+Version: 0.2.2
 Summary: make sorted() fast for strings
 Home-page: https://github.com/cameronbae/camSort
 Author: cameronbae / cameron jay
 Author-email: <contact@camjay.io>
 License: UNKNOWN
 Description: 
         # camSort
```

### Comparing `camSort-0.2.1/README.md` & `camSort-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `camSort-0.2.1/camSort/camSort.c` & `camSort-0.2.2/camSort/camSort.c`

 * *Files identical despite different names*

### Comparing `camSort-0.2.1/camSort.egg-info/PKG-INFO` & `camSort-0.2.2/camSort.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: camSort
-Version: 0.2.1
+Version: 0.2.2
 Summary: make sorted() fast for strings
 Home-page: https://github.com/cameronbae/camSort
 Author: cameronbae / cameron jay
 Author-email: <contact@camjay.io>
 License: UNKNOWN
 Description: 
         # camSort
```

### Comparing `camSort-0.2.1/setup.py` & `camSort-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 LONG_DESCRIPTION = ''
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 setup(
     name="camSort",
-    version="0.2.1",
+    version="0.2.2",
     packages=["camSort"], 
     ext_modules = cythonize('camSort/camSort.pyx'),
     author="cameronbae / cameron jay",
     author_email="<contact@camjay.io>",
     url="https://github.com/cameronbae/camSort",
     description="make sorted() fast for strings",
     long_description_content_type="text/markdown",
```

