# Comparing `tmp/etlwrench-0.0.1.tar.gz` & `tmp/etlwrench-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etlwrench-0.0.1.tar", last modified: Tue Aug  1 03:21:03 2023, max compression
+gzip compressed data, was "etlwrench-0.0.2.tar", last modified: Tue Aug  1 03:42:32 2023, max compression
```

## Comparing `etlwrench-0.0.1.tar` & `etlwrench-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 gabecordovado   (501) staff       (20)        0 2023-08-01 03:21:03.555056 etlwrench-0.0.1/
--rw-r--r--   0 gabecordovado   (501) staff       (20)     1074 2023-08-01 03:20:50.000000 etlwrench-0.0.1/LICENSE
--rw-r--r--   0 gabecordovado   (501) staff       (20)      245 2023-08-01 03:21:03.555228 etlwrench-0.0.1/PKG-INFO
-drwxr-xr-x   0 gabecordovado   (501) staff       (20)        0 2023-08-01 03:21:03.554064 etlwrench-0.0.1/etlwrench.egg-info/
--rw-r--r--   0 gabecordovado   (501) staff       (20)      245 2023-08-01 03:21:03.000000 etlwrench-0.0.1/etlwrench.egg-info/PKG-INFO
--rw-r--r--   0 gabecordovado   (501) staff       (20)      205 2023-08-01 03:21:03.000000 etlwrench-0.0.1/etlwrench.egg-info/SOURCES.txt
--rw-r--r--   0 gabecordovado   (501) staff       (20)        1 2023-08-01 03:21:03.000000 etlwrench-0.0.1/etlwrench.egg-info/dependency_links.txt
--rw-r--r--   0 gabecordovado   (501) staff       (20)        9 2023-08-01 03:21:03.000000 etlwrench-0.0.1/etlwrench.egg-info/requires.txt
--rw-r--r--   0 gabecordovado   (501) staff       (20)        1 2023-08-01 03:21:03.000000 etlwrench-0.0.1/etlwrench.egg-info/top_level.txt
--rw-r--r--   0 gabecordovado   (501) staff       (20)       86 2023-07-31 02:50:48.000000 etlwrench-0.0.1/pyproject.toml
--rw-r--r--   0 gabecordovado   (501) staff       (20)      345 2023-08-01 03:21:03.556534 etlwrench-0.0.1/setup.cfg
--rw-r--r--   0 gabecordovado   (501) staff       (20)       36 2023-07-31 03:32:30.000000 etlwrench-0.0.1/setup.py
+drwxr-xr-x   0 gabecordovado   (501) staff       (20)        0 2023-08-01 03:42:32.834693 etlwrench-0.0.2/
+-rw-r--r--   0 gabecordovado   (501) staff       (20)     1074 2023-08-01 03:20:50.000000 etlwrench-0.0.2/LICENSE
+-rw-r--r--   0 gabecordovado   (501) staff       (20)      245 2023-08-01 03:42:32.834877 etlwrench-0.0.2/PKG-INFO
+drwxr-xr-x   0 gabecordovado   (501) staff       (20)        0 2023-08-01 03:42:32.834165 etlwrench-0.0.2/etlwrench.egg-info/
+-rw-r--r--   0 gabecordovado   (501) staff       (20)      245 2023-08-01 03:42:32.000000 etlwrench-0.0.2/etlwrench.egg-info/PKG-INFO
+-rw-r--r--   0 gabecordovado   (501) staff       (20)      205 2023-08-01 03:42:32.000000 etlwrench-0.0.2/etlwrench.egg-info/SOURCES.txt
+-rw-r--r--   0 gabecordovado   (501) staff       (20)        1 2023-08-01 03:42:32.000000 etlwrench-0.0.2/etlwrench.egg-info/dependency_links.txt
+-rw-r--r--   0 gabecordovado   (501) staff       (20)        9 2023-08-01 03:42:32.000000 etlwrench-0.0.2/etlwrench.egg-info/requires.txt
+-rw-r--r--   0 gabecordovado   (501) staff       (20)        1 2023-08-01 03:42:32.000000 etlwrench-0.0.2/etlwrench.egg-info/top_level.txt
+-rw-r--r--   0 gabecordovado   (501) staff       (20)       86 2023-07-31 02:50:48.000000 etlwrench-0.0.2/pyproject.toml
+-rw-r--r--   0 gabecordovado   (501) staff       (20)      346 2023-08-01 03:42:32.835546 etlwrench-0.0.2/setup.cfg
+-rw-r--r--   0 gabecordovado   (501) staff       (20)       36 2023-07-31 03:32:30.000000 etlwrench-0.0.2/setup.py
```

### Comparing `etlwrench-0.0.1/LICENSE` & `etlwrench-0.0.2/LICENSE`

 * *Files identical despite different names*

