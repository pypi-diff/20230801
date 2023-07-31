# Comparing `tmp/pqam_dparamhu2021-0.1.5.tar.gz` & `tmp/pqam_dparamhu2021-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pqam_dparamhu2021-0.1.5.tar", last modified: Tue May  2 16:27:48 2023, max compression
+gzip compressed data, was "pqam_dparamhu2021-0.1.6.tar", last modified: Mon Jul 31 23:27:28 2023, max compression
```

## Comparing `pqam_dparamhu2021-0.1.5.tar` & `pqam_dparamhu2021-0.1.6.tar`

### file list

```diff
@@ -1,28 +1,30 @@
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-05-02 16:27:48.383468 pqam_dparamhu2021-0.1.5/
--rw-r--r--   0 adam       (501) staff       (20)       37 2023-04-28 20:32:16.000000 pqam_dparamhu2021-0.1.5/MANIFEST.in
--rw-r--r--   0 adam       (501) staff       (20)     4600 2023-05-02 16:27:48.383320 pqam_dparamhu2021-0.1.5/PKG-INFO
--rw-r--r--   0 adam       (501) staff       (20)     3734 2023-05-02 16:27:13.000000 pqam_dparamhu2021-0.1.5/README.md
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-05-02 16:27:48.381745 pqam_dparamhu2021-0.1.5/pqam_dparamhu2021/
--rw-r--r--   0 adam       (501) staff       (20)     1029 2023-05-02 16:17:29.000000 pqam_dparamhu2021-0.1.5/pqam_dparamhu2021/HEA_pred.R
--rw-r--r--   0 adam       (501) staff       (20)     1710 2023-04-28 19:43:08.000000 pqam_dparamhu2021-0.1.5/pqam_dparamhu2021/LICENSE
--rw-r--r--   0 adam       (501) staff       (20)       37 2023-04-28 20:51:33.000000 pqam_dparamhu2021-0.1.5/pqam_dparamhu2021/__init__.py
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-05-02 16:27:48.382999 pqam_dparamhu2021-0.1.5/pqam_dparamhu2021/__pycache__/
--rw-r--r--   0 adam       (501) staff       (20)      206 2023-04-28 20:53:13.000000 pqam_dparamhu2021-0.1.5/pqam_dparamhu2021/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 adam       (501) staff       (20)     2479 2023-05-02 16:17:34.000000 pqam_dparamhu2021-0.1.5/pqam_dparamhu2021/__pycache__/model.cpython-39.pyc
--rw-r--r--   0 adam       (501) staff       (20)     1693 2023-04-28 20:56:11.000000 pqam_dparamhu2021-0.1.5/pqam_dparamhu2021/descriptors_gen_dev_predict_gsf.R
--rw-r--r--   0 adam       (501) staff       (20)     1704 2023-04-28 20:56:11.000000 pqam_dparamhu2021-0.1.5/pqam_dparamhu2021/descriptors_gen_dev_predict_surf.R
--rw-r--r--   0 adam       (501) staff       (20)      158 1979-11-30 04:00:00.000000 pqam_dparamhu2021-0.1.5/pqam_dparamhu2021/elemental_features.csv
--rw-r--r--   0 adam       (501) staff       (20)    12504 1979-11-30 04:00:00.000000 pqam_dparamhu2021-0.1.5/pqam_dparamhu2021/features_gsf.Rdata
--rw-r--r--   0 adam       (501) staff       (20)    12683 1979-11-30 04:00:00.000000 pqam_dparamhu2021-0.1.5/pqam_dparamhu2021/features_surf.Rdata
--rw-r--r--   0 adam       (501) staff       (20)    16646 1979-11-30 04:00:00.000000 pqam_dparamhu2021-0.1.5/pqam_dparamhu2021/gbm-locfit.R
--rw-r--r--   0 adam       (501) staff       (20)  5181124 1979-11-30 04:00:00.000000 pqam_dparamhu2021-0.1.5/pqam_dparamhu2021/locfit_3_var_all.Rdata
--rw-r--r--   0 adam       (501) staff       (20)  1855653 1979-11-30 04:00:00.000000 pqam_dparamhu2021-0.1.5/pqam_dparamhu2021/locfit_surf_2_var_all.Rdata
--rw-r--r--   0 adam       (501) staff       (20)     2107 2023-05-02 16:22:36.000000 pqam_dparamhu2021-0.1.5/pqam_dparamhu2021/model.py
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-05-02 16:27:48.382604 pqam_dparamhu2021-0.1.5/pqam_dparamhu2021.egg-info/
--rw-r--r--   0 adam       (501) staff       (20)     4600 2023-05-02 16:27:48.000000 pqam_dparamhu2021-0.1.5/pqam_dparamhu2021.egg-info/PKG-INFO
--rw-r--r--   0 adam       (501) staff       (20)      796 2023-05-02 16:27:48.000000 pqam_dparamhu2021-0.1.5/pqam_dparamhu2021.egg-info/SOURCES.txt
--rw-r--r--   0 adam       (501) staff       (20)        1 2023-05-02 16:27:48.000000 pqam_dparamhu2021-0.1.5/pqam_dparamhu2021.egg-info/dependency_links.txt
--rw-r--r--   0 adam       (501) staff       (20)       30 2023-05-02 16:27:48.000000 pqam_dparamhu2021-0.1.5/pqam_dparamhu2021.egg-info/requires.txt
--rw-r--r--   0 adam       (501) staff       (20)       18 2023-05-02 16:27:48.000000 pqam_dparamhu2021-0.1.5/pqam_dparamhu2021.egg-info/top_level.txt
--rw-r--r--   0 adam       (501) staff       (20)     1013 2023-05-02 16:27:40.000000 pqam_dparamhu2021-0.1.5/pyproject.toml
--rw-r--r--   0 adam       (501) staff       (20)       38 2023-05-02 16:27:48.383507 pqam_dparamhu2021-0.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 23:27:28.230455 pqam_dparamhu2021-0.1.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 23:27:28.218455 pqam_dparamhu2021-0.1.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 23:27:28.222455 pqam_dparamhu2021-0.1.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-31 23:27:10.000000 pqam_dparamhu2021-0.1.6/.github/workflows/publishPyPI.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-31 23:27:10.000000 pqam_dparamhu2021-0.1.6/.github/workflows/runtimeTest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-07-31 23:27:10.000000 pqam_dparamhu2021-0.1.6/.github/workflows/weeklyRuntimeTest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-31 23:27:10.000000 pqam_dparamhu2021-0.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-07-31 23:27:28.230455 pqam_dparamhu2021-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4689 2023-07-31 23:27:10.000000 pqam_dparamhu2021-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 23:27:28.230455 pqam_dparamhu2021-0.1.6/pqam_dparamhu2021/
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-31 23:27:10.000000 pqam_dparamhu2021-0.1.6/pqam_dparamhu2021/HEA_pred.R
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-07-31 23:27:10.000000 pqam_dparamhu2021-0.1.6/pqam_dparamhu2021/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-31 23:27:10.000000 pqam_dparamhu2021-0.1.6/pqam_dparamhu2021/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-07-31 23:27:10.000000 pqam_dparamhu2021-0.1.6/pqam_dparamhu2021/descriptors_gen_dev_predict_gsf.R
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-31 23:27:10.000000 pqam_dparamhu2021-0.1.6/pqam_dparamhu2021/descriptors_gen_dev_predict_surf.R
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-31 23:27:10.000000 pqam_dparamhu2021-0.1.6/pqam_dparamhu2021/elemental_features.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    12504 2023-07-31 23:27:10.000000 pqam_dparamhu2021-0.1.6/pqam_dparamhu2021/features_gsf.Rdata
+-rw-r--r--   0 runner    (1001) docker     (123)    12683 2023-07-31 23:27:10.000000 pqam_dparamhu2021-0.1.6/pqam_dparamhu2021/features_surf.Rdata
+-rw-r--r--   0 runner    (1001) docker     (123)    16307 2023-07-31 23:27:10.000000 pqam_dparamhu2021-0.1.6/pqam_dparamhu2021/gbm-locfit.R
+-rw-r--r--   0 runner    (1001) docker     (123)  5181124 2023-07-31 23:27:10.000000 pqam_dparamhu2021-0.1.6/pqam_dparamhu2021/locfit_3_var_all.Rdata
+-rw-r--r--   0 runner    (1001) docker     (123)  1855653 2023-07-31 23:27:10.000000 pqam_dparamhu2021-0.1.6/pqam_dparamhu2021/locfit_surf_2_var_all.Rdata
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-07-31 23:27:10.000000 pqam_dparamhu2021-0.1.6/pqam_dparamhu2021/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 23:27:28.230455 pqam_dparamhu2021-0.1.6/pqam_dparamhu2021.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-07-31 23:27:28.000000 pqam_dparamhu2021-0.1.6/pqam_dparamhu2021.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-31 23:27:28.000000 pqam_dparamhu2021-0.1.6/pqam_dparamhu2021.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 23:27:28.000000 pqam_dparamhu2021-0.1.6/pqam_dparamhu2021.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-31 23:27:28.000000 pqam_dparamhu2021-0.1.6/pqam_dparamhu2021.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-31 23:27:28.000000 pqam_dparamhu2021-0.1.6/pqam_dparamhu2021.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-31 23:27:10.000000 pqam_dparamhu2021-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 23:27:28.230455 pqam_dparamhu2021-0.1.6/setup.cfg
```

### Comparing `pqam_dparamhu2021-0.1.5/PKG-INFO` & `pqam_dparamhu2021-0.1.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pqam_dparamhu2021
-Version: 0.1.5
-Summary: PyQAlloy-compatible Model for D Parameter prediction based on Hu2021
+Version: 0.1.6
+Summary: PyQAlloy-compatible Model for D Parameter prediction based on Hu 2021 (10.1016/j.actamat.2021.116800)
 Author-email: Adam Krajewski <ak@psu.edu>
 Project-URL: Homepage, https://github.com/amkrajewski/pqam-dparamhu2021
 Project-URL: Bug Tracker, https://github.com/amkrajewski/pqam-dparamhu2021/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -15,17 +15,31 @@
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # PyQAlloy-compatible Model for D Parameter prediction based on Hu2021
 
-This repository contains a PyQAlloy-compatible compositionalModel for D Parameter Prediction Based on Yong-Jie Hu 2021 (10.1016/j.actamat.2021.116800) that 
-accepts a chemical formula of an alloy or a pymatgen Composition object and returns the predicted Genralized Stacking Fault Energy (GSF), Surface Energy (Surf), and the 
-calculated D Parameter.
+Release: ![PyPI](https://img.shields.io/pypi/v/pqam-dparamhu2021)
+
+Tests: [![small runtime test](https://github.com/amkrajewski/pqam-dparamhu2021/actions/workflows/runtimeTest.yml/badge.svg)](https://github.com/amkrajewski/pqam-dparamhu2021/actions/workflows/runtimeTest.yml)
+
+License: [![License: LGPL v3](https://img.shields.io/badge/License-LGPL_v3-blue.svg)](https://www.gnu.org/licenses/lgpl-3.0)
+
+This repository contains a PyQAlloy-compatible compositionalModel, compatible with [ULTERA Database (ultera.org)](https://ultera.org) infrastructure, for D Parameter Prediction Based on [Yong-Jie Hu 2021 (10.1016/j.actamat.2021.116800)](https://doi.org/10.1016/j.actamat.2021.116800) that 
+accepts a chemical formula string of an alloy or a `pymatgen.Composition` object. It return:
+
+Output Order: [`gfse`, `surf`, `dparam`]
+
+Output Meaning (all based on [10.1016/j.actamat.2021.116800](https://doi.org/10.1016/j.actamat.2021.116800)):
+- `gfse` - Genralized Stacking Fault Energy (GSF) [J/m^2]
+- `surf` - Surface Energy (Surf) [J/m^2]
+- `dparam` - D Parameter [unitless] calculated as `surf/gfse`
+
+
 
 ## Install and use
 
 To run this model you will need **Python 3.9+** and **R 4.1.0+** installed on your system, ideally **before** you install
 this software. For Python, we recommend you use a virtual Conda environment, which chan be created with minimal effort 
 (see [Miniconda install instructions](https://docs.conda.io/en/latest/miniconda.html)). For R, it can be downloaded 
 pre-compiled from a _Comprehensive R Archive Network_ repository (e.g. [Case CRAN](https://cran.case.edu)) and should 
@@ -44,14 +58,18 @@
 ***
 
 In some cases, required `locfit` R package may not be installed automatically. If you get an error message about it,
 try to go to your R console, typically by typing `R` in your terminal, and install it manually with:
 
     install.packages("locfit")
 
+Or, if you are automating things and need a single-liner, on Mac OS and Linux, the following should work:
+
+    Rscript -e "install.packages('locfit', repos='http://cran.us.r-project.org')"
+
 ## Attribution
 
 This repository has been created by Adam M. Krajewski (https://orcid.org/0000-0002-2266-0099) and is licensed under the MIT License. 
 **Please cite this repository if you use it in your work.**
 
 The featurizer and predictive model (HEA_pred.R and dependencies) have been optimized across and re-styled by Adam M.
 Krajewski based on code originally developed by Young-Jie Hu (https://orcid.org/0000-0003-1500-4015) et al. for their
@@ -64,18 +82,18 @@
 The gbm-locfit package (Gradient Boosting Machine-Locfit: A GBM framework using local regresssion via Locfit) has been 
 developed by Materials Project in 2016 and is distributed under the terms of the MIT License. Details can be found in
 its code.
 
 
 ## Hu's README File
 
-Hello, thank you for your interest in our work!
-Here we provide a script written in R language to take an alloy composition of interest and correspondingly predict the GSF energy, surface energy, and the ductility parameter based on the SL models in our manuscript ( https://doi.org/10.1016/j.actamat.2021.116800)
-To run the script and make predictions, you need to:
-1)	Download the RStudio platform. (https://www.rstudio.com/) ## No worry, it is open access 😊
-2)	Put all the files you downloaded from Materials Commons (basically all our files) into one local folder
-3)	Open the “predict.R” file in RStudio, input the alloy composition there, execute every line there, and the prediction will jump out in the console window below. 
-
-Please contact qiliang@umich.edu or yh593@drexel.edu if you have any questions. 
-
-P.S.,
-“predict_screen_4nary_all.csv” is the original data for plotting Figure 7&8 in the manuscript. Other figures in the manuscript can be reproduced by the data listed in the tables in the manuscript.
+>Hello, thank you for your interest in our work!
+>Here we provide a script written in R language to take an alloy composition of interest and correspondingly predict the GSF energy, surface energy, and the >ductility parameter based on the SL models in our manuscript ( https://doi.org/10.1016/j.actamat.2021.116800)
+>To run the script and make predictions, you need to:
+>1)	Download the RStudio platform. (https://www.rstudio.com/) ## No worry, it is open access 😊
+>2)	Put all the files you downloaded from Materials Commons (basically all our files) into one local folder
+>3)	Open the “predict.R” file in RStudio, input the alloy composition there, execute every line there, and the prediction will jump out in the console window >below. 
+>
+>Please contact qiliang@umich.edu or yh593@drexel.edu if you have any questions. 
+>
+>P.S.,
+>“predict_screen_4nary_all.csv” is the original data for plotting Figure 7&8 in the manuscript. Other figures in the manuscript can be reproduced by the data >listed in the tables in the manuscript.
```

### Comparing `pqam_dparamhu2021-0.1.5/README.md` & `pqam_dparamhu2021-0.1.6/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,26 @@
 # PyQAlloy-compatible Model for D Parameter prediction based on Hu2021
 
-This repository contains a PyQAlloy-compatible compositionalModel for D Parameter Prediction Based on Yong-Jie Hu 2021 (10.1016/j.actamat.2021.116800) that 
-accepts a chemical formula of an alloy or a pymatgen Composition object and returns the predicted Genralized Stacking Fault Energy (GSF), Surface Energy (Surf), and the 
-calculated D Parameter.
+Release: ![PyPI](https://img.shields.io/pypi/v/pqam-dparamhu2021)
+
+Tests: [![small runtime test](https://github.com/amkrajewski/pqam-dparamhu2021/actions/workflows/runtimeTest.yml/badge.svg)](https://github.com/amkrajewski/pqam-dparamhu2021/actions/workflows/runtimeTest.yml)
+
+License: [![License: LGPL v3](https://img.shields.io/badge/License-LGPL_v3-blue.svg)](https://www.gnu.org/licenses/lgpl-3.0)
+
+This repository contains a PyQAlloy-compatible compositionalModel, compatible with [ULTERA Database (ultera.org)](https://ultera.org) infrastructure, for D Parameter Prediction Based on [Yong-Jie Hu 2021 (10.1016/j.actamat.2021.116800)](https://doi.org/10.1016/j.actamat.2021.116800) that 
+accepts a chemical formula string of an alloy or a `pymatgen.Composition` object. It return:
+
+Output Order: [`gfse`, `surf`, `dparam`]
+
+Output Meaning (all based on [10.1016/j.actamat.2021.116800](https://doi.org/10.1016/j.actamat.2021.116800)):
+- `gfse` - Genralized Stacking Fault Energy (GSF) [J/m^2]
+- `surf` - Surface Energy (Surf) [J/m^2]
+- `dparam` - D Parameter [unitless] calculated as `surf/gfse`
+
+
 
 ## Install and use
 
 To run this model you will need **Python 3.9+** and **R 4.1.0+** installed on your system, ideally **before** you install
 this software. For Python, we recommend you use a virtual Conda environment, which chan be created with minimal effort 
 (see [Miniconda install instructions](https://docs.conda.io/en/latest/miniconda.html)). For R, it can be downloaded 
 pre-compiled from a _Comprehensive R Archive Network_ repository (e.g. [Case CRAN](https://cran.case.edu)) and should 
@@ -25,14 +39,18 @@
 ***
 
 In some cases, required `locfit` R package may not be installed automatically. If you get an error message about it,
 try to go to your R console, typically by typing `R` in your terminal, and install it manually with:
 
     install.packages("locfit")
 
+Or, if you are automating things and need a single-liner, on Mac OS and Linux, the following should work:
+
+    Rscript -e "install.packages('locfit', repos='http://cran.us.r-project.org')"
+
 ## Attribution
 
 This repository has been created by Adam M. Krajewski (https://orcid.org/0000-0002-2266-0099) and is licensed under the MIT License. 
 **Please cite this repository if you use it in your work.**
 
 The featurizer and predictive model (HEA_pred.R and dependencies) have been optimized across and re-styled by Adam M.
 Krajewski based on code originally developed by Young-Jie Hu (https://orcid.org/0000-0003-1500-4015) et al. for their
@@ -45,18 +63,18 @@
 The gbm-locfit package (Gradient Boosting Machine-Locfit: A GBM framework using local regresssion via Locfit) has been 
 developed by Materials Project in 2016 and is distributed under the terms of the MIT License. Details can be found in
 its code.
 
 
 ## Hu's README File
 
-Hello, thank you for your interest in our work!
-Here we provide a script written in R language to take an alloy composition of interest and correspondingly predict the GSF energy, surface energy, and the ductility parameter based on the SL models in our manuscript ( https://doi.org/10.1016/j.actamat.2021.116800)
-To run the script and make predictions, you need to:
-1)	Download the RStudio platform. (https://www.rstudio.com/) ## No worry, it is open access 😊
-2)	Put all the files you downloaded from Materials Commons (basically all our files) into one local folder
-3)	Open the “predict.R” file in RStudio, input the alloy composition there, execute every line there, and the prediction will jump out in the console window below. 
-
-Please contact qiliang@umich.edu or yh593@drexel.edu if you have any questions. 
-
-P.S.,
-“predict_screen_4nary_all.csv” is the original data for plotting Figure 7&8 in the manuscript. Other figures in the manuscript can be reproduced by the data listed in the tables in the manuscript.
+>Hello, thank you for your interest in our work!
+>Here we provide a script written in R language to take an alloy composition of interest and correspondingly predict the GSF energy, surface energy, and the >ductility parameter based on the SL models in our manuscript ( https://doi.org/10.1016/j.actamat.2021.116800)
+>To run the script and make predictions, you need to:
+>1)	Download the RStudio platform. (https://www.rstudio.com/) ## No worry, it is open access 😊
+>2)	Put all the files you downloaded from Materials Commons (basically all our files) into one local folder
+>3)	Open the “predict.R” file in RStudio, input the alloy composition there, execute every line there, and the prediction will jump out in the console window >below. 
+>
+>Please contact qiliang@umich.edu or yh593@drexel.edu if you have any questions. 
+>
+>P.S.,
+>“predict_screen_4nary_all.csv” is the original data for plotting Figure 7&8 in the manuscript. Other figures in the manuscript can be reproduced by the data >listed in the tables in the manuscript.
```

### Comparing `pqam_dparamhu2021-0.1.5/pqam_dparamhu2021/HEA_pred.R` & `pqam_dparamhu2021-0.1.6/pqam_dparamhu2021/HEA_pred.R`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-init <- function (path) {
-  source(paste(path,"/descriptors_gen_dev_predict_surf.R", sep = ""))
-  source(paste(path,"/descriptors_gen_dev_predict_gsf.R", sep = ""))
-  source(paste(path,"/gbm-locfit.R", sep = ""))
-  load(paste(path,"/locfit_3_var_all.Rdata", sep = ""))
-  model_gsf <<- model
-  load(paste(path,"/locfit_surf_2_var_all.Rdata", sep = ""))
-  model_surf <<- model
-  return('init done')
-}
-
-HEA_pred <- function(composition = composition, path) {
-  descriptors.gsf <- des_gsf(comp = composition, path = path)
-  descriptors.surf <- des_surf(comp = composition, path = path)
-  sel <- c(1:26, 35:38)
-  descriptors.gsf <- as.matrix(descriptors.gsf[, sel])
-  descriptors.surf <- as.matrix(descriptors.surf[, sel])
-  pre.gsf <- predict.gbm.locfit(model_gsf, descriptors.gsf)
-  pre.surf <- predict.gbm.locfit(model_surf, descriptors.surf)
-  D <- pre.surf[2] / pre.gsf[2]
-  result <- t(as.matrix(c(pre.gsf[2], pre.surf[2], D)))
-  colnames(result) <- c("GSF", "Surface", "D parameter")
-  return(result)
-}
+init <- function (path) {
+  source(paste(path,"/descriptors_gen_dev_predict_surf.R", sep = ""))
+  source(paste(path,"/descriptors_gen_dev_predict_gsf.R", sep = ""))
+  source(paste(path,"/gbm-locfit.R", sep = ""))
+  load(paste(path,"/locfit_3_var_all.Rdata", sep = ""))
+  model_gsf <<- model
+  load(paste(path,"/locfit_surf_2_var_all.Rdata", sep = ""))
+  model_surf <<- model
+  return('init done')
+}
+
+HEA_pred <- function(composition = composition, path) {
+  descriptors.gsf <- des_gsf(comp = composition, path = path)
+  descriptors.surf <- des_surf(comp = composition, path = path)
+  sel <- c(1:26, 35:38)
+  descriptors.gsf <- as.matrix(descriptors.gsf[, sel])
+  descriptors.surf <- as.matrix(descriptors.surf[, sel])
+  pre.gsf <- predict.gbm.locfit(model_gsf, descriptors.gsf)
+  pre.surf <- predict.gbm.locfit(model_surf, descriptors.surf)
+  D <- pre.surf[2] / pre.gsf[2]
+  result <- t(as.matrix(c(pre.gsf[2], pre.surf[2], D)))
+  colnames(result) <- c("GSF", "Surface", "D parameter")
+  return(result)
+}
```

### Comparing `pqam_dparamhu2021-0.1.5/pqam_dparamhu2021/descriptors_gen_dev_predict_surf.R` & `pqam_dparamhu2021-0.1.6/pqam_dparamhu2021/descriptors_gen_dev_predict_gsf.R`

 * *Files 27% similar despite different names*

```diff
@@ -1,54 +1,53 @@
-des_surf <- function(comp = comp, path) {
-  comp_n <- comp / sum(comp)
-  a <- c(1, 1, 1, 1, 1, 1, 1, 1, 1, 1)
-  data.1 <- data.frame(rbind(a, comp_n))
-
-  file.3 <- paste(path,"/elemental_features.csv", sep = "")
-  data.3 <- read.csv(file = file.3, header = T)
-  para_ele <- as.matrix(data.3[, 2:4])
-
-  load(file = paste(path,"/features_surf.Rdata", sep = ""))
-
-  feature.surf.select <- feature.surf.all
-  n.ob <- length(data.1[, 1])
-  n.feature <- length(feature.surf.select[1, 1,])
-  n.feature.ele <- length(para_ele[1,])
-  n.feature.all <- n.feature + n.feature.ele
-
-  parameter.surf <- array(0, c(n.ob, 10, n.feature))
-
-  comp_ele <- as.matrix(data.1)
-  for (i in seq(n.feature)) {
-    parameter.surf[, , i] <- comp_ele %*% as.matrix(feature.surf.select[, , i])
-  }
-
-  size <- 2 * n.feature.all
-  predictors <- array(0, c(n.ob, size))
-  for (i in seq(n.ob)) {
-    nonzvec <- which(comp_ele[i,] != 0)
-    avg1 <- NULL
-    for (k in seq(n.feature)) {
-      para.temp <- parameter.surf[i, nonzvec, k]
-      avgtemp <- para.temp %*% comp_ele[i, nonzvec]
-      dvetemp <- ((1 / (1 - sum(comp_ele[i, nonzvec]^2))) * ((para.temp - avgtemp[1])^2 %*% comp_ele[i, nonzvec]))^(1 / 2)
-      avg1 <- c(avg1, avgtemp, dvetemp)
-    }
-
-    avg2 <- NULL
-    for (n in seq(n.feature.ele)) {
-      avgtemp <- comp_ele[i, nonzvec] %*% para_ele[nonzvec, n]
-      dvetemp <- ((1 / (1 - sum(comp_ele[i, nonzvec]^2))) * ((para_ele[nonzvec, n] - avgtemp[1])^2 %*% comp_ele[i, nonzvec]))^(1 / 2)
-      avg2 <- c(avg2, avgtemp, dvetemp)
-    }
-    avg <- c(avg1, avg2)
-    predictors[i,] <- avg
-  }
-
-  all <- data.frame(predictors)
-  all[is.na(all)] <- 0
-  return(all)
-}
-
-
-
-
+des_gsf <- function(comp = comp, path) {
+  comp_n <- comp / sum(comp)
+  a <- c(1, 1, 1, 1, 1, 1, 1, 1, 1, 1)
+  data.1 <- data.frame(rbind(a, comp_n))
+
+  file.3 <- paste(path,"/elemental_features.csv", sep = "")
+  data.3 <- read.csv(file = file.3, header = T)
+  para_ele <- as.matrix(data.3[, 2:4])
+
+  load(file = paste(path,"/features_gsf.Rdata", sep = ""))
+
+  feature.gsf.select <- feature.gsf.all
+  n.ob <- length(data.1[, 1])
+  n.feature <- length(feature.gsf.select[1, 1,])
+  n.feature.ele <- length(para_ele[1,])
+  n.feature.all <- n.feature + n.feature.ele
+
+  parameter.gsf <- array(0, c(n.ob, 10, n.feature))
+
+  comp_ele <- as.matrix(data.1)
+  for (i in seq(n.feature)) {
+    parameter.gsf[, , i] <- comp_ele %*% as.matrix(feature.gsf.select[, , i])
+  }
+
+  size <- 2 * n.feature.all
+  predictors <- array(0, c(n.ob, size))
+  for (i in seq(n.ob)) {
+    nonzvec <- which(comp_ele[i,] != 0)
+    avg1 <- NULL
+    for (k in seq(n.feature)) {
+      para.temp <- parameter.gsf[i, nonzvec, k]
+      avgtemp <- para.temp %*% comp_ele[i, nonzvec]
+      dvetemp <- ((1 / (1 - sum(comp_ele[i, nonzvec]^2))) * ((para.temp - avgtemp[1])^2 %*% comp_ele[i, nonzvec]))^(1 / 2)
+      avg1 <- c(avg1, avgtemp, dvetemp)
+    }
+
+    avg2 <- NULL
+    for (n in seq(n.feature.ele)) {
+      avgtemp <- comp_ele[i, nonzvec] %*% para_ele[nonzvec, n]
+      dvetemp <- ((1 / (1 - sum(comp_ele[i, nonzvec]^2))) * ((para_ele[nonzvec, n] - avgtemp[1])^2 %*% comp_ele[i, nonzvec]))^(1 / 2)
+      avg2 <- c(avg2, avgtemp, dvetemp)
+    }
+    avg <- c(avg1, avg2)
+    predictors[i,] <- avg
+  }
+
+
+  all <- data.frame(predictors)
+  all[is.na(all)] <- 0
+  return(all)
+}
+
+
```

### Comparing `pqam_dparamhu2021-0.1.5/pqam_dparamhu2021/features_gsf.Rdata` & `pqam_dparamhu2021-0.1.6/pqam_dparamhu2021/features_gsf.Rdata`

 * *Files identical despite different names*

### Comparing `pqam_dparamhu2021-0.1.5/pqam_dparamhu2021/features_surf.Rdata` & `pqam_dparamhu2021-0.1.6/pqam_dparamhu2021/features_surf.Rdata`

 * *Files identical despite different names*

### Comparing `pqam_dparamhu2021-0.1.5/pqam_dparamhu2021/gbm-locfit.R` & `pqam_dparamhu2021-0.1.6/pqam_dparamhu2021/gbm-locfit.R`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,339 +1,339 @@
-# Gradient Boosting Machine-Locfit: A GBM framework using local regresssion via Locfit.
-# For information on Locfit see: http://ect.bell-labs.com/sl/project/locfit/index.html
-#
-# Copyright 2016, The Materials Project, LBNL
-# Distributed under the terms of the MIT License.
-#
-# Permission is hereby granted, free of charge, to any person obtaining a copy of
-# this software and associated documentation files (the "Software"), to deal in
-# the Software without restriction, including without limitation the rights to
-# use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
-# the Software, and to permit persons to whom the Software is furnished to do so,
-# subject to the following conditions:
-#
-# The above copyright notice and this permission notice shall be included in all
-# copies or substantial portions of the Software.
-#
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
-# FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
-# COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
-# IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
-# CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-
-
-# Function Name:         gbm.locfit
-# Version:               V1.2
-# Date:                  2015-09-16
-#
-# Function Description:  This function provides a cross-validation wrapper for gbm.locfit.core
-
-gbm.locfit <- function(predictors, response, n.interactions=1, n.steps=5, learning.rate=0.15, locfit.alpha=0.7,
-                       locfit.degree=1, cv.folds=10, seed.folds=NULL)
-{
-  # Variable checks and other preliminaries
-  require(locfit)
-  n.observations = length(response)
-  if (is.null(n.observations) || n.observations < 2) { message("Error: response must be a vector!"); return(1) }
-  predictors.dim = dim(predictors)
-  if (is.null(predictors.dim)) { message("Error: predictors must be a 2-D matrix!"); return(1) }
-  if (predictors.dim[1] != n.observations) { message("Error: lengths of response and predictors must match!"); return(1) }
-  n.predictors = predictors.dim[2]
-  if (n.predictors < 2) { message("Error: minimum of two predictors is required!"); return(1) }
-  if (is.null(n.interactions) || round(n.interactions) != n.interactions || n.interactions < 1 || n.interactions > 5)
-    { message("Error: n.interactions must be an integer between 1 and 5!"); return(1) }
-  if (n.interactions > n.predictors)
-    { message("Error: n.interactions may not exceed number of predictors!"); return(1) }
-  if (is.null(n.steps) || round(n.steps) != n.steps || n.steps < 1)
-    { message("Error: n.steps must be at least two!"); return(1) }
-  if (is.null(learning.rate) || learning.rate <= 0.0 || learning.rate >= 1.0)
-    { message("Error: learning.rate must of positive but less than 1!"); return(1) }
-  if (is.null(locfit.degree) || round(locfit.degree) != locfit.degree || locfit.degree < 1)
-    { message("Error: locfit.degree must be a positive integer!"); return(1) }
-  if (is.null(cv.folds) || round(cv.folds) != cv.folds || cv.folds <= 1)
-    { message("Error: cv.folds must be a positive integer, greater than one."); return(1) }
-
-  # Define CV sets
-  set.seed(seed.folds)
-  rounds = ceiling(n.observations / cv.folds)
-  sets = rep(seq(1, cv.folds), rounds)[seq(1, n.observations)]
-  sets = sample(sets, n.observations, replace=FALSE)  # random permutation
-  train.weights = rep(0, cv.folds);  train.mse.matrix = matrix(0, nrow=n.steps, ncol=cv.folds)
-  test.weights  = rep(0, cv.folds);  test.mse.matrix  = matrix(0, nrow=n.steps, ncol=cv.folds)
-
-  # Run CV models, dropping the test set from each run
-  for ( fold in seq(1, cv.folds) ) {
-    message("fold:",fold)
-    train.predictors = predictors[sets != fold, ];  test.predictors = predictors[sets == fold, ]
-    train.response = response[sets != fold];        test.response = response[sets == fold]
-    train.weights[fold] = length(train.response);   test.weights[fold] = length(test.response)
-
-    object = gbm.locfit.core(train.predictors, train.response, n.interactions=n.interactions, n.steps=n.steps,
-              learning.rate=learning.rate, locfit.alpha=locfit.alpha, locfit.degree=locfit.degree)
-
-    # Fill train.mse.matrix
-    train.mse.matrix[ , fold] = object$mean.squared.errors
-
-    # Fill test.mse.matrix
-    test.predicted.step = rep(object$response.mean, length=length(test.predictors[, 1]) )
-    for ( step in seq(1, n.steps) ) {
-      cat("\r",step)
-      # compute prediction error for each step, incrementally (for this fold)
-      test.predicted.step = incremental.predict.gbm.locfit(object, test.predictors, test.predicted.step, step)
-      test.mse.matrix[step, fold] = sum((test.response - test.predicted.step)^2) / length(test.response)
-  } }
-
-  # Normalize the train and test weights
-  train.weights = train.weights / sum(train.weights)
-  test.weights  = test.weights  / sum(test.weights)
-
-  # Calculate observed.errs, prediction.errs, and prediction.stderrs
-  observed.errs   = apply(train.mse.matrix, 1, weighted.mean, w=train.weights)
-  prediction.errs = apply(test.mse.matrix,  1, weighted.mean, w=test.weights)
-  prediction.stderrs = apply(test.mse.matrix, 1, weighted.sd, w=test.weights) / sqrt(cv.folds-1)
-  ns0 = which(prediction.errs == min(prediction.errs))
-  ns = min(which(prediction.errs < prediction.errs[ns0]+prediction.stderrs[ns0]))
-
-  # Run gbm.locfit.core again with all of the data, but only to ns0 steps
-  object = gbm.locfit.core(predictors, response, n.interactions=n.interactions, n.steps=ns0,
-            learning.rate=learning.rate, locfit.alpha=locfit.alpha, locfit.degree=locfit.degree)
-
-  list(locfit.list=object$locfit.list, predictor.list=object$predictor.list, learning.rate=learning.rate,
-      response.mean=object$response.mean, prediction.means=object$prediction.means,
-      locfit.alpha=locfit.alpha, locfit.degree=locfit.degree, cv.folds=cv.folds, observed.errs=observed.errs,
-      prediction.errs=prediction.errs, prediction.stderrs=prediction.stderrs, n.steps=n.steps, ns0=ns0, ns=ns)
-}
-
-
-# Function Name:         gbm.locfit.core
-# Version:               V1.1
-# Date:                  2015-07-02
-#
-# Function Description:  This function provides a gbm framework for locfit.
-
-gbm.locfit.core <- function(predictors, response, n.interactions=1, n.steps=5, learning.rate=0.15, locfit.alpha=0.7,
-                            locfit.degree=1, verbose=FALSE)
-{
-  # Variable checks and other preliminaries
-  require(locfit)
-  maxk=250
-  n.predictors = dim(predictors)[2]
-  response.mean = mean(response)
-  residual = response - response.mean  # Center response
-  locfit.list = vector(mode="list", length=n.steps)
-  predictor.list = vector(mode="list", length=n.steps)
-  prediction.means = rep(0, length=n.steps)
-  mean.squared.errors = rep(0, length=n.steps)
-
-  for (step in seq(1, n.steps)) {
-    mse.min = mean(residual^2)/learning.rate  # Set mse.min "high"
-    cat("\r",step)
-    if (n.interactions == 1) {
-      # Run locfit on individual predictors (first level interactions only)
-      for (predictor.i in seq(1, n.predictors)) {
-        predictors.tmp = predictors[, predictor.i]
-        locfit.i = locfit.raw(predictors.tmp, residual, alpha=locfit.alpha, deg=locfit.degree, maxk=maxk)
-        predicted.i = predict(locfit.i, newdata=predictors.tmp)
-        mse = mean((residual - predicted.i)^2)
-        if (verbose) cat(predictor.i, ": - :", mse, "\n")
-        if (mse < mse.min) {
-          mse.min=mse; predicted.step = predicted.i
-          predictor.list[[step]]=predictor.i; locfit.list[[step]]=locfit.i } }
-
-    } else if (n.interactions == 2) {
-      # Run locfit on pairs of predictors (first thru second level interactions)
-      for (predictor.i in seq(1, n.predictors-1)) {
-        for (predictor.j in seq(predictor.i+1, n.predictors)) {
-          predictor.ij = c(predictor.i, predictor.j)
-          predictors.tmp = predictors[, predictor.ij]
-          locfit.i = locfit.raw(predictors.tmp, residual, alpha=locfit.alpha, deg=locfit.degree, maxk=maxk)
-          predicted.i = predict(locfit.i, newdata=predictors.tmp)
-          mse = mean((residual - predicted.i)^2)
-          if (verbose) cat(predictor.i, ":", predictor.j, ":", mse, "\n")
-          if (mse < mse.min) {
-            mse.min=mse; predicted.step = predicted.i
-            predictor.list[[step]]=predictor.ij; locfit.list[[step]]=locfit.i } } }
-
-    } else if (n.interactions == 3) {
-      # Run locfit on triples of predictors (first thru third level interactions)
-      for (predictor.i in seq(1, n.predictors-2)) {
-        for (predictor.j in seq(predictor.i+1, n.predictors-1)) {
-          for (predictor.k in seq(predictor.j+1, n.predictors)) {
-            predictor.ijk = c(predictor.i, predictor.j, predictor.k)
-            predictors.tmp = predictors[, predictor.ijk]
-            locfit.i = locfit.raw(predictors.tmp, residual, alpha=locfit.alpha, deg=locfit.degree, maxk=maxk)
-            predicted.i = predict(locfit.i, newdata=predictors.tmp)
-            mse = mean((residual - predicted.i)^2)
-            if (verbose) cat(predictor.i, ":", predictor.j, ":", predictor.k, ":", mse, "\n")
-            if (mse < mse.min) {
-              mse.min=mse; predicted.step = predicted.i
-              predictor.list[[step]]=predictor.ijk; locfit.list[[step]]=locfit.i } } } }
-
-    } else if (n.interactions == 4) {
-      # Run locfit on quads of predictors (first thru fourth level interactions)
-      for (predictor.i in seq(1, n.predictors-3)) {
-        for (predictor.j in seq(predictor.i+1, n.predictors-2)) {
-          for (predictor.k in seq(predictor.j+1, n.predictors-1)) {
-            for (predictor.l in seq(predictor.k+1, n.predictors)) {
-              predictor.ijkl = c(predictor.i, predictor.j, predictor.k, predictor.l)
-              predictors.tmp = predictors[, predictor.ijkl]
-              locfit.i = locfit.raw(predictors.tmp, residual, alpha=locfit.alpha, deg=locfit.degree, maxk=maxk)
-              predicted.i = predict(locfit.i, newdata=predictors.tmp)
-              mse = mean((residual - predicted.i)^2)
-              if (verbose) cat(predictor.i, ":", predictor.j, ":", predictor.k, ":", predictor.l, ":", rmse, "\n")
-              if (mse < mse.min) {
-                mse.min=mse; predicted.step = predicted.i
-                predictor.list[[step]]=predictor.ijkl; locfit.list[[step]]=locfit.i } } } } }
-
-    } else {
-      # Run locfit on quints of predictors (first thru fifth level interactions)
-      for (predictor.i in seq(1, n.predictors-4)) {
-        for (predictor.j in seq(predictor.i+1, n.predictors-3)) {
-          for (predictor.k in seq(predictor.j+1, n.predictors-2)) {
-            for (predictor.l in seq(predictor.k+1, n.predictors-1)) {
-              for (predictor.m in seq(predictor.l+1, n.predictors)) {
-                predictor.ijklm = c(predictor.i, predictor.j, predictor.k, predictor.l, predictor.m)
-                predictors.tmp = predictors[, predictor.ijklm]
-                locfit.i = locfit.raw(predictors.tmp, residual, alpha=locfit.alpha, deg=locfit.degree, maxk=maxk)
-                predicted.i = predict(locfit.i, newdata=predictors.tmp)
-                mse = mean((residual - predicted.i)^2)
-                if (verbose) cat(predictor.i, ":", predictor.j, ":", predictor.k, ":", predictor.l, ":", predictor.m, ":", rmse, "\n")
-                if (mse < mse.min) {
-                  mse.min=mse; predicted.step = predicted.i
-                  predictor.list[[step]]=predictor.ijklm; locfit.list[[step]]=locfit.i } } } } } }
-    }
-
-    # Update residual
-    if (verbose) cat(step, " mse.min =", mse.min, predictor.list[[step]], "\n\n")
-    residual = residual - learning.rate * predicted.step
- 
-    prediction.means[step]    = mean(predicted.step)
-    mean.squared.errors[step] = mean(residual^2)
-  }
-  list(locfit.list=locfit.list, predictor.list=predictor.list, learning.rate=learning.rate,
-      response.mean=response.mean, prediction.means=prediction.means, mean.squared.errors=mean.squared.errors)
-}
-
-
-# Function Name:         plot.gbm.locfit
-# Version:               V1.0
-# Date:                  2015-02-28
-#
-# Function Description:  This function provides a plot routine for gbm.locfit.
-
-plot.gbm.locfit <- function(object, predictors, n.steps=object$ns, i.var, n.eval=100, ...)
-{
-  require(locfit)
-  eval.points = seq(min(predictors[, i.var]), max(predictors[, i.var]), length.out = n.eval)
-  marginal.values = rep(0, n.eval)
-
-  # Loop over evaluation points
-  for (j.eval in seq(1, n.eval)) {
-    tmp.predictors = predictors
-    tmp.predictors[, i.var] = rep(eval.points[j.eval], dim(predictors)[1])
-
-    marginal.values[j.eval] = mean(predict.gbm.locfit(object, tmp.predictors, n.steps))
-  }
-  plot(eval.points, marginal.values, ...)
-}
-
-
-# Function Name:         predict.gbm.locfit
-# Version:               V1.0
-# Date:                  2015-02-26
-#
-# Function Description:  This function provides a predict routine for gbm.locfit.
-
-predict.gbm.locfit <- function(object, predictors, n.steps=object$ns)
-{
-  require(locfit)
-  predicted = rep(object$response.mean, length=length(predictors[, 1]) )
-
-  # Assemble predicted
-  for (step in seq(1, n.steps))
-    predicted = predicted + object$learning.rate *
-                  predict(object$locfit.list[[step]], newdata=predictors[, object$predictor.list[[step]] ])
-
-  predicted
-}
-
-
-# Function Name:         incremental.predict.gbm.locfit
-# Version:               V1.0
-# Date:                  2015-07-02
-#
-# Function Description:  This function provides a predict routine for gbm.locfit.
-
-incremental.predict.gbm.locfit <- function(object, predictors, previous.predicted, step)
-{
-  require(locfit)
-
-  incremental.predicted = previous.predicted + object$learning.rate *
-                            predict(object$locfit.list[[step]], newdata=predictors[, object$predictor.list[[step]] ])
-
-  incremental.predicted
-}
-
-
-# Function Name:         summary.gbm.locfit
-# Version:               V1.0
-# Date:                  2015-02-26
-#
-# Function Description:  This function provides a summary routine for gbm.locfit.
-
-summary.gbm.locfit <- function(object, predictors, n.steps=object$ns, plot=TRUE)
-{
-  # Variable checks and other preliminaries
-  n.observations = dim(predictors)[1]
-  n.predictors = dim(predictors)[2]
-  influence = vector("numeric", length=n.predictors)
-  predictor.list = unique(c(object$predictor.list, recursive=TRUE))
-
-  # Calculate predictor influence
-  for ( j.pred in seq(1, n.predictors) ) {
-    if (length(predictor.list[predictor.list == j.pred]) > 0) {  # predictor is used
-      predictor.j.sd = sd(predictors[, j.pred])
-      epsilon.j = predictor.j.sd / sqrt(n.observations)
-
-      predictors.hi = predictors
-      predictors.lo = predictors
-      predictors.hi[, j.pred] = predictors.hi[, j.pred] + rep(epsilon.j, n.observations)
-      predictors.lo[, j.pred] = predictors.lo[, j.pred] - rep(epsilon.j, n.observations)
-
-      prediction.hi = predict.gbm.locfit(object, predictors.hi, n.steps)
-      prediction.lo = predict.gbm.locfit(object, predictors.lo, n.steps)
-
-      influence[j.pred] = sqrt(sum((prediction.hi - prediction.lo)^2)) / 2
-    } else  # predictor is NOT used
-    influence[j.pred] = 0
-  }
-
-  # Rescale influences to sum to 100 and determine order
-  influence = influence / sum(influence) * 100
-  order = order(influence, decreasing=TRUE)
-
-  # Extract names
-  names.predictors = colnames(predictors)
-
-  # Report relative influence
-  cat("Predictor relative influence:\n")
-  for ( j.pred in seq(1, n.predictors) )
-    cat(j.pred, names.predictors[order[j.pred]], influence[order[j.pred]], "\n")
-
-  if (plot == TRUE) {
-    par(las=1, mar=c(5,6,2,2))  # horizontal label text, increase y-axis margin slightly
-    color = rgb(0, 1-influence[rev(order)]/max(influence), 1)
-    barplot(influence[rev(order)], xlab="Relative Influence", horiz=TRUE, col=color,
-        names.arg=names.predictors[rev(order)]) 
-  }
-  list(influence=influence, order=order)
-}
-
-weighted.sd <- function(x, w, na.rm=FALSE)
-{
-  if (na.rm) { w = w[i = !is.na(x)]; x = x[i] }
-  sum.w = sum(w)
-  sum.w2 = sum(w^2)
-  mean.w = sum(x * w) / sum(w)
-  sqrt((sum.w / (sum.w^2 - sum.w2)) * sum(w * (x - mean.w)^2, na.rm=na.rm))
-}
+# Gradient Boosting Machine-Locfit: A GBM framework using local regresssion via Locfit.
+# For information on Locfit see: http://ect.bell-labs.com/sl/project/locfit/index.html
+#
+# Copyright 2016, The Materials Project, LBNL
+# Distributed under the terms of the MIT License.
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy of
+# this software and associated documentation files (the "Software"), to deal in
+# the Software without restriction, including without limitation the rights to
+# use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
+# the Software, and to permit persons to whom the Software is furnished to do so,
+# subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
+# FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
+# COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
+# IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
+# CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+
+
+# Function Name:         gbm.locfit
+# Version:               V1.2
+# Date:                  2015-09-16
+#
+# Function Description:  This function provides a cross-validation wrapper for gbm.locfit.core
+
+gbm.locfit <- function(predictors, response, n.interactions=1, n.steps=5, learning.rate=0.15, locfit.alpha=0.7,
+                       locfit.degree=1, cv.folds=10, seed.folds=NULL)
+{
+  # Variable checks and other preliminaries
+  require(locfit)
+  n.observations = length(response)
+  if (is.null(n.observations) || n.observations < 2) { message("Error: response must be a vector!"); return(1) }
+  predictors.dim = dim(predictors)
+  if (is.null(predictors.dim)) { message("Error: predictors must be a 2-D matrix!"); return(1) }
+  if (predictors.dim[1] != n.observations) { message("Error: lengths of response and predictors must match!"); return(1) }
+  n.predictors = predictors.dim[2]
+  if (n.predictors < 2) { message("Error: minimum of two predictors is required!"); return(1) }
+  if (is.null(n.interactions) || round(n.interactions) != n.interactions || n.interactions < 1 || n.interactions > 5)
+    { message("Error: n.interactions must be an integer between 1 and 5!"); return(1) }
+  if (n.interactions > n.predictors)
+    { message("Error: n.interactions may not exceed number of predictors!"); return(1) }
+  if (is.null(n.steps) || round(n.steps) != n.steps || n.steps < 1)
+    { message("Error: n.steps must be at least two!"); return(1) }
+  if (is.null(learning.rate) || learning.rate <= 0.0 || learning.rate >= 1.0)
+    { message("Error: learning.rate must of positive but less than 1!"); return(1) }
+  if (is.null(locfit.degree) || round(locfit.degree) != locfit.degree || locfit.degree < 1)
+    { message("Error: locfit.degree must be a positive integer!"); return(1) }
+  if (is.null(cv.folds) || round(cv.folds) != cv.folds || cv.folds <= 1)
+    { message("Error: cv.folds must be a positive integer, greater than one."); return(1) }
+
+  # Define CV sets
+  set.seed(seed.folds)
+  rounds = ceiling(n.observations / cv.folds)
+  sets = rep(seq(1, cv.folds), rounds)[seq(1, n.observations)]
+  sets = sample(sets, n.observations, replace=FALSE)  # random permutation
+  train.weights = rep(0, cv.folds);  train.mse.matrix = matrix(0, nrow=n.steps, ncol=cv.folds)
+  test.weights  = rep(0, cv.folds);  test.mse.matrix  = matrix(0, nrow=n.steps, ncol=cv.folds)
+
+  # Run CV models, dropping the test set from each run
+  for ( fold in seq(1, cv.folds) ) {
+    message("fold:",fold)
+    train.predictors = predictors[sets != fold, ];  test.predictors = predictors[sets == fold, ]
+    train.response = response[sets != fold];        test.response = response[sets == fold]
+    train.weights[fold] = length(train.response);   test.weights[fold] = length(test.response)
+
+    object = gbm.locfit.core(train.predictors, train.response, n.interactions=n.interactions, n.steps=n.steps,
+              learning.rate=learning.rate, locfit.alpha=locfit.alpha, locfit.degree=locfit.degree)
+
+    # Fill train.mse.matrix
+    train.mse.matrix[ , fold] = object$mean.squared.errors
+
+    # Fill test.mse.matrix
+    test.predicted.step = rep(object$response.mean, length=length(test.predictors[, 1]) )
+    for ( step in seq(1, n.steps) ) {
+      cat("\r",step)
+      # compute prediction error for each step, incrementally (for this fold)
+      test.predicted.step = incremental.predict.gbm.locfit(object, test.predictors, test.predicted.step, step)
+      test.mse.matrix[step, fold] = sum((test.response - test.predicted.step)^2) / length(test.response)
+  } }
+
+  # Normalize the train and test weights
+  train.weights = train.weights / sum(train.weights)
+  test.weights  = test.weights  / sum(test.weights)
+
+  # Calculate observed.errs, prediction.errs, and prediction.stderrs
+  observed.errs   = apply(train.mse.matrix, 1, weighted.mean, w=train.weights)
+  prediction.errs = apply(test.mse.matrix,  1, weighted.mean, w=test.weights)
+  prediction.stderrs = apply(test.mse.matrix, 1, weighted.sd, w=test.weights) / sqrt(cv.folds-1)
+  ns0 = which(prediction.errs == min(prediction.errs))
+  ns = min(which(prediction.errs < prediction.errs[ns0]+prediction.stderrs[ns0]))
+
+  # Run gbm.locfit.core again with all of the data, but only to ns0 steps
+  object = gbm.locfit.core(predictors, response, n.interactions=n.interactions, n.steps=ns0,
+            learning.rate=learning.rate, locfit.alpha=locfit.alpha, locfit.degree=locfit.degree)
+
+  list(locfit.list=object$locfit.list, predictor.list=object$predictor.list, learning.rate=learning.rate,
+      response.mean=object$response.mean, prediction.means=object$prediction.means,
+      locfit.alpha=locfit.alpha, locfit.degree=locfit.degree, cv.folds=cv.folds, observed.errs=observed.errs,
+      prediction.errs=prediction.errs, prediction.stderrs=prediction.stderrs, n.steps=n.steps, ns0=ns0, ns=ns)
+}
+
+
+# Function Name:         gbm.locfit.core
+# Version:               V1.1
+# Date:                  2015-07-02
+#
+# Function Description:  This function provides a gbm framework for locfit.
+
+gbm.locfit.core <- function(predictors, response, n.interactions=1, n.steps=5, learning.rate=0.15, locfit.alpha=0.7,
+                            locfit.degree=1, verbose=FALSE)
+{
+  # Variable checks and other preliminaries
+  require(locfit)
+  maxk=250
+  n.predictors = dim(predictors)[2]
+  response.mean = mean(response)
+  residual = response - response.mean  # Center response
+  locfit.list = vector(mode="list", length=n.steps)
+  predictor.list = vector(mode="list", length=n.steps)
+  prediction.means = rep(0, length=n.steps)
+  mean.squared.errors = rep(0, length=n.steps)
+
+  for (step in seq(1, n.steps)) {
+    mse.min = mean(residual^2)/learning.rate  # Set mse.min "high"
+    cat("\r",step)
+    if (n.interactions == 1) {
+      # Run locfit on individual predictors (first level interactions only)
+      for (predictor.i in seq(1, n.predictors)) {
+        predictors.tmp = predictors[, predictor.i]
+        locfit.i = locfit.raw(predictors.tmp, residual, alpha=locfit.alpha, deg=locfit.degree, maxk=maxk)
+        predicted.i = predict(locfit.i, newdata=predictors.tmp)
+        mse = mean((residual - predicted.i)^2)
+        if (verbose) cat(predictor.i, ": - :", mse, "\n")
+        if (mse < mse.min) {
+          mse.min=mse; predicted.step = predicted.i
+          predictor.list[[step]]=predictor.i; locfit.list[[step]]=locfit.i } }
+
+    } else if (n.interactions == 2) {
+      # Run locfit on pairs of predictors (first thru second level interactions)
+      for (predictor.i in seq(1, n.predictors-1)) {
+        for (predictor.j in seq(predictor.i+1, n.predictors)) {
+          predictor.ij = c(predictor.i, predictor.j)
+          predictors.tmp = predictors[, predictor.ij]
+          locfit.i = locfit.raw(predictors.tmp, residual, alpha=locfit.alpha, deg=locfit.degree, maxk=maxk)
+          predicted.i = predict(locfit.i, newdata=predictors.tmp)
+          mse = mean((residual - predicted.i)^2)
+          if (verbose) cat(predictor.i, ":", predictor.j, ":", mse, "\n")
+          if (mse < mse.min) {
+            mse.min=mse; predicted.step = predicted.i
+            predictor.list[[step]]=predictor.ij; locfit.list[[step]]=locfit.i } } }
+
+    } else if (n.interactions == 3) {
+      # Run locfit on triples of predictors (first thru third level interactions)
+      for (predictor.i in seq(1, n.predictors-2)) {
+        for (predictor.j in seq(predictor.i+1, n.predictors-1)) {
+          for (predictor.k in seq(predictor.j+1, n.predictors)) {
+            predictor.ijk = c(predictor.i, predictor.j, predictor.k)
+            predictors.tmp = predictors[, predictor.ijk]
+            locfit.i = locfit.raw(predictors.tmp, residual, alpha=locfit.alpha, deg=locfit.degree, maxk=maxk)
+            predicted.i = predict(locfit.i, newdata=predictors.tmp)
+            mse = mean((residual - predicted.i)^2)
+            if (verbose) cat(predictor.i, ":", predictor.j, ":", predictor.k, ":", mse, "\n")
+            if (mse < mse.min) {
+              mse.min=mse; predicted.step = predicted.i
+              predictor.list[[step]]=predictor.ijk; locfit.list[[step]]=locfit.i } } } }
+
+    } else if (n.interactions == 4) {
+      # Run locfit on quads of predictors (first thru fourth level interactions)
+      for (predictor.i in seq(1, n.predictors-3)) {
+        for (predictor.j in seq(predictor.i+1, n.predictors-2)) {
+          for (predictor.k in seq(predictor.j+1, n.predictors-1)) {
+            for (predictor.l in seq(predictor.k+1, n.predictors)) {
+              predictor.ijkl = c(predictor.i, predictor.j, predictor.k, predictor.l)
+              predictors.tmp = predictors[, predictor.ijkl]
+              locfit.i = locfit.raw(predictors.tmp, residual, alpha=locfit.alpha, deg=locfit.degree, maxk=maxk)
+              predicted.i = predict(locfit.i, newdata=predictors.tmp)
+              mse = mean((residual - predicted.i)^2)
+              if (verbose) cat(predictor.i, ":", predictor.j, ":", predictor.k, ":", predictor.l, ":", rmse, "\n")
+              if (mse < mse.min) {
+                mse.min=mse; predicted.step = predicted.i
+                predictor.list[[step]]=predictor.ijkl; locfit.list[[step]]=locfit.i } } } } }
+
+    } else {
+      # Run locfit on quints of predictors (first thru fifth level interactions)
+      for (predictor.i in seq(1, n.predictors-4)) {
+        for (predictor.j in seq(predictor.i+1, n.predictors-3)) {
+          for (predictor.k in seq(predictor.j+1, n.predictors-2)) {
+            for (predictor.l in seq(predictor.k+1, n.predictors-1)) {
+              for (predictor.m in seq(predictor.l+1, n.predictors)) {
+                predictor.ijklm = c(predictor.i, predictor.j, predictor.k, predictor.l, predictor.m)
+                predictors.tmp = predictors[, predictor.ijklm]
+                locfit.i = locfit.raw(predictors.tmp, residual, alpha=locfit.alpha, deg=locfit.degree, maxk=maxk)
+                predicted.i = predict(locfit.i, newdata=predictors.tmp)
+                mse = mean((residual - predicted.i)^2)
+                if (verbose) cat(predictor.i, ":", predictor.j, ":", predictor.k, ":", predictor.l, ":", predictor.m, ":", rmse, "\n")
+                if (mse < mse.min) {
+                  mse.min=mse; predicted.step = predicted.i
+                  predictor.list[[step]]=predictor.ijklm; locfit.list[[step]]=locfit.i } } } } } }
+    }
+
+    # Update residual
+    if (verbose) cat(step, " mse.min =", mse.min, predictor.list[[step]], "\n\n")
+    residual = residual - learning.rate * predicted.step
+ 
+    prediction.means[step]    = mean(predicted.step)
+    mean.squared.errors[step] = mean(residual^2)
+  }
+  list(locfit.list=locfit.list, predictor.list=predictor.list, learning.rate=learning.rate,
+      response.mean=response.mean, prediction.means=prediction.means, mean.squared.errors=mean.squared.errors)
+}
+
+
+# Function Name:         plot.gbm.locfit
+# Version:               V1.0
+# Date:                  2015-02-28
+#
+# Function Description:  This function provides a plot routine for gbm.locfit.
+
+plot.gbm.locfit <- function(object, predictors, n.steps=object$ns, i.var, n.eval=100, ...)
+{
+  require(locfit)
+  eval.points = seq(min(predictors[, i.var]), max(predictors[, i.var]), length.out = n.eval)
+  marginal.values = rep(0, n.eval)
+
+  # Loop over evaluation points
+  for (j.eval in seq(1, n.eval)) {
+    tmp.predictors = predictors
+    tmp.predictors[, i.var] = rep(eval.points[j.eval], dim(predictors)[1])
+
+    marginal.values[j.eval] = mean(predict.gbm.locfit(object, tmp.predictors, n.steps))
+  }
+  plot(eval.points, marginal.values, ...)
+}
+
+
+# Function Name:         predict.gbm.locfit
+# Version:               V1.0
+# Date:                  2015-02-26
+#
+# Function Description:  This function provides a predict routine for gbm.locfit.
+
+predict.gbm.locfit <- function(object, predictors, n.steps=object$ns)
+{
+  require(locfit)
+  predicted = rep(object$response.mean, length=length(predictors[, 1]) )
+
+  # Assemble predicted
+  for (step in seq(1, n.steps))
+    predicted = predicted + object$learning.rate *
+                  predict(object$locfit.list[[step]], newdata=predictors[, object$predictor.list[[step]] ])
+
+  predicted
+}
+
+
+# Function Name:         incremental.predict.gbm.locfit
+# Version:               V1.0
+# Date:                  2015-07-02
+#
+# Function Description:  This function provides a predict routine for gbm.locfit.
+
+incremental.predict.gbm.locfit <- function(object, predictors, previous.predicted, step)
+{
+  require(locfit)
+
+  incremental.predicted = previous.predicted + object$learning.rate *
+                            predict(object$locfit.list[[step]], newdata=predictors[, object$predictor.list[[step]] ])
+
+  incremental.predicted
+}
+
+
+# Function Name:         summary.gbm.locfit
+# Version:               V1.0
+# Date:                  2015-02-26
+#
+# Function Description:  This function provides a summary routine for gbm.locfit.
+
+summary.gbm.locfit <- function(object, predictors, n.steps=object$ns, plot=TRUE)
+{
+  # Variable checks and other preliminaries
+  n.observations = dim(predictors)[1]
+  n.predictors = dim(predictors)[2]
+  influence = vector("numeric", length=n.predictors)
+  predictor.list = unique(c(object$predictor.list, recursive=TRUE))
+
+  # Calculate predictor influence
+  for ( j.pred in seq(1, n.predictors) ) {
+    if (length(predictor.list[predictor.list == j.pred]) > 0) {  # predictor is used
+      predictor.j.sd = sd(predictors[, j.pred])
+      epsilon.j = predictor.j.sd / sqrt(n.observations)
+
+      predictors.hi = predictors
+      predictors.lo = predictors
+      predictors.hi[, j.pred] = predictors.hi[, j.pred] + rep(epsilon.j, n.observations)
+      predictors.lo[, j.pred] = predictors.lo[, j.pred] - rep(epsilon.j, n.observations)
+
+      prediction.hi = predict.gbm.locfit(object, predictors.hi, n.steps)
+      prediction.lo = predict.gbm.locfit(object, predictors.lo, n.steps)
+
+      influence[j.pred] = sqrt(sum((prediction.hi - prediction.lo)^2)) / 2
+    } else  # predictor is NOT used
+    influence[j.pred] = 0
+  }
+
+  # Rescale influences to sum to 100 and determine order
+  influence = influence / sum(influence) * 100
+  order = order(influence, decreasing=TRUE)
+
+  # Extract names
+  names.predictors = colnames(predictors)
+
+  # Report relative influence
+  cat("Predictor relative influence:\n")
+  for ( j.pred in seq(1, n.predictors) )
+    cat(j.pred, names.predictors[order[j.pred]], influence[order[j.pred]], "\n")
+
+  if (plot == TRUE) {
+    par(las=1, mar=c(5,6,2,2))  # horizontal label text, increase y-axis margin slightly
+    color = rgb(0, 1-influence[rev(order)]/max(influence), 1)
+    barplot(influence[rev(order)], xlab="Relative Influence", horiz=TRUE, col=color,
+        names.arg=names.predictors[rev(order)]) 
+  }
+  list(influence=influence, order=order)
+}
+
+weighted.sd <- function(x, w, na.rm=FALSE)
+{
+  if (na.rm) { w = w[i = !is.na(x)]; x = x[i] }
+  sum.w = sum(w)
+  sum.w2 = sum(w^2)
+  mean.w = sum(x * w) / sum(w)
+  sqrt((sum.w / (sum.w^2 - sum.w2)) * sum(w * (x - mean.w)^2, na.rm=na.rm))
+}
```

### Comparing `pqam_dparamhu2021-0.1.5/pqam_dparamhu2021/locfit_3_var_all.Rdata` & `pqam_dparamhu2021-0.1.6/pqam_dparamhu2021/locfit_3_var_all.Rdata`

 * *Files identical despite different names*

### Comparing `pqam_dparamhu2021-0.1.5/pqam_dparamhu2021/locfit_surf_2_var_all.Rdata` & `pqam_dparamhu2021-0.1.6/pqam_dparamhu2021/locfit_surf_2_var_all.Rdata`

 * *Files identical despite different names*

### Comparing `pqam_dparamhu2021-0.1.5/pqam_dparamhu2021/model.py` & `pqam_dparamhu2021-0.1.6/pqam_dparamhu2021/model.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from rpy2.robjects.packages import importr
 import rpy2.robjects as robjects
 from pymatgen.core import Composition
 from typing import Union, List
 from importlib import resources
+import sys
 
 base = importr('base')
 utils = importr('utils')
 locfit = importr('locfit')
 
 r = robjects.r
 path = str(resources.files('pqam_dparamhu2021'))
@@ -18,43 +19,62 @@
 # Load the prediction function
 heaPredFunc = robjects.globalenv['HEA_pred']
 
 # (Ti,Zr,Hf,V,Nb,Ta,Mo,W,Re,Ru)
 elementsSpace = ['Ti', 'Zr', 'Hf', 'V', 'Nb', 'Ta', 'Mo', 'W', 'Re', 'Ru']
 
 
-def predict(comp: Union[str, Composition]) -> list:
+def predict(
+        comp: Union[Composition, str],
+        outputType: str = "array") -> Union[dict, list]:
     """
-    Predicts the GSF, Surd, and resulting D parameter for a given HEA composition in the
+    Predicts the GSF, Surf, and resulting D parameter for a given HEA composition in the
     composition space of (Ti,Zr,Hf,V,Nb,Ta,Mo,W,Re,Ru) based on Hu's 2021 model (10.1016/j.actamat.2021.116800).
 
     Args:
         comp: A composition string which will be cast into pymatgen Composition object or ready Composition object.
-
+        outputType: A setting to select whether the model will output a minimalistic ordered array of values (default) 
+            or dictionary of labeled values. Currently implemented options are ['array', 'dict'] and the first one is 
+            default.
     Returns:
-        A float list representing the predicted GSF, Surd, and D parameter.
+        A float list representing the predicted GSF, Surf, and D parameter. Or a labeled dictionary of these output values.
     """
 
     assert isinstance(comp, (str, Composition)), \
         "comp must be a string or a pymatgen Composition object."
     if isinstance(comp, str):
         comp = Composition(comp)
 
     assert all([e.symbol in elementsSpace for e in comp.elements]), \
         "The composition must be in the composition space of (Ti,Zr,Hf,V,Nb,Ta,Mo,W,Re,Ru)."
 
     compList = [comp.get_atomic_fraction(e) for e in elementsSpace]
     result = heaPredFunc(robjects.FloatVector(compList), path)
-    return list(result)
+    result = list(result)
+    
+    assert len(result)==3
+
+    if outputType == "array":
+        return result
+    elif outputType == "dict":
+        return {"gfse": result[0],
+                "surf": result[1],
+                "dparam": result[2]}
+    else:
+        raise ValueError("Not recognized output type requested.")
 
 
 def cite() -> List[str]:
     """
     Returns the citation of the model.
 
     Returns:
         A list of strings representing the citation of the model.
     """
     return ["Yong-Jie Hu, Aditya Sundar, Shigenobu Ogata, Liang Qi, Screening of generalized stacking fault energies, "
             "surface energies and intrinsic ductile potency of refractory multicomponent alloys, Acta Materialia, "
             "Volume 210, 2021, 116800, https://doi.org/10.1016/j.actamat.2021.116800."
             ]
+
+if __name__ == "__main__":
+    assert len(sys.argv) == 2
+    print(predict(Composition(sys.argv[1]), outputType="array"))
```

### Comparing `pqam_dparamhu2021-0.1.5/pqam_dparamhu2021.egg-info/PKG-INFO` & `pqam_dparamhu2021-0.1.6/pqam_dparamhu2021.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pqam-dparamhu2021
-Version: 0.1.5
-Summary: PyQAlloy-compatible Model for D Parameter prediction based on Hu2021
+Version: 0.1.6
+Summary: PyQAlloy-compatible Model for D Parameter prediction based on Hu 2021 (10.1016/j.actamat.2021.116800)
 Author-email: Adam Krajewski <ak@psu.edu>
 Project-URL: Homepage, https://github.com/amkrajewski/pqam-dparamhu2021
 Project-URL: Bug Tracker, https://github.com/amkrajewski/pqam-dparamhu2021/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -15,17 +15,31 @@
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # PyQAlloy-compatible Model for D Parameter prediction based on Hu2021
 
-This repository contains a PyQAlloy-compatible compositionalModel for D Parameter Prediction Based on Yong-Jie Hu 2021 (10.1016/j.actamat.2021.116800) that 
-accepts a chemical formula of an alloy or a pymatgen Composition object and returns the predicted Genralized Stacking Fault Energy (GSF), Surface Energy (Surf), and the 
-calculated D Parameter.
+Release: ![PyPI](https://img.shields.io/pypi/v/pqam-dparamhu2021)
+
+Tests: [![small runtime test](https://github.com/amkrajewski/pqam-dparamhu2021/actions/workflows/runtimeTest.yml/badge.svg)](https://github.com/amkrajewski/pqam-dparamhu2021/actions/workflows/runtimeTest.yml)
+
+License: [![License: LGPL v3](https://img.shields.io/badge/License-LGPL_v3-blue.svg)](https://www.gnu.org/licenses/lgpl-3.0)
+
+This repository contains a PyQAlloy-compatible compositionalModel, compatible with [ULTERA Database (ultera.org)](https://ultera.org) infrastructure, for D Parameter Prediction Based on [Yong-Jie Hu 2021 (10.1016/j.actamat.2021.116800)](https://doi.org/10.1016/j.actamat.2021.116800) that 
+accepts a chemical formula string of an alloy or a `pymatgen.Composition` object. It return:
+
+Output Order: [`gfse`, `surf`, `dparam`]
+
+Output Meaning (all based on [10.1016/j.actamat.2021.116800](https://doi.org/10.1016/j.actamat.2021.116800)):
+- `gfse` - Genralized Stacking Fault Energy (GSF) [J/m^2]
+- `surf` - Surface Energy (Surf) [J/m^2]
+- `dparam` - D Parameter [unitless] calculated as `surf/gfse`
+
+
 
 ## Install and use
 
 To run this model you will need **Python 3.9+** and **R 4.1.0+** installed on your system, ideally **before** you install
 this software. For Python, we recommend you use a virtual Conda environment, which chan be created with minimal effort 
 (see [Miniconda install instructions](https://docs.conda.io/en/latest/miniconda.html)). For R, it can be downloaded 
 pre-compiled from a _Comprehensive R Archive Network_ repository (e.g. [Case CRAN](https://cran.case.edu)) and should 
@@ -44,14 +58,18 @@
 ***
 
 In some cases, required `locfit` R package may not be installed automatically. If you get an error message about it,
 try to go to your R console, typically by typing `R` in your terminal, and install it manually with:
 
     install.packages("locfit")
 
+Or, if you are automating things and need a single-liner, on Mac OS and Linux, the following should work:
+
+    Rscript -e "install.packages('locfit', repos='http://cran.us.r-project.org')"
+
 ## Attribution
 
 This repository has been created by Adam M. Krajewski (https://orcid.org/0000-0002-2266-0099) and is licensed under the MIT License. 
 **Please cite this repository if you use it in your work.**
 
 The featurizer and predictive model (HEA_pred.R and dependencies) have been optimized across and re-styled by Adam M.
 Krajewski based on code originally developed by Young-Jie Hu (https://orcid.org/0000-0003-1500-4015) et al. for their
@@ -64,18 +82,18 @@
 The gbm-locfit package (Gradient Boosting Machine-Locfit: A GBM framework using local regresssion via Locfit) has been 
 developed by Materials Project in 2016 and is distributed under the terms of the MIT License. Details can be found in
 its code.
 
 
 ## Hu's README File
 
-Hello, thank you for your interest in our work!
-Here we provide a script written in R language to take an alloy composition of interest and correspondingly predict the GSF energy, surface energy, and the ductility parameter based on the SL models in our manuscript ( https://doi.org/10.1016/j.actamat.2021.116800)
-To run the script and make predictions, you need to:
-1)	Download the RStudio platform. (https://www.rstudio.com/) ## No worry, it is open access 😊
-2)	Put all the files you downloaded from Materials Commons (basically all our files) into one local folder
-3)	Open the “predict.R” file in RStudio, input the alloy composition there, execute every line there, and the prediction will jump out in the console window below. 
-
-Please contact qiliang@umich.edu or yh593@drexel.edu if you have any questions. 
-
-P.S.,
-“predict_screen_4nary_all.csv” is the original data for plotting Figure 7&8 in the manuscript. Other figures in the manuscript can be reproduced by the data listed in the tables in the manuscript.
+>Hello, thank you for your interest in our work!
+>Here we provide a script written in R language to take an alloy composition of interest and correspondingly predict the GSF energy, surface energy, and the >ductility parameter based on the SL models in our manuscript ( https://doi.org/10.1016/j.actamat.2021.116800)
+>To run the script and make predictions, you need to:
+>1)	Download the RStudio platform. (https://www.rstudio.com/) ## No worry, it is open access 😊
+>2)	Put all the files you downloaded from Materials Commons (basically all our files) into one local folder
+>3)	Open the “predict.R” file in RStudio, input the alloy composition there, execute every line there, and the prediction will jump out in the console window >below. 
+>
+>Please contact qiliang@umich.edu or yh593@drexel.edu if you have any questions. 
+>
+>P.S.,
+>“predict_screen_4nary_all.csv” is the original data for plotting Figure 7&8 in the manuscript. Other figures in the manuscript can be reproduced by the data >listed in the tables in the manuscript.
```

### Comparing `pqam_dparamhu2021-0.1.5/pyproject.toml` & `pqam_dparamhu2021-0.1.6/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [build-system]
 requires = ["setuptools>=61.0", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pqam_dparamhu2021"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   { name="Adam Krajewski", email="ak@psu.edu" },
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Topic :: Scientific/Engineering :: Chemistry",
     "Topic :: Scientific/Engineering :: Physics",
 ]
-description = "PyQAlloy-compatible Model for D Parameter prediction based on Hu2021"
+description = "PyQAlloy-compatible Model for D Parameter prediction based on Hu 2021 (10.1016/j.actamat.2021.116800)"
 readme = "README.md"
 
 requires-python = ">=3.9"
 dependencies = [
     "pymatgen>=2022.1.9",
     "rpy2>3.5.0",
 ]
```

