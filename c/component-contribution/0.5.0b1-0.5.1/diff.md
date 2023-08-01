# Comparing `tmp/component-contribution-0.5.0b1.tar.gz` & `tmp/component-contribution-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "component-contribution-0.5.0b1.tar", last modified: Sun Jul 30 10:48:04 2023, max compression
+gzip compressed data, was "component-contribution-0.5.1.tar", last modified: Tue Aug  1 15:41:10 2023, max compression
```

## Comparing `component-contribution-0.5.0b1.tar` & `component-contribution-0.5.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 10:48:04.071328 component-contribution-0.5.0b1/
--rw-rw-rw-   0 root         (0) root         (0)     1282 2023-07-30 10:47:52.000000 component-contribution-0.5.0b1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      103 2023-07-30 10:47:52.000000 component-contribution-0.5.0b1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3066 2023-07-30 10:48:04.071328 component-contribution-0.5.0b1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1707 2023-07-30 10:47:52.000000 component-contribution-0.5.0b1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      177 2023-07-30 10:47:52.000000 component-contribution-0.5.0b1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1983 2023-07-30 10:48:04.071328 component-contribution-0.5.0b1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      195 2023-07-30 10:47:52.000000 component-contribution-0.5.0b1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 10:48:04.066329 component-contribution-0.5.0b1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 10:48:04.071328 component-contribution-0.5.0b1/src/component_contribution/
--rw-rw-rw-   0 root         (0) root         (0)     3004 2023-07-30 10:47:52.000000 component-contribution-0.5.0b1/src/component_contribution/__init__.py
--rw-r--r--   0 root         (0) root         (0)      499 2023-07-30 10:48:04.071328 component-contribution-0.5.0b1/src/component_contribution/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 10:48:04.071328 component-contribution-0.5.0b1/src/component_contribution/data/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-30 10:47:52.000000 component-contribution-0.5.0b1/src/component_contribution/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3701 2023-07-30 10:47:52.000000 component-contribution-0.5.0b1/src/component_contribution/data/toy_training_data.csv
--rw-rw-rw-   0 root         (0) root         (0)     6476 2023-07-30 10:47:52.000000 component-contribution-0.5.0b1/src/component_contribution/linalg.py
--rw-rw-rw-   0 root         (0) root         (0)     4420 2023-07-30 10:47:52.000000 component-contribution-0.5.0b1/src/component_contribution/parameters.py
--rw-rw-rw-   0 root         (0) root         (0)    21974 2023-07-30 10:47:52.000000 component-contribution-0.5.0b1/src/component_contribution/predict.py
--rw-rw-rw-   0 root         (0) root         (0)    13507 2023-07-30 10:47:52.000000 component-contribution-0.5.0b1/src/component_contribution/preprocessor.py
--rw-rw-rw-   0 root         (0) root         (0)     8724 2023-07-30 10:47:52.000000 component-contribution-0.5.0b1/src/component_contribution/trainer.py
--rw-rw-rw-   0 root         (0) root         (0)    25505 2023-07-30 10:47:52.000000 component-contribution-0.5.0b1/src/component_contribution/training_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 10:48:04.070329 component-contribution-0.5.0b1/src/component_contribution.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3066 2023-07-30 10:48:04.000000 component-contribution-0.5.0b1/src/component_contribution.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      788 2023-07-30 10:48:04.000000 component-contribution-0.5.0b1/src/component_contribution.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-30 10:48:04.000000 component-contribution-0.5.0b1/src/component_contribution.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      309 2023-07-30 10:48:04.000000 component-contribution-0.5.0b1/src/component_contribution.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-07-30 10:48:04.000000 component-contribution-0.5.0b1/src/component_contribution.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-30 10:48:04.000000 component-contribution-0.5.0b1/src/component_contribution.egg-info/zip-safe
--rw-rw-rw-   0 root         (0) root         (0)    68611 2023-07-30 10:47:52.000000 component-contribution-0.5.0b1/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 15:41:10.008078 component-contribution-0.5.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1282 2023-08-01 15:40:58.000000 component-contribution-0.5.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      103 2023-08-01 15:40:58.000000 component-contribution-0.5.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3064 2023-08-01 15:41:10.009078 component-contribution-0.5.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1707 2023-08-01 15:40:58.000000 component-contribution-0.5.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      177 2023-08-01 15:40:58.000000 component-contribution-0.5.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1954 2023-08-01 15:41:10.009078 component-contribution-0.5.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      195 2023-08-01 15:40:58.000000 component-contribution-0.5.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 15:41:10.003078 component-contribution-0.5.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 15:41:10.009078 component-contribution-0.5.1/src/component_contribution/
+-rw-rw-rw-   0 root         (0) root         (0)     3004 2023-08-01 15:40:58.000000 component-contribution-0.5.1/src/component_contribution/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-08-01 15:41:10.009078 component-contribution-0.5.1/src/component_contribution/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 15:41:10.008078 component-contribution-0.5.1/src/component_contribution/data/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 15:40:58.000000 component-contribution-0.5.1/src/component_contribution/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3701 2023-08-01 15:40:58.000000 component-contribution-0.5.1/src/component_contribution/data/toy_training_data.csv
+-rw-rw-rw-   0 root         (0) root         (0)     6476 2023-08-01 15:40:58.000000 component-contribution-0.5.1/src/component_contribution/linalg.py
+-rw-rw-rw-   0 root         (0) root         (0)     4420 2023-08-01 15:40:58.000000 component-contribution-0.5.1/src/component_contribution/parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)    21974 2023-08-01 15:40:58.000000 component-contribution-0.5.1/src/component_contribution/predict.py
+-rw-rw-rw-   0 root         (0) root         (0)    13507 2023-08-01 15:40:58.000000 component-contribution-0.5.1/src/component_contribution/preprocessor.py
+-rw-rw-rw-   0 root         (0) root         (0)     8724 2023-08-01 15:40:58.000000 component-contribution-0.5.1/src/component_contribution/trainer.py
+-rw-rw-rw-   0 root         (0) root         (0)    25505 2023-08-01 15:40:58.000000 component-contribution-0.5.1/src/component_contribution/training_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 15:41:10.008078 component-contribution-0.5.1/src/component_contribution.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3064 2023-08-01 15:41:09.000000 component-contribution-0.5.1/src/component_contribution.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      788 2023-08-01 15:41:09.000000 component-contribution-0.5.1/src/component_contribution.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 15:41:09.000000 component-contribution-0.5.1/src/component_contribution.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      279 2023-08-01 15:41:09.000000 component-contribution-0.5.1/src/component_contribution.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-08-01 15:41:09.000000 component-contribution-0.5.1/src/component_contribution.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 15:41:09.000000 component-contribution-0.5.1/src/component_contribution.egg-info/zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)    68611 2023-08-01 15:40:58.000000 component-contribution-0.5.1/versioneer.py
```

### Comparing `component-contribution-0.5.0b1/LICENSE` & `component-contribution-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `component-contribution-0.5.0b1/PKG-INFO` & `component-contribution-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: component-contribution
-Version: 0.5.0b1
+Version: 0.5.1
 Summary: Standard reaction Gibbs energy estimation for biochemical reactions.
 Home-page: https://gitlab.com/equilibrator/component-contribution
 Download-URL: https://pypi.org/project/component-contribution/
 Author: Elad Noor, Moritz E. Beber
 Author-email: eladn@weizmann.ac.il, midnighter@posteo.net
 License: MIT
 Project-URL: Source Code, https://gitlab.com/equilibrator/component-contribution
```

### Comparing `component-contribution-0.5.0b1/README.md` & `component-contribution-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `component-contribution-0.5.0b1/setup.cfg` & `component-contribution-0.5.1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -29,17 +29,17 @@
 	biochemical reaction
 	eQuilibrator
 	cache
 
 [options]
 zip_safe = True
 install_requires = 
-	equilibrator-cache~=0.5.0b2
+	equilibrator-cache~=0.5.1
+	scipy >=1.11
 	path~=16.7
-	periodictable~=1.6
 	uncertainties~=3.1
 python_requires = >=3.9
 tests_require = 
 	tox
 packages = find:
 package_dir = 
 	= src
@@ -48,18 +48,18 @@
 where = src
 
 [options.package_data]
 component_contribution.data = *.csv
 
 [options.extras_require]
 test = 
-	pytest~=7.0
-	pytest-cov~=3.0
-	pytest-raises~=0.11
-	pytest-mock~=3.7
+	pytest
+	pytest-cov
+	pytest-raises
+	pytest-mock
 development = 
 	black~=23.7
 	isort~=5.12
 	flake8~=6.1
 	safety~=2.3
 	tox==3.28
 	twine~=4.0
```

### Comparing `component-contribution-0.5.0b1/src/component_contribution/__init__.py` & `component-contribution-0.5.1/src/component_contribution/__init__.py`

 * *Files identical despite different names*

### Comparing `component-contribution-0.5.0b1/src/component_contribution/data/toy_training_data.csv` & `component-contribution-0.5.1/src/component_contribution/data/toy_training_data.csv`

 * *Files identical despite different names*

### Comparing `component-contribution-0.5.0b1/src/component_contribution/linalg.py` & `component-contribution-0.5.1/src/component_contribution/linalg.py`

 * *Files identical despite different names*

### Comparing `component-contribution-0.5.0b1/src/component_contribution/parameters.py` & `component-contribution-0.5.1/src/component_contribution/parameters.py`

 * *Files identical despite different names*

### Comparing `component-contribution-0.5.0b1/src/component_contribution/predict.py` & `component-contribution-0.5.1/src/component_contribution/predict.py`

 * *Files identical despite different names*

### Comparing `component-contribution-0.5.0b1/src/component_contribution/preprocessor.py` & `component-contribution-0.5.1/src/component_contribution/preprocessor.py`

 * *Files identical despite different names*

### Comparing `component-contribution-0.5.0b1/src/component_contribution/trainer.py` & `component-contribution-0.5.1/src/component_contribution/trainer.py`

 * *Files identical despite different names*

### Comparing `component-contribution-0.5.0b1/src/component_contribution/training_data.py` & `component-contribution-0.5.1/src/component_contribution/training_data.py`

 * *Files identical despite different names*

### Comparing `component-contribution-0.5.0b1/src/component_contribution.egg-info/PKG-INFO` & `component-contribution-0.5.1/src/component_contribution.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: component-contribution
-Version: 0.5.0b1
+Version: 0.5.1
 Summary: Standard reaction Gibbs energy estimation for biochemical reactions.
 Home-page: https://gitlab.com/equilibrator/component-contribution
 Download-URL: https://pypi.org/project/component-contribution/
 Author: Elad Noor, Moritz E. Beber
 Author-email: eladn@weizmann.ac.il, midnighter@posteo.net
 License: MIT
 Project-URL: Source Code, https://gitlab.com/equilibrator/component-contribution
```

### Comparing `component-contribution-0.5.0b1/src/component_contribution.egg-info/SOURCES.txt` & `component-contribution-0.5.1/src/component_contribution.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `component-contribution-0.5.0b1/versioneer.py` & `component-contribution-0.5.1/versioneer.py`

 * *Files identical despite different names*

