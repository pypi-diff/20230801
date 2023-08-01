# Comparing `tmp/list_packages-1.0.3.tar.gz` & `tmp/list_packages-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "list_packages-1.0.3.tar", last modified: Tue Aug  1 11:02:31 2023, max compression
+gzip compressed data, was "list_packages-1.0.4.tar", last modified: Tue Aug  1 11:52:02 2023, max compression
```

## Comparing `list_packages-1.0.3.tar` & `list_packages-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:02:31.854251 list_packages-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-01 11:02:21.000000 list_packages-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-01 11:02:21.000000 list_packages-1.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-08-01 11:02:31.850250 list_packages-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-08-01 11:02:21.000000 list_packages-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:02:31.850250 list_packages-1.0.3/list_packages/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-01 11:02:21.000000 list_packages-1.0.3/list_packages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-08-01 11:02:21.000000 list_packages-1.0.3/list_packages/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:02:31.850250 list_packages-1.0.3/list_packages.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-08-01 11:02:31.000000 list_packages-1.0.3/list_packages.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-08-01 11:02:31.000000 list_packages-1.0.3/list_packages.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:02:31.000000 list_packages-1.0.3/list_packages.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-01 11:02:31.000000 list_packages-1.0.3/list_packages.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-01 11:02:31.000000 list_packages-1.0.3/list_packages.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:02:31.854251 list_packages-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-08-01 11:02:21.000000 list_packages-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:02:31.850250 list_packages-1.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-08-01 11:02:21.000000 list_packages-1.0.3/tests/test_list_packages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:52:02.707060 list_packages-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-01 11:51:54.000000 list_packages-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-01 11:51:54.000000 list_packages-1.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-08-01 11:52:02.707060 list_packages-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-08-01 11:51:54.000000 list_packages-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:52:02.703060 list_packages-1.0.4/list_packages/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-01 11:51:54.000000 list_packages-1.0.4/list_packages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-08-01 11:51:54.000000 list_packages-1.0.4/list_packages/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:52:02.703060 list_packages-1.0.4/list_packages.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-08-01 11:52:02.000000 list_packages-1.0.4/list_packages.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-08-01 11:52:02.000000 list_packages-1.0.4/list_packages.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:52:02.000000 list_packages-1.0.4/list_packages.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-01 11:52:02.000000 list_packages-1.0.4/list_packages.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-01 11:52:02.000000 list_packages-1.0.4/list_packages.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:52:02.707060 list_packages-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-08-01 11:51:54.000000 list_packages-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:52:02.703060 list_packages-1.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-08-01 11:51:54.000000 list_packages-1.0.4/tests/test_list_packages.py
```

### Comparing `list_packages-1.0.3/LICENSE` & `list_packages-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `list_packages-1.0.3/PKG-INFO` & `list_packages-1.0.4/list_packages.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: list_packages
-Version: 1.0.3
+Name: list-packages
+Version: 1.0.4
 Summary: A package to list all the installed Python packages and their dependencies
 Home-page: https://github.com/maurya-anand/py-list-packages
 Author: Anand Maurya
 Author-email: anandmaurya@hotmail.com
 License: MIT
 Platform: Any
 Classifier: License :: OSI Approved :: MIT License
@@ -23,29 +23,19 @@
 
 A utility to retrieve a list of installed Python packages and their dependencies.
 
 Link to the [documentation](https://py-list-packages.readthedocs.io/).
 
 ## Installation
 
-Install via Terminal:
-
-1. Clone or download the repository from GitHub to your local computer.
-
-2. Open a terminal or command prompt and navigate to the root directory of the downloaded repository.
-
-3. (Optional) It is recommended to create a virtual environment to isolate the package dependencies. Run the following command to create a virtual environment (assuming you have `venv` installed):
-
-```bash
-cd list_packages
-python3 -m venv env
-pip3 install -e .
+``` python
+pip install list-packages
 ```
 
-Install via Pip:
+Alternative:
 
 ``` python
 pip install git+https://github.com/maurya-anand/py-list-packages.git
 ```
 
 ## Usage
```

### Comparing `list_packages-1.0.3/README.md` & `list_packages-1.0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,41 @@
+Metadata-Version: 2.1
+Name: list_packages
+Version: 1.0.4
+Summary: A package to list all the installed Python packages and their dependencies
+Home-page: https://github.com/maurya-anand/py-list-packages
+Author: Anand Maurya
+Author-email: anandmaurya@hotmail.com
+License: MIT
+Platform: Any
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # list_packages
 
 ![example workflow](https://github.com/maurya-anand/py-list-packages/actions/workflows/python-package.yml/badge.svg)
 
 A utility to retrieve a list of installed Python packages and their dependencies.
 
 Link to the [documentation](https://py-list-packages.readthedocs.io/).
 
 ## Installation
 
-Install via Terminal:
-
-1. Clone or download the repository from GitHub to your local computer.
-
-2. Open a terminal or command prompt and navigate to the root directory of the downloaded repository.
-
-3. (Optional) It is recommended to create a virtual environment to isolate the package dependencies. Run the following command to create a virtual environment (assuming you have `venv` installed):
-
-```bash
-cd list_packages
-python3 -m venv env
-pip3 install -e .
+``` python
+pip install list-packages
 ```
 
-Install via Pip:
+Alternative:
 
 ``` python
 pip install git+https://github.com/maurya-anand/py-list-packages.git
 ```
 
 ## Usage
```

### Comparing `list_packages-1.0.3/list_packages/main.py` & `list_packages-1.0.4/list_packages/main.py`

 * *Files identical despite different names*

### Comparing `list_packages-1.0.3/setup.py` & `list_packages-1.0.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='list_packages',
-    version='1.0.3',
+    version='1.0.4',
     description='A package to list all the installed Python packages and their dependencies',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Anand Maurya',
     author_email='anandmaurya@hotmail.com',
     platforms=['Any'],
     packages=find_packages(),
```

### Comparing `list_packages-1.0.3/tests/test_list_packages.py` & `list_packages-1.0.4/tests/test_list_packages.py`

 * *Files identical despite different names*

