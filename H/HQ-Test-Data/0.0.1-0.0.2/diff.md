# Comparing `tmp/HQ_Test_Data-0.0.1.tar.gz` & `tmp/HQ_Test_Data-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HQ_Test_Data-0.0.1.tar", last modified: Tue Aug  1 08:28:28 2023, max compression
+gzip compressed data, was "HQ_Test_Data-0.0.2.tar", last modified: Tue Aug  1 08:47:27 2023, max compression
```

## Comparing `HQ_Test_Data-0.0.1.tar` & `HQ_Test_Data-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 08:28:29.103650 HQ_Test_Data-0.0.1/
--rw-rw-rw-   0        0        0     1079 2023-08-01 08:06:48.000000 HQ_Test_Data-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1696 2023-08-01 08:28:29.009664 HQ_Test_Data-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      229 2023-08-01 08:05:27.000000 HQ_Test_Data-0.0.1/README.md
--rw-rw-rw-   0        0        0      389 2023-08-01 08:27:56.000000 HQ_Test_Data-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-01 08:28:29.109657 HQ_Test_Data-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-01 08:28:25.934646 HQ_Test_Data-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-08-01 08:28:27.181649 HQ_Test_Data-0.0.1/src/HQ_Test_Data/
--rw-rw-rw-   0        0        0       33 2023-08-01 07:59:40.000000 HQ_Test_Data-0.0.1/src/HQ_Test_Data/__init__.py
--rw-rw-rw-   0        0        0     3354 2023-08-01 07:57:25.000000 HQ_Test_Data-0.0.1/src/HQ_Test_Data/main.py
-drwxrwxrwx   0        0        0        0 2023-08-01 08:28:28.729650 HQ_Test_Data-0.0.1/src/HQ_Test_Data.egg-info/
--rw-rw-rw-   0        0        0     1696 2023-08-01 08:28:24.000000 HQ_Test_Data-0.0.1/src/HQ_Test_Data.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2023-08-01 08:28:25.000000 HQ_Test_Data-0.0.1/src/HQ_Test_Data.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 08:28:24.000000 HQ_Test_Data-0.0.1/src/HQ_Test_Data.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-08-01 08:28:25.000000 HQ_Test_Data-0.0.1/src/HQ_Test_Data.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-08-01 08:28:25.000000 HQ_Test_Data-0.0.1/src/HQ_Test_Data.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 08:47:28.065493 HQ_Test_Data-0.0.2/
+-rw-rw-rw-   0        0        0     1079 2023-08-01 08:06:48.000000 HQ_Test_Data-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1792 2023-08-01 08:47:27.979461 HQ_Test_Data-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      325 2023-08-01 08:42:54.000000 HQ_Test_Data-0.0.2/README.md
+-rw-rw-rw-   0        0        0      373 2023-08-01 08:47:03.000000 HQ_Test_Data-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-01 08:47:28.070466 HQ_Test_Data-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-01 08:47:25.011461 HQ_Test_Data-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-08-01 08:47:26.224456 HQ_Test_Data-0.0.2/src/HQ_Test_Data/
+-rw-rw-rw-   0        0        0       33 2023-08-01 07:59:40.000000 HQ_Test_Data-0.0.2/src/HQ_Test_Data/__init__.py
+-rw-rw-rw-   0        0        0     3354 2023-08-01 07:57:25.000000 HQ_Test_Data-0.0.2/src/HQ_Test_Data/main.py
+drwxrwxrwx   0        0        0        0 2023-08-01 08:47:27.681459 HQ_Test_Data-0.0.2/src/HQ_Test_Data.egg-info/
+-rw-rw-rw-   0        0        0     1792 2023-08-01 08:47:24.000000 HQ_Test_Data-0.0.2/src/HQ_Test_Data.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2023-08-01 08:47:24.000000 HQ_Test_Data-0.0.2/src/HQ_Test_Data.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 08:47:24.000000 HQ_Test_Data-0.0.2/src/HQ_Test_Data.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-08-01 08:47:24.000000 HQ_Test_Data-0.0.2/src/HQ_Test_Data.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-08-01 08:47:24.000000 HQ_Test_Data-0.0.2/src/HQ_Test_Data.egg-info/top_level.txt
```

### Comparing `HQ_Test_Data-0.0.1/LICENSE` & `HQ_Test_Data-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `HQ_Test_Data-0.0.1/PKG-INFO` & `HQ_Test_Data-0.0.2/src/HQ_Test_Data.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: HQ_Test_Data
-Version: 0.0.1
+Name: HQ-Test-Data
+Version: 0.0.2
 Summary: A Python package to fetch and print data.
 Author-email: Hossam Ibrahim <hossam.ibrahim@hlag.com>
 License: Copyright (c) [2023] [Hossam_Ibrahim]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -21,17 +21,18 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# My Package
+# HQ_Test_Data
 
 This is a Python package that connects to a specific database and fetches certain data based on user permissions.
 
 ## Installation
 
-This package can be installed via pip:
+Before installing this package, ensure that `pymssql` is installed. You can install it via conda:
 
 ```bash
+conda install -c anaconda pymssql
 pip install HQ_Test_Data
```

### Comparing `HQ_Test_Data-0.0.1/src/HQ_Test_Data/main.py` & `HQ_Test_Data-0.0.2/src/HQ_Test_Data/main.py`

 * *Files identical despite different names*

