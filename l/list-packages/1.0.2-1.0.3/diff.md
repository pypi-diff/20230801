# Comparing `tmp/list_packages-1.0.2.tar.gz` & `tmp/list_packages-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "list_packages-1.0.2.tar", last modified: Tue Aug  1 10:43:53 2023, max compression
+gzip compressed data, was "list_packages-1.0.3.tar", last modified: Tue Aug  1 11:02:31 2023, max compression
```

## Comparing `list_packages-1.0.2.tar` & `list_packages-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:43:53.535709 list_packages-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-01 10:43:43.000000 list_packages-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-01 10:43:43.000000 list_packages-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-08-01 10:43:53.535709 list_packages-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-08-01 10:43:43.000000 list_packages-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:43:53.531709 list_packages-1.0.2/list_packages/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-01 10:43:43.000000 list_packages-1.0.2/list_packages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-08-01 10:43:43.000000 list_packages-1.0.2/list_packages/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:43:53.535709 list_packages-1.0.2/list_packages.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-08-01 10:43:53.000000 list_packages-1.0.2/list_packages.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-08-01 10:43:53.000000 list_packages-1.0.2/list_packages.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 10:43:53.000000 list_packages-1.0.2/list_packages.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-01 10:43:53.000000 list_packages-1.0.2/list_packages.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-01 10:43:53.000000 list_packages-1.0.2/list_packages.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 10:43:53.535709 list_packages-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-08-01 10:43:43.000000 list_packages-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:43:53.535709 list_packages-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-08-01 10:43:43.000000 list_packages-1.0.2/tests/test_list_packages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:02:31.854251 list_packages-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-01 11:02:21.000000 list_packages-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-01 11:02:21.000000 list_packages-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-08-01 11:02:31.850250 list_packages-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-08-01 11:02:21.000000 list_packages-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:02:31.850250 list_packages-1.0.3/list_packages/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-01 11:02:21.000000 list_packages-1.0.3/list_packages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-08-01 11:02:21.000000 list_packages-1.0.3/list_packages/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:02:31.850250 list_packages-1.0.3/list_packages.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-08-01 11:02:31.000000 list_packages-1.0.3/list_packages.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-08-01 11:02:31.000000 list_packages-1.0.3/list_packages.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:02:31.000000 list_packages-1.0.3/list_packages.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-01 11:02:31.000000 list_packages-1.0.3/list_packages.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-01 11:02:31.000000 list_packages-1.0.3/list_packages.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:02:31.854251 list_packages-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-08-01 11:02:21.000000 list_packages-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:02:31.850250 list_packages-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-08-01 11:02:21.000000 list_packages-1.0.3/tests/test_list_packages.py
```

### Comparing `list_packages-1.0.2/LICENSE` & `list_packages-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `list_packages-1.0.2/PKG-INFO` & `list_packages-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: list_packages
-Version: 1.0.2
+Version: 1.0.3
+Summary: A package to list all the installed Python packages and their dependencies
 Home-page: https://github.com/maurya-anand/py-list-packages
 Author: Anand Maurya
 Author-email: anandmaurya@hotmail.com
 License: MIT
 Platform: Any
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `list_packages-1.0.2/README.md` & `list_packages-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `list_packages-1.0.2/list_packages/main.py` & `list_packages-1.0.3/list_packages/main.py`

 * *Files identical despite different names*

### Comparing `list_packages-1.0.2/list_packages.egg-info/PKG-INFO` & `list_packages-1.0.3/list_packages.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: list-packages
-Version: 1.0.2
+Version: 1.0.3
+Summary: A package to list all the installed Python packages and their dependencies
 Home-page: https://github.com/maurya-anand/py-list-packages
 Author: Anand Maurya
 Author-email: anandmaurya@hotmail.com
 License: MIT
 Platform: Any
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `list_packages-1.0.2/setup.py` & `list_packages-1.0.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='list_packages',
-    version='1.0.2',
+    version='1.0.3',
+    description='A package to list all the installed Python packages and their dependencies',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Anand Maurya',
     author_email='anandmaurya@hotmail.com',
     platforms=['Any'],
     packages=find_packages(),
     url='https://github.com/maurya-anand/py-list-packages',
```

### Comparing `list_packages-1.0.2/tests/test_list_packages.py` & `list_packages-1.0.3/tests/test_list_packages.py`

 * *Files identical despite different names*

