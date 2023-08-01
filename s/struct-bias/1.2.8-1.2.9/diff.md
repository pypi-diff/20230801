# Comparing `tmp/struct-bias-1.2.8.tar.gz` & `tmp/struct-bias-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "struct-bias-1.2.8.tar", last modified: Tue Aug  1 12:56:58 2023, max compression
+gzip compressed data, was "struct-bias-1.2.9.tar", last modified: Tue Aug  1 14:02:39 2023, max compression
```

## Comparing `struct-bias-1.2.8.tar` & `struct-bias-1.2.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 bas       (1000) bas       (1000)        0 2023-08-01 12:56:58.401411 struct-bias-1.2.8/
-drwxr-xr-x   0 bas       (1000) bas       (1000)        0 2023-08-01 12:56:58.401411 struct-bias-1.2.8/BIAS/
--rw-r--r--   0 bas       (1000) bas       (1000)     3430 2023-06-16 06:53:48.000000 struct-bias-1.2.8/BIAS/Create_RF.py
--rw-r--r--   0 bas       (1000) bas       (1000)    24319 2023-08-01 11:43:58.000000 struct-bias-1.2.8/BIAS/SB_Test_runner.py
--rw-r--r--   0 bas       (1000) bas       (1000)    23018 2023-08-01 12:56:25.000000 struct-bias-1.2.8/BIAS/SB_Toolbox.py
--rw-r--r--   0 bas       (1000) bas       (1000)      104 2023-06-16 06:53:48.000000 struct-bias-1.2.8/BIAS/__init__.py
--rw-r--r--   0 bas       (1000) bas       (1000)      760 2023-06-16 06:53:49.000000 struct-bias-1.2.8/BIAS/install.r
-drwxr-xr-x   0 bas       (1000) bas       (1000)        0 2023-08-01 12:56:58.401411 struct-bias-1.2.8/BIAS/models/
--rw-r--r--   0 bas       (1000) bas       (1000)       46 2023-06-16 06:53:49.000000 struct-bias-1.2.8/BIAS/models/empty.txt
--rw-r--r--   0 bas       (1000) bas       (1000)   246488 2023-08-01 12:27:12.000000 struct-bias-1.2.8/BIAS/models/opt_cnn_model-100.keras
--rw-r--r--   0 bas       (1000) bas       (1000)   436136 2023-08-01 12:27:13.000000 struct-bias-1.2.8/BIAS/models/opt_cnn_model-200.keras
--rw-r--r--   0 bas       (1000) bas       (1000)   125608 2023-08-01 12:27:12.000000 struct-bias-1.2.8/BIAS/models/opt_cnn_model-30.keras
--rw-r--r--   0 bas       (1000) bas       (1000)   138408 2023-08-01 12:27:12.000000 struct-bias-1.2.8/BIAS/models/opt_cnn_model-50.keras
--rw-r--r--   0 bas       (1000) bas       (1000)   954256 2023-08-01 12:27:13.000000 struct-bias-1.2.8/BIAS/models/opt_cnn_model-500.keras
--rw-r--r--   0 bas       (1000) bas       (1000)   814456 2023-08-01 12:27:13.000000 struct-bias-1.2.8/BIAS/models/opt_cnn_model-600.keras
--rw-r--r--   0 bas       (1000) bas       (1000)      350 2023-06-16 06:53:49.000000 struct-bias-1.2.8/BIAS/models/targetnames.npy
--rw-r--r--   0 bas       (1000) bas       (1000)     1632 2022-11-29 08:36:48.000000 struct-bias-1.2.8/LICENSE.md
--rw-r--r--   0 bas       (1000) bas       (1000)     3503 2023-08-01 12:56:58.401411 struct-bias-1.2.8/PKG-INFO
--rw-r--r--   0 bas       (1000) bas       (1000)     3138 2023-08-01 11:43:58.000000 struct-bias-1.2.8/README.md
--rw-r--r--   0 bas       (1000) bas       (1000)       38 2023-08-01 12:56:58.401411 struct-bias-1.2.8/setup.cfg
--rw-r--r--   0 bas       (1000) bas       (1000)     1208 2023-08-01 12:56:54.000000 struct-bias-1.2.8/setup.py
-drwxr-xr-x   0 bas       (1000) bas       (1000)        0 2023-08-01 12:56:58.401411 struct-bias-1.2.8/struct_bias.egg-info/
--rw-r--r--   0 bas       (1000) bas       (1000)     3503 2023-08-01 12:56:58.000000 struct-bias-1.2.8/struct_bias.egg-info/PKG-INFO
--rw-r--r--   0 bas       (1000) bas       (1000)      559 2023-08-01 12:56:58.000000 struct-bias-1.2.8/struct_bias.egg-info/SOURCES.txt
--rw-r--r--   0 bas       (1000) bas       (1000)        1 2023-08-01 12:56:58.000000 struct-bias-1.2.8/struct_bias.egg-info/dependency_links.txt
--rw-r--r--   0 bas       (1000) bas       (1000)       95 2023-08-01 12:56:58.000000 struct-bias-1.2.8/struct_bias.egg-info/requires.txt
--rw-r--r--   0 bas       (1000) bas       (1000)        5 2023-08-01 12:56:58.000000 struct-bias-1.2.8/struct_bias.egg-info/top_level.txt
+drwxr-xr-x   0 bas       (1000) bas       (1000)        0 2023-08-01 14:02:39.119601 struct-bias-1.2.9/
+drwxr-xr-x   0 bas       (1000) bas       (1000)        0 2023-08-01 14:02:39.119601 struct-bias-1.2.9/BIAS/
+-rw-r--r--   0 bas       (1000) bas       (1000)     3430 2023-06-16 06:53:48.000000 struct-bias-1.2.9/BIAS/Create_RF.py
+-rw-r--r--   0 bas       (1000) bas       (1000)    24319 2023-08-01 11:43:58.000000 struct-bias-1.2.9/BIAS/SB_Test_runner.py
+-rw-r--r--   0 bas       (1000) bas       (1000)    23013 2023-08-01 14:01:12.000000 struct-bias-1.2.9/BIAS/SB_Toolbox.py
+-rw-r--r--   0 bas       (1000) bas       (1000)      104 2023-06-16 06:53:48.000000 struct-bias-1.2.9/BIAS/__init__.py
+-rw-r--r--   0 bas       (1000) bas       (1000)      760 2023-06-16 06:53:49.000000 struct-bias-1.2.9/BIAS/install.r
+drwxr-xr-x   0 bas       (1000) bas       (1000)        0 2023-08-01 14:02:39.119601 struct-bias-1.2.9/BIAS/models/
+-rw-r--r--   0 bas       (1000) bas       (1000)       46 2023-06-16 06:53:49.000000 struct-bias-1.2.9/BIAS/models/empty.txt
+-rw-r--r--   0 bas       (1000) bas       (1000)   246488 2023-08-01 12:27:12.000000 struct-bias-1.2.9/BIAS/models/opt_cnn_model-100.keras
+-rw-r--r--   0 bas       (1000) bas       (1000)   436136 2023-08-01 12:27:13.000000 struct-bias-1.2.9/BIAS/models/opt_cnn_model-200.keras
+-rw-r--r--   0 bas       (1000) bas       (1000)   125608 2023-08-01 12:27:12.000000 struct-bias-1.2.9/BIAS/models/opt_cnn_model-30.keras
+-rw-r--r--   0 bas       (1000) bas       (1000)   138408 2023-08-01 12:27:12.000000 struct-bias-1.2.9/BIAS/models/opt_cnn_model-50.keras
+-rw-r--r--   0 bas       (1000) bas       (1000)   954256 2023-08-01 12:27:13.000000 struct-bias-1.2.9/BIAS/models/opt_cnn_model-500.keras
+-rw-r--r--   0 bas       (1000) bas       (1000)   814456 2023-08-01 12:27:13.000000 struct-bias-1.2.9/BIAS/models/opt_cnn_model-600.keras
+-rw-r--r--   0 bas       (1000) bas       (1000)      350 2023-06-16 06:53:49.000000 struct-bias-1.2.9/BIAS/models/targetnames.npy
+-rw-r--r--   0 bas       (1000) bas       (1000)     1632 2022-11-29 08:36:48.000000 struct-bias-1.2.9/LICENSE.md
+-rw-r--r--   0 bas       (1000) bas       (1000)     3503 2023-08-01 14:02:39.119601 struct-bias-1.2.9/PKG-INFO
+-rw-r--r--   0 bas       (1000) bas       (1000)     3138 2023-08-01 11:43:58.000000 struct-bias-1.2.9/README.md
+-rw-r--r--   0 bas       (1000) bas       (1000)       38 2023-08-01 14:02:39.119601 struct-bias-1.2.9/setup.cfg
+-rw-r--r--   0 bas       (1000) bas       (1000)     1208 2023-08-01 14:02:33.000000 struct-bias-1.2.9/setup.py
+drwxr-xr-x   0 bas       (1000) bas       (1000)        0 2023-08-01 14:02:39.119601 struct-bias-1.2.9/struct_bias.egg-info/
+-rw-r--r--   0 bas       (1000) bas       (1000)     3503 2023-08-01 14:02:39.000000 struct-bias-1.2.9/struct_bias.egg-info/PKG-INFO
+-rw-r--r--   0 bas       (1000) bas       (1000)      559 2023-08-01 14:02:39.000000 struct-bias-1.2.9/struct_bias.egg-info/SOURCES.txt
+-rw-r--r--   0 bas       (1000) bas       (1000)        1 2023-08-01 14:02:39.000000 struct-bias-1.2.9/struct_bias.egg-info/dependency_links.txt
+-rw-r--r--   0 bas       (1000) bas       (1000)       95 2023-08-01 14:02:39.000000 struct-bias-1.2.9/struct_bias.egg-info/requires.txt
+-rw-r--r--   0 bas       (1000) bas       (1000)        5 2023-08-01 14:02:39.000000 struct-bias-1.2.9/struct_bias.egg-info/top_level.txt
```

### Comparing `struct-bias-1.2.8/BIAS/Create_RF.py` & `struct-bias-1.2.9/BIAS/Create_RF.py`

 * *Files identical despite different names*

### Comparing `struct-bias-1.2.8/BIAS/SB_Test_runner.py` & `struct-bias-1.2.9/BIAS/SB_Test_runner.py`

 * *Files identical despite different names*

### Comparing `struct-bias-1.2.8/BIAS/SB_Toolbox.py` & `struct-bias-1.2.9/BIAS/SB_Toolbox.py`

 * *Files 0% similar despite different names*

```diff
@@ -361,15 +361,15 @@
             figsize=(12, data.shape[1] * 2),
             gridspec_kw={"width_ratios": [1, 3]},
         )
         for d in range(data.shape[1]):
             x = [np.sort(data[:, d])]
             x = np.expand_dims(x, axis=2)
             shap_val = self.explainer.shap_values(x)
-            if self.verbose:
+            if verbose:
                 print(preds[d])
             y = np.argmax(preds[d], axis=1)  # prediction of the dimension
             shap_vals_pred = shap_val[y[0]][0]
 
             cmap = sbs.color_palette("coolwarm", as_cmap=True)
             norm = plt.Normalize(
                 vmin=-1 * np.max(np.abs(shap_vals_pred)),
```

### Comparing `struct-bias-1.2.8/BIAS/install.r` & `struct-bias-1.2.9/BIAS/install.r`

 * *Files identical despite different names*

### Comparing `struct-bias-1.2.8/BIAS/models/opt_cnn_model-100.keras` & `struct-bias-1.2.9/BIAS/models/opt_cnn_model-100.keras`

 * *Files identical despite different names*

### Comparing `struct-bias-1.2.8/BIAS/models/opt_cnn_model-200.keras` & `struct-bias-1.2.9/BIAS/models/opt_cnn_model-200.keras`

 * *Files identical despite different names*

### Comparing `struct-bias-1.2.8/BIAS/models/opt_cnn_model-30.keras` & `struct-bias-1.2.9/BIAS/models/opt_cnn_model-30.keras`

 * *Files identical despite different names*

### Comparing `struct-bias-1.2.8/BIAS/models/opt_cnn_model-50.keras` & `struct-bias-1.2.9/BIAS/models/opt_cnn_model-50.keras`

 * *Files identical despite different names*

### Comparing `struct-bias-1.2.8/BIAS/models/opt_cnn_model-500.keras` & `struct-bias-1.2.9/BIAS/models/opt_cnn_model-500.keras`

 * *Files identical despite different names*

### Comparing `struct-bias-1.2.8/BIAS/models/opt_cnn_model-600.keras` & `struct-bias-1.2.9/BIAS/models/opt_cnn_model-600.keras`

 * *Files identical despite different names*

### Comparing `struct-bias-1.2.8/LICENSE.md` & `struct-bias-1.2.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `struct-bias-1.2.8/PKG-INFO` & `struct-bias-1.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: struct-bias
-Version: 1.2.8
+Version: 1.2.9
 Summary: BIAS toolbox: Structural bias detection for continuous optimization algorithms
 Author: Diederick Vermetten, Niki van Stein
 Author-email: d.l.vermetten@liacs.leidenuniv.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `struct-bias-1.2.8/README.md` & `struct-bias-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `struct-bias-1.2.8/setup.py` & `struct-bias-1.2.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
-__version__ = "1.2.8"
+__version__ = "1.2.9"
 gh_ref = os.environ.get("GITHUB_REF")
 if gh_ref:
     *_, tag = gh_ref.split("/")
     __version__ = tag.replace("v", "")
 
 setuptools.setup(
     name='struct-bias',
```

### Comparing `struct-bias-1.2.8/struct_bias.egg-info/PKG-INFO` & `struct-bias-1.2.9/struct_bias.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: struct-bias
-Version: 1.2.8
+Version: 1.2.9
 Summary: BIAS toolbox: Structural bias detection for continuous optimization algorithms
 Author: Diederick Vermetten, Niki van Stein
 Author-email: d.l.vermetten@liacs.leidenuniv.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `struct-bias-1.2.8/struct_bias.egg-info/SOURCES.txt` & `struct-bias-1.2.9/struct_bias.egg-info/SOURCES.txt`

 * *Files identical despite different names*

