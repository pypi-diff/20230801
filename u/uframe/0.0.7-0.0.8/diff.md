# Comparing `tmp/uframe-0.0.7.tar.gz` & `tmp/uframe-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uframe-0.0.7.tar", last modified: Mon Jul 24 11:12:34 2023, max compression
+gzip compressed data, was "uframe-0.0.8.tar", last modified: Tue Aug  1 11:51:39 2023, max compression
```

## Comparing `uframe-0.0.7.tar` & `uframe-0.0.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 11:12:34.880882 uframe-0.0.7/
--rw-rw-rw-   0        0        0     1090 2023-07-11 11:16:34.000000 uframe-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     5081 2023-07-24 11:12:34.880882 uframe-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     4479 2023-07-11 11:16:34.000000 uframe-0.0.7/README.md
--rw-rw-rw-   0        0        0     1055 2023-07-24 11:02:02.000000 uframe-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0      462 2023-07-24 11:12:34.880882 uframe-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      223 2023-07-20 12:52:29.000000 uframe-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-24 11:12:34.837648 uframe-0.0.7/src/
-drwxrwxrwx   0        0        0        0 2023-07-24 11:12:34.865181 uframe-0.0.7/src/uframe/
--rw-rw-rw-   0        0        0      583 2023-07-21 13:40:49.000000 uframe-0.0.7/src/uframe/__init__.py
--rw-rw-rw-   0        0        0    60935 2023-07-21 13:39:57.000000 uframe-0.0.7/src/uframe/uframe.py
--rw-rw-rw-   0        0        0     6880 2023-07-24 08:36:56.000000 uframe-0.0.7/src/uframe/uframe_from_mice.py
--rw-rw-rw-   0        0        0    12958 2023-07-24 06:43:12.000000 uframe-0.0.7/src/uframe/uframe_instance.py
--rw-rw-rw-   0        0        0      123 2023-07-21 13:40:05.000000 uframe-0.0.7/src/uframe/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-24 11:12:34.880882 uframe-0.0.7/src/uframe.egg-info/
--rw-rw-rw-   0        0        0     5081 2023-07-24 11:12:34.000000 uframe-0.0.7/src/uframe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      429 2023-07-24 11:12:34.000000 uframe-0.0.7/src/uframe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 11:12:34.000000 uframe-0.0.7/src/uframe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-20 07:40:14.000000 uframe-0.0.7/src/uframe.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      142 2023-07-24 11:12:34.000000 uframe-0.0.7/src/uframe.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-24 11:12:34.000000 uframe-0.0.7/src/uframe.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-24 11:12:34.880882 uframe-0.0.7/tests/
--rw-rw-rw-   0        0        0      224 2023-07-11 11:16:34.000000 uframe-0.0.7/tests/test_uframe.py
--rw-rw-rw-   0        0        0     2703 2023-07-11 11:16:34.000000 uframe-0.0.7/tests/test_uframe_instance.py
+drwxrwxrwx   0        0        0        0 2023-08-01 11:51:39.080892 uframe-0.0.8/
+-rw-rw-rw-   0        0        0     1090 2023-07-11 11:16:34.000000 uframe-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     5081 2023-08-01 11:51:39.080892 uframe-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     4479 2023-07-11 11:16:34.000000 uframe-0.0.8/README.md
+-rw-rw-rw-   0        0        0     1055 2023-07-26 11:56:43.000000 uframe-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0      462 2023-08-01 11:51:39.082891 uframe-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      223 2023-07-20 12:52:29.000000 uframe-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 11:51:39.011892 uframe-0.0.8/src/
+drwxrwxrwx   0        0        0        0 2023-08-01 11:51:39.051893 uframe-0.0.8/src/uframe/
+-rw-rw-rw-   0        0        0      583 2023-07-21 13:40:49.000000 uframe-0.0.8/src/uframe/__init__.py
+-rw-rw-rw-   0        0        0    50775 2023-07-26 12:41:19.000000 uframe-0.0.8/src/uframe/uframe.py
+-rw-rw-rw-   0        0        0     6880 2023-07-24 08:36:56.000000 uframe-0.0.8/src/uframe/uframe_from_mice.py
+-rw-rw-rw-   0        0        0    12958 2023-07-24 06:43:12.000000 uframe-0.0.8/src/uframe/uframe_instance.py
+-rw-rw-rw-   0        0        0      123 2023-07-21 13:40:05.000000 uframe-0.0.8/src/uframe/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-01 11:51:39.066892 uframe-0.0.8/src/uframe.egg-info/
+-rw-rw-rw-   0        0        0     5081 2023-08-01 11:51:38.000000 uframe-0.0.8/src/uframe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      429 2023-08-01 11:51:38.000000 uframe-0.0.8/src/uframe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 11:51:38.000000 uframe-0.0.8/src/uframe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-20 07:40:14.000000 uframe-0.0.8/src/uframe.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      142 2023-08-01 11:51:38.000000 uframe-0.0.8/src/uframe.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-08-01 11:51:38.000000 uframe-0.0.8/src/uframe.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 11:51:39.079893 uframe-0.0.8/tests/
+-rw-rw-rw-   0        0        0      224 2023-07-11 11:16:34.000000 uframe-0.0.8/tests/test_uframe.py
+-rw-rw-rw-   0        0        0     2703 2023-07-11 11:16:34.000000 uframe-0.0.8/tests/test_uframe_instance.py
```

### Comparing `uframe-0.0.7/LICENSE` & `uframe-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `uframe-0.0.7/PKG-INFO` & `uframe-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uframe
-Version: 0.0.7
+Version: 0.0.8
 Summary: Package for handling uncertain data
 Author: Christian Amesoeder and Michael Hagn
 Author-email: Christian Amesoder <christian.amesoeder@informatik.uni-regensburg.de>, Michael Hagn <michael.hagn@stud.uni-regensburg.de>
 Project-URL: Homepage, https://github.com/URWI2/uframe
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `uframe-0.0.7/README.md` & `uframe-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `uframe-0.0.7/pyproject.toml` & `uframe-0.0.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 warn_unreachable = true
 warn_unused_configs = true
 no_implicit_reexport = true
 
 
 [project]
 name = "uframe"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Christian Amesoder", email="christian.amesoeder@informatik.uni-regensburg.de" },
   { name="Michael Hagn", email="michael.hagn@stud.uni-regensburg.de" }
 ]
 description = "Package for handling uncertain data"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `uframe-0.0.7/src/uframe/__init__.py` & `uframe-0.0.8/src/uframe/__init__.py`

 * *Files identical despite different names*

### Comparing `uframe-0.0.7/src/uframe/uframe.py` & `uframe-0.0.8/src/uframe/uframe.py`

 * *Files 13% similar despite different names*

```diff
@@ -74,33 +74,26 @@
         Append new rows to the data which can be either certain or uncertain.
         In place. New rows have to be numpy arrays at first, later add
         different sources of uncertain new rows.
 
 
     """
 
-    def __init__(self):
+    def __init__(self,  new = None, colnames = None, rownames = None):
 
         self.data = []
         self._columns = []
         self._colnames = {}
         self._rows = []
         self._rownames = {}
         self._col_dtype = []
 
-        return
+        if new is not None: 
+            self.append(new = new, colnames = colnames, rownames = rownames)
 
-        """  
-        def mean_dev(true_data): 
-            ev = self.ev() 
-            mode = self.mode()
-            
-            for i in range(self.data):
-                """        
-            
             
             
             
    
     def analysis(self, true_data, save = False, **kwargs): 
         
         if save is not False:
@@ -256,15 +249,18 @@
             # Fall, wo Liste von Listen von 1D Distribs übergeben wird
             # checke, dass hier keine kategorischen Verteilungen übergeben werden
             elif isinstance(new[0], list):
                 if len(new[0]) > 0 and not isinstance(new[0][0], dict):
                     self.append_from_rv_cont(new, colnames)
                 elif len(new[0]) > 0 and isinstance(new[0][0], dict):
                     self.append_from_categorical(new, colnames)
-
+        
+        else: 
+            raise ValueError("Unknown type of new")
+            
         # sollte evtl. lieber die rownames in jeder append Funktion gesondert adressieren
         if isinstance(new, np.ndarray):
             return
         elif not isinstance(new, list):
             self.addRownames([new], rownames)
         elif isinstance(new[0], np.ndarray):
             self.addRownames(new[0], rownames)
@@ -1049,37 +1045,30 @@
         #if not, append new keys with them and give them the correct index 
         
         
         return 
             
     
     def __getitem__(self, index):
-        return self.data[index]
+        return uframe(new = self.data[index], colnames = self._columns, rownames = self._rows[index])
 
     # TO DO: function which takes i,j and returns element of uframe (need marginal distributions for that)
 
     def add_cat_values(self, cat_value_dict):
         
         if hasattr(self, 'cat_values'):
             self.cat_values.update(cat_value_dict)
         else:
             self.cat_values = cat_value_dict
         
         self.update_cat_value_dicts()
         
         return 
     
-    #Funktion, die automatisch cat valuesbestimmt (oder aus cat value dict übernimmt) und dict mit Codierung macht
-    #falls die Werte Integer sind, ist einfach {i:i für alle i} das dict 
-    #update Funktion benötigt, die am Ende von append aufgerufen wird 
-    #self cat value code dict muss an uframe instances übergeben werden 
-    #damit dann auch die label encoder Geschichten ersetzen!
-    
-    #neue get dummies Funktion, die gleich ein array nimmt, später dann die bisherige Version anpassen 
-    
+     
     def save(self, name="saved_uframe.pkl"):
             
         with open(name, 'wb') as f:
             pickle.dump(self,f)
         return 
      
 
@@ -1089,324 +1078,19 @@
     new_q = np.array([sum(preds[k]<true)/len(true) for k in range(len(true))])
 
     return [["Var",str(round(np.var(residues),2))],
             ["MAE", str(round(np.mean(np.abs(residues)),2))],
             ["RMSE", str(round(np.sqrt(np.mean(residues**2)),2))],
             ["Diff Quantile", str(round(np.mean(np.abs(true_q - new_q)),2))]]
             
-       
-
-
-        
-# takes np array, randomly picks percentage of values p and introduces uncertainty there
-# allow different kernels for the values given by mice, then use the mixed distr append function
-# allow scipy or sklearn kernels
-# one multidimensional kernel is fitted for each row with missing values
-def uframe_from_array_mice(a: np.ndarray, p=0.1, mice_iterations=5, kernel="stats.gaussian_kde",
-                           scaler= "min_max"):
-
-    x, missing = generate_missing_values(a, p)
-
-    distr = {}
-
-    # train mice imputation correctly
-    kds = mf.ImputationKernel(
-        x,
-        save_all_iterations=True,
-        random_state=100)
-
-    kds.mice(mice_iterations)
-    for i in range(x.shape[0]):
-        # print("Line", i)
-        imp_distr = None
-        imp_arrays = []
-        for j in range(x.shape[1]):
-            if np.isnan(x[i, j]):
-                #diese Schleife durch list comprehension ersetzen 
-                imp_values = []
-
-               
-                for k in range(mice_iterations):
-                    imput_x = kds.complete_data(iteration=k)
-                    imp_values.append(imput_x[i, j])
-
-                imp_value_arr = np.array(imp_values).reshape((1, mice_iterations))
-                imp_arrays.append(imp_value_arr)
-
-        if len(imp_arrays) == 0:
-            continue
-        
-        
-        # for i, arr in enumerate(imp_arrays):
-        #     scaler= MinMaxScaler()
-        #     arr = scaler.fit_transform(arr)
-        #     imp_arrays[i]= arr
-        
-        # print("Imp arrays after scaling")
-        
-        imp_array = np.concatenate(imp_arrays, axis=0)
-        scaler = MinMaxScaler()
-        imp_array = (scaler.fit_transform(imp_array.T)).T
-        #print("Shape of imp array", imp_array.shape)
-
-        if kernel == "stats.gaussian_kde":
-            kde = stats.gaussian_kde(imp_array)
-
-        else:
-            imp_array = imp_array.T
-            kde = KernelDensity(kernel=kernel, bandwidth=1.0).fit(imp_array)
-            #print("Dimension of kde", kde.n_features_in_)
-
-        imp_distr = kde
-
-        distr[i] = imp_distr
 
+if __name__ == "__main__":
+   
     
-    scaler= MinMaxScaler()
-    x = scaler.fit_transform(x)
-    #a[missing==1]=np.nan
-    u = uframe()
-    u.append(new=[x, distr])
+   
+   import scipy.stats as ss  
+   a = uframe(new = [ss.norm(1), ss.norm(10), ss.norm(112)])
+   a[0:1].sample()
     
-
-    return u
-
-#all columns in cat_indices are treated as categoricals: the mice results are used to calculate probs
-#später das als einzige Version der mice Funktion behalten 
-def uframe_from_array_mice_2(a: np.ndarray, p=0.1, mice_iterations=5, kernel="stats.gaussian_kde",
-                           scaler= "min_max", cat_indices=[]):
-
-    x, missing = generate_missing_values(a, p)
-
-    distr = {}
-    cat_distr = {}
-    index_dict={}
-
-    # train mice imputation correctly
-    kds = mf.ImputationKernel(
-        x,
-        save_all_iterations=True,
-        random_state=100)
-
-    kds.mice(mice_iterations)
-    for i in range(x.shape[0]):
-        # print("Line", i)
-        imp_distr = None
-        imp_arrays = []
-        cat_distributions = []
-        for j in range(x.shape[1]):
-            if np.isnan(x[i, j]) and j not in cat_indices:
-
-                imp_values = []
-
-                for k in range(mice_iterations):
-                    imput_x = kds.complete_data(iteration=k)
-                    imp_values.append(imput_x[i, j])
-
-                imp_value_arr = np.array(imp_values).reshape((1, mice_iterations))
-                imp_arrays.append(imp_value_arr)
-                
-                if i in index_dict.keys():
-                    index_dict[i][0].append(j)
-                else:
-                    index_dict[i]=[[j], []]
-                
-            if np.isnan(x[i,j]) and j in cat_indices:
-                
-                imp_values = []
-                for k in range(mice_iterations):
-                    imput_x = kds.complete_data(iteration=k)
-                    imp_values.append(imput_x[i,j])
-                
-                d={}
-                for imp_value in imp_values:
-                    if imp_value in d.keys():
-                        d[int(imp_value)]+= 1/mice_iterations
-                    else:
-                        d[int(imp_value)] = 1/mice_iterations 
-                        
-                cat_distributions.append(d)
-                
-                if i in index_dict.keys():
-                    index_dict[i][1].append(j)
-                else:
-                    index_dict[i]=[[],[j]]
-                
-            cat_distr[i]= cat_distributions
-            
-        if len(imp_arrays) == 0:
-            continue
-        
-        imp_array = np.concatenate(imp_arrays, axis=0)
-        scaler = MinMaxScaler()
-        imp_array = (scaler.fit_transform(imp_array.T)).T
-        #print("Shape of imp array", imp_array.shape)
-
-        if kernel == "stats.gaussian_kde":
-            kde = stats.gaussian_kde(imp_array)
-
-        else:
-            imp_array = imp_array.T
-            kde = KernelDensity(kernel=kernel, bandwidth=1.0).fit(imp_array)
-            #print("Dimension of kde", kde.n_features_in_)
-
-        imp_distr = kde
-
-        distr[i] = imp_distr
-
-    #print(x)
-    cont_indices = [i for i in range(x.shape[1]) if i not in cat_indices]
-    #print("Cont indices")
-    scaler= MinMaxScaler()
-    x_cont = scaler.fit_transform(x[:,cont_indices])
-    #print("X cont scaled", x_cont)
-    x[:,cont_indices]=x_cont
-    #print("X after scaling", x, x[:,cat_indices])
-    #a[missing==1]=np.nan
-    u = uframe()
     
-    #print("Cat distr", cat_distr)
-    u.append(new=[x, distr, cat_distr, index_dict])
-
-    #print("Col dtype", u._col_dtype)
-    return u
-
-
-# add Gaussian noise of given std to chosen entries
-# relative=True: multiply std with standard deviation of the column to get the std for a column
-def uframe_noisy_array(a: np.ndarray, std=0.1, relative=False, unc_percentage=0.1):
-
-    if relative:
-        #print("Get standard deviations of each column")
-        stds = std * np.std(a, axis=1)
-    else:
-        stds = np.repeat(std, a.shape[1])
-
-    print(stds)
-
-    # delete unc_percentage of all values
-    x, missing = generate_missing_values(a, unc_percentage)
-
-    print(x, missing)
-    # create suitable dictionary of distributions
-    distr = {}
-    for i in range(x.shape[0]):
-        if np.any(np.isnan(x[i, :])) == False:
-            continue
-        mean = a[i, :][np.where(np.isnan(x[i, :]))[0]]
-        cov = np.diag([stds[np.where(np.isnan(x[i, :]))[0]]])
-
-        print(mean, cov)
-
-        distr[i] = scipy.stats.multivariate_normal(mean=mean, cov=cov)
-
-    # generate uframe und use append function and return it
-    u = uframe()
-    u.append(new=[x, distr])
-
-    return u
-
-
-def generate_missing_values(complete_data, p):
-    shape = complete_data.shape
-    y = complete_data.copy()
-    missing = np.random.binomial(1, p, shape)
-    
-    y[missing.astype('bool')] = np.nan
-    return y, missing
-
-
-if __name__ == "__main__":
-    a = uframe()
-
-    def measure(n):
-        m1 = np.random.normal(size=n)
-        m2 = np.random.normal(scale=0.5, size=n)
-        return m1 + m2, m1 - m2
-
-    m1, m2 = measure(2000)
-    m1, m2 = measure(2000)
-    values = np.vstack([m1, m2])
-    kernel = stats.gaussian_kde(values)
-
-    kernel_list = [kernel]
-
-    b = uframe()
-    b.append(kernel_list)
-    print(b.sample(n=8))
-    print(b.mode())
-    b.append(new=np.identity(2))
-    uframe_i = b.data[1]
-    print(type(uframe_i))
-    b.append([uframe_i])
-
-    b.append_from_samples([values, values, values], kernel='tophat')
-    print(len(b.data))
-    b.append(new=kernel_list)
-    b.append([uframe_i])
-
-    print(len(b.data))
-
-    c = uframe()
-    c_array = np.array([[1, np.nan, 3], [np.nan, np.nan, 2]])
-
-    kernel2 = stats.gaussian_kde(m1)
-
-    kernel3 = KernelDensity(kernel='gaussian', bandwidth=1.0).fit(values.T)
-
-    distr1 = scipy.stats.norm()
-
-    distr2 = scipy.stats.multivariate_normal()
-    # c.append_from_mix_with_distr(certain=c_array, distr={0: kernel2, 1:kernel3})
-
-    d = uframe()
-    d.append_from_rv_cont([distr1])
-    d.append([distr1])
-    d.append(distr2)
-    d.append_from_rv_cont([[distr1], distr1])
-
-    e = uframe()
-
-    mv = scipy.stats.multivariate_normal(mean=np.array([1, 1]))
-    mv2 = scipy.stats.multivariate_normal(mean=np.array([1, 1, 1]))
-
-    # e.append_from_rv_cont([mv2])
-    # e.append_from_rv_cont([[distr1,distr1, distr1]])
-    # e.append_from_rv_cont([[distr1, mv]])
-
-    e.append(mv2)
-    e.append([mv2])
-    e.append([[distr1, distr1, distr1]])
-    e.append([[distr1, distr1, distr1], mv2])
-
-    # mixed mit RV Distributionen
-
-    e = uframe()
-    e_array = np.array([[1, np.nan, 3], [np.nan, 2, np.nan], [0, np.nan, np.nan]])
-
-    e.append(new=[e_array, {0: distr1, 1: [distr1, distr1], 2: mv}])
-
-    f = uframe()
-    f.append([np.array([[1, np.nan], [1, 1]]), {0: [distr1]}])
-
-    g = uframe()
-    g.append_from_rv_cont([distr1])
-
-    # fehlend: columns tauschen - da gibt es noch Dinge zu klären
-
-    a = np.array([[1, 3.6, 4.2], [2.2, 1, 3], [7, 6, 5], [8, 8, 2]])
-    u = uframe_noisy_array(a, 0.1, True, 0.3)
-
-    h = uframe()
-    h.append([[{0: 0.3, 1: 0.4, 2: 0.3}], [{0: 0.8, 1: 0.2}]])
-
-    h = uframe()
-    a = np.array([[1, 2, np.nan], [1, 3, np.nan]])
-    h.append([a, {0: [{0: 0.7, 1: 0.3}], 1: [{0: 0.1, 3: 0.9}]}])
-    x_ohe = h.get_dummies()
     
-    from scipy.stats import gamma, norm
-    uncertain = [uframe_instance(certain_data = np.array([2.1]), continuous = [norm(0.2,1), gamma(0.3)], indices = [[1],[0,2],[]]),
-                 uframe_instance(continuous = [norm(0.1,1), norm(0.3,0.7), gamma(1)], indices = [[],[1,0,2],[]])]
-    data = uframe()
-    data.append(uncertain)
-    print(data.sample())
+
```

### Comparing `uframe-0.0.7/src/uframe/uframe_from_mice.py` & `uframe-0.0.8/src/uframe/uframe_from_mice.py`

 * *Files identical despite different names*

### Comparing `uframe-0.0.7/src/uframe/uframe_instance.py` & `uframe-0.0.8/src/uframe/uframe_instance.py`

 * *Files identical despite different names*

### Comparing `uframe-0.0.7/src/uframe.egg-info/PKG-INFO` & `uframe-0.0.8/src/uframe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uframe
-Version: 0.0.7
+Version: 0.0.8
 Summary: Package for handling uncertain data
 Author: Christian Amesoeder and Michael Hagn
 Author-email: Christian Amesoder <christian.amesoeder@informatik.uni-regensburg.de>, Michael Hagn <michael.hagn@stud.uni-regensburg.de>
 Project-URL: Homepage, https://github.com/URWI2/uframe
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `uframe-0.0.7/tests/test_uframe_instance.py` & `uframe-0.0.8/tests/test_uframe_instance.py`

 * *Files identical despite different names*

