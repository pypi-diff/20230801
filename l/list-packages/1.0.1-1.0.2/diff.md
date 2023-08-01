# Comparing `tmp/list_packages-1.0.1.tar.gz` & `tmp/list_packages-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "list_packages-1.0.1.tar", last modified: Tue Aug  1 10:17:53 2023, max compression
+gzip compressed data, was "list_packages-1.0.2.tar", last modified: Tue Aug  1 10:43:53 2023, max compression
```

## Comparing `list_packages-1.0.1.tar` & `list_packages-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:17:53.715582 list_packages-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-01 10:17:41.000000 list_packages-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-01 10:17:41.000000 list_packages-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-08-01 10:17:53.715582 list_packages-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-08-01 10:17:41.000000 list_packages-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:17:53.715582 list_packages-1.0.1/list_packages/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-01 10:17:41.000000 list_packages-1.0.1/list_packages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-08-01 10:17:41.000000 list_packages-1.0.1/list_packages/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:17:53.715582 list_packages-1.0.1/list_packages.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-08-01 10:17:53.000000 list_packages-1.0.1/list_packages.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-08-01 10:17:53.000000 list_packages-1.0.1/list_packages.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 10:17:53.000000 list_packages-1.0.1/list_packages.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-01 10:17:53.000000 list_packages-1.0.1/list_packages.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-01 10:17:53.000000 list_packages-1.0.1/list_packages.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 10:17:53.715582 list_packages-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-08-01 10:17:41.000000 list_packages-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:17:53.715582 list_packages-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-08-01 10:17:41.000000 list_packages-1.0.1/tests/test_list_packages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:43:53.535709 list_packages-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-01 10:43:43.000000 list_packages-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-01 10:43:43.000000 list_packages-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-08-01 10:43:53.535709 list_packages-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-08-01 10:43:43.000000 list_packages-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:43:53.531709 list_packages-1.0.2/list_packages/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-01 10:43:43.000000 list_packages-1.0.2/list_packages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-08-01 10:43:43.000000 list_packages-1.0.2/list_packages/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:43:53.535709 list_packages-1.0.2/list_packages.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-08-01 10:43:53.000000 list_packages-1.0.2/list_packages.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-08-01 10:43:53.000000 list_packages-1.0.2/list_packages.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 10:43:53.000000 list_packages-1.0.2/list_packages.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-01 10:43:53.000000 list_packages-1.0.2/list_packages.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-01 10:43:53.000000 list_packages-1.0.2/list_packages.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 10:43:53.535709 list_packages-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-08-01 10:43:43.000000 list_packages-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:43:53.535709 list_packages-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-08-01 10:43:43.000000 list_packages-1.0.2/tests/test_list_packages.py
```

### Comparing `list_packages-1.0.1/LICENSE` & `list_packages-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `list_packages-1.0.1/README.md` & `list_packages-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `list_packages-1.0.1/list_packages/main.py` & `list_packages-1.0.2/list_packages/main.py`

 * *Files identical despite different names*

### Comparing `list_packages-1.0.1/setup.py` & `list_packages-1.0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='list_packages',
-    version='1.0.1',
-    long_description='A package to list installed Python packages',
+    version='1.0.2',
+    long_description=open('README.md').read(),
+    long_description_content_type='text/markdown',
     author='Anand Maurya',
     author_email='anandmaurya@hotmail.com',
     platforms=['Any'],
     packages=find_packages(),
     url='https://github.com/maurya-anand/py-list-packages',
     entry_points={
         'console_scripts': ['list_packages=list_packages.main:command_line']
```

### Comparing `list_packages-1.0.1/tests/test_list_packages.py` & `list_packages-1.0.2/tests/test_list_packages.py`

 * *Files identical despite different names*

