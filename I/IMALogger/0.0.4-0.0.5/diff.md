# Comparing `tmp/IMALogger-0.0.4.tar.gz` & `tmp/IMALogger-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IMALogger-0.0.4.tar", last modified: Tue Aug  1 03:16:11 2023, max compression
+gzip compressed data, was "IMALogger-0.0.5.tar", last modified: Tue Aug  1 03:19:00 2023, max compression
```

## Comparing `IMALogger-0.0.4.tar` & `IMALogger-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 03:16:11.389827 IMALogger-0.0.4/
-drwxrwxrwx   0        0        0        0 2023-08-01 03:16:11.364893 IMALogger-0.0.4/IMALogger/
--rw-rw-rw-   0        0        0     2356 2023-08-01 02:40:40.000000 IMALogger-0.0.4/IMALogger/IMALogger.py
--rw-rw-rw-   0        0        0       31 2023-08-01 03:15:30.000000 IMALogger-0.0.4/IMALogger/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 03:16:11.384840 IMALogger-0.0.4/IMALogger.egg-info/
--rw-rw-rw-   0        0        0      426 2023-08-01 03:16:11.000000 IMALogger-0.0.4/IMALogger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      203 2023-08-01 03:16:11.000000 IMALogger-0.0.4/IMALogger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 03:16:11.000000 IMALogger-0.0.4/IMALogger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-08-01 03:16:11.000000 IMALogger-0.0.4/IMALogger.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1086 2023-08-01 02:48:32.000000 IMALogger-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      426 2023-08-01 03:16:11.387832 IMALogger-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       64 2023-08-01 02:48:32.000000 IMALogger-0.0.4/README.md
--rw-rw-rw-   0        0        0       42 2023-08-01 03:16:11.389827 IMALogger-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      575 2023-08-01 03:16:07.000000 IMALogger-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 03:18:59.998863 IMALogger-0.0.5/
+drwxrwxrwx   0        0        0        0 2023-08-01 03:18:59.974926 IMALogger-0.0.5/IMALogger/
+-rw-rw-rw-   0        0        0     2359 2023-08-01 03:17:41.000000 IMALogger-0.0.5/IMALogger/IMALogger.py
+-rw-rw-rw-   0        0        0       44 2023-08-01 03:18:24.000000 IMALogger-0.0.5/IMALogger/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 03:18:59.993875 IMALogger-0.0.5/IMALogger.egg-info/
+-rw-rw-rw-   0        0        0      426 2023-08-01 03:18:59.000000 IMALogger-0.0.5/IMALogger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      203 2023-08-01 03:18:59.000000 IMALogger-0.0.5/IMALogger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 03:18:59.000000 IMALogger-0.0.5/IMALogger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-08-01 03:18:59.000000 IMALogger-0.0.5/IMALogger.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1086 2023-08-01 02:48:32.000000 IMALogger-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      426 2023-08-01 03:18:59.997864 IMALogger-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       64 2023-08-01 02:48:32.000000 IMALogger-0.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-01 03:18:59.998863 IMALogger-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      575 2023-08-01 03:18:51.000000 IMALogger-0.0.5/setup.py
```

### Comparing `IMALogger-0.0.4/IMALogger/IMALogger.py` & `IMALogger-0.0.5/IMALogger/IMALogger.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import datetime
 import re
 
-class logging:
+class IMALogging:
     def __init__(self, log_file_path=None, log_to_console=False, log_date_time=False, time_format_24hr=True):
         self.log_file_path = log_file_path
         self.log_to_console = log_to_console
         self.log_date_time = log_date_time
         self.time_format_24hr = time_format_24hr
         self.log_colors = {
             "DEBUG": "\033[94m",    # Blue
```

### Comparing `IMALogger-0.0.4/LICENSE` & `IMALogger-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `IMALogger-0.0.4/setup.py` & `IMALogger-0.0.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="IMALogger",
-    version="0.0.4",
+    version="0.0.5",
     packages=find_packages(),
     install_requires=[],
     author="1mag1n33dev",
     author_email="1mag1n33dev@gmail.com",
     description="Custom Logger Python Package",
     long_description="A custom logger implementation for Python.",
     url="https://github.com/1mag1n33/1m33-Logger-Py",
```

