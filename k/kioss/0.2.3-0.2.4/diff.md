# Comparing `tmp/kioss-0.2.3.tar.gz` & `tmp/kioss-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kioss-0.2.3.tar", last modified: Tue Aug  1 00:06:00 2023, max compression
+gzip compressed data, was "kioss-0.2.4.tar", last modified: Tue Aug  1 00:06:56 2023, max compression
```

## Comparing `kioss-0.2.3.tar` & `kioss-0.2.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:06:00.465623 kioss-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-01 00:05:46.000000 kioss-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-08-01 00:06:00.465623 kioss-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-08-01 00:05:46.000000 kioss-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:06:00.465623 kioss-0.2.3/kioss/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-01 00:05:46.000000 kioss-0.2.3/kioss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18474 2023-08-01 00:05:46.000000 kioss-0.2.3/kioss/pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-08-01 00:05:46.000000 kioss-0.2.3/kioss/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:06:00.465623 kioss-0.2.3/kioss.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-08-01 00:06:00.000000 kioss-0.2.3/kioss.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-08-01 00:06:00.000000 kioss-0.2.3/kioss.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 00:06:00.000000 kioss-0.2.3/kioss.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-01 00:06:00.000000 kioss-0.2.3/kioss.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 00:06:00.465623 kioss-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-08-01 00:05:46.000000 kioss-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:06:00.465623 kioss-0.2.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)    11258 2023-08-01 00:05:46.000000 kioss-0.2.3/test/test_pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-08-01 00:05:46.000000 kioss-0.2.3/test/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:06:56.626949 kioss-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-01 00:06:44.000000 kioss-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-08-01 00:06:56.626949 kioss-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-08-01 00:06:44.000000 kioss-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:06:56.622949 kioss-0.2.4/kioss/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-01 00:06:44.000000 kioss-0.2.4/kioss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18474 2023-08-01 00:06:44.000000 kioss-0.2.4/kioss/pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-08-01 00:06:44.000000 kioss-0.2.4/kioss/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:06:56.622949 kioss-0.2.4/kioss.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-08-01 00:06:56.000000 kioss-0.2.4/kioss.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-08-01 00:06:56.000000 kioss-0.2.4/kioss.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 00:06:56.000000 kioss-0.2.4/kioss.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-01 00:06:56.000000 kioss-0.2.4/kioss.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 00:06:56.626949 kioss-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-08-01 00:06:44.000000 kioss-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:06:56.622949 kioss-0.2.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    11258 2023-08-01 00:06:44.000000 kioss-0.2.4/test/test_pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-08-01 00:06:44.000000 kioss-0.2.4/test/test_util.py
```

### Comparing `kioss-0.2.3/LICENSE` & `kioss-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `kioss-0.2.3/README.md` & `kioss-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `kioss-0.2.3/kioss/pipe.py` & `kioss-0.2.4/kioss/pipe.py`

 * *Files identical despite different names*

### Comparing `kioss-0.2.3/kioss/util.py` & `kioss-0.2.4/kioss/util.py`

 * *Files identical despite different names*

### Comparing `kioss-0.2.3/test/test_pipe.py` & `kioss-0.2.4/test/test_pipe.py`

 * *Files identical despite different names*

### Comparing `kioss-0.2.3/test/test_util.py` & `kioss-0.2.4/test/test_util.py`

 * *Files identical despite different names*

