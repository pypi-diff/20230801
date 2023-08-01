# Comparing `tmp/SRLR-0.1.5.tar.gz` & `tmp/SRLR-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SRLR-0.1.5.tar", last modified: Tue Aug  1 19:57:36 2023, max compression
+gzip compressed data, was "SRLR-0.1.6.tar", last modified: Tue Aug  1 20:00:34 2023, max compression
```

## Comparing `SRLR-0.1.5.tar` & `SRLR-0.1.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 siyueyang   (501) staff       (20)        0 2023-08-01 19:57:36.409671 SRLR-0.1.5/
--rw-r--r--   0 siyueyang   (501) staff       (20)        0 2023-07-31 19:49:25.000000 SRLR-0.1.5/LICENSE
--rw-r--r--   0 siyueyang   (501) staff       (20)     2365 2023-08-01 19:57:36.409384 SRLR-0.1.5/PKG-INFO
--rw-r--r--   0 siyueyang   (501) staff       (20)     1513 2023-07-31 19:48:02.000000 SRLR-0.1.5/README.md
--rw-r--r--   0 siyueyang   (501) staff       (20)       38 2023-08-01 19:57:36.409809 SRLR-0.1.5/setup.cfg
--rw-r--r--   0 siyueyang   (501) staff       (20)     1587 2023-08-01 19:57:32.000000 SRLR-0.1.5/setup.py
-drwxr-xr-x   0 siyueyang   (501) staff       (20)        0 2023-08-01 19:57:36.400769 SRLR-0.1.5/src/
-drwxr-xr-x   0 siyueyang   (501) staff       (20)        0 2023-08-01 19:57:36.405995 SRLR-0.1.5/src/SRLR/
--rw-r--r--   0 siyueyang   (501) staff       (20)      148 2023-08-01 19:20:07.000000 SRLR-0.1.5/src/SRLR/__init__.py
--rw-r--r--   0 siyueyang   (501) staff       (20)     7269 2023-07-31 21:25:12.000000 SRLR-0.1.5/src/SRLR/asymptotics.py
--rw-r--r--   0 siyueyang   (501) staff       (20)     2649 2023-07-31 21:25:20.000000 SRLR-0.1.5/src/SRLR/datasets.py
--rw-r--r--   0 siyueyang   (501) staff       (20)     2527 2023-07-31 19:48:02.000000 SRLR-0.1.5/src/SRLR/estimators.py
--rw-r--r--   0 siyueyang   (501) staff       (20)      854 2023-07-31 19:48:02.000000 SRLR-0.1.5/src/SRLR/optimal_m.py
--rw-r--r--   0 siyueyang   (501) staff       (20)     6093 2023-07-31 19:48:02.000000 SRLR-0.1.5/src/SRLR/simulation.py
--rw-r--r--   0 siyueyang   (501) staff       (20)    12461 2023-08-01 19:57:15.000000 SRLR-0.1.5/src/SRLR/utils.py
-drwxr-xr-x   0 siyueyang   (501) staff       (20)        0 2023-08-01 19:57:36.408779 SRLR-0.1.5/src/SRLR.egg-info/
--rw-r--r--   0 siyueyang   (501) staff       (20)     2365 2023-08-01 19:57:36.000000 SRLR-0.1.5/src/SRLR.egg-info/PKG-INFO
--rw-r--r--   0 siyueyang   (501) staff       (20)      337 2023-08-01 19:57:36.000000 SRLR-0.1.5/src/SRLR.egg-info/SOURCES.txt
--rw-r--r--   0 siyueyang   (501) staff       (20)        1 2023-08-01 19:57:36.000000 SRLR-0.1.5/src/SRLR.egg-info/dependency_links.txt
--rw-r--r--   0 siyueyang   (501) staff       (20)       87 2023-08-01 19:57:36.000000 SRLR-0.1.5/src/SRLR.egg-info/requires.txt
--rw-r--r--   0 siyueyang   (501) staff       (20)        5 2023-08-01 19:57:36.000000 SRLR-0.1.5/src/SRLR.egg-info/top_level.txt
+drwxr-xr-x   0 siyueyang   (501) staff       (20)        0 2023-08-01 20:00:34.123022 SRLR-0.1.6/
+-rw-r--r--   0 siyueyang   (501) staff       (20)        0 2023-07-31 19:49:25.000000 SRLR-0.1.6/LICENSE
+-rw-r--r--   0 siyueyang   (501) staff       (20)     2365 2023-08-01 20:00:34.122748 SRLR-0.1.6/PKG-INFO
+-rw-r--r--   0 siyueyang   (501) staff       (20)     1513 2023-07-31 19:48:02.000000 SRLR-0.1.6/README.md
+-rw-r--r--   0 siyueyang   (501) staff       (20)       38 2023-08-01 20:00:34.123149 SRLR-0.1.6/setup.cfg
+-rw-r--r--   0 siyueyang   (501) staff       (20)     1587 2023-08-01 19:59:51.000000 SRLR-0.1.6/setup.py
+drwxr-xr-x   0 siyueyang   (501) staff       (20)        0 2023-08-01 20:00:34.116500 SRLR-0.1.6/src/
+drwxr-xr-x   0 siyueyang   (501) staff       (20)        0 2023-08-01 20:00:34.120237 SRLR-0.1.6/src/SRLR/
+-rw-r--r--   0 siyueyang   (501) staff       (20)      148 2023-08-01 19:20:07.000000 SRLR-0.1.6/src/SRLR/__init__.py
+-rw-r--r--   0 siyueyang   (501) staff       (20)     7269 2023-07-31 21:25:12.000000 SRLR-0.1.6/src/SRLR/asymptotics.py
+-rw-r--r--   0 siyueyang   (501) staff       (20)     2649 2023-07-31 21:25:20.000000 SRLR-0.1.6/src/SRLR/datasets.py
+-rw-r--r--   0 siyueyang   (501) staff       (20)     2527 2023-07-31 19:48:02.000000 SRLR-0.1.6/src/SRLR/estimators.py
+-rw-r--r--   0 siyueyang   (501) staff       (20)      854 2023-07-31 19:48:02.000000 SRLR-0.1.6/src/SRLR/optimal_m.py
+-rw-r--r--   0 siyueyang   (501) staff       (20)     6093 2023-07-31 19:48:02.000000 SRLR-0.1.6/src/SRLR/simulation.py
+-rw-r--r--   0 siyueyang   (501) staff       (20)    12514 2023-08-01 20:00:24.000000 SRLR-0.1.6/src/SRLR/utils.py
+drwxr-xr-x   0 siyueyang   (501) staff       (20)        0 2023-08-01 20:00:34.122277 SRLR-0.1.6/src/SRLR.egg-info/
+-rw-r--r--   0 siyueyang   (501) staff       (20)     2365 2023-08-01 20:00:34.000000 SRLR-0.1.6/src/SRLR.egg-info/PKG-INFO
+-rw-r--r--   0 siyueyang   (501) staff       (20)      337 2023-08-01 20:00:34.000000 SRLR-0.1.6/src/SRLR.egg-info/SOURCES.txt
+-rw-r--r--   0 siyueyang   (501) staff       (20)        1 2023-08-01 20:00:34.000000 SRLR-0.1.6/src/SRLR.egg-info/dependency_links.txt
+-rw-r--r--   0 siyueyang   (501) staff       (20)       87 2023-08-01 20:00:34.000000 SRLR-0.1.6/src/SRLR.egg-info/requires.txt
+-rw-r--r--   0 siyueyang   (501) staff       (20)        5 2023-08-01 20:00:34.000000 SRLR-0.1.6/src/SRLR.egg-info/top_level.txt
```

### Comparing `SRLR-0.1.5/PKG-INFO` & `SRLR-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SRLR
-Version: 0.1.5
+Version: 0.1.6
 Summary: A package for sketched ridgeless estimator simulations, optimizing generalization. Identify the best sketching size to minimize out-of-sample risks. Stable risk curves in optimally sketched estimator eliminate peaks found in full-sample estimator. SRLR offers practical method to discover the ideal sketching size.
 Home-page: https://github.com/statsle/SRLR_python
 Author: Siyue Yang
 Author-email: syue.yang@mail.utoronto.ca
 License: MIT
 Keywords: python,sketched ridgeless linear regression
 Platform: UNKNOWN
```

### Comparing `SRLR-0.1.5/README.md` & `SRLR-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `SRLR-0.1.5/setup.py` & `SRLR-0.1.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 # Package metadata
 NAME = 'SRLR'
-VERSION = '0.1.5'
+VERSION = '0.1.6'
 DESCRIPTION = 'A package for sketched ridgeless estimator simulations, optimizing generalization. Identify the best sketching size to minimize out-of-sample risks. Stable risk curves in optimally sketched estimator eliminate peaks found in full-sample estimator. SRLR offers practical method to discover the ideal sketching size.'
 AUTHOR = 'Siyue Yang'
 EMAIL = 'syue.yang@mail.utoronto.ca'
 URL = 'https://github.com/statsle/SRLR_python'
 LICENSE = 'MIT'
 PYTHON_REQUIRES = '>=3.6'
```

### Comparing `SRLR-0.1.5/src/SRLR/asymptotics.py` & `SRLR-0.1.6/src/SRLR/asymptotics.py`

 * *Files identical despite different names*

### Comparing `SRLR-0.1.5/src/SRLR/datasets.py` & `SRLR-0.1.6/src/SRLR/datasets.py`

 * *Files identical despite different names*

### Comparing `SRLR-0.1.5/src/SRLR/estimators.py` & `SRLR-0.1.6/src/SRLR/estimators.py`

 * *Files identical despite different names*

### Comparing `SRLR-0.1.5/src/SRLR/optimal_m.py` & `SRLR-0.1.6/src/SRLR/optimal_m.py`

 * *Files identical despite different names*

### Comparing `SRLR-0.1.5/src/SRLR/simulation.py` & `SRLR-0.1.6/src/SRLR/simulation.py`

 * *Files identical despite different names*

### Comparing `SRLR-0.1.5/src/SRLR/utils.py` & `SRLR-0.1.6/src/SRLR/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -209,23 +209,23 @@
             if 'orthogonal' in file:
                 sketching_type = "orthogonal sketching"
             else:
                 sketching_type = "i.i.d. sketching"
         
             if correlated:
                 alpha, sigma, emp_phi, emp_sketch_risk, phi, ridgeless_risk = load_files_cmp(file, correlated)
-                plt.scatter(x=emp_phi, y=emp_sketch_risk, color='darkred', s=60, label=sketching_type)
-                sns.lineplot(x=phi, y=ridgeless_risk, label="no sketching")
-                sns.lineplot(x=emp_phi, y=emp_sketch_risk, color='darkred')
+                ax = plt.scatter(x=emp_phi, y=emp_sketch_risk, color='darkred', s=60, label=sketching_type)
+                ax = sns.lineplot(x=phi, y=ridgeless_risk, label="no sketching")
+                ax = sns.lineplot(x=emp_phi, y=emp_sketch_risk, color='darkred')
             else:
                 alpha, sigma, emp_phi, emp_sketch_risk, emp_ridgeless_risk, phi, sketch_risk, ridgeless_risk = load_files_cmp(file, correlated=correlated)
-                plt.scatter(x=emp_phi, y=emp_ridgeless_risk, marker='X', s=60, label="no sketching", ax=ax)
-                plt.scatter(x=emp_phi, y=emp_sketch_risk, color='darkred', s=60, label=sketching_type)
-                sns.lineplot(x=phi, y=ridgeless_risk)
-                sns.lineplot(x=phi, y=sketch_risk, color='darkred')
+                ax = plt.scatter(x=emp_phi, y=emp_ridgeless_risk, marker='X', s=60, label="no sketching")
+                ax = plt.scatter(x=emp_phi, y=emp_sketch_risk, color='darkred', s=60, label=sketching_type)
+                ax = sns.lineplot(x=phi, y=ridgeless_risk)
+                ax = sns.lineplot(x=phi, y=sketch_risk, color='darkred')
             
             if snr is not None:
                 if snr > 1: 
                     ax.axvline(x=1, color="grey", linestyle='dashed', linewidth=1)
                     ax.axvspan((1 - sigma/(2*alpha)), alpha/(alpha - sigma), facecolor='pink', alpha=0.3, **dict())
                     ax.axvline(x=(1 - sigma/(2*alpha)), color="grey", linestyle='dashed', linewidth=1)
                     ax.axvline(x=alpha/(alpha - sigma), color="grey", linestyle='dashed', linewidth=1)
@@ -269,25 +269,25 @@
     ticks = [0.1, 0.2, 0.5, 1, 2, 5, 10]
     labels = [i for i in ticks]
 
     with plt.style.context(['science', 'no-latex', 'std-colors']):
         fig, ax = plt.subplots(1, 1, figsize=(6, 5))
         for i, file in enumerate(files_base):
             alpha, sigma, emp_phi, emp_sketch_risk, phi, ridgeless_risk = load_files_cmp(file, correlated=True)
-            sns.lineplot(x=phi, y=ridgeless_risk, label="no sketching")
-            sns.lineplot(x=emp_phi, y=emp_sketch_risk, color='darkred')
-            plt.scatter(x=emp_phi, y=emp_sketch_risk, color='darkred', label=r"sketching with ${m^{*}}$")
+            ax = sns.lineplot(x=phi, y=ridgeless_risk, label="no sketching")
+            ax = sns.lineplot(x=emp_phi, y=emp_sketch_risk, color='darkred')
+            ax = plt.scatter(x=emp_phi, y=emp_sketch_risk, color='darkred', label=r"sketching with ${m^{*}}$")
 
         markers = ['v', 'P', 's']
         colors = ["plum", "mediumvioletred", "mediumpurple"]
         for i, file in enumerate(files_emp_m):
             n_val = file.split('_')[-1].split('.')[0]
             alpha, sigma, emp_phi, emp_sketch_risk, phi, ridgeless_risk = load_files_cmp(file, correlated=True)
-            plt.scatter(x=emp_phi, y=emp_sketch_risk, alpha=0.8, color=colors[i], marker=markers[i], s=60, label=r"sketching with $\widehat{m}, n_{val}=$"+str(n_val))
-            sns.lineplot(x=emp_phi, y=emp_sketch_risk, color=colors[i])
+            ax = plt.scatter(x=emp_phi, y=emp_sketch_risk, color=colors[i], marker=markers[i], s=60, alpha=0.8, label=r"sketching with $\widehat{m}, n_{val}=$"+str(n_val))
+            ax = sns.lineplot(x=emp_phi, y=emp_sketch_risk, color=colors[i])
 
         ax.set(xticks = ticks, xticklabels = labels)
         ax.set_xlabel(r"$\phi$", fontsize=18)
         ax.set_ylim(-5, 100)
         ax.axvline(x=1, color="grey", linestyle='dashed', linewidth=1)
         ax.set_xlim(0.1, 10)
         ax.set_xscale('log')
```

### Comparing `SRLR-0.1.5/src/SRLR.egg-info/PKG-INFO` & `SRLR-0.1.6/src/SRLR.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SRLR
-Version: 0.1.5
+Version: 0.1.6
 Summary: A package for sketched ridgeless estimator simulations, optimizing generalization. Identify the best sketching size to minimize out-of-sample risks. Stable risk curves in optimally sketched estimator eliminate peaks found in full-sample estimator. SRLR offers practical method to discover the ideal sketching size.
 Home-page: https://github.com/statsle/SRLR_python
 Author: Siyue Yang
 Author-email: syue.yang@mail.utoronto.ca
 License: MIT
 Keywords: python,sketched ridgeless linear regression
 Platform: UNKNOWN
```

