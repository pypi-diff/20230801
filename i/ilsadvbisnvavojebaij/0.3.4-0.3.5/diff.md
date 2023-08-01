# Comparing `tmp/ilsadvbisnvavojebaij-0.3.4.tar.gz` & `tmp/ilsadvbisnvavojebaij-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ilsadvbisnvavojebaij-0.3.4.tar", last modified: Wed Jul 19 07:10:29 2023, max compression
+gzip compressed data, was "ilsadvbisnvavojebaij-0.3.5.tar", last modified: Tue Aug  1 20:05:25 2023, max compression
```

## Comparing `ilsadvbisnvavojebaij-0.3.4.tar` & `ilsadvbisnvavojebaij-0.3.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:10:29.828250 ilsadvbisnvavojebaij-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-19 07:10:29.828250 ilsadvbisnvavojebaij-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 07:10:10.000000 ilsadvbisnvavojebaij-0.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-19 07:10:10.000000 ilsadvbisnvavojebaij-0.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-19 07:10:29.832250 ilsadvbisnvavojebaij-0.3.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:10:29.828250 ilsadvbisnvavojebaij-0.3.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:10:29.828250 ilsadvbisnvavojebaij-0.3.4/src/ilsadvbisnvavojebaij/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-19 07:10:10.000000 ilsadvbisnvavojebaij-0.3.4/src/ilsadvbisnvavojebaij/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:10:29.828250 ilsadvbisnvavojebaij-0.3.4/src/ilsadvbisnvavojebaij/math/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 07:10:10.000000 ilsadvbisnvavojebaij-0.3.4/src/ilsadvbisnvavojebaij/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-19 07:10:10.000000 ilsadvbisnvavojebaij-0.3.4/src/ilsadvbisnvavojebaij/math/scalars.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-19 07:10:10.000000 ilsadvbisnvavojebaij-0.3.4/src/ilsadvbisnvavojebaij/math/vectors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:10:29.828250 ilsadvbisnvavojebaij-0.3.4/src/ilsadvbisnvavojebaij/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 07:10:10.000000 ilsadvbisnvavojebaij-0.3.4/src/ilsadvbisnvavojebaij/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-19 07:10:10.000000 ilsadvbisnvavojebaij-0.3.4/src/ilsadvbisnvavojebaij/utils/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:10:29.828250 ilsadvbisnvavojebaij-0.3.4/src/ilsadvbisnvavojebaij.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-19 07:10:29.000000 ilsadvbisnvavojebaij-0.3.4/src/ilsadvbisnvavojebaij.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-19 07:10:29.000000 ilsadvbisnvavojebaij-0.3.4/src/ilsadvbisnvavojebaij.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 07:10:29.000000 ilsadvbisnvavojebaij-0.3.4/src/ilsadvbisnvavojebaij.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-19 07:10:29.000000 ilsadvbisnvavojebaij-0.3.4/src/ilsadvbisnvavojebaij.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-19 07:10:29.000000 ilsadvbisnvavojebaij-0.3.4/src/ilsadvbisnvavojebaij.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:05:25.050787 ilsadvbisnvavojebaij-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-08-01 20:05:25.050787 ilsadvbisnvavojebaij-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:05:04.000000 ilsadvbisnvavojebaij-0.3.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-08-01 20:05:04.000000 ilsadvbisnvavojebaij-0.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-08-01 20:05:25.050787 ilsadvbisnvavojebaij-0.3.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:05:25.042786 ilsadvbisnvavojebaij-0.3.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:05:25.046786 ilsadvbisnvavojebaij-0.3.5/src/ilsadvbisnvavojebaij/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-01 20:05:04.000000 ilsadvbisnvavojebaij-0.3.5/src/ilsadvbisnvavojebaij/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:05:25.046786 ilsadvbisnvavojebaij-0.3.5/src/ilsadvbisnvavojebaij/math/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:05:04.000000 ilsadvbisnvavojebaij-0.3.5/src/ilsadvbisnvavojebaij/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-08-01 20:05:04.000000 ilsadvbisnvavojebaij-0.3.5/src/ilsadvbisnvavojebaij/math/scalars.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-08-01 20:05:04.000000 ilsadvbisnvavojebaij-0.3.5/src/ilsadvbisnvavojebaij/math/vectors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:05:25.046786 ilsadvbisnvavojebaij-0.3.5/src/ilsadvbisnvavojebaij/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:05:04.000000 ilsadvbisnvavojebaij-0.3.5/src/ilsadvbisnvavojebaij/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-08-01 20:05:04.000000 ilsadvbisnvavojebaij-0.3.5/src/ilsadvbisnvavojebaij/utils/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:05:25.046786 ilsadvbisnvavojebaij-0.3.5/src/ilsadvbisnvavojebaij.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-08-01 20:05:25.000000 ilsadvbisnvavojebaij-0.3.5/src/ilsadvbisnvavojebaij.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-01 20:05:25.000000 ilsadvbisnvavojebaij-0.3.5/src/ilsadvbisnvavojebaij.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 20:05:25.000000 ilsadvbisnvavojebaij-0.3.5/src/ilsadvbisnvavojebaij.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-01 20:05:25.000000 ilsadvbisnvavojebaij-0.3.5/src/ilsadvbisnvavojebaij.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-01 20:05:25.000000 ilsadvbisnvavojebaij-0.3.5/src/ilsadvbisnvavojebaij.egg-info/top_level.txt
```

### Comparing `ilsadvbisnvavojebaij-0.3.4/PKG-INFO` & `ilsadvbisnvavojebaij-0.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ilsadvbisnvavojebaij
-Version: 0.3.4
+Version: 0.3.5
 Summary: A randome placeholder package for CI testing
 Author: Francisco Castillo
 Author-email: fjcastillocarrasco@gmail.com
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `ilsadvbisnvavojebaij-0.3.4/setup.cfg` & `ilsadvbisnvavojebaij-0.3.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `ilsadvbisnvavojebaij-0.3.4/src/ilsadvbisnvavojebaij/math/vectors.py` & `ilsadvbisnvavojebaij-0.3.5/src/ilsadvbisnvavojebaij/math/vectors.py`

 * *Files identical despite different names*

### Comparing `ilsadvbisnvavojebaij-0.3.4/src/ilsadvbisnvavojebaij/utils/logging.py` & `ilsadvbisnvavojebaij-0.3.5/src/ilsadvbisnvavojebaij/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ilsadvbisnvavojebaij-0.3.4/src/ilsadvbisnvavojebaij.egg-info/PKG-INFO` & `ilsadvbisnvavojebaij-0.3.5/src/ilsadvbisnvavojebaij.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ilsadvbisnvavojebaij
-Version: 0.3.4
+Version: 0.3.5
 Summary: A randome placeholder package for CI testing
 Author: Francisco Castillo
 Author-email: fjcastillocarrasco@gmail.com
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `ilsadvbisnvavojebaij-0.3.4/src/ilsadvbisnvavojebaij.egg-info/SOURCES.txt` & `ilsadvbisnvavojebaij-0.3.5/src/ilsadvbisnvavojebaij.egg-info/SOURCES.txt`

 * *Files identical despite different names*

