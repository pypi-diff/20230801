# Comparing `tmp/mongodriver-1.2.2.tar.gz` & `tmp/mongodriver-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongodriver-1.2.2.tar", last modified: Mon Jul 24 15:55:22 2023, max compression
+gzip compressed data, was "mongodriver-1.2.3.tar", last modified: Tue Aug  1 11:09:49 2023, max compression
```

## Comparing `mongodriver-1.2.2.tar` & `mongodriver-1.2.3.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxr-xr-x   0 jstrouse   (501) staff       (20)        0 2023-07-24 15:55:22.548739 mongodriver-1.2.2/
--rw-r--r--   0 jstrouse   (501) staff       (20)     1061 2022-08-27 03:52:41.000000 mongodriver-1.2.2/LICENSE
--rw-r--r--   0 jstrouse   (501) staff       (20)     3323 2023-07-24 15:55:22.548868 mongodriver-1.2.2/PKG-INFO
--rw-r--r--   0 jstrouse   (501) staff       (20)     2844 2023-07-20 15:38:01.000000 mongodriver-1.2.2/README.md
--rw-r--r--   0 jstrouse   (501) staff       (20)       80 2023-07-20 15:31:35.000000 mongodriver-1.2.2/pyproject.toml
--rw-r--r--   0 jstrouse   (501) staff       (20)      491 2023-07-24 15:55:22.549247 mongodriver-1.2.2/setup.cfg
--rw-r--r--   0 jstrouse   (501) staff       (20)      891 2023-07-24 15:54:30.000000 mongodriver-1.2.2/setup.py
-drwxr-xr-x   0 jstrouse   (501) staff       (20)        0 2023-07-24 15:55:22.545881 mongodriver-1.2.2/src/
-drwxr-xr-x   0 jstrouse   (501) staff       (20)        0 2023-07-24 15:55:22.547497 mongodriver-1.2.2/src/mongodriver/
--rw-r--r--   0 jstrouse   (501) staff       (20)        0 2022-02-01 18:07:29.000000 mongodriver-1.2.2/src/mongodriver/__init__.py
--rw-r--r--   0 jstrouse   (501) staff       (20)     7943 2023-07-24 15:51:04.000000 mongodriver-1.2.2/src/mongodriver/mongodriver.py
-drwxr-xr-x   0 jstrouse   (501) staff       (20)        0 2023-07-24 15:55:22.548562 mongodriver-1.2.2/src/mongodriver.egg-info/
--rw-r--r--   0 jstrouse   (501) staff       (20)     3323 2023-07-24 15:55:22.000000 mongodriver-1.2.2/src/mongodriver.egg-info/PKG-INFO
--rw-r--r--   0 jstrouse   (501) staff       (20)      304 2023-07-24 15:55:22.000000 mongodriver-1.2.2/src/mongodriver.egg-info/SOURCES.txt
--rw-r--r--   0 jstrouse   (501) staff       (20)        1 2023-07-24 15:55:22.000000 mongodriver-1.2.2/src/mongodriver.egg-info/dependency_links.txt
--rw-r--r--   0 jstrouse   (501) staff       (20)       29 2023-07-24 15:55:22.000000 mongodriver-1.2.2/src/mongodriver.egg-info/requires.txt
--rw-r--r--   0 jstrouse   (501) staff       (20)       12 2023-07-24 15:55:22.000000 mongodriver-1.2.2/src/mongodriver.egg-info/top_level.txt
+drwxr-xr-x   0 jstrouse   (501) staff       (20)        0 2023-08-01 11:09:49.894350 mongodriver-1.2.3/
+-rw-r--r--   0 jstrouse   (501) staff       (20)     1061 2022-08-27 03:52:41.000000 mongodriver-1.2.3/LICENSE
+-rw-r--r--   0 jstrouse   (501) staff       (20)      363 2023-08-01 11:09:49.894458 mongodriver-1.2.3/PKG-INFO
+-rw-r--r--   0 jstrouse   (501) staff       (20)     2844 2023-07-20 15:38:01.000000 mongodriver-1.2.3/README.md
+-rw-r--r--   0 jstrouse   (501) staff       (20)       80 2023-07-20 15:31:35.000000 mongodriver-1.2.3/pyproject.toml
+-rw-r--r--   0 jstrouse   (501) staff       (20)      491 2023-08-01 11:09:49.894799 mongodriver-1.2.3/setup.cfg
+drwxr-xr-x   0 jstrouse   (501) staff       (20)        0 2023-08-01 11:09:49.891146 mongodriver-1.2.3/src/
+drwxr-xr-x   0 jstrouse   (501) staff       (20)        0 2023-08-01 11:09:49.892902 mongodriver-1.2.3/src/mongodriver/
+-rw-r--r--   0 jstrouse   (501) staff       (20)        0 2022-02-01 18:07:29.000000 mongodriver-1.2.3/src/mongodriver/__init__.py
+-rw-r--r--   0 jstrouse   (501) staff       (20)     7943 2023-07-24 15:51:04.000000 mongodriver-1.2.3/src/mongodriver/mongodriver.py
+drwxr-xr-x   0 jstrouse   (501) staff       (20)        0 2023-08-01 11:09:49.894179 mongodriver-1.2.3/src/mongodriver.egg-info/
+-rw-r--r--   0 jstrouse   (501) staff       (20)      363 2023-08-01 11:09:49.000000 mongodriver-1.2.3/src/mongodriver.egg-info/PKG-INFO
+-rw-r--r--   0 jstrouse   (501) staff       (20)      295 2023-08-01 11:09:49.000000 mongodriver-1.2.3/src/mongodriver.egg-info/SOURCES.txt
+-rw-r--r--   0 jstrouse   (501) staff       (20)        1 2023-08-01 11:09:49.000000 mongodriver-1.2.3/src/mongodriver.egg-info/dependency_links.txt
+-rw-r--r--   0 jstrouse   (501) staff       (20)       29 2023-08-01 11:09:49.000000 mongodriver-1.2.3/src/mongodriver.egg-info/requires.txt
+-rw-r--r--   0 jstrouse   (501) staff       (20)        1 2023-08-01 11:09:49.000000 mongodriver-1.2.3/src/mongodriver.egg-info/top_level.txt
```

### Comparing `mongodriver-1.2.2/LICENSE` & `mongodriver-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mongodriver-1.2.2/PKG-INFO` & `mongodriver-1.2.3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: mongodriver
-Version: 1.2.2
-Summary: Object-oriented interactions with MongoDB
-Home-page: https://github.com/jakestrouse00/mongodriver
-Author: Jake Strouse
-Author-email: jstrouse@meh.llc
-License: MIT
-Keywords: mongodb
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # MongoDriver
 
 An object-oriented package for interacting with MongoDB documents
 
 
 
 Features
@@ -118,8 +102,8 @@
 # OR
 
 new_document.new_val1 = 15
 new_document.new_val2 = 10
 
 print(new_document)
 
-```
+```
```

### Comparing `mongodriver-1.2.2/src/mongodriver/mongodriver.py` & `mongodriver-1.2.3/src/mongodriver/mongodriver.py`

 * *Files identical despite different names*

