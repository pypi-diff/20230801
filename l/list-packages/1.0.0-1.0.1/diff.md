# Comparing `tmp/list_packages-1.0.0.tar.gz` & `tmp/list_packages-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "list_packages-1.0.0.tar", last modified: Tue Aug  1 09:59:59 2023, max compression
+gzip compressed data, was "list_packages-1.0.1.tar", last modified: Tue Aug  1 10:17:53 2023, max compression
```

## Comparing `list_packages-1.0.0.tar` & `list_packages-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:59:59.279050 list_packages-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-01 09:59:48.000000 list_packages-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-01 09:59:48.000000 list_packages-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-08-01 09:59:59.279050 list_packages-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-08-01 09:59:48.000000 list_packages-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:59:59.279050 list_packages-1.0.0/list_packages/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-01 09:59:48.000000 list_packages-1.0.0/list_packages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-08-01 09:59:48.000000 list_packages-1.0.0/list_packages/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:59:59.279050 list_packages-1.0.0/list_packages.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-08-01 09:59:59.000000 list_packages-1.0.0/list_packages.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-08-01 09:59:59.000000 list_packages-1.0.0/list_packages.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 09:59:59.000000 list_packages-1.0.0/list_packages.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-01 09:59:59.000000 list_packages-1.0.0/list_packages.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-01 09:59:59.000000 list_packages-1.0.0/list_packages.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 09:59:59.279050 list_packages-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-08-01 09:59:48.000000 list_packages-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:59:59.279050 list_packages-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-08-01 09:59:48.000000 list_packages-1.0.0/tests/test_list_packages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:17:53.715582 list_packages-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-01 10:17:41.000000 list_packages-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-01 10:17:41.000000 list_packages-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-08-01 10:17:53.715582 list_packages-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-08-01 10:17:41.000000 list_packages-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:17:53.715582 list_packages-1.0.1/list_packages/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-01 10:17:41.000000 list_packages-1.0.1/list_packages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-08-01 10:17:41.000000 list_packages-1.0.1/list_packages/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:17:53.715582 list_packages-1.0.1/list_packages.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-08-01 10:17:53.000000 list_packages-1.0.1/list_packages.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-08-01 10:17:53.000000 list_packages-1.0.1/list_packages.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 10:17:53.000000 list_packages-1.0.1/list_packages.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-01 10:17:53.000000 list_packages-1.0.1/list_packages.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-01 10:17:53.000000 list_packages-1.0.1/list_packages.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 10:17:53.715582 list_packages-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-08-01 10:17:41.000000 list_packages-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:17:53.715582 list_packages-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-08-01 10:17:41.000000 list_packages-1.0.1/tests/test_list_packages.py
```

### Comparing `list_packages-1.0.0/LICENSE` & `list_packages-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `list_packages-1.0.0/PKG-INFO` & `list_packages-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: list_packages
-Version: 1.0.0
+Version: 1.0.1
 Home-page: https://github.com/maurya-anand/py-list-packages
 Author: Anand Maurya
 Author-email: anandmaurya@hotmail.com
 License: MIT
 Platform: Any
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `list_packages-1.0.0/README.md` & `list_packages-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `list_packages-1.0.0/list_packages/main.py` & `list_packages-1.0.1/list_packages/main.py`

 * *Files identical despite different names*

### Comparing `list_packages-1.0.0/list_packages.egg-info/PKG-INFO` & `list_packages-1.0.1/list_packages.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: list-packages
-Version: 1.0.0
+Version: 1.0.1
 Home-page: https://github.com/maurya-anand/py-list-packages
 Author: Anand Maurya
 Author-email: anandmaurya@hotmail.com
 License: MIT
 Platform: Any
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `list_packages-1.0.0/setup.py` & `list_packages-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='list_packages',
-    version='1.0.0',
+    version='1.0.1',
     long_description='A package to list installed Python packages',
     author='Anand Maurya',
     author_email='anandmaurya@hotmail.com',
     platforms=['Any'],
     packages=find_packages(),
     url='https://github.com/maurya-anand/py-list-packages',
     entry_points={
```

### Comparing `list_packages-1.0.0/tests/test_list_packages.py` & `list_packages-1.0.1/tests/test_list_packages.py`

 * *Files identical despite different names*

