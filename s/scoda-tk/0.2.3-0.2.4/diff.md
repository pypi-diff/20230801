# Comparing `tmp/scoda-tk-0.2.3.tar.gz` & `tmp/scoda-tk-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scoda-tk-0.2.3.tar", last modified: Mon Jul 31 13:01:40 2023, max compression
+gzip compressed data, was "scoda-tk-0.2.4.tar", last modified: Tue Aug  1 06:06:11 2023, max compression
```

## Comparing `scoda-tk-0.2.3.tar` & `scoda-tk-0.2.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-31 13:01:40.164673 scoda-tk-0.2.3/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-07-30 14:49:21.000000 scoda-tk-0.2.3/LICENSE
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      128 2023-07-30 14:49:22.000000 scoda-tk-0.2.3/MANIFEST.in
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-07-31 13:01:40.164673 scoda-tk-0.2.3/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-07-30 14:49:22.000000 scoda-tk-0.2.3/README.md
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      826 2023-07-31 13:01:22.000000 scoda-tk-0.2.3/pyproject.toml
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       38 2023-07-31 13:01:40.164673 scoda-tk-0.2.3/setup.cfg
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       49 2023-07-30 14:49:21.000000 scoda-tk-0.2.3/setup.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-31 13:01:39.988677 scoda-tk-0.2.3/src/
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-31 13:01:40.012676 scoda-tk-0.2.3/src/scoda/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-07-30 14:49:25.000000 scoda-tk-0.2.3/src/scoda/__init__.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    21388 2023-07-30 14:49:23.000000 scoda-tk-0.2.3/src/scoda/cpdb.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-31 13:01:40.160673 scoda-tk-0.2.3/src/scoda/default_optional_files/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      291 2023-07-30 14:49:23.000000 scoda-tk-0.2.3/src/scoda/default_optional_files/analysis_config.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)   110525 2023-07-30 14:49:24.000000 scoda-tk-0.2.3/src/scoda/default_optional_files/cpdb.zip
--rw-rw-r--   0 syoon     (1001) syoon     (1001)  9812023 2023-07-30 14:49:24.000000 scoda-tk-0.2.3/src/scoda/default_optional_files/hg38_gene_only.gtf
--rw-rw-r--   0 syoon     (1001) syoon     (1001)     9771 2023-07-30 14:49:23.000000 scoda-tk-0.2.3/src/scoda/default_optional_files/markers_hs.tsv
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    10054 2023-07-30 14:49:23.000000 scoda-tk-0.2.3/src/scoda/default_optional_files/markers_mm.tsv
--rw-rw-r--   0 syoon     (1001) syoon     (1001)  6641898 2023-07-30 14:49:25.000000 scoda-tk-0.2.3/src/scoda/default_optional_files/mm10_gene_only.gtf
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    98551 2023-07-30 14:49:23.000000 scoda-tk-0.2.3/src/scoda/default_optional_files/msig.gmt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    17850 2023-07-30 14:49:25.000000 scoda-tk-0.2.3/src/scoda/deg.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    13716 2023-07-30 14:49:22.000000 scoda-tk-0.2.3/src/scoda/gsea.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)   157974 2023-07-30 14:49:22.000000 scoda-tk-0.2.3/src/scoda/hicat.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    43161 2023-07-31 13:01:09.000000 scoda-tk-0.2.3/src/scoda/icnv.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    31368 2023-07-30 14:49:25.000000 scoda-tk-0.2.3/src/scoda/misc.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    23351 2023-07-31 13:01:06.000000 scoda-tk-0.2.3/src/scoda/pipeline.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    58085 2023-07-31 13:01:13.000000 scoda-tk-0.2.3/src/scoda/viz.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-31 13:01:40.164673 scoda-tk-0.2.3/src/scoda_tk.egg-info/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-07-31 13:01:39.000000 scoda-tk-0.2.3/src/scoda_tk.egg-info/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      776 2023-07-31 13:01:39.000000 scoda-tk-0.2.3/src/scoda_tk.egg-info/SOURCES.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-07-31 13:01:39.000000 scoda-tk-0.2.3/src/scoda_tk.egg-info/dependency_links.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       52 2023-07-31 13:01:39.000000 scoda-tk-0.2.3/src/scoda_tk.egg-info/entry_points.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       54 2023-07-31 13:01:39.000000 scoda-tk-0.2.3/src/scoda_tk.egg-info/requires.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        6 2023-07-31 13:01:39.000000 scoda-tk-0.2.3/src/scoda_tk.egg-info/top_level.txt
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-01 06:06:11.416899 scoda-tk-0.2.4/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-07-30 14:49:21.000000 scoda-tk-0.2.4/LICENSE
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      128 2023-07-30 14:49:22.000000 scoda-tk-0.2.4/MANIFEST.in
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-08-01 06:06:11.416899 scoda-tk-0.2.4/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-07-30 14:49:22.000000 scoda-tk-0.2.4/README.md
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      826 2023-08-01 06:05:53.000000 scoda-tk-0.2.4/pyproject.toml
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       38 2023-08-01 06:06:11.416899 scoda-tk-0.2.4/setup.cfg
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       49 2023-07-30 14:49:21.000000 scoda-tk-0.2.4/setup.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-01 06:06:11.284902 scoda-tk-0.2.4/src/
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-01 06:06:11.296902 scoda-tk-0.2.4/src/scoda/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-07-30 14:49:25.000000 scoda-tk-0.2.4/src/scoda/__init__.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    21388 2023-07-30 14:49:23.000000 scoda-tk-0.2.4/src/scoda/cpdb.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-01 06:06:11.412899 scoda-tk-0.2.4/src/scoda/default_optional_files/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      291 2023-07-30 14:49:23.000000 scoda-tk-0.2.4/src/scoda/default_optional_files/analysis_config.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)   110525 2023-07-30 14:49:24.000000 scoda-tk-0.2.4/src/scoda/default_optional_files/cpdb.zip
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)  9812023 2023-07-30 14:49:24.000000 scoda-tk-0.2.4/src/scoda/default_optional_files/hg38_gene_only.gtf
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)     9771 2023-07-30 14:49:23.000000 scoda-tk-0.2.4/src/scoda/default_optional_files/markers_hs.tsv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    10054 2023-07-30 14:49:23.000000 scoda-tk-0.2.4/src/scoda/default_optional_files/markers_mm.tsv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)  6641898 2023-07-30 14:49:25.000000 scoda-tk-0.2.4/src/scoda/default_optional_files/mm10_gene_only.gtf
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    98551 2023-07-30 14:49:23.000000 scoda-tk-0.2.4/src/scoda/default_optional_files/msig.gmt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    17850 2023-07-30 14:49:25.000000 scoda-tk-0.2.4/src/scoda/deg.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    13716 2023-07-30 14:49:22.000000 scoda-tk-0.2.4/src/scoda/gsea.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)   157974 2023-07-30 14:49:22.000000 scoda-tk-0.2.4/src/scoda/hicat.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    29133 2023-08-01 06:05:21.000000 scoda-tk-0.2.4/src/scoda/icnv.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    31368 2023-07-30 14:49:25.000000 scoda-tk-0.2.4/src/scoda/misc.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    23430 2023-08-01 06:05:17.000000 scoda-tk-0.2.4/src/scoda/pipeline.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    58085 2023-07-31 13:01:13.000000 scoda-tk-0.2.4/src/scoda/viz.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-01 06:06:11.412899 scoda-tk-0.2.4/src/scoda_tk.egg-info/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-08-01 06:06:11.000000 scoda-tk-0.2.4/src/scoda_tk.egg-info/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      776 2023-08-01 06:06:11.000000 scoda-tk-0.2.4/src/scoda_tk.egg-info/SOURCES.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-08-01 06:06:11.000000 scoda-tk-0.2.4/src/scoda_tk.egg-info/dependency_links.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       52 2023-08-01 06:06:11.000000 scoda-tk-0.2.4/src/scoda_tk.egg-info/entry_points.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       54 2023-08-01 06:06:11.000000 scoda-tk-0.2.4/src/scoda_tk.egg-info/requires.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        6 2023-08-01 06:06:11.000000 scoda-tk-0.2.4/src/scoda_tk.egg-info/top_level.txt
```

### Comparing `scoda-tk-0.2.3/LICENSE` & `scoda-tk-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.3/PKG-INFO` & `scoda-tk-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoda-tk
-Version: 0.2.3
+Version: 0.2.4
 Summary: Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Author-email: Seokhyun Yoon <syoon@dku.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `scoda-tk-0.2.3/pyproject.toml` & `scoda-tk-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "scoda-tk"
-version = "0.2.3"
+version = "0.2.4"
 description = "Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)"
 readme = "README.md"
 authors = [{ name = "Seokhyun Yoon", email = "syoon@dku.edu" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `scoda-tk-0.2.3/src/scoda/cpdb.py` & `scoda-tk-0.2.4/src/scoda/cpdb.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.3/src/scoda/default_optional_files/cpdb.zip` & `scoda-tk-0.2.4/src/scoda/default_optional_files/cpdb.zip`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.3/src/scoda/default_optional_files/hg38_gene_only.gtf` & `scoda-tk-0.2.4/src/scoda/default_optional_files/hg38_gene_only.gtf`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.3/src/scoda/default_optional_files/markers_hs.tsv` & `scoda-tk-0.2.4/src/scoda/default_optional_files/markers_hs.tsv`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.3/src/scoda/default_optional_files/markers_mm.tsv` & `scoda-tk-0.2.4/src/scoda/default_optional_files/markers_mm.tsv`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.3/src/scoda/default_optional_files/mm10_gene_only.gtf` & `scoda-tk-0.2.4/src/scoda/default_optional_files/mm10_gene_only.gtf`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.3/src/scoda/default_optional_files/msig.gmt` & `scoda-tk-0.2.4/src/scoda/default_optional_files/msig.gmt`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.3/src/scoda/deg.py` & `scoda-tk-0.2.4/src/scoda/deg.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.3/src/scoda/gsea.py` & `scoda-tk-0.2.4/src/scoda/gsea.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.3/src/scoda/hicat.py` & `scoda-tk-0.2.4/src/scoda/hicat.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.3/src/scoda/icnv.py` & `scoda-tk-0.2.4/src/scoda/icnv.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import warnings, math, time, copy
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 from sklearn import cluster, mixture
 from sklearn.neighbors import kneighbors_graph
 from sknetwork.clustering import Louvain
+from sklearn.decomposition import PCA, IncrementalPCA, TruncatedSVD
 
 import scanpy as sc
 import infercnvpy as cnv
 
 cell_cycle_genes_s = ['ATAD2', 'BLM', 'BRIP1', 'CASP8AP2', 'CCNE2',
          'CDC45', 'CDC6', 'CDCA7', 'CHAF1B', 'CLSPN', 'DSCC1',
          'DTL', 'E2F8', 'EXO1', 'FEN1', 'GINS2', 'GMNN', 'HELLS',
@@ -423,294 +424,14 @@
                     label_fs = 12, tick_fs = 11, legend_fs = 11, 
                     legend_loc = 'upper left', bbox_to_anchor = (1, 1),
                     figsize = (4,3), log = False, alpha = 0.8 )
         
     return obs[['tumor_dec'+ suffix, 'tumor_prob'+ suffix, 'tumor_cluster'+ suffix]], params
 
 
-def get_cnv_threshold( obs, cluster_sel, score_key = 'cnv_score', 
-                       cluster_key = 'cnv_leiden', th_min = 0, refp_min = 0.9, 
-                       p_exc = 0.1, plot_stat = True, suffix = '', Data = None ):
-    
-    ## obs must contain columns 'cnv_cluster', 'cnv_score'
-    start_time = time.time()
-    
-    df = obs.groupby([cluster_key])[score_key].agg(**{'cmean':'median'})
-    idx_lst = list(df.index.values)
-    
-    ns = 0
-    # while(ns == 0):
-        
-    b_inc = []
-    for idx in idx_lst:
-        if idx in cluster_sel:
-            b_inc.append(True)
-        else:
-            b_inc.append(False)
-
-    df['b_inc'] = b_inc
-    b = np.array(b_inc)
-    # print(df)
-
-    ns = np.sum(b)
-    # if ns == 0: refp_min *= 0.95
-    if ns == 0:
-        print('ERROR: no reference type clusters found.')
-        obs['tumor_score'+ suffix] = 0
-        obs['tumor_dec'+ suffix] = 'NA'
-        obs['tumor_cluster'+ suffix] = ''
-        return None
-    elif ns == 1:
-        print('WARNING: Only one reference type cluster found.')
-        cmeans = np.array(df.loc[b,'cmean'])
-        th2 = cmeans[0]
-        b2 = df['cmean'] <= th2
-    else:        
-        cmeans = np.array(df.loc[b,'cmean'])
-        odr = cmeans.argsort()
-        m = int(round(ns*(1-p_exc)))
-        if m == len(odr):
-            m = m-1
-        if m < 0: m = 0
-        # th2 = cmeans[odr[m]]
-        th2 = cmeans.max()
-        b2 = df['cmean'] <= th2
-        # b = b & b2
-    
-    ns = np.sum(~b)
-    if ns > 0:
-        cmeans = np.array(df.loc[~b,'cmean'])
-        odr = cmeans.argsort()
-
-        m = int(round(ns*(p_exc)))
-        if m == len(odr):
-            m = m-1
-        th3 = cmeans[odr[m]]
-        b3 = df['cmean'] >= max(th3, th2) 
-    else:
-        th3 = df['cmean'].max()
-        b3 = False
-
-    
-    # print(th2, th3)
-    
-    w0 = np.sum(b&b2)/(len(b)*p_exc)
-    m0 = df.loc[b&b2,'cmean'].mean()
-    if np.sum(b&b2) > 1:
-        v0 = df.loc[b&b2,'cmean'].var()
-    else:
-        idx = df.index.values[b&b2][0]
-        bt = obs[cluster_key] == idx
-        v0 = obs.loc[bt, score_key].var()
-        
-
-    for k, idx in enumerate(idx_lst):
-        if df.loc[idx, 'cmean'] <= (m0 + np.sqrt(v0)):
-            b[k] = True
-                    
-    if np.sum((~b)&b3) > 0:
-        w1 = np.sum((~b)&b3)/(len(b)*p_exc)
-        m1 = df.loc[(~b)&b3,'cmean'].mean()
-        if np.sum((~b)&b3) > 1:
-            v1 = df.loc[(~b)&b3,'cmean'].var()
-        else:
-            idx = df.index.values[(~b)&b3][0]
-            bt = obs[cluster_key] == idx
-            v1 = obs.loc[bt, score_key].var()
-    else:
-        w1 = 0
-        m1 = np.abs(th3 - m0)*2 + m0 # m0*10
-        v1 = v0
-
-    mxv = df['cmean'].max()
-    mnv = df['cmean'].min()
-    Dv = mxv - mnv
-    dv = Dv/200
-    n_bins = 30
-
-    x = np.arange(mnv,mxv,dv)
-    pdf0, xs0 = get_normal_pdf( x, m0, v0, 100)
-    pdf1, xs1 = get_normal_pdf( x, m1, v1, 100)
-
-    pdf0 = pdf0 #*w0
-    pdf1 = pdf1 #*w1
-    
-    th = -1
-    for k in range(len(xs0)):
-        if (pdf1[k] >= pdf0[k]) & (xs0[k] > m0):
-            th = xs0[k]
-            break
-            
-    ss_div_dm = (np.sqrt(v1)+np.sqrt(v0))/(m1-m0)
-    if ss_div_dm > 1:
-        print('INFO: Std_sum/Mean_diff: %f > 1' % (ss_div_dm))
-        print('INFO: indicating that no tumor cells might be present in this sample.' % (ss_div_dm))
-        # th = m0 + np.sqrt(v0)
-        
-    # print('threshold: ', th )
-    th = max(th, th_min)
-            
-    s = obs[score_key]
-    tpr = get_malignancy_prob( s, [w0, m0, v0, w1, m1, v1] )
-    
-    obs['tumor_score'+ suffix] = tpr
-    
-    dec = pd.Series(['Normal']*len(s), index = obs.index)
-    '''
-    b = s >= th
-    dec[b] = 'Tumor'
-    dec[~b] = 'Normal'
-    '''
-    bs = (s > th)
-    for idx in idx_lst:
-        if df.loc[idx, 'cmean'] > th:
-            b1 = obs[cluster_key] == idx
-            dec[b1] = 'Tumor'
-            
-    '''
-    lt = th - (th - m0)*0.05 
-    ut = th + (m1 - th)*0.05
-    b = (s > lt) & (s < ut) & (~br)
-    print(lt, ut, np.sum(~br), np.sum(b))
-    dec[b] = 'unclear'
-    '''
-    if ss_div_dm > 1:
-        b = dec == 'Tumor'
-        print('INFO: %i among %i were identified as tumor cells, which, however, might be normal cells.' \
-              % (np.sum(b), len(b)))
-    
-    # b = (obs[ref_key].isin(ref_types)) | (s <= th)
-    # dec[b] = 'Normal'    
-    obs['tumor_dec'+ suffix] = dec
-
-    tclust = dec.copy(deep = True)
-    tclust[:] = None
-    cnt = 1
-    for c in idx_lst:
-        b = obs[cluster_key] == c
-        b1 = dec == 'Tumor'
-        if np.sum(b&b1) > 0:
-            tclust[b&b1] = 'Tumor_c%i' % cnt
-            cnt += 1        
-    obs['tumor_cluster'+ suffix] = tclust
-    
-    etime = round(time.time() - start_time) 
-    # print('CNVth(%i) ' % etime, end = '', flush = True)
-    
-    params = {}
-    params['th'] = th
-    params['m0'] = m0
-    params['v0'] = v0
-    params['w0'] = w0
-    params['m1'] = m1
-    params['v1'] = v1
-    params['w1'] = w1
-    params['df'] = df
-    
-    if plot_stat:
-        plot_stats( params, n_bins = 30, title = None, title_fs = 14,
-                    label_fs = 12, tick_fs = 11, legend_fs = 11, 
-                    legend_loc = 'upper left', bbox_to_anchor = (1, 1),
-                    figsize = (4,3), log = False, alpha = 0.8 )
-
-    return obs[['tumor_dec'+ suffix, 'tumor_score'+ suffix, 'tumor_cluster'+ suffix]], params
-
-
-def plot_stats( params, n_bins = 30, title = None, title_fs = 14,
-                label_fs = 12, tick_fs = 11, legend_fs = 11, 
-                legend_loc = 'upper left', bbox_to_anchor = (1, 1),
-                figsize = (4,3), log = True, alpha = 0.8 ):
-    
-    th = params['th']
-    m0 = params['m0']
-    v0 = params['v0']
-    w0 = params['w0']
-    m1 = params['m1']
-    v1 = params['v1']
-    w1 = params['w1']
-    df = params['df']
-        
-    mxv = df['cmean'].max()
-    mnv = df['cmean'].min()
-    Dv = mxv - mnv
-    dv = Dv/200
-
-    x = np.arange(mnv,mxv,dv)
-    pdf0, xs0 = get_normal_pdf( x, m0, v0, 100)
-    pdf1, xs1 = get_normal_pdf( x, m1, v1, 100)
-    
-    pr = pdf1/(pdf1 + pdf0) # get_malignancy_prob( xs0, [w0, m0, v0, w1, m1, v1] )
-    bx = (xs0 >= m0) & ((xs1 <= m1))
-
-    nn = len(df['cmean'])
-    pdf0 = pdf0*(w0*nn*(200/n_bins)/pdf0.sum())
-    pdf1 = pdf1*(w1*nn*(200/n_bins)/(pdf1.sum())) 
-
-    max_pdf = max(pdf0.max(), pdf1.max())
-    
-    plt.figure(figsize = figsize)
-    ax = plt.gca()
-    
-    counts, bins = np.histogram(df['cmean'], bins = n_bins)
-    # max_cnt = np.max(counts)
-
-    legend_labels = []
-    
-    max_cnt = 0
-    b = df['dec'] == 'Normal'
-    if np.sum(b) > 0:
-        legend_labels.append('Normal')
-        counts, bins_t, bar_t = plt.hist(df.loc[b, 'cmean'], bins = bins, alpha = alpha)
-        max_cnt = max(max_cnt, np.max(counts))
-    b = df['dec'] == 'Tumor'
-    if np.sum(b) > 0:
-        legend_labels.append('Tumor')
-        counts, bins_t, bar_t = plt.hist(df.loc[b, 'cmean'], bins = bins, alpha = alpha)
-        max_cnt = max(max_cnt, np.max(counts))
-    b = df['dec'] == 'unclear'
-    if np.sum(b) > 0:
-        legend_labels.append('unclear')
-        counts, bins_t, bar_t = plt.hist(df.loc[b, 'cmean'], bins = bins, alpha = alpha)
-        max_cnt = max(max_cnt, np.max(counts))
-    
-    sf = 0.9*max_cnt/max_pdf
-    plt.plot(xs0, pdf0*sf)
-    plt.plot(xs1, pdf1*sf)
-    plt.plot([th, th], [0, max_cnt]) # max(pdf0.max()*sf, pdf1.max()*sf)])
-    plt.plot(xs0[bx], pr[bx]*max_cnt)
-
-    if title is not None: plt.title(title, fontsize = title_fs)
-    plt.xlabel('CNV_score', fontsize = label_fs)
-    plt.ylabel('Number of clusters', fontsize = label_fs)
-    plt.legend(['Normal distr.', 'Tumor distr.', 'Threshold', 'Tumor Prob.'], #, 'Score hist.'], 
-               loc = legend_loc, bbox_to_anchor = bbox_to_anchor, fontsize = legend_fs)
-    if log: plt.yscale('log')
-    ax.tick_params(axis='x', labelsize=tick_fs)
-    ax.tick_params(axis='y', labelsize=tick_fs)
-    plt.grid()
-    plt.show()
-        
-    return 
-    
-
-def get_cnv_dec(adata, ref_key, ref_types, cluster_key = 'cnv_leiden', 
-                       score_key = 'cnv_score', th_min = 0, use_ref = True, suffix = ''):
-    
-    if use_ref:
-        df = get_cnv_threshold_useref( adata.obs, ref_key, ref_types, 
-                                       score_key = score_key, cluster_key = cluster_key, th_min = th_min,
-                                       plot_stat = True, suffix = suffix )
-    else:
-        df = get_cnv_threshold_bimodal( adata.obs, ref_key, ref_types, score_key = score_key, 
-                                        cluster_key = cluster_key, th_min = th_min, 
-                                        plot_stat = True, suffix = suffix )
-    
-    return adata.obs[[cluster_key, score_key, 'tumor_dec'+suffix, 'tumor_score'+suffix]]
-
-
 def detect_communities(X_pca, y_clust, cobj, pmaj = 0.7, 
                              cutoff = 0.01, verbose = False ):
     
     adj_agg = cobj.aggregate_
     adj_agg_mat = adj_agg.todense().astype(int) 
     labels_unique, counts = np.unique(y_clust, return_counts=True)
 
@@ -789,156 +510,75 @@
     
     ss = np.array(ss)
     odr = ss.argsort()
     
     return cm[odr[0]]
 
 
-def compute_cnv_scores(adata, ref_ind, use_cnv_score = False,
-                       cluster_key = 'cnv_leiden', score_key = 'tumor_score', 
-                       gmm_N_comp = 20, th_min = 0, refp_min = 0.9, p_exc = 0.1, 
-                       dec_margin = 0.05, clustering_res = 4, n_neighbors = 10, gcm = 0.05,
-                       plot_stat = False, use_cnv_cluster = True, use_ref = True, suffix = '', Data = None):
-    
-    score_key = score_key + suffix
-    ## Get X_pca for ref_type cells
+def find_major_clusters(adj_agg_mat, seed_clusters):
 
-    X_pca = adata.obsm['X_cnv_pca']
-    
-    start_time = time.time()
-    print('Running iCNV addon .. ', end = '', flush = True)
-    
-    if use_cnv_cluster:      
-        y_clust = adata.obs[cluster_key].copy(deep = True)
-        cnv_clust_lst = list(set(y_clust))
-        cobj = None
-    else:
-        # y_clust, cobj = clustering_alg(X_pca, clust_algo = 'lv', 
-        #                                resolution = clustering_res, N_neighbors = n_neighbors)         
-        adj = kneighbors_graph(X_pca, int(n_neighbors), mode='connectivity', include_self=True)
-        etime = round(time.time() - start_time) 
-        print('N(%i).' % etime, end = '', flush = True)
-            
-        cobj = Louvain(resolution = clustering_res)
-        y_clust = cobj.fit_transform(adj)        
-        
-        adata.obs[cluster_key] = y_clust
-        adata.obs[cluster_key] = adata.obs[cluster_key].astype(str)
-        y_clust = pd.Series(y_clust, index = adata.obs.index)
-        cnv_clust_lst = list(set(y_clust))
-        
-    if use_cnv_score:
-        adata.obs[score_key] = adata.obs['cnv_score']
-    else:
-        if use_ref:
-            cnv_clust_lst.sort()
-            b_inc = []
-            for idx in cnv_clust_lst:
-                b = y_clust == idx
-                bt = ref_ind
-                cnt = np.sum(b&bt)
-
-                if (cnt >= refp_min*np.sum(b)):
-                    b_inc.append(True)
-                else:
-                    b_inc.append(False)
-
-            if np.sum(b_inc) > 0:
-                cluster_sel = list(np.array(cnv_clust_lst)[b_inc]) 
-                b = y_clust == cluster_sel[0]
-                for c in cluster_sel[1:]:
-                    b = b | (y_clust == c)
-            else:
-                print('ERROR: No reference cell types found.')
-                adata.obs[score_key] = 0
-                adata.obs['tumor_prob'+ suffix] = 0
-                adata.obs['tumor_dec'+ suffix] = 'NA'
-                adata.obs['tumor_cluster'+ suffix] = ''
-                return adata.obs[[cluster_key, score_key, 'tumor_dec'+suffix, 
-                          'tumor_prob'+suffix, 'tumor_cluster'+ suffix]]
-            X_pca_sel = X_pca[b,:]
+    adj_agg_mat = adj_agg_mat - np.diag(np.diag(adj_agg_mat))
+
+    for a in range(adj_agg_mat.shape[0] - len(seed_clusters)):
+        # def get_pv( s, adj_agg_mat, seed_clusters ):
+        mn = adj_agg_mat[seed_clusters, :].mean(axis = 0)
+        sd = adj_agg_mat[seed_clusters, :].std(axis = 0)
+
+        pvss = []
+        for n in range(adj_agg_mat.shape[0]):
+
+            if n in seed_clusters:
+                pvs = []
+                for s in seed_clusters:
+                    if n != s:
+                        st = np.abs(mn[s] - mn[n])/((sd[s] + sd[n]))
+                        pv = stats.t.sf(st*np.sqrt(2), df = len(seed_clusters))*2
+                        pv = np.round(pv, 3)
+                        pvs.append(pv)
+
+                # print(n, pvs, np.max(pvs))
+                pvss.append(pvs)
+
+        pvss = np.array(pvss)
+        th = pvss.max(axis = 1).min()
+
+        pvss = []
+        nodes = []
+        for n in range(adj_agg_mat.shape[0]):
+
+            if n not in seed_clusters:
+                pvs = []
+                for s in seed_clusters:
+                    st = np.abs(mn[s] - mn[n])/((sd[s] + sd[n]))
+                    pv = stats.t.sf(st*np.sqrt(2), df = len(seed_clusters))*2
+                    pv = np.round(pv, 3)
+                    pvs.append(pv)
+
+                # print(n, pvs, np.max(pvs))
+                nodes.append(n)
+                pvss.append(pvs)
+
+        pvss = np.array(pvss)
+        nodes = np.array(nodes)
+        pvs = pvss.max(axis = 1)
+        odr = pvs.argsort()
+        mx_pv = pvs[odr[-1]]
+        if mx_pv >= th:
+            seed_clusters.append(nodes[odr[-1]])
+            # print(th, mx_pv, seed_clusters)
         else:
+            break
             
-            if cobj is None:
-                X_pca_sel = X_pca
-            else:
-                communities = detect_communities(X_pca, y_clust, cobj, pmaj = 0.7, 
-                                 cutoff = 0.01, verbose = False )
-                cluster_sel = merge_communities( communities )
-
-                if len(cluster_sel) > 0:
-                    b = y_clust == cluster_sel[0]
-                    for c in cluster_sel[1:]:
-                        b = b | (y_clust == c)
-                else:
-                    print('ERROR: No reference cell types found.')
-                    adata.obs[score_key] = 0
-                    adata.obs['tumor_prob'+ suffix] = 0
-                    adata.obs['tumor_dec'+ suffix] = 'NA'
-                    adata.obs['tumor_cluster'+ suffix] = ''
-                    return adata.obs[[cluster_key, score_key, 'tumor_dec'+suffix, 
-                              'tumor_prob'+suffix, 'tumor_cluster'+ suffix]]
-                
-                X_pca_sel = X_pca[b,:]
-
-
-        etime = round(time.time() - start_time) 
-        # print('C(%i).' % etime, end = '', flush = True)
-
-        ## Get GMM model parameters
-        gmm = mixture.GaussianMixture(n_components = int(gmm_N_comp), random_state = 0)
-        gmm.fit(X_pca_sel)
-        y_conf_gmm = -gmm.score_samples(X_pca)
-        #'''
-        X_cnv = pd.DataFrame(adata.obsm['X_cnv'].todense(), index = adata.obs.index.values)
-        y_conf = np.sqrt((X_cnv**2).mean(axis = 1))*100  
-
-        yc = np.array(y_conf)
-        odr = yc.argsort()
-        n = int(len(yc)*0.975)
-        ymax = yc[odr[n]]
-        b = y_conf > ymax
-        y_conf[b] = ymax
-
-        adata.obs[score_key] = y_conf*(1/(1+np.exp(-y_conf_gmm*gcm)))
-
-        etime = round(time.time() - start_time) 
-        print('G(%i)' % etime, end = '', flush = True)
-    
-    ## Replace GMM scores with their cluster mean
-    '''
-    cnv_clust_lst = list(set(adata.obs[cluster_key]))
-    for c in cnv_clust_lst:
-        b = adata.obs[cluster_key] == c
-        adata.obs.loc[b, score_key] = adata.obs.loc[b, score_key].mean()
-    '''
-    # if use_ref:
-    df, params = get_cnv_threshold_useref( adata.obs, ref_ind, 
-                                   score_key = score_key, cluster_key = cluster_key,
-                                   th_min = th_min, refp_min = refp_min, p_exc = p_exc, ucr = dec_margin,
-                                   plot_stat = plot_stat, suffix = suffix, Data = Data )
-    '''
-    else:
-        df, params = get_cnv_threshold_bimodal( adata.obs, ref_ind, 
-                                        score_key = score_key, cluster_key = cluster_key, 
-                                        th_min = th_min, refp_min = refp_min, ucr = dec_margin,
-                                        plot_stat = plot_stat, suffix = suffix, Data = Data )
-    #'''
-    
-    etime = round(time.time() - start_time) 
-    print(' .. done (%i) ' % etime) #, end = '', flush = True)
-    
-    return adata.obs[[cluster_key, score_key, 'tumor_dec'+suffix, 
-                      'tumor_prob'+suffix, 'tumor_cluster'+ suffix]], params
+    return seed_clusters
 
 
 import warnings
 
 def run_icnv(adata, ref_key, ref_types, gtf_file, cluster_key = 'cnv_leiden', 
-             resolution = 2, N_pca = 15, n_neighbors = 10, umap = True, pca_umap = True, n_cores = 4 ):
+             resolution = 2, N_pca = 15, n_neighbors = 10, umap = True, pca = True, n_cores = 4 ):
     
     pca_umap = umap
     with warnings.catch_warnings():
         warnings.simplefilter("ignore")
     
         ## Normalize and log-transform
         sc.pp.normalize_total(adata, target_sum=1e4)
@@ -947,16 +587,17 @@
         sc.pp.highly_variable_genes(adata, n_top_genes = 2000) # , flavor = 'seurat_v3')
         # sc.tl.score_genes_cell_cycle(adata, cell_cycle_genes_s, cell_cycle_genes_g2m)
 
         cnv.io.genomic_position_from_gtf(gtf_file, adata, gtf_gene_id='gene_name', adata_gene_id=None, inplace=True)
         cnv.tl.infercnv(adata, reference_key = ref_key, reference_cat=ref_types, 
                         window_size=100, n_jobs = n_cores)
 
-        print('PCA .. ', end = '')
-        cnv.tl.pca(adata, n_comps = N_pca) 
+        if pca:
+            print('PCA .. ', end = '')
+            cnv.tl.pca(adata, n_comps = N_pca) 
         
         if umap:
             print('Finding neighbors .. ', end = '')
             cnv.pp.neighbors(adata, key_added = 'cnv_neighbors', n_neighbors=n_neighbors, n_pcs=N_pca)
             print('Clustering .. ', end = '')
             cnv.tl.leiden(adata, neighbors_key='cnv_neighbors', key_added=cluster_key, resolution = resolution)
             print('UMAP .. ', end = '')
@@ -982,29 +623,14 @@
 try:
     from sknetwork.clustering import Louvain
 except ImportError:
     print('WARNING: sknetwork not installed. Will used GMM for clustering.')
     CLUSTERING_AGO = 'gmm'
     SKNETWORK = False
 
-from sklearn.decomposition import PCA
-from sklearn import cluster, mixture
-from sklearn.neighbors import KNeighborsRegressor
-from sklearn.neighbors import kneighbors_graph
-from sklearn.neighbors import NearestNeighbors
-
-CLUSTERING_AGO = 'lv'
-SKNETWORK = True
-try:
-    from sknetwork.clustering import Louvain
-except ImportError:
-    print('WARNING: sknetwork not installed. Will used GMM for clustering.')
-    CLUSTERING_AGO = 'gmm'
-    SKNETWORK = False
-
     
 def clustering_alg(X_pca, clust_algo = 'lv', N_clusters = 25, resolution = 1, N_neighbors = 10, 
                    mode='distance', n_cores = 4):
     
     if clust_algo[:2] == 'gm':
         gmm = mixture.GaussianMixture(n_components = int(N_clusters), random_state = 0)
         cluster_label = gmm.fit_predict(np.array(X_pca))
@@ -1026,15 +652,51 @@
     elif clust_algo[:2] == 'ld':
         leiden = LeidenClustering()
         leiden.fit(X)
         cluster_label = leiden.labels_
         return cluster_label, km
     '''
 
-def detect_tumor_cells(X_cnv, ref_ind, pca = False, use_cnv_score = False, 
+def get_cluster_stat( obs, ref_ind, cluster_key = 'cnv_cluster', 
+                      score_key = 'tumor_score', refp_min = 0.9):
+    
+    # df = obs.groupby([cluster_key])[score_key].agg(**{'cmean':'median'})
+    df = obs.groupby([cluster_key])[score_key].agg(**{'cmean':'mean'})
+    idx_lst = list(df.index.values)
+    
+    ns = 0
+    # while(ns == 0):
+        
+    b_inc = []
+    df['Ref_percent'] = 0
+    for idx in idx_lst:
+        b = obs[cluster_key] == idx
+        # cts = obs.loc[b, ref_key]
+        '''
+        ct_vc = cts.value_counts()
+        cnt = 0
+        for ct in list(ct_vc.index.values):
+            if ct in ref_types:
+                cnt += ct_vc[ct]
+        '''
+        cnt = np.sum(np.array(ref_ind)[b])
+        ref_percent = cnt/np.sum(b)
+        df.loc[idx, 'Ref_percent'] = ref_percent
+        if (ref_percent >= refp_min):
+            b_inc.append(True)
+        else:
+            b_inc.append(False)
+
+    df['b_inc'] = b_inc
+    b = np.array(b_inc)
+    # print(df)
+    return df
+
+
+def identify_tumor_cells(X_cnv, ref_ind, pca = False, use_cnv_score = False, 
                        clust = None, Clustering_resolution = 1, N_clusters = 30,
                        # cluster_key = 'cnv_leiden', score_key = 'tumor_score', 
                        gmm_N_comp = 20, th_min = 0, refp_min = 0.9, p_exc = 0.1, 
                        dec_margin = 0.05, n_neighbors = 10, cmd_cutoff = 0.03, 
                        gcm = 0.05, plot_stat = False, use_ref = False, 
                        n_cores = 4, suffix = '', Data = None):
     
@@ -1050,37 +712,33 @@
     if isinstance(X_cnv, pd.DataFrame):
         df = pd.DataFrame(index = X_cnv.index.values)
     else:
         df = pd.DataFrame()
         X_cnv = pd.DataFrame(X_cnv)
     
     N_components_pca = 15
-    pca_obj = PCA(n_components = int(N_components_pca), copy = True, random_state = 0)
-
+    # pca_obj = PCA(n_components = int(N_components_pca), copy = True, random_state = 0)
+    pca_obj = TruncatedSVD(n_components = int(N_components_pca)) # , algorithm = 'arpack')
+    
     if not pca: 
         X_pca = pca_obj.fit_transform(X_cnv)
         
         etime = round(time.time() - start_time) 
         print('P(%i) .. ' % etime, end = '', flush = True)
-        start_time = time.time()
-           
+        start_time = time.time()           
     else: 
         X_pca = np.array(X_cnv.copy(deep = True)) #.copy(deep = True)
             
-    if (clust is not None) & (use_ref):      
-        y_clust = list(clust)
-        cobj = None
-    else:
-        y_clust, cobj = clustering_alg(X_pca, clust_algo = CLUSTERING_AGO, N_clusters = N_clusters, 
-                                       resolution = Clustering_resolution, N_neighbors = n_neighbors, 
-                                       n_cores = n_cores)
+    y_clust, cobj = clustering_alg(X_pca, clust_algo = CLUSTERING_AGO, N_clusters = N_clusters, 
+                                   resolution = Clustering_resolution, N_neighbors = n_neighbors, 
+                                   n_cores = n_cores)
         
-        etime = round(time.time() - start_time) 
-        print('C(%i) .. ' % etime, end = '', flush = True)
-        start_time = time.time()
+    etime = round(time.time() - start_time) 
+    print('C(%i) .. ' % etime, end = '', flush = True)
+    start_time = time.time()
     
     cnv_clust_lst = list(set(y_clust))
     df[cluster_key] = y_clust
         
     cluster_sel = None
     
     if ref_ind is not None: # use_ref:
@@ -1096,122 +754,80 @@
             if (cnt >= refp_min*np.sum(b)):
                 b_inc.append(True)
             else:
                 b_inc.append(False)
 
         if np.sum(b_inc) > 0:
             cluster_sel = list(np.array(cnv_clust_lst)[b_inc]) 
-            b = y_clust == cluster_sel[0]
-            for c in cluster_sel[1:]:
-                b = b | (y_clust == c)
         else:
             print('ERROR: No reference cell types found.')
             df[score_key] = 0
             df['tumor_prob'+ suffix] = 0
             df['tumor_dec'+ suffix] = 'NA'
             df['tumor_cluster'+ suffix] = ''
             return df[[cluster_key, score_key, 'tumor_dec'+suffix, 
                       'tumor_prob'+suffix, 'tumor_cluster'+ suffix]]
         #'''
-        
-        X_pca_sel = X_pca[b,:]
-    # else:
-    
-    if (cobj is None) & (ref_ind is None):
-        y_clust, cobj = clustering_alg(X_pca, clust_algo = CLUSTERING_AGO, N_clusters = N_clusters, 
-                                       resolution = Clustering_resolution, N_neighbors = n_neighbors, 
-                                       n_cores = n_cores)
-        
-        etime = round(time.time() - start_time) 
-        print('C(%i) .. ' % etime, end = '', flush = True)
-        start_time = time.time()
-        
-    if (cobj is not None) & ((ref_ind is None) | (not use_ref)):
-        
+    else:
         communities = detect_communities(X_pca, y_clust, cobj, pmaj = 0.7, 
                          cutoff = cmd_cutoff, verbose = False )
-        cluster_sel_addon = merge_communities( communities )
+        cluster_sel = merge_communities( communities )
         
-        if cluster_sel is None:
-            cluster_sel = cluster_sel_addon
-        else:
-            cluster_sel = list(set(cluster_sel).union(cluster_sel_addon))
 
-        if len(cluster_sel) > 0:
-            b = y_clust == cluster_sel[0]
-            if len(cluster_sel) > 1:
-                for c in cluster_sel[1:]:
-                    b = b | (y_clust == c)
-            ref_addon = b
-        else:
-            print('ERROR: No reference cell types found.')
-            adata.obs[score_key] = 0
-            adata.obs['tumor_prob'+ suffix] = 0
-            adata.obs['tumor_dec'+ suffix] = 'NA'
-            adata.obs['tumor_cluster'+ suffix] = ''
-            return adata.obs[[cluster_key, score_key, 'tumor_dec'+suffix, 
-                      'tumor_prob'+suffix, 'tumor_cluster'+ suffix]]
+    adj_agg = cobj.aggregate_
+    adj_agg_mat = np.array(adj_agg.todense().astype(int)) 
+    adj_agg_mat = adj_agg_mat - np.diag(np.diag(adj_agg_mat))
 
-        X_pca_sel = X_pca[b,:]
+    cluster_sel = find_major_clusters(adj_agg_mat, cluster_sel)
+    
+    b = y_clust == cluster_sel[0]
+    if len(cluster_sel) > 1:
+        for c in cluster_sel[1:]:
+            b = b | (y_clust == c)
+    ref_ind2 = b
+    
+    print('N_ref: %i -> %i .. ' % \
+          (np.sum(ref_ind), np.sum(ref_ind2)), end = '')
 
-    ## Get GMM model parameters
+    #'''
+    X_pca_sel = X_pca[ref_ind2,:]
+    
     gmm = mixture.GaussianMixture(n_components = int(gmm_N_comp), random_state = 0)
     gmm.fit(X_pca_sel)
     y_conf_gmm = -gmm.score_samples(X_pca)
     #'''
-    y_conf = np.sqrt((X_cnv**2).mean(axis = 1))*100  
 
+    y_conf = np.sqrt((X_cnv**2).mean(axis = 1))*100  
+    #'''
     yc = np.array(y_conf)
     odr = yc.argsort()
     n = int(len(yc)*0.975)
     ymax = yc[odr[n]]
     b = y_conf > ymax
     y_conf[b] = ymax
+    #'''
 
     # df[score_key] = y_conf*(1/(1+np.exp(-y_conf_gmm)))
-    df[score_key] = np.log(y_conf*(1/(1+np.exp(-y_conf_gmm*gcm)))) 
+    df[score_key] = np.log((y_conf)*(1/(1+np.exp(-y_conf_gmm*gcm))) + 1e-10) 
+    # df[score_key] = np.log(y_conf + 1e-10)
 
     etime = round(time.time() - start_time) 
     print('G(%i) .. ' % etime, end = '', flush = True)
     start_time = time.time()
     
-    ## Replace GMM scores with their cluster mean
-    #'''
-    if (ref_ind is not None):
-        #'''
-        if (ref_addon is not None):
-            ref_ind2 = ref_ind | ref_addon
-            print('N_ref: %i + %i -> %i .. ' % \
-                  (np.sum(ref_ind), np.sum(ref_addon), np.sum(ref_ind2)), end = '')
-        else:
-            #'''
-            ref_ind2 = ref_ind
-            print('N_ref: %i + X .. ' % (np.sum(ref_ind2)), end = '')
-    else:
-        ref_ind2 = ref_addon
-        print('N_ref: X + %i ..' % (np.sum(ref_ind2)), end = '')
-    #'''
-        
     dft, params = get_cnv_threshold_useref( df, ref_ind2, 
                                        score_key = score_key, cluster_key = cluster_key,
                                        th_min = th_min, refp_min = refp_min, p_exc = p_exc, 
                                        ucr = dec_margin, plot_stat = plot_stat, 
                                        suffix = suffix, Data = Data )
-    '''
-    else:
-        dft, params = get_cnv_threshold_bimodal( df, ref_ind, 
-                                        score_key = score_key, cluster_key = cluster_key, 
-                                        th_min = th_min, refp_min = refp_min, ucr = dec_margin,
-                                        plot_stat = plot_stat, suffix = suffix, Data = Data )
-    #'''
     
     etime = round(time.time() - start_time_a) 
     print('done (%i) ' % etime) #, end = '', flush = True)
     
-    return df, params, cobj
+    return df, params, cobj, X_pca
 
 
 def plot_td_stats( params, n_bins = 30, title = None, title_fs = 14,
                    label_fs = 12, tick_fs = 11, legend_fs = 11, 
                    legend_loc = 'upper left', bbox_to_anchor = (1, 1),
                    figsize = (4,3), log = True, alpha = 0.8 ):
     
@@ -1281,8 +897,8 @@
     if log: plt.yscale('log')
     ax.tick_params(axis='x', labelsize=tick_fs)
     ax.tick_params(axis='y', labelsize=tick_fs)
     plt.grid()
     plt.show()
         
     return 
-    
+
```

### Comparing `scoda-tk-0.2.3/src/scoda/misc.py` & `scoda-tk-0.2.4/src/scoda/misc.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.3/src/scoda/pipeline.py` & `scoda-tk-0.2.4/src/scoda/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,32 +98,34 @@
         if isinstance(ref_types, list):
             if len(ref_types) > 0:
                 ref_types2 = list(set(ref_types).intersection(adata.obs[ref_key].unique()))
                 ref_ind = adata.obs[ref_key].isin(ref_types)
     #'''
     adata = run_icnv(adata, ref_key, ref_types2, gtf_file, 
                      resolution = 2, N_pca = 15, n_neighbors = 10,
-                     cluster_key = 'cnv_leiden', umap = False,
+                     cluster_key = 'cnv_leiden', umap = False, pca = False,
                      n_cores = n_cores )
 
     #'''
-    # X_cnv = adata.obsm['X_cnv'].todense()
-    # pca = False
+    X_cnv = adata.obsm['X_cnv'].todense()
+    pca = False
 
-    X_cnv = adata.obsm['X_cnv_pca']
-    pca = True
+    # X_cnv = adata.obsm['X_cnv_pca']
+    # pca = True
 
-    df_res, params, cobj = detect_tumor_cells(X_cnv, ref_ind, pca = pca, 
+    df_res, params, cobj, X_pca = identify_tumor_cells(X_cnv, ref_ind, pca = pca, 
                            use_cnv_score = False, clust = None, 
                            Clustering_resolution = 1, N_clusters = 30,
                            gmm_N_comp = 20, th_min = 0, refp_min = 0.9, p_exc = 0.1, 
                            dec_margin = 0.05, n_neighbors = 15, cmd_cutoff = cmd_cutoff, 
                            gcm = gcm, plot_stat = False, use_ref = use_ref_only, 
                            suffix = '', Data = None, n_cores = n_cores)
 
+    if not pca: adata.obsm['X_cnv_pca'] = X_pca
+        
     adata_t.obsm['X_cnv'] = adata.obsm['X_cnv']
     adata_t.obsm['X_cnv_pca'] = adata.obsm['X_cnv_pca']
 
     # adata_t.obsm['X_cnv_umap'] = adata.obsm['X_cnv_umap']
     # adata_t.obs['cnv_leiden'] = adata.obs['cnv_leiden']
     # adata_t.obs['cnv_score'] = adata.obs['cnv_score']
     # adata_t.uns['cnv_neighbors'] = adata.uns['cnv_neighbors']
@@ -135,30 +137,30 @@
 
     adata_t.obs['cnv_cluster'] = list(df_res['cnv_cluster'].astype(str))
     adata_t.obs['tumor_dec'] = list(df_res['tumor_dec'])
     adata_t.obs['tumor_score'] = list(df_res['tumor_score'])
 
     adata_t.uns['cnv_ref_celltypes'] = ref_types2
     # adata_t.uns['cnv_clustering_obj'] = cobj
-    adata_t.uns['cnv_params'] = params
+    adata_t.uns['cnv_stats'] = params
 
     lst1 = list(df_res.index.values)
     lst2 = list(adata_t.obs.index.values)
     rend = dict(zip(lst1, lst2))
     df_res.rename(index = rend, inplace = True)
 
     adata_t.obsm['cnv_results'] = df_res[df_res.columns.values[:-1]] ## except tumor_cluster
 
     adata_t.obs['celltype_minor_rev'] = adata_t.obs['celltype_minor'].copy(deep = True).astype(str)
     b = (adata_t.obs['tumor_dec'] == 'Tumor')
     if ref_types is not None:
         b = b & (~adata_t.obs['celltype_major'].isin(ref_types))
     adata_t.obs.loc[b, 'celltype_minor_rev'] = 'Tumor cell'
 
-    return
+    return 
 
 
 def scoda_cci( adata_t, cpdb_path, cond_col = 'condition', sample_col = 'sample', 
                unit_of_cci_run = 'sample', min_n_cells_for_cci = 40, 
                data_dir = '.', pval_max = 0.1, mean_min = 0, Rth = 0.5, n_cores = 4,
                print_prefix = ''):
```

### Comparing `scoda-tk-0.2.3/src/scoda/viz.py` & `scoda-tk-0.2.4/src/scoda/viz.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.3/src/scoda_tk.egg-info/PKG-INFO` & `scoda-tk-0.2.4/src/scoda_tk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoda-tk
-Version: 0.2.3
+Version: 0.2.4
 Summary: Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Author-email: Seokhyun Yoon <syoon@dku.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `scoda-tk-0.2.3/src/scoda_tk.egg-info/SOURCES.txt` & `scoda-tk-0.2.4/src/scoda_tk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

