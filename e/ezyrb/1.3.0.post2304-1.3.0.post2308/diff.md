# Comparing `tmp/ezyrb-1.3.0.post2304.tar.gz` & `tmp/ezyrb-1.3.0.post2308.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/EZyRB/EZyRB/dist/.tmp-iyr9jyzt/ezyrb-1.3.0.post2304.tar", last modified: Sat Apr  1 02:51:20 2023, max compression
+gzip compressed data, was "/home/runner/work/EZyRB/EZyRB/dist/.tmp-oi1xmniy/ezyrb-1.3.0.post2308.tar", last modified: Tue Aug  1 02:49:10 2023, max compression
```

## Comparing `ezyrb-1.3.0.post2304.tar` & `ezyrb-1.3.0.post2308.tar`

### file list

```diff
@@ -1,57 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-04-01 02:51:20.000000 ezyrb-1.3.0.post2304/
--rw-r--r--   0 runner    (1001) docker     (116)     1111 2023-04-01 02:51:12.000000 ezyrb-1.3.0.post2304/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (116)     1310 2023-04-01 02:51:20.000000 ezyrb-1.3.0.post2304/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)    14910 2023-04-01 02:51:12.000000 ezyrb-1.3.0.post2304/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-04-01 02:51:20.000000 ezyrb-1.3.0.post2304/ezyrb/
--rw-r--r--   0 runner    (1001) docker     (116)      663 2023-04-01 02:51:12.000000 ezyrb-1.3.0.post2304/ezyrb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     8476 2023-04-01 02:51:12.000000 ezyrb-1.3.0.post2304/ezyrb/ae.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     7395 2023-04-01 02:51:12.000000 ezyrb-1.3.0.post2304/ezyrb/ann.py
--rw-r--r--   0 runner    (1001) docker     (116)      445 2023-04-01 02:51:12.000000 ezyrb-1.3.0.post2304/ezyrb/approximation.py
--rw-r--r--   0 runner    (1001) docker     (116)     5460 2023-04-01 02:51:12.000000 ezyrb-1.3.0.post2304/ezyrb/database.py
--rw-r--r--   0 runner    (1001) docker     (116)     4067 2023-04-01 02:51:12.000000 ezyrb-1.3.0.post2304/ezyrb/gpr.py
--rw-r--r--   0 runner    (1001) docker     (116)      423 2023-04-01 02:51:12.000000 ezyrb-1.3.0.post2304/ezyrb/kneighbors_regressor.py
--rw-r--r--   0 runner    (1001) docker     (116)     2068 2023-04-01 02:51:12.000000 ezyrb-1.3.0.post2304/ezyrb/linear.py
--rw-r--r--   0 runner    (1001) docker     (116)      476 2023-04-01 02:51:12.000000 ezyrb-1.3.0.post2304/ezyrb/meta.py
--rw-r--r--   0 runner    (1001) docker     (116)     1216 2023-04-01 02:51:12.000000 ezyrb-1.3.0.post2304/ezyrb/neighbors_regressor.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-04-01 02:51:20.000000 ezyrb-1.3.0.post2304/ezyrb/parallel/
--rw-r--r--   0 runner    (1001) docker     (116)      625 2023-04-01 02:51:12.000000 ezyrb-1.3.0.post2304/ezyrb/parallel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     9389 2023-04-01 02:51:12.000000 ezyrb-1.3.0.post2304/ezyrb/parallel/ae.py
--rw-r--r--   0 runner    (1001) docker     (116)    20674 2023-04-01 02:51:12.000000 ezyrb-1.3.0.post2304/ezyrb/parallel/ae_eddl.py
--rw-r--r--   0 runner    (1001) docker     (116)     6472 2023-04-01 02:51:12.000000 ezyrb-1.3.0.post2304/ezyrb/parallel/ann.py
--rw-r--r--   0 runner    (1001) docker     (116)      464 2023-04-01 02:51:12.000000 ezyrb-1.3.0.post2304/ezyrb/parallel/approximation.py
--rw-r--r--   0 runner    (1001) docker     (116)     4514 2023-04-01 02:51:12.000000 ezyrb-1.3.0.post2304/ezyrb/parallel/gpr.py
--rw-r--r--   0 runner    (1001) docker     (116)      439 2023-04-01 02:51:12.000000 ezyrb-1.3.0.post2304/ezyrb/parallel/kneighbors_regressor.py
--rw-r--r--   0 runner    (1001) docker     (116)     2847 2023-04-01 02:51:12.000000 ezyrb-1.3.0.post2304/ezyrb/parallel/linear.py
--rw-r--r--   0 runner    (1001) docker     (116)     1698 2023-04-01 02:51:12.000000 ezyrb-1.3.0.post2304/ezyrb/parallel/neighbors_regressor.py
--rw-r--r--   0 runner    (1001) docker     (116)     9942 2023-04-01 02:51:12.000000 ezyrb-1.3.0.post2304/ezyrb/parallel/pod.py
--rw-r--r--   0 runner    (1001) docker     (116)      462 2023-04-01 02:51:12.000000 ezyrb-1.3.0.post2304/ezyrb/parallel/radius_neighbors_regressor.py
--rw-r--r--   0 runner    (1001) docker     (116)     3927 2023-04-01 02:51:12.000000 ezyrb-1.3.0.post2304/ezyrb/parallel/rbf.py
--rw-r--r--   0 runner    (1001) docker     (116)    10333 2023-04-01 02:51:12.000000 ezyrb-1.3.0.post2304/ezyrb/parallel/reducedordermodel.py
--rw-r--r--   0 runner    (1001) docker     (116)      535 2023-04-01 02:51:12.000000 ezyrb-1.3.0.post2304/ezyrb/parallel/reduction.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     8924 2023-04-01 02:51:12.000000 ezyrb-1.3.0.post2304/ezyrb/pod.py
--rw-r--r--   0 runner    (1001) docker     (116)     1700 2023-04-01 02:51:12.000000 ezyrb-1.3.0.post2304/ezyrb/pod_ae.py
--rw-r--r--   0 runner    (1001) docker     (116)      446 2023-04-01 02:51:12.000000 ezyrb-1.3.0.post2304/ezyrb/radius_neighbors_regressor.py
--rw-r--r--   0 runner    (1001) docker     (116)     3483 2023-04-01 02:51:12.000000 ezyrb-1.3.0.post2304/ezyrb/rbf.py
--rw-r--r--   0 runner    (1001) docker     (116)    10778 2023-04-01 02:51:12.000000 ezyrb-1.3.0.post2304/ezyrb/reducedordermodel.py
--rw-r--r--   0 runner    (1001) docker     (116)      512 2023-04-01 02:51:12.000000 ezyrb-1.3.0.post2304/ezyrb/reduction.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-04-01 02:51:20.000000 ezyrb-1.3.0.post2304/ezyrb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     1310 2023-04-01 02:51:20.000000 ezyrb-1.3.0.post2304/ezyrb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1179 2023-04-01 02:51:20.000000 ezyrb-1.3.0.post2304/ezyrb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-04-01 02:51:20.000000 ezyrb-1.3.0.post2304/ezyrb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-04-01 02:51:20.000000 ezyrb-1.3.0.post2304/ezyrb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)      112 2023-04-01 02:51:20.000000 ezyrb-1.3.0.post2304/ezyrb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       12 2023-04-01 02:51:20.000000 ezyrb-1.3.0.post2304/ezyrb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2023-04-01 02:51:20.000000 ezyrb-1.3.0.post2304/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1970 2023-04-01 02:51:12.000000 ezyrb-1.3.0.post2304/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-04-01 02:51:20.000000 ezyrb-1.3.0.post2304/tests/
--rw-r--r--   0 runner    (1001) docker     (116)       40 2023-04-01 02:51:12.000000 ezyrb-1.3.0.post2304/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1743 2023-04-01 02:51:12.000000 ezyrb-1.3.0.post2304/tests/test_ae.py
--rw-r--r--   0 runner    (1001) docker     (116)     5140 2023-04-01 02:51:12.000000 ezyrb-1.3.0.post2304/tests/test_ann.py
--rw-r--r--   0 runner    (1001) docker     (116)     2084 2023-04-01 02:51:12.000000 ezyrb-1.3.0.post2304/tests/test_database.py
--rw-r--r--   0 runner    (1001) docker     (116)     1985 2023-04-01 02:51:12.000000 ezyrb-1.3.0.post2304/tests/test_gpr.py
--rw-r--r--   0 runner    (1001) docker     (116)     2863 2023-04-01 02:51:12.000000 ezyrb-1.3.0.post2304/tests/test_k_neighbors_regressor.py
--rw-r--r--   0 runner    (1001) docker     (116)     2333 2023-04-01 02:51:12.000000 ezyrb-1.3.0.post2304/tests/test_linear.py
--rw-r--r--   0 runner    (1001) docker     (116)     4045 2023-04-01 02:51:12.000000 ezyrb-1.3.0.post2304/tests/test_pod.py
--rw-r--r--   0 runner    (1001) docker     (116)     1149 2023-04-01 02:51:12.000000 ezyrb-1.3.0.post2304/tests/test_podae.py
--rw-r--r--   0 runner    (1001) docker     (116)     2908 2023-04-01 02:51:12.000000 ezyrb-1.3.0.post2304/tests/test_radius_neighbors_regressor.py
--rw-r--r--   0 runner    (1001) docker     (116)     7055 2023-04-01 02:51:12.000000 ezyrb-1.3.0.post2304/tests/test_reducedordermodel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:49:10.000000 ezyrb-1.3.0.post2308/
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-08-01 02:48:58.000000 ezyrb-1.3.0.post2308/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-08-01 02:49:10.000000 ezyrb-1.3.0.post2308/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14910 2023-08-01 02:48:58.000000 ezyrb-1.3.0.post2308/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:49:10.000000 ezyrb-1.3.0.post2308/ezyrb/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-08-01 02:48:58.000000 ezyrb-1.3.0.post2308/ezyrb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8476 2023-08-01 02:48:58.000000 ezyrb-1.3.0.post2308/ezyrb/ae.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7395 2023-08-01 02:48:58.000000 ezyrb-1.3.0.post2308/ezyrb/ann.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-08-01 02:48:58.000000 ezyrb-1.3.0.post2308/ezyrb/approximation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-08-01 02:48:58.000000 ezyrb-1.3.0.post2308/ezyrb/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-08-01 02:48:58.000000 ezyrb-1.3.0.post2308/ezyrb/gpr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-08-01 02:48:58.000000 ezyrb-1.3.0.post2308/ezyrb/kneighbors_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-08-01 02:48:58.000000 ezyrb-1.3.0.post2308/ezyrb/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-08-01 02:48:58.000000 ezyrb-1.3.0.post2308/ezyrb/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-08-01 02:48:58.000000 ezyrb-1.3.0.post2308/ezyrb/neighbors_regressor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:49:10.000000 ezyrb-1.3.0.post2308/ezyrb/parallel/
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-08-01 02:48:58.000000 ezyrb-1.3.0.post2308/ezyrb/parallel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9389 2023-08-01 02:48:58.000000 ezyrb-1.3.0.post2308/ezyrb/parallel/ae.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20674 2023-08-01 02:48:58.000000 ezyrb-1.3.0.post2308/ezyrb/parallel/ae_eddl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-08-01 02:48:58.000000 ezyrb-1.3.0.post2308/ezyrb/parallel/ann.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-08-01 02:48:58.000000 ezyrb-1.3.0.post2308/ezyrb/parallel/approximation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-08-01 02:48:58.000000 ezyrb-1.3.0.post2308/ezyrb/parallel/gpr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-08-01 02:48:58.000000 ezyrb-1.3.0.post2308/ezyrb/parallel/kneighbors_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-08-01 02:48:58.000000 ezyrb-1.3.0.post2308/ezyrb/parallel/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-08-01 02:48:58.000000 ezyrb-1.3.0.post2308/ezyrb/parallel/neighbors_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9942 2023-08-01 02:48:58.000000 ezyrb-1.3.0.post2308/ezyrb/parallel/pod.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-08-01 02:48:58.000000 ezyrb-1.3.0.post2308/ezyrb/parallel/radius_neighbors_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-08-01 02:48:58.000000 ezyrb-1.3.0.post2308/ezyrb/parallel/rbf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10333 2023-08-01 02:48:58.000000 ezyrb-1.3.0.post2308/ezyrb/parallel/reducedordermodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-08-01 02:48:58.000000 ezyrb-1.3.0.post2308/ezyrb/parallel/reduction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8924 2023-08-01 02:48:58.000000 ezyrb-1.3.0.post2308/ezyrb/pod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-08-01 02:48:58.000000 ezyrb-1.3.0.post2308/ezyrb/pod_ae.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-08-01 02:48:58.000000 ezyrb-1.3.0.post2308/ezyrb/radius_neighbors_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-08-01 02:48:58.000000 ezyrb-1.3.0.post2308/ezyrb/rbf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10778 2023-08-01 02:48:58.000000 ezyrb-1.3.0.post2308/ezyrb/reducedordermodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-08-01 02:48:58.000000 ezyrb-1.3.0.post2308/ezyrb/reduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-08-01 02:48:58.000000 ezyrb-1.3.0.post2308/ezyrb/regular_grid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:49:10.000000 ezyrb-1.3.0.post2308/ezyrb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-08-01 02:49:10.000000 ezyrb-1.3.0.post2308/ezyrb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-08-01 02:49:10.000000 ezyrb-1.3.0.post2308/ezyrb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 02:49:10.000000 ezyrb-1.3.0.post2308/ezyrb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 02:49:10.000000 ezyrb-1.3.0.post2308/ezyrb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-08-01 02:49:10.000000 ezyrb-1.3.0.post2308/ezyrb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-01 02:49:10.000000 ezyrb-1.3.0.post2308/ezyrb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 02:49:10.000000 ezyrb-1.3.0.post2308/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-08-01 02:48:58.000000 ezyrb-1.3.0.post2308/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:49:10.000000 ezyrb-1.3.0.post2308/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-01 02:48:58.000000 ezyrb-1.3.0.post2308/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-08-01 02:48:58.000000 ezyrb-1.3.0.post2308/tests/test_ae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5140 2023-08-01 02:48:58.000000 ezyrb-1.3.0.post2308/tests/test_ann.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-08-01 02:48:58.000000 ezyrb-1.3.0.post2308/tests/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-08-01 02:48:58.000000 ezyrb-1.3.0.post2308/tests/test_gpr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-08-01 02:48:58.000000 ezyrb-1.3.0.post2308/tests/test_k_neighbors_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-08-01 02:48:58.000000 ezyrb-1.3.0.post2308/tests/test_linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-08-01 02:48:58.000000 ezyrb-1.3.0.post2308/tests/test_pod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-08-01 02:48:58.000000 ezyrb-1.3.0.post2308/tests/test_podae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-08-01 02:48:58.000000 ezyrb-1.3.0.post2308/tests/test_radius_neighbors_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-08-01 02:48:58.000000 ezyrb-1.3.0.post2308/tests/test_reducedordermodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-08-01 02:48:58.000000 ezyrb-1.3.0.post2308/tests/test_regular_grid.py
```

### Comparing `ezyrb-1.3.0.post2304/LICENSE.rst` & `ezyrb-1.3.0.post2308/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `ezyrb-1.3.0.post2304/PKG-INFO` & `ezyrb-1.3.0.post2308/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezyrb
-Version: 1.3.0.post2304
+Version: 1.3.0.post2308
 Summary: Easy Reduced Basis
 Home-page: https://github.com/mathLab/EZyRB
 Author: Nicola Demo, Marco Tezzele
 Author-email: demo.nicola@gmail.com, marcotez@gmail.com
 License: MIT
 Keywords: pod interpolation reduced-basis model-order-reduction
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ezyrb-1.3.0.post2304/README.md` & `ezyrb-1.3.0.post2308/README.md`

 * *Files identical despite different names*

### Comparing `ezyrb-1.3.0.post2304/ezyrb/__init__.py` & `ezyrb-1.3.0.post2308/ezyrb/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """EZyRB package"""
 
 __all__ = [
     'Database', 'Reduction', 'POD', 'Approximation', 'RBF', 'Linear', 'GPR',
     'ANN', 'KNeighborsRegressor', 'RadiusNeighborsRegressor', 'AE',
-    'ReducedOrderModel', 'PODAE'
+    'ReducedOrderModel', 'PODAE', 'RegularGrid'
 ]
 
 from .meta import *
 from .database import Database
 from .reduction import Reduction
 from .pod import POD
 from .ae import AE
 from .pod_ae import PODAE
 from .approximation import Approximation
 from .rbf import RBF
 from .linear import Linear
+from .regular_grid import RegularGrid
 from .gpr import GPR
 from .reducedordermodel import ReducedOrderModel
 from .ann import ANN
 from .kneighbors_regressor import KNeighborsRegressor
 from .radius_neighbors_regressor import RadiusNeighborsRegressor
```

### Comparing `ezyrb-1.3.0.post2304/ezyrb/ae.py` & `ezyrb-1.3.0.post2308/ezyrb/ae.py`

 * *Files identical despite different names*

### Comparing `ezyrb-1.3.0.post2304/ezyrb/ann.py` & `ezyrb-1.3.0.post2308/ezyrb/ann.py`

 * *Files identical despite different names*

### Comparing `ezyrb-1.3.0.post2304/ezyrb/database.py` & `ezyrb-1.3.0.post2308/ezyrb/database.py`

 * *Files identical despite different names*

### Comparing `ezyrb-1.3.0.post2304/ezyrb/gpr.py` & `ezyrb-1.3.0.post2308/ezyrb/gpr.py`

 * *Files identical despite different names*

### Comparing `ezyrb-1.3.0.post2304/ezyrb/linear.py` & `ezyrb-1.3.0.post2308/ezyrb/linear.py`

 * *Files identical despite different names*

### Comparing `ezyrb-1.3.0.post2304/ezyrb/neighbors_regressor.py` & `ezyrb-1.3.0.post2308/ezyrb/neighbors_regressor.py`

 * *Files identical despite different names*

### Comparing `ezyrb-1.3.0.post2304/ezyrb/parallel/__init__.py` & `ezyrb-1.3.0.post2308/ezyrb/parallel/__init__.py`

 * *Files identical despite different names*

### Comparing `ezyrb-1.3.0.post2304/ezyrb/parallel/ae.py` & `ezyrb-1.3.0.post2308/ezyrb/parallel/ae.py`

 * *Files identical despite different names*

### Comparing `ezyrb-1.3.0.post2304/ezyrb/parallel/ae_eddl.py` & `ezyrb-1.3.0.post2308/ezyrb/parallel/ae_eddl.py`

 * *Files identical despite different names*

### Comparing `ezyrb-1.3.0.post2304/ezyrb/parallel/ann.py` & `ezyrb-1.3.0.post2308/ezyrb/parallel/ann.py`

 * *Files identical despite different names*

### Comparing `ezyrb-1.3.0.post2304/ezyrb/parallel/gpr.py` & `ezyrb-1.3.0.post2308/ezyrb/parallel/gpr.py`

 * *Files identical despite different names*

### Comparing `ezyrb-1.3.0.post2304/ezyrb/parallel/linear.py` & `ezyrb-1.3.0.post2308/ezyrb/parallel/linear.py`

 * *Files identical despite different names*

### Comparing `ezyrb-1.3.0.post2304/ezyrb/parallel/neighbors_regressor.py` & `ezyrb-1.3.0.post2308/ezyrb/parallel/neighbors_regressor.py`

 * *Files identical despite different names*

### Comparing `ezyrb-1.3.0.post2304/ezyrb/parallel/pod.py` & `ezyrb-1.3.0.post2308/ezyrb/parallel/pod.py`

 * *Files identical despite different names*

### Comparing `ezyrb-1.3.0.post2304/ezyrb/parallel/rbf.py` & `ezyrb-1.3.0.post2308/ezyrb/parallel/rbf.py`

 * *Files identical despite different names*

### Comparing `ezyrb-1.3.0.post2304/ezyrb/parallel/reducedordermodel.py` & `ezyrb-1.3.0.post2308/ezyrb/parallel/reducedordermodel.py`

 * *Files identical despite different names*

### Comparing `ezyrb-1.3.0.post2304/ezyrb/parallel/reduction.py` & `ezyrb-1.3.0.post2308/ezyrb/parallel/reduction.py`

 * *Files identical despite different names*

### Comparing `ezyrb-1.3.0.post2304/ezyrb/pod.py` & `ezyrb-1.3.0.post2308/ezyrb/pod.py`

 * *Files identical despite different names*

### Comparing `ezyrb-1.3.0.post2304/ezyrb/pod_ae.py` & `ezyrb-1.3.0.post2308/ezyrb/pod_ae.py`

 * *Files identical despite different names*

### Comparing `ezyrb-1.3.0.post2304/ezyrb/rbf.py` & `ezyrb-1.3.0.post2308/ezyrb/rbf.py`

 * *Files identical despite different names*

### Comparing `ezyrb-1.3.0.post2304/ezyrb/reducedordermodel.py` & `ezyrb-1.3.0.post2308/ezyrb/reducedordermodel.py`

 * *Files identical despite different names*

### Comparing `ezyrb-1.3.0.post2304/ezyrb/reduction.py` & `ezyrb-1.3.0.post2308/ezyrb/reduction.py`

 * *Files identical despite different names*

### Comparing `ezyrb-1.3.0.post2304/ezyrb.egg-info/PKG-INFO` & `ezyrb-1.3.0.post2308/ezyrb.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezyrb
-Version: 1.3.0.post2304
+Version: 1.3.0.post2308
 Summary: Easy Reduced Basis
 Home-page: https://github.com/mathLab/EZyRB
 Author: Nicola Demo, Marco Tezzele
 Author-email: demo.nicola@gmail.com, marcotez@gmail.com
 License: MIT
 Keywords: pod interpolation reduced-basis model-order-reduction
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ezyrb-1.3.0.post2304/ezyrb.egg-info/SOURCES.txt` & `ezyrb-1.3.0.post2308/ezyrb.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 ezyrb/neighbors_regressor.py
 ezyrb/pod.py
 ezyrb/pod_ae.py
 ezyrb/radius_neighbors_regressor.py
 ezyrb/rbf.py
 ezyrb/reducedordermodel.py
 ezyrb/reduction.py
+ezyrb/regular_grid.py
 ezyrb.egg-info/PKG-INFO
 ezyrb.egg-info/SOURCES.txt
 ezyrb.egg-info/dependency_links.txt
 ezyrb.egg-info/not-zip-safe
 ezyrb.egg-info/requires.txt
 ezyrb.egg-info/top_level.txt
 ezyrb/parallel/__init__.py
@@ -43,8 +44,9 @@
 tests/test_database.py
 tests/test_gpr.py
 tests/test_k_neighbors_regressor.py
 tests/test_linear.py
 tests/test_pod.py
 tests/test_podae.py
 tests/test_radius_neighbors_regressor.py
-tests/test_reducedordermodel.py
+tests/test_reducedordermodel.py
+tests/test_regular_grid.py
```

### Comparing `ezyrb-1.3.0.post2304/setup.py` & `ezyrb-1.3.0.post2308/setup.py`

 * *Files identical despite different names*

### Comparing `ezyrb-1.3.0.post2304/tests/test_ae.py` & `ezyrb-1.3.0.post2308/tests/test_ae.py`

 * *Files identical despite different names*

### Comparing `ezyrb-1.3.0.post2304/tests/test_ann.py` & `ezyrb-1.3.0.post2308/tests/test_ann.py`

 * *Files identical despite different names*

### Comparing `ezyrb-1.3.0.post2304/tests/test_database.py` & `ezyrb-1.3.0.post2308/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `ezyrb-1.3.0.post2304/tests/test_gpr.py` & `ezyrb-1.3.0.post2308/tests/test_gpr.py`

 * *Files identical despite different names*

### Comparing `ezyrb-1.3.0.post2304/tests/test_k_neighbors_regressor.py` & `ezyrb-1.3.0.post2308/tests/test_k_neighbors_regressor.py`

 * *Files identical despite different names*

### Comparing `ezyrb-1.3.0.post2304/tests/test_linear.py` & `ezyrb-1.3.0.post2308/tests/test_linear.py`

 * *Files identical despite different names*

### Comparing `ezyrb-1.3.0.post2304/tests/test_pod.py` & `ezyrb-1.3.0.post2308/tests/test_pod.py`

 * *Files identical despite different names*

### Comparing `ezyrb-1.3.0.post2304/tests/test_podae.py` & `ezyrb-1.3.0.post2308/tests/test_podae.py`

 * *Files identical despite different names*

### Comparing `ezyrb-1.3.0.post2304/tests/test_radius_neighbors_regressor.py` & `ezyrb-1.3.0.post2308/tests/test_radius_neighbors_regressor.py`

 * *Files identical despite different names*

### Comparing `ezyrb-1.3.0.post2304/tests/test_reducedordermodel.py` & `ezyrb-1.3.0.post2308/tests/test_reducedordermodel.py`

 * *Files identical despite different names*

