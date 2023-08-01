# Comparing `tmp/SRLR-0.1.3.tar.gz` & `tmp/SRLR-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SRLR-0.1.3.tar", last modified: Tue Aug  1 19:25:08 2023, max compression
+gzip compressed data, was "SRLR-0.1.4.tar", last modified: Tue Aug  1 19:46:22 2023, max compression
```

## Comparing `SRLR-0.1.3.tar` & `SRLR-0.1.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 siyueyang   (501) staff       (20)        0 2023-08-01 19:25:08.100972 SRLR-0.1.3/
--rw-r--r--   0 siyueyang   (501) staff       (20)        0 2023-07-31 19:49:25.000000 SRLR-0.1.3/LICENSE
--rw-r--r--   0 siyueyang   (501) staff       (20)     2365 2023-08-01 19:25:08.100321 SRLR-0.1.3/PKG-INFO
--rw-r--r--   0 siyueyang   (501) staff       (20)     1513 2023-07-31 19:48:02.000000 SRLR-0.1.3/README.md
--rw-r--r--   0 siyueyang   (501) staff       (20)       38 2023-08-01 19:25:08.101138 SRLR-0.1.3/setup.cfg
--rw-r--r--   0 siyueyang   (501) staff       (20)     1587 2023-08-01 19:24:42.000000 SRLR-0.1.3/setup.py
-drwxr-xr-x   0 siyueyang   (501) staff       (20)        0 2023-08-01 19:25:08.091939 SRLR-0.1.3/src/
-drwxr-xr-x   0 siyueyang   (501) staff       (20)        0 2023-08-01 19:25:08.096492 SRLR-0.1.3/src/SRLR/
--rw-r--r--   0 siyueyang   (501) staff       (20)      148 2023-08-01 19:20:07.000000 SRLR-0.1.3/src/SRLR/__init__.py
--rw-r--r--   0 siyueyang   (501) staff       (20)     7269 2023-07-31 21:25:12.000000 SRLR-0.1.3/src/SRLR/asymptotics.py
--rw-r--r--   0 siyueyang   (501) staff       (20)     2649 2023-07-31 21:25:20.000000 SRLR-0.1.3/src/SRLR/datasets.py
--rw-r--r--   0 siyueyang   (501) staff       (20)     2527 2023-07-31 19:48:02.000000 SRLR-0.1.3/src/SRLR/estimators.py
--rw-r--r--   0 siyueyang   (501) staff       (20)      854 2023-07-31 19:48:02.000000 SRLR-0.1.3/src/SRLR/optimal_m.py
--rw-r--r--   0 siyueyang   (501) staff       (20)     6093 2023-07-31 19:48:02.000000 SRLR-0.1.3/src/SRLR/simulation.py
--rw-r--r--   0 siyueyang   (501) staff       (20)    12538 2023-08-01 19:24:33.000000 SRLR-0.1.3/src/SRLR/utils.py
-drwxr-xr-x   0 siyueyang   (501) staff       (20)        0 2023-08-01 19:25:08.099583 SRLR-0.1.3/src/SRLR.egg-info/
--rw-r--r--   0 siyueyang   (501) staff       (20)     2365 2023-08-01 19:25:08.000000 SRLR-0.1.3/src/SRLR.egg-info/PKG-INFO
--rw-r--r--   0 siyueyang   (501) staff       (20)      337 2023-08-01 19:25:08.000000 SRLR-0.1.3/src/SRLR.egg-info/SOURCES.txt
--rw-r--r--   0 siyueyang   (501) staff       (20)        1 2023-08-01 19:25:08.000000 SRLR-0.1.3/src/SRLR.egg-info/dependency_links.txt
--rw-r--r--   0 siyueyang   (501) staff       (20)       87 2023-08-01 19:25:08.000000 SRLR-0.1.3/src/SRLR.egg-info/requires.txt
--rw-r--r--   0 siyueyang   (501) staff       (20)        5 2023-08-01 19:25:08.000000 SRLR-0.1.3/src/SRLR.egg-info/top_level.txt
+drwxr-xr-x   0 siyueyang   (501) staff       (20)        0 2023-08-01 19:46:22.131602 SRLR-0.1.4/
+-rw-r--r--   0 siyueyang   (501) staff       (20)        0 2023-07-31 19:49:25.000000 SRLR-0.1.4/LICENSE
+-rw-r--r--   0 siyueyang   (501) staff       (20)     2365 2023-08-01 19:46:22.130967 SRLR-0.1.4/PKG-INFO
+-rw-r--r--   0 siyueyang   (501) staff       (20)     1513 2023-07-31 19:48:02.000000 SRLR-0.1.4/README.md
+-rw-r--r--   0 siyueyang   (501) staff       (20)       38 2023-08-01 19:46:22.131819 SRLR-0.1.4/setup.cfg
+-rw-r--r--   0 siyueyang   (501) staff       (20)     1587 2023-08-01 19:46:17.000000 SRLR-0.1.4/setup.py
+drwxr-xr-x   0 siyueyang   (501) staff       (20)        0 2023-08-01 19:46:22.121621 SRLR-0.1.4/src/
+drwxr-xr-x   0 siyueyang   (501) staff       (20)        0 2023-08-01 19:46:22.127611 SRLR-0.1.4/src/SRLR/
+-rw-r--r--   0 siyueyang   (501) staff       (20)      148 2023-08-01 19:20:07.000000 SRLR-0.1.4/src/SRLR/__init__.py
+-rw-r--r--   0 siyueyang   (501) staff       (20)     7269 2023-07-31 21:25:12.000000 SRLR-0.1.4/src/SRLR/asymptotics.py
+-rw-r--r--   0 siyueyang   (501) staff       (20)     2649 2023-07-31 21:25:20.000000 SRLR-0.1.4/src/SRLR/datasets.py
+-rw-r--r--   0 siyueyang   (501) staff       (20)     2527 2023-07-31 19:48:02.000000 SRLR-0.1.4/src/SRLR/estimators.py
+-rw-r--r--   0 siyueyang   (501) staff       (20)      854 2023-07-31 19:48:02.000000 SRLR-0.1.4/src/SRLR/optimal_m.py
+-rw-r--r--   0 siyueyang   (501) staff       (20)     6093 2023-07-31 19:48:02.000000 SRLR-0.1.4/src/SRLR/simulation.py
+-rw-r--r--   0 siyueyang   (501) staff       (20)    12510 2023-08-01 19:46:12.000000 SRLR-0.1.4/src/SRLR/utils.py
+drwxr-xr-x   0 siyueyang   (501) staff       (20)        0 2023-08-01 19:46:22.130104 SRLR-0.1.4/src/SRLR.egg-info/
+-rw-r--r--   0 siyueyang   (501) staff       (20)     2365 2023-08-01 19:46:22.000000 SRLR-0.1.4/src/SRLR.egg-info/PKG-INFO
+-rw-r--r--   0 siyueyang   (501) staff       (20)      337 2023-08-01 19:46:22.000000 SRLR-0.1.4/src/SRLR.egg-info/SOURCES.txt
+-rw-r--r--   0 siyueyang   (501) staff       (20)        1 2023-08-01 19:46:22.000000 SRLR-0.1.4/src/SRLR.egg-info/dependency_links.txt
+-rw-r--r--   0 siyueyang   (501) staff       (20)       87 2023-08-01 19:46:22.000000 SRLR-0.1.4/src/SRLR.egg-info/requires.txt
+-rw-r--r--   0 siyueyang   (501) staff       (20)        5 2023-08-01 19:46:22.000000 SRLR-0.1.4/src/SRLR.egg-info/top_level.txt
```

### Comparing `SRLR-0.1.3/PKG-INFO` & `SRLR-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SRLR
-Version: 0.1.3
+Version: 0.1.4
 Summary: A package for sketched ridgeless estimator simulations, optimizing generalization. Identify the best sketching size to minimize out-of-sample risks. Stable risk curves in optimally sketched estimator eliminate peaks found in full-sample estimator. SRLR offers practical method to discover the ideal sketching size.
 Home-page: https://github.com/statsle/SRLR_python
 Author: Siyue Yang
 Author-email: syue.yang@mail.utoronto.ca
 License: MIT
 Keywords: python,sketched ridgeless linear regression
 Platform: UNKNOWN
```

### Comparing `SRLR-0.1.3/README.md` & `SRLR-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `SRLR-0.1.3/setup.py` & `SRLR-0.1.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 # Package metadata
 NAME = 'SRLR'
-VERSION = '0.1.3'
+VERSION = '0.1.4'
 DESCRIPTION = 'A package for sketched ridgeless estimator simulations, optimizing generalization. Identify the best sketching size to minimize out-of-sample risks. Stable risk curves in optimally sketched estimator eliminate peaks found in full-sample estimator. SRLR offers practical method to discover the ideal sketching size.'
 AUTHOR = 'Siyue Yang'
 EMAIL = 'syue.yang@mail.utoronto.ca'
 URL = 'https://github.com/statsle/SRLR_python'
 LICENSE = 'MIT'
 PYTHON_REQUIRES = '>=3.6'
```

### Comparing `SRLR-0.1.3/src/SRLR/asymptotics.py` & `SRLR-0.1.4/src/SRLR/asymptotics.py`

 * *Files identical despite different names*

### Comparing `SRLR-0.1.3/src/SRLR/datasets.py` & `SRLR-0.1.4/src/SRLR/datasets.py`

 * *Files identical despite different names*

### Comparing `SRLR-0.1.3/src/SRLR/estimators.py` & `SRLR-0.1.4/src/SRLR/estimators.py`

 * *Files identical despite different names*

### Comparing `SRLR-0.1.3/src/SRLR/optimal_m.py` & `SRLR-0.1.4/src/SRLR/optimal_m.py`

 * *Files identical despite different names*

### Comparing `SRLR-0.1.3/src/SRLR/simulation.py` & `SRLR-0.1.4/src/SRLR/simulation.py`

 * *Files identical despite different names*

### Comparing `SRLR-0.1.3/src/SRLR/utils.py` & `SRLR-0.1.4/src/SRLR/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,15 +148,15 @@
     with plt.style.context(['science', 'no-latex', 'std-colors']):
         fig, ax = plt.subplots(1, 1, figsize=(6, 5))
         
         if fix_psi:
             markers = ['o', 'X', 'd']
             for i, file in enumerate(files):
                 snr, emp_psi, emp_risk, psi, risk = load_files(file, fix_psi)
-                ax = sns.scatterplot(x=emp_psi, y=emp_risk, marker=markers[i%len(markers)], s=60, label = "SNR = " + str(np.round(snr, 2)))
+                ax = plt.scatter(x=emp_psi, y=emp_risk, marker=markers[i%len(markers)], s=60, label = "SNR = " + str(np.round(snr, 2)))
                 ax = sns.lineplot(x=psi, y=risk)
 
             ax.set(xticks = ticks, xticklabels = labels)
             ax.set_xlabel(r"$\phi$", fontsize=18)
             ax.set_ylim(-10, 300)
             ax.set_xlim(0.1, 9.99)
             ax.set_xscale('log')
@@ -165,15 +165,15 @@
         else:
             for i, file in enumerate(files):
                 is_orthogonal = 'orthogonal' in file
                 label = 'orthogonal sketching' if is_orthogonal else 'i.i.d. sketching'
                 marker = 'o' if is_orthogonal else 'X'
 
                 snr, emp_psi, emp_risk, psi, risk = load_files(file, fix_psi)
-                ax = sns.scatterplot(x=emp_psi, y=emp_risk, marker=marker, s=60, label=label)
+                ax = plt.scatter(x=emp_psi, y=emp_risk, marker=marker, s=60, label=label)
                 ax = sns.lineplot(x=psi, y=risk)
 
             ax.set_xlabel(r"$\psi$", fontsize=18)
             ax.set_ylim(-50, 300)
             ax.set_xlim(0, 1)
             ax.axvline(x=0.5, color="grey", linestyle='dashed', linewidth=1)
             ax.invert_xaxis()
@@ -209,21 +209,21 @@
             if 'orthogonal' in file:
                 sketching_type = "orthogonal sketching"
             else:
                 sketching_type = "i.i.d. sketching"
         
             if correlated:
                 alpha, sigma, emp_phi, emp_sketch_risk, phi, ridgeless_risk = load_files_cmp(file, correlated)
-                ax = sns.scatterplot(x=emp_phi, y=emp_sketch_risk, color='darkred', s=60, label=sketching_type)
+                ax = plt.scatter(x=emp_phi, y=emp_sketch_risk, color='darkred', s=60, label=sketching_type)
                 ax = sns.lineplot(x=phi, y=ridgeless_risk, label="no sketching")
                 ax = sns.lineplot(x=emp_phi, y=emp_sketch_risk, color='darkred')
             else:
                 alpha, sigma, emp_phi, emp_sketch_risk, emp_ridgeless_risk, phi, sketch_risk, ridgeless_risk = load_files_cmp(file, correlated=correlated)
-                ax = sns.scatterplot(x=emp_phi, y=emp_ridgeless_risk, marker='X', s=60, label="no sketching", ax=ax)
-                ax = sns.scatterplot(x=emp_phi, y=emp_sketch_risk, color='darkred', s=60, label=sketching_type)
+                ax = plt.scatter(x=emp_phi, y=emp_ridgeless_risk, marker='X', s=60, label="no sketching", ax=ax)
+                ax = plt.scatter(x=emp_phi, y=emp_sketch_risk, color='darkred', s=60, label=sketching_type)
                 ax = sns.lineplot(x=phi, y=ridgeless_risk)
                 ax = sns.lineplot(x=phi, y=sketch_risk, color='darkred')
             
             if snr is not None:
                 if snr > 1: 
                     ax.axvline(x=1, color="grey", linestyle='dashed', linewidth=1)
                     ax.axvspan((1 - sigma/(2*alpha)), alpha/(alpha - sigma), facecolor='pink', alpha=0.3, **dict())
@@ -271,22 +271,22 @@
 
     with plt.style.context(['science', 'no-latex', 'std-colors']):
         fig, ax = plt.subplots(1, 1, figsize=(6, 5))
         for i, file in enumerate(files_base):
             alpha, sigma, emp_phi, emp_sketch_risk, phi, ridgeless_risk = load_files_cmp(file, correlated=True)
             ax = sns.lineplot(x=phi, y=ridgeless_risk, label="no sketching")
             ax = sns.lineplot(x=emp_phi, y=emp_sketch_risk, color='darkred')
-            ax = sns.scatterplot(x=emp_phi, y=emp_sketch_risk, color='darkred', label=r"sketching with ${m^{*}}$")
+            ax = plt.scatter(x=emp_phi, y=emp_sketch_risk, color='darkred', label=r"sketching with ${m^{*}}$")
 
         markers = ['v', 'P', 's']
         colors = ["plum", "mediumvioletred", "mediumpurple"]
         for i, file in enumerate(files_emp_m):
             n_val = file.split('_')[-1].split('.')[0]
             alpha, sigma, emp_phi, emp_sketch_risk, phi, ridgeless_risk = load_files_cmp(file, correlated=True)
-            ax = sns.scatterplot(x=emp_phi, y=emp_sketch_risk, color=colors[i], marker=markers[i], s=60, label=r"sketching with $\widehat{m}, n_{val}=$"+str(n_val))
+            ax = plt.scatter(x=emp_phi, y=emp_sketch_risk, color=colors[i], marker=markers[i], s=60, label=r"sketching with $\widehat{m}, n_{val}=$"+str(n_val))
             ax = sns.lineplot(x=emp_phi, y=emp_sketch_risk, color=colors[i])
 
         ax.set(xticks = ticks, xticklabels = labels)
         ax.set_xlabel(r"$\phi$", fontsize=18)
         ax.set_ylim(-5, 100)
         ax.axvline(x=1, color="grey", linestyle='dashed', linewidth=1)
         ax.set_xlim(0.1, 10)
```

### Comparing `SRLR-0.1.3/src/SRLR.egg-info/PKG-INFO` & `SRLR-0.1.4/src/SRLR.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SRLR
-Version: 0.1.3
+Version: 0.1.4
 Summary: A package for sketched ridgeless estimator simulations, optimizing generalization. Identify the best sketching size to minimize out-of-sample risks. Stable risk curves in optimally sketched estimator eliminate peaks found in full-sample estimator. SRLR offers practical method to discover the ideal sketching size.
 Home-page: https://github.com/statsle/SRLR_python
 Author: Siyue Yang
 Author-email: syue.yang@mail.utoronto.ca
 License: MIT
 Keywords: python,sketched ridgeless linear regression
 Platform: UNKNOWN
```

