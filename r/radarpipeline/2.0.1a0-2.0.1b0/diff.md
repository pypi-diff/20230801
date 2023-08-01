# Comparing `tmp/radarpipeline-2.0.1a0.tar.gz` & `tmp/radarpipeline-2.0.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/radarpipeline-2.0.1a0.tar", last modified: Tue Aug  1 09:02:02 2023, max compression
+gzip compressed data, was "dist/radarpipeline-2.0.1b0.tar", last modified: Tue Aug  1 15:56:03 2023, max compression
```

## Comparing `radarpipeline-2.0.1a0.tar` & `radarpipeline-2.0.1b0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 heetsankesara   (501) staff       (20)        0 2023-08-01 09:02:02.243361 radarpipeline-2.0.1a0/
--rw-r--r--   0 heetsankesara   (501) staff       (20)      527 2023-01-30 12:52:44.000000 radarpipeline-2.0.1a0/CITATION.cff
--rw-r--r--   0 heetsankesara   (501) staff       (20)    11357 2022-09-09 10:12:31.000000 radarpipeline-2.0.1a0/LICENSE
--rw-r--r--   0 heetsankesara   (501) staff       (20)       54 2023-08-01 08:52:44.000000 radarpipeline-2.0.1a0/MANIFEST.in
--rw-r--r--   0 heetsankesara   (501) staff       (20)     5980 2023-08-01 09:02:02.243627 radarpipeline-2.0.1a0/PKG-INFO
--rw-r--r--   0 heetsankesara   (501) staff       (20)     5095 2023-07-24 11:09:53.000000 radarpipeline-2.0.1a0/README.md
--rw-r--r--   0 heetsankesara   (501) staff       (20)      284 2023-07-24 11:09:53.000000 radarpipeline-2.0.1a0/pyproject.toml
-drwxr-xr-x   0 heetsankesara   (501) staff       (20)        0 2023-08-01 09:02:02.214133 radarpipeline-2.0.1a0/radarpipeline/
--rw-r--r--   0 heetsankesara   (501) staff       (20)       42 2022-10-31 14:22:37.000000 radarpipeline-2.0.1a0/radarpipeline/__init__.py
-drwxr-xr-x   0 heetsankesara   (501) staff       (20)        0 2023-08-01 09:02:02.220219 radarpipeline-2.0.1a0/radarpipeline/common/
--rw-r--r--   0 heetsankesara   (501) staff       (20)       58 2022-10-31 14:22:37.000000 radarpipeline-2.0.1a0/radarpipeline/common/__init__.py
--rw-r--r--   0 heetsankesara   (501) staff       (20)      834 2023-07-24 11:09:53.000000 radarpipeline-2.0.1a0/radarpipeline/common/constants.py
--rw-r--r--   0 heetsankesara   (501) staff       (20)     1333 2023-07-24 11:09:53.000000 radarpipeline-2.0.1a0/radarpipeline/common/logger.py
--rw-r--r--   0 heetsankesara   (501) staff       (20)     5761 2023-07-24 11:09:53.000000 radarpipeline-2.0.1a0/radarpipeline/common/utils.py
-drwxr-xr-x   0 heetsankesara   (501) staff       (20)        0 2023-08-01 09:02:02.224207 radarpipeline-2.0.1a0/radarpipeline/datalib/
--rw-r--r--   0 heetsankesara   (501) staff       (20)      234 2022-10-31 14:22:37.000000 radarpipeline-2.0.1a0/radarpipeline/datalib/__init__.py
--rw-r--r--   0 heetsankesara   (501) staff       (20)      677 2023-07-18 09:47:35.000000 radarpipeline-2.0.1a0/radarpipeline/datalib/abc.py
--rw-r--r--   0 heetsankesara   (501) staff       (20)     4676 2023-07-24 11:09:53.000000 radarpipeline-2.0.1a0/radarpipeline/datalib/radar_data.py
--rw-r--r--   0 heetsankesara   (501) staff       (20)     2283 2022-10-31 14:22:37.000000 radarpipeline-2.0.1a0/radarpipeline/datalib/radar_user_data.py
--rw-r--r--   0 heetsankesara   (501) staff       (20)     2247 2022-10-31 14:22:37.000000 radarpipeline-2.0.1a0/radarpipeline/datalib/radar_variable_data.py
-drwxr-xr-x   0 heetsankesara   (501) staff       (20)        0 2023-08-01 09:02:02.225771 radarpipeline-2.0.1a0/radarpipeline/datatypes/
--rw-r--r--   0 heetsankesara   (501) staff       (20)       56 2022-10-31 14:22:37.000000 radarpipeline-2.0.1a0/radarpipeline/datatypes/__init__.py
--rw-r--r--   0 heetsankesara   (501) staff       (20)      117 2022-10-31 14:22:37.000000 radarpipeline-2.0.1a0/radarpipeline/datatypes/data_types.py
-drwxr-xr-x   0 heetsankesara   (501) staff       (20)        0 2023-08-01 09:02:02.228132 radarpipeline-2.0.1a0/radarpipeline/features/
--rw-r--r--   0 heetsankesara   (501) staff       (20)      113 2022-10-31 14:22:37.000000 radarpipeline-2.0.1a0/radarpipeline/features/__init__.py
--rw-r--r--   0 heetsankesara   (501) staff       (20)      945 2023-07-24 11:09:53.000000 radarpipeline-2.0.1a0/radarpipeline/features/feature.py
--rw-r--r--   0 heetsankesara   (501) staff       (20)     3517 2023-07-24 11:09:53.000000 radarpipeline-2.0.1a0/radarpipeline/features/feature_group.py
-drwxr-xr-x   0 heetsankesara   (501) staff       (20)        0 2023-08-01 09:02:02.233486 radarpipeline-2.0.1a0/radarpipeline/io/
--rw-r--r--   0 heetsankesara   (501) staff       (20)      232 2023-07-24 11:09:53.000000 radarpipeline-2.0.1a0/radarpipeline/io/__init__.py
--rw-r--r--   0 heetsankesara   (501) staff       (20)     1121 2023-07-18 09:54:14.000000 radarpipeline-2.0.1a0/radarpipeline/io/abc.py
--rw-r--r--   0 heetsankesara   (501) staff       (20)     8434 2023-07-24 11:09:53.000000 radarpipeline-2.0.1a0/radarpipeline/io/connection.py
--rw-r--r--   0 heetsankesara   (501) staff       (20)     5745 2023-07-24 11:09:53.000000 radarpipeline-2.0.1a0/radarpipeline/io/downloader.py
--rw-r--r--   0 heetsankesara   (501) staff       (20)    16845 2023-07-24 11:09:53.000000 radarpipeline-2.0.1a0/radarpipeline/io/reader.py
--rw-r--r--   0 heetsankesara   (501) staff       (20)     2964 2023-02-16 14:17:56.000000 radarpipeline-2.0.1a0/radarpipeline/io/writer.py
-drwxr-xr-x   0 heetsankesara   (501) staff       (20)        0 2023-08-01 09:02:02.237041 radarpipeline-2.0.1a0/radarpipeline/project/
--rw-r--r--   0 heetsankesara   (501) staff       (20)       50 2023-05-24 14:54:38.000000 radarpipeline-2.0.1a0/radarpipeline/project/__init__.py
--rw-r--r--   0 heetsankesara   (501) staff       (20)    11459 2023-07-24 11:09:53.000000 radarpipeline-2.0.1a0/radarpipeline/project/project.py
--rw-r--r--   0 heetsankesara   (501) staff       (20)     9167 2023-07-24 11:09:53.000000 radarpipeline-2.0.1a0/radarpipeline/project/validations.py
--rw-r--r--   0 heetsankesara   (501) staff       (20)     1827 2023-07-24 11:09:53.000000 radarpipeline-2.0.1a0/radarpipeline/radarpipeline.py
-drwxr-xr-x   0 heetsankesara   (501) staff       (20)        0 2023-08-01 09:02:02.238130 radarpipeline-2.0.1a0/radarpipeline/visualization/
--rw-r--r--   0 heetsankesara   (501) staff       (20)        0 2022-10-31 14:22:37.000000 radarpipeline-2.0.1a0/radarpipeline/visualization/__init__.py
-drwxr-xr-x   0 heetsankesara   (501) staff       (20)        0 2023-08-01 09:02:02.217316 radarpipeline-2.0.1a0/radarpipeline.egg-info/
--rw-r--r--   0 heetsankesara   (501) staff       (20)     5980 2023-08-01 09:02:02.000000 radarpipeline-2.0.1a0/radarpipeline.egg-info/PKG-INFO
--rw-r--r--   0 heetsankesara   (501) staff       (20)     1192 2023-08-01 09:02:02.000000 radarpipeline-2.0.1a0/radarpipeline.egg-info/SOURCES.txt
--rw-r--r--   0 heetsankesara   (501) staff       (20)        1 2023-08-01 09:02:02.000000 radarpipeline-2.0.1a0/radarpipeline.egg-info/dependency_links.txt
--rw-r--r--   0 heetsankesara   (501) staff       (20)       92 2023-08-01 09:02:02.000000 radarpipeline-2.0.1a0/radarpipeline.egg-info/requires.txt
--rw-r--r--   0 heetsankesara   (501) staff       (20)       23 2023-08-01 09:02:02.000000 radarpipeline-2.0.1a0/radarpipeline.egg-info/top_level.txt
--rw-r--r--   0 heetsankesara   (501) staff       (20)       79 2023-08-01 09:02:02.244392 radarpipeline-2.0.1a0/setup.cfg
--rw-r--r--   0 heetsankesara   (501) staff       (20)     1479 2023-08-01 08:53:17.000000 radarpipeline-2.0.1a0/setup.py
-drwxr-xr-x   0 heetsankesara   (501) staff       (20)        0 2023-08-01 09:02:02.240373 radarpipeline-2.0.1a0/temp/
--rw-r--r--   0 heetsankesara   (501) staff       (20)      200 2023-06-07 10:12:34.000000 radarpipeline-2.0.1a0/temp/__init__.py
--rw-r--r--   0 heetsankesara   (501) staff       (20)       92 2023-06-07 10:12:34.000000 radarpipeline-2.0.1a0/temp/__main__.py
-drwxr-xr-x   0 heetsankesara   (501) staff       (20)        0 2023-08-01 09:02:02.242389 radarpipeline-2.0.1a0/tmp/
--rw-r--r--   0 heetsankesara   (501) staff       (20)      200 2023-06-07 10:17:33.000000 radarpipeline-2.0.1a0/tmp/__init__.py
--rw-r--r--   0 heetsankesara   (501) staff       (20)       92 2023-06-07 10:17:33.000000 radarpipeline-2.0.1a0/tmp/__main__.py
+drwxr-xr-x   0 heetsankesara   (501) staff       (20)        0 2023-08-01 15:56:03.630357 radarpipeline-2.0.1b0/
+-rw-r--r--   0 heetsankesara   (501) staff       (20)      527 2023-01-30 12:52:44.000000 radarpipeline-2.0.1b0/CITATION.cff
+-rw-r--r--   0 heetsankesara   (501) staff       (20)    11357 2022-09-09 10:12:31.000000 radarpipeline-2.0.1b0/LICENSE
+-rw-r--r--   0 heetsankesara   (501) staff       (20)       54 2023-08-01 08:52:44.000000 radarpipeline-2.0.1b0/MANIFEST.in
+-rw-r--r--   0 heetsankesara   (501) staff       (20)     5918 2023-08-01 15:56:03.630496 radarpipeline-2.0.1b0/PKG-INFO
+-rw-r--r--   0 heetsankesara   (501) staff       (20)     5095 2023-07-24 11:09:53.000000 radarpipeline-2.0.1b0/README.md
+-rw-r--r--   0 heetsankesara   (501) staff       (20)      284 2023-07-24 11:09:53.000000 radarpipeline-2.0.1b0/pyproject.toml
+drwxr-xr-x   0 heetsankesara   (501) staff       (20)        0 2023-08-01 15:56:03.613440 radarpipeline-2.0.1b0/radarpipeline/
+-rw-r--r--   0 heetsankesara   (501) staff       (20)       42 2022-10-31 14:22:37.000000 radarpipeline-2.0.1b0/radarpipeline/__init__.py
+drwxr-xr-x   0 heetsankesara   (501) staff       (20)        0 2023-08-01 15:56:03.617318 radarpipeline-2.0.1b0/radarpipeline/common/
+-rw-r--r--   0 heetsankesara   (501) staff       (20)       58 2022-10-31 14:22:37.000000 radarpipeline-2.0.1b0/radarpipeline/common/__init__.py
+-rw-r--r--   0 heetsankesara   (501) staff       (20)      834 2023-07-24 11:09:53.000000 radarpipeline-2.0.1b0/radarpipeline/common/constants.py
+-rw-r--r--   0 heetsankesara   (501) staff       (20)     1333 2023-07-24 11:09:53.000000 radarpipeline-2.0.1b0/radarpipeline/common/logger.py
+-rw-r--r--   0 heetsankesara   (501) staff       (20)     5761 2023-07-24 11:09:53.000000 radarpipeline-2.0.1b0/radarpipeline/common/utils.py
+drwxr-xr-x   0 heetsankesara   (501) staff       (20)        0 2023-08-01 15:56:03.620410 radarpipeline-2.0.1b0/radarpipeline/datalib/
+-rw-r--r--   0 heetsankesara   (501) staff       (20)      234 2022-10-31 14:22:37.000000 radarpipeline-2.0.1b0/radarpipeline/datalib/__init__.py
+-rw-r--r--   0 heetsankesara   (501) staff       (20)      677 2023-07-18 09:47:35.000000 radarpipeline-2.0.1b0/radarpipeline/datalib/abc.py
+-rw-r--r--   0 heetsankesara   (501) staff       (20)     4676 2023-07-24 11:09:53.000000 radarpipeline-2.0.1b0/radarpipeline/datalib/radar_data.py
+-rw-r--r--   0 heetsankesara   (501) staff       (20)     2283 2022-10-31 14:22:37.000000 radarpipeline-2.0.1b0/radarpipeline/datalib/radar_user_data.py
+-rw-r--r--   0 heetsankesara   (501) staff       (20)     2247 2022-10-31 14:22:37.000000 radarpipeline-2.0.1b0/radarpipeline/datalib/radar_variable_data.py
+drwxr-xr-x   0 heetsankesara   (501) staff       (20)        0 2023-08-01 15:56:03.621353 radarpipeline-2.0.1b0/radarpipeline/datatypes/
+-rw-r--r--   0 heetsankesara   (501) staff       (20)       56 2022-10-31 14:22:37.000000 radarpipeline-2.0.1b0/radarpipeline/datatypes/__init__.py
+-rw-r--r--   0 heetsankesara   (501) staff       (20)      117 2022-10-31 14:22:37.000000 radarpipeline-2.0.1b0/radarpipeline/datatypes/data_types.py
+drwxr-xr-x   0 heetsankesara   (501) staff       (20)        0 2023-08-01 15:56:03.622800 radarpipeline-2.0.1b0/radarpipeline/features/
+-rw-r--r--   0 heetsankesara   (501) staff       (20)      113 2022-10-31 14:22:37.000000 radarpipeline-2.0.1b0/radarpipeline/features/__init__.py
+-rw-r--r--   0 heetsankesara   (501) staff       (20)      945 2023-07-24 11:09:53.000000 radarpipeline-2.0.1b0/radarpipeline/features/feature.py
+-rw-r--r--   0 heetsankesara   (501) staff       (20)     3517 2023-07-24 11:09:53.000000 radarpipeline-2.0.1b0/radarpipeline/features/feature_group.py
+drwxr-xr-x   0 heetsankesara   (501) staff       (20)        0 2023-08-01 15:56:03.626233 radarpipeline-2.0.1b0/radarpipeline/io/
+-rw-r--r--   0 heetsankesara   (501) staff       (20)      232 2023-07-24 11:09:53.000000 radarpipeline-2.0.1b0/radarpipeline/io/__init__.py
+-rw-r--r--   0 heetsankesara   (501) staff       (20)     1121 2023-07-18 09:54:14.000000 radarpipeline-2.0.1b0/radarpipeline/io/abc.py
+-rw-r--r--   0 heetsankesara   (501) staff       (20)     8434 2023-07-24 11:09:53.000000 radarpipeline-2.0.1b0/radarpipeline/io/connection.py
+-rw-r--r--   0 heetsankesara   (501) staff       (20)     5745 2023-07-24 11:09:53.000000 radarpipeline-2.0.1b0/radarpipeline/io/downloader.py
+-rw-r--r--   0 heetsankesara   (501) staff       (20)    16845 2023-07-24 11:09:53.000000 radarpipeline-2.0.1b0/radarpipeline/io/reader.py
+-rw-r--r--   0 heetsankesara   (501) staff       (20)     2964 2023-02-16 14:17:56.000000 radarpipeline-2.0.1b0/radarpipeline/io/writer.py
+drwxr-xr-x   0 heetsankesara   (501) staff       (20)        0 2023-08-01 15:56:03.628059 radarpipeline-2.0.1b0/radarpipeline/project/
+-rw-r--r--   0 heetsankesara   (501) staff       (20)       50 2023-05-24 14:54:38.000000 radarpipeline-2.0.1b0/radarpipeline/project/__init__.py
+-rw-r--r--   0 heetsankesara   (501) staff       (20)    11459 2023-07-24 11:09:53.000000 radarpipeline-2.0.1b0/radarpipeline/project/project.py
+-rw-r--r--   0 heetsankesara   (501) staff       (20)     9167 2023-07-24 11:09:53.000000 radarpipeline-2.0.1b0/radarpipeline/project/validations.py
+-rw-r--r--   0 heetsankesara   (501) staff       (20)     1827 2023-07-24 11:09:53.000000 radarpipeline-2.0.1b0/radarpipeline/radarpipeline.py
+drwxr-xr-x   0 heetsankesara   (501) staff       (20)        0 2023-08-01 15:56:03.628453 radarpipeline-2.0.1b0/radarpipeline/visualization/
+-rw-r--r--   0 heetsankesara   (501) staff       (20)        0 2022-10-31 14:22:37.000000 radarpipeline-2.0.1b0/radarpipeline/visualization/__init__.py
+drwxr-xr-x   0 heetsankesara   (501) staff       (20)        0 2023-08-01 15:56:03.615978 radarpipeline-2.0.1b0/radarpipeline.egg-info/
+-rw-r--r--   0 heetsankesara   (501) staff       (20)     5918 2023-08-01 15:56:03.000000 radarpipeline-2.0.1b0/radarpipeline.egg-info/PKG-INFO
+-rw-r--r--   0 heetsankesara   (501) staff       (20)     1192 2023-08-01 15:56:03.000000 radarpipeline-2.0.1b0/radarpipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 heetsankesara   (501) staff       (20)        1 2023-08-01 15:56:03.000000 radarpipeline-2.0.1b0/radarpipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 heetsankesara   (501) staff       (20)      126 2023-08-01 15:56:03.000000 radarpipeline-2.0.1b0/radarpipeline.egg-info/requires.txt
+-rw-r--r--   0 heetsankesara   (501) staff       (20)       23 2023-08-01 15:56:03.000000 radarpipeline-2.0.1b0/radarpipeline.egg-info/top_level.txt
+-rw-r--r--   0 heetsankesara   (501) staff       (20)       79 2023-08-01 15:56:03.630926 radarpipeline-2.0.1b0/setup.cfg
+-rw-r--r--   0 heetsankesara   (501) staff       (20)     1475 2023-08-01 15:55:51.000000 radarpipeline-2.0.1b0/setup.py
+drwxr-xr-x   0 heetsankesara   (501) staff       (20)        0 2023-08-01 15:56:03.629045 radarpipeline-2.0.1b0/temp/
+-rw-r--r--   0 heetsankesara   (501) staff       (20)      200 2023-06-07 10:12:34.000000 radarpipeline-2.0.1b0/temp/__init__.py
+-rw-r--r--   0 heetsankesara   (501) staff       (20)       92 2023-06-07 10:12:34.000000 radarpipeline-2.0.1b0/temp/__main__.py
+drwxr-xr-x   0 heetsankesara   (501) staff       (20)        0 2023-08-01 15:56:03.629799 radarpipeline-2.0.1b0/tmp/
+-rw-r--r--   0 heetsankesara   (501) staff       (20)      200 2023-06-07 10:17:33.000000 radarpipeline-2.0.1b0/tmp/__init__.py
+-rw-r--r--   0 heetsankesara   (501) staff       (20)       92 2023-06-07 10:17:33.000000 radarpipeline-2.0.1b0/tmp/__main__.py
```

### Comparing `radarpipeline-2.0.1a0/CITATION.cff` & `radarpipeline-2.0.1b0/CITATION.cff`

 * *Files identical despite different names*

### Comparing `radarpipeline-2.0.1a0/LICENSE` & `radarpipeline-2.0.1b0/LICENSE`

 * *Files identical despite different names*

### Comparing `radarpipeline-2.0.1a0/PKG-INFO` & `radarpipeline-2.0.1b0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 Metadata-Version: 2.1
 Name: radarpipeline
-Version: 2.0.1a0
+Version: 2.0.1b0
 Summary: A python feature generation and visualization package use with RADAR project data.
 Home-page: https://github.com/RADAR-base/radarpipeline
 Download-URL: https://github.com/RADAR-base/radarpipeline/archive/refs/tags/v2.0.0.tar.gz
-Author: Heet Sankesara
-Author-email: heet.sankesara@kcl.ac.uk
+Author: Heet Sankesara, Amos Folarin
+Author-email: heet.sankesara@kcl.ac.uk, amos.folarin@kcl.ac.uk
 License: Apache
 Keywords: mhealth,pipeline,big-data
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">RADAR Pipeline</h1>
```

#### html2text {}

```diff
@@ -1,19 +1,18 @@
-Metadata-Version: 2.1 Name: radarpipeline Version: 2.0.1a0 Summary: A python
+Metadata-Version: 2.1 Name: radarpipeline Version: 2.0.1b0 Summary: A python
 feature generation and visualization package use with RADAR project data. Home-
 page: https://github.com/RADAR-base/radarpipeline Download-URL: https://
 github.com/RADAR-base/radarpipeline/archive/refs/tags/v2.0.0.tar.gz Author:
-Heet Sankesara Author-email: heet.sankesara@kcl.ac.uk License: Apache Keywords:
-mhealth,pipeline,big-data Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License Classifier:
-Intended Audience :: Science/Research Classifier: Programming Language ::
-Python :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Description-
-Content-Type: text/markdown License-File: LICENSE
+Heet Sankesara, Amos Folarin Author-email: heet.sankesara@kcl.ac.uk,
+amos.folarin@kcl.ac.uk License: Apache Keywords: mhealth,pipeline,big-data
+Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
+Approved :: Apache Software License Classifier: Intended Audience :: Science/
+Research Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Description-Content-Type: text/markdown License-File: LICENSE
                          ****** RADAR Pipeline ******
   [GitHub_branch_checks_state] [GitHub_issues] [GitHub_pull_requests] [GitHub
           forks] [GitHub_stars] [GitHub_license] [Code_style:_black]
   An open-source python feature generation and visualization package use with
                               RADAR project data.
 --- ## Wiki Please visit the [RADAR Pipeline Wiki](https://github.com/RADAR-
 base/radarpipeline/wiki) to learn more about RADAR Pipeline. Also see the
```

### Comparing `radarpipeline-2.0.1a0/README.md` & `radarpipeline-2.0.1b0/README.md`

 * *Files identical despite different names*

### Comparing `radarpipeline-2.0.1a0/radarpipeline/common/constants.py` & `radarpipeline-2.0.1b0/radarpipeline/common/constants.py`

 * *Files identical despite different names*

### Comparing `radarpipeline-2.0.1a0/radarpipeline/common/logger.py` & `radarpipeline-2.0.1b0/radarpipeline/common/logger.py`

 * *Files identical despite different names*

### Comparing `radarpipeline-2.0.1a0/radarpipeline/common/utils.py` & `radarpipeline-2.0.1b0/radarpipeline/common/utils.py`

 * *Files identical despite different names*

### Comparing `radarpipeline-2.0.1a0/radarpipeline/datalib/abc.py` & `radarpipeline-2.0.1b0/radarpipeline/datalib/abc.py`

 * *Files identical despite different names*

### Comparing `radarpipeline-2.0.1a0/radarpipeline/datalib/radar_data.py` & `radarpipeline-2.0.1b0/radarpipeline/datalib/radar_data.py`

 * *Files identical despite different names*

### Comparing `radarpipeline-2.0.1a0/radarpipeline/datalib/radar_user_data.py` & `radarpipeline-2.0.1b0/radarpipeline/datalib/radar_user_data.py`

 * *Files identical despite different names*

### Comparing `radarpipeline-2.0.1a0/radarpipeline/datalib/radar_variable_data.py` & `radarpipeline-2.0.1b0/radarpipeline/datalib/radar_variable_data.py`

 * *Files identical despite different names*

### Comparing `radarpipeline-2.0.1a0/radarpipeline/features/feature.py` & `radarpipeline-2.0.1b0/radarpipeline/features/feature.py`

 * *Files identical despite different names*

### Comparing `radarpipeline-2.0.1a0/radarpipeline/features/feature_group.py` & `radarpipeline-2.0.1b0/radarpipeline/features/feature_group.py`

 * *Files identical despite different names*

### Comparing `radarpipeline-2.0.1a0/radarpipeline/io/abc.py` & `radarpipeline-2.0.1b0/radarpipeline/io/abc.py`

 * *Files identical despite different names*

### Comparing `radarpipeline-2.0.1a0/radarpipeline/io/connection.py` & `radarpipeline-2.0.1b0/radarpipeline/io/connection.py`

 * *Files identical despite different names*

### Comparing `radarpipeline-2.0.1a0/radarpipeline/io/downloader.py` & `radarpipeline-2.0.1b0/radarpipeline/io/downloader.py`

 * *Files identical despite different names*

### Comparing `radarpipeline-2.0.1a0/radarpipeline/io/reader.py` & `radarpipeline-2.0.1b0/radarpipeline/io/reader.py`

 * *Files identical despite different names*

### Comparing `radarpipeline-2.0.1a0/radarpipeline/io/writer.py` & `radarpipeline-2.0.1b0/radarpipeline/io/writer.py`

 * *Files identical despite different names*

### Comparing `radarpipeline-2.0.1a0/radarpipeline/project/project.py` & `radarpipeline-2.0.1b0/radarpipeline/project/project.py`

 * *Files identical despite different names*

### Comparing `radarpipeline-2.0.1a0/radarpipeline/project/validations.py` & `radarpipeline-2.0.1b0/radarpipeline/project/validations.py`

 * *Files identical despite different names*

### Comparing `radarpipeline-2.0.1a0/radarpipeline/radarpipeline.py` & `radarpipeline-2.0.1b0/radarpipeline/radarpipeline.py`

 * *Files identical despite different names*

### Comparing `radarpipeline-2.0.1a0/radarpipeline.egg-info/PKG-INFO` & `radarpipeline-2.0.1b0/radarpipeline.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 Metadata-Version: 2.1
 Name: radarpipeline
-Version: 2.0.1a0
+Version: 2.0.1b0
 Summary: A python feature generation and visualization package use with RADAR project data.
 Home-page: https://github.com/RADAR-base/radarpipeline
 Download-URL: https://github.com/RADAR-base/radarpipeline/archive/refs/tags/v2.0.0.tar.gz
-Author: Heet Sankesara
-Author-email: heet.sankesara@kcl.ac.uk
+Author: Heet Sankesara, Amos Folarin
+Author-email: heet.sankesara@kcl.ac.uk, amos.folarin@kcl.ac.uk
 License: Apache
 Keywords: mhealth,pipeline,big-data
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">RADAR Pipeline</h1>
```

#### html2text {}

```diff
@@ -1,19 +1,18 @@
-Metadata-Version: 2.1 Name: radarpipeline Version: 2.0.1a0 Summary: A python
+Metadata-Version: 2.1 Name: radarpipeline Version: 2.0.1b0 Summary: A python
 feature generation and visualization package use with RADAR project data. Home-
 page: https://github.com/RADAR-base/radarpipeline Download-URL: https://
 github.com/RADAR-base/radarpipeline/archive/refs/tags/v2.0.0.tar.gz Author:
-Heet Sankesara Author-email: heet.sankesara@kcl.ac.uk License: Apache Keywords:
-mhealth,pipeline,big-data Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License Classifier:
-Intended Audience :: Science/Research Classifier: Programming Language ::
-Python :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Description-
-Content-Type: text/markdown License-File: LICENSE
+Heet Sankesara, Amos Folarin Author-email: heet.sankesara@kcl.ac.uk,
+amos.folarin@kcl.ac.uk License: Apache Keywords: mhealth,pipeline,big-data
+Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
+Approved :: Apache Software License Classifier: Intended Audience :: Science/
+Research Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Description-Content-Type: text/markdown License-File: LICENSE
                          ****** RADAR Pipeline ******
   [GitHub_branch_checks_state] [GitHub_issues] [GitHub_pull_requests] [GitHub
           forks] [GitHub_stars] [GitHub_license] [Code_style:_black]
   An open-source python feature generation and visualization package use with
                               RADAR project data.
 --- ## Wiki Please visit the [RADAR Pipeline Wiki](https://github.com/RADAR-
 base/radarpipeline/wiki) to learn more about RADAR Pipeline. Also see the
```

### Comparing `radarpipeline-2.0.1a0/radarpipeline.egg-info/SOURCES.txt` & `radarpipeline-2.0.1b0/radarpipeline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `radarpipeline-2.0.1a0/setup.py` & `radarpipeline-2.0.1b0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,39 +6,39 @@
 def read_file(filename):
     with open(os.path.join(os.path.dirname(__file__), filename)) as file:
         return file.read()
 
 
 setup(
     name="radarpipeline",
-    version="2.0.1a",
+    version="2.0.1b",
     license='Apache',
     description="A python feature generation and visualization package use with RADAR project data.",
     url="https://github.com/RADAR-base/radarpipeline",
     download_url='https://github.com/RADAR-base/radarpipeline/archive/refs/tags/v2.0.0.tar.gz',
     readme="README.md",
     long_description=read_file('README.md'),
     long_description_content_type='text/markdown',
-    author="Heet Sankesara",
-    author_email="heet.sankesara@kcl.ac.uk",
+    author="Heet Sankesara, Amos Folarin",
+    author_email="heet.sankesara@kcl.ac.uk, amos.folarin@kcl.ac.uk",
     keywords=['mhealth', 'pipeline', 'big-data'],
     packages=find_packages(),
     install_requires=[
         "pyYaml==6.0",
         "pandas==1.4.1",
         "numpy==1.22.3",
         "scipy==1.10.0",
         "pyspark[sql]==3.3.0",
-        "GitPython==3.1.30"],
+        "GitPython==3.1.30",
+        "strictyaml==1.7.3",
+        "paramiko==3.1.0"],
     test_suite="tests",
     include_package_data=True,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Intended Audience :: Science/Research",
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
     ],
 )
```

