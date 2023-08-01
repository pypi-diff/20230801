# Comparing `tmp/aifactory-1.7.3.tar.gz` & `tmp/aifactory-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aifactory-1.7.3.tar", last modified: Wed Jul 19 08:29:14 2023, max compression
+gzip compressed data, was "aifactory-1.8.0.tar", last modified: Tue Aug  1 01:55:38 2023, max compression
```

## Comparing `aifactory-1.7.3.tar` & `aifactory-1.8.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 kyj        (501) staff       (20)        0 2023-07-19 08:29:14.576268 aifactory-1.7.3/
--rw-r--r--   0 kyj        (501) staff       (20)      228 2023-07-19 08:29:14.576099 aifactory-1.7.3/PKG-INFO
-drwxr-xr-x   0 kyj        (501) staff       (20)        0 2023-07-19 08:29:14.574999 aifactory-1.7.3/aifactory/
--rw-r--r--   0 kyj        (501) staff       (20)        0 2023-05-10 03:11:14.000000 aifactory-1.7.3/aifactory/__init__.py
--rw-r--r--   0 kyj        (501) staff       (20)     3743 2023-05-10 03:11:14.000000 aifactory-1.7.3/aifactory/api.py
--rw-r--r--   0 kyj        (501) staff       (20)     3710 2023-05-10 03:11:14.000000 aifactory-1.7.3/aifactory/demo.py
--rw-r--r--   0 kyj        (501) staff       (20)    14314 2023-05-10 03:11:14.000000 aifactory-1.7.3/aifactory/grade.py
--rw-r--r--   0 kyj        (501) staff       (20)     5966 2023-05-10 03:11:14.000000 aifactory-1.7.3/aifactory/make_zip.py
--rw-r--r--   0 kyj        (501) staff       (20)     7503 2023-07-19 08:14:00.000000 aifactory-1.7.3/aifactory/score.py
--rw-r--r--   0 kyj        (501) staff       (20)       50 2023-05-10 03:11:14.000000 aifactory-1.7.3/aifactory/train.py
-drwxr-xr-x   0 kyj        (501) staff       (20)        0 2023-07-19 08:29:14.575881 aifactory-1.7.3/aifactory.egg-info/
--rw-r--r--   0 kyj        (501) staff       (20)      228 2023-07-19 08:29:14.000000 aifactory-1.7.3/aifactory.egg-info/PKG-INFO
--rw-r--r--   0 kyj        (501) staff       (20)      308 2023-07-19 08:29:14.000000 aifactory-1.7.3/aifactory.egg-info/SOURCES.txt
--rw-r--r--   0 kyj        (501) staff       (20)        1 2023-07-19 08:29:14.000000 aifactory-1.7.3/aifactory.egg-info/dependency_links.txt
--rw-r--r--   0 kyj        (501) staff       (20)       41 2023-07-19 08:29:14.000000 aifactory-1.7.3/aifactory.egg-info/requires.txt
--rw-r--r--   0 kyj        (501) staff       (20)       17 2023-07-19 08:29:14.000000 aifactory-1.7.3/aifactory.egg-info/top_level.txt
--rw-r--r--   0 kyj        (501) staff       (20)       38 2023-07-19 08:29:14.576327 aifactory-1.7.3/setup.cfg
--rw-r--r--   0 kyj        (501) staff       (20)      430 2023-07-19 08:29:11.000000 aifactory-1.7.3/setup.py
+drwxr-xr-x   0 kyj        (501) staff       (20)        0 2023-08-01 01:55:38.343094 aifactory-1.8.0/
+-rw-r--r--   0 kyj        (501) staff       (20)      228 2023-08-01 01:55:38.342848 aifactory-1.8.0/PKG-INFO
+drwxr-xr-x   0 kyj        (501) staff       (20)        0 2023-08-01 01:55:38.341919 aifactory-1.8.0/aifactory/
+-rw-r--r--   0 kyj        (501) staff       (20)        0 2023-05-10 03:11:14.000000 aifactory-1.8.0/aifactory/__init__.py
+-rw-r--r--   0 kyj        (501) staff       (20)     3743 2023-05-10 03:11:14.000000 aifactory-1.8.0/aifactory/api.py
+-rw-r--r--   0 kyj        (501) staff       (20)     3710 2023-05-10 03:11:14.000000 aifactory-1.8.0/aifactory/demo.py
+-rw-r--r--   0 kyj        (501) staff       (20)    14314 2023-05-10 03:11:14.000000 aifactory-1.8.0/aifactory/grade.py
+-rw-r--r--   0 kyj        (501) staff       (20)     5966 2023-05-10 03:11:14.000000 aifactory-1.8.0/aifactory/make_zip.py
+-rw-r--r--   0 kyj        (501) staff       (20)    13391 2023-07-31 08:05:15.000000 aifactory-1.8.0/aifactory/score.py
+-rw-r--r--   0 kyj        (501) staff       (20)       50 2023-05-10 03:11:14.000000 aifactory-1.8.0/aifactory/train.py
+drwxr-xr-x   0 kyj        (501) staff       (20)        0 2023-08-01 01:55:38.342644 aifactory-1.8.0/aifactory.egg-info/
+-rw-r--r--   0 kyj        (501) staff       (20)      228 2023-08-01 01:55:38.000000 aifactory-1.8.0/aifactory.egg-info/PKG-INFO
+-rw-r--r--   0 kyj        (501) staff       (20)      308 2023-08-01 01:55:38.000000 aifactory-1.8.0/aifactory.egg-info/SOURCES.txt
+-rw-r--r--   0 kyj        (501) staff       (20)        1 2023-08-01 01:55:38.000000 aifactory-1.8.0/aifactory.egg-info/dependency_links.txt
+-rw-r--r--   0 kyj        (501) staff       (20)       41 2023-08-01 01:55:38.000000 aifactory-1.8.0/aifactory.egg-info/requires.txt
+-rw-r--r--   0 kyj        (501) staff       (20)       17 2023-08-01 01:55:38.000000 aifactory-1.8.0/aifactory.egg-info/top_level.txt
+-rw-r--r--   0 kyj        (501) staff       (20)       38 2023-08-01 01:55:38.343159 aifactory-1.8.0/setup.cfg
+-rw-r--r--   0 kyj        (501) staff       (20)      430 2023-07-31 08:05:21.000000 aifactory-1.8.0/setup.py
```

### Comparing `aifactory-1.7.3/aifactory/api.py` & `aifactory-1.8.0/aifactory/api.py`

 * *Files identical despite different names*

### Comparing `aifactory-1.7.3/aifactory/demo.py` & `aifactory-1.8.0/aifactory/demo.py`

 * *Files identical despite different names*

### Comparing `aifactory-1.7.3/aifactory/grade.py` & `aifactory-1.8.0/aifactory/grade.py`

 * *Files identical despite different names*

### Comparing `aifactory-1.7.3/aifactory/make_zip.py` & `aifactory-1.8.0/aifactory/make_zip.py`

 * *Files identical despite different names*

