# Comparing `tmp/Pygeun-0.0.3.tar.gz` & `tmp/Pygeun-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pygeun-0.0.3.tar", last modified: Tue Aug  1 07:37:12 2023, max compression
+gzip compressed data, was "Pygeun-0.0.4.tar", last modified: Tue Aug  1 07:38:48 2023, max compression
```

## Comparing `Pygeun-0.0.3.tar` & `Pygeun-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-01 07:37:12.819695 Pygeun-0.0.3/
--rw-r--r--   0 daegeun    (501) staff       (20)      503 2023-08-01 07:37:12.819472 Pygeun-0.0.3/PKG-INFO
-drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-01 07:37:12.817915 Pygeun-0.0.3/Pygeun/
--rw-r--r--   0 daegeun    (501) staff       (20)      430 2023-08-01 07:36:23.000000 Pygeun-0.0.3/Pygeun/__init__.py
--rw-r--r--   0 daegeun    (501) staff       (20)      996 2023-06-01 09:57:12.000000 Pygeun-0.0.3/Pygeun/gradient_descent.py
--rw-r--r--   0 daegeun    (501) staff       (20)     2170 2023-05-10 09:39:09.000000 Pygeun-0.0.3/Pygeun/levenberg_marquardt.py
--rw-r--r--   0 daegeun    (501) staff       (20)     1140 2023-05-28 06:20:21.000000 Pygeun-0.0.3/Pygeun/newton_raphson.py
-drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-01 07:37:12.819170 Pygeun-0.0.3/Pygeun.egg-info/
--rw-r--r--   0 daegeun    (501) staff       (20)      503 2023-08-01 07:37:12.000000 Pygeun-0.0.3/Pygeun.egg-info/PKG-INFO
--rw-r--r--   0 daegeun    (501) staff       (20)      268 2023-08-01 07:37:12.000000 Pygeun-0.0.3/Pygeun.egg-info/SOURCES.txt
--rw-r--r--   0 daegeun    (501) staff       (20)        1 2023-08-01 07:37:12.000000 Pygeun-0.0.3/Pygeun.egg-info/dependency_links.txt
--rw-r--r--   0 daegeun    (501) staff       (20)        1 2023-08-01 07:37:12.000000 Pygeun-0.0.3/Pygeun.egg-info/not-zip-safe
--rw-r--r--   0 daegeun    (501) staff       (20)        7 2023-08-01 07:37:12.000000 Pygeun-0.0.3/Pygeun.egg-info/top_level.txt
--rw-r--r--   0 daegeun    (501) staff       (20)       49 2023-08-01 07:16:34.000000 Pygeun-0.0.3/README.md
--rw-r--r--   0 daegeun    (501) staff       (20)       38 2023-08-01 07:37:12.819787 Pygeun-0.0.3/setup.cfg
--rw-r--r--   0 daegeun    (501) staff       (20)      674 2023-08-01 07:36:25.000000 Pygeun-0.0.3/setup.py
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-01 07:38:48.031027 Pygeun-0.0.4/
+-rw-r--r--   0 daegeun    (501) staff       (20)      503 2023-08-01 07:38:48.030810 Pygeun-0.0.4/PKG-INFO
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-01 07:38:48.029344 Pygeun-0.0.4/Pygeun/
+-rw-r--r--   0 daegeun    (501) staff       (20)      430 2023-08-01 07:38:39.000000 Pygeun-0.0.4/Pygeun/__init__.py
+-rw-r--r--   0 daegeun    (501) staff       (20)      996 2023-06-01 09:57:12.000000 Pygeun-0.0.4/Pygeun/gradient_descent.py
+-rw-r--r--   0 daegeun    (501) staff       (20)     2170 2023-05-10 09:39:09.000000 Pygeun-0.0.4/Pygeun/levenberg_marquardt.py
+-rw-r--r--   0 daegeun    (501) staff       (20)     1140 2023-05-28 06:20:21.000000 Pygeun-0.0.4/Pygeun/newton_raphson.py
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-01 07:38:48.030463 Pygeun-0.0.4/Pygeun.egg-info/
+-rw-r--r--   0 daegeun    (501) staff       (20)      503 2023-08-01 07:38:47.000000 Pygeun-0.0.4/Pygeun.egg-info/PKG-INFO
+-rw-r--r--   0 daegeun    (501) staff       (20)      268 2023-08-01 07:38:47.000000 Pygeun-0.0.4/Pygeun.egg-info/SOURCES.txt
+-rw-r--r--   0 daegeun    (501) staff       (20)        1 2023-08-01 07:38:47.000000 Pygeun-0.0.4/Pygeun.egg-info/dependency_links.txt
+-rw-r--r--   0 daegeun    (501) staff       (20)        1 2023-08-01 07:38:47.000000 Pygeun-0.0.4/Pygeun.egg-info/not-zip-safe
+-rw-r--r--   0 daegeun    (501) staff       (20)        7 2023-08-01 07:38:47.000000 Pygeun-0.0.4/Pygeun.egg-info/top_level.txt
+-rw-r--r--   0 daegeun    (501) staff       (20)       49 2023-08-01 07:16:34.000000 Pygeun-0.0.4/README.md
+-rw-r--r--   0 daegeun    (501) staff       (20)       38 2023-08-01 07:38:48.031106 Pygeun-0.0.4/setup.cfg
+-rw-r--r--   0 daegeun    (501) staff       (20)      674 2023-08-01 07:38:42.000000 Pygeun-0.0.4/setup.py
```

### Comparing `Pygeun-0.0.3/Pygeun/gradient_descent.py` & `Pygeun-0.0.4/Pygeun/gradient_descent.py`

 * *Files identical despite different names*

### Comparing `Pygeun-0.0.3/Pygeun/levenberg_marquardt.py` & `Pygeun-0.0.4/Pygeun/levenberg_marquardt.py`

 * *Files identical despite different names*

### Comparing `Pygeun-0.0.3/Pygeun/newton_raphson.py` & `Pygeun-0.0.4/Pygeun/newton_raphson.py`

 * *Files identical despite different names*

### Comparing `Pygeun-0.0.3/setup.py` & `Pygeun-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 
 
 setup(
     name='Pygeun',
-    version='0.0.3',
+    version='0.0.4',
     description='Pygeun is for convenience',
     author='Daegeun02',
     author_email='redhawkdg02@gmail.com',
     url='https://github.com/Daegeun02/Pygeun.git',
     install_requires=[],
     packages=find_packages( exclude=[] ),
     keywords=['Pygeun', 'by daegeun', 'for convenience'],
```

