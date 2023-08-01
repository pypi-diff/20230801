# Comparing `tmp/mlops_shape_project-0.1.1.tar.gz` & `tmp/mlops_shape_project-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlops_shape_project-0.1.1.tar", max compression
+gzip compressed data, was "mlops_shape_project-0.1.2.tar", max compression
```

## Comparing `mlops_shape_project-0.1.1.tar` & `mlops_shape_project-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       23 2023-07-31 05:01:46.969290 mlops_shape_project-0.1.1/mlops_shape_project/__init__.py
--rw-r--r--   0        0        0     1375 2023-07-31 04:49:17.779008 mlops_shape_project-0.1.1/mlops_shape_project/app.py
--rw-r--r--   0        0        0     3218 2023-07-31 22:02:11.147467 mlops_shape_project-0.1.1/mlops_shape_project/data_loader.py
--rw-r--r--   0        0        0     3478 2023-07-31 03:32:55.063354 mlops_shape_project-0.1.1/mlops_shape_project/dataframe_checker.py
--rw-r--r--   0        0        0     2213 2023-07-31 05:56:11.704527 mlops_shape_project-0.1.1/mlops_shape_project/feature_engineering_predict.py
--rw-r--r--   0        0        0     4060 2023-07-31 03:56:56.781253 mlops_shape_project-0.1.1/mlops_shape_project/pipeline_utils.py
--rw-r--r--   0        0        0     1766 2023-08-01 03:29:06.567150 mlops_shape_project-0.1.1/pyproject.toml
--rw-r--r--   0        0        0    10691 2023-08-01 03:27:38.205636 mlops_shape_project-0.1.1/README.md
--rw-r--r--   0        0        0    11730 1970-01-01 00:00:00.000000 mlops_shape_project-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       23 2023-07-31 05:01:46.969290 mlops_shape_project-0.1.2/mlops_shape_project/__init__.py
+-rw-r--r--   0        0        0     1375 2023-07-31 04:49:17.779008 mlops_shape_project-0.1.2/mlops_shape_project/app.py
+-rw-r--r--   0        0        0     3218 2023-07-31 22:02:11.147467 mlops_shape_project-0.1.2/mlops_shape_project/data_loader.py
+-rw-r--r--   0        0        0     3478 2023-07-31 03:32:55.063354 mlops_shape_project-0.1.2/mlops_shape_project/dataframe_checker.py
+-rw-r--r--   0        0        0     2213 2023-07-31 05:56:11.704527 mlops_shape_project-0.1.2/mlops_shape_project/feature_engineering_predict.py
+-rw-r--r--   0        0        0     4060 2023-07-31 03:56:56.781253 mlops_shape_project-0.1.2/mlops_shape_project/pipeline_utils.py
+-rw-r--r--   0        0        0     1766 2023-08-01 03:36:08.277292 mlops_shape_project-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0    10974 2023-08-01 03:33:48.518911 mlops_shape_project-0.1.2/README.md
+-rw-r--r--   0        0        0    12010 1970-01-01 00:00:00.000000 mlops_shape_project-0.1.2/PKG-INFO
```

### Comparing `mlops_shape_project-0.1.1/mlops_shape_project/app.py` & `mlops_shape_project-0.1.2/mlops_shape_project/app.py`

 * *Files identical despite different names*

### Comparing `mlops_shape_project-0.1.1/mlops_shape_project/data_loader.py` & `mlops_shape_project-0.1.2/mlops_shape_project/data_loader.py`

 * *Files identical despite different names*

### Comparing `mlops_shape_project-0.1.1/mlops_shape_project/dataframe_checker.py` & `mlops_shape_project-0.1.2/mlops_shape_project/dataframe_checker.py`

 * *Files identical despite different names*

### Comparing `mlops_shape_project-0.1.1/mlops_shape_project/feature_engineering_predict.py` & `mlops_shape_project-0.1.2/mlops_shape_project/feature_engineering_predict.py`

 * *Files identical despite different names*

### Comparing `mlops_shape_project-0.1.1/mlops_shape_project/pipeline_utils.py` & `mlops_shape_project-0.1.2/mlops_shape_project/pipeline_utils.py`

 * *Files identical despite different names*

### Comparing `mlops_shape_project-0.1.1/pyproject.toml` & `mlops_shape_project-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mlops-shape-project"
-version = "0.1.1"
+version = "0.1.2"
 description = "This project was initiated as part of Shape's Hard Skill Test for the Machine Learning Engineer role. The core objective was to take an initial script named `job_test_challenge.py` and transform it into a more organized 📐, maintainable 🛠️, and production-ready codebase."
 license = "MIT"
 authors = ["Junior Torres <galas.apps@gmail.com>"]
 readme = "README.md"
 packages = [{include = "mlops_shape_project"}]
 classifiers = [
     "Programming Language :: Python :: 3.8",
```

### Comparing `mlops_shape_project-0.1.1/README.md` & `mlops_shape_project-0.1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # **<p align="center" style="color: #DA1B5D;"><strong>Welcome to Shape MLOps Project</strong></p>**
 
+[![Documentation Status](https://readthedocs.org/projects/notas-musicais/badge/?version=latest)](https://mlops-shape-project.readthedocs.io/en/latest/?badge=latest)
+[![PyPI version](https://badge.fury.io/py/mlops-shape-project.svg)](https://badge.fury.io/py/mlops-shape-project)
+
 ## 🌐 **Overview** 
 ***
 
 This project was initiated as part of Shape's Hard Skill Test for the Machine Learning Engineer role. The core objective was to take an initial script named `job_test_challenge.py` and transform it into a more organized 📐, maintainable 🛠️, and production-ready codebase, all the while preserving its primary functionality. The envisioned transformation entailed the integration of best practices, robust documentation 📄, and a modularized (preferentially object-oriented 📦) design to render the code apt for product release.
 
 ### Key Tasks 🔑:
```

### Comparing `mlops_shape_project-0.1.1/PKG-INFO` & `mlops_shape_project-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlops-shape-project
-Version: 0.1.1
+Version: 0.1.2
 Summary: This project was initiated as part of Shape's Hard Skill Test for the Machine Learning Engineer role. The core objective was to take an initial script named `job_test_challenge.py` and transform it into a more organized 📐, maintainable 🛠️, and production-ready codebase.
 License: MIT
 Author: Junior Torres
 Author-email: galas.apps@gmail.com
 Requires-Python: >=3.8.10,<4.0.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -20,14 +20,17 @@
 Requires-Dist: scikit-learn (==1.0.2)
 Project-URL: Code, https://github.com/JuniorTorresMTJ/mlops_shape_project
 Project-URL: Documentation, https://mlops-shape-project.readthedocs.io/en/latest/
 Description-Content-Type: text/markdown
 
 # **<p align="center" style="color: #DA1B5D;"><strong>Welcome to Shape MLOps Project</strong></p>**
 
+[![Documentation Status](https://readthedocs.org/projects/notas-musicais/badge/?version=latest)](https://mlops-shape-project.readthedocs.io/en/latest/?badge=latest)
+[![PyPI version](https://badge.fury.io/py/mlops-shape-project.svg)](https://badge.fury.io/py/mlops-shape-project)
+
 ## 🌐 **Overview** 
 ***
 
 This project was initiated as part of Shape's Hard Skill Test for the Machine Learning Engineer role. The core objective was to take an initial script named `job_test_challenge.py` and transform it into a more organized 📐, maintainable 🛠️, and production-ready codebase, all the while preserving its primary functionality. The envisioned transformation entailed the integration of best practices, robust documentation 📄, and a modularized (preferentially object-oriented 📦) design to render the code apt for product release.
 
 ### Key Tasks 🔑:
```

