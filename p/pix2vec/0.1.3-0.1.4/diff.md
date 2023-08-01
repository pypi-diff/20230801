# Comparing `tmp/pix2vec-0.1.3.tar.gz` & `tmp/pix2vec-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pix2vec-0.1.3.tar", last modified: Sun Jul  9 06:04:32 2023, max compression
+gzip compressed data, was "pix2vec-0.1.4.tar", last modified: Tue Aug  1 16:52:44 2023, max compression
```

## Comparing `pix2vec-0.1.3.tar` & `pix2vec-0.1.4.tar`

### file list

```diff
@@ -1,58 +1,60 @@
-drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-07-09 06:04:32.056028 pix2vec-0.1.3/
--rw-r--r--   0 alf        (501) staff       (20)     1204 2023-06-21 09:12:34.000000 pix2vec-0.1.3/.gitignore
--rw-r--r--   0 alf        (501) staff       (20)      205 2023-06-21 10:32:57.000000 pix2vec-0.1.3/.readthedocs.yaml
--rw-r--r--   0 alf        (501) staff       (20)      593 2023-07-09 06:02:38.000000 pix2vec-0.1.3/.zenodo.json
--rw-r--r--   0 alf        (501) staff       (20)      212 2023-06-21 09:38:53.000000 pix2vec-0.1.3/AUTHORS.rst
--rw-r--r--   0 alf        (501) staff       (20)      284 2023-07-07 14:13:32.000000 pix2vec-0.1.3/CITATION.cff
--rw-r--r--   0 alf        (501) staff       (20)     3524 2023-06-22 08:52:00.000000 pix2vec-0.1.3/CONTRIBUTING.rst
--rw-r--r--   0 alf        (501) staff       (20)      429 2023-07-09 06:04:28.000000 pix2vec-0.1.3/HISTORY.rst
--rw-r--r--   0 alf        (501) staff       (20)     1564 2023-06-21 09:12:34.000000 pix2vec-0.1.3/LICENSE
--rw-r--r--   0 alf        (501) staff       (20)      262 2023-06-21 09:12:34.000000 pix2vec-0.1.3/MANIFEST.in
--rw-r--r--   0 alf        (501) staff       (20)     2295 2023-06-21 09:12:34.000000 pix2vec-0.1.3/Makefile
--rw-r--r--   0 alf        (501) staff       (20)     5430 2023-07-09 06:04:32.056266 pix2vec-0.1.3/PKG-INFO
--rw-r--r--   0 alf        (501) staff       (20)     4034 2023-07-09 05:59:59.000000 pix2vec-0.1.3/README.rst
-drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-07-09 06:04:32.039224 pix2vec-0.1.3/docs/
--rw-r--r--   0 alf        (501) staff       (20)      608 2023-06-21 09:12:34.000000 pix2vec-0.1.3/docs/Makefile
-drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-07-09 06:04:32.021183 pix2vec-0.1.3/docs/_build/
-drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-07-09 06:04:32.021665 pix2vec-0.1.3/docs/_build/html/
-drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-07-09 06:04:32.039730 pix2vec-0.1.3/docs/_build/html/_images/
--rw-r--r--   0 alf        (501) staff       (20)   530877 2023-06-21 13:49:17.000000 pix2vec-0.1.3/docs/_build/html/_images/m3cube-a.png
-drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-07-09 06:04:32.042428 pix2vec-0.1.3/docs/_build/html/_static/
--rw-r--r--   0 alf        (501) staff       (20)      286 2021-10-12 12:18:02.000000 pix2vec-0.1.3/docs/_build/html/_static/file.png
--rw-r--r--   0 alf        (501) staff       (20)       90 2021-10-12 12:18:02.000000 pix2vec-0.1.3/docs/_build/html/_static/minus.png
--rw-r--r--   0 alf        (501) staff       (20)       90 2021-10-12 12:18:02.000000 pix2vec-0.1.3/docs/_build/html/_static/plus.png
--rw-r--r--   0 alf        (501) staff       (20)       28 2023-06-21 09:12:34.000000 pix2vec-0.1.3/docs/authors.rst
--rwxr-xr-x   0 alf        (501) staff       (20)     4876 2023-06-21 10:42:06.000000 pix2vec-0.1.3/docs/conf.py
--rw-r--r--   0 alf        (501) staff       (20)       33 2023-06-21 09:12:34.000000 pix2vec-0.1.3/docs/contributing.rst
--rw-r--r--   0 alf        (501) staff       (20)       28 2023-06-21 09:12:34.000000 pix2vec-0.1.3/docs/history.rst
-drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-07-09 06:04:32.047296 pix2vec-0.1.3/docs/images/
--rw-r--r--   0 alf        (501) staff       (20)   339139 2023-06-23 23:06:07.000000 pix2vec-0.1.3/docs/images/m3-PixelValue.png
--rw-r--r--   0 alf        (501) staff       (20)   337959 2023-06-23 23:06:07.000000 pix2vec-0.1.3/docs/images/m3-detail.png
--rw-r--r--   0 alf        (501) staff       (20)   530877 2023-06-21 13:49:17.000000 pix2vec-0.1.3/docs/images/m3cube-a.png
--rw-r--r--   0 alf        (501) staff       (20)   948490 2023-06-23 18:50:51.000000 pix2vec-0.1.3/docs/images/m3cube-c.png
--rw-r--r--   0 alf        (501) staff       (20)      552 2023-06-23 21:34:41.000000 pix2vec-0.1.3/docs/index.rst
--rw-r--r--   0 alf        (501) staff       (20)     1114 2023-06-22 08:51:18.000000 pix2vec-0.1.3/docs/installation.rst
--rw-r--r--   0 alf        (501) staff       (20)      805 2023-06-21 09:12:34.000000 pix2vec-0.1.3/docs/make.bat
--rw-r--r--   0 alf        (501) staff       (20)       58 2023-06-23 20:25:10.000000 pix2vec-0.1.3/docs/modules.rst
--rw-r--r--   0 alf        (501) staff       (20)      423 2023-06-23 20:25:10.000000 pix2vec-0.1.3/docs/pix2vec.rst
--rw-r--r--   0 alf        (501) staff       (20)       27 2023-06-21 09:12:34.000000 pix2vec-0.1.3/docs/readme.rst
--rw-r--r--   0 alf        (501) staff       (20)      181 2023-06-21 14:04:55.000000 pix2vec-0.1.3/docs/usage.rst
-drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-07-09 06:04:32.051509 pix2vec-0.1.3/pix2vec/
--rw-r--r--   0 alf        (501) staff       (20)      404 2023-06-26 16:37:14.000000 pix2vec-0.1.3/pix2vec/__init__.py
--rw-r--r--   0 alf        (501) staff       (20)     2086 2023-06-26 16:37:03.000000 pix2vec-0.1.3/pix2vec/cli.py
--rw-r--r--   0 alf        (501) staff       (20)     8802 2023-06-23 21:01:11.000000 pix2vec-0.1.3/pix2vec/pix2vec.py
-drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-07-09 06:04:32.054669 pix2vec-0.1.3/pix2vec.egg-info/
--rw-r--r--   0 alf        (501) staff       (20)     5430 2023-07-09 06:04:31.000000 pix2vec-0.1.3/pix2vec.egg-info/PKG-INFO
--rw-r--r--   0 alf        (501) staff       (20)      928 2023-07-09 06:04:31.000000 pix2vec-0.1.3/pix2vec.egg-info/SOURCES.txt
--rw-r--r--   0 alf        (501) staff       (20)        1 2023-07-09 06:04:31.000000 pix2vec-0.1.3/pix2vec.egg-info/dependency_links.txt
--rw-r--r--   0 alf        (501) staff       (20)       45 2023-07-09 06:04:31.000000 pix2vec-0.1.3/pix2vec.egg-info/entry_points.txt
--rw-r--r--   0 alf        (501) staff       (20)        1 2023-06-21 09:26:55.000000 pix2vec-0.1.3/pix2vec.egg-info/not-zip-safe
--rw-r--r--   0 alf        (501) staff       (20)        8 2023-07-09 06:04:31.000000 pix2vec-0.1.3/pix2vec.egg-info/top_level.txt
--rw-r--r--   0 alf        (501) staff       (20)       32 2023-06-23 19:30:18.000000 pix2vec-0.1.3/requirements.txt
--rw-r--r--   0 alf        (501) staff       (20)      185 2023-06-23 19:30:11.000000 pix2vec-0.1.3/requirements_dev.txt
--rw-r--r--   0 alf        (501) staff       (20)      379 2023-07-09 06:04:32.057340 pix2vec-0.1.3/setup.cfg
--rw-r--r--   0 alf        (501) staff       (20)     1625 2023-07-09 05:51:07.000000 pix2vec-0.1.3/setup.py
-drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-07-09 06:04:32.055622 pix2vec-0.1.3/tests/
--rw-r--r--   0 alf        (501) staff       (20)       37 2023-06-21 09:12:34.000000 pix2vec-0.1.3/tests/__init__.py
--rw-r--r--   0 alf        (501) staff       (20)      387 2023-06-21 09:12:34.000000 pix2vec-0.1.3/tests/test_pix2vec.py
--rw-r--r--   0 alf        (501) staff       (20)      268 2023-06-21 09:12:34.000000 pix2vec-0.1.3/tox.ini
+drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-08-01 16:52:44.177693 pix2vec-0.1.4/
+-rw-r--r--   0 alf        (501) staff       (20)     1204 2023-06-21 09:12:34.000000 pix2vec-0.1.4/.gitignore
+-rw-r--r--   0 alf        (501) staff       (20)      205 2023-06-21 10:32:57.000000 pix2vec-0.1.4/.readthedocs.yaml
+-rw-r--r--   0 alf        (501) staff       (20)      593 2023-07-09 06:02:38.000000 pix2vec-0.1.4/.zenodo.json
+-rw-r--r--   0 alf        (501) staff       (20)      278 2023-07-31 08:29:22.000000 pix2vec-0.1.4/AUTHORS.rst
+-rw-r--r--   0 alf        (501) staff       (20)      284 2023-07-07 14:13:32.000000 pix2vec-0.1.4/CITATION.cff
+-rw-r--r--   0 alf        (501) staff       (20)     3524 2023-06-22 08:52:00.000000 pix2vec-0.1.4/CONTRIBUTING.rst
+-rw-r--r--   0 alf        (501) staff       (20)      429 2023-07-09 06:04:28.000000 pix2vec-0.1.4/HISTORY.rst
+-rw-r--r--   0 alf        (501) staff       (20)     1564 2023-06-21 09:12:34.000000 pix2vec-0.1.4/LICENSE
+-rw-r--r--   0 alf        (501) staff       (20)      262 2023-06-21 09:12:34.000000 pix2vec-0.1.4/MANIFEST.in
+-rw-r--r--   0 alf        (501) staff       (20)     2295 2023-06-21 09:12:34.000000 pix2vec-0.1.4/Makefile
+-rw-r--r--   0 alf        (501) staff       (20)     5431 2023-08-01 16:52:44.177964 pix2vec-0.1.4/PKG-INFO
+-rw-r--r--   0 alf        (501) staff       (20)     4035 2023-07-09 06:18:16.000000 pix2vec-0.1.4/README.rst
+drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-08-01 16:52:44.119823 pix2vec-0.1.4/docs/
+-rw-r--r--   0 alf        (501) staff       (20)      608 2023-06-21 09:12:34.000000 pix2vec-0.1.4/docs/Makefile
+drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-08-01 16:52:44.100459 pix2vec-0.1.4/docs/_build/
+drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-08-01 16:52:44.100866 pix2vec-0.1.4/docs/_build/html/
+drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-08-01 16:52:44.120386 pix2vec-0.1.4/docs/_build/html/_images/
+-rw-r--r--   0 alf        (501) staff       (20)   530877 2023-06-21 13:49:17.000000 pix2vec-0.1.4/docs/_build/html/_images/m3cube-a.png
+drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-08-01 16:52:44.125416 pix2vec-0.1.4/docs/_build/html/_static/
+-rw-r--r--   0 alf        (501) staff       (20)      286 2021-10-12 12:18:02.000000 pix2vec-0.1.4/docs/_build/html/_static/file.png
+-rw-r--r--   0 alf        (501) staff       (20)       90 2021-10-12 12:18:02.000000 pix2vec-0.1.4/docs/_build/html/_static/minus.png
+-rw-r--r--   0 alf        (501) staff       (20)       90 2021-10-12 12:18:02.000000 pix2vec-0.1.4/docs/_build/html/_static/plus.png
+-rw-r--r--   0 alf        (501) staff       (20)       28 2023-06-21 09:12:34.000000 pix2vec-0.1.4/docs/authors.rst
+-rwxr-xr-x   0 alf        (501) staff       (20)     4876 2023-06-21 10:42:06.000000 pix2vec-0.1.4/docs/conf.py
+-rw-r--r--   0 alf        (501) staff       (20)       33 2023-06-21 09:12:34.000000 pix2vec-0.1.4/docs/contributing.rst
+-rw-r--r--   0 alf        (501) staff       (20)       28 2023-06-21 09:12:34.000000 pix2vec-0.1.4/docs/history.rst
+drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-08-01 16:52:44.143835 pix2vec-0.1.4/docs/images/
+-rw-r--r--   0 alf        (501) staff       (20)   339139 2023-06-23 23:06:07.000000 pix2vec-0.1.4/docs/images/m3-PixelValue.png
+-rw-r--r--   0 alf        (501) staff       (20)   337959 2023-06-23 23:06:07.000000 pix2vec-0.1.4/docs/images/m3-detail.png
+-rw-r--r--   0 alf        (501) staff       (20)   530877 2023-06-21 13:49:17.000000 pix2vec-0.1.4/docs/images/m3cube-a.png
+-rw-r--r--   0 alf        (501) staff       (20)   948490 2023-06-23 18:50:51.000000 pix2vec-0.1.4/docs/images/m3cube-c.png
+-rw-r--r--   0 alf        (501) staff       (20)      552 2023-06-23 21:34:41.000000 pix2vec-0.1.4/docs/index.rst
+-rw-r--r--   0 alf        (501) staff       (20)     1114 2023-06-22 08:51:18.000000 pix2vec-0.1.4/docs/installation.rst
+-rw-r--r--   0 alf        (501) staff       (20)      805 2023-06-21 09:12:34.000000 pix2vec-0.1.4/docs/make.bat
+-rw-r--r--   0 alf        (501) staff       (20)       58 2023-06-23 20:25:10.000000 pix2vec-0.1.4/docs/modules.rst
+-rw-r--r--   0 alf        (501) staff       (20)      423 2023-06-23 20:25:10.000000 pix2vec-0.1.4/docs/pix2vec.rst
+-rw-r--r--   0 alf        (501) staff       (20)       27 2023-06-21 09:12:34.000000 pix2vec-0.1.4/docs/readme.rst
+-rw-r--r--   0 alf        (501) staff       (20)      181 2023-06-21 14:04:55.000000 pix2vec-0.1.4/docs/usage.rst
+drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-08-01 16:52:44.156826 pix2vec-0.1.4/pix2vec/
+-rw-r--r--   0 alf        (501) staff       (20)      202 2023-07-31 08:28:18.000000 pix2vec-0.1.4/pix2vec/__init__.py
+-rw-r--r--   0 alf        (501) staff       (20)     2086 2023-06-26 16:37:03.000000 pix2vec-0.1.4/pix2vec/cli.py
+-rw-r--r--   0 alf        (501) staff       (20)     8802 2023-06-23 21:01:11.000000 pix2vec-0.1.4/pix2vec/pix2vec.py
+drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-08-01 16:52:44.159759 pix2vec-0.1.4/pix2vec.egg-info/
+-rw-r--r--   0 alf        (501) staff       (20)     5431 2023-08-01 16:52:43.000000 pix2vec-0.1.4/pix2vec.egg-info/PKG-INFO
+-rw-r--r--   0 alf        (501) staff       (20)      950 2023-08-01 16:52:44.000000 pix2vec-0.1.4/pix2vec.egg-info/SOURCES.txt
+-rw-r--r--   0 alf        (501) staff       (20)        1 2023-08-01 16:52:43.000000 pix2vec-0.1.4/pix2vec.egg-info/dependency_links.txt
+-rw-r--r--   0 alf        (501) staff       (20)       45 2023-08-01 16:52:43.000000 pix2vec-0.1.4/pix2vec.egg-info/entry_points.txt
+-rw-r--r--   0 alf        (501) staff       (20)        1 2023-06-21 09:26:55.000000 pix2vec-0.1.4/pix2vec.egg-info/not-zip-safe
+-rw-r--r--   0 alf        (501) staff       (20)        8 2023-08-01 16:52:43.000000 pix2vec-0.1.4/pix2vec.egg-info/top_level.txt
+-rw-r--r--   0 alf        (501) staff       (20)       32 2023-06-23 19:30:18.000000 pix2vec-0.1.4/requirements.txt
+-rw-r--r--   0 alf        (501) staff       (20)      185 2023-06-23 19:30:11.000000 pix2vec-0.1.4/requirements_dev.txt
+-rw-r--r--   0 alf        (501) staff       (20)      379 2023-08-01 16:52:44.178970 pix2vec-0.1.4/setup.cfg
+-rw-r--r--   0 alf        (501) staff       (20)     1625 2023-07-31 08:30:01.000000 pix2vec-0.1.4/setup.py
+drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-08-01 16:52:44.160791 pix2vec-0.1.4/tests/
+-rw-r--r--   0 alf        (501) staff       (20)       37 2023-06-21 09:12:34.000000 pix2vec-0.1.4/tests/__init__.py
+drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-08-01 16:52:44.161490 pix2vec-0.1.4/tests/files/
+-rwxr-xr-x   0 alf        (501) staff       (20)  1188930 2023-07-31 08:22:19.000000 pix2vec-0.1.4/tests/files/crism.cub
+-rw-r--r--   0 alf        (501) staff       (20)      387 2023-06-21 09:12:34.000000 pix2vec-0.1.4/tests/test_pix2vec.py
+-rw-r--r--   0 alf        (501) staff       (20)      268 2023-06-21 09:12:34.000000 pix2vec-0.1.4/tox.ini
```

### Comparing `pix2vec-0.1.3/.gitignore` & `pix2vec-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `pix2vec-0.1.3/.zenodo.json` & `pix2vec-0.1.4/.zenodo.json`

 * *Files identical despite different names*

### Comparing `pix2vec-0.1.3/CONTRIBUTING.rst` & `pix2vec-0.1.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pix2vec-0.1.3/LICENSE` & `pix2vec-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pix2vec-0.1.3/Makefile` & `pix2vec-0.1.4/Makefile`

 * *Files identical despite different names*

### Comparing `pix2vec-0.1.3/PKG-INFO` & `pix2vec-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pix2vec
-Version: 0.1.3
+Version: 0.1.4
 Summary: pix2vec produces a vector representation of planetary mapping spectrometers hyperspectral and camera ISIS data cube
 Home-page: https://github.com/afrigeri/pix2vec
 Author: Alessandro Frigeri
 Author-email: alessandro.frigeri@inaf.it
 License: GNU General Public License v3
 Keywords: pix2vec
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -33,14 +33,15 @@
 .. image:: https://img.shields.io/pypi/v/pix2vec.svg
         :target: https://pypi.python.org/pypi/pix2vec
 
 .. image:: https://readthedocs.org/projects/pix2vec/badge/?version=latest
         :target: https://pix2vec.readthedocs.io/en/latest/?version=latest
         :alt: Documentation Status
 
+
 pix2vec: Vector Representation of Planetary Hyperspectral Data Cubes
 
 
 * Free software: GNU General Public License v3
 * Documentation: https://pix2vec.readthedocs.io.
```

### Comparing `pix2vec-0.1.3/README.rst` & `pix2vec-0.1.4/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 .. image:: https://img.shields.io/pypi/v/pix2vec.svg
         :target: https://pypi.python.org/pypi/pix2vec
 
 .. image:: https://readthedocs.org/projects/pix2vec/badge/?version=latest
         :target: https://pix2vec.readthedocs.io/en/latest/?version=latest
         :alt: Documentation Status
 
+
 pix2vec: Vector Representation of Planetary Hyperspectral Data Cubes
 
 
 * Free software: GNU General Public License v3
 * Documentation: https://pix2vec.readthedocs.io.
```

### Comparing `pix2vec-0.1.3/docs/Makefile` & `pix2vec-0.1.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pix2vec-0.1.3/docs/_build/html/_images/m3cube-a.png` & `pix2vec-0.1.4/docs/_build/html/_images/m3cube-a.png`

 * *Files identical despite different names*

### Comparing `pix2vec-0.1.3/docs/conf.py` & `pix2vec-0.1.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pix2vec-0.1.3/docs/images/m3-PixelValue.png` & `pix2vec-0.1.4/docs/images/m3-PixelValue.png`

 * *Files identical despite different names*

### Comparing `pix2vec-0.1.3/docs/images/m3-detail.png` & `pix2vec-0.1.4/docs/images/m3-detail.png`

 * *Files identical despite different names*

### Comparing `pix2vec-0.1.3/docs/images/m3cube-a.png` & `pix2vec-0.1.4/docs/images/m3cube-a.png`

 * *Files identical despite different names*

### Comparing `pix2vec-0.1.3/docs/images/m3cube-c.png` & `pix2vec-0.1.4/docs/images/m3cube-c.png`

 * *Files identical despite different names*

### Comparing `pix2vec-0.1.3/docs/index.rst` & `pix2vec-0.1.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pix2vec-0.1.3/docs/installation.rst` & `pix2vec-0.1.4/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `pix2vec-0.1.3/docs/make.bat` & `pix2vec-0.1.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pix2vec-0.1.3/pix2vec/cli.py` & `pix2vec-0.1.4/pix2vec/cli.py`

 * *Files identical despite different names*

### Comparing `pix2vec-0.1.3/pix2vec/pix2vec.py` & `pix2vec-0.1.4/pix2vec/pix2vec.py`

 * *Files identical despite different names*

### Comparing `pix2vec-0.1.3/pix2vec.egg-info/PKG-INFO` & `pix2vec-0.1.4/pix2vec.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pix2vec
-Version: 0.1.3
+Version: 0.1.4
 Summary: pix2vec produces a vector representation of planetary mapping spectrometers hyperspectral and camera ISIS data cube
 Home-page: https://github.com/afrigeri/pix2vec
 Author: Alessandro Frigeri
 Author-email: alessandro.frigeri@inaf.it
 License: GNU General Public License v3
 Keywords: pix2vec
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -33,14 +33,15 @@
 .. image:: https://img.shields.io/pypi/v/pix2vec.svg
         :target: https://pypi.python.org/pypi/pix2vec
 
 .. image:: https://readthedocs.org/projects/pix2vec/badge/?version=latest
         :target: https://pix2vec.readthedocs.io/en/latest/?version=latest
         :alt: Documentation Status
 
+
 pix2vec: Vector Representation of Planetary Hyperspectral Data Cubes
 
 
 * Free software: GNU General Public License v3
 * Documentation: https://pix2vec.readthedocs.io.
```

### Comparing `pix2vec-0.1.3/pix2vec.egg-info/SOURCES.txt` & `pix2vec-0.1.4/pix2vec.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -40,8 +40,9 @@
 pix2vec.egg-info/PKG-INFO
 pix2vec.egg-info/SOURCES.txt
 pix2vec.egg-info/dependency_links.txt
 pix2vec.egg-info/entry_points.txt
 pix2vec.egg-info/not-zip-safe
 pix2vec.egg-info/top_level.txt
 tests/__init__.py
-tests/test_pix2vec.py
+tests/test_pix2vec.py
+tests/files/crism.cub
```

### Comparing `pix2vec-0.1.3/setup.py` & `pix2vec-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,10 +43,10 @@
     include_package_data=True,
     keywords='pix2vec',
     name='pix2vec',
     packages=find_packages(include=['pix2vec', 'pix2vec.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/afrigeri/pix2vec',
-    version='0.1.3',
+    version='0.1.4',
     zip_safe=False,
 )
```

