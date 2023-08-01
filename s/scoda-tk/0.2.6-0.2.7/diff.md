# Comparing `tmp/scoda-tk-0.2.6.tar.gz` & `tmp/scoda-tk-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scoda-tk-0.2.6.tar", last modified: Tue Aug  1 08:51:42 2023, max compression
+gzip compressed data, was "scoda-tk-0.2.7.tar", last modified: Tue Aug  1 19:25:30 2023, max compression
```

## Comparing `scoda-tk-0.2.6.tar` & `scoda-tk-0.2.7.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-01 08:51:42.478350 scoda-tk-0.2.6/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-07-30 14:49:21.000000 scoda-tk-0.2.6/LICENSE
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      128 2023-07-30 14:49:22.000000 scoda-tk-0.2.6/MANIFEST.in
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-08-01 08:51:42.478350 scoda-tk-0.2.6/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-07-30 14:49:22.000000 scoda-tk-0.2.6/README.md
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      826 2023-08-01 08:51:26.000000 scoda-tk-0.2.6/pyproject.toml
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       38 2023-08-01 08:51:42.478350 scoda-tk-0.2.6/setup.cfg
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       49 2023-07-30 14:49:21.000000 scoda-tk-0.2.6/setup.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-01 08:51:42.458350 scoda-tk-0.2.6/src/
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-01 08:51:42.458350 scoda-tk-0.2.6/src/scoda/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-07-30 14:49:25.000000 scoda-tk-0.2.6/src/scoda/__init__.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    21388 2023-07-30 14:49:23.000000 scoda-tk-0.2.6/src/scoda/cpdb.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-01 08:51:42.478350 scoda-tk-0.2.6/src/scoda/default_optional_files/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      291 2023-07-30 14:49:23.000000 scoda-tk-0.2.6/src/scoda/default_optional_files/analysis_config.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)   110525 2023-07-30 14:49:24.000000 scoda-tk-0.2.6/src/scoda/default_optional_files/cpdb.zip
--rw-rw-r--   0 syoon     (1001) syoon     (1001)  9812023 2023-07-30 14:49:24.000000 scoda-tk-0.2.6/src/scoda/default_optional_files/hg38_gene_only.gtf
--rw-rw-r--   0 syoon     (1001) syoon     (1001)     9771 2023-07-30 14:49:23.000000 scoda-tk-0.2.6/src/scoda/default_optional_files/markers_hs.tsv
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    10054 2023-07-30 14:49:23.000000 scoda-tk-0.2.6/src/scoda/default_optional_files/markers_mm.tsv
--rw-rw-r--   0 syoon     (1001) syoon     (1001)  6641898 2023-07-30 14:49:25.000000 scoda-tk-0.2.6/src/scoda/default_optional_files/mm10_gene_only.gtf
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    98551 2023-07-30 14:49:23.000000 scoda-tk-0.2.6/src/scoda/default_optional_files/msig.gmt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    17850 2023-07-30 14:49:25.000000 scoda-tk-0.2.6/src/scoda/deg.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    13716 2023-07-30 14:49:22.000000 scoda-tk-0.2.6/src/scoda/gsea.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)   157974 2023-07-30 14:49:22.000000 scoda-tk-0.2.6/src/scoda/hicat.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    29743 2023-08-01 08:51:14.000000 scoda-tk-0.2.6/src/scoda/icnv.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    31368 2023-07-30 14:49:25.000000 scoda-tk-0.2.6/src/scoda/misc.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    23316 2023-08-01 08:46:07.000000 scoda-tk-0.2.6/src/scoda/pipeline.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    58085 2023-07-31 13:01:13.000000 scoda-tk-0.2.6/src/scoda/viz.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-01 08:51:42.478350 scoda-tk-0.2.6/src/scoda_tk.egg-info/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-08-01 08:51:42.000000 scoda-tk-0.2.6/src/scoda_tk.egg-info/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      776 2023-08-01 08:51:42.000000 scoda-tk-0.2.6/src/scoda_tk.egg-info/SOURCES.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-08-01 08:51:42.000000 scoda-tk-0.2.6/src/scoda_tk.egg-info/dependency_links.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       52 2023-08-01 08:51:42.000000 scoda-tk-0.2.6/src/scoda_tk.egg-info/entry_points.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       54 2023-08-01 08:51:42.000000 scoda-tk-0.2.6/src/scoda_tk.egg-info/requires.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        6 2023-08-01 08:51:42.000000 scoda-tk-0.2.6/src/scoda_tk.egg-info/top_level.txt
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-01 19:25:30.005855 scoda-tk-0.2.7/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-07-30 14:49:21.000000 scoda-tk-0.2.7/LICENSE
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      128 2023-07-30 14:49:22.000000 scoda-tk-0.2.7/MANIFEST.in
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-08-01 19:25:30.005855 scoda-tk-0.2.7/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-07-30 14:49:22.000000 scoda-tk-0.2.7/README.md
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      826 2023-08-01 19:23:26.000000 scoda-tk-0.2.7/pyproject.toml
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       38 2023-08-01 19:25:30.005855 scoda-tk-0.2.7/setup.cfg
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       49 2023-07-30 14:49:21.000000 scoda-tk-0.2.7/setup.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-01 19:25:29.901858 scoda-tk-0.2.7/src/
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-01 19:25:29.901858 scoda-tk-0.2.7/src/scoda/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-07-30 14:49:25.000000 scoda-tk-0.2.7/src/scoda/__init__.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    21388 2023-07-30 14:49:23.000000 scoda-tk-0.2.7/src/scoda/cpdb.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-01 19:25:30.001856 scoda-tk-0.2.7/src/scoda/default_optional_files/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      291 2023-07-30 14:49:23.000000 scoda-tk-0.2.7/src/scoda/default_optional_files/analysis_config.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)   110525 2023-07-30 14:49:24.000000 scoda-tk-0.2.7/src/scoda/default_optional_files/cpdb.zip
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)  9812023 2023-07-30 14:49:24.000000 scoda-tk-0.2.7/src/scoda/default_optional_files/hg38_gene_only.gtf
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)     9771 2023-07-30 14:49:23.000000 scoda-tk-0.2.7/src/scoda/default_optional_files/markers_hs.tsv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    10054 2023-07-30 14:49:23.000000 scoda-tk-0.2.7/src/scoda/default_optional_files/markers_mm.tsv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)  6641898 2023-07-30 14:49:25.000000 scoda-tk-0.2.7/src/scoda/default_optional_files/mm10_gene_only.gtf
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    98551 2023-07-30 14:49:23.000000 scoda-tk-0.2.7/src/scoda/default_optional_files/msig.gmt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    17850 2023-07-30 14:49:25.000000 scoda-tk-0.2.7/src/scoda/deg.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    13716 2023-07-30 14:49:22.000000 scoda-tk-0.2.7/src/scoda/gsea.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)   157974 2023-07-30 14:49:22.000000 scoda-tk-0.2.7/src/scoda/hicat.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    33929 2023-08-01 19:07:26.000000 scoda-tk-0.2.7/src/scoda/icnv.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    31368 2023-07-30 14:49:25.000000 scoda-tk-0.2.7/src/scoda/misc.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    23411 2023-08-01 19:22:11.000000 scoda-tk-0.2.7/src/scoda/pipeline.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    58085 2023-07-31 13:01:13.000000 scoda-tk-0.2.7/src/scoda/viz.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-01 19:25:30.005855 scoda-tk-0.2.7/src/scoda_tk.egg-info/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-08-01 19:25:29.000000 scoda-tk-0.2.7/src/scoda_tk.egg-info/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      776 2023-08-01 19:25:29.000000 scoda-tk-0.2.7/src/scoda_tk.egg-info/SOURCES.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-08-01 19:25:29.000000 scoda-tk-0.2.7/src/scoda_tk.egg-info/dependency_links.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       52 2023-08-01 19:25:29.000000 scoda-tk-0.2.7/src/scoda_tk.egg-info/entry_points.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       54 2023-08-01 19:25:29.000000 scoda-tk-0.2.7/src/scoda_tk.egg-info/requires.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        6 2023-08-01 19:25:29.000000 scoda-tk-0.2.7/src/scoda_tk.egg-info/top_level.txt
```

### Comparing `scoda-tk-0.2.6/LICENSE` & `scoda-tk-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.6/PKG-INFO` & `scoda-tk-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoda-tk
-Version: 0.2.6
+Version: 0.2.7
 Summary: Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Author-email: Seokhyun Yoon <syoon@dku.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `scoda-tk-0.2.6/pyproject.toml` & `scoda-tk-0.2.7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "scoda-tk"
-version = "0.2.6"
+version = "0.2.7"
 description = "Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)"
 readme = "README.md"
 authors = [{ name = "Seokhyun Yoon", email = "syoon@dku.edu" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `scoda-tk-0.2.6/src/scoda/cpdb.py` & `scoda-tk-0.2.7/src/scoda/cpdb.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.6/src/scoda/default_optional_files/cpdb.zip` & `scoda-tk-0.2.7/src/scoda/default_optional_files/cpdb.zip`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.6/src/scoda/default_optional_files/hg38_gene_only.gtf` & `scoda-tk-0.2.7/src/scoda/default_optional_files/hg38_gene_only.gtf`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.6/src/scoda/default_optional_files/markers_hs.tsv` & `scoda-tk-0.2.7/src/scoda/default_optional_files/markers_hs.tsv`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.6/src/scoda/default_optional_files/markers_mm.tsv` & `scoda-tk-0.2.7/src/scoda/default_optional_files/markers_mm.tsv`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.6/src/scoda/default_optional_files/mm10_gene_only.gtf` & `scoda-tk-0.2.7/src/scoda/default_optional_files/mm10_gene_only.gtf`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.6/src/scoda/default_optional_files/msig.gmt` & `scoda-tk-0.2.7/src/scoda/default_optional_files/msig.gmt`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.6/src/scoda/deg.py` & `scoda-tk-0.2.7/src/scoda/deg.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.6/src/scoda/gsea.py` & `scoda-tk-0.2.7/src/scoda/gsea.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.6/src/scoda/hicat.py` & `scoda-tk-0.2.7/src/scoda/hicat.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.6/src/scoda/icnv.py` & `scoda-tk-0.2.7/src/scoda/icnv.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import warnings, math, time, copy
+    import warnings, math, time, copy
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 from sklearn import cluster, mixture
 from sklearn.neighbors import kneighbors_graph
 from sknetwork.clustering import Louvain
 from sklearn.decomposition import PCA, IncrementalPCA, TruncatedSVD
@@ -157,15 +157,15 @@
     cnt = 1
     for c in idx_lst:
         b = obs[cluster_key] == c
         b1 = dec == 'Tumor'
         if np.sum(b&b1) > 0:
             tclust[b&b1] = 'Tumor_c%i' % cnt
             cnt += 1        
-    obs['tumor_cluster'+ suffix] = tclust
+    # obs['tumor_cluster'+ suffix] = tclust
 
     ss_div_dm = (np.sqrt(v1)+np.sqrt(v0))/(m1-m0)
     if ss_div_dm > 1:
         print('INFO: Std_sum/Mean_diff: %f > 1' % (ss_div_dm))
         print('INFO: indicating that no tumor cells might be present in this sample.' % (ss_div_dm))
     
     params = {}
@@ -199,28 +199,28 @@
     df = obs.groupby([cluster_key])[score_key].agg(**{'cmean':'mean'})
     idx_lst = list(df.index.values)
     
     ns = 0
     # while(ns == 0):
         
     b_inc = []
-    df['Ref_percent'] = 0
+    df['ref_frac'] = 0
     for idx in idx_lst:
         b = obs[cluster_key] == idx
         # cts = obs.loc[b, ref_key]
         '''
         ct_vc = cts.value_counts()
         cnt = 0
         for ct in list(ct_vc.index.values):
             if ct in ref_types:
                 cnt += ct_vc[ct]
         '''
         cnt = np.sum(np.array(ref_ind)[b])
         ref_percent = cnt/np.sum(b)
-        df.loc[idx, 'Ref_percent'] = ref_percent
+        df.loc[idx, 'ref_frac'] = ref_percent
         if (ref_percent >= refp_min):
             b_inc.append(True)
         else:
             b_inc.append(False)
 
     df['b_inc'] = b_inc
     b = np.array(b_inc)
@@ -228,15 +228,15 @@
 
     ns = np.sum(b)
     # if ns == 0: refp_min *= 0.95
     if ns == 0:
         print('ERROR: no reference type clusters found.')
         obs['tumor_prob'+ suffix] = 0
         obs['tumor_dec'+ suffix] = 'NA'
-        obs['tumor_cluster'+ suffix] = ''
+        # obs['tumor_cluster'+ suffix] = ''
         return None
     elif ns == 1:
         print('WARNING: Only one reference type cluster found.')
         cmeans = np.array(df.loc[b,'cmean'])
         th2 = cmeans[0]
         b2 = df['cmean'] <= th2
     else:        
@@ -320,15 +320,15 @@
     for k in range(len(xs0)):
         if (pdf1[k] >= pdf0[k]) & (xs0[k] > m0):
             th = xs0[k]
             break
             
     ss_div_dm = (np.sqrt(v1)+np.sqrt(v0))/(m1-m0)
     if ss_div_dm > 1:
-        print('INFO: Std_sum/Mean_diff: %f > 1' % (ss_div_dm))
+        print('\nINFO: Std_sum/Mean_diff: %f > 1' % (ss_div_dm))
         print('INFO: indicating that no tumor cells might be present in this sample.' % (ss_div_dm))
         # th = m0 + np.sqrt(v0)
         
     # print('threshold: ', th )
     th = max(th, th_min)
             
     s = obs[score_key]
@@ -385,15 +385,15 @@
     ut = th + (m1 - th)*p_exc
     b = (s > lt) & (s < ut) & (~br)
     print(lt, ut, np.sum(~br), np.sum(b))
     dec[b] = 'unclear'
     #'''
     if ss_div_dm > 1:
         b = dec == 'Tumor'
-        print('INFO: %i among %i were identified as tumor cells, which, however, might be normal cells.' \
+        print('INFO: %i among %i were identified as tumor cells.' \
               % (np.sum(b), len(b)))
     
     # b = (obs[ref_key].isin(ref_types)) | (s <= th)
     # dec[b] = 'Normal'    
     obs['tumor_dec'+ suffix] = dec
 
     tclust = dec.copy(deep = True)
@@ -401,15 +401,15 @@
     cnt = 1
     for c in idx_lst:
         b = obs[cluster_key] == c
         b1 = dec == 'Tumor'
         if np.sum(b&b1) > 0:
             tclust[b&b1] = 'Tumor_c%i' % cnt
             cnt += 1        
-    obs['tumor_cluster'+ suffix] = tclust
+    # obs['tumor_cluster'+ suffix] = tclust
     
     etime = round(time.time() - start_time) 
     # print('CNVth(%i) ' % etime, end = '', flush = True)
     
     params = {}
     params['th'] = th
     params['m0'] = m0
@@ -422,15 +422,16 @@
     
     if plot_stat:
         plot_stats( params, n_bins = 30, title = None, title_fs = 14,
                     label_fs = 12, tick_fs = 11, legend_fs = 11, 
                     legend_loc = 'upper left', bbox_to_anchor = (1, 1),
                     figsize = (4,3), log = False, alpha = 0.8 )
         
-    return obs[['tumor_dec'+ suffix, 'tumor_prob'+ suffix, 'tumor_cluster'+ suffix]], params
+    return obs[['tumor_dec'+ suffix, 'tumor_prob'+ suffix]], params
+    # return obs[['tumor_dec'+ suffix, 'tumor_prob'+ suffix, 'tumor_cluster'+ suffix]], params
 
 
 def initially_detect_major_clusters( X_pca, y_clust, cobj, pmaj = 0.7, 
                              cutoff = 0.01, verbose = False ):
     
     adj_agg = cobj.aggregate_
     adj_agg_mat = adj_agg.todense().astype(int) 
@@ -511,15 +512,15 @@
     
     ss = np.array(ss)
     odr = ss.argsort()
     
     return cm[odr[0]]
 
 
-def extend_major_clusters(adj_agg_mat, seed_clusters):
+def extend_major_clusters_old(adj_agg_mat, seed_clusters):
 
     adj_agg_mat = adj_agg_mat - np.diag(np.diag(adj_agg_mat))
 
     for a in range(adj_agg_mat.shape[0] - len(seed_clusters)):
         # def get_pv( s, adj_agg_mat, seed_clusters ):
         mn = adj_agg_mat[seed_clusters, :].mean(axis = 0)
         sd = adj_agg_mat[seed_clusters, :].std(axis = 0)
@@ -568,14 +569,86 @@
             # print(th, mx_pv, seed_clusters)
         else:
             break
             
     return seed_clusters
 
 
+def extend_major_clusters( adj_agg_mat, seed_clusters, 
+                           cluster_size, alpha = 1, 
+                           pv_cutoff = None, verbose = False ):
+
+    maj_clusters = copy.deepcopy(seed_clusters)
+    selected_clusters = copy.deepcopy(maj_clusters)
+    
+    adj_agg_mat = np.array(adj_agg_mat)
+    adj_agg_mat = adj_agg_mat - np.diag(np.diag(adj_agg_mat))
+    adj_agg_mat = adj_agg_mat + adj_agg_mat.transpose()
+    
+    flag = True
+    for a in range(adj_agg_mat.shape[0] - len(seed_clusters)):
+        
+        core_mat = adj_agg_mat[maj_clusters, :][:,maj_clusters]
+        core_mxs = core_mat.max(axis = 1)
+        
+        # odr = (-core_mxs).argsort()
+        # core_mxs = core_mxs[odr]
+        # maj_clusters = list(np.array(maj_clusters)[odr])
+        
+        core_dm = np.mean(core_mxs)
+        core_ds = np.std(core_mxs)
+        
+        dvs = []
+        nodes = []
+        pair = []
+        for n in range(adj_agg_mat.shape[0]):
+
+            if n not in maj_clusters:
+                cnt_n = adj_agg_mat[maj_clusters,n]
+                odr = np.array(cnt_n).argsort()
+                nodes.append(n)
+                p = maj_clusters[int(odr[-1])]
+                pair.append(p)
+                dvs.append(adj_agg_mat[p,n])
+                    
+        if len(dvs) == 1:
+            md = dvs[0]
+            cn = nodes[0]
+        else:
+            odr = np.array(dvs).argsort()
+
+            md = dvs[odr[-1]]
+            cn = nodes[odr[-1]]
+            pp = pair[odr[-1]]
+
+        if alpha is not None:
+            condition = md >= cluster_size[cn]*alpha
+        else:
+            st = np.abs(core_dm - md)/(core_ds)
+            pv = stats.t.sf(st*np.sqrt(2), df = 1)*2
+            condition = pv >= pv_cutoff
+            
+        if flag & condition:
+            maj_clusters.append(cn)
+            selected_clusters = copy.deepcopy(maj_clusters)
+            if verbose: print(cn, pp, md, cluster_size[cn]) 
+        else:
+            flag = False
+            if verbose: print(cn, pp, md, cluster_size[cn]) 
+            # break
+            maj_clusters.append(cn)
+            pass
+                    
+    core_mat = adj_agg_mat[maj_clusters, :][:,maj_clusters]
+    core_mxs = core_mat.max(axis = 1)
+    
+    return np.array(selected_clusters), np.array(maj_clusters), core_mxs
+
+
+
 import warnings
 
 def run_icnv(adata, ref_key, ref_types, gtf_file, cluster_key = 'cnv_leiden', 
              resolution = 2, N_pca = 15, n_neighbors = 10, umap = True, pca = True, n_cores = 4 ):
     
     pca_umap = umap
     with warnings.catch_warnings():
@@ -620,39 +693,41 @@
 from sklearn.neighbors import NearestNeighbors
 
 CLUSTERING_AGO = 'lv'
 SKNETWORK = True
 try:
     from sknetwork.clustering import Louvain
 except ImportError:
-    print('WARNING: sknetwork not installed. Will used GMM for clustering.')
-    CLUSTERING_AGO = 'gmm'
+    print('ERROR: sknetwork not installed.')
     SKNETWORK = False
 
     
 def clustering_alg(X_pca, clust_algo = 'lv', N_clusters = 25, resolution = 1, N_neighbors = 10, 
-                   mode='distance', n_cores = 4):
+                   mode='connectivity', n_cores = 4):
+                   # mode='distance', n_cores = 4):
     
+    adj = None
     if clust_algo[:2] == 'gm':
         gmm = mixture.GaussianMixture(n_components = int(N_clusters), random_state = 0)
         cluster_label = gmm.fit_predict(np.array(X_pca))
-        return cluster_label, gmm
+        return cluster_label, gmm, adj
     elif clust_algo[:2] == 'km':
         km = cluster.KMeans(n_clusters = int(N_clusters), random_state = 0)
         km.fit(X_pca)
         cluster_label = km.labels_
-        return cluster_label, km
+        return cluster_label, km, adj
     else:
-        adj = kneighbors_graph(X_pca, int(N_neighbors), mode=mode, include_self=True, n_jobs = n_cores)
+        adj = kneighbors_graph(X_pca, int(N_neighbors), mode=mode, include_self=True, 
+                               n_jobs = n_cores)
         louvain = Louvain(resolution = resolution)
         if hasattr(louvain, 'fit_predict'):
             cluster_label = louvain.fit_predict(adj)        
         else:
             cluster_label = louvain.fit_transform(adj)        
-        return cluster_label, louvain
+        return cluster_label, louvain, adj
     '''
     elif clust_algo[:2] == 'ld':
         leiden = LeidenClustering()
         leiden.fit(X)
         cluster_label = leiden.labels_
         return cluster_label, km
     '''
@@ -664,28 +739,28 @@
     df = obs.groupby([cluster_key])[score_key].agg(**{'cmean':'mean'})
     idx_lst = list(df.index.values)
     
     ns = 0
     # while(ns == 0):
         
     b_inc = []
-    df['Ref_percent'] = 0
+    df['ref_frac'] = 0
     for idx in idx_lst:
         b = obs[cluster_key] == idx
         # cts = obs.loc[b, ref_key]
         '''
         ct_vc = cts.value_counts()
         cnt = 0
         for ct in list(ct_vc.index.values):
             if ct in ref_types:
                 cnt += ct_vc[ct]
         '''
         cnt = np.sum(np.array(ref_ind)[b])
         ref_percent = cnt/np.sum(b)
-        df.loc[idx, 'Ref_percent'] = ref_percent
+        df.loc[idx, 'ref_frac'] = ref_percent
         if (ref_percent >= refp_min):
             b_inc.append(True)
         else:
             b_inc.append(False)
 
     df['b_inc'] = b_inc
     b = np.array(b_inc)
@@ -695,21 +770,21 @@
 
 def identify_tumor_cells(X_cnv, ref_ind, pca = False, use_cnv_score = False, 
                        clust = None, Clustering_resolution = 1, N_clusters = 30,
                        # cluster_key = 'cnv_leiden', score_key = 'tumor_score', 
                        gmm_N_comp = 20, th_min = 0, refp_min = 0.9, p_exc = 0.1, 
                        dec_margin = 0.05, n_neighbors = 10, cmd_cutoff = 0.03, 
                        gcm = 0.05, plot_stat = False, use_ref = False, 
-                       n_cores = 4, suffix = '', Data = None):
+                       n_cores = 4, cd_alpha = 1, suffix = '', Data = None):
     
     ## Remove all zero X_cnv
     X_cnv_mean = np.array(X_cnv.sum(axis = 1))
     b = X_cnv_mean == 0
     if np.sum(b) > 0:
-        print(np.sum(b))
+        # print(np.sum(b))
         odr = np.array(X_cnv_mean).argsort()
         o_min = odr[int(np.sum(b))]
         x_cnv = X_cnv[o_min,:]
         idxs = np.arange(X_cnv.shape[0])[list(b)]
         for i in idxs:
             X_cnv[i,:] = x_cnv
             
@@ -737,31 +812,35 @@
         
         etime = round(time.time() - start_time) 
         print('P(%i) .. ' % etime, end = '', flush = True)
         start_time = time.time()           
     else: 
         X_pca = np.array(X_cnv.copy(deep = True)) #.copy(deep = True)
             
-    y_clust, cobj = clustering_alg(X_pca, clust_algo = CLUSTERING_AGO, N_clusters = N_clusters, 
+    y_clust, cobj, adj = clustering_alg(X_pca, clust_algo = CLUSTERING_AGO, N_clusters = N_clusters, 
                                    resolution = Clustering_resolution, N_neighbors = n_neighbors, 
                                    n_cores = n_cores)
-        
+
+    if adj is None:
+        adj = kneighbors_graph(X_pca, int(n_neighbors), mode = 'connectivity', 
+                               include_self=True, n_jobs = n_cores)
+    
     etime = round(time.time() - start_time) 
     print('C(%i) .. ' % etime, end = '', flush = True)
     start_time = time.time()
     
     cnv_clust_lst = list(set(y_clust))
+    cnv_clust_lst.sort()
     df[cluster_key] = y_clust
         
     cluster_sel = None
     
     if ref_ind is not None: # use_ref:
         b = ref_ind
         #'''
-        cnv_clust_lst.sort()
         b_inc = []
         for idx in cnv_clust_lst:
             b = y_clust == idx
             bt = b & ref_ind
             cnt = np.sum(bt)
 
             if (cnt >= refp_min*np.sum(b)):
@@ -772,27 +851,44 @@
         if np.sum(b_inc) > 0:
             cluster_sel = list(np.array(cnv_clust_lst)[b_inc]) 
         else:
             print('ERROR: No reference cell types found.')
             df[score_key] = 0
             df['tumor_prob'+ suffix] = 0
             df['tumor_dec'+ suffix] = 'NA'
-            df['tumor_cluster'+ suffix] = ''
+            # df['tumor_cluster'+ suffix] = ''
             return df[[cluster_key, score_key, 'tumor_dec'+suffix, 
-                      'tumor_prob'+suffix, 'tumor_cluster'+ suffix]]
+                      'tumor_prob'+suffix]]
+            # return df[[cluster_key, score_key, 'tumor_dec'+suffix, 
+            #           'tumor_prob'+suffix, 'tumor_cluster'+ suffix]]
         #'''
     else:
         cluster_sel = initially_detect_major_clusters(X_pca, y_clust, cobj, pmaj = 0.7, 
                          cutoff = cmd_cutoff, verbose = False )        
 
-    adj_agg = cobj.aggregate_
-    adj_agg_mat = np.array(adj_agg.todense().astype(int)) 
-    adj_agg_mat = adj_agg_mat - np.diag(np.diag(adj_agg_mat))
-
-    cluster_sel = extend_major_clusters(adj_agg_mat, cluster_sel)
+    if CLUSTERING_AGO == 'lv':
+        adj_agg = cobj.aggregate_
+        adj_agg_mat = np.array(adj_agg.todense().astype(int)) 
+    else:
+        rows = adj.tocoo().row
+        cols = adj.tocoo().col
+        vals = adj.data
+
+        adj_agg_mat = np.zeros([len(cnv_clust_lst), len(cnv_clust_lst)], dtype = int)
+        for r, c, v in zip(rows, cols, vals):
+            adj_agg_mat[y_clust[r],y_clust[c]] += 1
+
+    cluster_size = [] 
+    for c in cnv_clust_lst:
+        b = y_clust == c
+        cluster_size.append(np.sum(b))
+    
+    cluster_sel, cluster_odr, strength_odr = extend_major_clusters(adj_agg_mat, 
+                                               cluster_sel, cluster_size, 
+                                               alpha = cd_alpha, pv_cutoff = None)
     
     b = y_clust == cluster_sel[0]
     if len(cluster_sel) > 1:
         for c in cluster_sel[1:]:
             b = b | (y_clust == c)
     ref_ind2 = b
     
@@ -826,24 +922,46 @@
     df.loc[b, score_key] = mnv
     #'''
     
     etime = round(time.time() - start_time) 
     print('G(%i) .. ' % etime, end = '', flush = True)
     start_time = time.time()
     
-    dft, params = get_cnv_threshold_useref( df, ref_ind2, 
+    dft, td_params = get_cnv_threshold_useref( df, ref_ind2, 
                                        score_key = score_key, cluster_key = cluster_key,
                                        th_min = th_min, refp_min = refp_min, p_exc = p_exc, 
                                        ucr = dec_margin, plot_stat = plot_stat, 
                                        suffix = suffix, Data = Data )
     
+    results = {}
+    results['tumor_dec_params'] = td_params
+    results['adj_mat'] = adj
+    results['agg_adj_mat'] = adj_agg_mat
+    # results['cluster_sizes'] = cluster_size
+    # results['normal_clusters'] = cluster_sel
+    # results['cluster_selection_order'] = cluster_odr
+    # results['connection_strengths'] = strength_odr
+    results['alpha_for_cluster_discovery'] = cd_alpha
+    
+    df_res = td_params['df']
+    # df_res['Normal'] = False
+    # for c in cluster_sel: df_res.loc[c, 'Normal'] = True
+    df_res['cluster_size'] = cluster_size
+    df_res['selection_order'] = 0
+    for j, (c, v) in enumerate(zip(cluster_odr, strength_odr)): 
+        df_res.loc[c, 'selection_order'] = j
+        df_res.loc[c, 'edge_wgt'] = v
+    df_res.rename(columns = {'dec': 'tumor_dec'}, inplace = True)
+    df_res.drop(columns = 'b_inc', inplace = True)
+    results['cnv_cluster_info'] = df_res    
+    
     etime = round(time.time() - start_time_a) 
     print('done (%i) ' % etime) #, end = '', flush = True)
     
-    return df, params, cobj, X_pca
+    return df, results, cobj, X_pca
 
 
 def plot_td_stats( params, n_bins = 30, title = None, title_fs = 14,
                    label_fs = 12, tick_fs = 11, legend_fs = 11, 
                    legend_loc = 'upper left', bbox_to_anchor = (1, 1),
                    figsize = (4,3), log = True, alpha = 0.8 ):
     
@@ -879,25 +997,25 @@
     
     counts, bins = np.histogram(df['cmean'], bins = n_bins)
     # max_cnt = np.max(counts)
 
     legend_labels = []
     
     max_cnt = 0
-    b = df['dec'] == 'Normal'
+    b = df['tumor_dec'] == 'Normal'
     if np.sum(b) > 0:
         legend_labels.append('Normal')
         counts, bins_t, bar_t = plt.hist(df.loc[b, 'cmean'], bins = bins, alpha = alpha)
         max_cnt = max(max_cnt, np.max(counts))
-    b = df['dec'] == 'Tumor'
+    b = df['tumor_dec'] == 'Tumor'
     if np.sum(b) > 0:
         legend_labels.append('Tumor')
         counts, bins_t, bar_t = plt.hist(df.loc[b, 'cmean'], bins = bins, alpha = alpha)
         max_cnt = max(max_cnt, np.max(counts))
-    b = df['dec'] == 'unclear'
+    b = df['tumor_dec'] == 'unclear'
     if np.sum(b) > 0:
         legend_labels.append('unclear')
         counts, bins_t, bar_t = plt.hist(df.loc[b, 'cmean'], bins = bins, alpha = alpha)
         max_cnt = max(max_cnt, np.max(counts))
     
     sf = 0.9*max_cnt/max_pdf
     plt.plot(xs0, pdf0*sf)
```

### Comparing `scoda-tk-0.2.6/src/scoda/misc.py` & `scoda-tk-0.2.7/src/scoda/misc.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.6/src/scoda/pipeline.py` & `scoda-tk-0.2.7/src/scoda/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,76 +82,77 @@
     
     return # adata
 
 
 def scoda_icnv_addon( adata_t, gtf_file, ref_types = None, 
                       ref_key = "celltype_major", n_cores = 4,
                       use_ref_only = False, cmd_cutoff = 0.03, 
-                      gcm = 0.05, tumor_dec_margin = 0.05 ):
+                      gcm = 0.05, tumor_dec_margin = 0.05, cd_alpha = 1 ):
     
     adata = adata_t[:,:]
 
     ref_types2 = ref_types
     ref_ind = None
 
     if ref_types is not None:
         if isinstance(ref_types, list):
             if len(ref_types) > 0:
                 ref_types2 = list(set(ref_types).intersection(adata.obs[ref_key].unique()))
                 ref_ind = adata.obs[ref_key].isin(ref_types)
-    #'''
+    '''
     adata = run_icnv(adata, ref_key, ref_types2, gtf_file, 
                      resolution = 2, N_pca = 15, n_neighbors = 10,
                      cluster_key = 'cnv_leiden', umap = False, pca = False,
                      n_cores = n_cores )
 
     #'''
     X_cnv = np.array(adata.obsm['X_cnv'].todense())
     pca = False
 
     # X_cnv = adata.obsm['X_cnv_pca']
     # pca = True
 
-    df_res, params, cobj, X_pca = identify_tumor_cells(X_cnv, ref_ind, pca = pca, 
+    df_res, results, cobj, X_pca = identify_tumor_cells(X_cnv, ref_ind, pca = pca, 
                            use_cnv_score = False, clust = None, 
                            Clustering_resolution = 1, N_clusters = 30,
                            gmm_N_comp = 20, th_min = 0, refp_min = 0.9, p_exc = 0.1, 
                            dec_margin = tumor_dec_margin, n_neighbors = 15, cmd_cutoff = cmd_cutoff, 
                            gcm = gcm, plot_stat = False, use_ref = use_ref_only, 
-                           suffix = '', Data = None, n_cores = n_cores)
+                           cd_alpha = cd_alpha, suffix = '', Data = None, n_cores = n_cores)
 
     if not pca: adata.obsm['X_cnv_pca'] = X_pca
         
     adata_t.obsm['X_cnv'] = adata.obsm['X_cnv']
     adata_t.obsm['X_cnv_pca'] = adata.obsm['X_cnv_pca']
 
     # adata_t.obsm['X_cnv_umap'] = adata.obsm['X_cnv_umap']
     # adata_t.obs['cnv_leiden'] = adata.obs['cnv_leiden']
     # adata_t.obs['cnv_score'] = adata.obs['cnv_score']
     # adata_t.uns['cnv_neighbors'] = adata.uns['cnv_neighbors']
     # adata_t.uns['log1p'] = adata.uns['log1p']
     # adata_t.uns['hvg'] = adata.uns['hvg']
     # adata_t.uns['leiden'] = adata.uns['leiden']
     adata_t.uns['cnv'] = adata.uns['cnv']
-    adata_t.obsp = adata.obsp
+    # adata_t.obsp = adata.obsp
 
     adata_t.obs['cnv_cluster'] = list(df_res['cnv_cluster'].astype(str))
     adata_t.obs['tumor_dec'] = list(df_res['tumor_dec'])
     adata_t.obs['tumor_score'] = list(df_res['tumor_score'])
 
     adata_t.uns['cnv_ref_celltypes'] = ref_types2
     # adata_t.uns['cnv_clustering_obj'] = cobj
-    adata_t.uns['cnv_stats'] = params
+    adata_t.uns['cnv_addon_summary'] = results
+    # adata_t.uns['cnv_adj_mat'] = adj
 
     lst1 = list(df_res.index.values)
     lst2 = list(adata_t.obs.index.values)
     rend = dict(zip(lst1, lst2))
     df_res.rename(index = rend, inplace = True)
 
-    adata_t.obsm['cnv_results'] = df_res[df_res.columns.values[:-1]] ## except tumor_cluster
+    adata_t.obsm['cnv_addon_summary'] = df_res ## except tumor_cluster
 
     adata_t.obs['celltype_minor_rev'] = adata_t.obs['celltype_minor'].copy(deep = True).astype(str)
     b = (adata_t.obs['tumor_dec'] == 'Tumor')
     if ref_types is not None:
         b = b & (~adata_t.obs['celltype_major'].isin(ref_types))
     adata_t.obs.loc[b, 'celltype_minor_rev'] = 'Tumor cell'
 
@@ -489,15 +490,15 @@
     
     return
 
 
 def scoda_all_in_one( adata_t, mkr_db, cpdb_path, gsea_pw_db, cnv_gtf = None, 
                       cond_col = 'condition', sample_col = 'sample', 
                       cnv_ref_list = None, cnv_cmd_cutoff = 0.03, cnv_use_ref_only = False,
-                      cnv_gcm = 0.05, cnv_tdec_margin = 0.05, 
+                      cnv_gcm = 0.05, cnv_tdec_margin = 0.05, cnv_cd_alpha = 1, 
                       cci_run_unit = 'sample', cci_n_cells_min = 40, 
                       cci_pval_cutoff = 0.1, cci_mean_cutoff = 0, cci_rth = 0.5, 
                       deg_ref = None, deg_pval_cutoff = 0.01, deg_n_cells_min = 100, 
                       n_cores = 4, data_dir = '.', verbose = True, prefix = ''):
 
     df_mkr_db = mkr_db
     gtf_file = cnv_gtf 
@@ -555,15 +556,15 @@
         if verbose: print('%sIdentifying tumor cells .. ' % prefix)
 
         ref_types = tumor_id_ref_celltypes
 
         df = scoda_icnv_addon( adata_t, gtf_file, ref_types = ref_types, 
                                ref_key = "celltype_major", n_cores = n_cores_to_use,
                                use_ref_only = False, cmd_cutoff = 0.03, gcm = 0.05, 
-                               tumor_dec_margin = cnv_tdec_margin )
+                               tumor_dec_margin = 0.01, cd_alpha = cnv_cd_alpha )
         
         if verbose: print('%sTumor cells identification done. ' % prefix)
         # adata_t.write(file_h5ad)
            
     #############################
     ### Cell-cell interaction ###
```

### Comparing `scoda-tk-0.2.6/src/scoda/viz.py` & `scoda-tk-0.2.7/src/scoda/viz.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.6/src/scoda_tk.egg-info/PKG-INFO` & `scoda-tk-0.2.7/src/scoda_tk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoda-tk
-Version: 0.2.6
+Version: 0.2.7
 Summary: Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Author-email: Seokhyun Yoon <syoon@dku.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `scoda-tk-0.2.6/src/scoda_tk.egg-info/SOURCES.txt` & `scoda-tk-0.2.7/src/scoda_tk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

