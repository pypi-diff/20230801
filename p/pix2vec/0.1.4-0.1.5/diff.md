# Comparing `tmp/pix2vec-0.1.4.tar.gz` & `tmp/pix2vec-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pix2vec-0.1.4.tar", last modified: Tue Aug  1 16:52:44 2023, max compression
+gzip compressed data, was "pix2vec-0.1.5.tar", last modified: Tue Aug  1 17:02:06 2023, max compression
```

## Comparing `pix2vec-0.1.4.tar` & `pix2vec-0.1.5.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-08-01 16:52:44.177693 pix2vec-0.1.4/
--rw-r--r--   0 alf        (501) staff       (20)     1204 2023-06-21 09:12:34.000000 pix2vec-0.1.4/.gitignore
--rw-r--r--   0 alf        (501) staff       (20)      205 2023-06-21 10:32:57.000000 pix2vec-0.1.4/.readthedocs.yaml
--rw-r--r--   0 alf        (501) staff       (20)      593 2023-07-09 06:02:38.000000 pix2vec-0.1.4/.zenodo.json
--rw-r--r--   0 alf        (501) staff       (20)      278 2023-07-31 08:29:22.000000 pix2vec-0.1.4/AUTHORS.rst
--rw-r--r--   0 alf        (501) staff       (20)      284 2023-07-07 14:13:32.000000 pix2vec-0.1.4/CITATION.cff
--rw-r--r--   0 alf        (501) staff       (20)     3524 2023-06-22 08:52:00.000000 pix2vec-0.1.4/CONTRIBUTING.rst
--rw-r--r--   0 alf        (501) staff       (20)      429 2023-07-09 06:04:28.000000 pix2vec-0.1.4/HISTORY.rst
--rw-r--r--   0 alf        (501) staff       (20)     1564 2023-06-21 09:12:34.000000 pix2vec-0.1.4/LICENSE
--rw-r--r--   0 alf        (501) staff       (20)      262 2023-06-21 09:12:34.000000 pix2vec-0.1.4/MANIFEST.in
--rw-r--r--   0 alf        (501) staff       (20)     2295 2023-06-21 09:12:34.000000 pix2vec-0.1.4/Makefile
--rw-r--r--   0 alf        (501) staff       (20)     5431 2023-08-01 16:52:44.177964 pix2vec-0.1.4/PKG-INFO
--rw-r--r--   0 alf        (501) staff       (20)     4035 2023-07-09 06:18:16.000000 pix2vec-0.1.4/README.rst
-drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-08-01 16:52:44.119823 pix2vec-0.1.4/docs/
--rw-r--r--   0 alf        (501) staff       (20)      608 2023-06-21 09:12:34.000000 pix2vec-0.1.4/docs/Makefile
-drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-08-01 16:52:44.100459 pix2vec-0.1.4/docs/_build/
-drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-08-01 16:52:44.100866 pix2vec-0.1.4/docs/_build/html/
-drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-08-01 16:52:44.120386 pix2vec-0.1.4/docs/_build/html/_images/
--rw-r--r--   0 alf        (501) staff       (20)   530877 2023-06-21 13:49:17.000000 pix2vec-0.1.4/docs/_build/html/_images/m3cube-a.png
-drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-08-01 16:52:44.125416 pix2vec-0.1.4/docs/_build/html/_static/
--rw-r--r--   0 alf        (501) staff       (20)      286 2021-10-12 12:18:02.000000 pix2vec-0.1.4/docs/_build/html/_static/file.png
--rw-r--r--   0 alf        (501) staff       (20)       90 2021-10-12 12:18:02.000000 pix2vec-0.1.4/docs/_build/html/_static/minus.png
--rw-r--r--   0 alf        (501) staff       (20)       90 2021-10-12 12:18:02.000000 pix2vec-0.1.4/docs/_build/html/_static/plus.png
--rw-r--r--   0 alf        (501) staff       (20)       28 2023-06-21 09:12:34.000000 pix2vec-0.1.4/docs/authors.rst
--rwxr-xr-x   0 alf        (501) staff       (20)     4876 2023-06-21 10:42:06.000000 pix2vec-0.1.4/docs/conf.py
--rw-r--r--   0 alf        (501) staff       (20)       33 2023-06-21 09:12:34.000000 pix2vec-0.1.4/docs/contributing.rst
--rw-r--r--   0 alf        (501) staff       (20)       28 2023-06-21 09:12:34.000000 pix2vec-0.1.4/docs/history.rst
-drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-08-01 16:52:44.143835 pix2vec-0.1.4/docs/images/
--rw-r--r--   0 alf        (501) staff       (20)   339139 2023-06-23 23:06:07.000000 pix2vec-0.1.4/docs/images/m3-PixelValue.png
--rw-r--r--   0 alf        (501) staff       (20)   337959 2023-06-23 23:06:07.000000 pix2vec-0.1.4/docs/images/m3-detail.png
--rw-r--r--   0 alf        (501) staff       (20)   530877 2023-06-21 13:49:17.000000 pix2vec-0.1.4/docs/images/m3cube-a.png
--rw-r--r--   0 alf        (501) staff       (20)   948490 2023-06-23 18:50:51.000000 pix2vec-0.1.4/docs/images/m3cube-c.png
--rw-r--r--   0 alf        (501) staff       (20)      552 2023-06-23 21:34:41.000000 pix2vec-0.1.4/docs/index.rst
--rw-r--r--   0 alf        (501) staff       (20)     1114 2023-06-22 08:51:18.000000 pix2vec-0.1.4/docs/installation.rst
--rw-r--r--   0 alf        (501) staff       (20)      805 2023-06-21 09:12:34.000000 pix2vec-0.1.4/docs/make.bat
--rw-r--r--   0 alf        (501) staff       (20)       58 2023-06-23 20:25:10.000000 pix2vec-0.1.4/docs/modules.rst
--rw-r--r--   0 alf        (501) staff       (20)      423 2023-06-23 20:25:10.000000 pix2vec-0.1.4/docs/pix2vec.rst
--rw-r--r--   0 alf        (501) staff       (20)       27 2023-06-21 09:12:34.000000 pix2vec-0.1.4/docs/readme.rst
--rw-r--r--   0 alf        (501) staff       (20)      181 2023-06-21 14:04:55.000000 pix2vec-0.1.4/docs/usage.rst
-drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-08-01 16:52:44.156826 pix2vec-0.1.4/pix2vec/
--rw-r--r--   0 alf        (501) staff       (20)      202 2023-07-31 08:28:18.000000 pix2vec-0.1.4/pix2vec/__init__.py
--rw-r--r--   0 alf        (501) staff       (20)     2086 2023-06-26 16:37:03.000000 pix2vec-0.1.4/pix2vec/cli.py
--rw-r--r--   0 alf        (501) staff       (20)     8802 2023-06-23 21:01:11.000000 pix2vec-0.1.4/pix2vec/pix2vec.py
-drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-08-01 16:52:44.159759 pix2vec-0.1.4/pix2vec.egg-info/
--rw-r--r--   0 alf        (501) staff       (20)     5431 2023-08-01 16:52:43.000000 pix2vec-0.1.4/pix2vec.egg-info/PKG-INFO
--rw-r--r--   0 alf        (501) staff       (20)      950 2023-08-01 16:52:44.000000 pix2vec-0.1.4/pix2vec.egg-info/SOURCES.txt
--rw-r--r--   0 alf        (501) staff       (20)        1 2023-08-01 16:52:43.000000 pix2vec-0.1.4/pix2vec.egg-info/dependency_links.txt
--rw-r--r--   0 alf        (501) staff       (20)       45 2023-08-01 16:52:43.000000 pix2vec-0.1.4/pix2vec.egg-info/entry_points.txt
--rw-r--r--   0 alf        (501) staff       (20)        1 2023-06-21 09:26:55.000000 pix2vec-0.1.4/pix2vec.egg-info/not-zip-safe
--rw-r--r--   0 alf        (501) staff       (20)        8 2023-08-01 16:52:43.000000 pix2vec-0.1.4/pix2vec.egg-info/top_level.txt
--rw-r--r--   0 alf        (501) staff       (20)       32 2023-06-23 19:30:18.000000 pix2vec-0.1.4/requirements.txt
--rw-r--r--   0 alf        (501) staff       (20)      185 2023-06-23 19:30:11.000000 pix2vec-0.1.4/requirements_dev.txt
--rw-r--r--   0 alf        (501) staff       (20)      379 2023-08-01 16:52:44.178970 pix2vec-0.1.4/setup.cfg
--rw-r--r--   0 alf        (501) staff       (20)     1625 2023-07-31 08:30:01.000000 pix2vec-0.1.4/setup.py
-drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-08-01 16:52:44.160791 pix2vec-0.1.4/tests/
--rw-r--r--   0 alf        (501) staff       (20)       37 2023-06-21 09:12:34.000000 pix2vec-0.1.4/tests/__init__.py
-drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-08-01 16:52:44.161490 pix2vec-0.1.4/tests/files/
--rwxr-xr-x   0 alf        (501) staff       (20)  1188930 2023-07-31 08:22:19.000000 pix2vec-0.1.4/tests/files/crism.cub
--rw-r--r--   0 alf        (501) staff       (20)      387 2023-06-21 09:12:34.000000 pix2vec-0.1.4/tests/test_pix2vec.py
--rw-r--r--   0 alf        (501) staff       (20)      268 2023-06-21 09:12:34.000000 pix2vec-0.1.4/tox.ini
+drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-08-01 17:02:06.547780 pix2vec-0.1.5/
+-rw-r--r--   0 alf        (501) staff       (20)     1204 2023-06-21 09:12:34.000000 pix2vec-0.1.5/.gitignore
+-rw-r--r--   0 alf        (501) staff       (20)      205 2023-06-21 10:32:57.000000 pix2vec-0.1.5/.readthedocs.yaml
+-rw-r--r--   0 alf        (501) staff       (20)      592 2023-08-01 17:00:04.000000 pix2vec-0.1.5/.zenodo.json
+-rw-r--r--   0 alf        (501) staff       (20)      278 2023-07-31 08:29:22.000000 pix2vec-0.1.5/AUTHORS.rst
+-rw-r--r--   0 alf        (501) staff       (20)      284 2023-07-07 14:13:32.000000 pix2vec-0.1.5/CITATION.cff
+-rw-r--r--   0 alf        (501) staff       (20)     3524 2023-06-22 08:52:00.000000 pix2vec-0.1.5/CONTRIBUTING.rst
+-rw-r--r--   0 alf        (501) staff       (20)      429 2023-07-09 06:04:28.000000 pix2vec-0.1.5/HISTORY.rst
+-rw-r--r--   0 alf        (501) staff       (20)     1564 2023-06-21 09:12:34.000000 pix2vec-0.1.5/LICENSE
+-rw-r--r--   0 alf        (501) staff       (20)      262 2023-06-21 09:12:34.000000 pix2vec-0.1.5/MANIFEST.in
+-rw-r--r--   0 alf        (501) staff       (20)     2295 2023-06-21 09:12:34.000000 pix2vec-0.1.5/Makefile
+-rw-r--r--   0 alf        (501) staff       (20)     5431 2023-08-01 17:02:06.548027 pix2vec-0.1.5/PKG-INFO
+-rw-r--r--   0 alf        (501) staff       (20)     4035 2023-07-09 06:18:16.000000 pix2vec-0.1.5/README.rst
+drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-08-01 17:02:06.493477 pix2vec-0.1.5/docs/
+-rw-r--r--   0 alf        (501) staff       (20)      608 2023-06-21 09:12:34.000000 pix2vec-0.1.5/docs/Makefile
+drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-08-01 17:02:06.474740 pix2vec-0.1.5/docs/_build/
+drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-08-01 17:02:06.475030 pix2vec-0.1.5/docs/_build/html/
+drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-08-01 17:02:06.494132 pix2vec-0.1.5/docs/_build/html/_images/
+-rw-r--r--   0 alf        (501) staff       (20)   530877 2023-06-21 13:49:17.000000 pix2vec-0.1.5/docs/_build/html/_images/m3cube-a.png
+drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-08-01 17:02:06.501120 pix2vec-0.1.5/docs/_build/html/_static/
+-rw-r--r--   0 alf        (501) staff       (20)      286 2021-10-12 12:18:02.000000 pix2vec-0.1.5/docs/_build/html/_static/file.png
+-rw-r--r--   0 alf        (501) staff       (20)       90 2021-10-12 12:18:02.000000 pix2vec-0.1.5/docs/_build/html/_static/minus.png
+-rw-r--r--   0 alf        (501) staff       (20)       90 2021-10-12 12:18:02.000000 pix2vec-0.1.5/docs/_build/html/_static/plus.png
+-rw-r--r--   0 alf        (501) staff       (20)       28 2023-06-21 09:12:34.000000 pix2vec-0.1.5/docs/authors.rst
+-rwxr-xr-x   0 alf        (501) staff       (20)     4876 2023-06-21 10:42:06.000000 pix2vec-0.1.5/docs/conf.py
+-rw-r--r--   0 alf        (501) staff       (20)       33 2023-06-21 09:12:34.000000 pix2vec-0.1.5/docs/contributing.rst
+-rw-r--r--   0 alf        (501) staff       (20)       28 2023-06-21 09:12:34.000000 pix2vec-0.1.5/docs/history.rst
+drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-08-01 17:02:06.519871 pix2vec-0.1.5/docs/images/
+-rw-r--r--   0 alf        (501) staff       (20)   339139 2023-06-23 23:06:07.000000 pix2vec-0.1.5/docs/images/m3-PixelValue.png
+-rw-r--r--   0 alf        (501) staff       (20)   337959 2023-06-23 23:06:07.000000 pix2vec-0.1.5/docs/images/m3-detail.png
+-rw-r--r--   0 alf        (501) staff       (20)   530877 2023-06-21 13:49:17.000000 pix2vec-0.1.5/docs/images/m3cube-a.png
+-rw-r--r--   0 alf        (501) staff       (20)   948490 2023-06-23 18:50:51.000000 pix2vec-0.1.5/docs/images/m3cube-c.png
+-rw-r--r--   0 alf        (501) staff       (20)      552 2023-06-23 21:34:41.000000 pix2vec-0.1.5/docs/index.rst
+-rw-r--r--   0 alf        (501) staff       (20)     1114 2023-06-22 08:51:18.000000 pix2vec-0.1.5/docs/installation.rst
+-rw-r--r--   0 alf        (501) staff       (20)      805 2023-06-21 09:12:34.000000 pix2vec-0.1.5/docs/make.bat
+-rw-r--r--   0 alf        (501) staff       (20)       58 2023-06-23 20:25:10.000000 pix2vec-0.1.5/docs/modules.rst
+-rw-r--r--   0 alf        (501) staff       (20)      423 2023-06-23 20:25:10.000000 pix2vec-0.1.5/docs/pix2vec.rst
+-rw-r--r--   0 alf        (501) staff       (20)       27 2023-06-21 09:12:34.000000 pix2vec-0.1.5/docs/readme.rst
+-rw-r--r--   0 alf        (501) staff       (20)      181 2023-06-21 14:04:55.000000 pix2vec-0.1.5/docs/usage.rst
+drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-08-01 17:02:06.534746 pix2vec-0.1.5/pix2vec/
+-rw-r--r--   0 alf        (501) staff       (20)      202 2023-08-01 17:01:27.000000 pix2vec-0.1.5/pix2vec/__init__.py
+-rw-r--r--   0 alf        (501) staff       (20)     2086 2023-06-26 16:37:03.000000 pix2vec-0.1.5/pix2vec/cli.py
+-rw-r--r--   0 alf        (501) staff       (20)     8802 2023-06-23 21:01:11.000000 pix2vec-0.1.5/pix2vec/pix2vec.py
+drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-08-01 17:02:06.537687 pix2vec-0.1.5/pix2vec.egg-info/
+-rw-r--r--   0 alf        (501) staff       (20)     5431 2023-08-01 17:02:06.000000 pix2vec-0.1.5/pix2vec.egg-info/PKG-INFO
+-rw-r--r--   0 alf        (501) staff       (20)      950 2023-08-01 17:02:06.000000 pix2vec-0.1.5/pix2vec.egg-info/SOURCES.txt
+-rw-r--r--   0 alf        (501) staff       (20)        1 2023-08-01 17:02:06.000000 pix2vec-0.1.5/pix2vec.egg-info/dependency_links.txt
+-rw-r--r--   0 alf        (501) staff       (20)       45 2023-08-01 17:02:06.000000 pix2vec-0.1.5/pix2vec.egg-info/entry_points.txt
+-rw-r--r--   0 alf        (501) staff       (20)        1 2023-06-21 09:26:55.000000 pix2vec-0.1.5/pix2vec.egg-info/not-zip-safe
+-rw-r--r--   0 alf        (501) staff       (20)        8 2023-08-01 17:02:06.000000 pix2vec-0.1.5/pix2vec.egg-info/top_level.txt
+-rw-r--r--   0 alf        (501) staff       (20)       32 2023-06-23 19:30:18.000000 pix2vec-0.1.5/requirements.txt
+-rw-r--r--   0 alf        (501) staff       (20)      185 2023-06-23 19:30:11.000000 pix2vec-0.1.5/requirements_dev.txt
+-rw-r--r--   0 alf        (501) staff       (20)      379 2023-08-01 17:02:06.548849 pix2vec-0.1.5/setup.cfg
+-rw-r--r--   0 alf        (501) staff       (20)     1625 2023-08-01 17:01:12.000000 pix2vec-0.1.5/setup.py
+drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-08-01 17:02:06.538947 pix2vec-0.1.5/tests/
+-rw-r--r--   0 alf        (501) staff       (20)       37 2023-06-21 09:12:34.000000 pix2vec-0.1.5/tests/__init__.py
+drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-08-01 17:02:06.539604 pix2vec-0.1.5/tests/files/
+-rwxr-xr-x   0 alf        (501) staff       (20)  1188930 2023-07-31 08:22:19.000000 pix2vec-0.1.5/tests/files/crism.cub
+-rw-r--r--   0 alf        (501) staff       (20)      387 2023-06-21 09:12:34.000000 pix2vec-0.1.5/tests/test_pix2vec.py
+-rw-r--r--   0 alf        (501) staff       (20)      268 2023-06-21 09:12:34.000000 pix2vec-0.1.5/tox.ini
```

### Comparing `pix2vec-0.1.4/.gitignore` & `pix2vec-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `pix2vec-0.1.4/.zenodo.json` & `pix2vec-0.1.5/.zenodo.json`

 * *Files 1% similar despite different names*

```diff
@@ -17,22 +17,21 @@
 00000100: 6f6c 6f67 6963 616c 2053 7572 7665 792c  ological Survey,
 00000110: 2041 7374 726f 6765 6f6c 6f67 7920 5363   Astrogeology Sc
 00000120: 6965 6e63 6520 4365 6e74 6572 222c 0a20  ience Center",. 
 00000130: 2020 2020 2022 6e61 6d65 223a 2022 4861       "name": "Ha
 00000140: 7265 2c20 5472 656e 7422 2c0a 2020 2020  re, Trent",.    
 00000150: 2020 226f 7263 6964 223a 2022 3030 3030    "orcid": "0000
 00000160: 2d30 3030 312d 3838 3432 2d33 3839 5822  -0001-8842-389X"
-00000170: 0a20 2020 207d 2c0a 2020 5d2c 0a20 2022  .    },.  ],.  "
-00000180: 7469 746c 6522 3a20 2270 6978 3276 6563  title": "pix2vec
-00000190: 7422 2c0a 2020 2264 6573 6372 6970 7469  t",.  "descripti
-000001a0: 6f6e 223a 2022 4120 736f 6674 7761 7265  on": "A software
-000001b0: 2074 6f6f 6c20 746f 2067 656e 6572 6174   tool to generat
-000001c0: 6520 6765 6f73 7061 7469 616c 2076 6563  e geospatial vec
-000001d0: 746f 7220 7265 7072 6573 656e 7461 7469  tor representati
-000001e0: 6f6e 206f 6620 706c 616e 6574 6172 7920  on of planetary 
-000001f0: 7370 6563 7472 6f6d 6574 6572 732e 222c  spectrometers.",
-00000200: 0a20 2022 6c69 6365 6e73 6522 3a20 2267  .  "license": "g
-00000210: 706c 222c 0a20 2022 6163 6365 7373 5f72  pl",.  "access_r
-00000220: 6967 6874 223a 2022 6f70 656e 222c 0a20  ight": "open",. 
-00000230: 2022 7570 6c6f 6164 5f74 7970 6522 3a20   "upload_type": 
-00000240: 2273 6f66 7477 6172 6522 2020 2020 0a7d  "software"    .}
-00000250: 0a                                       .
+00000170: 0a20 2020 207d 0a20 205d 2c0a 2020 2274  .    }.  ],.  "t
+00000180: 6974 6c65 223a 2022 7069 7832 7665 6374  itle": "pix2vect
+00000190: 222c 0a20 2022 6465 7363 7269 7074 696f  ",.  "descriptio
+000001a0: 6e22 3a20 2241 2073 6f66 7477 6172 6520  n": "A software 
+000001b0: 746f 6f6c 2074 6f20 6765 6e65 7261 7465  tool to generate
+000001c0: 2067 656f 7370 6174 6961 6c20 7665 6374   geospatial vect
+000001d0: 6f72 2072 6570 7265 7365 6e74 6174 696f  or representatio
+000001e0: 6e20 6f66 2070 6c61 6e65 7461 7279 2073  n of planetary s
+000001f0: 7065 6374 726f 6d65 7465 7273 2e22 2c0a  pectrometers.",.
+00000200: 2020 226c 6963 656e 7365 223a 2022 6770    "license": "gp
+00000210: 6c22 2c0a 2020 2261 6363 6573 735f 7269  l",.  "access_ri
+00000220: 6768 7422 3a20 226f 7065 6e22 2c0a 2020  ght": "open",.  
+00000230: 2275 706c 6f61 645f 7479 7065 223a 2022  "upload_type": "
+00000240: 736f 6674 7761 7265 2220 2020 200a 7d0a  software"    .}.
```

### Comparing `pix2vec-0.1.4/CONTRIBUTING.rst` & `pix2vec-0.1.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pix2vec-0.1.4/LICENSE` & `pix2vec-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pix2vec-0.1.4/Makefile` & `pix2vec-0.1.5/Makefile`

 * *Files identical despite different names*

### Comparing `pix2vec-0.1.4/PKG-INFO` & `pix2vec-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pix2vec
-Version: 0.1.4
+Version: 0.1.5
 Summary: pix2vec produces a vector representation of planetary mapping spectrometers hyperspectral and camera ISIS data cube
 Home-page: https://github.com/afrigeri/pix2vec
 Author: Alessandro Frigeri
 Author-email: alessandro.frigeri@inaf.it
 License: GNU General Public License v3
 Keywords: pix2vec
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `pix2vec-0.1.4/README.rst` & `pix2vec-0.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `pix2vec-0.1.4/docs/Makefile` & `pix2vec-0.1.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pix2vec-0.1.4/docs/_build/html/_images/m3cube-a.png` & `pix2vec-0.1.5/docs/_build/html/_images/m3cube-a.png`

 * *Files identical despite different names*

### Comparing `pix2vec-0.1.4/docs/conf.py` & `pix2vec-0.1.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pix2vec-0.1.4/docs/images/m3-PixelValue.png` & `pix2vec-0.1.5/docs/images/m3-PixelValue.png`

 * *Files identical despite different names*

### Comparing `pix2vec-0.1.4/docs/images/m3-detail.png` & `pix2vec-0.1.5/docs/images/m3-detail.png`

 * *Files identical despite different names*

### Comparing `pix2vec-0.1.4/docs/images/m3cube-a.png` & `pix2vec-0.1.5/docs/images/m3cube-a.png`

 * *Files identical despite different names*

### Comparing `pix2vec-0.1.4/docs/images/m3cube-c.png` & `pix2vec-0.1.5/docs/images/m3cube-c.png`

 * *Files identical despite different names*

### Comparing `pix2vec-0.1.4/docs/index.rst` & `pix2vec-0.1.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pix2vec-0.1.4/docs/installation.rst` & `pix2vec-0.1.5/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `pix2vec-0.1.4/docs/make.bat` & `pix2vec-0.1.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pix2vec-0.1.4/pix2vec/cli.py` & `pix2vec-0.1.5/pix2vec/cli.py`

 * *Files identical despite different names*

### Comparing `pix2vec-0.1.4/pix2vec/pix2vec.py` & `pix2vec-0.1.5/pix2vec/pix2vec.py`

 * *Files identical despite different names*

### Comparing `pix2vec-0.1.4/pix2vec.egg-info/PKG-INFO` & `pix2vec-0.1.5/pix2vec.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pix2vec
-Version: 0.1.4
+Version: 0.1.5
 Summary: pix2vec produces a vector representation of planetary mapping spectrometers hyperspectral and camera ISIS data cube
 Home-page: https://github.com/afrigeri/pix2vec
 Author: Alessandro Frigeri
 Author-email: alessandro.frigeri@inaf.it
 License: GNU General Public License v3
 Keywords: pix2vec
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `pix2vec-0.1.4/pix2vec.egg-info/SOURCES.txt` & `pix2vec-0.1.5/pix2vec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pix2vec-0.1.4/setup.py` & `pix2vec-0.1.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,10 +43,10 @@
     include_package_data=True,
     keywords='pix2vec',
     name='pix2vec',
     packages=find_packages(include=['pix2vec', 'pix2vec.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/afrigeri/pix2vec',
-    version='0.1.4',
+    version='0.1.5',
     zip_safe=False,
 )
```

### Comparing `pix2vec-0.1.4/tests/files/crism.cub` & `pix2vec-0.1.5/tests/files/crism.cub`

 * *Files identical despite different names*

