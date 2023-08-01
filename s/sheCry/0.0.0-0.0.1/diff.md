# Comparing `tmp/sheCry-0.0.0.tar.gz` & `tmp/sheCry-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sheCry-0.0.0.tar", last modified: Tue Aug  1 07:14:42 2023, max compression
+gzip compressed data, was "sheCry-0.0.1.tar", last modified: Tue Aug  1 07:40:31 2023, max compression
```

## Comparing `sheCry-0.0.0.tar` & `sheCry-0.0.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 07:14:42.939179 sheCry-0.0.0/
--rw-rw-rw-   0        0        0    35821 2023-07-31 18:14:15.000000 sheCry-0.0.0/LICENSE.md
--rw-rw-rw-   0        0        0     3147 2023-08-01 07:14:42.933601 sheCry-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2500 2023-08-01 07:14:25.000000 sheCry-0.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-08-01 07:14:42.939179 sheCry-0.0.0/setup.cfg
--rw-rw-rw-   0        0        0      909 2023-07-31 21:49:12.000000 sheCry-0.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-01 07:14:42.932600 sheCry-0.0.0/sheCry.egg-info/
--rw-rw-rw-   0        0        0     3147 2023-08-01 07:14:42.000000 sheCry-0.0.0/sheCry.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      149 2023-08-01 07:14:42.000000 sheCry-0.0.0/sheCry.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 07:14:42.000000 sheCry-0.0.0/sheCry.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 07:14:42.000000 sheCry-0.0.0/sheCry.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 07:40:31.950933 sheCry-0.0.1/
+-rw-rw-rw-   0        0        0    35821 2023-07-31 18:14:15.000000 sheCry-0.0.1/LICENSE.md
+-rw-rw-rw-   0        0        0     6349 2023-08-01 07:40:31.944900 sheCry-0.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5702 2023-08-01 07:39:52.000000 sheCry-0.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-01 07:40:31.950933 sheCry-0.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      909 2023-08-01 07:18:37.000000 sheCry-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 07:40:31.943395 sheCry-0.0.1/sheCry.egg-info/
+-rw-rw-rw-   0        0        0     6349 2023-08-01 07:40:31.000000 sheCry-0.0.1/sheCry.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      149 2023-08-01 07:40:31.000000 sheCry-0.0.1/sheCry.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 07:40:31.000000 sheCry-0.0.1/sheCry.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 07:40:31.000000 sheCry-0.0.1/sheCry.egg-info/top_level.txt
```

### Comparing `sheCry-0.0.0/LICENSE.md` & `sheCry-0.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sheCry-0.0.0/setup.py` & `sheCry-0.0.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name = "sheCry",
 
-    version = "0.0.0",
+    version = "0.0.1",
     
     author = "Tahsin Ahmed",
 
     description = "SHE Cryptography is architectured by Tahsin Ahmed.",
 
     long_description = open("README.md", encoding="utf-8").read(),
```

