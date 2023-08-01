# Comparing `tmp/scibd-0.1.3.tar.gz` & `tmp/scibd-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scibd-0.1.3.tar", last modified: Tue Jan 31 06:27:36 2023, max compression
+gzip compressed data, was "scibd-1.0.0.tar", last modified: Tue Aug  1 16:26:34 2023, max compression
```

## Comparing `scibd-0.1.3.tar` & `scibd-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 yingwang  (1000) yingwang  (1000)        0 2023-01-31 06:27:36.054908 scibd-0.1.3/
--rw-r--r--   0 yingwang  (1000) yingwang  (1000)     1060 2023-01-18 09:22:20.000000 scibd-0.1.3/LICENSE
--rw-r--r--   0 yingwang  (1000) yingwang  (1000)       26 2023-01-18 09:22:20.000000 scibd-0.1.3/MANIFEST.in
--rw-r--r--   0 yingwang  (1000) yingwang  (1000)     2215 2023-01-31 06:27:36.054908 scibd-0.1.3/PKG-INFO
--rw-r--r--   0 yingwang  (1000) yingwang  (1000)     1537 2023-01-28 15:11:37.000000 scibd-0.1.3/README.md
--rw-r--r--   0 yingwang  (1000) yingwang  (1000)      238 2023-01-18 08:54:31.000000 scibd-0.1.3/README.rst
-drwxr-xr-x   0 yingwang  (1000) yingwang  (1000)        0 2023-01-31 06:27:36.054908 scibd-0.1.3/scibd/
--rw-r--r--   0 yingwang  (1000) yingwang  (1000)       21 2023-01-18 09:34:52.000000 scibd-0.1.3/scibd/__init__.py
--rw-r--r--   0 yingwang  (1000) yingwang  (1000)      352 2023-01-18 09:33:16.000000 scibd-0.1.3/scibd/__version__.py
--rw-r--r--   0 yingwang  (1000) yingwang  (1000)    27940 2023-01-28 13:00:41.000000 scibd-0.1.3/scibd/scibd.py
-drwxr-xr-x   0 yingwang  (1000) yingwang  (1000)        0 2023-01-31 06:27:36.054908 scibd-0.1.3/scibd.egg-info/
--rw-r--r--   0 yingwang  (1000) yingwang  (1000)     2215 2023-01-31 06:27:35.000000 scibd-0.1.3/scibd.egg-info/PKG-INFO
--rw-r--r--   0 yingwang  (1000) yingwang  (1000)      219 2023-01-31 06:27:36.000000 scibd-0.1.3/scibd.egg-info/SOURCES.txt
--rw-r--r--   0 yingwang  (1000) yingwang  (1000)        1 2023-01-31 06:27:35.000000 scibd-0.1.3/scibd.egg-info/dependency_links.txt
--rw-r--r--   0 yingwang  (1000) yingwang  (1000)        6 2023-01-31 06:27:35.000000 scibd-0.1.3/scibd.egg-info/top_level.txt
--rw-r--r--   0 yingwang  (1000) yingwang  (1000)       38 2023-01-31 06:27:36.054908 scibd-0.1.3/setup.cfg
--rw-r--r--   0 yingwang  (1000) yingwang  (1000)     5224 2023-01-31 06:25:02.000000 scibd-0.1.3/setup.py
+drwxr-xr-x   0 yingwang  (1000) yingwang  (1000)        0 2023-08-01 16:26:34.674943 scibd-1.0.0/
+-rw-r--r--   0 yingwang  (1000) yingwang  (1000)     1060 2023-01-18 09:22:20.000000 scibd-1.0.0/LICENSE
+-rw-r--r--   0 yingwang  (1000) yingwang  (1000)       26 2023-01-18 09:22:20.000000 scibd-1.0.0/MANIFEST.in
+-rw-r--r--   0 yingwang  (1000) yingwang  (1000)     2208 2023-08-01 16:26:34.674943 scibd-1.0.0/PKG-INFO
+-rw-r--r--   0 yingwang  (1000) yingwang  (1000)     1537 2023-01-28 15:11:37.000000 scibd-1.0.0/README.md
+-rw-r--r--   0 yingwang  (1000) yingwang  (1000)      238 2023-01-18 08:54:31.000000 scibd-1.0.0/README.rst
+drwxr-xr-x   0 yingwang  (1000) yingwang  (1000)        0 2023-08-01 16:26:34.674943 scibd-1.0.0/scibd/
+-rw-r--r--   0 yingwang  (1000) yingwang  (1000)       21 2023-01-18 09:34:52.000000 scibd-1.0.0/scibd/__init__.py
+-rw-r--r--   0 yingwang  (1000) yingwang  (1000)      352 2023-01-18 09:33:16.000000 scibd-1.0.0/scibd/__version__.py
+-rw-r--r--   0 yingwang  (1000) yingwang  (1000)    30373 2023-08-01 15:14:14.000000 scibd-1.0.0/scibd/scibd.py
+drwxr-xr-x   0 yingwang  (1000) yingwang  (1000)        0 2023-08-01 16:26:34.674943 scibd-1.0.0/scibd.egg-info/
+-rw-r--r--   0 yingwang  (1000) yingwang  (1000)     2208 2023-08-01 16:26:34.000000 scibd-1.0.0/scibd.egg-info/PKG-INFO
+-rw-r--r--   0 yingwang  (1000) yingwang  (1000)      219 2023-08-01 16:26:34.000000 scibd-1.0.0/scibd.egg-info/SOURCES.txt
+-rw-r--r--   0 yingwang  (1000) yingwang  (1000)        1 2023-08-01 16:26:34.000000 scibd-1.0.0/scibd.egg-info/dependency_links.txt
+-rw-r--r--   0 yingwang  (1000) yingwang  (1000)        6 2023-08-01 16:26:34.000000 scibd-1.0.0/scibd.egg-info/top_level.txt
+-rw-r--r--   0 yingwang  (1000) yingwang  (1000)       38 2023-08-01 16:26:34.674943 scibd-1.0.0/setup.cfg
+-rw-r--r--   0 yingwang  (1000) yingwang  (1000)     5217 2023-08-01 15:19:28.000000 scibd-1.0.0/setup.py
```

### Comparing `scibd-0.1.3/LICENSE` & `scibd-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scibd-0.1.3/PKG-INFO` & `scibd-1.0.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: scibd
-Version: 0.1.3
+Version: 1.0.0
 Summary: A doublet detetion tool for scCAS data. https://github.com/Ying-Lab/scIBD
 Home-page: https://github.com/Ying-Lab/scIBD/
 Author: Wenhao Zhang
-Author-email: 23220210156258@stu.xmu.edu.cn
+Author-email: zscotty@stu.xmu.edu.cn
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
```

### Comparing `scibd-0.1.3/README.md` & `scibd-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `scibd-0.1.3/scibd/scibd.py` & `scibd-1.0.0/scibd/scibd.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 # -*- coding: utf-8 -*-
 """
 Created on Wed Oct 20 14:49:41 2021
 
 @author: User
 """
-######final version
+######only calculate 1 round TF-IDF & record memory
 
 import sys
 import numpy as np
 import pandas as pd
+import anndata
 import scipy 
 import math
 from scipy import spatial
 import os
 import random
 import time
 import tracemalloc
+import multiprocessing as mp
 import psutil
-import anndata
 from sklearn import metrics
 from sklearn.decomposition import PCA
 from sklearn.preprocessing import MinMaxScaler
 import scipy.io as scio
 import umap
 import skbio
-import multiprocessing as mp
 from mpl_toolkits.mplot3d import axes3d
 from scipy import stats
 import seaborn as sns
 import scanpy as sc
 ###plt setting
 import warnings
 import matplotlib.pyplot as plt
@@ -37,31 +37,64 @@
 from sklearn.metrics.cluster import normalized_mutual_info_score
 from sklearn.metrics import roc_auc_score
 from sklearn.metrics import precision_recall_curve
 from sklearn.metrics import average_precision_score
 from sklearn.metrics import roc_curve, auc
 from sklearn import preprocessing
 from sklearn.metrics import calinski_harabasz_score
+from sklearn.feature_extraction.text import TfidfTransformer
 import matplotlib
 warnings.filterwarnings("ignore")
 random.seed(1111)
 np.random.seed(1111)
 
 
-def TF_IDF_Pro(count_mat):
-    nfreqs = (1.0 * count_mat / np.tile(np.sum(count_mat,axis=0), (count_mat.shape[0],1))).A
-    tfidf_mat = nfreqs * (np.tile(np.log(1 + 1.0 * count_mat.shape[1] / np.sum(count_mat,axis=1)).reshape(-1,1), (1,count_mat.shape[1]))).A
-    if np.sum(np.isnan(tfidf_mat) == True) != 0:
-        #print("The results of TF-IDF contain nan, replacing it with zero!")
-        tfidf_mat[np.isnan(tfidf_mat)] = 0 
-    if np.sum(np.isinf(tfidf_mat) == True) != 0:
-        print("The results of TF-IDF contain inf, replacing it with mean value!")
-        tfidf_mat = fill_ndarray(tfidf_mat)
-#     print('tf-idf done')
-    return scipy.sparse.csr_matrix(tfidf_mat.T)
+# def TF_IDF_Pro(count_mat):
+#     nfreqs = (1.0 * count_mat / np.tile(np.sum(count_mat,axis=0), (count_mat.shape[0],1))).A
+#     tfidf_mat = nfreqs * (np.tile(np.log(1 + 1.0 * count_mat.shape[1] / np.sum(count_mat,axis=1)).reshape(-1,1), (1,count_mat.shape[1]))).A
+#     if np.sum(np.isnan(tfidf_mat) == True) != 0:
+#         #print("The results of TF-IDF contain nan, replacing it with zero!")
+#         tfidf_mat[np.isnan(tfidf_mat)] = 0 
+#     if np.sum(np.isinf(tfidf_mat) == True) != 0:
+#         print("The results of TF-IDF contain inf, replacing it with mean value!")
+#         tfidf_mat = fill_ndarray(tfidf_mat)
+# #     print('tf-idf done')
+#     return scipy.sparse.csr_matrix(tfidf_mat.T)
+
+# Perform TF-IDF (count_mat: peak*cell)
+def TF_IDF_Pro(count_mat): 
+    
+    if not scipy.sparse.issparse(count_mat):
+        count_mat = scipy.sparse.coo_matrix(count_mat)
+        
+    nfreqs = count_mat.multiply(1.0 / count_mat.sum(axis=0))
+    tfidf_mat = nfreqs.multiply(np.log(1 + 1.0 * count_mat.shape[1] / count_mat.sum(axis=1)).reshape(-1,1)).tocoo()
+    
+    return tfidf_mat
+
+# def TF_IDF_Pro(count_mat): ##cell*peak
+#     model = TfidfTransformer(smooth_idf=False, norm="l2")
+#     model = model.fit(np.transpose(count_mat))
+#     model.idf_ -= 1
+#     tf_idf = np.transpose(model.transform(np.transpose(count_mat)))
+#     return scipy.sparse.csr_matrix(tf_idf)
+
+def CalJac(A,B=None):##scipy mat
+    A = A.astype(bool).astype(int)
+    if B is None:
+        B = A
+    else:
+        B = B.astype(bool).astype(int)
+    intersect = A.dot(B.T)
+    a_sum = A.sum(axis=1).A1
+    b_sum = B.sum(axis=1).A1
+    xx,yy = np.meshgrid(a_sum, b_sum)
+    union = ((xx+yy).T - intersect)
+    jac_distance = (1-intersect/union).A
+    return jac_distance
 
 def F1(score, label):
     assert len(score) == len(label)
     P  = len(label[label=='DOUB'])
     PP = len(score[np.all([score!= 0,score!= 0.05],axis = 0)]) #TP+FP
     TP = len(label[np.all([score!= 0,score!= 0.05],axis = 0)][label[np.all([score!= 0,score!= 0.05],axis = 0)]=='DOUB'])
     precision = TP/PP
@@ -80,15 +113,15 @@
 
 ## get clusters based on PCA+UMAP+DBSCAN 
 def GetCluster(mat):
     PCA_umap = GetUMAP(mat)
     PCA_umap = StandardScaler().fit_transform(PCA_umap) 
     
     distance = metrics.pairwise_distances(PCA_umap, Y=None, metric='euclidean', n_jobs=64)
-    Parameters ={'eps':0.1,'min_samples':mat.shape[0]*0.005}
+    Parameters ={'eps':0.1,'min_samples':int(mat.shape[0]*0.005)}
     db = DBSCAN(eps = Parameters['eps'], min_samples = Parameters['min_samples'],metric = 'precomputed').fit(distance) 
     cl = db.labels_
     return cl,distance
 
 def random_weight(i,weight_data):
     random.seed(i)
     total = sum(weight_data.values())    # 权重求和
@@ -110,32 +143,44 @@
     cl_score = np.array([]).reshape(0,mat.shape[1])
     for item in cl_uni:
         cl_score = np.vstack((cl_score,np.mean(mat[cl == item],axis = 0))).A
     var_peak = np.var(np.log2(cl_score+1),axis=0)
     idxbool = var_peak > np.quantile(var_peak,rate,interpolation='higher')
     return idxbool
 
-
+##import scipy
 def GetUMAP(mat):
     var_names = pd.DataFrame(np.array(range(mat.shape[1])), columns=['peak_names'])
     col_names = pd.DataFrame(np.array(range(mat.shape[0])), columns=['cell_names'])
-
-    adata = sc.AnnData(TF_IDF_Pro(mat.T),obs=col_names, var=var_names,)
+    adata = sc.AnnData(TF_IDF_Pro(mat.T).T,obs=col_names, var=var_names,)
+    ##this step used the former TF-IDF matrix
     adata.obs_names = col_names.cell_names
     adata.var_names = var_names.peak_names
     sc.tl.pca(adata, svd_solver='arpack')
     sc.pp.neighbors(adata, n_neighbors=30,n_pcs=30)
     sc.tl.umap(adata,min_dist=0.4)
     return adata.obsm['X_umap']
 
+##import scipy
+def GetSparseUnion(A, B = None):
+    if B is None:
+        B = A
+    intersect = A.dot(B.T)
+    A_sum = A.sum(axis=1).A1
+    B_sum = B.sum(axis=1).A1
+    xx,yy = np.meshgrid(A_sum,B_sum)
+    union = ((xx+yy).T - intersect)
+    return union
+
+##import scipy
 def CreateDoublets_Cluster_weighted(simulate_size, mat, distancemat, clusterlab):
 #     print('simulating start',simulate_size)
     np.random.seed(1111)
     assert simulate_size != 0
-    mat = scipy.sparse.csr_matrix(mat.astype(np.uint8))
+#     mat = scipy.sparse.csr_matrix(mat.astype(np.uint8))
     clusterlab = clusterlab.astype(str)     
     cluster_uniq = list(set(clusterlab))
 #     print(len(cluster_uniq), 'clusters')
 
     ####设置单个类大小权重dict
     cluster_weight = {}
     ####设置两类大小权重dict
@@ -154,69 +199,84 @@
     for item in cluster_weight:
         cluster_weight[item] = cw_st[idx]
         idx += 1 
         
     for item in cluster_bi_weight:
         cluster_bi_weight[item] = cluster_weight[item.split('_')[0]] * cluster_weight[item.split('_')[1]]
 
-    single1set = []
-    single2set = []
-    simulatelabel = []
+#     single1set = []
+#     single2set = []
+#     simulatelabel = []
     L1_size = int(simulate_size/3*2)
     ####若聚类只有1，全部随机
     
     if len(cluster_uniq) == 1:
         L1_size = 0 
     for i in range(L1_size):
 
         ramtype = random_weight(i,cluster_bi_weight).split('_')
         
         idx1 = np.random.choice(len(clusterlab[clusterlab == ramtype[0]]),1)
         idx2 = np.random.choice(len(clusterlab[clusterlab == ramtype[1]]),1)
-        single1set.append(mat[clusterlab == ramtype[0]][idx1].A)
-        single2set.append(mat[clusterlab == ramtype[1]][idx2].A)
+        try:
+            single1set = scipy.sparse.vstack((single1set,mat[clusterlab == ramtype[0]][idx1]))
+            single2set = scipy.sparse.vstack((single2set,mat[clusterlab == ramtype[1]][idx2]))
+        except:
+            single1set = mat[clusterlab == ramtype[0]][idx1]
+            single2set = mat[clusterlab == ramtype[1]][idx2]
+#         single1set.append(mat[clusterlab == ramtype[0]][idx1].A)
+#         single2set.append(mat[clusterlab == ramtype[1]][idx2].A)。
 #         doublet = scipy.sparse.csr_matrix(mat[clusterlab == ramtype[0]][idx1].A | mat[clusterlab == ramtype[1]][idx2].A)
 
     
     for i in range(simulate_size - L1_size):
 
         idxset = np.random.choice(mat.shape[0],2)
-        single1set.append(mat[idxset[0]].A)
-        single2set.append(mat[idxset[1]].A)
+        single1set = scipy.sparse.vstack((single1set,mat[idxset[0]]))
+        single2set = scipy.sparse.vstack((single2set,mat[idxset[1]]))
+#         single1set.append(mat[idxset[0]].A)
+#         single2set.append(mat[idxset[1]].A)
 #         doublet = scipy.sparse.csr_matrix(mat[clusterlab == ramtype[0]][idx1].A | mat[clusterlab == ramtype[1]][idx2].A)
 
-    single1set = np.array(single1set).squeeze().astype(np.uint8)
-    single2set = np.array(single2set).squeeze().astype(np.uint8)
-    sim_set = scipy.sparse.csr_matrix(single1set|single2set)
-    simulatelabel = np.array(simulatelabel)
+
+#     sim_set = GetSparseUnion(single1set,single2set)
+    sim_set = (single1set + single2set).astype(np.uint8)
+
+#     sim_set = scipy.sparse.csr_matrix(single1set|single2set)
+#     simulatelabel = np.array(simulatelabel)
     print(simulate_size,'Doublets Construction Done!')
+    print(sim_set.shape)
     return sim_set
 
 
+
+
 def Splitmat(matsize,ncore):
     idx_set =[]
 #     mat_size = mat.shape[0]
     size_scale = round(matsize/ncore)
     for i in range(ncore-1):
         idx_set.append(list(range(i*size_scale,(i+1)*size_scale)))
     idx_set.append(list(range((ncore-1)*size_scale, matsize)))
     return idx_set
 
 
+##import csr
 def ReshapeJac(mat_conc,label_conc,jac_raw,core):
 #     print('reshape jaccard')
     A = mat_conc[label_conc != 1]  
     B = mat_conc[label_conc == 1]
     ###判断是不是simulated doublets
-    jac_extra = metrics.pairwise_distances(B.A, Y=mat_conc.A, metric='jaccard', n_jobs=core)
+#     jac_extra = metrics.pairwise_distances(B.A, Y=mat_conc.A, metric='jaccard', n_jobs=core)
+    jac_extra = CalJac(B,mat_conc)
     jac_new = np.vstack((jac_raw, jac_extra[:,0:A.shape[0]]))
     jac_new = np.hstack((jac_new,jac_extra.T))
 
-    for i in range(len(jac_new)):
-        assert jac_new[i][i] == 0 
+#     for i in range(len(jac_new)):
+#         assert jac_new[i][i] == 0 
     return jac_new
 
 def PCoA(mat_jaccard,npc,showfig=False):
 
 #     mat_jaccard = Jaccard_Index(mat)
     OrdinationResults = skbio.stats.ordination.pcoa(mat_jaccard, method='eigh', number_of_dimensions=0, inplace=False)
     return np.array(OrdinationResults.samples)[:,0:npc]
@@ -231,14 +291,15 @@
     ####先对未被分类的细胞做聚类，基于原始的jaccard；label_refer为0或0.05 
     mat_unlabel = mat[np.any([label_refer == 0, label_refer == 0.05],axis = 0)]
     jac_unlabel = jac[np.any([label_refer == 0, label_refer == 0.05],axis = 0)][:,np.any([label_refer == 0, label_refer == 0.05],axis = 0)]
     cl_refer = label_refer[np.any([label_refer == 0, label_refer == 0.05],axis = 0)]
     cl, cd = GetCluster(mat_unlabel)
     #######在这一步决定simsize，为未分类样本数的10% - 40% 
     sim_size = int(sim_rate * mat_unlabel.shape[0])
+    time_start = time.time()
     simDOU = CreateDoublets_Cluster_weighted(sim_size, mat_unlabel,cd,cl)
     mat_concat = scipy.sparse.vstack((mat,simDOU)).astype(np.uint8)
     label_refer[label_refer==0.05] = 0
     label_concat = np.hstack((label_refer,np.array([1]*sim_size))).astype(np.float64)
 
     return mat_concat,label_concat
 
@@ -411,17 +472,17 @@
 def CallDoublet_PCA(iteration, mat, sim, jac, core, npc, k, n_tree,label_refer,labelmat):
     time1 = time.time()
     mat_concat, label_concat = concat_set(iteration, jac, mat,sim,label_refer)
     ####label_concat只包含{0:unlabel; 0-1:predicted doublets; 1:simulated doublets}
     ###mat_concat所有细胞+sim
     ###label_concat 带标记的raw(0 /3)+ sim(1) 
     
-    mat_inuse = GetUMAP(mat_concat)
+    distance_inuse = GetUMAP(mat_concat)
     ###k为构建knn图时所用的邻居节点default
-    knn,distance = get_knn_graph(mat_inuse, k, n_tree)
+    knn,distance = get_knn_graph(distance_inuse, k, n_tree)
     
     ####3 parts: 1. 未标记unlabel； 2.已标记detected; 3.simulated 
     cells_unlabel_knn = knn[label_concat==0]
     cells_sim_knn = knn[label_concat==1]
     cells_detected_knn = knn[np.all([label_concat!=0, label_concat !=1],axis =0)]
     
     cells_unlabel_distance = distance[label_concat==0]
@@ -448,25 +509,25 @@
         score_detected = CalKNNScore(cells_detected_knn,cells_detected_distance,np.min(distance),np.max(distance),label_concat)
         score_detected = pd.DataFrame(score_detected)
         score_detected.index = cell_detected_idx 
 
     return score_unlabel,score_sim,score_detected
 
 def CallDoublet_PCoA(iteration, mat, sim, jac, core, npc, k, n_tree,label_refer,labelmat):
-
     mat_concat, label_concat = concat_set(iteration, jac, mat,sim,label_refer)
     ####label_concat只包含{0:unlabel; 0-1:predicted doublets; 1:simulated doublets}
     ###mat_concat所有细胞+sim
     ####基于重构的mat，计算原始细胞与新的doublet之间的关系
     ###只需计算新的simulated 与 raw 的jaccard
     mat_jaccard = ReshapeJac(mat_concat, label_concat, jac, core)
+#     mat_jaccard = CalJac(mat_concat)
+
     ##PCoA_ased
     mat_inuse = PCoA(mat_jaccard,npc)
 
-
     ###k为构建knn图时所用的邻居节点default
     knn,distance = get_knn_graph(mat_inuse, k, n_tree)
     
     ####3 parts: 1. 未标记unlabel； 2.已标记detected; 3.simulated 
     cells_unlabel_knn = knn[label_concat==0]
     cells_sim_knn = knn[label_concat==1]
     cells_detected_knn = knn[np.all([label_concat!=0, label_concat !=1],axis =0)]
@@ -490,26 +551,26 @@
     ###返回pd格式 的unlabelled cell score
     if len(cells_detected_knn) == 0:
         score_detected = pd.DataFrame(np.array([]))
     else:
         score_detected = CalKNNScore(cells_detected_knn,cells_detected_distance,np.min(distance),np.max(distance),label_concat)
         score_detected = pd.DataFrame(score_detected)
         score_detected.index = cell_detected_idx
-
     return score_unlabel,score_sim,score_detected
 
 
 
 def GetStrategy(mat,jac):
-    PCA_umap = GetUMAP(scipy.sparse.csr_matrix(mat))
+#     PCA_umap = GetUMAP(scipy.sparse.csr_matrix(mat))
+    PCA_umap = GetUMAP(mat)
 #     PCA_umap = MinMaxScaler().fit_transform(PCA_umap) 
     PCA_umap = StandardScaler().fit_transform(PCA_umap) 
 #     distance = metrics.pairwise_distances(PCA_umap, Y=None, metric='euclidean', n_jobs=64)
     ##adjusted
-    Parameters ={'eps':0.1,'min_samples':mat.shape[0]*0.005}
+    Parameters ={'eps':0.1,'min_samples':int(mat.shape[0]*0.005)}
     db1 = DBSCAN(eps = Parameters['eps'], min_samples = Parameters['min_samples'], metric = 'euclidean').fit(PCA_umap) 
     cl_PCA = db1.labels_
 
     try:
         chs1 = calinski_harabasz_score(PCA_umap,cl_PCA)
     except:
         chs1 = 0.0001
@@ -532,25 +593,26 @@
     else:
         strategy = 'PCoA'
     print(strategy)
     return strategy
 
 ###define main function here
 class KNNIter(object):
-    def __init__(self, rawmat, strategy = None, core = None, sim_rate= None, nPC=None, neighbors=None, nTree=None, label= None, exprate = None):
-        ##preprocess1, select the peaks that are open in more than 1% cells
+    def __init__(self, rawmat, strategy = None, core = None, sim_rate= None, nPC=None, neigbors=None, nTree=None, label= None, exprate = None):
         if isinstance(rawmat, anndata.AnnData):
-            ##判断是否是adata格式输入
-            rawmat_ann = rawmat
-            rawmat = rawmat.X
-            
+            self.rawmat_ann = rawmat
+            rawmat = rawmat.X 
         else:
-            rawmat = rawmat
+            self.rawmat_ann = None
+            rawmat = rawmat   
+        ##preprocess1, select the peaks that are open in more than 1% cells
+        ## transfer to scipy
+        rawmat = scipy.sparse.csr_matrix(rawmat).astype(np.uint8)
         rawmat_pf = rawmat[:,(rawmat.sum(axis = 0)> 0.01* rawmat.shape[0]).A.squeeze()]
-#         print(rawmat_pf.shape)
+        print(rawmat_pf.shape)
         self.rawmat = rawmat
         self.fmat = rawmat_pf
         
         ###csr matrix
         self.core_max = mp.cpu_count()
         
         if core is None:
@@ -563,76 +625,80 @@
             self.sim_rate = 0.3
         else:
             self.sim_size = sim_size
         if nPC is None:
             self.nPC = 5
         else:
             self.nPC = nPC
-        if neighbors is None:
-            self.neighbors = 40
+        if neigbors is None:
+            self.neigbors = 40
         else:
-            self.neighbors = neighbors
+            self.neigbors = neigbors
         if nTree is None:
             self.nTree = 30
         else:
             self.nTree = nTree   
         if label is None:
             self.label = np.array(range(self.rawmat.shape[0]))
         else:
             self.label = label
         if exprate is None:
             self.exprate = 0.1
         else:
             self.exprate = exprate
         ##jaccard distance mat of raw set
-        self.jac = metrics.pairwise_distances(self.rawmat.A, Y=None, metric='jaccard', n_jobs=self.core)
+        time0 = time.time()
+#         self.jac = metrics.pairwise_distances(self.rawmat.A, Y=None, metric='jaccard', n_jobs=self.core)
+        self.jac = CalJac(self.rawmat)
+
+        print('raw jaccard cal: ',time1-time0)
         if strategy is None:
             print('evaluating the input data!')
             self.strategy = GetStrategy(self.rawmat,self.jac)
         else:
             self.strategy = strategy
     def IterCall(self, mat=None, strategy=None, core=None, simrate=None, npc=None, k=None, n_tree=None, labelmat=None, exprate=None):
 # #     def IterCall(mat=self.rawmat, strategy=self.strategy, core=self.core, simrate=self.sim_rate, npc=self.nPC, k=self.neigbors, n_tree=self.nTree, labelmat=self.label, exprate=self.exprate):
 #     def IterCall(self):
-        
         if mat is None:
             mat = self.fmat 
         if isinstance(mat, np.ndarray):
             mat = scipy.sparse.csr_matrix(mat)
         if strategy is None:
             strategy = self.strategy
         if core is None:
             core = self.core_max
         if simrate is None:
             simrate = self.sim_rate
         if npc is None:
             npc = self.nPC
         if k is None:
-            k = self.neighbors
+            k = self.neigbors
         if n_tree is None:
             n_tree = self.nTree
         if labelmat is None:
             labelmat = self.label
         if exprate is None:
             exprate = self.exprate
 
-#         time1 = time.time()
+        time_start = time.time()
         ###原始数据的jaccard
         jaccard_raw = self.jac
         ###参与KNN计算
         label_refer = np.zeros(mat.shape[0]).astype(np.float64)
         ###控制迭代
         loopproba = 10
         iteration = 1
         ###保存每一轮的分数
         score_pool = np.array([]).reshape(-1,mat.shape[0])
         random.seed(2222)
         ####
         while random.sample([1]*loopproba+[0]*(10-loopproba),1)[0]:
             print('Iteration',iteration, 'start')
+#             time_iter_start = time.time()
             if strategy == 'PCA':
                 score_unlabel, score_sim, score_detected = CallDoublet_PCA(iteration, mat, simrate, jaccard_raw, core, npc, k, n_tree,label_refer,labelmat)
 
             else:
                 score_unlabel, score_sim, score_detected = CallDoublet_PCoA(iteration, mat, simrate, jaccard_raw, core, npc, k, n_tree,label_refer,labelmat)
     
             ##当前轮次的分数
@@ -679,26 +745,27 @@
             
             #####labelrefer不为0(从未被预测为doublets)和0.05(被预测为doublets后又被reject)
             pred_doub = label_refer[np.all([label_refer!=0,label_refer!=0.05],axis=0)]
 #             print(len(pred_doub),'cells have been detected')
             ####加上这轮预测的减去这轮拒绝后的数量达到expect，开启退火
             if len(pred_doub) > int(exprate * mat.shape[0]*0.9):
                 loopproba -= int(np.ceil(5/iteration))  
-#             print('Iteraion', iteration, 'elapse', time.time()-time_iter)
+#             print('Iteraion', iteration, 'elapse', time.time()-time_iter_start)
             iteration += 1
         
         proba_final = np.mean(score_pool,axis = 0)
         min_max_scaler = MinMaxScaler( )
         proba_final = min_max_scaler.fit_transform(proba_final.reshape(-1, 1)).squeeze()
         thresh_final = np.quantile(proba_final,1-exprate,interpolation= 'higher')
-        ####如果是ann格式输入，返回一个ann;如果是numpy输入，返回predicted doublet序号及doublet score
-        try:
-            rawmat_ann
+        print('Done')
+        time_final = time.time()
+        print('ALL time:', time_final - time_start)
+        if self.rawmat_ann is None:
+            return labelmat[proba_final > thresh_final],proba_final
+        else:
+#             print('ann')
             pred_results = np.zeros(proba_final.shape[0])
             pred_results[proba_final > thresh_final] = 1
-            rawmat_ann.obs['PredDBL'] = pred_results
-            rawmat_ann.obs['DBLscore'] = proba_final
-            return rawmat_ann
-        except:
-            return labelmat[proba_final > thresh_final],proba_final
-
+            self.rawmat_ann.obs['PredDBL'] = pred_results
+            self.rawmat_ann.obs['DBLscore'] = proba_final
+            return self.rawmat_ann
```

### Comparing `scibd-0.1.3/scibd.egg-info/PKG-INFO` & `scibd-1.0.0/scibd.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: scibd
-Version: 0.1.3
+Version: 1.0.0
 Summary: A doublet detetion tool for scCAS data. https://github.com/Ying-Lab/scIBD
 Home-page: https://github.com/Ying-Lab/scIBD/
 Author: Wenhao Zhang
-Author-email: 23220210156258@stu.xmu.edu.cn
+Author-email: zscotty@stu.xmu.edu.cn
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
```

### Comparing `scibd-0.1.3/setup.py` & `scibd-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,18 +55,18 @@
 
 from setuptools import find_packages, setup, Command
 
 # Package meta-data.
 NAME = 'scibd'
 DESCRIPTION = 'A doublet detetion tool for scCAS data. https://github.com/Ying-Lab/scIBD'
 URL = 'https://github.com/Ying-Lab/scIBD/'
-EMAIL = '23220210156258@stu.xmu.edu.cn'
+EMAIL = 'zscotty@stu.xmu.edu.cn'
 AUTHOR = 'Wenhao Zhang'
 REQUIRES_PYTHON = '>=3.8.0'
-VERSION = '0.1.3'
+VERSION = '1.0.0'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
```

