# Comparing `tmp/Pygeun-0.0.1.tar.gz` & `tmp/Pygeun-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pygeun-0.0.1.tar", last modified: Tue Aug  1 07:20:14 2023, max compression
+gzip compressed data, was "Pygeun-0.0.2.tar", last modified: Tue Aug  1 07:33:06 2023, max compression
```

## Comparing `Pygeun-0.0.1.tar` & `Pygeun-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-01 07:20:14.937106 Pygeun-0.0.1/
--rw-r--r--   0 daegeun    (501) staff       (20)      503 2023-08-01 07:20:14.936887 Pygeun-0.0.1/PKG-INFO
-drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-01 07:20:14.935008 Pygeun-0.0.1/Pygeun.egg-info/
--rw-r--r--   0 daegeun    (501) staff       (20)      503 2023-08-01 07:20:14.000000 Pygeun-0.0.1/Pygeun.egg-info/PKG-INFO
--rw-r--r--   0 daegeun    (501) staff       (20)      292 2023-08-01 07:20:14.000000 Pygeun-0.0.1/Pygeun.egg-info/SOURCES.txt
--rw-r--r--   0 daegeun    (501) staff       (20)        1 2023-08-01 07:20:14.000000 Pygeun-0.0.1/Pygeun.egg-info/dependency_links.txt
--rw-r--r--   0 daegeun    (501) staff       (20)        1 2023-08-01 07:20:14.000000 Pygeun-0.0.1/Pygeun.egg-info/not-zip-safe
--rw-r--r--   0 daegeun    (501) staff       (20)       13 2023-08-01 07:20:14.000000 Pygeun-0.0.1/Pygeun.egg-info/top_level.txt
--rw-r--r--   0 daegeun    (501) staff       (20)       49 2023-08-01 07:16:34.000000 Pygeun-0.0.1/README.md
-drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-01 07:20:14.936489 Pygeun-0.0.1/optimization/
--rw-r--r--   0 daegeun    (501) staff       (20)      430 2023-08-01 07:19:24.000000 Pygeun-0.0.1/optimization/__init__.py
--rw-r--r--   0 daegeun    (501) staff       (20)      996 2023-06-01 09:57:12.000000 Pygeun-0.0.1/optimization/gradient_descent.py
--rw-r--r--   0 daegeun    (501) staff       (20)     2170 2023-05-10 09:39:09.000000 Pygeun-0.0.1/optimization/levenberg_marquardt.py
--rw-r--r--   0 daegeun    (501) staff       (20)     1140 2023-05-28 06:20:21.000000 Pygeun-0.0.1/optimization/newton_raphson.py
--rw-r--r--   0 daegeun    (501) staff       (20)       38 2023-08-01 07:20:14.937179 Pygeun-0.0.1/setup.cfg
--rw-r--r--   0 daegeun    (501) staff       (20)      674 2023-08-01 07:19:01.000000 Pygeun-0.0.1/setup.py
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-01 07:33:06.898915 Pygeun-0.0.2/
+-rw-r--r--   0 daegeun    (501) staff       (20)      503 2023-08-01 07:33:06.898697 Pygeun-0.0.2/PKG-INFO
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-01 07:33:06.897215 Pygeun-0.0.2/Pygeun/
+-rw-r--r--   0 daegeun    (501) staff       (20)      430 2023-08-01 07:29:23.000000 Pygeun-0.0.2/Pygeun/__init__.py
+-rw-r--r--   0 daegeun    (501) staff       (20)      996 2023-06-01 09:57:12.000000 Pygeun-0.0.2/Pygeun/gradient_descent.py
+-rw-r--r--   0 daegeun    (501) staff       (20)     2170 2023-05-10 09:39:09.000000 Pygeun-0.0.2/Pygeun/levenberg_marquardt.py
+-rw-r--r--   0 daegeun    (501) staff       (20)     1140 2023-05-28 06:20:21.000000 Pygeun-0.0.2/Pygeun/newton_raphson.py
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-01 07:33:06.898351 Pygeun-0.0.2/Pygeun.egg-info/
+-rw-r--r--   0 daegeun    (501) staff       (20)      503 2023-08-01 07:33:06.000000 Pygeun-0.0.2/Pygeun.egg-info/PKG-INFO
+-rw-r--r--   0 daegeun    (501) staff       (20)      268 2023-08-01 07:33:06.000000 Pygeun-0.0.2/Pygeun.egg-info/SOURCES.txt
+-rw-r--r--   0 daegeun    (501) staff       (20)        1 2023-08-01 07:33:06.000000 Pygeun-0.0.2/Pygeun.egg-info/dependency_links.txt
+-rw-r--r--   0 daegeun    (501) staff       (20)        1 2023-08-01 07:33:06.000000 Pygeun-0.0.2/Pygeun.egg-info/not-zip-safe
+-rw-r--r--   0 daegeun    (501) staff       (20)        7 2023-08-01 07:33:06.000000 Pygeun-0.0.2/Pygeun.egg-info/top_level.txt
+-rw-r--r--   0 daegeun    (501) staff       (20)       49 2023-08-01 07:16:34.000000 Pygeun-0.0.2/README.md
+-rw-r--r--   0 daegeun    (501) staff       (20)       38 2023-08-01 07:33:06.898985 Pygeun-0.0.2/setup.cfg
+-rw-r--r--   0 daegeun    (501) staff       (20)      674 2023-08-01 07:29:20.000000 Pygeun-0.0.2/setup.py
```

### Comparing `Pygeun-0.0.1/optimization/gradient_descent.py` & `Pygeun-0.0.2/Pygeun/gradient_descent.py`

 * *Files identical despite different names*

### Comparing `Pygeun-0.0.1/optimization/levenberg_marquardt.py` & `Pygeun-0.0.2/Pygeun/levenberg_marquardt.py`

 * *Files identical despite different names*

### Comparing `Pygeun-0.0.1/optimization/newton_raphson.py` & `Pygeun-0.0.2/Pygeun/newton_raphson.py`

 * *Files identical despite different names*

### Comparing `Pygeun-0.0.1/setup.py` & `Pygeun-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 
 
 setup(
     name='Pygeun',
-    version='0.0.1',
+    version='0.0.2',
     description='Pygeun is for convenience',
     author='Daegeun02',
     author_email='redhawkdg02@gmail.com',
     url='https://github.com/Daegeun02/Pygeun.git',
     install_requires=[],
     packages=find_packages( exclude=[] ),
     keywords=['Pygeun', 'by daegeun', 'for convenience'],
```

