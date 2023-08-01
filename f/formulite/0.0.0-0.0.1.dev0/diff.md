# Comparing `tmp/formulite-0.0.0.tar.gz` & `tmp/formulite-0.0.1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "formulite-0.0.0.tar", last modified: Tue Aug  1 14:25:21 2023, max compression
+gzip compressed data, was "formulite-0.0.1.dev0.tar", last modified: Tue Aug  1 15:01:26 2023, max compression
```

## Comparing `formulite-0.0.0.tar` & `formulite-0.0.1.dev0.tar`

### file list

```diff
@@ -1,10 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 14:25:21.661211 formulite-0.0.0/
--rw-rw-rw-   0        0        0      296 2023-08-01 14:25:21.661211 formulite-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       41 2023-08-01 13:35:39.000000 formulite-0.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-08-01 14:25:21.660234 formulite-0.0.0/formulite.egg-info/
--rw-rw-rw-   0        0        0      296 2023-08-01 14:25:21.000000 formulite-0.0.0/formulite.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      150 2023-08-01 14:25:21.000000 formulite-0.0.0/formulite.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 14:25:21.000000 formulite-0.0.0/formulite.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 14:25:21.000000 formulite-0.0.0/formulite.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-01 14:25:21.661211 formulite-0.0.0/setup.cfg
--rw-rw-rw-   0        0        0      539 2023-08-01 14:23:05.000000 formulite-0.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 15:01:26.640467 formulite-0.0.1.dev0/
+-rw-rw-rw-   0        0        0      301 2023-08-01 15:01:26.637841 formulite-0.0.1.dev0/PKG-INFO
+-rw-rw-rw-   0        0        0       41 2023-08-01 13:35:39.000000 formulite-0.0.1.dev0/README.md
+drwxrwxrwx   0        0        0        0 2023-08-01 15:01:26.628006 formulite-0.0.1.dev0/formulite/
+-rw-rw-rw-   0        0        0      112 2023-08-01 13:35:03.000000 formulite-0.0.1.dev0/formulite/__init__.py
+-rw-rw-rw-   0        0        0    14403 2023-07-28 00:52:13.000000 formulite-0.0.1.dev0/formulite/calc_parser.py
+drwxrwxrwx   0        0        0        0 2023-08-01 15:01:26.633856 formulite-0.0.1.dev0/formulite.egg-info/
+-rw-rw-rw-   0        0        0      301 2023-08-01 15:01:26.000000 formulite-0.0.1.dev0/formulite.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-08-01 15:01:26.000000 formulite-0.0.1.dev0/formulite.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 15:01:26.000000 formulite-0.0.1.dev0/formulite.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-08-01 15:01:26.000000 formulite-0.0.1.dev0/formulite.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-01 15:01:26.640467 formulite-0.0.1.dev0/setup.cfg
+-rw-rw-rw-   0        0        0      515 2023-08-01 15:00:50.000000 formulite-0.0.1.dev0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 15:01:26.635847 formulite-0.0.1.dev0/test/
+-rw-rw-rw-   0        0        0        0 2023-08-01 13:20:13.000000 formulite-0.0.1.dev0/test/__init__.py
+-rw-rw-rw-   0        0        0      251 2023-08-01 13:28:02.000000 formulite-0.0.1.dev0/test/main.py
```

### Comparing `formulite-0.0.0/setup.py` & `formulite-0.0.1.dev0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 from setuptools import setup,find_packages
 
 with open("README.md",encoding="utf-8",mode="r")as f:
     long_description = f.read()
 
 setup(
     name="formulite",
-    version="0.0.0",
+    version="0.0.1.dev0",
     description='Simple Formula Parser',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Tom0427',
     author_email='tom.ipynb@gmail.com',
     license='MIT',
     keywords='parser, formula, formulite',
     python_requires='>=3',
-    packages=find_packages(
-        where="src.*"
-    )
+    packages=find_packages()
 )
```

