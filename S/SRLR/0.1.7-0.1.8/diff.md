# Comparing `tmp/SRLR-0.1.7.tar.gz` & `tmp/SRLR-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SRLR-0.1.7.tar", last modified: Tue Aug  1 20:03:01 2023, max compression
+gzip compressed data, was "SRLR-0.1.8.tar", last modified: Tue Aug  1 20:06:57 2023, max compression
```

## Comparing `SRLR-0.1.7.tar` & `SRLR-0.1.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 siyueyang   (501) staff       (20)        0 2023-08-01 20:03:01.163974 SRLR-0.1.7/
--rw-r--r--   0 siyueyang   (501) staff       (20)        0 2023-07-31 19:49:25.000000 SRLR-0.1.7/LICENSE
--rw-r--r--   0 siyueyang   (501) staff       (20)     2365 2023-08-01 20:03:01.163436 SRLR-0.1.7/PKG-INFO
--rw-r--r--   0 siyueyang   (501) staff       (20)     1513 2023-07-31 19:48:02.000000 SRLR-0.1.7/README.md
--rw-r--r--   0 siyueyang   (501) staff       (20)       38 2023-08-01 20:03:01.164178 SRLR-0.1.7/setup.cfg
--rw-r--r--   0 siyueyang   (501) staff       (20)     1587 2023-08-01 20:02:58.000000 SRLR-0.1.7/setup.py
-drwxr-xr-x   0 siyueyang   (501) staff       (20)        0 2023-08-01 20:03:01.143873 SRLR-0.1.7/src/
-drwxr-xr-x   0 siyueyang   (501) staff       (20)        0 2023-08-01 20:03:01.155270 SRLR-0.1.7/src/SRLR/
--rw-r--r--   0 siyueyang   (501) staff       (20)      148 2023-08-01 19:20:07.000000 SRLR-0.1.7/src/SRLR/__init__.py
--rw-r--r--   0 siyueyang   (501) staff       (20)     7269 2023-07-31 21:25:12.000000 SRLR-0.1.7/src/SRLR/asymptotics.py
--rw-r--r--   0 siyueyang   (501) staff       (20)     2649 2023-07-31 21:25:20.000000 SRLR-0.1.7/src/SRLR/datasets.py
--rw-r--r--   0 siyueyang   (501) staff       (20)     2527 2023-07-31 19:48:02.000000 SRLR-0.1.7/src/SRLR/estimators.py
--rw-r--r--   0 siyueyang   (501) staff       (20)      854 2023-07-31 19:48:02.000000 SRLR-0.1.7/src/SRLR/optimal_m.py
--rw-r--r--   0 siyueyang   (501) staff       (20)     6093 2023-07-31 19:48:02.000000 SRLR-0.1.7/src/SRLR/simulation.py
--rw-r--r--   0 siyueyang   (501) staff       (20)    12479 2023-08-01 20:02:15.000000 SRLR-0.1.7/src/SRLR/utils.py
-drwxr-xr-x   0 siyueyang   (501) staff       (20)        0 2023-08-01 20:03:01.161532 SRLR-0.1.7/src/SRLR.egg-info/
--rw-r--r--   0 siyueyang   (501) staff       (20)     2365 2023-08-01 20:03:01.000000 SRLR-0.1.7/src/SRLR.egg-info/PKG-INFO
--rw-r--r--   0 siyueyang   (501) staff       (20)      337 2023-08-01 20:03:01.000000 SRLR-0.1.7/src/SRLR.egg-info/SOURCES.txt
--rw-r--r--   0 siyueyang   (501) staff       (20)        1 2023-08-01 20:03:01.000000 SRLR-0.1.7/src/SRLR.egg-info/dependency_links.txt
--rw-r--r--   0 siyueyang   (501) staff       (20)       87 2023-08-01 20:03:01.000000 SRLR-0.1.7/src/SRLR.egg-info/requires.txt
--rw-r--r--   0 siyueyang   (501) staff       (20)        5 2023-08-01 20:03:01.000000 SRLR-0.1.7/src/SRLR.egg-info/top_level.txt
+drwxr-xr-x   0 siyueyang   (501) staff       (20)        0 2023-08-01 20:06:57.785631 SRLR-0.1.8/
+-rw-r--r--   0 siyueyang   (501) staff       (20)        0 2023-07-31 19:49:25.000000 SRLR-0.1.8/LICENSE
+-rw-r--r--   0 siyueyang   (501) staff       (20)     2365 2023-08-01 20:06:57.785261 SRLR-0.1.8/PKG-INFO
+-rw-r--r--   0 siyueyang   (501) staff       (20)     1513 2023-07-31 19:48:02.000000 SRLR-0.1.8/README.md
+-rw-r--r--   0 siyueyang   (501) staff       (20)       38 2023-08-01 20:06:57.785747 SRLR-0.1.8/setup.cfg
+-rw-r--r--   0 siyueyang   (501) staff       (20)     1587 2023-08-01 20:06:54.000000 SRLR-0.1.8/setup.py
+drwxr-xr-x   0 siyueyang   (501) staff       (20)        0 2023-08-01 20:06:57.776634 SRLR-0.1.8/src/
+drwxr-xr-x   0 siyueyang   (501) staff       (20)        0 2023-08-01 20:06:57.783104 SRLR-0.1.8/src/SRLR/
+-rw-r--r--   0 siyueyang   (501) staff       (20)      148 2023-08-01 19:20:07.000000 SRLR-0.1.8/src/SRLR/__init__.py
+-rw-r--r--   0 siyueyang   (501) staff       (20)     7269 2023-07-31 21:25:12.000000 SRLR-0.1.8/src/SRLR/asymptotics.py
+-rw-r--r--   0 siyueyang   (501) staff       (20)     2649 2023-07-31 21:25:20.000000 SRLR-0.1.8/src/SRLR/datasets.py
+-rw-r--r--   0 siyueyang   (501) staff       (20)     2527 2023-07-31 19:48:02.000000 SRLR-0.1.8/src/SRLR/estimators.py
+-rw-r--r--   0 siyueyang   (501) staff       (20)      854 2023-07-31 19:48:02.000000 SRLR-0.1.8/src/SRLR/optimal_m.py
+-rw-r--r--   0 siyueyang   (501) staff       (20)     6093 2023-07-31 19:48:02.000000 SRLR-0.1.8/src/SRLR/simulation.py
+-rw-r--r--   0 siyueyang   (501) staff       (20)    12477 2023-08-01 20:05:17.000000 SRLR-0.1.8/src/SRLR/utils.py
+drwxr-xr-x   0 siyueyang   (501) staff       (20)        0 2023-08-01 20:06:57.784827 SRLR-0.1.8/src/SRLR.egg-info/
+-rw-r--r--   0 siyueyang   (501) staff       (20)     2365 2023-08-01 20:06:57.000000 SRLR-0.1.8/src/SRLR.egg-info/PKG-INFO
+-rw-r--r--   0 siyueyang   (501) staff       (20)      337 2023-08-01 20:06:57.000000 SRLR-0.1.8/src/SRLR.egg-info/SOURCES.txt
+-rw-r--r--   0 siyueyang   (501) staff       (20)        1 2023-08-01 20:06:57.000000 SRLR-0.1.8/src/SRLR.egg-info/dependency_links.txt
+-rw-r--r--   0 siyueyang   (501) staff       (20)       87 2023-08-01 20:06:57.000000 SRLR-0.1.8/src/SRLR.egg-info/requires.txt
+-rw-r--r--   0 siyueyang   (501) staff       (20)        5 2023-08-01 20:06:57.000000 SRLR-0.1.8/src/SRLR.egg-info/top_level.txt
```

### Comparing `SRLR-0.1.7/PKG-INFO` & `SRLR-0.1.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SRLR
-Version: 0.1.7
+Version: 0.1.8
 Summary: A package for sketched ridgeless estimator simulations, optimizing generalization. Identify the best sketching size to minimize out-of-sample risks. Stable risk curves in optimally sketched estimator eliminate peaks found in full-sample estimator. SRLR offers practical method to discover the ideal sketching size.
 Home-page: https://github.com/statsle/SRLR_python
 Author: Siyue Yang
 Author-email: syue.yang@mail.utoronto.ca
 License: MIT
 Keywords: python,sketched ridgeless linear regression
 Platform: UNKNOWN
```

### Comparing `SRLR-0.1.7/README.md` & `SRLR-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `SRLR-0.1.7/setup.py` & `SRLR-0.1.8/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 # Package metadata
 NAME = 'SRLR'
-VERSION = '0.1.7'
+VERSION = '0.1.8'
 DESCRIPTION = 'A package for sketched ridgeless estimator simulations, optimizing generalization. Identify the best sketching size to minimize out-of-sample risks. Stable risk curves in optimally sketched estimator eliminate peaks found in full-sample estimator. SRLR offers practical method to discover the ideal sketching size.'
 AUTHOR = 'Siyue Yang'
 EMAIL = 'syue.yang@mail.utoronto.ca'
 URL = 'https://github.com/statsle/SRLR_python'
 LICENSE = 'MIT'
 PYTHON_REQUIRES = '>=3.6'
```

### Comparing `SRLR-0.1.7/src/SRLR/asymptotics.py` & `SRLR-0.1.8/src/SRLR/asymptotics.py`

 * *Files identical despite different names*

### Comparing `SRLR-0.1.7/src/SRLR/datasets.py` & `SRLR-0.1.8/src/SRLR/datasets.py`

 * *Files identical despite different names*

### Comparing `SRLR-0.1.7/src/SRLR/estimators.py` & `SRLR-0.1.8/src/SRLR/estimators.py`

 * *Files identical despite different names*

### Comparing `SRLR-0.1.7/src/SRLR/optimal_m.py` & `SRLR-0.1.8/src/SRLR/optimal_m.py`

 * *Files identical despite different names*

### Comparing `SRLR-0.1.7/src/SRLR/simulation.py` & `SRLR-0.1.8/src/SRLR/simulation.py`

 * *Files identical despite different names*

### Comparing `SRLR-0.1.7/src/SRLR/utils.py` & `SRLR-0.1.8/src/SRLR/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -214,16 +214,16 @@
             if correlated:
                 alpha, sigma, emp_phi, emp_sketch_risk, phi, ridgeless_risk = load_files_cmp(file, correlated)
                 plt.scatter(x=emp_phi, y=emp_sketch_risk, color='darkred', s=60, label=sketching_type)
                 sns.lineplot(x=phi, y=ridgeless_risk, label="no sketching")
                 sns.lineplot(x=emp_phi, y=emp_sketch_risk, color='darkred')
             else:
                 alpha, sigma, emp_phi, emp_sketch_risk, emp_ridgeless_risk, phi, sketch_risk, ridgeless_risk = load_files_cmp(file, correlated=correlated)
-                plt.scatter(x=emp_phi, y=emp_ridgeless_risk, marker='X', s=60, label="no sketching")
-                plt.scatter(x=emp_phi, y=emp_sketch_risk, color='darkred', s=60, label=sketching_type)
+                ax.scatter(x=emp_phi, y=emp_ridgeless_risk, marker='X', s=60, label="no sketching")
+                ax.scatter(x=emp_phi, y=emp_sketch_risk, color='darkred', s=60, label=sketching_type)
                 sns.lineplot(x=phi, y=ridgeless_risk)
                 sns.lineplot(x=phi, y=sketch_risk, color='darkred')
             
             if snr is not None:
                 if snr > 1: 
                     ax.axvline(x=1, color="grey", linestyle='dashed', linewidth=1)
                     ax.axvspan((1 - sigma/(2*alpha)), alpha/(alpha - sigma), facecolor='pink', alpha=0.3, **dict())
```

### Comparing `SRLR-0.1.7/src/SRLR.egg-info/PKG-INFO` & `SRLR-0.1.8/src/SRLR.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SRLR
-Version: 0.1.7
+Version: 0.1.8
 Summary: A package for sketched ridgeless estimator simulations, optimizing generalization. Identify the best sketching size to minimize out-of-sample risks. Stable risk curves in optimally sketched estimator eliminate peaks found in full-sample estimator. SRLR offers practical method to discover the ideal sketching size.
 Home-page: https://github.com/statsle/SRLR_python
 Author: Siyue Yang
 Author-email: syue.yang@mail.utoronto.ca
 License: MIT
 Keywords: python,sketched ridgeless linear regression
 Platform: UNKNOWN
```

