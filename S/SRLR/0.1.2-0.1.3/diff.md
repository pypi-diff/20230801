# Comparing `tmp/SRLR-0.1.2.tar.gz` & `tmp/SRLR-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SRLR-0.1.2.tar", last modified: Tue Aug  1 19:20:19 2023, max compression
+gzip compressed data, was "SRLR-0.1.3.tar", last modified: Tue Aug  1 19:25:08 2023, max compression
```

## Comparing `SRLR-0.1.2.tar` & `SRLR-0.1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 siyueyang   (501) staff       (20)        0 2023-08-01 19:20:19.344045 SRLR-0.1.2/
--rw-r--r--   0 siyueyang   (501) staff       (20)        0 2023-07-31 19:49:25.000000 SRLR-0.1.2/LICENSE
--rw-r--r--   0 siyueyang   (501) staff       (20)     2365 2023-08-01 19:20:19.343773 SRLR-0.1.2/PKG-INFO
--rw-r--r--   0 siyueyang   (501) staff       (20)     1513 2023-07-31 19:48:02.000000 SRLR-0.1.2/README.md
--rw-r--r--   0 siyueyang   (501) staff       (20)       38 2023-08-01 19:20:19.344146 SRLR-0.1.2/setup.cfg
--rw-r--r--   0 siyueyang   (501) staff       (20)     1587 2023-08-01 19:20:16.000000 SRLR-0.1.2/setup.py
-drwxr-xr-x   0 siyueyang   (501) staff       (20)        0 2023-08-01 19:20:19.337256 SRLR-0.1.2/src/
-drwxr-xr-x   0 siyueyang   (501) staff       (20)        0 2023-08-01 19:20:19.341467 SRLR-0.1.2/src/SRLR/
--rw-r--r--   0 siyueyang   (501) staff       (20)      148 2023-08-01 19:20:07.000000 SRLR-0.1.2/src/SRLR/__init__.py
--rw-r--r--   0 siyueyang   (501) staff       (20)     7269 2023-07-31 21:25:12.000000 SRLR-0.1.2/src/SRLR/asymptotics.py
--rw-r--r--   0 siyueyang   (501) staff       (20)     2649 2023-07-31 21:25:20.000000 SRLR-0.1.2/src/SRLR/datasets.py
--rw-r--r--   0 siyueyang   (501) staff       (20)     2527 2023-07-31 19:48:02.000000 SRLR-0.1.2/src/SRLR/estimators.py
--rw-r--r--   0 siyueyang   (501) staff       (20)      854 2023-07-31 19:48:02.000000 SRLR-0.1.2/src/SRLR/optimal_m.py
--rw-r--r--   0 siyueyang   (501) staff       (20)     6093 2023-07-31 19:48:02.000000 SRLR-0.1.2/src/SRLR/simulation.py
--rw-r--r--   0 siyueyang   (501) staff       (20)    12562 2023-07-31 19:48:02.000000 SRLR-0.1.2/src/SRLR/utils.py
-drwxr-xr-x   0 siyueyang   (501) staff       (20)        0 2023-08-01 19:20:19.343318 SRLR-0.1.2/src/SRLR.egg-info/
--rw-r--r--   0 siyueyang   (501) staff       (20)     2365 2023-08-01 19:20:19.000000 SRLR-0.1.2/src/SRLR.egg-info/PKG-INFO
--rw-r--r--   0 siyueyang   (501) staff       (20)      337 2023-08-01 19:20:19.000000 SRLR-0.1.2/src/SRLR.egg-info/SOURCES.txt
--rw-r--r--   0 siyueyang   (501) staff       (20)        1 2023-08-01 19:20:19.000000 SRLR-0.1.2/src/SRLR.egg-info/dependency_links.txt
--rw-r--r--   0 siyueyang   (501) staff       (20)       87 2023-08-01 19:20:19.000000 SRLR-0.1.2/src/SRLR.egg-info/requires.txt
--rw-r--r--   0 siyueyang   (501) staff       (20)        5 2023-08-01 19:20:19.000000 SRLR-0.1.2/src/SRLR.egg-info/top_level.txt
+drwxr-xr-x   0 siyueyang   (501) staff       (20)        0 2023-08-01 19:25:08.100972 SRLR-0.1.3/
+-rw-r--r--   0 siyueyang   (501) staff       (20)        0 2023-07-31 19:49:25.000000 SRLR-0.1.3/LICENSE
+-rw-r--r--   0 siyueyang   (501) staff       (20)     2365 2023-08-01 19:25:08.100321 SRLR-0.1.3/PKG-INFO
+-rw-r--r--   0 siyueyang   (501) staff       (20)     1513 2023-07-31 19:48:02.000000 SRLR-0.1.3/README.md
+-rw-r--r--   0 siyueyang   (501) staff       (20)       38 2023-08-01 19:25:08.101138 SRLR-0.1.3/setup.cfg
+-rw-r--r--   0 siyueyang   (501) staff       (20)     1587 2023-08-01 19:24:42.000000 SRLR-0.1.3/setup.py
+drwxr-xr-x   0 siyueyang   (501) staff       (20)        0 2023-08-01 19:25:08.091939 SRLR-0.1.3/src/
+drwxr-xr-x   0 siyueyang   (501) staff       (20)        0 2023-08-01 19:25:08.096492 SRLR-0.1.3/src/SRLR/
+-rw-r--r--   0 siyueyang   (501) staff       (20)      148 2023-08-01 19:20:07.000000 SRLR-0.1.3/src/SRLR/__init__.py
+-rw-r--r--   0 siyueyang   (501) staff       (20)     7269 2023-07-31 21:25:12.000000 SRLR-0.1.3/src/SRLR/asymptotics.py
+-rw-r--r--   0 siyueyang   (501) staff       (20)     2649 2023-07-31 21:25:20.000000 SRLR-0.1.3/src/SRLR/datasets.py
+-rw-r--r--   0 siyueyang   (501) staff       (20)     2527 2023-07-31 19:48:02.000000 SRLR-0.1.3/src/SRLR/estimators.py
+-rw-r--r--   0 siyueyang   (501) staff       (20)      854 2023-07-31 19:48:02.000000 SRLR-0.1.3/src/SRLR/optimal_m.py
+-rw-r--r--   0 siyueyang   (501) staff       (20)     6093 2023-07-31 19:48:02.000000 SRLR-0.1.3/src/SRLR/simulation.py
+-rw-r--r--   0 siyueyang   (501) staff       (20)    12538 2023-08-01 19:24:33.000000 SRLR-0.1.3/src/SRLR/utils.py
+drwxr-xr-x   0 siyueyang   (501) staff       (20)        0 2023-08-01 19:25:08.099583 SRLR-0.1.3/src/SRLR.egg-info/
+-rw-r--r--   0 siyueyang   (501) staff       (20)     2365 2023-08-01 19:25:08.000000 SRLR-0.1.3/src/SRLR.egg-info/PKG-INFO
+-rw-r--r--   0 siyueyang   (501) staff       (20)      337 2023-08-01 19:25:08.000000 SRLR-0.1.3/src/SRLR.egg-info/SOURCES.txt
+-rw-r--r--   0 siyueyang   (501) staff       (20)        1 2023-08-01 19:25:08.000000 SRLR-0.1.3/src/SRLR.egg-info/dependency_links.txt
+-rw-r--r--   0 siyueyang   (501) staff       (20)       87 2023-08-01 19:25:08.000000 SRLR-0.1.3/src/SRLR.egg-info/requires.txt
+-rw-r--r--   0 siyueyang   (501) staff       (20)        5 2023-08-01 19:25:08.000000 SRLR-0.1.3/src/SRLR.egg-info/top_level.txt
```

### Comparing `SRLR-0.1.2/PKG-INFO` & `SRLR-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SRLR
-Version: 0.1.2
+Version: 0.1.3
 Summary: A package for sketched ridgeless estimator simulations, optimizing generalization. Identify the best sketching size to minimize out-of-sample risks. Stable risk curves in optimally sketched estimator eliminate peaks found in full-sample estimator. SRLR offers practical method to discover the ideal sketching size.
 Home-page: https://github.com/statsle/SRLR_python
 Author: Siyue Yang
 Author-email: syue.yang@mail.utoronto.ca
 License: MIT
 Keywords: python,sketched ridgeless linear regression
 Platform: UNKNOWN
```

### Comparing `SRLR-0.1.2/README.md` & `SRLR-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `SRLR-0.1.2/setup.py` & `SRLR-0.1.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 # Package metadata
 NAME = 'SRLR'
-VERSION = '0.1.2'
+VERSION = '0.1.3'
 DESCRIPTION = 'A package for sketched ridgeless estimator simulations, optimizing generalization. Identify the best sketching size to minimize out-of-sample risks. Stable risk curves in optimally sketched estimator eliminate peaks found in full-sample estimator. SRLR offers practical method to discover the ideal sketching size.'
 AUTHOR = 'Siyue Yang'
 EMAIL = 'syue.yang@mail.utoronto.ca'
 URL = 'https://github.com/statsle/SRLR_python'
 LICENSE = 'MIT'
 PYTHON_REQUIRES = '>=3.6'
```

### Comparing `SRLR-0.1.2/src/SRLR/asymptotics.py` & `SRLR-0.1.3/src/SRLR/asymptotics.py`

 * *Files identical despite different names*

### Comparing `SRLR-0.1.2/src/SRLR/datasets.py` & `SRLR-0.1.3/src/SRLR/datasets.py`

 * *Files identical despite different names*

### Comparing `SRLR-0.1.2/src/SRLR/estimators.py` & `SRLR-0.1.3/src/SRLR/estimators.py`

 * *Files identical despite different names*

### Comparing `SRLR-0.1.2/src/SRLR/optimal_m.py` & `SRLR-0.1.3/src/SRLR/optimal_m.py`

 * *Files identical despite different names*

### Comparing `SRLR-0.1.2/src/SRLR/simulation.py` & `SRLR-0.1.3/src/SRLR/simulation.py`

 * *Files identical despite different names*

### Comparing `SRLR-0.1.2/src/SRLR/utils.py` & `SRLR-0.1.3/src/SRLR/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,15 @@
     
     Parameters:
     - file_loc: location of the file
     
     Returns:
     - snr, emp_psi, emp_risk, psi, risk
     """
-    file = json.loads(codecs.open('result/' + file_loc, 'r').read())
+    file = json.loads(codecs.open(file_loc, 'r').read())
     if fix_psi:
         emp_phi = file["emp_phi"]
         emp_risk = file["emp_risk"]
         phi = file["phi"]
         risk = file["risk"]
         return file["alpha"]/file["sigma"], emp_phi, emp_risk, phi, risk
     else:
@@ -115,15 +115,15 @@
         emp_risk = file["emp_risk"]
         psi = file["psi"]
         risk = file["risk"]
         return file["alpha"]/file["sigma"], emp_psi, emp_risk, psi, risk
 
 
 def load_files_cmp(file_loc, correlated=False):
-    file = json.loads(codecs.open('result/' + file_loc, 'r').read())
+    file = json.loads(codecs.open(file_loc, 'r').read())
     emp_phi = file["emp_phi"]
     emp_sketch_risk = file["emp_sketch_risk"]
 
     phi = file["phi"]
     ridgeless_risk = file["ridgeless_risk"]
 
     if not correlated:
```

### Comparing `SRLR-0.1.2/src/SRLR.egg-info/PKG-INFO` & `SRLR-0.1.3/src/SRLR.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SRLR
-Version: 0.1.2
+Version: 0.1.3
 Summary: A package for sketched ridgeless estimator simulations, optimizing generalization. Identify the best sketching size to minimize out-of-sample risks. Stable risk curves in optimally sketched estimator eliminate peaks found in full-sample estimator. SRLR offers practical method to discover the ideal sketching size.
 Home-page: https://github.com/statsle/SRLR_python
 Author: Siyue Yang
 Author-email: syue.yang@mail.utoronto.ca
 License: MIT
 Keywords: python,sketched ridgeless linear regression
 Platform: UNKNOWN
```

