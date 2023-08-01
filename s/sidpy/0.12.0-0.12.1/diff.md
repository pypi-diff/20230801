# Comparing `tmp/sidpy-0.12.0.tar.gz` & `tmp/sidpy-0.12.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sidpy-0.12.0.tar", last modified: Mon Jul  3 20:48:28 2023, max compression
+gzip compressed data, was "sidpy-0.12.1.tar", last modified: Tue Aug  1 14:48:30 2023, max compression
```

## Comparing `sidpy-0.12.0.tar` & `sidpy-0.12.1.tar`

### file list

```diff
@@ -1,50 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:48:28.791724 sidpy-0.12.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-03 20:43:43.000000 sidpy-0.12.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 20:43:43.000000 sidpy-0.12.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-07-03 20:48:28.791724 sidpy-0.12.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-03 20:43:43.000000 sidpy-0.12.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-03 20:48:28.795724 sidpy-0.12.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-07-03 20:43:43.000000 sidpy-0.12.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:48:28.791724 sidpy-0.12.0/sidpy/
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-03 20:43:43.000000 sidpy-0.12.0/sidpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-03 20:43:43.000000 sidpy-0.12.0/sidpy/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:48:28.791724 sidpy-0.12.0/sidpy/base/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-03 20:43:43.000000 sidpy-0.12.0/sidpy/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7401 2023-07-03 20:43:43.000000 sidpy-0.12.0/sidpy/base/dict_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8253 2023-07-03 20:43:43.000000 sidpy-0.12.0/sidpy/base/num_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14095 2023-07-03 20:43:43.000000 sidpy-0.12.0/sidpy/base/string_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:48:28.791724 sidpy-0.12.0/sidpy/hdf/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-03 20:43:43.000000 sidpy-0.12.0/sidpy/hdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27179 2023-07-03 20:43:43.000000 sidpy-0.12.0/sidpy/hdf/dtype_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    30933 2023-07-03 20:43:43.000000 sidpy-0.12.0/sidpy/hdf/hdf_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15037 2023-07-03 20:43:43.000000 sidpy-0.12.0/sidpy/hdf/prov_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    19974 2023-07-03 20:43:43.000000 sidpy-0.12.0/sidpy/hdf/reg_ref.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:48:28.791724 sidpy-0.12.0/sidpy/io/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-03 20:43:43.000000 sidpy-0.12.0/sidpy/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11964 2023-07-03 20:43:43.000000 sidpy-0.12.0/sidpy/io/interface_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:48:28.791724 sidpy-0.12.0/sidpy/proc/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-03 20:43:43.000000 sidpy-0.12.0/sidpy/proc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11298 2023-07-03 20:43:43.000000 sidpy-0.12.0/sidpy/proc/comp_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    25463 2023-07-03 20:43:43.000000 sidpy-0.12.0/sidpy/proc/fitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:48:28.791724 sidpy-0.12.0/sidpy/sid/
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-03 20:43:43.000000 sidpy-0.12.0/sidpy/sid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    64690 2023-07-03 20:43:43.000000 sidpy-0.12.0/sidpy/sid/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-07-03 20:43:43.000000 sidpy-0.12.0/sidpy/sid/dimension.py
--rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-07-03 20:43:43.000000 sidpy-0.12.0/sidpy/sid/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-07-03 20:43:43.000000 sidpy-0.12.0/sidpy/sid/translator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:48:28.791724 sidpy-0.12.0/sidpy/viz/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-03 20:43:43.000000 sidpy-0.12.0/sidpy/viz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    53698 2023-07-03 20:43:43.000000 sidpy-0.12.0/sidpy/viz/dataset_viz.py
--rw-r--r--   0 runner    (1001) docker     (123)    18219 2023-07-03 20:43:43.000000 sidpy-0.12.0/sidpy/viz/jupyter_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:48:28.791724 sidpy-0.12.0/sidpy/viz/plot_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-03 20:43:43.000000 sidpy-0.12.0/sidpy/viz/plot_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8075 2023-07-03 20:43:43.000000 sidpy-0.12.0/sidpy/viz/plot_utils/cmap.py
--rw-r--r--   0 runner    (1001) docker     (123)    22689 2023-07-03 20:43:43.000000 sidpy-0.12.0/sidpy/viz/plot_utils/curve.py
--rw-r--r--   0 runner    (1001) docker     (123)    17268 2023-07-03 20:43:43.000000 sidpy-0.12.0/sidpy/viz/plot_utils/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     9510 2023-07-03 20:43:43.000000 sidpy-0.12.0/sidpy/viz/plot_utils/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:48:28.791724 sidpy-0.12.0/sidpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-07-03 20:48:28.000000 sidpy-0.12.0/sidpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-03 20:48:28.000000 sidpy-0.12.0/sidpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 20:48:28.000000 sidpy-0.12.0/sidpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-03 20:48:28.000000 sidpy-0.12.0/sidpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-03 20:48:28.000000 sidpy-0.12.0/sidpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:48:30.508401 sidpy-0.12.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-08-01 14:44:26.000000 sidpy-0.12.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-01 14:44:26.000000 sidpy-0.12.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-08-01 14:48:30.508401 sidpy-0.12.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-08-01 14:44:26.000000 sidpy-0.12.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-08-01 14:48:30.508401 sidpy-0.12.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-08-01 14:44:26.000000 sidpy-0.12.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:48:30.504401 sidpy-0.12.1/sidpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-08-01 14:44:26.000000 sidpy-0.12.1/sidpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-01 14:44:26.000000 sidpy-0.12.1/sidpy/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:48:30.504401 sidpy-0.12.1/sidpy/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-08-01 14:44:26.000000 sidpy-0.12.1/sidpy/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7401 2023-08-01 14:44:26.000000 sidpy-0.12.1/sidpy/base/dict_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8253 2023-08-01 14:44:26.000000 sidpy-0.12.1/sidpy/base/num_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14095 2023-08-01 14:44:26.000000 sidpy-0.12.1/sidpy/base/string_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:48:30.504401 sidpy-0.12.1/sidpy/hdf/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-08-01 14:44:26.000000 sidpy-0.12.1/sidpy/hdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27179 2023-08-01 14:44:26.000000 sidpy-0.12.1/sidpy/hdf/dtype_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30933 2023-08-01 14:44:26.000000 sidpy-0.12.1/sidpy/hdf/hdf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15037 2023-08-01 14:44:26.000000 sidpy-0.12.1/sidpy/hdf/prov_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19974 2023-08-01 14:44:26.000000 sidpy-0.12.1/sidpy/hdf/reg_ref.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:48:30.504401 sidpy-0.12.1/sidpy/io/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-01 14:44:26.000000 sidpy-0.12.1/sidpy/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11964 2023-08-01 14:44:26.000000 sidpy-0.12.1/sidpy/io/interface_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:48:30.504401 sidpy-0.12.1/sidpy/proc/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-08-01 14:44:26.000000 sidpy-0.12.1/sidpy/proc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25244 2023-08-01 14:44:26.000000 sidpy-0.12.1/sidpy/proc/fitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:48:30.504401 sidpy-0.12.1/sidpy/sid/
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-08-01 14:44:26.000000 sidpy-0.12.1/sidpy/sid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71833 2023-08-01 14:44:26.000000 sidpy-0.12.1/sidpy/sid/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7738 2023-08-01 14:44:26.000000 sidpy-0.12.1/sidpy/sid/dimension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-08-01 14:44:26.000000 sidpy-0.12.1/sidpy/sid/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-08-01 14:44:26.000000 sidpy-0.12.1/sidpy/sid/translator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:48:30.508401 sidpy-0.12.1/sidpy/viz/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-08-01 14:44:26.000000 sidpy-0.12.1/sidpy/viz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57824 2023-08-01 14:44:26.000000 sidpy-0.12.1/sidpy/viz/dataset_viz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18219 2023-08-01 14:44:26.000000 sidpy-0.12.1/sidpy/viz/jupyter_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:48:30.508401 sidpy-0.12.1/sidpy/viz/plot_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-08-01 14:44:26.000000 sidpy-0.12.1/sidpy/viz/plot_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8075 2023-08-01 14:44:26.000000 sidpy-0.12.1/sidpy/viz/plot_utils/cmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22689 2023-08-01 14:44:26.000000 sidpy-0.12.1/sidpy/viz/plot_utils/curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17268 2023-08-01 14:44:26.000000 sidpy-0.12.1/sidpy/viz/plot_utils/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9510 2023-08-01 14:44:26.000000 sidpy-0.12.1/sidpy/viz/plot_utils/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:48:30.504401 sidpy-0.12.1/sidpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-08-01 14:48:30.000000 sidpy-0.12.1/sidpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-08-01 14:48:30.000000 sidpy-0.12.1/sidpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 14:48:30.000000 sidpy-0.12.1/sidpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-08-01 14:48:30.000000 sidpy-0.12.1/sidpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-01 14:48:30.000000 sidpy-0.12.1/sidpy.egg-info/top_level.txt
```

### Comparing `sidpy-0.12.0/LICENSE` & `sidpy-0.12.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sidpy-0.12.0/PKG-INFO` & `sidpy-0.12.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sidpy
-Version: 0.12.0
+Version: 0.12.1
 Summary: Python utilities for storing, visualizing, and processing Spectroscopic and Imaging Data (SID)
 Home-page: https://pycroscopy.github.io/sidpy/about.html
 Author: Pycroscopy contributors
 Author-email: pycroscopy@gmail.com
 License: MIT
 Keywords: imaging,spectra,multidimensional,scientific,visualization,processing,storage,hdf5
 Platform: Linux
```

### Comparing `sidpy-0.12.0/README.rst` & `sidpy-0.12.1/README.rst`

 * *Files identical despite different names*

### Comparing `sidpy-0.12.0/setup.py` & `sidpy-0.12.1/setup.py`

 * *Files identical despite different names*

### Comparing `sidpy-0.12.0/sidpy/__init__.py` & `sidpy-0.12.1/sidpy/__init__.py`

 * *Files identical despite different names*

### Comparing `sidpy-0.12.0/sidpy/base/dict_utils.py` & `sidpy-0.12.1/sidpy/base/dict_utils.py`

 * *Files identical despite different names*

### Comparing `sidpy-0.12.0/sidpy/base/num_utils.py` & `sidpy-0.12.1/sidpy/base/num_utils.py`

 * *Files identical despite different names*

### Comparing `sidpy-0.12.0/sidpy/base/string_utils.py` & `sidpy-0.12.1/sidpy/base/string_utils.py`

 * *Files identical despite different names*

### Comparing `sidpy-0.12.0/sidpy/hdf/dtype_utils.py` & `sidpy-0.12.1/sidpy/hdf/dtype_utils.py`

 * *Files identical despite different names*

### Comparing `sidpy-0.12.0/sidpy/hdf/hdf_utils.py` & `sidpy-0.12.1/sidpy/hdf/hdf_utils.py`

 * *Files identical despite different names*

### Comparing `sidpy-0.12.0/sidpy/hdf/prov_utils.py` & `sidpy-0.12.1/sidpy/hdf/prov_utils.py`

 * *Files identical despite different names*

### Comparing `sidpy-0.12.0/sidpy/hdf/reg_ref.py` & `sidpy-0.12.1/sidpy/hdf/reg_ref.py`

 * *Files identical despite different names*

### Comparing `sidpy-0.12.0/sidpy/io/interface_utils.py` & `sidpy-0.12.1/sidpy/io/interface_utils.py`

 * *Files identical despite different names*

### Comparing `sidpy-0.12.0/sidpy/proc/fitter.py` & `sidpy-0.12.1/sidpy/proc/fitter.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,15 +171,15 @@
         self.num_workers = num_workers
         self.threads = threads
         self.guess_completed = False
         self.return_std = return_std
         self.return_cov = return_cov
         self.return_fit = return_fit
         self.fitted_dset = None
-        self._numpy = True
+
 
         self.mean_fit_results = []
         if self.return_cov:
             self.cov_fit_results = None
         if self.return_std:
             self.std_fit_results = None
 
@@ -200,14 +200,16 @@
             if i in self.ind_dims:
                 self.fold_order[0].extend([i])
                 self.num_computations *= self.dataset.shape[i]
             else:
                 self.fold_order.append([i])
 
         self.folded_dataset = self.dataset.fold(dim_order=self.fold_order)
+        self.folded_dataset_numpy = np.array(self.folded_dataset)
+        self.dep_vec = np.array(self.dep_vec)
 
         # Here is the tricky part, dataset.unfold is designed to get back the original dataset with minimal loss of
         # information. To do this, unfold utilizes the saved information while folding the original dataset.
         # Here, we are going to tweak that information and use the unfold method on the dataset with fitted parameters.
 
         self._unfold_attr = {
             'dim_order_flattened': list(np.arange(len(self.fold_order[0]))) + [len(self.fold_order[0])],
@@ -227,33 +229,30 @@
         Returns:
         None
         -------
 
         """
         guess_results = []
         for ind in range(self.num_computations):
-            if self._numpy:
-                self.dep_vec=np.array(self.dep_vec)
-                ydata = np.array(self.folded_dataset)
-            else:
-                ydata = self.folded_dataset
-
+            ydata = self.folded_dataset_numpy
             lazy_result = dask.delayed(self.guess_fn)(self.dep_vec, ydata[ind, :])
             guess_results.append(lazy_result)
 
         guess_results = dask.compute(*guess_results)
         self.prior = np.squeeze(np.array(guess_results))
         self.num_fit_parms = self.prior.shape[-1]
         self.guess_completed = True
 
     def do_fit(self, **kwargs):
         """
         Perform the fit.
         **kwargs: extra parameters passed to scipy.optimize.curve_fit, e.g. bounds, type of lsq algorithm, etc.
         """
+        
+
         if self.guess_fn is not None:
             guess_function_str = inspect.getsource(self.guess_fn)
         else:
             guess_function_str = 'Not Provided'
 
         fit_results = []
         if not self.km_guess:
@@ -261,22 +260,18 @@
                 self.do_guess()
 
             for ind in range(self.num_computations):
                 if self.prior is None:
                     p0 = np.random.normal(loc=0.5, scale=0.1, size=self.num_fit_parms)
                 else:
                     p0 = self.prior[ind, :]
-                ydata = self.folded_dataset[ind, :]
+                ydata = self.folded_dataset_numpy[ind, :]
                 if self._complex_data:
-                    ydata = ydata.flatten_complex()
+                    ydata = np.array(np.hstack([np.real(ydata), np.imag(ydata)]))
 
-                #Convert to numpy - see if this makes it faster??
-                if self._numpy:
-                    ydata = np.array(ydata)
-                    self.dep_vec = np.array(self.dep_vec)
                 lazy_result = dask.delayed(SidFitter.default_curve_fit)(self.fit_fn, self.dep_vec,
                                                                         ydata, self.num_fit_parms,
                                                                         return_cov=(self.return_cov or self.return_std),
                                                                         p0=p0, **kwargs)
                 fit_results.append(lazy_result)
 
             fit_results_comp = dask.compute(*fit_results)
```

### Comparing `sidpy-0.12.0/sidpy/sid/dataset.py` & `sidpy-0.12.1/sidpy/sid/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,35 +26,45 @@
 import dask.array.core
 import numpy as np
 import matplotlib.pylab as plt
 import string
 import dask.array as da
 import h5py
 from enum import Enum
+from numbers import Number
 
 from .dimension import Dimension, DimensionType
 from ..base.num_utils import get_slope
 from ..base.dict_utils import print_nested_dict
 from ..viz.dataset_viz import CurveVisualizer, ImageVisualizer, ImageStackVisualizer
 from ..viz.dataset_viz import SpectralImageVisualizer, FourDimImageVisualizer, ComplexSpectralImageVisualizer
 # from ..hdf.hdf_utils import is_editable_h5
 from .dimension import DimensionType
-from copy import deepcopy
+from copy import deepcopy, copy
+from sidpy.base.string_utils import validate_single_string_arg
+import logging
+
+
+def is_simple_list(lst):
+    if isinstance(lst, list):
+        return any(hasattr(item, '__getitem__') for item in lst)
+    return False
 
 
 class DataType(Enum):
     UNKNOWN = -1
     SPECTRUM = 1
     LINE_PLOT = 2
     LINE_PLOT_FAMILY = 3
     IMAGE = 4
     IMAGE_MAP = 5
     IMAGE_STACK = 6
     SPECTRAL_IMAGE = 7
     IMAGE_4D = 8
+    POINT_CLOUD = 9
 
 
 def view_subclass(dask_array, cls):
     """
     View a dask Array as an instance of a dask Array sub-class.
 
     Parameters
@@ -159,14 +169,16 @@
         self._h5_dataset = None
         self._metadata = {}
         self._original_metadata = {}
         self._axes = {}
 
         self.view = None  # this will hold the figure and axis reference for a plot
 
+        self.__protected = set()  # a set to keep track of protected attributes
+
     def __repr__(self):
         rep = 'sidpy.Dataset of type {} with:\n '.format(self.data_type.name)
         rep = rep + super(Dataset, self).__repr__()
         rep = rep + '\n data contains: {} ({})'.format(self.quantity, self.units)
         rep = rep + '\n and Dimensions: '
 
         for key in self._axes:
@@ -178,14 +190,37 @@
         return rep
 
     def hdf_close(self):
         if self.h5_dataset is not None:
             self.h5_dataset.file.close()
             print(self.h5_dataset)
 
+    def __setattr__(self, key, value):
+        if not hasattr(self, '_Dataset__protected'):
+            super().__setattr__(key, value)
+        else:
+            # if key is in __protected, only Dimension and numpy.ndarray instances are allowed to be set
+            if key != 'none' and key in self._Dataset__protected:
+                if not isinstance(value, Dimension):
+                    raise AttributeError('The attribute "{}" is reserved to represent a dimension'.format(key))
+                else:
+                    if getattr(self, key).name == value.name and len(getattr(self, key)) == len(value):
+                        cur_ind = [i for i in self._axes if self._axes[i].name == key][0]
+                        self.del_dimension(cur_ind)
+                        self._axes[cur_ind] = value
+                        self.__dict__[key] = value
+                        self.__dict__['dim_{}'.format(cur_ind)] = value
+                        self.__protected.add(key)
+                        self.__protected.add('dim_{}'.format(cur_ind))
+                    else:
+                        raise NotImplementedError("The new dimension's name or length does not "
+                                                  "match with the existing dimension.")
+            else:
+                super().__setattr__(key, value)
+
     @classmethod
     def from_array(cls, x, title='generic', chunks='auto', lock=False,
                    datatype='UNKNOWN', units='generic', quantity='generic',
                    modality='generic', source='generic', **kwargs):
         """
         Initializes a sidpy dataset from an array-like object (i.e. numpy array)
         All meta-data will be set to be generically.
@@ -209,15 +244,15 @@
         Returns
         -------
         sidpy dataset
 
         """
 
         # create vanilla dask array
-        if isinstance(x, da.Array):
+        if isinstance(x, da.Array) and not np.any(np.isnan(x.shape)):
             dask_array = x
         else:
             dask_array = da.from_array(np.array(x), chunks=chunks, lock=lock)
         # view as subclass
         sid_dataset = view_subclass(dask_array, cls)
         sid_dataset.data_type = datatype
         sid_dataset.units = units
@@ -315,15 +350,15 @@
                         print('using generic parameters for dimension ', dim)
 
         new_data.metadata = dict(self.metadata).copy()
         new_data.original_metadata = {}
         return new_data
 
     def __reduce_dimensions(self, new_dataset, axes, keepdims=False):
-        new_dataset._axes = {}
+        new_dataset.del_dimension()
         if not keepdims:
             i = 0
             for key, dim in self._axes.items():
                 new_dim = dim.copy()
                 if key not in axes:
                     new_dataset.set_dimension(i, new_dim)
                     i += 1
@@ -342,15 +377,15 @@
     def __rearrange_axes(self, new_dataset, new_order=None):
         """Rearranges the dimension order of the current instance
         Parameters:
             new_order: list or tuple of integers
 
         All the dimensions that are not in the new_order are deleted
         """
-        new_dataset._axes = {}
+        new_dataset.del_dimension()
 
         for i, dim in enumerate(new_order):
             new_dataset.set_dimension(i, self._axes[dim])
 
         return new_dataset
 
     def copy(self):
@@ -367,15 +402,15 @@
         dataset_copy.title = self.title
         dataset_copy.units = self.units
         dataset_copy.quantity = self.quantity
         dataset_copy.data_type = self.data_type
         dataset_copy.modality = self.modality
         dataset_copy.source = self.source
 
-        dataset_copy._axes = {}
+        dataset_copy.del_dimension()
         for dim in self._axes:
             dataset_copy.set_dimension(dim, self._axes[dim])
         dataset_copy.metadata = dict(self.metadata).copy()
 
         return dataset_copy
 
     def __validate_dim(self, ind, name):
@@ -416,19 +451,26 @@
             New name for Dimension
         """
         self.__validate_dim(ind, name)
         if not isinstance(name, str):
             raise TypeError('New Dimension name must be a string')
         if hasattr(self, self._axes[ind].name):
             delattr(self, self._axes[ind].name)
+            if self._axes[ind].name in self.__protected:
+                self.__protected.remove(self._axes[ind].name)
+
         if hasattr(self, 'dim_{}'.format(ind)):
             delattr(self, 'dim_{}'.format(ind))
-        self._axes[ind].name = name
+            self.__protected.remove('dim_{}'.format(ind))
+
+        self._axes[ind]._name = validate_single_string_arg(name, 'name')  # protected attribute name
         setattr(self, name, self._axes[ind])
+        self.__protected.add(name)
         setattr(self, 'dim_{}'.format(ind), self._axes[ind])
+        self.__protected.add('dim_{}'.format(ind))
 
     def set_dimension(self, ind, dimension):
         """
         sets the dimension for the dataset including new name and updating the axes dictionary
 
         Parameters
         ----------
@@ -450,24 +492,58 @@
                              )
 
         dim = dimension.copy()
 
         try:
             if hasattr(self, self._axes[ind].name):
                 delattr(self, self._axes[ind].name)
+                if self._axes[ind].name in self.__protected:
+                    self.__protected.remove(self._axes[ind].name)
         except KeyError:
             pass
 
         setattr(self, dimension.name, dim)
+        self.__protected.add(dimension.name)
 
         if hasattr(self, 'dim_{}'.format(ind)):
             delattr(self, 'dim_{}'.format(ind))
+            if 'dim_{}'.format(ind) in self.__protected:
+                self.__protected.remove('dim_{}'.format(ind))  # we don't need this. But I am trying to be consistent
 
         setattr(self, 'dim_{}'.format(ind), dim)
         self._axes[ind] = dim
+        self.__protected.add('dim_{}'.format(ind))
+
+    def del_dimension(self, ind=None):
+        """
+        Deletes the dimension attached to axis 'ind'.
+        """
+        if isinstance(ind, int):
+            ind = [ind]
+        elif ind is None:
+            ind = list(np.arange(self.ndim))
+        else:
+            ind = list(ind)
+
+        for i in ind:
+            # Delete the attribute with the format dim_0
+            if hasattr(self, 'dim_{}'.format(i)):
+                delattr(self, 'dim_{}'.format(i))
+                if 'dim_{}'.format(i) in self.__protected:
+                    self.__protected.remove('dim_{}'.format(i))
+
+            if i in self._axes.keys():
+                # Deleting the dataset attribute that has the dimension's name
+                if hasattr(self, self._axes[i].name):
+                    delattr(self, self._axes[i].name)
+                    if self._axes[i].name in self.__protected:
+                        self.__protected.remove(self._axes[i].name)
+
+                # Deleting the key-value pair from the _axes dictionary
+                del self._axes[i]
 
     def view_metadata(self):
         """
         Prints the metadata to stdout
 
         Returns
         -------
@@ -532,14 +608,18 @@
             if self.data_type == DataType.IMAGE:
                 self.view = ImageVisualizer(self, figure=figure, **kwargs)
                 # plt.show()
             elif self.data_type.value <= DataType['LINE_PLOT'].value:
                 # self.data_type in ['spectrum_family', 'line_family', 'line_plot_family', 'spectra']:
                 self.view = CurveVisualizer(self, figure=figure, **kwargs)
                 # plt.show()
+            elif self.data_type == DataType.POINT_CLOUD:
+                _obj, _coord = self._griddata_transform(**kwargs)
+                self.view = SpectralImageVisualizer(_obj, figure=figure, **kwargs)
+                self.view.axes[0].scatter(_coord[0], _coord[1], color='red', s=1)
             else:
                 raise NotImplementedError('Datasets with data_type {} cannot be plotted, yet.'.format(self.data_type))
         elif len(self.shape) == 3:
             if verbose:
                 print('3D dataset')
             if self.data_type == DataType.IMAGE:
                 self.view = ImageVisualizer(self, figure=figure, **kwargs)
@@ -551,14 +631,19 @@
                 # plt.show()
             elif self.data_type == DataType.SPECTRAL_IMAGE:
                 if 'complex' in self.dtype.name:
                     self.view = ComplexSpectralImageVisualizer(self, figure=figure, **kwargs)
                 else:
                     self.view = SpectralImageVisualizer(self, figure=figure, **kwargs)
                 # plt.show()
+            elif self.data_type == DataType.POINT_CLOUD:
+                _obj, _coord = self._griddata_transform(**kwargs)
+                self.view = SpectralImageVisualizer(_obj, figure=figure, **kwargs)
+                self.view.axes[0].scatter(_coord[0], _coord[1], color='red', s=1)
+
             else:
                 raise NotImplementedError('Datasets with data_type {} cannot be plotted, yet.'.format(self.data_type))
         elif len(self.shape) == 4:
             if verbose:
                 print('4D dataset')
             if self.data_type == DataType.IMAGE:
                 self.view = ImageVisualizer(self, **kwargs)
@@ -697,14 +782,72 @@
 
         spec_dims = []
         for dim, axis in self._axes.items():
             if axis.dimension_type == DimensionType.SPECTRAL:
                 spec_dims.append(dim)
         return spec_dims
 
+    def _griddata_transform(self, **kwargs):
+        '''
+        Interpolate unstructured point cloud for the visualization to 3D/4D sidpy.Dataset
+        Parameters
+        ----------
+        kwards: parameters to reduce dataset dimentions to 2D (number of point, spectral data)
+
+        Returns
+        -------
+        sidpy.Dataset with data_type = SPECTRAL_IMAGE
+        '''
+        from scipy.interpolate import griddata
+
+        if 'coordinates' in self.metadata.keys():
+            coord = self.metadata['coordinates']
+        else:
+            raise NotImplementedError('Datasets with data_type POINT_CLOUD must contain coordinates in metadata.')
+
+        if 'spacial_units' in self.metadata.keys():
+            sp_units  = self.metadata['spacial_units']
+        else:
+            sp_units = 'a.u.'
+
+        im_size = coord.shape[0]
+        _x0, _x1 = np.min(coord, axis=0)[0], np.max(coord, axis=0)[0]
+        _y0, _y1 = np.min(coord, axis=0)[1], np.max(coord, axis=0)[1]
+
+        _px_x = np.array((coord[:,0] - _x0)*im_size/(_x1 - _x0)).astype(int)
+        _px_y = np.array((coord[:, 1] - _y0) * im_size / (_y1 - _y0)).astype(int)
+
+        grid_x, grid_y = np.mgrid[_x0: _x1: (_x1 - _x0)/im_size,
+                                  _y0: _y1: (_y1 - _y0)/im_size]
+        grid_z = griddata(coord, self, (grid_x, grid_y), method='nearest')
+
+        #transpform to 3D
+        _dset = Dataset.from_array(grid_z)
+        _dset.data_type = 'spectral_image'
+        _dset.units = self.units
+        _dset.quantity = self.quantity
+        _dset.title = self.title
+        _dset.set_dimension(0, Dimension(grid_x[:,0], 'x'))
+        _dset.x.dimension_type = 'spatial'
+        _dset.x.units = sp_units
+        _dset.x.quantity = 'distance'
+        _dset.set_dimension(1, Dimension(grid_y[0], 'y'))
+        _dset.y.dimension_type = 'spatial'
+        _dset.y.units = sp_units
+        _dset.y.quantity = 'distance'
+        _dset.set_dimension(2, self.get_dimension_by_number(1)[0])
+        if len(self.shape) == 3:
+            _dset.set_dimension(3, self.get_dimension_by_number(2)[0])
+        return _dset, (_px_x, _px_y)
+
+    @staticmethod
+    def _min_dist(array):
+        _sort_ar = np.sort(array)
+        return np.min(_sort_ar[1:] - _sort_ar[:-1])
+
     @property
     def labels(self):
         labels = []
         for key, dim in self._axes.items():
             labels.append('{} ({})'.format(dim.quantity, dim.units))
         return labels
 
@@ -1162,25 +1305,26 @@
                                 title_prefix='Transposed_', checkdims=False)
         if not axes:
             new_axes_order = range(self.ndim)[::-1]
         elif len(axes) == 1 and isinstance(axes[0], Iterable):
             new_axes_order = axes[0]
         else:
             new_axes_order = axes
+
         return self.__rearrange_axes(result, new_axes_order)
 
     def round(self, decimals=0):
         return self.like_data(super().round(decimals=decimals),
                               title_prefix='Rounded_')
 
-    def reshape(self, *shape, merge_chunks=True):
+    def reshape(self, shape, merge_chunks=True, limit=None):
         # This somehow adds an extra dimension at the end
         # Will come back to this
         warnings.warn('Dimensional information will be lost.\
-                Please use fold, unfold to combine dimensions')
+                       Please use fold, unfold to combine dimensions')
         if len(shape) == 1 and isinstance(shape[0], Iterable):
             new_shape = shape[0]
         else:
             new_shape = shape
         return super().reshape(*new_shape, merge_chunks)
 
     @reduce_dims
@@ -1208,15 +1352,15 @@
         local_args['axis'] = axes
         return result, local_args
 
     def repeat(self, repeats, axis=None):
         result = self.like_data(super().repeat(repeats=repeats, axis=axis),
                                 title_prefix='Repeated_', checkdims=False)
 
-        result._axes = {}
+        # result._axes = {}
         for i, dim in self._axes.items():
             if axis != i:
                 new_dim = dim.copy()
             else:
                 new_dim = Dimension(np.repeat(dim.values, repeats=repeats),
                                     name=dim.name, quantity=dim.quantity,
                                     units=dim.units, dimension_type=dim.dimension_type)
@@ -1462,48 +1606,62 @@
             idx = tuple([idx])
 
         # The following line creates a new sidpy dataset with generic dimensions and ..
         # all the other attributes copied from 'self' aka parent dataset.
         sliced = self.like_data(super().__getitem__(idx), checkdims=False)
 
         # Delete the dimensions created by like_data
-        sliced._axes.clear()
+        sliced.del_dimension()
 
-        old_dims = deepcopy(self._axes)
+        old_dims = copy(self._axes)
         j, k = 0, 0  # j is for self (old_dims) and k is for the sliced dataset (new dimensions)
 
         for ind in idx:
             if ind is None:  # Add a new dimension
                 sliced.set_dimension(k, Dimension(1))
                 k += 1
             elif isinstance(ind, (int, np.integer)):
                 j += 1
-            elif isinstance(ind, (slice, np.ndarray, list)):
+            elif isinstance(ind, (slice, list)):
                 old_dim = old_dims[j]
-                sliced.set_dimension(k, Dimension(old_dim[ind],
+                sliced.set_dimension(k, Dimension(old_dim[ind].values,
                                                   name=old_dim.name, quantity=old_dim.quantity,
                                                   units=old_dim.units,
                                                   dimension_type=old_dim.dimension_type))
                 j += 1
                 k += 1
+
+            elif isinstance(ind, (np.ndarray, da.Array)):
+                if not ind.ndim == 1:
+                    raise NotImplementedError('Multi Dimensional Slicing of sidpy Dataset'
+                                              'is not available at this moment, please'
+                                              'raise an issue on out GitHub page')
+                old_dim = old_dims[j]
+                sliced.set_dimension(k, Dimension(old_dim[np.array(ind)].values,
+                                                  name=old_dim.name, quantity=old_dim.quantity,
+                                                  units=old_dim.units,
+                                                  dimension_type=old_dim.dimension_type))
+                j += 1
+                k += 1
+
             elif ind is Ellipsis:
                 start_dim = idx.index(Ellipsis)
                 ellipsis_dims = sliced.ndim - (len(idx) - 1)
                 stop_dim = start_dim + ellipsis_dims
 
                 for l in range(start_dim, stop_dim):
                     old_dim = old_dims[j]
                     sliced.set_dimension(k, old_dim)
                     j += 1
                     k += 1
 
         # Adding the rest of the dimensions
         for k in range(k, sliced.ndim):
             old_dim = old_dims[j]
-            sliced.set_dimension(k, Dimension(old_dim,
+            sliced.set_dimension(k, Dimension(old_dim.values,
                                               name=old_dim.name, quantity=old_dim.quantity,
                                               units=old_dim.units,
                                               dimension_type=old_dim.dimension_type))
             j += 1
             k += 1
 
         return sliced
```

### Comparing `sidpy-0.12.0/sidpy/sid/dimension.py` & `sidpy-0.12.1/sidpy/sid/dimension.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from __future__ import division, print_function, unicode_literals, \
     absolute_import
 from warnings import warn
 import sys
 import numpy as np
 from enum import Enum
 from sidpy.base.string_utils import validate_single_string_arg
+import copy
 
 __all__ = ['Dimension', 'DimensionType']
 
 if sys.version_info.major == 3:
     unicode = str
 
 
@@ -79,46 +80,71 @@
             values = np.arange(values)
         elif len(np.array(values)) < 1:
             raise TypeError("When specifying values over which a parameter is "
                             "varied, values should not be an empty array")
         if np.array(values).ndim != 1:
             raise ValueError('Dimension can only be 1 dimensional')
         new_dim = np.asarray(values, dtype=float).view(cls)
-        new_dim.name = name
+        new_dim._name = validate_single_string_arg(name, 'name')
         new_dim.quantity = quantity
         new_dim.units = units
         new_dim.dimension_type = dimension_type
         return new_dim
 
     def __array_finalize__(self, obj):
         # see InfoArray.__array_finalize__ for comments
         if obj is None:
             return
-        self.name = getattr(obj, 'name', 'generic')
-        self.quantity = getattr(obj, 'quantity', 'generic')
-        self.units = getattr(obj, 'name', 'units')
-        self.dimension_type = getattr(obj, 'dimension_type', 'UNKNOWN')
-
+        self._name = validate_single_string_arg(getattr(obj, '_name', 'generic'), 'name')
+        self.quantity = getattr(obj, '_quantity', 'generic')
+        self.units = getattr(obj, '_units', 'generic')
+        self.dimension_type = getattr(obj, '_dimension_type', 'UNKNOWN')
 
     def __array_wrap__(self, out_arr, context=None):
         # just call the parent
         super(Dimension, self).__array_wrap__(self, out_arr, context)
         # return correct values
         return out_arr
 
     def __repr__(self):
         return '{}:  {} ({}) of size {}'.format(self.name, self.quantity, self.units, self.shape)
 
     def __str__(self):
         return '{}:  {} ({}) of size {}'.format(self.name, self.quantity, self.units, self.shape)
 
+    # def __copy__(self):
+    #     new_dim = Dimension(np.array(self), name=self.name, quantity=self.quantity, units=self.units)
+    #     new_dim.dimension_type = self.dimension_type
+    #     return new_dim
+
     def __copy__(self):
-        new_dim = Dimension(np.array(self), name=self.name, quantity=self.quantity, units=self.units)
-        new_dim.dimension_type = self.dimension_type
-        return new_dim
+        # Create a new instance of Dimension
+        new_instance = Dimension(
+            copy.copy(self.values),
+            copy.copy(self.name),
+            copy.copy(self.quantity),
+            copy.copy(self.units),
+            copy.copy(self.dimension_type)
+        )
+
+        return new_instance
+
+    def __deepcopy__(self, memo):
+        # For now this is what chatGPT came up with and it does not break any tests
+
+        # Create a new instance of Dimension
+        new_instance = Dimension(
+            copy.deepcopy(self.values, memo),
+            copy.deepcopy(self.name, memo),
+            copy.deepcopy(self.quantity, memo),
+            copy.deepcopy(self.units, memo),
+            copy.deepcopy(self.dimension_type, memo)
+        )
+
+        return new_instance
 
     # TODO: Implement equality
 
     # TODO: Find out how to get rid of this
     def copy(self):
         # Not sure why __copy__() would not be called by itself
         new_dim = self.__copy__()
@@ -131,15 +157,19 @@
 
     @property
     def name(self):
         return self._name
 
     @name.setter
     def name(self, value):
-        self._name = validate_single_string_arg(value, 'name')
+        raise AttributeError("Cannot change the name of the dimension. "
+                             "If the dimension is associated with the dataset, please try "
+                             "dataset.rename_dimension")
+
+    #     # self._name = validate_single_string_arg(value, 'name')
 
     @property
     def quantity(self):
         return self._quantity
 
     @quantity.setter
     def quantity(self, value):
@@ -158,15 +188,15 @@
         return self._dimension_type
 
     @dimension_type.setter
     def dimension_type(self, value):
         if isinstance(value, DimensionType):
             self._dimension_type = value
         else:
-            dimension_type = validate_single_string_arg(value,'dimension_type')
+            dimension_type = validate_single_string_arg(value, 'dimension_type')
 
             if dimension_type.upper() in [member.name for member in DimensionType]:
                 self._dimension_type = DimensionType[dimension_type.upper()]
             elif dimension_type.lower() in ['frame', 'time', 'stack']:
                 self._dimension_type = DimensionType.TEMPORAL
             else:
                 self._dimension_type = DimensionType.UNKNOWN
@@ -174,23 +204,27 @@
                      ''.format([member.name for member in DimensionType]))
                 warn('Setting DimensionType to UNKNOWN')
 
     @property
     def values(self):
         return np.array(self)
 
+    # @values.setter
+    # def values(self, value):
+    #     isinstance(np.ndarray)
+
     def __eq__(self, other):
         if not isinstance(other, Dimension):
             return False
         if self.name != other.name:
             return False
         if self.units != other.units:
             return False
         if self.quantity != other.quantity:
             return False
         if len(self.values) != len(other):
             return False
         if not (np.array(self) == np.array(other)).all():
             return False
-        if not (self.values==other.values).all():
+        if not (self.values == other.values).all():
             return False
         return True
```

### Comparing `sidpy-0.12.0/sidpy/sid/reader.py` & `sidpy-0.12.1/sidpy/sid/reader.py`

 * *Files identical despite different names*

### Comparing `sidpy-0.12.0/sidpy/sid/translator.py` & `sidpy-0.12.1/sidpy/sid/translator.py`

 * *Files identical despite different names*

### Comparing `sidpy-0.12.0/sidpy/viz/dataset_viz.py` & `sidpy-0.12.1/sidpy/viz/dataset_viz.py`

 * *Files 4% similar despite different names*

```diff
@@ -543,14 +543,15 @@
         self.scaleX = 1.0
         self.scaleY = 1.0
         self.analysis = []
         self.plot_legend = False
 
         self.image_dims = image_dims
         self.spec_dim = spectral_dim[0]
+        self.extent_rd = self.dset.get_extent(self.image_dims)
 
         if horizontal:
             self.axes = self.fig.subplots(ncols=2)
         else:
             self.axes = self.fig.subplots(nrows=2, **fig_args)
 
         if self.set_title:
@@ -566,45 +567,114 @@
             # self.extent[2]=self.image.shape[1]
             # self.bin_y=self.image.shape[1]
             self.axes[0].set_aspect('auto')
         else:
             self.axes[0].set_aspect('equal')
 
         self.axes[0].imshow(self.image.T, extent=self.extent, **kwargs)
-        if horizontal:
-            self.axes[0].set_xlabel('{} [pixels]'.format(self.dset._axes[image_dims[0]].quantity))
-        else:
-            self.axes[0].set_ylabel('{} [pixels]'.format(self.dset._axes[image_dims[1]].quantity))
-
+        
         if 1 in self.dset.shape:
             self.axes[0].set_aspect('auto')
             self.axes[0].get_yaxis().set_visible(False)
         else:
             self.axes[0].set_aspect('equal')
 
+        self.axes[0].set_xticks(np.linspace(self.extent[0], self.extent[1], 5),
+                                    np.round(np.linspace(self.extent[0], self.extent[1], 5),2))
+        self.axes[0].set_yticks(np.linspace(self.extent[2], self.extent[3], 5),
+                                np.round(np.linspace(self.extent[2], self.extent[3], 5),1))
+
+        self.axes[0].set_xlabel('{} [{}]'.format(self.dset._axes[self.image_dims[0]].quantity,
+                                                    'px'))
+        self.axes[0].set_ylabel('{} [{}]'.format(self.dset._axes[self.image_dims[1]].quantity,
+                                                        'px'))
+
         # self.rect = patches.Rectangle((0,0),1,1,linewidth=1,edgecolor='r',facecolor='red', alpha = 0.2)
         self.rect = patches.Rectangle((0, 0), self.bin_x, self.bin_y, linewidth=1, edgecolor='r',
                                       facecolor='red', alpha=0.2)
 
         self.axes[0].add_patch(self.rect)
+
+        #Below is code for the spectrum parts
         self.intensity_scale = 1.
         self.spectrum = self.get_spectrum()
         if len(self.energy_scale)!=self.spectrum.shape[0]:
             self.spectrum = self.spectrum.T
         self.axes[1].plot(self.energy_scale, self.spectrum.compute())
         self.axes[1].set_title('spectrum {}, {}'.format(self.x, self.y))
         self.xlabel = self.dset.labels[self.spec_dim]
         self.ylabel = self.dset.data_descriptor
         self.axes[1].set_xlabel(self.dset.labels[self.spec_dim])  # + x_suffix)
         self.axes[1].set_ylabel(self.dset.data_descriptor)
         self.axes[1].ticklabel_format(style='sci', scilimits=(-2, 3))
         self.fig.tight_layout()
         self.cid = self.axes[1].figure.canvas.mpl_connect('button_press_event', self._onclick)
 
+        import ipywidgets as iwgt
+        self.button = iwgt.widgets.Dropdown( options=[('Pixel Wise', 1), ('Units Wise', 2)],
+                            value=1,
+                            description='Image',
+                            tooltip='How to plot spatial data: Pixel Wise (by px), Units wise (in given units)', 
+                            layout = iwgt.Layout(width='30%', height='50px',))
+
+        self.button.observe(self._pw_uw, 'value') #pixel or unit wise
         self.fig.canvas.draw_idle()
+        widg = iwgt.HBox([self.button])
+        widg
+        from IPython.display import display
+        display(widg)
+
+    def _pw_uw(self, event): 
+        pw_uw = event.new
+        self._update_image(pw_uw)
+    
+    def _update_image(self, event_value):
+        #pixel wise or unit wise listener
+        if event_value==1:
+            self.axes[0].set_xticks(np.linspace(self.extent[0], self.extent[1], 5),
+                                    np.round(np.linspace(self.extent[0], self.extent[1], 5),2))
+            self.axes[0].set_yticks(np.linspace(self.extent[2], self.extent[3], 5),
+                                    np.round(np.linspace(self.extent[2], self.extent[3], 5),1))
+
+            self.axes[0].set_xlabel('{} [{}]'.format(self.dset._axes[self.image_dims[0]].quantity,
+                                                     'px'))
+            self.axes[0].set_ylabel('{} [{}]'.format(self.dset._axes[self.image_dims[1]].quantity,
+                                                         'px'))
+        else:
+            self.axes[0].set_ylabel('{} [{}]'.format(self.dset._axes[self.image_dims[1]].quantity,
+                                                            self.dset._axes[self.image_dims[1]].units))
+
+            self.axes[0].set_xticks(np.linspace(self.extent[0], self.extent[1], 5),
+                                    np.round(np.linspace(self.extent_rd[0], self.extent_rd[1], 5), 2))
+
+            self.axes[0].set_yticks(np.linspace(self.extent[2], self.extent[3], 5),
+                                    np.round(np.linspace(self.extent_rd[2], self.extent_rd[3], 5), 2))
+            
+            self.axes[0].set_xlabel('{} [{}]'.format(self.dset._axes[self.image_dims[0]].quantity,
+                                                        self.dset._axes[self.image_dims[0]].units))
+            
+            self.axes[0].set_ylabel('{} [{}]'.format(self.dset._axes[self.image_dims[1]].quantity,
+                                                            self.dset._axes[self.image_dims[1]].units))
+
+            if self.dset._axes[self.image_dims[0]].units =='m':
+                scaled_values_y = self.dset._axes[self.image_dims[1]].values*1E9
+                scaled_values_x = self.dset._axes[self.image_dims[0]].values*1E9
+                if scaled_values_x.mean() >=0.1 and  scaled_values_x.mean() <=1000:
+                    self.axes[0].set_xticks(np.linspace(self.extent[0], self.extent[1], 5),
+                                    np.round(np.linspace(scaled_values_x[0], scaled_values_x[-1], 5), 2))
+                    self.axes[0].set_yticks(np.linspace(self.extent[2], self.extent[3], 5),
+                                    np.round(np.linspace(scaled_values_y[0], scaled_values_y[-1], 5), 2))
+                    
+                    self.axes[0].set_xlabel('{} [{}]'.format(self.dset._axes[self.image_dims[0]].quantity,
+                                                        'nm'))
+            
+                    self.axes[0].set_ylabel('{} [{}]'.format(self.dset._axes[self.image_dims[1]].quantity,
+                                                            'nm'))
+                    
+        return
 
     def set_bin(self, bin_xy):
 
         old_bin_x = self.bin_x
         old_bin_y = self.bin_y
         if isinstance(bin_xy, list):
 
@@ -629,23 +699,21 @@
 
         self.rect.set_xy([self.x * self.rect.get_width() / self.bin_x + self.rectangle[0],
                           self.y * self.rect.get_height() / self.bin_y + self.rectangle[2]])
         self._update()
 
     def get_spectrum(self):
         from ..sid.dimension import DimensionType
-
         if self.x > self.dset.shape[self.image_dims[0]] - self.bin_x:
             self.x = self.dset.shape[self.image_dims[0]] - self.bin_x
         if self.y > self.dset.shape[self.image_dims[1]] - self.bin_y:
             self.y = self.dset.shape[self.image_dims[1]] - self.bin_y
         selection = []
 
         for dim, axis in self.dset._axes.items():
-            # print(dim, axis.dimension_type)
             if axis.dimension_type == DimensionType.SPATIAL:
                 if dim == self.image_dims[0]:
                     selection.append(slice(self.x, self.x + self.bin_x))
                 else:
                     selection.append(slice(self.y, self.y + self.bin_y))
 
             elif axis.dimension_type == DimensionType.SPECTRAL:
```

### Comparing `sidpy-0.12.0/sidpy/viz/jupyter_utils.py` & `sidpy-0.12.1/sidpy/viz/jupyter_utils.py`

 * *Files identical despite different names*

### Comparing `sidpy-0.12.0/sidpy/viz/plot_utils/cmap.py` & `sidpy-0.12.1/sidpy/viz/plot_utils/cmap.py`

 * *Files identical despite different names*

### Comparing `sidpy-0.12.0/sidpy/viz/plot_utils/curve.py` & `sidpy-0.12.1/sidpy/viz/plot_utils/curve.py`

 * *Files identical despite different names*

### Comparing `sidpy-0.12.0/sidpy/viz/plot_utils/image.py` & `sidpy-0.12.1/sidpy/viz/plot_utils/image.py`

 * *Files identical despite different names*

### Comparing `sidpy-0.12.0/sidpy/viz/plot_utils/misc.py` & `sidpy-0.12.1/sidpy/viz/plot_utils/misc.py`

 * *Files identical despite different names*

### Comparing `sidpy-0.12.0/sidpy.egg-info/PKG-INFO` & `sidpy-0.12.1/sidpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sidpy
-Version: 0.12.0
+Version: 0.12.1
 Summary: Python utilities for storing, visualizing, and processing Spectroscopic and Imaging Data (SID)
 Home-page: https://pycroscopy.github.io/sidpy/about.html
 Author: Pycroscopy contributors
 Author-email: pycroscopy@gmail.com
 License: MIT
 Keywords: imaging,spectra,multidimensional,scientific,visualization,processing,storage,hdf5
 Platform: Linux
```

### Comparing `sidpy-0.12.0/sidpy.egg-info/SOURCES.txt` & `sidpy-0.12.1/sidpy.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 sidpy/hdf/dtype_utils.py
 sidpy/hdf/hdf_utils.py
 sidpy/hdf/prov_utils.py
 sidpy/hdf/reg_ref.py
 sidpy/io/__init__.py
 sidpy/io/interface_utils.py
 sidpy/proc/__init__.py
-sidpy/proc/comp_utils.py
 sidpy/proc/fitter.py
 sidpy/sid/__init__.py
 sidpy/sid/dataset.py
 sidpy/sid/dimension.py
 sidpy/sid/reader.py
 sidpy/sid/translator.py
 sidpy/viz/__init__.py
```

