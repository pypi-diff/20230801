# Comparing `tmp/SRLR-0.1.0.tar.gz` & `tmp/SRLR-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SRLR-0.1.0.tar", last modified: Tue Aug  1 19:02:42 2023, max compression
+gzip compressed data, was "SRLR-0.1.1.tar", last modified: Tue Aug  1 19:09:04 2023, max compression
```

## Comparing `SRLR-0.1.0.tar` & `SRLR-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 siyueyang   (501) staff       (20)        0 2023-08-01 19:02:42.082442 SRLR-0.1.0/
--rw-r--r--   0 siyueyang   (501) staff       (20)        0 2023-07-31 19:49:25.000000 SRLR-0.1.0/LICENSE
--rw-r--r--   0 siyueyang   (501) staff       (20)     2365 2023-08-01 19:02:42.082033 SRLR-0.1.0/PKG-INFO
--rw-r--r--   0 siyueyang   (501) staff       (20)     1513 2023-07-31 19:48:02.000000 SRLR-0.1.0/README.md
--rw-r--r--   0 siyueyang   (501) staff       (20)       38 2023-08-01 19:02:42.082606 SRLR-0.1.0/setup.cfg
--rw-r--r--   0 siyueyang   (501) staff       (20)     1587 2023-08-01 19:02:27.000000 SRLR-0.1.0/setup.py
-drwxr-xr-x   0 siyueyang   (501) staff       (20)        0 2023-08-01 19:02:42.073033 SRLR-0.1.0/src/
-drwxr-xr-x   0 siyueyang   (501) staff       (20)        0 2023-08-01 19:02:42.078383 SRLR-0.1.0/src/SRLR/
--rw-r--r--   0 siyueyang   (501) staff       (20)        0 2023-07-31 21:25:15.000000 SRLR-0.1.0/src/SRLR/__init__.py
--rw-r--r--   0 siyueyang   (501) staff       (20)     7269 2023-07-31 21:25:12.000000 SRLR-0.1.0/src/SRLR/asymptotics.py
--rw-r--r--   0 siyueyang   (501) staff       (20)     2649 2023-07-31 21:25:20.000000 SRLR-0.1.0/src/SRLR/datasets.py
--rw-r--r--   0 siyueyang   (501) staff       (20)     2527 2023-07-31 19:48:02.000000 SRLR-0.1.0/src/SRLR/estimators.py
--rw-r--r--   0 siyueyang   (501) staff       (20)      854 2023-07-31 19:48:02.000000 SRLR-0.1.0/src/SRLR/optimal_m.py
--rw-r--r--   0 siyueyang   (501) staff       (20)     6093 2023-07-31 19:48:02.000000 SRLR-0.1.0/src/SRLR/simulation.py
--rw-r--r--   0 siyueyang   (501) staff       (20)    12562 2023-07-31 19:48:02.000000 SRLR-0.1.0/src/SRLR/utils.py
-drwxr-xr-x   0 siyueyang   (501) staff       (20)        0 2023-08-01 19:02:42.081345 SRLR-0.1.0/src/SRLR.egg-info/
--rw-r--r--   0 siyueyang   (501) staff       (20)     2365 2023-08-01 19:02:42.000000 SRLR-0.1.0/src/SRLR.egg-info/PKG-INFO
--rw-r--r--   0 siyueyang   (501) staff       (20)      337 2023-08-01 19:02:42.000000 SRLR-0.1.0/src/SRLR.egg-info/SOURCES.txt
--rw-r--r--   0 siyueyang   (501) staff       (20)        1 2023-08-01 19:02:42.000000 SRLR-0.1.0/src/SRLR.egg-info/dependency_links.txt
--rw-r--r--   0 siyueyang   (501) staff       (20)       87 2023-08-01 19:02:42.000000 SRLR-0.1.0/src/SRLR.egg-info/requires.txt
--rw-r--r--   0 siyueyang   (501) staff       (20)        5 2023-08-01 19:02:42.000000 SRLR-0.1.0/src/SRLR.egg-info/top_level.txt
+drwxr-xr-x   0 siyueyang   (501) staff       (20)        0 2023-08-01 19:09:04.823789 SRLR-0.1.1/
+-rw-r--r--   0 siyueyang   (501) staff       (20)        0 2023-07-31 19:49:25.000000 SRLR-0.1.1/LICENSE
+-rw-r--r--   0 siyueyang   (501) staff       (20)     2365 2023-08-01 19:09:04.823385 SRLR-0.1.1/PKG-INFO
+-rw-r--r--   0 siyueyang   (501) staff       (20)     1513 2023-07-31 19:48:02.000000 SRLR-0.1.1/README.md
+-rw-r--r--   0 siyueyang   (501) staff       (20)       38 2023-08-01 19:09:04.823940 SRLR-0.1.1/setup.cfg
+-rw-r--r--   0 siyueyang   (501) staff       (20)     1587 2023-08-01 19:08:41.000000 SRLR-0.1.1/setup.py
+drwxr-xr-x   0 siyueyang   (501) staff       (20)        0 2023-08-01 19:09:04.814741 SRLR-0.1.1/src/
+drwxr-xr-x   0 siyueyang   (501) staff       (20)        0 2023-08-01 19:09:04.819213 SRLR-0.1.1/src/SRLR/
+-rw-r--r--   0 siyueyang   (501) staff       (20)       87 2023-08-01 19:07:37.000000 SRLR-0.1.1/src/SRLR/__init__.py
+-rw-r--r--   0 siyueyang   (501) staff       (20)     7269 2023-07-31 21:25:12.000000 SRLR-0.1.1/src/SRLR/asymptotics.py
+-rw-r--r--   0 siyueyang   (501) staff       (20)     2649 2023-07-31 21:25:20.000000 SRLR-0.1.1/src/SRLR/datasets.py
+-rw-r--r--   0 siyueyang   (501) staff       (20)     2527 2023-07-31 19:48:02.000000 SRLR-0.1.1/src/SRLR/estimators.py
+-rw-r--r--   0 siyueyang   (501) staff       (20)      854 2023-07-31 19:48:02.000000 SRLR-0.1.1/src/SRLR/optimal_m.py
+-rw-r--r--   0 siyueyang   (501) staff       (20)     6093 2023-07-31 19:48:02.000000 SRLR-0.1.1/src/SRLR/simulation.py
+-rw-r--r--   0 siyueyang   (501) staff       (20)    12562 2023-07-31 19:48:02.000000 SRLR-0.1.1/src/SRLR/utils.py
+drwxr-xr-x   0 siyueyang   (501) staff       (20)        0 2023-08-01 19:09:04.822568 SRLR-0.1.1/src/SRLR.egg-info/
+-rw-r--r--   0 siyueyang   (501) staff       (20)     2365 2023-08-01 19:09:04.000000 SRLR-0.1.1/src/SRLR.egg-info/PKG-INFO
+-rw-r--r--   0 siyueyang   (501) staff       (20)      337 2023-08-01 19:09:04.000000 SRLR-0.1.1/src/SRLR.egg-info/SOURCES.txt
+-rw-r--r--   0 siyueyang   (501) staff       (20)        1 2023-08-01 19:09:04.000000 SRLR-0.1.1/src/SRLR.egg-info/dependency_links.txt
+-rw-r--r--   0 siyueyang   (501) staff       (20)       87 2023-08-01 19:09:04.000000 SRLR-0.1.1/src/SRLR.egg-info/requires.txt
+-rw-r--r--   0 siyueyang   (501) staff       (20)        5 2023-08-01 19:09:04.000000 SRLR-0.1.1/src/SRLR.egg-info/top_level.txt
```

### Comparing `SRLR-0.1.0/PKG-INFO` & `SRLR-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SRLR
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package for sketched ridgeless estimator simulations, optimizing generalization. Identify the best sketching size to minimize out-of-sample risks. Stable risk curves in optimally sketched estimator eliminate peaks found in full-sample estimator. SRLR offers practical method to discover the ideal sketching size.
 Home-page: https://github.com/statsle/SRLR_python
 Author: Siyue Yang
 Author-email: syue.yang@mail.utoronto.ca
 License: MIT
 Keywords: python,sketched ridgeless linear regression
 Platform: UNKNOWN
```

### Comparing `SRLR-0.1.0/README.md` & `SRLR-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `SRLR-0.1.0/setup.py` & `SRLR-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 # Package metadata
 NAME = 'SRLR'
-VERSION = '0.1.0'
+VERSION = '0.1.1'
 DESCRIPTION = 'A package for sketched ridgeless estimator simulations, optimizing generalization. Identify the best sketching size to minimize out-of-sample risks. Stable risk curves in optimally sketched estimator eliminate peaks found in full-sample estimator. SRLR offers practical method to discover the ideal sketching size.'
 AUTHOR = 'Siyue Yang'
 EMAIL = 'syue.yang@mail.utoronto.ca'
 URL = 'https://github.com/statsle/SRLR_python'
 LICENSE = 'MIT'
 PYTHON_REQUIRES = '>=3.6'
```

### Comparing `SRLR-0.1.0/src/SRLR/asymptotics.py` & `SRLR-0.1.1/src/SRLR/asymptotics.py`

 * *Files identical despite different names*

### Comparing `SRLR-0.1.0/src/SRLR/datasets.py` & `SRLR-0.1.1/src/SRLR/datasets.py`

 * *Files identical despite different names*

### Comparing `SRLR-0.1.0/src/SRLR/estimators.py` & `SRLR-0.1.1/src/SRLR/estimators.py`

 * *Files identical despite different names*

### Comparing `SRLR-0.1.0/src/SRLR/optimal_m.py` & `SRLR-0.1.1/src/SRLR/optimal_m.py`

 * *Files identical despite different names*

### Comparing `SRLR-0.1.0/src/SRLR/simulation.py` & `SRLR-0.1.1/src/SRLR/simulation.py`

 * *Files identical despite different names*

### Comparing `SRLR-0.1.0/src/SRLR/utils.py` & `SRLR-0.1.1/src/SRLR/utils.py`

 * *Files identical despite different names*

### Comparing `SRLR-0.1.0/src/SRLR.egg-info/PKG-INFO` & `SRLR-0.1.1/src/SRLR.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SRLR
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package for sketched ridgeless estimator simulations, optimizing generalization. Identify the best sketching size to minimize out-of-sample risks. Stable risk curves in optimally sketched estimator eliminate peaks found in full-sample estimator. SRLR offers practical method to discover the ideal sketching size.
 Home-page: https://github.com/statsle/SRLR_python
 Author: Siyue Yang
 Author-email: syue.yang@mail.utoronto.ca
 License: MIT
 Keywords: python,sketched ridgeless linear regression
 Platform: UNKNOWN
```

