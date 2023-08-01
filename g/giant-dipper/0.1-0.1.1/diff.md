# Comparing `tmp/giant-dipper-0.1.tar.gz` & `tmp/giant-dipper-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "giant-dipper-0.1.tar", last modified: Tue Aug  1 19:54:52 2023, max compression
+gzip compressed data, was "giant-dipper-0.1.1.tar", last modified: Tue Aug  1 20:19:37 2023, max compression
```

## Comparing `giant-dipper-0.1.tar` & `giant-dipper-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:54:52.215505 giant-dipper-0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-01 19:54:42.000000 giant-dipper-0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-08-01 19:54:52.215505 giant-dipper-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16591 2023-08-01 19:54:42.000000 giant-dipper-0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:54:52.211505 giant-dipper-0.1/giant-dipper/
--rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-08-01 19:54:42.000000 giant-dipper-0.1/giant-dipper/GiantDipper.py
--rw-r--r--   0 runner    (1001) docker     (123)    21186 2023-08-01 19:54:42.000000 giant-dipper-0.1/giant-dipper/OrderManager.py
--rw-r--r--   0 runner    (1001) docker     (123)    12691 2023-08-01 19:54:42.000000 giant-dipper-0.1/giant-dipper/OrderServices.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-01 19:54:42.000000 giant-dipper-0.1/giant-dipper/OrderSides.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-08-01 19:54:42.000000 giant-dipper-0.1/giant-dipper/OrderStatuses.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-08-01 19:54:42.000000 giant-dipper-0.1/giant-dipper/RobinHoodAuth.py
--rw-r--r--   0 runner    (1001) docker     (123)     8622 2023-08-01 19:54:42.000000 giant-dipper-0.1/giant-dipper/StateManagers.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 19:54:42.000000 giant-dipper-0.1/giant-dipper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:54:52.215505 giant-dipper-0.1/giant_dipper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-08-01 19:54:52.000000 giant-dipper-0.1/giant_dipper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-08-01 19:54:52.000000 giant-dipper-0.1/giant_dipper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 19:54:52.000000 giant-dipper-0.1/giant_dipper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-01 19:54:52.000000 giant-dipper-0.1/giant_dipper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-01 19:54:52.215505 giant-dipper-0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-08-01 19:54:42.000000 giant-dipper-0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:19:37.686559 giant-dipper-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-01 20:19:27.000000 giant-dipper-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17000 2023-08-01 20:19:37.686559 giant-dipper-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16591 2023-08-01 20:19:27.000000 giant-dipper-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:19:37.686559 giant-dipper-0.1.1/giant-dipper/
+-rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-08-01 20:19:27.000000 giant-dipper-0.1.1/giant-dipper/GiantDipper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21186 2023-08-01 20:19:27.000000 giant-dipper-0.1.1/giant-dipper/OrderManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12691 2023-08-01 20:19:27.000000 giant-dipper-0.1.1/giant-dipper/OrderServices.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-01 20:19:27.000000 giant-dipper-0.1.1/giant-dipper/OrderSides.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-08-01 20:19:27.000000 giant-dipper-0.1.1/giant-dipper/OrderStatuses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-08-01 20:19:27.000000 giant-dipper-0.1.1/giant-dipper/RobinHoodAuth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8622 2023-08-01 20:19:27.000000 giant-dipper-0.1.1/giant-dipper/StateManagers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:19:27.000000 giant-dipper-0.1.1/giant-dipper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:19:37.686559 giant-dipper-0.1.1/giant_dipper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17000 2023-08-01 20:19:37.000000 giant-dipper-0.1.1/giant_dipper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-08-01 20:19:37.000000 giant-dipper-0.1.1/giant_dipper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 20:19:37.000000 giant-dipper-0.1.1/giant_dipper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-01 20:19:37.000000 giant-dipper-0.1.1/giant_dipper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-01 20:19:37.000000 giant-dipper-0.1.1/giant_dipper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-01 20:19:37.686559 giant-dipper-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-08-01 20:19:27.000000 giant-dipper-0.1.1/setup.py
```

### Comparing `giant-dipper-0.1/LICENSE` & `giant-dipper-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `giant-dipper-0.1/README.md` & `giant-dipper-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `giant-dipper-0.1/giant-dipper/GiantDipper.py` & `giant-dipper-0.1.1/giant-dipper/GiantDipper.py`

 * *Files identical despite different names*

### Comparing `giant-dipper-0.1/giant-dipper/OrderManager.py` & `giant-dipper-0.1.1/giant-dipper/OrderManager.py`

 * *Files identical despite different names*

### Comparing `giant-dipper-0.1/giant-dipper/OrderServices.py` & `giant-dipper-0.1.1/giant-dipper/OrderServices.py`

 * *Files identical despite different names*

### Comparing `giant-dipper-0.1/giant-dipper/RobinHoodAuth.py` & `giant-dipper-0.1.1/giant-dipper/RobinHoodAuth.py`

 * *Files identical despite different names*

### Comparing `giant-dipper-0.1/giant-dipper/StateManagers.py` & `giant-dipper-0.1.1/giant-dipper/StateManagers.py`

 * *Files identical despite different names*

