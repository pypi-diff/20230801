# Comparing `tmp/sk_variable_handler-1.0.101.tar.gz` & `tmp/sk_variable_handler-1.0.102.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sk_variable_handler-1.0.101.tar", last modified: Fri Jul 28 16:12:33 2023, max compression
+gzip compressed data, was "sk_variable_handler-1.0.102.tar", last modified: Tue Aug  1 17:22:14 2023, max compression
```

## Comparing `sk_variable_handler-1.0.101.tar` & `sk_variable_handler-1.0.102.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 16:12:33.787136 sk_variable_handler-1.0.101/
--rw-rw-rw-   0        0        0     1055 2023-07-18 15:19:22.000000 sk_variable_handler-1.0.101/LICENSE.txt
--rw-rw-rw-   0        0        0     3043 2023-07-28 16:12:33.787136 sk_variable_handler-1.0.101/PKG-INFO
--rw-rw-rw-   0        0        0     2596 2023-07-18 15:19:22.000000 sk_variable_handler-1.0.101/README.md
--rw-rw-rw-   0        0        0       42 2023-07-28 16:12:33.787136 sk_variable_handler-1.0.101/setup.cfg
--rw-rw-rw-   0        0        0      767 2023-07-28 16:12:27.000000 sk_variable_handler-1.0.101/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-28 16:12:33.771113 sk_variable_handler-1.0.101/sk_variable_handler/
--rw-rw-rw-   0        0        0        2 2023-07-18 15:19:22.000000 sk_variable_handler-1.0.101/sk_variable_handler/__init__.py
--rw-rw-rw-   0        0        0     6586 2023-07-18 15:19:22.000000 sk_variable_handler-1.0.101/sk_variable_handler/variable_handler.py
-drwxrwxrwx   0        0        0        0 2023-07-28 16:12:33.787136 sk_variable_handler-1.0.101/sk_variable_handler.egg-info/
--rw-rw-rw-   0        0        0     3043 2023-07-28 16:12:33.000000 sk_variable_handler-1.0.101/sk_variable_handler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      316 2023-07-28 16:12:33.000000 sk_variable_handler-1.0.101/sk_variable_handler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 16:12:33.000000 sk_variable_handler-1.0.101/sk_variable_handler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-28 16:12:33.000000 sk_variable_handler-1.0.101/sk_variable_handler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-07-28 16:12:33.000000 sk_variable_handler-1.0.101/sk_variable_handler.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 17:22:14.191716 sk_variable_handler-1.0.102/
+-rw-rw-rw-   0        0        0     1055 2023-07-18 15:19:22.000000 sk_variable_handler-1.0.102/LICENSE.txt
+-rw-rw-rw-   0        0        0     3043 2023-08-01 17:22:14.191716 sk_variable_handler-1.0.102/PKG-INFO
+-rw-rw-rw-   0        0        0     2596 2023-07-18 15:19:22.000000 sk_variable_handler-1.0.102/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-01 17:22:14.191716 sk_variable_handler-1.0.102/setup.cfg
+-rw-rw-rw-   0        0        0      767 2023-08-01 17:22:00.000000 sk_variable_handler-1.0.102/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 17:22:14.177283 sk_variable_handler-1.0.102/sk_variable_handler/
+-rw-rw-rw-   0        0        0        2 2023-07-18 15:19:22.000000 sk_variable_handler-1.0.102/sk_variable_handler/__init__.py
+-rw-rw-rw-   0        0        0     3192 2023-08-01 16:01:14.000000 sk_variable_handler-1.0.102/sk_variable_handler/variable_handler.py
+drwxrwxrwx   0        0        0        0 2023-08-01 17:22:14.190720 sk_variable_handler-1.0.102/sk_variable_handler.egg-info/
+-rw-rw-rw-   0        0        0     3043 2023-08-01 17:22:14.000000 sk_variable_handler-1.0.102/sk_variable_handler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      316 2023-08-01 17:22:14.000000 sk_variable_handler-1.0.102/sk_variable_handler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 17:22:14.000000 sk_variable_handler-1.0.102/sk_variable_handler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-08-01 17:22:14.000000 sk_variable_handler-1.0.102/sk_variable_handler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-08-01 17:22:14.000000 sk_variable_handler-1.0.102/sk_variable_handler.egg-info/top_level.txt
```

### Comparing `sk_variable_handler-1.0.101/LICENSE.txt` & `sk_variable_handler-1.0.102/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sk_variable_handler-1.0.101/PKG-INFO` & `sk_variable_handler-1.0.102/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sk_variable_handler
-Version: 1.0.101
+Version: 1.0.102
 Summary: A simple Variable Handling  program
 Author: gkibria
 Author-email: gkibria121@gmail.com
 Keywords: python,report generator
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sk_variable_handler-1.0.101/README.md` & `sk_variable_handler-1.0.102/README.md`

 * *Files identical despite different names*

### Comparing `sk_variable_handler-1.0.101/setup.py` & `sk_variable_handler-1.0.102/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='sk_variable_handler',
-    version='1.0.101',
+    version='1.0.102',
     description='A simple Variable Handling  program',
     author='gkibria',
     long_description=long_description,
     long_description_content_type="text/markdown",  # Specify the content type as Markdown
     author_email='gkibria121@gmail.com',
     packages=find_packages(),
     install_requires=['regex'],
```

### Comparing `sk_variable_handler-1.0.101/sk_variable_handler.egg-info/PKG-INFO` & `sk_variable_handler-1.0.102/sk_variable_handler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sk-variable-handler
-Version: 1.0.101
+Version: 1.0.102
 Summary: A simple Variable Handling  program
 Author: gkibria
 Author-email: gkibria121@gmail.com
 Keywords: python,report generator
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

