# Comparing `tmp/GPopt-0.2.3.tar.gz` & `tmp/GPopt-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/GPopt-0.2.3.tar", last modified: Sun Jan 23 16:14:25 2022, max compression
+gzip compressed data, was "dist/GPopt-0.2.4.tar", last modified: Tue Aug  1 13:41:13 2023, max compression
```

## Comparing `GPopt-0.2.3.tar` & `GPopt-0.2.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 t          (501) staff       (20)        0 2022-01-23 16:14:25.170869 GPopt-0.2.3/
-drwxr-xr-x   0 t          (501) staff       (20)        0 2022-01-23 16:14:25.154358 GPopt-0.2.3/GPopt/
-drwxr-xr-x   0 t          (501) staff       (20)        0 2022-01-23 16:14:25.161829 GPopt-0.2.3/GPopt/GPOpt/
--rw-r--r--   0 t          (501) staff       (20)    21236 2022-01-23 16:12:29.000000 GPopt-0.2.3/GPopt/GPOpt/GPOpt.py
--rw-r--r--   0 t          (501) staff       (20)       46 2021-05-13 16:52:43.000000 GPopt-0.2.3/GPopt/GPOpt/__init__.py
--rw-r--r--   0 t          (501) staff       (20)       52 2021-05-13 16:54:22.000000 GPopt-0.2.3/GPopt/__init__.py
-drwxr-xr-x   0 t          (501) staff       (20)        0 2022-01-23 16:14:25.166473 GPopt-0.2.3/GPopt/utils/
--rw-r--r--   0 t          (501) staff       (20)      120 2019-06-14 17:54:14.000000 GPopt-0.2.3/GPopt/utils/__init__.py
--rw-r--r--   0 t          (501) staff       (20)     2836 2022-01-23 16:12:29.000000 GPopt-0.2.3/GPopt/utils/nodesimulation.py
--rw-r--r--   0 t          (501) staff       (20)     6794 2022-01-23 16:12:29.000000 GPopt-0.2.3/GPopt/utils/progress_bar.py
--rw-r--r--   0 t          (501) staff       (20)   346940 2022-01-23 16:12:29.000000 GPopt-0.2.3/GPopt/utils/sobol_lib.py
-drwxr-xr-x   0 t          (501) staff       (20)        0 2022-01-23 16:14:25.158962 GPopt-0.2.3/GPopt.egg-info/
--rw-r--r--   0 t          (501) staff       (20)      533 2022-01-23 16:14:24.000000 GPopt-0.2.3/GPopt.egg-info/PKG-INFO
--rw-r--r--   0 t          (501) staff       (20)      371 2022-01-23 16:14:24.000000 GPopt-0.2.3/GPopt.egg-info/SOURCES.txt
--rw-r--r--   0 t          (501) staff       (20)        1 2022-01-23 16:14:24.000000 GPopt-0.2.3/GPopt.egg-info/dependency_links.txt
--rw-r--r--   0 t          (501) staff       (20)      764 2022-01-23 16:14:24.000000 GPopt-0.2.3/GPopt.egg-info/requires.txt
--rw-r--r--   0 t          (501) staff       (20)        6 2022-01-23 16:14:24.000000 GPopt-0.2.3/GPopt.egg-info/top_level.txt
--rw-r--r--   0 t          (501) staff       (20)       42 2019-06-11 00:45:02.000000 GPopt-0.2.3/MANIFEST.in
--rw-r--r--   0 t          (501) staff       (20)      533 2022-01-23 16:14:25.171082 GPopt-0.2.3/PKG-INFO
--rw-r--r--   0 t          (501) staff       (20)      954 2021-07-01 14:35:23.000000 GPopt-0.2.3/README.md
--rw-r--r--   0 t          (501) staff       (20)      764 2021-04-09 13:19:14.000000 GPopt-0.2.3/requirements.txt
--rw-r--r--   0 t          (501) staff       (20)      108 2022-01-23 16:14:25.172047 GPopt-0.2.3/setup.cfg
--rw-r--r--   0 t          (501) staff       (20)     1269 2022-01-23 16:12:29.000000 GPopt-0.2.3/setup.py
+drwxr-xr-x   0 t          (501) staff       (20)        0 2023-08-01 13:41:13.380276 GPopt-0.2.4/
+drwxr-xr-x   0 t          (501) staff       (20)        0 2023-08-01 13:41:13.092302 GPopt-0.2.4/GPopt/
+drwxr-xr-x   0 t          (501) staff       (20)        0 2023-08-01 13:41:13.283545 GPopt-0.2.4/GPopt/GPOpt/
+-rw-r--r--   0 t          (501) staff       (20)    21184 2023-08-01 13:38:24.000000 GPopt-0.2.4/GPopt/GPOpt/GPOpt.py
+-rw-r--r--   0 t          (501) staff       (20)       46 2021-05-13 16:52:43.000000 GPopt-0.2.4/GPopt/GPOpt/__init__.py
+-rw-r--r--   0 t          (501) staff       (20)       52 2021-05-13 16:54:22.000000 GPopt-0.2.4/GPopt/__init__.py
+drwxr-xr-x   0 t          (501) staff       (20)        0 2023-08-01 13:41:13.340558 GPopt-0.2.4/GPopt/utils/
+-rw-r--r--   0 t          (501) staff       (20)      120 2019-06-14 17:54:14.000000 GPopt-0.2.4/GPopt/utils/__init__.py
+-rw-r--r--   0 t          (501) staff       (20)     2836 2022-01-23 16:12:29.000000 GPopt-0.2.4/GPopt/utils/nodesimulation.py
+-rw-r--r--   0 t          (501) staff       (20)     6794 2022-01-23 16:12:29.000000 GPopt-0.2.4/GPopt/utils/progress_bar.py
+-rw-r--r--   0 t          (501) staff       (20)   346940 2022-01-23 16:12:29.000000 GPopt-0.2.4/GPopt/utils/sobol_lib.py
+drwxr-xr-x   0 t          (501) staff       (20)        0 2023-08-01 13:41:13.243219 GPopt-0.2.4/GPopt.egg-info/
+-rw-r--r--   0 t          (501) staff       (20)      533 2023-08-01 13:41:12.000000 GPopt-0.2.4/GPopt.egg-info/PKG-INFO
+-rw-r--r--   0 t          (501) staff       (20)      371 2023-08-01 13:41:13.000000 GPopt-0.2.4/GPopt.egg-info/SOURCES.txt
+-rw-r--r--   0 t          (501) staff       (20)        1 2023-08-01 13:41:12.000000 GPopt-0.2.4/GPopt.egg-info/dependency_links.txt
+-rw-r--r--   0 t          (501) staff       (20)       53 2023-08-01 13:41:12.000000 GPopt-0.2.4/GPopt.egg-info/requires.txt
+-rw-r--r--   0 t          (501) staff       (20)        6 2023-08-01 13:41:12.000000 GPopt-0.2.4/GPopt.egg-info/top_level.txt
+-rw-r--r--   0 t          (501) staff       (20)       42 2019-06-11 00:45:02.000000 GPopt-0.2.4/MANIFEST.in
+-rw-r--r--   0 t          (501) staff       (20)      533 2023-08-01 13:41:13.381078 GPopt-0.2.4/PKG-INFO
+-rw-r--r--   0 t          (501) staff       (20)      954 2021-07-01 14:35:23.000000 GPopt-0.2.4/README.md
+-rw-r--r--   0 t          (501) staff       (20)       52 2023-08-01 13:38:24.000000 GPopt-0.2.4/requirements.txt
+-rw-r--r--   0 t          (501) staff       (20)      108 2023-08-01 13:41:13.388652 GPopt-0.2.4/setup.cfg
+-rw-r--r--   0 t          (501) staff       (20)     1269 2023-08-01 13:38:24.000000 GPopt-0.2.4/setup.py
```

### Comparing `GPopt-0.2.3/GPopt/GPOpt/GPOpt.py` & `GPopt-0.2.4/GPopt/GPOpt/GPOpt.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,19 +8,17 @@
 import pickle
 import shelve
 from sklearn.gaussian_process import GaussianProcessRegressor
 from sklearn.ensemble import RandomForestRegressor
 from sklearn.gaussian_process.kernels import Matern
 import scipy.stats as st
 from joblib import Parallel, delayed
+from time import time
 from ..utils import generate_sobol2
 from ..utils import Progbar
-from datetime import datetime
-from tqdm import tqdm
-from time import time
 
 
 class GPOpt:
     """Class GPOpt.
 
     # Arguments:
```

### Comparing `GPopt-0.2.3/GPopt/utils/nodesimulation.py` & `GPopt-0.2.4/GPopt/utils/nodesimulation.py`

 * *Files identical despite different names*

### Comparing `GPopt-0.2.3/GPopt/utils/progress_bar.py` & `GPopt-0.2.4/GPopt/utils/progress_bar.py`

 * *Files identical despite different names*

### Comparing `GPopt-0.2.3/GPopt/utils/sobol_lib.py` & `GPopt-0.2.4/GPopt/utils/sobol_lib.py`

 * *Files identical despite different names*

### Comparing `GPopt-0.2.3/GPopt.egg-info/PKG-INFO` & `GPopt-0.2.4/GPopt.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 1.1
 Name: GPopt
-Version: 0.2.3
+Version: 0.2.4
 Summary: Bayesian Optimization using Gaussian Process Regression
 Home-page: https://github.com/thierrymoudiki/GPopt
 Author: Thierry Moudiki
 Author-email: thierry.moudiki@gmail.com
 License: BSD
-Download-URL: https://github.com/thierrymoudiki/GPopt/tarball/0.2.3
+Download-URL: https://github.com/thierrymoudiki/GPopt/tarball/0.2.4
 Description: Bayesian Optimization using Gaussian Process Regression
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `GPopt-0.2.3/PKG-INFO` & `GPopt-0.2.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 1.1
 Name: GPopt
-Version: 0.2.3
+Version: 0.2.4
 Summary: Bayesian Optimization using Gaussian Process Regression
 Home-page: https://github.com/thierrymoudiki/GPopt
 Author: Thierry Moudiki
 Author-email: thierry.moudiki@gmail.com
 License: BSD
-Download-URL: https://github.com/thierrymoudiki/GPopt/tarball/0.2.3
+Download-URL: https://github.com/thierrymoudiki/GPopt/tarball/0.2.4
 Description: Bayesian Optimization using Gaussian Process Regression
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `GPopt-0.2.3/README.md` & `GPopt-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `GPopt-0.2.3/setup.py` & `GPopt-0.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 from codecs import open
 from os import path
 
-__version__ = "0.2.3"
+__version__ = "0.2.4"
 
 here = path.abspath(path.dirname(__file__))
 
 # get the dependencies and installs
 with open(
     path.join(here, "requirements.txt"), encoding="utf-8"
 ) as f:
```

