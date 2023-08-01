# Comparing `tmp/python-wars-solo-2.0.tar.gz` & `tmp/Python-Wars-Solo-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/python-wars-solo-2.0.tar", last modified: Wed Nov  8 05:33:10 2017, max compression
+gzip compressed data, was "Python-Wars-Solo-3.0.0.tar", last modified: Tue Aug  1 12:52:07 2023, max compression
```

## Comparing `python-wars-solo-2.0.tar` & `Python-Wars-Solo-3.0.0.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxr-xr-x   0 danielgreenfeld   (501) staff       (20)        0 2017-11-08 05:33:10.000000 python-wars-solo-2.0/
--rw-r--r--   0 danielgreenfeld   (501) staff       (20)     4218 2017-11-08 05:17:49.000000 python-wars-solo-2.0/go.py
--rw-r--r--   0 danielgreenfeld   (501) staff       (20)     3847 2017-11-08 05:33:10.000000 python-wars-solo-2.0/PKG-INFO
-drwxr-xr-x   0 danielgreenfeld   (501) staff       (20)        0 2017-11-08 05:33:10.000000 python-wars-solo-2.0/python_wars_solo.egg-info/
--rw-r--r--   0 danielgreenfeld   (501) staff       (20)        1 2017-11-08 05:33:10.000000 python-wars-solo-2.0/python_wars_solo.egg-info/dependency_links.txt
--rw-r--r--   0 danielgreenfeld   (501) staff       (20)       43 2017-11-08 05:33:10.000000 python-wars-solo-2.0/python_wars_solo.egg-info/entry_points.txt
--rw-r--r--   0 danielgreenfeld   (501) staff       (20)     3847 2017-11-08 05:33:10.000000 python-wars-solo-2.0/python_wars_solo.egg-info/PKG-INFO
--rw-r--r--   0 danielgreenfeld   (501) staff       (20)      237 2017-11-08 05:33:10.000000 python-wars-solo-2.0/python_wars_solo.egg-info/SOURCES.txt
--rw-r--r--   0 danielgreenfeld   (501) staff       (20)        9 2017-11-08 05:33:10.000000 python-wars-solo-2.0/python_wars_solo.egg-info/top_level.txt
--rw-r--r--   0 danielgreenfeld   (501) staff       (20)     2683 2017-11-08 05:23:00.000000 python-wars-solo-2.0/README.rst
--rw-r--r--   0 danielgreenfeld   (501) staff       (20)       38 2017-11-08 05:33:10.000000 python-wars-solo-2.0/setup.cfg
--rw-r--r--   0 danielgreenfeld   (501) staff       (20)     1458 2017-11-08 05:32:16.000000 python-wars-solo-2.0/setup.py
--rw-r--r--   0 danielgreenfeld   (501) staff       (20)     5269 2017-11-08 05:17:49.000000 python-wars-solo-2.0/stuff.py
+drwxr-xr-x   0 drg        (501) staff       (20)        0 2023-08-01 12:52:07.050560 Python-Wars-Solo-3.0.0/
+-rw-r--r--   0 drg        (501) staff       (20)      667 2023-08-01 10:06:47.000000 Python-Wars-Solo-3.0.0/LICENSE.txt
+-rw-r--r--   0 drg        (501) staff       (20)     4329 2023-08-01 12:52:07.050205 Python-Wars-Solo-3.0.0/PKG-INFO
+-rw-r--r--   0 drg        (501) staff       (20)     2683 2023-08-01 10:06:47.000000 Python-Wars-Solo-3.0.0/README.rst
+-rw-r--r--   0 drg        (501) staff       (20)      979 2023-08-01 12:51:49.000000 Python-Wars-Solo-3.0.0/pyproject.toml
+-rw-r--r--   0 drg        (501) staff       (20)       38 2023-08-01 12:52:07.050680 Python-Wars-Solo-3.0.0/setup.cfg
+drwxr-xr-x   0 drg        (501) staff       (20)        0 2023-08-01 12:52:07.046798 Python-Wars-Solo-3.0.0/src/
+drwxr-xr-x   0 drg        (501) staff       (20)        0 2023-08-01 12:52:07.049698 Python-Wars-Solo-3.0.0/src/Python_Wars_Solo.egg-info/
+-rw-r--r--   0 drg        (501) staff       (20)     4329 2023-08-01 12:52:07.000000 Python-Wars-Solo-3.0.0/src/Python_Wars_Solo.egg-info/PKG-INFO
+-rw-r--r--   0 drg        (501) staff       (20)      283 2023-08-01 12:52:07.000000 Python-Wars-Solo-3.0.0/src/Python_Wars_Solo.egg-info/SOURCES.txt
+-rw-r--r--   0 drg        (501) staff       (20)        1 2023-08-01 12:52:07.000000 Python-Wars-Solo-3.0.0/src/Python_Wars_Solo.egg-info/dependency_links.txt
+-rw-r--r--   0 drg        (501) staff       (20)       42 2023-08-01 12:52:07.000000 Python-Wars-Solo-3.0.0/src/Python_Wars_Solo.egg-info/entry_points.txt
+-rw-r--r--   0 drg        (501) staff       (20)        9 2023-08-01 12:52:07.000000 Python-Wars-Solo-3.0.0/src/Python_Wars_Solo.egg-info/top_level.txt
+-rw-r--r--   0 drg        (501) staff       (20)     4218 2023-08-01 10:06:47.000000 Python-Wars-Solo-3.0.0/src/go.py
+-rw-r--r--   0 drg        (501) staff       (20)     5269 2023-08-01 10:06:47.000000 Python-Wars-Solo-3.0.0/src/stuff.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `python-wars-solo-2.0/go.py` & `Python-Wars-Solo-3.0.0/src/go.py`

 * *Files identical despite different names*

### Comparing `python-wars-solo-2.0/README.rst` & `Python-Wars-Solo-3.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `python-wars-solo-2.0/stuff.py` & `Python-Wars-Solo-3.0.0/src/stuff.py`

 * *Files identical despite different names*

