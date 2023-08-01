# Comparing `tmp/PyBacmman-0.5.1.tar.gz` & `tmp/PyBacmman-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyBacmman-0.5.1.tar", last modified: Tue Nov 29 11:37:53 2022, max compression
+gzip compressed data, was "PyBacmman-0.5.2.tar", last modified: Tue Aug  1 12:12:49 2023, max compression
```

## Comparing `PyBacmman-0.5.1.tar` & `PyBacmman-0.5.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 jollion   (1000) jollion   (1000)        0 2022-11-29 11:37:53.286855 PyBacmman-0.5.1/
--rw-rw-r--   0 jollion   (1000) jollion   (1000)    32453 2022-05-17 16:14:07.000000 PyBacmman-0.5.1/LICENSE
--rw-rw-r--   0 jollion   (1000) jollion   (1000)     1192 2022-11-29 11:37:53.286855 PyBacmman-0.5.1/PKG-INFO
-drwxrwxr-x   0 jollion   (1000) jollion   (1000)        0 2022-11-29 11:37:53.286855 PyBacmman-0.5.1/PyBacmman.egg-info/
--rw-rw-r--   0 jollion   (1000) jollion   (1000)     1192 2022-11-29 11:37:53.000000 PyBacmman-0.5.1/PyBacmman.egg-info/PKG-INFO
--rw-rw-r--   0 jollion   (1000) jollion   (1000)      534 2022-11-29 11:37:53.000000 PyBacmman-0.5.1/PyBacmman.egg-info/SOURCES.txt
--rw-rw-r--   0 jollion   (1000) jollion   (1000)        1 2022-11-29 11:37:53.000000 PyBacmman-0.5.1/PyBacmman.egg-info/dependency_links.txt
--rw-rw-r--   0 jollion   (1000) jollion   (1000)       12 2022-11-29 11:37:53.000000 PyBacmman-0.5.1/PyBacmman.egg-info/requires.txt
--rw-rw-r--   0 jollion   (1000) jollion   (1000)       10 2022-11-29 11:37:53.000000 PyBacmman-0.5.1/PyBacmman.egg-info/top_level.txt
--rw-rw-r--   0 jollion   (1000) jollion   (1000)      438 2022-11-29 11:37:34.000000 PyBacmman-0.5.1/README.md
-drwxrwxr-x   0 jollion   (1000) jollion   (1000)        0 2022-11-29 11:37:53.286855 PyBacmman-0.5.1/pybacmman/
--rw-rw-r--   0 jollion   (1000) jollion   (1000)       19 2022-05-17 16:14:07.000000 PyBacmman-0.5.1/pybacmman/__init__.py
-drwxrwxr-x   0 jollion   (1000) jollion   (1000)        0 2022-11-29 11:37:53.286855 PyBacmman-0.5.1/pybacmman/dataset/
--rw-rw-r--   0 jollion   (1000) jollion   (1000)       60 2022-11-25 11:07:45.000000 PyBacmman-0.5.1/pybacmman/dataset/__init__.py
--rw-rw-r--   0 jollion   (1000) jollion   (1000)     8787 2022-11-29 11:06:24.000000 PyBacmman-0.5.1/pybacmman/dataset/dataset.py
-drwxrwxr-x   0 jollion   (1000) jollion   (1000)        0 2022-11-29 11:37:53.286855 PyBacmman-0.5.1/pybacmman/evaluation/
--rw-rw-r--   0 jollion   (1000) jollion   (1000)       90 2022-05-17 16:14:07.000000 PyBacmman-0.5.1/pybacmman/evaluation/__init__.py
--rw-rw-r--   0 jollion   (1000) jollion   (1000)     5053 2022-05-17 16:14:07.000000 PyBacmman-0.5.1/pybacmman/evaluation/run_tasks.py
-drwxrwxr-x   0 jollion   (1000) jollion   (1000)        0 2022-11-29 11:37:53.286855 PyBacmman-0.5.1/pybacmman/pandas/
--rw-rw-r--   0 jollion   (1000) jollion   (1000)      101 2022-05-17 16:14:07.000000 PyBacmman-0.5.1/pybacmman/pandas/__init__.py
--rw-rw-r--   0 jollion   (1000) jollion   (1000)     1779 2022-05-17 16:14:07.000000 PyBacmman-0.5.1/pybacmman/pandas/curve_utils.py
--rw-rw-r--   0 jollion   (1000) jollion   (1000)      610 2022-05-17 16:14:07.000000 PyBacmman-0.5.1/pybacmman/pandas/indices_utils.py
--rw-rw-r--   0 jollion   (1000) jollion   (1000)     5225 2022-05-17 16:14:07.000000 PyBacmman-0.5.1/pybacmman/pandas/pandas_utils.py
-drwxrwxr-x   0 jollion   (1000) jollion   (1000)        0 2022-11-29 11:37:53.286855 PyBacmman-0.5.1/pybacmman/selections/
--rw-rw-r--   0 jollion   (1000) jollion   (1000)       66 2022-05-17 16:14:07.000000 PyBacmman-0.5.1/pybacmman/selections/__init__.py
--rw-rw-r--   0 jollion   (1000) jollion   (1000)     3668 2022-11-29 10:49:42.000000 PyBacmman-0.5.1/pybacmman/selections/selections.py
--rw-rw-r--   0 jollion   (1000) jollion   (1000)       38 2022-11-29 11:37:53.286855 PyBacmman-0.5.1/setup.cfg
--rw-rw-r--   0 jollion   (1000) jollion   (1000)      996 2022-11-29 11:36:14.000000 PyBacmman-0.5.1/setup.py
+drwxrwxr-x   0 jollion   (1000) jollion   (1000)        0 2023-08-01 12:12:49.675849 PyBacmman-0.5.2/
+-rw-rw-r--   0 jollion   (1000) jollion   (1000)    32453 2022-05-17 16:14:07.000000 PyBacmman-0.5.2/LICENSE
+-rw-rw-r--   0 jollion   (1000) jollion   (1000)     1287 2023-08-01 12:12:49.675849 PyBacmman-0.5.2/PKG-INFO
+drwxrwxr-x   0 jollion   (1000) jollion   (1000)        0 2023-08-01 12:12:49.675849 PyBacmman-0.5.2/PyBacmman.egg-info/
+-rw-rw-r--   0 jollion   (1000) jollion   (1000)     1287 2023-08-01 12:12:49.000000 PyBacmman-0.5.2/PyBacmman.egg-info/PKG-INFO
+-rw-rw-r--   0 jollion   (1000) jollion   (1000)      534 2023-08-01 12:12:49.000000 PyBacmman-0.5.2/PyBacmman.egg-info/SOURCES.txt
+-rw-rw-r--   0 jollion   (1000) jollion   (1000)        1 2023-08-01 12:12:49.000000 PyBacmman-0.5.2/PyBacmman.egg-info/dependency_links.txt
+-rw-rw-r--   0 jollion   (1000) jollion   (1000)       12 2023-08-01 12:12:49.000000 PyBacmman-0.5.2/PyBacmman.egg-info/requires.txt
+-rw-rw-r--   0 jollion   (1000) jollion   (1000)       10 2023-08-01 12:12:49.000000 PyBacmman-0.5.2/PyBacmman.egg-info/top_level.txt
+-rw-rw-r--   0 jollion   (1000) jollion   (1000)      533 2023-05-24 09:07:53.000000 PyBacmman-0.5.2/README.md
+drwxrwxr-x   0 jollion   (1000) jollion   (1000)        0 2023-08-01 12:12:49.675849 PyBacmman-0.5.2/pybacmman/
+-rw-rw-r--   0 jollion   (1000) jollion   (1000)       19 2022-05-17 16:14:07.000000 PyBacmman-0.5.2/pybacmman/__init__.py
+drwxrwxr-x   0 jollion   (1000) jollion   (1000)        0 2023-08-01 12:12:49.675849 PyBacmman-0.5.2/pybacmman/dataset/
+-rw-rw-r--   0 jollion   (1000) jollion   (1000)       60 2022-11-25 11:07:45.000000 PyBacmman-0.5.2/pybacmman/dataset/__init__.py
+-rw-rw-r--   0 jollion   (1000) jollion   (1000)    12905 2023-08-01 08:17:19.000000 PyBacmman-0.5.2/pybacmman/dataset/dataset.py
+drwxrwxr-x   0 jollion   (1000) jollion   (1000)        0 2023-08-01 12:12:49.675849 PyBacmman-0.5.2/pybacmman/evaluation/
+-rw-rw-r--   0 jollion   (1000) jollion   (1000)       90 2022-05-17 16:14:07.000000 PyBacmman-0.5.2/pybacmman/evaluation/__init__.py
+-rw-rw-r--   0 jollion   (1000) jollion   (1000)     5053 2022-05-17 16:14:07.000000 PyBacmman-0.5.2/pybacmman/evaluation/run_tasks.py
+drwxrwxr-x   0 jollion   (1000) jollion   (1000)        0 2023-08-01 12:12:49.675849 PyBacmman-0.5.2/pybacmman/pandas/
+-rw-rw-r--   0 jollion   (1000) jollion   (1000)      101 2022-05-17 16:14:07.000000 PyBacmman-0.5.2/pybacmman/pandas/__init__.py
+-rw-rw-r--   0 jollion   (1000) jollion   (1000)     1779 2022-05-17 16:14:07.000000 PyBacmman-0.5.2/pybacmman/pandas/curve_utils.py
+-rw-rw-r--   0 jollion   (1000) jollion   (1000)      610 2022-05-17 16:14:07.000000 PyBacmman-0.5.2/pybacmman/pandas/indices_utils.py
+-rw-rw-r--   0 jollion   (1000) jollion   (1000)     5225 2022-05-17 16:14:07.000000 PyBacmman-0.5.2/pybacmman/pandas/pandas_utils.py
+drwxrwxr-x   0 jollion   (1000) jollion   (1000)        0 2023-08-01 12:12:49.675849 PyBacmman-0.5.2/pybacmman/selections/
+-rw-rw-r--   0 jollion   (1000) jollion   (1000)       66 2022-05-17 16:14:07.000000 PyBacmman-0.5.2/pybacmman/selections/__init__.py
+-rw-rw-r--   0 jollion   (1000) jollion   (1000)     3668 2022-11-29 10:49:42.000000 PyBacmman-0.5.2/pybacmman/selections/selections.py
+-rw-rw-r--   0 jollion   (1000) jollion   (1000)       38 2023-08-01 12:12:49.675849 PyBacmman-0.5.2/setup.cfg
+-rw-rw-r--   0 jollion   (1000) jollion   (1000)      996 2023-08-01 12:08:53.000000 PyBacmman-0.5.2/setup.py
```

### Comparing `PyBacmman-0.5.1/LICENSE` & `PyBacmman-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PyBacmman-0.5.1/PKG-INFO` & `PyBacmman-0.5.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PyBacmman
-Version: 0.5.1
+Version: 0.5.2
 Summary: Utilities for analysis of data generated from bacmman software
 Home-page: https://github.com/jeanollion/PyBacmman.git
 Author: Jean Ollion
 Author-email: jean.ollion@polytechnique.org
 License: UNKNOWN
-Download-URL: https://github.com/jeanollion/PyBacmman/archive/v_051.tar.gz
+Download-URL: https://github.com/jeanollion/PyBacmman/archive/v_052.tar.gz
 Keywords: bacmman,pandas,data analysis
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
@@ -19,8 +19,10 @@
 License-File: LICENSE
 
 # PyBacmman
 - Helper functions to manipulate data generated by [BACMMAN software](https://github.com/jeanollion/bacmman) uder Pandas, see `pybacmman.pandas` module.
 - Helper functions to save selection from pandas to BACMMAN: see `pybacmman.selections.saveAndOpenSelection()` method.
 - Dataset class to facilitate handling of measurement tables and selections: see `pybacmman.dataset.Dataset` and `pybacmman.dataset.DatasetList` classes.
 
+Here is [another python package](https://gitlab.com/MEKlab/pyberries) to handle bacmman data.
+
```

### Comparing `PyBacmman-0.5.1/PyBacmman.egg-info/PKG-INFO` & `PyBacmman-0.5.2/PyBacmman.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PyBacmman
-Version: 0.5.1
+Version: 0.5.2
 Summary: Utilities for analysis of data generated from bacmman software
 Home-page: https://github.com/jeanollion/PyBacmman.git
 Author: Jean Ollion
 Author-email: jean.ollion@polytechnique.org
 License: UNKNOWN
-Download-URL: https://github.com/jeanollion/PyBacmman/archive/v_051.tar.gz
+Download-URL: https://github.com/jeanollion/PyBacmman/archive/v_052.tar.gz
 Keywords: bacmman,pandas,data analysis
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
@@ -19,8 +19,10 @@
 License-File: LICENSE
 
 # PyBacmman
 - Helper functions to manipulate data generated by [BACMMAN software](https://github.com/jeanollion/bacmman) uder Pandas, see `pybacmman.pandas` module.
 - Helper functions to save selection from pandas to BACMMAN: see `pybacmman.selections.saveAndOpenSelection()` method.
 - Dataset class to facilitate handling of measurement tables and selections: see `pybacmman.dataset.Dataset` and `pybacmman.dataset.DatasetList` classes.
 
+Here is [another python package](https://gitlab.com/MEKlab/pyberries) to handle bacmman data.
+
```

### Comparing `PyBacmman-0.5.1/PyBacmman.egg-info/SOURCES.txt` & `PyBacmman-0.5.2/PyBacmman.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyBacmman-0.5.1/pybacmman/evaluation/run_tasks.py` & `PyBacmman-0.5.2/pybacmman/evaluation/run_tasks.py`

 * *Files identical despite different names*

### Comparing `PyBacmman-0.5.1/pybacmman/pandas/curve_utils.py` & `PyBacmman-0.5.2/pybacmman/pandas/curve_utils.py`

 * *Files identical despite different names*

### Comparing `PyBacmman-0.5.1/pybacmman/pandas/indices_utils.py` & `PyBacmman-0.5.2/pybacmman/pandas/indices_utils.py`

 * *Files identical despite different names*

### Comparing `PyBacmman-0.5.1/pybacmman/pandas/pandas_utils.py` & `PyBacmman-0.5.2/pybacmman/pandas/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `PyBacmman-0.5.1/pybacmman/selections/selections.py` & `PyBacmman-0.5.2/pybacmman/selections/selections.py`

 * *Files identical despite different names*

### Comparing `PyBacmman-0.5.1/setup.py` & `PyBacmman-0.5.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="PyBacmman",
-    version="0.5.1",
+    version="0.5.2",
     author="Jean Ollion",
     author_email="jean.ollion@polytechnique.org",
     description="Utilities for analysis of data generated from bacmman software",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jeanollion/PyBacmman.git",
-    download_url = 'https://github.com/jeanollion/PyBacmman/archive/v_051.tar.gz',
+    download_url = 'https://github.com/jeanollion/PyBacmman/archive/v_052.tar.gz',
     packages=setuptools.find_packages(),
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Science/Research',
         "Programming Language :: Python :: 3",
         'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
         "Operating System :: OS Independent",
```

