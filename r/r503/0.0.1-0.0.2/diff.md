# Comparing `tmp/r503-0.0.1.tar.gz` & `tmp/r503-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "r503-0.0.1.tar", last modified: Tue Aug  1 08:04:50 2023, max compression
+gzip compressed data, was "r503-0.0.2.tar", last modified: Tue Aug  1 18:18:47 2023, max compression
```

## Comparing `r503-0.0.1.tar` & `r503-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 08:04:50.579051 r503-0.0.1/
--rw-rw-rw-   0        0        0      656 2023-08-01 08:04:50.577056 r503-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-01 08:04:50.487061 r503-0.0.1/r503/
--rw-rw-rw-   0        0        0       21 2023-08-01 07:48:23.000000 r503-0.0.1/r503/__init__.py
--rw-rw-rw-   0        0        0    21063 2023-08-01 07:46:59.000000 r503-0.0.1/r503/r503.py
-drwxrwxrwx   0        0        0        0 2023-08-01 08:04:50.574046 r503-0.0.1/r503.egg-info/
--rw-rw-rw-   0        0        0      656 2023-08-01 08:04:50.000000 r503-0.0.1/r503.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      177 2023-08-01 08:04:50.000000 r503-0.0.1/r503.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 08:04:50.000000 r503-0.0.1/r503.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-08-01 08:04:50.000000 r503-0.0.1/r503.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-08-01 08:04:50.000000 r503-0.0.1/r503.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-01 08:04:50.580045 r503-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      965 2023-08-01 08:01:10.000000 r503-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 18:18:47.544811 r503-0.0.2/
+-rw-rw-rw-   0        0        0     1084 2023-08-01 18:02:28.000000 r503-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      700 2023-08-01 18:18:47.543812 r503-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-01 18:18:47.509308 r503-0.0.2/r503/
+-rw-rw-rw-   0        0        0    21063 2023-08-01 18:11:22.000000 r503-0.0.2/r503/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 18:18:47.541812 r503-0.0.2/r503.egg-info/
+-rw-rw-rw-   0        0        0      700 2023-08-01 18:18:47.000000 r503-0.0.2/r503.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      176 2023-08-01 18:18:47.000000 r503-0.0.2/r503.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 18:18:47.000000 r503-0.0.2/r503.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-08-01 18:18:47.000000 r503-0.0.2/r503.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-08-01 18:18:47.000000 r503-0.0.2/r503.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-01 18:18:47.544811 r503-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      986 2023-08-01 18:18:37.000000 r503-0.0.2/setup.py
```

### Comparing `r503-0.0.1/r503/r503.py` & `r503-0.0.2/r503/__init__.py`

 * *Files identical despite different names*

### Comparing `r503-0.0.1/setup.py` & `r503-0.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1'
 DESCRIPTION = 'Fingerprint reader R503'
-LONG_DESCRIPTION = 'A package that allows a computer to direct interface with GROW R503 finger print sensor without using external microcontroller'
-
+LONG_DESCRIPTION = 'A package that allows a computer to direct interface with GROW R503 finger print sensor without using an external microcontroller'
+VERSION = '0.0.2'
 # Setting up
 setup(
     name="r503",
-    version=VERSION,
     author="RoshanCS",
+    version=VERSION,
     author_email="<roshan.cs790@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
+    license='MIT',
     install_requires=['pyserial'],
     keywords=['python', 'fingerprint', 'security', 'grow', 'r503', 'password'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
```

