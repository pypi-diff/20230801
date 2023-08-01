# Comparing `tmp/struct-bias-1.2.4.tar.gz` & `tmp/struct-bias-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "struct-bias-1.2.4.tar", last modified: Tue Aug  1 12:02:45 2023, max compression
+gzip compressed data, was "struct-bias-1.2.5.tar", last modified: Tue Aug  1 12:30:00 2023, max compression
```

## Comparing `struct-bias-1.2.4.tar` & `struct-bias-1.2.5.tar`

### file list

```diff
@@ -1,57 +1,21 @@
-drwxr-xr-x   0 bas       (1000) bas       (1000)        0 2023-08-01 12:02:45.732144 struct-bias-1.2.4/
-drwxr-xr-x   0 bas       (1000) bas       (1000)        0 2023-08-01 12:02:45.722144 struct-bias-1.2.4/BIAS/
--rw-r--r--   0 bas       (1000) bas       (1000)     3430 2023-06-16 06:53:48.000000 struct-bias-1.2.4/BIAS/Create_RF.py
--rw-r--r--   0 bas       (1000) bas       (1000)    24319 2023-08-01 11:43:58.000000 struct-bias-1.2.4/BIAS/SB_Test_runner.py
--rw-r--r--   0 bas       (1000) bas       (1000)    22889 2023-08-01 11:50:16.000000 struct-bias-1.2.4/BIAS/SB_Toolbox.py
--rw-r--r--   0 bas       (1000) bas       (1000)      104 2023-06-16 06:53:48.000000 struct-bias-1.2.4/BIAS/__init__.py
--rw-r--r--   0 bas       (1000) bas       (1000)      760 2023-06-16 06:53:49.000000 struct-bias-1.2.4/BIAS/install.r
-drwxr-xr-x   0 bas       (1000) bas       (1000)        0 2023-08-01 12:02:45.722144 struct-bias-1.2.4/BIAS/models/
--rw-r--r--   0 bas       (1000) bas       (1000)       46 2023-06-16 06:53:49.000000 struct-bias-1.2.4/BIAS/models/empty.txt
-drwxr-xr-x   0 bas       (1000) bas       (1000)        0 2023-08-01 12:02:45.722144 struct-bias-1.2.4/BIAS/models/opt_cnn_model-100/
--rw-r--r--   0 bas       (1000) bas       (1000)    20050 2023-08-01 11:43:07.000000 struct-bias-1.2.4/BIAS/models/opt_cnn_model-100/keras_metadata.pb
--rw-r--r--   0 bas       (1000) bas       (1000)   129724 2023-08-01 11:43:07.000000 struct-bias-1.2.4/BIAS/models/opt_cnn_model-100/saved_model.pb
-drwxr-xr-x   0 bas       (1000) bas       (1000)        0 2023-08-01 12:02:45.722144 struct-bias-1.2.4/BIAS/models/opt_cnn_model-100/variables/
--rw-r--r--   0 bas       (1000) bas       (1000)   221929 2023-08-01 11:43:07.000000 struct-bias-1.2.4/BIAS/models/opt_cnn_model-100/variables/variables.data-00000-of-00001
--rw-r--r--   0 bas       (1000) bas       (1000)      907 2023-08-01 11:43:07.000000 struct-bias-1.2.4/BIAS/models/opt_cnn_model-100/variables/variables.index
-drwxr-xr-x   0 bas       (1000) bas       (1000)        0 2023-08-01 12:02:45.722144 struct-bias-1.2.4/BIAS/models/opt_cnn_model-200/
--rw-r--r--   0 bas       (1000) bas       (1000)    20058 2023-08-01 11:43:08.000000 struct-bias-1.2.4/BIAS/models/opt_cnn_model-200/keras_metadata.pb
--rw-r--r--   0 bas       (1000) bas       (1000)   129998 2023-08-01 11:43:08.000000 struct-bias-1.2.4/BIAS/models/opt_cnn_model-200/saved_model.pb
-drwxr-xr-x   0 bas       (1000) bas       (1000)        0 2023-08-01 12:02:45.732144 struct-bias-1.2.4/BIAS/models/opt_cnn_model-200/variables/
--rw-r--r--   0 bas       (1000) bas       (1000)   412905 2023-08-01 11:43:08.000000 struct-bias-1.2.4/BIAS/models/opt_cnn_model-200/variables/variables.data-00000-of-00001
--rw-r--r--   0 bas       (1000) bas       (1000)      909 2023-08-01 11:43:08.000000 struct-bias-1.2.4/BIAS/models/opt_cnn_model-200/variables/variables.index
-drwxr-xr-x   0 bas       (1000) bas       (1000)        0 2023-08-01 12:02:45.732144 struct-bias-1.2.4/BIAS/models/opt_cnn_model-30/
--rw-r--r--   0 bas       (1000) bas       (1000)    20027 2023-08-01 11:43:06.000000 struct-bias-1.2.4/BIAS/models/opt_cnn_model-30/keras_metadata.pb
--rw-r--r--   0 bas       (1000) bas       (1000)   129496 2023-08-01 11:43:06.000000 struct-bias-1.2.4/BIAS/models/opt_cnn_model-30/saved_model.pb
-drwxr-xr-x   0 bas       (1000) bas       (1000)        0 2023-08-01 12:02:45.732144 struct-bias-1.2.4/BIAS/models/opt_cnn_model-30/variables/
--rw-r--r--   0 bas       (1000) bas       (1000)   102121 2023-08-01 11:43:06.000000 struct-bias-1.2.4/BIAS/models/opt_cnn_model-30/variables/variables.data-00000-of-00001
--rw-r--r--   0 bas       (1000) bas       (1000)      907 2023-08-01 11:43:06.000000 struct-bias-1.2.4/BIAS/models/opt_cnn_model-30/variables/variables.index
-drwxr-xr-x   0 bas       (1000) bas       (1000)        0 2023-08-01 12:02:45.732144 struct-bias-1.2.4/BIAS/models/opt_cnn_model-50/
--rw-r--r--   0 bas       (1000) bas       (1000)    20033 2023-08-01 11:43:07.000000 struct-bias-1.2.4/BIAS/models/opt_cnn_model-50/keras_metadata.pb
--rw-r--r--   0 bas       (1000) bas       (1000)   129724 2023-08-01 11:43:07.000000 struct-bias-1.2.4/BIAS/models/opt_cnn_model-50/saved_model.pb
-drwxr-xr-x   0 bas       (1000) bas       (1000)        0 2023-08-01 12:02:45.732144 struct-bias-1.2.4/BIAS/models/opt_cnn_model-50/variables/
--rw-r--r--   0 bas       (1000) bas       (1000)   114921 2023-08-01 11:43:06.000000 struct-bias-1.2.4/BIAS/models/opt_cnn_model-50/variables/variables.data-00000-of-00001
--rw-r--r--   0 bas       (1000) bas       (1000)      907 2023-08-01 11:43:06.000000 struct-bias-1.2.4/BIAS/models/opt_cnn_model-50/variables/variables.index
-drwxr-xr-x   0 bas       (1000) bas       (1000)        0 2023-08-01 12:02:45.732144 struct-bias-1.2.4/BIAS/models/opt_cnn_model-500/
--rw-r--r--   0 bas       (1000) bas       (1000)    19023 2023-08-01 11:43:08.000000 struct-bias-1.2.4/BIAS/models/opt_cnn_model-500/keras_metadata.pb
--rw-r--r--   0 bas       (1000) bas       (1000)   117952 2023-08-01 11:43:08.000000 struct-bias-1.2.4/BIAS/models/opt_cnn_model-500/saved_model.pb
-drwxr-xr-x   0 bas       (1000) bas       (1000)        0 2023-08-01 12:02:45.732144 struct-bias-1.2.4/BIAS/models/opt_cnn_model-500/variables/
--rw-r--r--   0 bas       (1000) bas       (1000)   930454 2023-08-01 11:43:08.000000 struct-bias-1.2.4/BIAS/models/opt_cnn_model-500/variables/variables.data-00000-of-00001
--rw-r--r--   0 bas       (1000) bas       (1000)      907 2023-08-01 11:43:08.000000 struct-bias-1.2.4/BIAS/models/opt_cnn_model-500/variables/variables.index
-drwxr-xr-x   0 bas       (1000) bas       (1000)        0 2023-08-01 12:02:45.732144 struct-bias-1.2.4/BIAS/models/opt_cnn_model-600/
--rw-r--r--   0 bas       (1000) bas       (1000)    24647 2023-08-01 11:43:09.000000 struct-bias-1.2.4/BIAS/models/opt_cnn_model-600/keras_metadata.pb
--rw-r--r--   0 bas       (1000) bas       (1000)   132148 2023-08-01 11:43:09.000000 struct-bias-1.2.4/BIAS/models/opt_cnn_model-600/saved_model.pb
-drwxr-xr-x   0 bas       (1000) bas       (1000)        0 2023-08-01 12:02:45.732144 struct-bias-1.2.4/BIAS/models/opt_cnn_model-600/variables/
--rw-r--r--   0 bas       (1000) bas       (1000)   788239 2023-08-01 11:43:09.000000 struct-bias-1.2.4/BIAS/models/opt_cnn_model-600/variables/variables.data-00000-of-00001
--rw-r--r--   0 bas       (1000) bas       (1000)     1007 2023-08-01 11:43:09.000000 struct-bias-1.2.4/BIAS/models/opt_cnn_model-600/variables/variables.index
--rw-r--r--   0 bas       (1000) bas       (1000)      350 2023-06-16 06:53:49.000000 struct-bias-1.2.4/BIAS/models/targetnames.npy
--rw-r--r--   0 bas       (1000) bas       (1000)     1632 2022-11-29 08:36:48.000000 struct-bias-1.2.4/LICENSE.md
--rw-r--r--   0 bas       (1000) bas       (1000)     3503 2023-08-01 12:02:45.732144 struct-bias-1.2.4/PKG-INFO
--rw-r--r--   0 bas       (1000) bas       (1000)     3138 2023-08-01 11:43:58.000000 struct-bias-1.2.4/README.md
--rw-r--r--   0 bas       (1000) bas       (1000)       38 2023-08-01 12:02:45.732144 struct-bias-1.2.4/setup.cfg
--rw-r--r--   0 bas       (1000) bas       (1000)     1202 2023-08-01 12:01:44.000000 struct-bias-1.2.4/setup.py
-drwxr-xr-x   0 bas       (1000) bas       (1000)        0 2023-08-01 12:02:45.732144 struct-bias-1.2.4/struct_bias.egg-info/
--rw-r--r--   0 bas       (1000) bas       (1000)     3503 2023-08-01 12:02:45.000000 struct-bias-1.2.4/struct_bias.egg-info/PKG-INFO
--rw-r--r--   0 bas       (1000) bas       (1000)     1651 2023-08-01 12:02:45.000000 struct-bias-1.2.4/struct_bias.egg-info/SOURCES.txt
--rw-r--r--   0 bas       (1000) bas       (1000)        1 2023-08-01 12:02:45.000000 struct-bias-1.2.4/struct_bias.egg-info/dependency_links.txt
--rw-r--r--   0 bas       (1000) bas       (1000)       85 2023-08-01 12:02:45.000000 struct-bias-1.2.4/struct_bias.egg-info/requires.txt
--rw-r--r--   0 bas       (1000) bas       (1000)        5 2023-08-01 12:02:45.000000 struct-bias-1.2.4/struct_bias.egg-info/top_level.txt
+drwxr-xr-x   0 bas       (1000) bas       (1000)        0 2023-08-01 12:30:00.069581 struct-bias-1.2.5/
+drwxr-xr-x   0 bas       (1000) bas       (1000)        0 2023-08-01 12:30:00.069581 struct-bias-1.2.5/BIAS/
+-rw-r--r--   0 bas       (1000) bas       (1000)     3430 2023-06-16 06:53:48.000000 struct-bias-1.2.5/BIAS/Create_RF.py
+-rw-r--r--   0 bas       (1000) bas       (1000)    24319 2023-08-01 11:43:58.000000 struct-bias-1.2.5/BIAS/SB_Test_runner.py
+-rw-r--r--   0 bas       (1000) bas       (1000)    22917 2023-08-01 12:28:52.000000 struct-bias-1.2.5/BIAS/SB_Toolbox.py
+-rw-r--r--   0 bas       (1000) bas       (1000)      104 2023-06-16 06:53:48.000000 struct-bias-1.2.5/BIAS/__init__.py
+-rw-r--r--   0 bas       (1000) bas       (1000)      760 2023-06-16 06:53:49.000000 struct-bias-1.2.5/BIAS/install.r
+drwxr-xr-x   0 bas       (1000) bas       (1000)        0 2023-08-01 12:30:00.069581 struct-bias-1.2.5/BIAS/models/
+-rw-r--r--   0 bas       (1000) bas       (1000)       46 2023-06-16 06:53:49.000000 struct-bias-1.2.5/BIAS/models/empty.txt
+-rw-r--r--   0 bas       (1000) bas       (1000)      350 2023-06-16 06:53:49.000000 struct-bias-1.2.5/BIAS/models/targetnames.npy
+-rw-r--r--   0 bas       (1000) bas       (1000)     1632 2022-11-29 08:36:48.000000 struct-bias-1.2.5/LICENSE.md
+-rw-r--r--   0 bas       (1000) bas       (1000)     3503 2023-08-01 12:30:00.069581 struct-bias-1.2.5/PKG-INFO
+-rw-r--r--   0 bas       (1000) bas       (1000)     3138 2023-08-01 11:43:58.000000 struct-bias-1.2.5/README.md
+-rw-r--r--   0 bas       (1000) bas       (1000)       38 2023-08-01 12:30:00.069581 struct-bias-1.2.5/setup.cfg
+-rw-r--r--   0 bas       (1000) bas       (1000)     1224 2023-08-01 12:29:25.000000 struct-bias-1.2.5/setup.py
+drwxr-xr-x   0 bas       (1000) bas       (1000)        0 2023-08-01 12:30:00.069581 struct-bias-1.2.5/struct_bias.egg-info/
+-rw-r--r--   0 bas       (1000) bas       (1000)     3503 2023-08-01 12:30:00.000000 struct-bias-1.2.5/struct_bias.egg-info/PKG-INFO
+-rw-r--r--   0 bas       (1000) bas       (1000)      345 2023-08-01 12:30:00.000000 struct-bias-1.2.5/struct_bias.egg-info/SOURCES.txt
+-rw-r--r--   0 bas       (1000) bas       (1000)        1 2023-08-01 12:30:00.000000 struct-bias-1.2.5/struct_bias.egg-info/dependency_links.txt
+-rw-r--r--   0 bas       (1000) bas       (1000)       95 2023-08-01 12:30:00.000000 struct-bias-1.2.5/struct_bias.egg-info/requires.txt
+-rw-r--r--   0 bas       (1000) bas       (1000)        5 2023-08-01 12:30:00.000000 struct-bias-1.2.5/struct_bias.egg-info/top_level.txt
```

### Comparing `struct-bias-1.2.4/BIAS/Create_RF.py` & `struct-bias-1.2.5/BIAS/Create_RF.py`

 * *Files identical despite different names*

### Comparing `struct-bias-1.2.4/BIAS/SB_Test_runner.py` & `struct-bias-1.2.5/BIAS/SB_Test_runner.py`

 * *Files identical despite different names*

### Comparing `struct-bias-1.2.4/BIAS/SB_Toolbox.py` & `struct-bias-1.2.5/BIAS/SB_Toolbox.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import rpy2.robjects as robjects
 import seaborn as sbs
 import shap
 import tensorflow as tf
 from rpy2.robjects.packages import importr
 from scipy.stats import percentileofscore
 from statsmodels.stats.multitest import multipletests
-
+import autokeras as ak
 from .SB_Test_runner import get_scens_per_dim, get_simulated_data, get_test_dict
 
 
 def install_r_packages():
     """Install the required R packages."""
     dirname = os.path.dirname(__file__)
     robjects.r.source(f"{dirname}/install.r", encoding="utf-8")
@@ -421,15 +421,15 @@
         n_samples = data.shape[0]
         if not n_samples in [30, 50, 100, 600]:
             raise ValueError("Sample size is not supported")
         if self.deepmodel == None:
             dirname = os.path.dirname(__file__)
             # download RF models if needed from
             self.deepmodel = tf.keras.models.load_model(
-                f"{dirname}/models/opt_cnn_model-{n_samples}"
+                f"{dirname}/models/opt_cnn_model-{n_samples}.keras"
             )
             self.targetnames = np.load(
                 f"{dirname}/models/targetnames.npy", allow_pickle=True
             )
             # loading explainable background samples and loading the explainer
             self.xai_background = getXAIBackground(data.shape[0])
             self.explainer = shap.DeepExplainer(self.deepmodel, self.xai_background)
```

### Comparing `struct-bias-1.2.4/BIAS/install.r` & `struct-bias-1.2.5/BIAS/install.r`

 * *Files identical despite different names*

### Comparing `struct-bias-1.2.4/LICENSE.md` & `struct-bias-1.2.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `struct-bias-1.2.4/PKG-INFO` & `struct-bias-1.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: struct-bias
-Version: 1.2.4
+Version: 1.2.5
 Summary: BIAS toolbox: Structural bias detection for continuous optimization algorithms
 Author: Diederick Vermetten, Niki van Stein
 Author-email: d.l.vermetten@liacs.leidenuniv.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `struct-bias-1.2.4/README.md` & `struct-bias-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `struct-bias-1.2.4/setup.py` & `struct-bias-1.2.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
-__version__ = "1.2.4"
+__version__ = "1.2.5"
 gh_ref = os.environ.get("GITHUB_REF")
 if gh_ref:
     *_, tag = gh_ref.split("/")
     __version__ = tag.replace("v", "")
 
 setuptools.setup(
     name='struct-bias',
@@ -30,15 +30,16 @@
         'rpy2',
         'scipy',
         'pandas',
         'sklearn',
         'matplotlib',
         'seaborn',
         'statsmodels',
-        'regex'
+        'regex',
+        'autokeras'
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
 )
```

### Comparing `struct-bias-1.2.4/struct_bias.egg-info/PKG-INFO` & `struct-bias-1.2.5/struct_bias.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: struct-bias
-Version: 1.2.4
+Version: 1.2.5
 Summary: BIAS toolbox: Structural bias detection for continuous optimization algorithms
 Author: Diederick Vermetten, Niki van Stein
 Author-email: d.l.vermetten@liacs.leidenuniv.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

