# Comparing `tmp/gspatial_tools-0.1.0.tar.gz` & `tmp/gspatial_tools-0.1.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gspatial_tools-0.1.0.tar", last modified: Tue Aug  1 12:16:54 2023, max compression
+gzip compressed data, was "gspatial_tools-0.1.0a0.tar", last modified: Thu Jul 27 15:38:21 2023, max compression
```

## Comparing `gspatial_tools-0.1.0.tar` & `gspatial_tools-0.1.0a0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 ambee      (501) staff       (20)        0 2023-08-01 12:16:54.834378 gspatial_tools-0.1.0/
--rw-r--r--   0 ambee      (501) staff       (20)     1062 2023-07-21 11:09:21.000000 gspatial_tools-0.1.0/LICENSE
--rw-r--r--   0 ambee      (501) staff       (20)     2030 2023-08-01 12:16:54.834434 gspatial_tools-0.1.0/PKG-INFO
--rwxr-xr-x   0 ambee      (501) staff       (20)     1482 2023-07-28 07:47:27.000000 gspatial_tools-0.1.0/README.md
-drwxr-xr-x   0 ambee      (501) staff       (20)        0 2023-08-01 12:16:54.833389 gspatial_tools-0.1.0/gspatial_tools/
--rwxr-xr-x   0 ambee      (501) staff       (20)       29 2023-07-27 09:13:05.000000 gspatial_tools-0.1.0/gspatial_tools/__init__.py
--rw-r--r--   0 ambee      (501) staff       (20)    15424 2023-07-27 15:18:24.000000 gspatial_tools-0.1.0/gspatial_tools/gspatial_tools.py
-drwxr-xr-x   0 ambee      (501) staff       (20)        0 2023-08-01 12:16:54.834179 gspatial_tools-0.1.0/gspatial_tools.egg-info/
--rw-r--r--   0 ambee      (501) staff       (20)     2030 2023-08-01 12:16:54.000000 gspatial_tools-0.1.0/gspatial_tools.egg-info/PKG-INFO
--rw-r--r--   0 ambee      (501) staff       (20)      309 2023-08-01 12:16:54.000000 gspatial_tools-0.1.0/gspatial_tools.egg-info/SOURCES.txt
--rw-r--r--   0 ambee      (501) staff       (20)        1 2023-08-01 12:16:54.000000 gspatial_tools-0.1.0/gspatial_tools.egg-info/dependency_links.txt
--rw-r--r--   0 ambee      (501) staff       (20)      115 2023-08-01 12:16:54.000000 gspatial_tools-0.1.0/gspatial_tools.egg-info/requires.txt
--rw-r--r--   0 ambee      (501) staff       (20)       15 2023-08-01 12:16:54.000000 gspatial_tools-0.1.0/gspatial_tools.egg-info/top_level.txt
--rwxr-xr-x   0 ambee      (501) staff       (20)       79 2023-08-01 12:16:54.834633 gspatial_tools-0.1.0/setup.cfg
--rwxr-xr-x   0 ambee      (501) staff       (20)     1195 2023-08-01 12:15:59.000000 gspatial_tools-0.1.0/setup.py
-drwxr-xr-x   0 ambee      (501) staff       (20)        0 2023-08-01 12:16:54.834287 gspatial_tools-0.1.0/tests/
--rwxr-xr-x   0 ambee      (501) staff       (20)        0 2023-01-21 20:20:29.000000 gspatial_tools-0.1.0/tests/test_functions.py
+drwxr-xr-x   0 ambee      (501) staff       (20)        0 2023-07-27 15:38:21.547030 gspatial_tools-0.1.0a0/
+-rw-r--r--   0 ambee      (501) staff       (20)     1062 2023-07-21 11:09:21.000000 gspatial_tools-0.1.0a0/LICENSE
+-rw-r--r--   0 ambee      (501) staff       (20)     1430 2023-07-27 15:38:21.547079 gspatial_tools-0.1.0a0/PKG-INFO
+-rwxr-xr-x   0 ambee      (501) staff       (20)      879 2023-07-27 15:13:26.000000 gspatial_tools-0.1.0a0/README.md
+drwxr-xr-x   0 ambee      (501) staff       (20)        0 2023-07-27 15:38:21.546278 gspatial_tools-0.1.0a0/gspatial_tools/
+-rwxr-xr-x   0 ambee      (501) staff       (20)       29 2023-07-27 09:13:05.000000 gspatial_tools-0.1.0a0/gspatial_tools/__init__.py
+-rw-r--r--   0 ambee      (501) staff       (20)    15424 2023-07-27 15:18:24.000000 gspatial_tools-0.1.0a0/gspatial_tools/gspatial_tools.py
+drwxr-xr-x   0 ambee      (501) staff       (20)        0 2023-07-27 15:38:21.546843 gspatial_tools-0.1.0a0/gspatial_tools.egg-info/
+-rw-r--r--   0 ambee      (501) staff       (20)     1430 2023-07-27 15:38:21.000000 gspatial_tools-0.1.0a0/gspatial_tools.egg-info/PKG-INFO
+-rw-r--r--   0 ambee      (501) staff       (20)      309 2023-07-27 15:38:21.000000 gspatial_tools-0.1.0a0/gspatial_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 ambee      (501) staff       (20)        1 2023-07-27 15:38:21.000000 gspatial_tools-0.1.0a0/gspatial_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 ambee      (501) staff       (20)      115 2023-07-27 15:38:21.000000 gspatial_tools-0.1.0a0/gspatial_tools.egg-info/requires.txt
+-rw-r--r--   0 ambee      (501) staff       (20)       15 2023-07-27 15:38:21.000000 gspatial_tools-0.1.0a0/gspatial_tools.egg-info/top_level.txt
+-rwxr-xr-x   0 ambee      (501) staff       (20)       79 2023-07-27 15:38:21.547483 gspatial_tools-0.1.0a0/setup.cfg
+-rwxr-xr-x   0 ambee      (501) staff       (20)     1197 2023-07-27 09:15:50.000000 gspatial_tools-0.1.0a0/setup.py
+drwxr-xr-x   0 ambee      (501) staff       (20)        0 2023-07-27 15:38:21.546952 gspatial_tools-0.1.0a0/tests/
+-rwxr-xr-x   0 ambee      (501) staff       (20)        0 2023-01-21 20:20:29.000000 gspatial_tools-0.1.0a0/tests/test_functions.py
```

### Comparing `gspatial_tools-0.1.0/LICENSE` & `gspatial_tools-0.1.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `gspatial_tools-0.1.0/gspatial_tools/gspatial_tools.py` & `gspatial_tools-0.1.0a0/gspatial_tools/gspatial_tools.py`

 * *Files identical despite different names*

### Comparing `gspatial_tools-0.1.0/setup.py` & `gspatial_tools-0.1.0a0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 long_description = open(os.path.join(here, "README.md")).read()
 
 setup(
     name="gspatial_tools",
     packages=find_packages(include=["gspatial_tools"]),
-    version="0.1.0",
+    version="0.1.0a",
     author="Ambee",
     license="MIT",
     url="https://github.com/ambeelabs/gspatial_tools/",
     description="Set of utility tools built on top of Geopandas, Xarray, Rasterio and Rioxarray",
     long_description_content_type="text/markdown",
     long_description=long_description,
     install_requires=[
@@ -21,15 +21,15 @@
         "pandas>=1.5.3",
         "rasterio>=1.3.8",
         "rioxarray>=0.13.3",
         "scikit_learn>=1.2.0",
         "shapely>=2.0.1",
     ],
     classifiers=[
-        "Development Status :: 4 - Beta",
+        "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.10",
     ],
     keywords="geospatial utilities geopandas rasterio rioxarray xarray",
     setup_requires=["pytest-runner"],
     tests_require=["pytest"],
```

