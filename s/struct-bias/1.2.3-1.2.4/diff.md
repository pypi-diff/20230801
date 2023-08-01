# Comparing `tmp/struct-bias-1.2.3.tar.gz` & `tmp/struct-bias-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "struct-bias-1.2.3.tar", last modified: Fri Jun 16 08:04:43 2023, max compression
+gzip compressed data, was "struct-bias-1.2.4.tar", last modified: Tue Aug  1 12:02:45 2023, max compression
```

## Comparing `struct-bias-1.2.3.tar` & `struct-bias-1.2.4.tar`

### file list

```diff
@@ -1,18 +1,57 @@
-drwxr-xr-x   0 bas       (1000) bas       (1000)        0 2023-06-16 08:04:43.943876 struct-bias-1.2.3/
-drwxr-xr-x   0 bas       (1000) bas       (1000)        0 2023-06-16 08:04:43.943876 struct-bias-1.2.3/BIAS/
--rw-r--r--   0 bas       (1000) bas       (1000)     3430 2023-06-16 06:53:48.000000 struct-bias-1.2.3/BIAS/Create_RF.py
--rw-r--r--   0 bas       (1000) bas       (1000)    24319 2023-06-16 06:53:55.000000 struct-bias-1.2.3/BIAS/SB_Test_runner.py
--rw-r--r--   0 bas       (1000) bas       (1000)    22892 2023-06-16 07:19:50.000000 struct-bias-1.2.3/BIAS/SB_Toolbox.py
--rw-r--r--   0 bas       (1000) bas       (1000)      104 2023-06-16 06:53:48.000000 struct-bias-1.2.3/BIAS/__init__.py
--rw-r--r--   0 bas       (1000) bas       (1000)      760 2023-06-16 06:53:49.000000 struct-bias-1.2.3/BIAS/install.r
--rw-r--r--   0 bas       (1000) bas       (1000)     1632 2022-11-29 08:36:48.000000 struct-bias-1.2.3/LICENSE.md
--rw-r--r--   0 bas       (1000) bas       (1000)     2348 2023-06-16 08:04:43.943876 struct-bias-1.2.3/PKG-INFO
--rw-r--r--   0 bas       (1000) bas       (1000)     1942 2023-06-16 07:18:43.000000 struct-bias-1.2.3/README.md
--rw-r--r--   0 bas       (1000) bas       (1000)       38 2023-06-16 08:04:43.943876 struct-bias-1.2.3/setup.cfg
--rw-r--r--   0 bas       (1000) bas       (1000)     1174 2023-06-16 08:04:42.000000 struct-bias-1.2.3/setup.py
-drwxr-xr-x   0 bas       (1000) bas       (1000)        0 2023-06-16 08:04:43.943876 struct-bias-1.2.3/struct_bias.egg-info/
--rw-r--r--   0 bas       (1000) bas       (1000)     2348 2023-06-16 08:04:43.000000 struct-bias-1.2.3/struct_bias.egg-info/PKG-INFO
--rw-r--r--   0 bas       (1000) bas       (1000)      295 2023-06-16 08:04:43.000000 struct-bias-1.2.3/struct_bias.egg-info/SOURCES.txt
--rw-r--r--   0 bas       (1000) bas       (1000)        1 2023-06-16 08:04:43.000000 struct-bias-1.2.3/struct_bias.egg-info/dependency_links.txt
--rw-r--r--   0 bas       (1000) bas       (1000)       85 2023-06-16 08:04:43.000000 struct-bias-1.2.3/struct_bias.egg-info/requires.txt
--rw-r--r--   0 bas       (1000) bas       (1000)        5 2023-06-16 08:04:43.000000 struct-bias-1.2.3/struct_bias.egg-info/top_level.txt
+drwxr-xr-x   0 bas       (1000) bas       (1000)        0 2023-08-01 12:02:45.732144 struct-bias-1.2.4/
+drwxr-xr-x   0 bas       (1000) bas       (1000)        0 2023-08-01 12:02:45.722144 struct-bias-1.2.4/BIAS/
+-rw-r--r--   0 bas       (1000) bas       (1000)     3430 2023-06-16 06:53:48.000000 struct-bias-1.2.4/BIAS/Create_RF.py
+-rw-r--r--   0 bas       (1000) bas       (1000)    24319 2023-08-01 11:43:58.000000 struct-bias-1.2.4/BIAS/SB_Test_runner.py
+-rw-r--r--   0 bas       (1000) bas       (1000)    22889 2023-08-01 11:50:16.000000 struct-bias-1.2.4/BIAS/SB_Toolbox.py
+-rw-r--r--   0 bas       (1000) bas       (1000)      104 2023-06-16 06:53:48.000000 struct-bias-1.2.4/BIAS/__init__.py
+-rw-r--r--   0 bas       (1000) bas       (1000)      760 2023-06-16 06:53:49.000000 struct-bias-1.2.4/BIAS/install.r
+drwxr-xr-x   0 bas       (1000) bas       (1000)        0 2023-08-01 12:02:45.722144 struct-bias-1.2.4/BIAS/models/
+-rw-r--r--   0 bas       (1000) bas       (1000)       46 2023-06-16 06:53:49.000000 struct-bias-1.2.4/BIAS/models/empty.txt
+drwxr-xr-x   0 bas       (1000) bas       (1000)        0 2023-08-01 12:02:45.722144 struct-bias-1.2.4/BIAS/models/opt_cnn_model-100/
+-rw-r--r--   0 bas       (1000) bas       (1000)    20050 2023-08-01 11:43:07.000000 struct-bias-1.2.4/BIAS/models/opt_cnn_model-100/keras_metadata.pb
+-rw-r--r--   0 bas       (1000) bas       (1000)   129724 2023-08-01 11:43:07.000000 struct-bias-1.2.4/BIAS/models/opt_cnn_model-100/saved_model.pb
+drwxr-xr-x   0 bas       (1000) bas       (1000)        0 2023-08-01 12:02:45.722144 struct-bias-1.2.4/BIAS/models/opt_cnn_model-100/variables/
+-rw-r--r--   0 bas       (1000) bas       (1000)   221929 2023-08-01 11:43:07.000000 struct-bias-1.2.4/BIAS/models/opt_cnn_model-100/variables/variables.data-00000-of-00001
+-rw-r--r--   0 bas       (1000) bas       (1000)      907 2023-08-01 11:43:07.000000 struct-bias-1.2.4/BIAS/models/opt_cnn_model-100/variables/variables.index
+drwxr-xr-x   0 bas       (1000) bas       (1000)        0 2023-08-01 12:02:45.722144 struct-bias-1.2.4/BIAS/models/opt_cnn_model-200/
+-rw-r--r--   0 bas       (1000) bas       (1000)    20058 2023-08-01 11:43:08.000000 struct-bias-1.2.4/BIAS/models/opt_cnn_model-200/keras_metadata.pb
+-rw-r--r--   0 bas       (1000) bas       (1000)   129998 2023-08-01 11:43:08.000000 struct-bias-1.2.4/BIAS/models/opt_cnn_model-200/saved_model.pb
+drwxr-xr-x   0 bas       (1000) bas       (1000)        0 2023-08-01 12:02:45.732144 struct-bias-1.2.4/BIAS/models/opt_cnn_model-200/variables/
+-rw-r--r--   0 bas       (1000) bas       (1000)   412905 2023-08-01 11:43:08.000000 struct-bias-1.2.4/BIAS/models/opt_cnn_model-200/variables/variables.data-00000-of-00001
+-rw-r--r--   0 bas       (1000) bas       (1000)      909 2023-08-01 11:43:08.000000 struct-bias-1.2.4/BIAS/models/opt_cnn_model-200/variables/variables.index
+drwxr-xr-x   0 bas       (1000) bas       (1000)        0 2023-08-01 12:02:45.732144 struct-bias-1.2.4/BIAS/models/opt_cnn_model-30/
+-rw-r--r--   0 bas       (1000) bas       (1000)    20027 2023-08-01 11:43:06.000000 struct-bias-1.2.4/BIAS/models/opt_cnn_model-30/keras_metadata.pb
+-rw-r--r--   0 bas       (1000) bas       (1000)   129496 2023-08-01 11:43:06.000000 struct-bias-1.2.4/BIAS/models/opt_cnn_model-30/saved_model.pb
+drwxr-xr-x   0 bas       (1000) bas       (1000)        0 2023-08-01 12:02:45.732144 struct-bias-1.2.4/BIAS/models/opt_cnn_model-30/variables/
+-rw-r--r--   0 bas       (1000) bas       (1000)   102121 2023-08-01 11:43:06.000000 struct-bias-1.2.4/BIAS/models/opt_cnn_model-30/variables/variables.data-00000-of-00001
+-rw-r--r--   0 bas       (1000) bas       (1000)      907 2023-08-01 11:43:06.000000 struct-bias-1.2.4/BIAS/models/opt_cnn_model-30/variables/variables.index
+drwxr-xr-x   0 bas       (1000) bas       (1000)        0 2023-08-01 12:02:45.732144 struct-bias-1.2.4/BIAS/models/opt_cnn_model-50/
+-rw-r--r--   0 bas       (1000) bas       (1000)    20033 2023-08-01 11:43:07.000000 struct-bias-1.2.4/BIAS/models/opt_cnn_model-50/keras_metadata.pb
+-rw-r--r--   0 bas       (1000) bas       (1000)   129724 2023-08-01 11:43:07.000000 struct-bias-1.2.4/BIAS/models/opt_cnn_model-50/saved_model.pb
+drwxr-xr-x   0 bas       (1000) bas       (1000)        0 2023-08-01 12:02:45.732144 struct-bias-1.2.4/BIAS/models/opt_cnn_model-50/variables/
+-rw-r--r--   0 bas       (1000) bas       (1000)   114921 2023-08-01 11:43:06.000000 struct-bias-1.2.4/BIAS/models/opt_cnn_model-50/variables/variables.data-00000-of-00001
+-rw-r--r--   0 bas       (1000) bas       (1000)      907 2023-08-01 11:43:06.000000 struct-bias-1.2.4/BIAS/models/opt_cnn_model-50/variables/variables.index
+drwxr-xr-x   0 bas       (1000) bas       (1000)        0 2023-08-01 12:02:45.732144 struct-bias-1.2.4/BIAS/models/opt_cnn_model-500/
+-rw-r--r--   0 bas       (1000) bas       (1000)    19023 2023-08-01 11:43:08.000000 struct-bias-1.2.4/BIAS/models/opt_cnn_model-500/keras_metadata.pb
+-rw-r--r--   0 bas       (1000) bas       (1000)   117952 2023-08-01 11:43:08.000000 struct-bias-1.2.4/BIAS/models/opt_cnn_model-500/saved_model.pb
+drwxr-xr-x   0 bas       (1000) bas       (1000)        0 2023-08-01 12:02:45.732144 struct-bias-1.2.4/BIAS/models/opt_cnn_model-500/variables/
+-rw-r--r--   0 bas       (1000) bas       (1000)   930454 2023-08-01 11:43:08.000000 struct-bias-1.2.4/BIAS/models/opt_cnn_model-500/variables/variables.data-00000-of-00001
+-rw-r--r--   0 bas       (1000) bas       (1000)      907 2023-08-01 11:43:08.000000 struct-bias-1.2.4/BIAS/models/opt_cnn_model-500/variables/variables.index
+drwxr-xr-x   0 bas       (1000) bas       (1000)        0 2023-08-01 12:02:45.732144 struct-bias-1.2.4/BIAS/models/opt_cnn_model-600/
+-rw-r--r--   0 bas       (1000) bas       (1000)    24647 2023-08-01 11:43:09.000000 struct-bias-1.2.4/BIAS/models/opt_cnn_model-600/keras_metadata.pb
+-rw-r--r--   0 bas       (1000) bas       (1000)   132148 2023-08-01 11:43:09.000000 struct-bias-1.2.4/BIAS/models/opt_cnn_model-600/saved_model.pb
+drwxr-xr-x   0 bas       (1000) bas       (1000)        0 2023-08-01 12:02:45.732144 struct-bias-1.2.4/BIAS/models/opt_cnn_model-600/variables/
+-rw-r--r--   0 bas       (1000) bas       (1000)   788239 2023-08-01 11:43:09.000000 struct-bias-1.2.4/BIAS/models/opt_cnn_model-600/variables/variables.data-00000-of-00001
+-rw-r--r--   0 bas       (1000) bas       (1000)     1007 2023-08-01 11:43:09.000000 struct-bias-1.2.4/BIAS/models/opt_cnn_model-600/variables/variables.index
+-rw-r--r--   0 bas       (1000) bas       (1000)      350 2023-06-16 06:53:49.000000 struct-bias-1.2.4/BIAS/models/targetnames.npy
+-rw-r--r--   0 bas       (1000) bas       (1000)     1632 2022-11-29 08:36:48.000000 struct-bias-1.2.4/LICENSE.md
+-rw-r--r--   0 bas       (1000) bas       (1000)     3503 2023-08-01 12:02:45.732144 struct-bias-1.2.4/PKG-INFO
+-rw-r--r--   0 bas       (1000) bas       (1000)     3138 2023-08-01 11:43:58.000000 struct-bias-1.2.4/README.md
+-rw-r--r--   0 bas       (1000) bas       (1000)       38 2023-08-01 12:02:45.732144 struct-bias-1.2.4/setup.cfg
+-rw-r--r--   0 bas       (1000) bas       (1000)     1202 2023-08-01 12:01:44.000000 struct-bias-1.2.4/setup.py
+drwxr-xr-x   0 bas       (1000) bas       (1000)        0 2023-08-01 12:02:45.732144 struct-bias-1.2.4/struct_bias.egg-info/
+-rw-r--r--   0 bas       (1000) bas       (1000)     3503 2023-08-01 12:02:45.000000 struct-bias-1.2.4/struct_bias.egg-info/PKG-INFO
+-rw-r--r--   0 bas       (1000) bas       (1000)     1651 2023-08-01 12:02:45.000000 struct-bias-1.2.4/struct_bias.egg-info/SOURCES.txt
+-rw-r--r--   0 bas       (1000) bas       (1000)        1 2023-08-01 12:02:45.000000 struct-bias-1.2.4/struct_bias.egg-info/dependency_links.txt
+-rw-r--r--   0 bas       (1000) bas       (1000)       85 2023-08-01 12:02:45.000000 struct-bias-1.2.4/struct_bias.egg-info/requires.txt
+-rw-r--r--   0 bas       (1000) bas       (1000)        5 2023-08-01 12:02:45.000000 struct-bias-1.2.4/struct_bias.egg-info/top_level.txt
```

### Comparing `struct-bias-1.2.3/BIAS/Create_RF.py` & `struct-bias-1.2.4/BIAS/Create_RF.py`

 * *Files identical despite different names*

### Comparing `struct-bias-1.2.3/BIAS/SB_Test_runner.py` & `struct-bias-1.2.4/BIAS/SB_Test_runner.py`

 * *Files identical despite different names*

### Comparing `struct-bias-1.2.3/BIAS/SB_Toolbox.py` & `struct-bias-1.2.4/BIAS/SB_Toolbox.py`

 * *Files 1% similar despite different names*

```diff
@@ -421,15 +421,15 @@
         n_samples = data.shape[0]
         if not n_samples in [30, 50, 100, 600]:
             raise ValueError("Sample size is not supported")
         if self.deepmodel == None:
             dirname = os.path.dirname(__file__)
             # download RF models if needed from
             self.deepmodel = tf.keras.models.load_model(
-                f"{dirname}/models/opt_cnn_model-{n_samples}.h5"
+                f"{dirname}/models/opt_cnn_model-{n_samples}"
             )
             self.targetnames = np.load(
                 f"{dirname}/models/targetnames.npy", allow_pickle=True
             )
             # loading explainable background samples and loading the explainer
             self.xai_background = getXAIBackground(data.shape[0])
             self.explainer = shap.DeepExplainer(self.deepmodel, self.xai_background)
```

### Comparing `struct-bias-1.2.3/BIAS/install.r` & `struct-bias-1.2.4/BIAS/install.r`

 * *Files identical despite different names*

### Comparing `struct-bias-1.2.3/LICENSE.md` & `struct-bias-1.2.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `struct-bias-1.2.3/PKG-INFO` & `struct-bias-1.2.4/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: struct-bias
-Version: 1.2.3
+Version: 1.2.4
 Summary: BIAS toolbox: Structural bias detection for continuous optimization algorithms
 Author: Diederick Vermetten, Niki van Stein
 Author-email: d.l.vermetten@liacs.leidenuniv.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -13,27 +13,40 @@
 
 # Deep-BIAS: Bias In Algorithms, Structural
 ## A toolbox for detecting structural bias in continuous optimization heuristics.
 ## With a deep-learning extension to better evaluate the type of bias and gain insights using explainable AI
 
 ## Setup
 
-This package requires an R-installation to be present, with the following packages installed:
+This package requires an R-installation to be present.
+
+The R packages can be installed with the `install_r_packages` command from the BIAS toolbox.
+
+Install the BIAS toolbox using pip:
+
+    pip install struct-bias
+
+Then install the required R packages
+
+```py
+from BIAS import install_r_packages
+
+#run first time to install required R packages
+install_r_packages()
+```
+
+This installs the following R packages:
+
 - PoweR
 - AutoSEARCH
 - nortest
 - data.table
 - goftest
 - ddst
 
-Then install via pip:
-
-    pip install struct-bias
-
-
 ### Detailed setup using virtual env
 
 1. Download and install R from https://cran.r-project.org/
 2. Download this repository (clone or as zip)
 3. Create a python virtual env `python -m venv env`
 4. Activate the env (in powershell for example: `env/Scripts/Activate.ps1 `)
 5. Install dependencies `pip install -r requirements.txt`
@@ -71,7 +84,35 @@
 ```
 
 ## Additional files
 
 Note: The code for generating the RF used to predict the type of bias is included, but the full RF is not. These can be found on zenodo: https://doi.org/10.6084/m9.figshare.16546041.
 The RF models will be downloaded automatically the first time the predict function requires them.
 
+### Citation
+
+If you use the BIAS toolbox in a scientific publication, we would appreciate using the following citations:
+
+```
+@ARTICLE{9828803,
+  author={Vermetten, Diederick and van Stein, Bas and Caraffini, Fabio and Minku, Leandro L. and Kononova, Anna V.},
+  journal={IEEE Transactions on Evolutionary Computation}, 
+  title={BIAS: A Toolbox for Benchmarking Structural Bias in the Continuous Domain}, 
+  year={2022},
+  volume={26},
+  number={6},
+  pages={1380-1393},
+  doi={10.1109/TEVC.2022.3189848}
+}
+
+@software{niki_van_stein_2023_7803623,
+  author       = {Niki van Stein and
+                  Diederick Vermetten},
+  title        = {Basvanstein/BIAS: v1.1 Deep-BIAS Toolbox},
+  month        = apr,
+  year         = 2023,
+  publisher    = {Zenodo},
+  version      = {v1.1},
+  doi          = {10.5281/zenodo.7803623},
+  url          = {https://doi.org/10.5281/zenodo.7803623}
+}
+```
```

### Comparing `struct-bias-1.2.3/README.md` & `struct-bias-1.2.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,39 @@
 # Deep-BIAS: Bias In Algorithms, Structural
 ## A toolbox for detecting structural bias in continuous optimization heuristics.
 ## With a deep-learning extension to better evaluate the type of bias and gain insights using explainable AI
 
 ## Setup
 
-This package requires an R-installation to be present, with the following packages installed:
+This package requires an R-installation to be present.
+
+The R packages can be installed with the `install_r_packages` command from the BIAS toolbox.
+
+Install the BIAS toolbox using pip:
+
+    pip install struct-bias
+
+Then install the required R packages
+
+```py
+from BIAS import install_r_packages
+
+#run first time to install required R packages
+install_r_packages()
+```
+
+This installs the following R packages:
+
 - PoweR
 - AutoSEARCH
 - nortest
 - data.table
 - goftest
 - ddst
 
-Then install via pip:
-
-    pip install struct-bias
-
-
 ### Detailed setup using virtual env
 
 1. Download and install R from https://cran.r-project.org/
 2. Download this repository (clone or as zip)
 3. Create a python virtual env `python -m venv env`
 4. Activate the env (in powershell for example: `env/Scripts/Activate.ps1 `)
 5. Install dependencies `pip install -r requirements.txt`
@@ -58,7 +71,35 @@
 ```
 
 ## Additional files
 
 Note: The code for generating the RF used to predict the type of bias is included, but the full RF is not. These can be found on zenodo: https://doi.org/10.6084/m9.figshare.16546041.
 The RF models will be downloaded automatically the first time the predict function requires them.
 
+### Citation
+
+If you use the BIAS toolbox in a scientific publication, we would appreciate using the following citations:
+
+```
+@ARTICLE{9828803,
+  author={Vermetten, Diederick and van Stein, Bas and Caraffini, Fabio and Minku, Leandro L. and Kononova, Anna V.},
+  journal={IEEE Transactions on Evolutionary Computation}, 
+  title={BIAS: A Toolbox for Benchmarking Structural Bias in the Continuous Domain}, 
+  year={2022},
+  volume={26},
+  number={6},
+  pages={1380-1393},
+  doi={10.1109/TEVC.2022.3189848}
+}
+
+@software{niki_van_stein_2023_7803623,
+  author       = {Niki van Stein and
+                  Diederick Vermetten},
+  title        = {Basvanstein/BIAS: v1.1 Deep-BIAS Toolbox},
+  month        = apr,
+  year         = 2023,
+  publisher    = {Zenodo},
+  version      = {v1.1},
+  doi          = {10.5281/zenodo.7803623},
+  url          = {https://doi.org/10.5281/zenodo.7803623}
+}
+```
```

### Comparing `struct-bias-1.2.3/setup.py` & `struct-bias-1.2.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
-__version__ = "1.2.3"
+__version__ = "1.2.4"
 gh_ref = os.environ.get("GITHUB_REF")
 if gh_ref:
     *_, tag = gh_ref.split("/")
     __version__ = tag.replace("v", "")
 
 setuptools.setup(
     name='struct-bias',
@@ -16,15 +16,15 @@
     author="Diederick Vermetten, Niki van Stein",
     author_email="d.l.vermetten@liacs.leidenuniv.nl",
     description="BIAS toolbox: Structural bias detection for continuous optimization algorithms",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     package_data={
-        'BIAS': ['install.r'],
+        'BIAS': ['install.r', 'models/opt_cnn_model-*/*'],
     },
     python_requires='>=3.6',
     install_requires=[
         'numpy',
         'tensorflow',
         'shap',
         'rpy2',
```

### Comparing `struct-bias-1.2.3/struct_bias.egg-info/PKG-INFO` & `struct-bias-1.2.4/struct_bias.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: struct-bias
-Version: 1.2.3
+Version: 1.2.4
 Summary: BIAS toolbox: Structural bias detection for continuous optimization algorithms
 Author: Diederick Vermetten, Niki van Stein
 Author-email: d.l.vermetten@liacs.leidenuniv.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -13,27 +13,40 @@
 
 # Deep-BIAS: Bias In Algorithms, Structural
 ## A toolbox for detecting structural bias in continuous optimization heuristics.
 ## With a deep-learning extension to better evaluate the type of bias and gain insights using explainable AI
 
 ## Setup
 
-This package requires an R-installation to be present, with the following packages installed:
+This package requires an R-installation to be present.
+
+The R packages can be installed with the `install_r_packages` command from the BIAS toolbox.
+
+Install the BIAS toolbox using pip:
+
+    pip install struct-bias
+
+Then install the required R packages
+
+```py
+from BIAS import install_r_packages
+
+#run first time to install required R packages
+install_r_packages()
+```
+
+This installs the following R packages:
+
 - PoweR
 - AutoSEARCH
 - nortest
 - data.table
 - goftest
 - ddst
 
-Then install via pip:
-
-    pip install struct-bias
-
-
 ### Detailed setup using virtual env
 
 1. Download and install R from https://cran.r-project.org/
 2. Download this repository (clone or as zip)
 3. Create a python virtual env `python -m venv env`
 4. Activate the env (in powershell for example: `env/Scripts/Activate.ps1 `)
 5. Install dependencies `pip install -r requirements.txt`
@@ -71,7 +84,35 @@
 ```
 
 ## Additional files
 
 Note: The code for generating the RF used to predict the type of bias is included, but the full RF is not. These can be found on zenodo: https://doi.org/10.6084/m9.figshare.16546041.
 The RF models will be downloaded automatically the first time the predict function requires them.
 
+### Citation
+
+If you use the BIAS toolbox in a scientific publication, we would appreciate using the following citations:
+
+```
+@ARTICLE{9828803,
+  author={Vermetten, Diederick and van Stein, Bas and Caraffini, Fabio and Minku, Leandro L. and Kononova, Anna V.},
+  journal={IEEE Transactions on Evolutionary Computation}, 
+  title={BIAS: A Toolbox for Benchmarking Structural Bias in the Continuous Domain}, 
+  year={2022},
+  volume={26},
+  number={6},
+  pages={1380-1393},
+  doi={10.1109/TEVC.2022.3189848}
+}
+
+@software{niki_van_stein_2023_7803623,
+  author       = {Niki van Stein and
+                  Diederick Vermetten},
+  title        = {Basvanstein/BIAS: v1.1 Deep-BIAS Toolbox},
+  month        = apr,
+  year         = 2023,
+  publisher    = {Zenodo},
+  version      = {v1.1},
+  doi          = {10.5281/zenodo.7803623},
+  url          = {https://doi.org/10.5281/zenodo.7803623}
+}
+```
```

