# Comparing `tmp/Local_Xampp_Apache-0.0.2.tar.gz` & `tmp/Local_Xampp_Apache-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Local_Xampp_Apache-0.0.2.tar", last modified: Tue Aug  1 17:04:54 2023, max compression
+gzip compressed data, was "Local_Xampp_Apache-0.0.3.tar", last modified: Tue Aug  1 17:18:47 2023, max compression
```

## Comparing `Local_Xampp_Apache-0.0.2.tar` & `Local_Xampp_Apache-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 17:04:54.144462 Local_Xampp_Apache-0.0.2/
-drwxrwxrwx   0        0        0        0 2023-08-01 17:04:54.126877 Local_Xampp_Apache-0.0.2/Local_Xampp_Apache.egg-info/
--rw-rw-rw-   0        0        0      325 2023-08-01 17:04:53.000000 Local_Xampp_Apache-0.0.2/Local_Xampp_Apache.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      340 2023-08-01 17:04:53.000000 Local_Xampp_Apache-0.0.2/Local_Xampp_Apache.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 17:04:53.000000 Local_Xampp_Apache-0.0.2/Local_Xampp_Apache.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-08-01 17:04:53.000000 Local_Xampp_Apache-0.0.2/Local_Xampp_Apache.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       51 2023-08-01 17:04:53.000000 Local_Xampp_Apache-0.0.2/Local_Xampp_Apache.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-08-01 17:04:53.000000 Local_Xampp_Apache-0.0.2/Local_Xampp_Apache.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      325 2023-08-01 17:04:54.143464 Local_Xampp_Apache-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-08-01 16:22:15.000000 Local_Xampp_Apache-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-08-01 17:04:54.144462 Local_Xampp_Apache-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      759 2023-08-01 17:04:49.000000 Local_Xampp_Apache-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-01 17:04:54.131203 Local_Xampp_Apache-0.0.2/src/
--rw-rw-rw-   0        0        0        0 2023-08-01 16:21:41.000000 Local_Xampp_Apache-0.0.2/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 17:04:54.141459 Local_Xampp_Apache-0.0.2/src/lib/
--rw-rw-rw-   0        0        0     1148 2023-08-01 14:50:59.000000 Local_Xampp_Apache-0.0.2/src/lib/Commands.py
--rw-rw-rw-   0        0        0        0 2023-08-01 16:22:02.000000 Local_Xampp_Apache-0.0.2/src/lib/__init__.py
--rw-rw-rw-   0        0        0     1721 2023-08-01 17:04:00.000000 Local_Xampp_Apache-0.0.2/src/main.py
+drwxrwxrwx   0        0        0        0 2023-08-01 17:18:47.408725 Local_Xampp_Apache-0.0.3/
+drwxrwxrwx   0        0        0        0 2023-08-01 17:18:47.389519 Local_Xampp_Apache-0.0.3/Local_Xampp_Apache.egg-info/
+-rw-rw-rw-   0        0        0      840 2023-08-01 17:18:47.000000 Local_Xampp_Apache-0.0.3/Local_Xampp_Apache.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      340 2023-08-01 17:18:47.000000 Local_Xampp_Apache-0.0.3/Local_Xampp_Apache.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 17:18:47.000000 Local_Xampp_Apache-0.0.3/Local_Xampp_Apache.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-08-01 17:18:47.000000 Local_Xampp_Apache-0.0.3/Local_Xampp_Apache.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       51 2023-08-01 17:18:47.000000 Local_Xampp_Apache-0.0.3/Local_Xampp_Apache.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-08-01 17:18:47.000000 Local_Xampp_Apache-0.0.3/Local_Xampp_Apache.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      840 2023-08-01 17:18:47.407738 Local_Xampp_Apache-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      513 2023-08-01 17:17:42.000000 Local_Xampp_Apache-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-01 17:18:47.408725 Local_Xampp_Apache-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      812 2023-08-01 17:18:42.000000 Local_Xampp_Apache-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 17:18:47.394516 Local_Xampp_Apache-0.0.3/src/
+-rw-rw-rw-   0        0        0        0 2023-08-01 16:21:41.000000 Local_Xampp_Apache-0.0.3/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 17:18:47.404732 Local_Xampp_Apache-0.0.3/src/lib/
+-rw-rw-rw-   0        0        0     1148 2023-08-01 14:50:59.000000 Local_Xampp_Apache-0.0.3/src/lib/Commands.py
+-rw-rw-rw-   0        0        0        0 2023-08-01 16:22:02.000000 Local_Xampp_Apache-0.0.3/src/lib/__init__.py
+-rw-rw-rw-   0        0        0     1721 2023-08-01 17:04:00.000000 Local_Xampp_Apache-0.0.3/src/main.py
```

### Comparing `Local_Xampp_Apache-0.0.2/setup.py` & `Local_Xampp_Apache-0.0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from setuptools import setup, find_packages
 
 
 with open("requirements.txt") as f:
     required_packages = f.read().splitlines()
 
+with open('README.md', 'r', encoding='utf-8') as fh:
+    long_description = fh.read()
 
 
 setup(
     name="Local_Xampp_Apache",
-    version="0.0.2",
+    version="0.0.3",
     author="Sridhar",
     author_email="sridhardscv@gmail.com",
     description="Access the Windows XamPP Apache Server via Command lines",
-    # long_description="A longer description or README for your package",
+    long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://git.selfmade.ninja/SRIDHARDSCV/automate_xampp_windows",
     packages=find_packages(),
     python_requires=">=3.6",
     install_requires=required_packages,
     entry_points={
         "console_scripts": [
```

### Comparing `Local_Xampp_Apache-0.0.2/src/lib/Commands.py` & `Local_Xampp_Apache-0.0.3/src/lib/Commands.py`

 * *Files identical despite different names*

### Comparing `Local_Xampp_Apache-0.0.2/src/main.py` & `Local_Xampp_Apache-0.0.3/src/main.py`

 * *Files identical despite different names*

