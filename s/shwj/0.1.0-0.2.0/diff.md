# Comparing `tmp/shwj-0.1.0.tar.gz` & `tmp/shwj-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\shwj-0.1.0.tar", last modified: Tue Aug  1 16:43:47 2023, max compression
+gzip compressed data, was "dist\shwj-0.2.0.tar", last modified: Tue Aug  1 17:40:13 2023, max compression
```

## Comparing `shwj-0.1.0.tar` & `shwj-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 16:43:47.000000 shwj-0.1.0/
--rw-rw-rw-   0        0        0     1106 2023-08-01 16:10:08.000000 shwj-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      678 2023-08-01 16:43:47.000000 shwj-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1694 2023-08-01 16:43:47.000000 shwj-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-08-01 16:43:47.000000 shwj-0.1.0/package1/
--rw-rw-rw-   0        0        0       70 2023-08-01 16:18:37.000000 shwj-0.1.0/package1/__init__.py
--rw-rw-rw-   0        0        0       72 2023-08-01 16:18:16.000000 shwj-0.1.0/package1/activation_functions.py
--rw-rw-rw-   0        0        0       39 2023-08-01 16:18:11.000000 shwj-0.1.0/package1/module1.py
--rw-rw-rw-   0        0        0       42 2023-08-01 16:43:47.000000 shwj-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      911 2023-08-01 16:39:30.000000 shwj-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-01 16:43:47.000000 shwj-0.1.0/shwj.egg-info/
--rw-rw-rw-   0        0        0      678 2023-08-01 16:43:47.000000 shwj-0.1.0/shwj.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      239 2023-08-01 16:43:47.000000 shwj-0.1.0/shwj.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 16:43:47.000000 shwj-0.1.0/shwj.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-08-01 16:43:47.000000 shwj-0.1.0/shwj.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-08-01 16:43:47.000000 shwj-0.1.0/shwj.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 17:40:13.000000 shwj-0.2.0/
+-rw-rw-rw-   0        0        0     1106 2023-08-01 16:10:08.000000 shwj-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0      678 2023-08-01 17:40:13.000000 shwj-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4746 2023-08-01 17:40:01.000000 shwj-0.2.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-01 17:40:13.000000 shwj-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      911 2023-08-01 17:35:26.000000 shwj-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 17:40:13.000000 shwj-0.2.0/shwj/
+-rw-rw-rw-   0        0        0       70 2023-08-01 16:18:37.000000 shwj-0.2.0/shwj/__init__.py
+-rw-rw-rw-   0        0        0       72 2023-08-01 16:18:16.000000 shwj-0.2.0/shwj/activation_functions.py
+-rw-rw-rw-   0        0        0       39 2023-08-01 16:18:11.000000 shwj-0.2.0/shwj/module1.py
+drwxrwxrwx   0        0        0        0 2023-08-01 17:40:13.000000 shwj-0.2.0/shwj.egg-info/
+-rw-rw-rw-   0        0        0      678 2023-08-01 17:40:13.000000 shwj-0.2.0/shwj.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-08-01 17:40:13.000000 shwj-0.2.0/shwj.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 17:40:13.000000 shwj-0.2.0/shwj.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-08-01 17:40:13.000000 shwj-0.2.0/shwj.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-08-01 17:40:13.000000 shwj-0.2.0/shwj.egg-info/top_level.txt
```

### Comparing `shwj-0.1.0/LICENSE` & `shwj-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `shwj-0.1.0/PKG-INFO` & `shwj-0.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shwj
-Version: 0.1.0
+Version: 0.2.0
 Summary: My package description
 Home-page: https://github.com/your-username/your-repo
 Author: shwj
 Author-email: 2591091196@email.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `shwj-0.1.0/setup.py` & `shwj-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='shwj',
-    version='0.1.0',
+    version='0.2.0',
     author='shwj',
     author_email='2591091196@email.com',
     description='My package description',
     long_description='Please refer to README.md for details.',
     long_description_content_type='text/markdown',
     url='https://github.com/your-username/your-repo',
     packages=find_packages(),
```

### Comparing `shwj-0.1.0/shwj.egg-info/PKG-INFO` & `shwj-0.2.0/shwj.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shwj
-Version: 0.1.0
+Version: 0.2.0
 Summary: My package description
 Home-page: https://github.com/your-username/your-repo
 Author: shwj
 Author-email: 2591091196@email.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

