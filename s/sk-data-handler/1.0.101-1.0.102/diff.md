# Comparing `tmp/sk_data_handler-1.0.101.tar.gz` & `tmp/sk_data_handler-1.0.102.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sk_data_handler-1.0.101.tar", last modified: Tue Aug  1 17:17:15 2023, max compression
+gzip compressed data, was "sk_data_handler-1.0.102.tar", last modified: Tue Aug  1 17:30:39 2023, max compression
```

## Comparing `sk_data_handler-1.0.101.tar` & `sk_data_handler-1.0.102.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 17:17:15.195012 sk_data_handler-1.0.101/
--rw-rw-rw-   0        0        0     1055 2023-07-18 15:19:22.000000 sk_data_handler-1.0.101/LICENSE.txt
--rw-rw-rw-   0        0        0     7595 2023-08-01 17:17:15.195012 sk_data_handler-1.0.101/PKG-INFO
--rw-rw-rw-   0        0        0     7117 2023-07-18 15:19:22.000000 sk_data_handler-1.0.101/README.md
--rw-rw-rw-   0        0        0       42 2023-08-01 17:17:15.195012 sk_data_handler-1.0.101/setup.cfg
--rw-rw-rw-   0        0        0      803 2023-08-01 17:16:07.000000 sk_data_handler-1.0.101/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-01 17:17:15.179753 sk_data_handler-1.0.101/sk_data_handler/
--rw-rw-rw-   0        0        0        0 2023-07-23 05:28:15.000000 sk_data_handler-1.0.101/sk_data_handler/__init__.py
--rw-rw-rw-   0        0        0     1447 2023-07-31 18:43:47.000000 sk_data_handler-1.0.101/sk_data_handler/data.py
-drwxrwxrwx   0        0        0        0 2023-08-01 17:17:15.193998 sk_data_handler-1.0.101/sk_data_handler.egg-info/
--rw-rw-rw-   0        0        0     7595 2023-08-01 17:17:15.000000 sk_data_handler-1.0.101/sk_data_handler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      276 2023-08-01 17:17:15.000000 sk_data_handler-1.0.101/sk_data_handler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 17:17:15.000000 sk_data_handler-1.0.101/sk_data_handler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-08-01 17:17:15.000000 sk_data_handler-1.0.101/sk_data_handler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-08-01 17:17:15.000000 sk_data_handler-1.0.101/sk_data_handler.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 17:30:39.612878 sk_data_handler-1.0.102/
+-rw-rw-rw-   0        0        0     1055 2023-07-18 15:19:22.000000 sk_data_handler-1.0.102/LICENSE.txt
+-rw-rw-rw-   0        0        0     7595 2023-08-01 17:30:39.611828 sk_data_handler-1.0.102/PKG-INFO
+-rw-rw-rw-   0        0        0     7117 2023-07-18 15:19:22.000000 sk_data_handler-1.0.102/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-01 17:30:39.612878 sk_data_handler-1.0.102/setup.cfg
+-rw-rw-rw-   0        0        0      803 2023-08-01 17:27:53.000000 sk_data_handler-1.0.102/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 17:30:39.597665 sk_data_handler-1.0.102/sk_data_handler/
+-rw-rw-rw-   0        0        0        0 2023-07-23 05:28:15.000000 sk_data_handler-1.0.102/sk_data_handler/__init__.py
+-rw-rw-rw-   0        0        0     1413 2023-08-01 17:27:14.000000 sk_data_handler-1.0.102/sk_data_handler/data.py
+drwxrwxrwx   0        0        0        0 2023-08-01 17:30:39.610600 sk_data_handler-1.0.102/sk_data_handler.egg-info/
+-rw-rw-rw-   0        0        0     7595 2023-08-01 17:30:39.000000 sk_data_handler-1.0.102/sk_data_handler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      276 2023-08-01 17:30:39.000000 sk_data_handler-1.0.102/sk_data_handler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 17:30:39.000000 sk_data_handler-1.0.102/sk_data_handler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-08-01 17:30:39.000000 sk_data_handler-1.0.102/sk_data_handler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-08-01 17:30:39.000000 sk_data_handler-1.0.102/sk_data_handler.egg-info/top_level.txt
```

### Comparing `sk_data_handler-1.0.101/LICENSE.txt` & `sk_data_handler-1.0.102/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sk_data_handler-1.0.101/PKG-INFO` & `sk_data_handler-1.0.102/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sk_data_handler
-Version: 1.0.101
+Version: 1.0.102
 Summary: A simple Reporting program
 Author: gkibria
 Author-email: gkibria121@gmail.com
 Keywords: python,calculator,python calculator,gk calculator,advanced calculator
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sk_data_handler-1.0.101/README.md` & `sk_data_handler-1.0.102/README.md`

 * *Files identical despite different names*

### Comparing `sk_data_handler-1.0.101/setup.py` & `sk_data_handler-1.0.102/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='sk_data_handler',
-    version='1.0.101',
+    version='1.0.102',
     description='A simple Reporting program',
     author='gkibria',
     long_description=long_description,
     long_description_content_type="text/markdown",  # Specify the content type as Markdown
     author_email='gkibria121@gmail.com',
     packages=find_packages(),
     install_requires=['regex'],
```

### Comparing `sk_data_handler-1.0.101/sk_data_handler/data.py` & `sk_data_handler-1.0.102/sk_data_handler/data.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from .variable.sk_variable_handler.variable_handler import VariableHandler
-from .random_variable.sk_random_variable import RandomVariableGenerator
-from .table.sk_table_hanlder import TableHandler
+from sk_variable_handler.variable_handler import VariableHandler
+from sk_random_variable import RandomVariableGenerator
+from sk_table_hanlder import TableHandler
 from sk_regex import RegexMaker
 import regex as re
 
 class DataStructure:
     def __init__(self):
         self.random = RandomVariableGenerator()
         self.variable = VariableHandler()
```

### Comparing `sk_data_handler-1.0.101/sk_data_handler.egg-info/PKG-INFO` & `sk_data_handler-1.0.102/sk_data_handler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sk-data-handler
-Version: 1.0.101
+Version: 1.0.102
 Summary: A simple Reporting program
 Author: gkibria
 Author-email: gkibria121@gmail.com
 Keywords: python,calculator,python calculator,gk calculator,advanced calculator
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

