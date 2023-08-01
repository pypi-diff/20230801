# Comparing `tmp/estyp-0.4.0.tar.gz` & `tmp/estyp-0.4.1.tar.gz`

## Comparing `estyp-0.4.0.tar` & `estyp-0.4.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 estyp-0.4.0/estyp/__init__.py
--rw-r--r--   0        0        0     6154 2020-02-02 00:00:00.000000 estyp-0.4.0/estyp/linear_model/__init__.py
--rw-r--r--   0        0        0     2903 2020-02-02 00:00:00.000000 estyp-0.4.0/estyp/linear_model/stepwise/__init__.py
--rw-r--r--   0        0        0     5159 2020-02-02 00:00:00.000000 estyp-0.4.0/estyp/linear_model/stepwise/__base/__init__.py
--rw-r--r--   0        0        0    19748 2020-02-02 00:00:00.000000 estyp-0.4.0/estyp/testing/__init__.py
--rw-r--r--   0        0        0    23090 2020-02-02 00:00:00.000000 estyp-0.4.0/estyp/testing/__base/__init__.py
--rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 estyp-0.4.0/.gitignore
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 estyp-0.4.0/LICENSE
--rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 estyp-0.4.0/README.md
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 estyp-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     5462 2020-02-02 00:00:00.000000 estyp-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 estyp-0.4.1/estyp/__init__.py
+-rw-r--r--   0        0        0     6157 2020-02-02 00:00:00.000000 estyp-0.4.1/estyp/linear_model/__init__.py
+-rw-r--r--   0        0        0     2903 2020-02-02 00:00:00.000000 estyp-0.4.1/estyp/linear_model/stepwise/__init__.py
+-rw-r--r--   0        0        0     5159 2020-02-02 00:00:00.000000 estyp-0.4.1/estyp/linear_model/stepwise/__base/__init__.py
+-rw-r--r--   0        0        0    19748 2020-02-02 00:00:00.000000 estyp-0.4.1/estyp/testing/__init__.py
+-rw-r--r--   0        0        0    23090 2020-02-02 00:00:00.000000 estyp-0.4.1/estyp/testing/__base/__init__.py
+-rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 estyp-0.4.1/.gitignore
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 estyp-0.4.1/LICENSE
+-rw-r--r--   0        0        0     3843 2020-02-02 00:00:00.000000 estyp-0.4.1/README.md
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 estyp-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     5730 2020-02-02 00:00:00.000000 estyp-0.4.1/PKG-INFO
```

### Comparing `estyp-0.4.0/estyp/linear_model/__init__.py` & `estyp-0.4.1/estyp/linear_model/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-import numpy as np
-from pandas import Series, DataFrame, concat
-from patsy import dmatrices, build_design_matrices
 from typing import Literal
+
+import numpy as np
+from pandas import DataFrame, Series, concat
+from patsy import build_design_matrices, dmatrices
 from scipy.stats import norm
-from sklearn._typing import Int
-from sklearn.linear_model import LinearRegression, LogisticRegression
+from sklearn.linear_model import LogisticRegression as LogisticRegression_
 
 
-class LogisticRegression(LogisticRegression):
+class LogisticRegression(LogisticRegression_):
     """
 # Logistic Regression
 
 This class implements a logistic regression model. It inherits from the `sklearn.linear_model.LogisticRegression` class, but adds additional methods for calculating confidence intervals, p-values, and model summaries.
 
 ## Parameters
 
@@ -51,29 +51,31 @@
 
 ## Examples
 
 ```python
 import numpy as np
 import pandas as pd
 
-data = DataFrame({
+np.random.seed(123)
+data = pd.DataFrame({
     "y": np.random.randint(2, size=100),
     "x1": np.random.uniform(-1, 1, size=100),
     "x2": np.random.uniform(-1, 1, size=100),
 })
 
 formula = "y ~ x1 + x2"
 
 spec = LogisticRegression.from_formula(formula, data)
 model = spec.fit()
 
 print(model.summary())
+```
     """
     
-    def __init__(self, penalty: Literal['l1', 'l2', 'elasticnet'] = "none", *, dual = False, tol = 0.0001, C = 1, fit_intercept = False, intercept_scaling = 1, class_weight = None, random_state = 2023, solver: Literal['lbfgs', 'liblinear', 'newton-cg', 'newton-cholesky', 'sag', 'saga'] = "lbfgs", max_iter = 100, multi_class: Literal['auto', 'ovr', 'multinomial'] = "auto", verbose = 0, warm_start: bool = False, n_jobs = -1, l1_ratio = 0.5):
+    def __init__(self, penalty: Literal['l1', 'l2', 'elasticnet'] = None, *, dual = False, tol = 0.0001, C = 1, fit_intercept = False, intercept_scaling = 1, class_weight = None, random_state = 2023, solver: Literal['lbfgs', 'liblinear', 'newton-cg', 'newton-cholesky', 'sag', 'saga'] = "lbfgs", max_iter = 100, multi_class: Literal['auto', 'ovr', 'multinomial'] = "auto", verbose = 0, warm_start: bool = False, n_jobs = -1, l1_ratio = None):
         super().__init__(penalty=penalty, dual=dual, tol=tol, C=C, fit_intercept=fit_intercept, intercept_scaling=intercept_scaling, class_weight=class_weight, random_state=random_state, solver=solver, max_iter=max_iter, multi_class=multi_class, verbose=verbose, warm_start=warm_start, n_jobs=n_jobs, l1_ratio=l1_ratio)
 
     @classmethod
     def from_formula(cls, formula, data):
         y, X = dmatrices(formula, data)
         cls.y = y.reshape(-1)
         cls.formula = formula
```

### Comparing `estyp-0.4.0/estyp/linear_model/stepwise/__init__.py` & `estyp-0.4.1/estyp/linear_model/stepwise/__init__.py`

 * *Files identical despite different names*

### Comparing `estyp-0.4.0/estyp/linear_model/stepwise/__base/__init__.py` & `estyp-0.4.1/estyp/linear_model/stepwise/__base/__init__.py`

 * *Files identical despite different names*

### Comparing `estyp-0.4.0/estyp/testing/__init__.py` & `estyp-0.4.1/estyp/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `estyp-0.4.0/estyp/testing/__base/__init__.py` & `estyp-0.4.1/estyp/testing/__base/__init__.py`

 * *Files identical despite different names*

### Comparing `estyp-0.4.0/.gitignore` & `estyp-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `estyp-0.4.0/LICENSE` & `estyp-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `estyp-0.4.0/README.md` & `estyp-0.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 # ESTYP: Extended Statistical Toolkit Yet Practical
 
-[![PyPI version](https://badge.fury.io/py/estyp.svg)](https://badge.fury.io/py/estyp) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![Contributions](https://img.shields.io/badge/Contributions-welcome-blue.svg)](https://github.com/estebanrucan/estyp/issues) [![Chilean](https://img.shields.io/badge/Made_in-%F0%9F%87%A8%F0%9F%87%B1_Chile-blue.svg)](https://es.wikipedia.org/wiki/Chile)
+[![Downloads](https://static.pepy.tech/badge/estyp)](https://pepy.tech/project/estyp) [![PyPI version](https://badge.fury.io/py/estyp.svg)](https://badge.fury.io/py/estyp) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![Contributions](https://img.shields.io/badge/Contributions-welcome-blue.svg)](https://github.com/estebanrucan/estyp/issues) [![Chilean](https://img.shields.io/badge/Made_in-%F0%9F%87%A8%F0%9F%87%B1_Chile-blue.svg)](https://es.wikipedia.org/wiki/Chile)
 
 ## Description
 
 This library is a collection of statistical functions for Python.
 
 Actually, the name comes from the way my friends call me (Esti), plus "p" which is the initial of `python`.
 
 ## Changelog 
 
+### V0.4.1
+
+* Bug fixes in `linear_model.LogisticRegression()` class.
+* Added downloads badge to README.
+* Changed `sklearn>=1.2.1` to `scipy>=1.3.0` as a depedency of the library.
+
 ### V0.4.0
 
 * Added `testing.prop_test()` function to perform a test of proportions.
 * Added `testing.CheckModel()` class to perform linear regression assumptions checking.
 * Added badges to README.
 * Minor changes in README.
 
@@ -37,15 +43,15 @@
 
 * `linear_model.LogisticRegression()`: This class implements a logistic regression model. It inherits from the `LogisticRegression()` class from `scikit-learn`, but adds additional methods for calculating confidence intervals, p-values, and model summaries like `Logit` class in `statsmodels`.
 * `linear_model.stepwise.both_selection()`: This function performs both forward and backward variable selection using the Akaike Information Criterion (AIC). 
 * `linear_model.stepwise.forward_selection()`: This function performs forward variable selection based on p-values.
 * `testing.CheckModel()`: This class provides methods to test the assumptions of the linear regression model., inspired by the `performance::check_model()` function of the R software.
 * `testing.t_test()`: Performs one and two sample t-tests on groups of data. This function is inspired by the `t.test()` function of the R software.
 * `testing.var_test()`: Performs an F test to compare the variances of two samples from normal populations. This function is inspired by the `var.test()` function of the R software.
-* `testing.prop.test()`: it can be used for testing the null that the proportions (probabilities of success) in several groups are the same, or that they equal certain given values. This function is inspired by the `prop.test()` function of the R software.
+* `testing.prop_test()`: it can be used for testing the null that the proportions (probabilities of success) in several groups are the same, or that they equal certain given values. This function is inspired by the `prop.test()` function of the R software.
 * `testing.nested_models_test()`: Performs a nested models test to compare two nested models using deviance criterion.
 
 ## Installation
 
 To install this library, you can use PyPI:
 
 ```bash
```

### Comparing `estyp-0.4.0/pyproject.toml` & `estyp-0.4.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "estyp"
-version = "0.4.0"
+version = "0.4.1"
 authors = [
     { name="estebanrucan", email="errucan@gmail.com" },
 ]
 description = "Extended Statistical Toolkit Yet Practical"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.9.12"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
 dependencies = [
     "numpy >= 1.22.3",
-    "scikit-learn >= 1.2.1",
+    "scikit-learn >= 1.3.0",
     "matplotlib >= 3.4.3",
     "patsy >= 0.5.3",
     "statsmodels >= 0.13.5",
     "scipy >= 1.10.1"
 ]
 
 [project.urls]
```

### Comparing `estyp-0.4.0/PKG-INFO` & `estyp-0.4.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: estyp
-Version: 0.4.0
+Version: 0.4.1
 Summary: Extended Statistical Toolkit Yet Practical
 Project-URL: Homepage, https://github.com/estebanrucan/estyp
 Project-URL: Bug Tracker, https://github.com/estebanrucan/estyp/issues
 Author-email: estebanrucan <errucan@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Esteban Rucán Carrasco
@@ -30,31 +30,37 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9.12
 Requires-Dist: matplotlib>=3.4.3
 Requires-Dist: numpy>=1.22.3
 Requires-Dist: patsy>=0.5.3
-Requires-Dist: scikit-learn>=1.2.1
+Requires-Dist: scikit-learn>=1.3.0
 Requires-Dist: scipy>=1.10.1
 Requires-Dist: statsmodels>=0.13.5
 Description-Content-Type: text/markdown
 
 # ESTYP: Extended Statistical Toolkit Yet Practical
 
-[![PyPI version](https://badge.fury.io/py/estyp.svg)](https://badge.fury.io/py/estyp) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![Contributions](https://img.shields.io/badge/Contributions-welcome-blue.svg)](https://github.com/estebanrucan/estyp/issues) [![Chilean](https://img.shields.io/badge/Made_in-%F0%9F%87%A8%F0%9F%87%B1_Chile-blue.svg)](https://es.wikipedia.org/wiki/Chile)
+[![Downloads](https://static.pepy.tech/badge/estyp)](https://pepy.tech/project/estyp) [![PyPI version](https://badge.fury.io/py/estyp.svg)](https://badge.fury.io/py/estyp) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![Contributions](https://img.shields.io/badge/Contributions-welcome-blue.svg)](https://github.com/estebanrucan/estyp/issues) [![Chilean](https://img.shields.io/badge/Made_in-%F0%9F%87%A8%F0%9F%87%B1_Chile-blue.svg)](https://es.wikipedia.org/wiki/Chile)
 
 ## Description
 
 This library is a collection of statistical functions for Python.
 
 Actually, the name comes from the way my friends call me (Esti), plus "p" which is the initial of `python`.
 
 ## Changelog 
 
+### V0.4.1
+
+* Bug fixes in `linear_model.LogisticRegression()` class.
+* Added downloads badge to README.
+* Changed `sklearn>=1.2.1` to `scipy>=1.3.0` as a depedency of the library.
+
 ### V0.4.0
 
 * Added `testing.prop_test()` function to perform a test of proportions.
 * Added `testing.CheckModel()` class to perform linear regression assumptions checking.
 * Added badges to README.
 * Minor changes in README.
 
@@ -78,15 +84,15 @@
 
 * `linear_model.LogisticRegression()`: This class implements a logistic regression model. It inherits from the `LogisticRegression()` class from `scikit-learn`, but adds additional methods for calculating confidence intervals, p-values, and model summaries like `Logit` class in `statsmodels`.
 * `linear_model.stepwise.both_selection()`: This function performs both forward and backward variable selection using the Akaike Information Criterion (AIC). 
 * `linear_model.stepwise.forward_selection()`: This function performs forward variable selection based on p-values.
 * `testing.CheckModel()`: This class provides methods to test the assumptions of the linear regression model., inspired by the `performance::check_model()` function of the R software.
 * `testing.t_test()`: Performs one and two sample t-tests on groups of data. This function is inspired by the `t.test()` function of the R software.
 * `testing.var_test()`: Performs an F test to compare the variances of two samples from normal populations. This function is inspired by the `var.test()` function of the R software.
-* `testing.prop.test()`: it can be used for testing the null that the proportions (probabilities of success) in several groups are the same, or that they equal certain given values. This function is inspired by the `prop.test()` function of the R software.
+* `testing.prop_test()`: it can be used for testing the null that the proportions (probabilities of success) in several groups are the same, or that they equal certain given values. This function is inspired by the `prop.test()` function of the R software.
 * `testing.nested_models_test()`: Performs a nested models test to compare two nested models using deviance criterion.
 
 ## Installation
 
 To install this library, you can use PyPI:
 
 ```bash
```

