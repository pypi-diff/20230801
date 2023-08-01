# Comparing `tmp/IMALogger-0.0.2.tar.gz` & `tmp/IMALogger-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IMALogger-0.0.2.tar", last modified: Tue Aug  1 03:07:04 2023, max compression
+gzip compressed data, was "IMALogger-0.0.3.tar", last modified: Tue Aug  1 03:14:10 2023, max compression
```

## Comparing `IMALogger-0.0.2.tar` & `IMALogger-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 03:07:04.146307 IMALogger-0.0.2/
-drwxrwxrwx   0        0        0        0 2023-08-01 03:07:04.117870 IMALogger-0.0.2/IMALogger/
--rw-rw-rw-   0        0        0     2356 2023-08-01 02:40:40.000000 IMALogger-0.0.2/IMALogger/IMALogger.py
--rw-rw-rw-   0        0        0        0 2023-08-01 02:43:25.000000 IMALogger-0.0.2/IMALogger/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 03:07:04.143315 IMALogger-0.0.2/IMALogger.egg-info/
--rw-rw-rw-   0        0        0      426 2023-08-01 03:07:03.000000 IMALogger-0.0.2/IMALogger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      203 2023-08-01 03:07:04.000000 IMALogger-0.0.2/IMALogger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 03:07:03.000000 IMALogger-0.0.2/IMALogger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-08-01 03:07:03.000000 IMALogger-0.0.2/IMALogger.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1086 2023-08-01 02:48:32.000000 IMALogger-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      426 2023-08-01 03:07:04.145309 IMALogger-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       64 2023-08-01 02:48:32.000000 IMALogger-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-08-01 03:07:04.147305 IMALogger-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      575 2023-08-01 03:06:55.000000 IMALogger-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 03:14:10.535820 IMALogger-0.0.3/
+drwxrwxrwx   0        0        0        0 2023-08-01 03:14:10.512881 IMALogger-0.0.3/IMALogger/
+-rw-rw-rw-   0        0        0     2356 2023-08-01 02:40:40.000000 IMALogger-0.0.3/IMALogger/IMALogger.py
+-rw-rw-rw-   0        0        0       30 2023-08-01 03:13:24.000000 IMALogger-0.0.3/IMALogger/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 03:14:10.531830 IMALogger-0.0.3/IMALogger.egg-info/
+-rw-rw-rw-   0        0        0      426 2023-08-01 03:14:10.000000 IMALogger-0.0.3/IMALogger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      203 2023-08-01 03:14:10.000000 IMALogger-0.0.3/IMALogger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 03:14:10.000000 IMALogger-0.0.3/IMALogger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-08-01 03:14:10.000000 IMALogger-0.0.3/IMALogger.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1086 2023-08-01 02:48:32.000000 IMALogger-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      426 2023-08-01 03:14:10.534823 IMALogger-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       64 2023-08-01 02:48:32.000000 IMALogger-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-01 03:14:10.536817 IMALogger-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      575 2023-08-01 03:13:58.000000 IMALogger-0.0.3/setup.py
```

### Comparing `IMALogger-0.0.2/IMALogger/IMALogger.py` & `IMALogger-0.0.3/IMALogger/IMALogger.py`

 * *Files identical despite different names*

### Comparing `IMALogger-0.0.2/LICENSE` & `IMALogger-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `IMALogger-0.0.2/setup.py` & `IMALogger-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="IMALogger",
-    version="0.0.2",
+    version="0.0.3",
     packages=find_packages(),
     install_requires=[],
     author="1mag1n33dev",
     author_email="1mag1n33dev@gmail.com",
     description="Custom Logger Python Package",
     long_description="A custom logger implementation for Python.",
     url="https://github.com/1mag1n33/1m33-Logger-Py",
```

