# Comparing `tmp/pyrage-stubs-1.0.1.tar.gz` & `tmp/pyrage-stubs-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrage-stubs-1.0.1.tar", last modified: Thu Aug  4 23:53:18 2022, max compression
+gzip compressed data, was "pyrage-stubs-1.1.0.tar", last modified: Tue Aug  1 03:36:29 2023, max compression
```

## Comparing `pyrage-stubs-1.0.1.tar` & `pyrage-stubs-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 william    (501) staff       (20)        0 2022-08-04 23:53:18.539996 pyrage-stubs-1.0.1/
--rw-r--r--   0 william    (501) staff       (20)     1109 2022-08-03 21:58:29.000000 pyrage-stubs-1.0.1/LICENSE
--rw-r--r--   0 william    (501) staff       (20)     2114 2022-08-04 23:53:18.539592 pyrage-stubs-1.0.1/PKG-INFO
--rw-r--r--   0 william    (501) staff       (20)      161 2022-08-03 21:58:29.000000 pyrage-stubs-1.0.1/README.md
--rw-r--r--   0 william    (501) staff       (20)      781 2022-08-04 23:52:46.000000 pyrage-stubs-1.0.1/pyproject.toml
-drwxr-xr-x   0 william    (501) staff       (20)        0 2022-08-04 23:53:18.536246 pyrage-stubs-1.0.1/pyrage-stubs/
--rw-r--r--   0 william    (501) staff       (20)      133 2022-08-03 21:58:29.000000 pyrage-stubs-1.0.1/pyrage-stubs/passphrase.py
--rw-r--r--   0 william    (501) staff       (20)      224 2022-08-03 21:58:29.000000 pyrage-stubs-1.0.1/pyrage-stubs/ssh.py
--rw-r--r--   0 william    (501) staff       (20)      252 2022-08-03 21:58:29.000000 pyrage-stubs-1.0.1/pyrage-stubs/x25519.py
-drwxr-xr-x   0 william    (501) staff       (20)        0 2022-08-04 23:53:18.538973 pyrage-stubs-1.0.1/pyrage_stubs.egg-info/
--rw-r--r--   0 william    (501) staff       (20)     2114 2022-08-04 23:53:18.000000 pyrage-stubs-1.0.1/pyrage_stubs.egg-info/PKG-INFO
--rw-r--r--   0 william    (501) staff       (20)      290 2022-08-04 23:53:18.000000 pyrage-stubs-1.0.1/pyrage_stubs.egg-info/SOURCES.txt
--rw-r--r--   0 william    (501) staff       (20)        1 2022-08-04 23:53:18.000000 pyrage-stubs-1.0.1/pyrage_stubs.egg-info/dependency_links.txt
--rw-r--r--   0 william    (501) staff       (20)       19 2022-08-04 23:53:18.000000 pyrage-stubs-1.0.1/pyrage_stubs.egg-info/requires.txt
--rw-r--r--   0 william    (501) staff       (20)       13 2022-08-04 23:53:18.000000 pyrage-stubs-1.0.1/pyrage_stubs.egg-info/top_level.txt
--rw-r--r--   0 william    (501) staff       (20)       38 2022-08-04 23:53:18.540149 pyrage-stubs-1.0.1/setup.cfg
--rw-r--r--   0 william    (501) staff       (20)      132 2022-08-03 21:58:29.000000 pyrage-stubs-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 03:36:29.067287 pyrage-stubs-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-08-01 03:35:59.000000 pyrage-stubs-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-08-01 03:36:29.063287 pyrage-stubs-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-08-01 03:35:59.000000 pyrage-stubs-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-08-01 03:35:59.000000 pyrage-stubs-1.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 03:36:29.063287 pyrage-stubs-1.1.0/pyrage-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-01 03:35:59.000000 pyrage-stubs-1.1.0/pyrage-stubs/passphrase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-08-01 03:35:59.000000 pyrage-stubs-1.1.0/pyrage-stubs/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-08-01 03:35:59.000000 pyrage-stubs-1.1.0/pyrage-stubs/x25519.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 03:36:29.063287 pyrage-stubs-1.1.0/pyrage_stubs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-08-01 03:36:29.000000 pyrage-stubs-1.1.0/pyrage_stubs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-08-01 03:36:29.000000 pyrage-stubs-1.1.0/pyrage_stubs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 03:36:29.000000 pyrage-stubs-1.1.0/pyrage_stubs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-01 03:36:29.000000 pyrage-stubs-1.1.0/pyrage_stubs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-01 03:36:29.000000 pyrage-stubs-1.1.0/pyrage_stubs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 03:36:29.067287 pyrage-stubs-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-08-01 03:35:59.000000 pyrage-stubs-1.1.0/setup.py
```

### Comparing `pyrage-stubs-1.0.1/LICENSE` & `pyrage-stubs-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrage-stubs-1.0.1/PKG-INFO` & `pyrage-stubs-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrage-stubs
-Version: 1.0.1
+Version: 1.1.0
 Summary: A PEP 561 stub package for pyrage's types
 Author-email: William Woodruff <william@yossarian.net>
 License: The MIT License (MIT)
         
         Copyright (c) 2022 William Woodruff <william @ yossarian.net>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyrage-stubs-1.0.1/pyproject.toml` & `pyrage-stubs-1.1.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 [build-system]
 requires = ["setuptools>=61.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyrage-stubs"
-version = "1.0.1"
+version = "1.1.0"
 description = "A PEP 561 stub package for pyrage's types"
 readme = "README.md"
 license = { file = "LICENSE" }
 authors = [{ name = "William Woodruff", email = "william@yossarian.net" }]
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Topic :: Security :: Cryptography",
   "Typing :: Stubs Only",
 ]
-dependencies = [
-  "pyrage>=1.0.0,<2.0"
-]
+dependencies = ["pyrage>=1.0.0,<2.0"]
 requires-python = ">= 3.7"
 
 [project.urls]
 Homepage = "https://pypi.org/project/pyrage/"
 Issues = "https://github.com/woodruffw/pyrage/issues"
 Source = "https://github.com/woodruffw/pyrage/tree/main/pyrage-stubs"
```

### Comparing `pyrage-stubs-1.0.1/pyrage_stubs.egg-info/PKG-INFO` & `pyrage-stubs-1.1.0/pyrage_stubs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrage-stubs
-Version: 1.0.1
+Version: 1.1.0
 Summary: A PEP 561 stub package for pyrage's types
 Author-email: William Woodruff <william@yossarian.net>
 License: The MIT License (MIT)
         
         Copyright (c) 2022 William Woodruff <william @ yossarian.net>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

