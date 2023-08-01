# Comparing `tmp/pyweatherlite-0.0.1.tar.gz` & `tmp/pyweatherlite-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyweatherlite-0.0.1.tar", last modified: Mon Jul 31 19:09:03 2023, max compression
+gzip compressed data, was "pyweatherlite-0.1.0.tar", last modified: Tue Aug  1 12:45:20 2023, max compression
```

## Comparing `pyweatherlite-0.0.1.tar` & `pyweatherlite-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-07-31 19:09:03.726276 pyweatherlite-0.0.1/
--rw-rw-r--   0 mike      (1000) mike      (1000)     1073 2023-07-31 14:38:44.000000 pyweatherlite-0.0.1/LICENSE
--rw-rw-r--   0 mike      (1000) mike      (1000)     3224 2023-07-31 19:09:03.726276 pyweatherlite-0.0.1/PKG-INFO
--rw-rw-r--   0 mike      (1000) mike      (1000)     2881 2023-07-31 19:06:02.000000 pyweatherlite-0.0.1/README.md
--rw-rw-r--   0 mike      (1000) mike      (1000)       38 2023-07-31 19:09:03.726276 pyweatherlite-0.0.1/setup.cfg
--rw-rw-r--   0 mike      (1000) mike      (1000)      724 2023-07-31 19:02:27.000000 pyweatherlite-0.0.1/setup.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-07-31 19:09:03.722276 pyweatherlite-0.0.1/src/
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-07-31 19:09:03.722276 pyweatherlite-0.0.1/src/pyweatherlite/
--rw-rw-r--   0 mike      (1000) mike      (1000)      701 2023-07-31 17:52:13.000000 pyweatherlite-0.0.1/src/pyweatherlite/Base.py
--rw-rw-r--   0 mike      (1000) mike      (1000)        0 2023-07-30 13:23:36.000000 pyweatherlite-0.0.1/src/pyweatherlite/__init__.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     1295 2023-07-31 17:25:29.000000 pyweatherlite-0.0.1/src/pyweatherlite/helpers.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     4135 2023-07-31 18:34:02.000000 pyweatherlite-0.0.1/src/pyweatherlite/index.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-07-31 19:09:03.722276 pyweatherlite-0.0.1/src/pyweatherlite.egg-info/
--rw-rw-r--   0 mike      (1000) mike      (1000)     3224 2023-07-31 19:09:03.000000 pyweatherlite-0.0.1/src/pyweatherlite.egg-info/PKG-INFO
--rw-rw-r--   0 mike      (1000) mike      (1000)      386 2023-07-31 19:09:03.000000 pyweatherlite-0.0.1/src/pyweatherlite.egg-info/SOURCES.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)        1 2023-07-31 19:09:03.000000 pyweatherlite-0.0.1/src/pyweatherlite.egg-info/dependency_links.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)       60 2023-07-31 19:09:03.000000 pyweatherlite-0.0.1/src/pyweatherlite.egg-info/entry_points.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)        9 2023-07-31 19:09:03.000000 pyweatherlite-0.0.1/src/pyweatherlite.egg-info/requires.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)       14 2023-07-31 19:09:03.000000 pyweatherlite-0.0.1/src/pyweatherlite.egg-info/top_level.txt
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-08-01 12:45:20.570766 pyweatherlite-0.1.0/
+-rw-rw-r--   0 mike      (1000) mike      (1000)     1073 2023-07-31 14:38:44.000000 pyweatherlite-0.1.0/LICENSE
+-rw-rw-r--   0 mike      (1000) mike      (1000)     3224 2023-08-01 12:45:20.570766 pyweatherlite-0.1.0/PKG-INFO
+-rw-rw-r--   0 mike      (1000) mike      (1000)     2881 2023-07-31 19:06:02.000000 pyweatherlite-0.1.0/README.md
+-rw-rw-r--   0 mike      (1000) mike      (1000)       38 2023-08-01 12:45:20.574766 pyweatherlite-0.1.0/setup.cfg
+-rw-rw-r--   0 mike      (1000) mike      (1000)      728 2023-08-01 12:39:59.000000 pyweatherlite-0.1.0/setup.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-08-01 12:45:20.566766 pyweatherlite-0.1.0/src/
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-08-01 12:45:20.570766 pyweatherlite-0.1.0/src/pyweatherlite/
+-rw-rw-r--   0 mike      (1000) mike      (1000)      701 2023-07-31 17:52:13.000000 pyweatherlite-0.1.0/src/pyweatherlite/Base.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)        0 2023-07-30 13:23:36.000000 pyweatherlite-0.1.0/src/pyweatherlite/__init__.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     1295 2023-07-31 17:25:29.000000 pyweatherlite-0.1.0/src/pyweatherlite/helpers.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     4135 2023-07-31 18:34:02.000000 pyweatherlite-0.1.0/src/pyweatherlite/index.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-08-01 12:45:20.570766 pyweatherlite-0.1.0/src/pyweatherlite.egg-info/
+-rw-rw-r--   0 mike      (1000) mike      (1000)     3224 2023-08-01 12:45:20.000000 pyweatherlite-0.1.0/src/pyweatherlite.egg-info/PKG-INFO
+-rw-rw-r--   0 mike      (1000) mike      (1000)      386 2023-08-01 12:45:20.000000 pyweatherlite-0.1.0/src/pyweatherlite.egg-info/SOURCES.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)        1 2023-08-01 12:45:20.000000 pyweatherlite-0.1.0/src/pyweatherlite.egg-info/dependency_links.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)       64 2023-08-01 12:45:20.000000 pyweatherlite-0.1.0/src/pyweatherlite.egg-info/entry_points.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)        9 2023-08-01 12:45:20.000000 pyweatherlite-0.1.0/src/pyweatherlite.egg-info/requires.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)       14 2023-08-01 12:45:20.000000 pyweatherlite-0.1.0/src/pyweatherlite.egg-info/top_level.txt
```

### Comparing `pyweatherlite-0.0.1/LICENSE` & `pyweatherlite-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyweatherlite-0.0.1/PKG-INFO` & `pyweatherlite-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyweatherlite
-Version: 0.0.1
+Version: 0.1.0
 Summary: A lightweight python library to extract weather data
 Home-page: https://github.com/Terre8055/pyweatherlite
 Author: Michael Appiah Dankwah
 Author-email: michaelappiah2018@icloud.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pyweatherlite-0.0.1/README.md` & `pyweatherlite-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pyweatherlite-0.0.1/setup.py` & `pyweatherlite-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pyweatherlite',
-    version='0.0.1',
+    version='0.1.0',
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     install_requires=[
         'requests',
     ],
     entry_points={
         'console_scripts': [
-            'pyweatherlite = pyweatherlite.index:main',
+            'pyweatherlite = pyweatherlite.index:Scaffold',
         ],
     },
     # Other metadata like author, description, etc.
     author='Michael Appiah Dankwah',
     author_email='michaelappiah2018@icloud.com',
     description='A lightweight python library to extract weather data',
     long_description=open('README.md').read(),
```

### Comparing `pyweatherlite-0.0.1/src/pyweatherlite/Base.py` & `pyweatherlite-0.1.0/src/pyweatherlite/Base.py`

 * *Files identical despite different names*

### Comparing `pyweatherlite-0.0.1/src/pyweatherlite/helpers.py` & `pyweatherlite-0.1.0/src/pyweatherlite/helpers.py`

 * *Files identical despite different names*

### Comparing `pyweatherlite-0.0.1/src/pyweatherlite/index.py` & `pyweatherlite-0.1.0/src/pyweatherlite/index.py`

 * *Files identical despite different names*

### Comparing `pyweatherlite-0.0.1/src/pyweatherlite.egg-info/PKG-INFO` & `pyweatherlite-0.1.0/src/pyweatherlite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyweatherlite
-Version: 0.0.1
+Version: 0.1.0
 Summary: A lightweight python library to extract weather data
 Home-page: https://github.com/Terre8055/pyweatherlite
 Author: Michael Appiah Dankwah
 Author-email: michaelappiah2018@icloud.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

