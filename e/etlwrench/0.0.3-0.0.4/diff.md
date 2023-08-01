# Comparing `tmp/etlwrench-0.0.3.tar.gz` & `tmp/etlwrench-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etlwrench-0.0.3.tar", last modified: Tue Aug  1 03:50:08 2023, max compression
+gzip compressed data, was "etlwrench-0.0.4.tar", last modified: Tue Aug  1 12:50:48 2023, max compression
```

## Comparing `etlwrench-0.0.3.tar` & `etlwrench-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 gabecordovado   (501) staff       (20)        0 2023-08-01 03:50:08.595431 etlwrench-0.0.3/
--rw-r--r--   0 gabecordovado   (501) staff       (20)     1074 2023-08-01 03:20:50.000000 etlwrench-0.0.3/LICENSE
--rw-r--r--   0 gabecordovado   (501) staff       (20)      321 2023-08-01 03:50:08.595754 etlwrench-0.0.3/PKG-INFO
-drwxr-xr-x   0 gabecordovado   (501) staff       (20)        0 2023-08-01 03:50:08.594728 etlwrench-0.0.3/etlwrench.egg-info/
--rw-r--r--   0 gabecordovado   (501) staff       (20)      321 2023-08-01 03:50:08.000000 etlwrench-0.0.3/etlwrench.egg-info/PKG-INFO
--rw-r--r--   0 gabecordovado   (501) staff       (20)      205 2023-08-01 03:50:08.000000 etlwrench-0.0.3/etlwrench.egg-info/SOURCES.txt
--rw-r--r--   0 gabecordovado   (501) staff       (20)        1 2023-08-01 03:50:08.000000 etlwrench-0.0.3/etlwrench.egg-info/dependency_links.txt
--rw-r--r--   0 gabecordovado   (501) staff       (20)        9 2023-08-01 03:50:08.000000 etlwrench-0.0.3/etlwrench.egg-info/requires.txt
--rw-r--r--   0 gabecordovado   (501) staff       (20)        1 2023-08-01 03:50:08.000000 etlwrench-0.0.3/etlwrench.egg-info/top_level.txt
--rw-r--r--   0 gabecordovado   (501) staff       (20)       86 2023-07-31 02:50:48.000000 etlwrench-0.0.3/pyproject.toml
--rw-r--r--   0 gabecordovado   (501) staff       (20)      437 2023-08-01 03:50:08.596631 etlwrench-0.0.3/setup.cfg
--rw-r--r--   0 gabecordovado   (501) staff       (20)       36 2023-07-31 03:32:30.000000 etlwrench-0.0.3/setup.py
+drwxr-xr-x   0 gabecordovado   (501) staff       (20)        0 2023-08-01 12:50:48.877600 etlwrench-0.0.4/
+-rw-r--r--   0 gabecordovado   (501) staff       (20)     1074 2023-08-01 03:20:50.000000 etlwrench-0.0.4/LICENSE
+-rw-r--r--   0 gabecordovado   (501) staff       (20)      321 2023-08-01 12:50:48.877878 etlwrench-0.0.4/PKG-INFO
+drwxr-xr-x   0 gabecordovado   (501) staff       (20)        0 2023-08-01 12:50:48.877042 etlwrench-0.0.4/etlwrench.egg-info/
+-rw-r--r--   0 gabecordovado   (501) staff       (20)      321 2023-08-01 12:50:48.000000 etlwrench-0.0.4/etlwrench.egg-info/PKG-INFO
+-rw-r--r--   0 gabecordovado   (501) staff       (20)      205 2023-08-01 12:50:48.000000 etlwrench-0.0.4/etlwrench.egg-info/SOURCES.txt
+-rw-r--r--   0 gabecordovado   (501) staff       (20)        1 2023-08-01 12:50:48.000000 etlwrench-0.0.4/etlwrench.egg-info/dependency_links.txt
+-rw-r--r--   0 gabecordovado   (501) staff       (20)        9 2023-08-01 12:50:48.000000 etlwrench-0.0.4/etlwrench.egg-info/requires.txt
+-rw-r--r--   0 gabecordovado   (501) staff       (20)        1 2023-08-01 12:50:48.000000 etlwrench-0.0.4/etlwrench.egg-info/top_level.txt
+-rw-r--r--   0 gabecordovado   (501) staff       (20)       86 2023-07-31 02:50:48.000000 etlwrench-0.0.4/pyproject.toml
+-rw-r--r--   0 gabecordovado   (501) staff       (20)      437 2023-08-01 12:50:48.878922 etlwrench-0.0.4/setup.cfg
+-rw-r--r--   0 gabecordovado   (501) staff       (20)       36 2023-07-31 03:32:30.000000 etlwrench-0.0.4/setup.py
```

### Comparing `etlwrench-0.0.3/LICENSE` & `etlwrench-0.0.4/LICENSE`

 * *Files identical despite different names*

