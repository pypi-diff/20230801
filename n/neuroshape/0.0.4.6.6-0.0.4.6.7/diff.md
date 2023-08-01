# Comparing `tmp/neuroshape-0.0.4.6.6.tar.gz` & `tmp/neuroshape-0.0.4.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuroshape-0.0.4.6.6.tar", last modified: Tue Jul 11 01:49:03 2023, max compression
+gzip compressed data, was "neuroshape-0.0.4.6.7.tar", last modified: Tue Aug  1 04:57:41 2023, max compression
```

## Comparing `neuroshape-0.0.4.6.6.tar` & `neuroshape-0.0.4.6.7.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 c3336955   (503) staff       (20)        0 2023-07-11 01:49:03.211407 neuroshape-0.0.4.6.6/
--rw-r--r--   0 c3336955   (503) staff       (20)     1501 2023-06-07 11:17:25.000000 neuroshape-0.0.4.6.6/LICENSE
--rw-r--r--   0 c3336955   (503) staff       (20)     6795 2023-07-11 01:49:03.210956 neuroshape-0.0.4.6.6/PKG-INFO
--rw-r--r--   0 c3336955   (503) staff       (20)     4445 2023-06-08 03:48:59.000000 neuroshape-0.0.4.6.6/README.rst
-drwxr-xr-x   0 c3336955   (503) staff       (20)        0 2023-07-11 01:49:03.183672 neuroshape-0.0.4.6.6/neuroshape/
--rw-r--r--   0 c3336955   (503) staff       (20)        0 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.6/neuroshape/__init__.py
--rw-r--r--   0 c3336955   (503) staff       (20)    22407 2023-06-16 11:25:08.000000 neuroshape-0.0.4.6.6/neuroshape/connectopic_laplacian.py
--rw-r--r--   0 c3336955   (503) staff       (20)    22913 2023-07-04 03:05:38.000000 neuroshape-0.0.4.6.6/neuroshape/eigenmodes.py
-drwxr-xr-x   0 c3336955   (503) staff       (20)        0 2023-07-11 01:49:03.196157 neuroshape-0.0.4.6.6/neuroshape/nulls/
--rw-r--r--   0 c3336955   (503) staff       (20)       44 2023-06-08 03:48:59.000000 neuroshape-0.0.4.6.6/neuroshape/nulls/__init__.py
--rw-r--r--   0 c3336955   (503) staff       (20)     5351 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.6/neuroshape/nulls/burt.py
--rw-r--r--   0 c3336955   (503) staff       (20)    20808 2023-06-13 01:26:03.000000 neuroshape-0.0.4.6.6/neuroshape/nulls/eigenshuff.py
--rw-r--r--   0 c3336955   (503) staff       (20)    15998 2023-06-28 22:07:04.000000 neuroshape-0.0.4.6.6/neuroshape/nulls/eigensphere.py
--rw-r--r--   0 c3336955   (503) staff       (20)    25239 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.6/neuroshape/nulls/nulls.py
--rw-r--r--   0 c3336955   (503) staff       (20)    27669 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.6/neuroshape/nulls/spins.py
-drwxr-xr-x   0 c3336955   (503) staff       (20)        0 2023-07-11 01:49:03.199159 neuroshape-0.0.4.6.6/neuroshape/nulls/tests/
--rw-r--r--   0 c3336955   (503) staff       (20)        0 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.6/neuroshape/nulls/tests/__init__.py
--rw-r--r--   0 c3336955   (503) staff       (20)     5042 2023-06-19 22:07:48.000000 neuroshape-0.0.4.6.6/neuroshape/nulls/tests/eigenmode_replication.py
--rw-r--r--   0 c3336955   (503) staff       (20)      530 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.6/neuroshape/nulls/tests/test_burt.py
--rw-r--r--   0 c3336955   (503) staff       (20)     4137 2023-06-19 22:07:48.000000 neuroshape-0.0.4.6.6/neuroshape/nulls/tests/test_eigenresamp.py
--rw-r--r--   0 c3336955   (503) staff       (20)      695 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.6/neuroshape/nulls/tests/test_nulls.py
--rw-r--r--   0 c3336955   (503) staff       (20)      814 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.6/neuroshape/nulls/tests/test_spins.py
--rw-r--r--   0 c3336955   (503) staff       (20)    12845 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.6/neuroshape/nulls/waveshuff.py
--rw-r--r--   0 c3336955   (503) staff       (20)     4078 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.6/neuroshape/permutation.py
--rw-r--r--   0 c3336955   (503) staff       (20)    13180 2023-06-18 23:49:14.000000 neuroshape-0.0.4.6.6/neuroshape/recon.py
--rw-r--r--   0 c3336955   (503) staff       (20)     5400 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.6/neuroshape/stats.py
-drwxr-xr-x   0 c3336955   (503) staff       (20)        0 2023-07-11 01:49:03.208435 neuroshape-0.0.4.6.6/neuroshape/utils/
--rw-r--r--   0 c3336955   (503) staff       (20)       25 2023-06-07 11:17:25.000000 neuroshape-0.0.4.6.6/neuroshape/utils/__init__.py
--rw-r--r--   0 c3336955   (503) staff       (20)     1345 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.6/neuroshape/utils/check_fs_subjid.py
--rw-r--r--   0 c3336955   (503) staff       (20)      616 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.6/neuroshape/utils/check_map.py
--rw-r--r--   0 c3336955   (503) staff       (20)     6553 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.6/neuroshape/utils/checks.py
--rw-r--r--   0 c3336955   (503) staff       (20)      917 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.6/neuroshape/utils/compare_parallel.py
--rw-r--r--   0 c3336955   (503) staff       (20)     3501 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.6/neuroshape/utils/compute_geodesic_distance.py
--rw-r--r--   0 c3336955   (503) staff       (20)     6248 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.6/neuroshape/utils/concavehull.py
--rw-r--r--   0 c3336955   (503) staff       (20)    11779 2023-06-28 11:45:24.000000 neuroshape-0.0.4.6.6/neuroshape/utils/eigen.py
--rw-r--r--   0 c3336955   (503) staff       (20)      763 2023-06-13 01:26:03.000000 neuroshape-0.0.4.6.6/neuroshape/utils/fetch_atlas.py
--rw-r--r--   0 c3336955   (503) staff       (20)    25397 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.6/neuroshape/utils/fs_shapeDNA.py
--rw-r--r--   0 c3336955   (503) staff       (20)    32940 2023-06-28 10:54:36.000000 neuroshape-0.0.4.6.6/neuroshape/utils/geometry.py
--rw-r--r--   0 c3336955   (503) staff       (20)      348 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.6/neuroshape/utils/load_mesh_vertices.py
--rw-r--r--   0 c3336955   (503) staff       (20)     2580 2023-07-01 22:04:11.000000 neuroshape-0.0.4.6.6/neuroshape/utils/meshtransforms.py
--rw-r--r--   0 c3336955   (503) staff       (20)      222 2023-06-13 01:26:03.000000 neuroshape-0.0.4.6.6/neuroshape/utils/normalize_data.py
--rw-r--r--   0 c3336955   (503) staff       (20)      201 2023-06-11 10:05:42.000000 neuroshape-0.0.4.6.6/neuroshape/utils/swap_single_row.py
--rw-r--r--   0 c3336955   (503) staff       (20)      540 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.6/neuroshape/utils/tmpname.py
--rw-r--r--   0 c3336955   (503) staff       (20)      193 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.6/neuroshape/utils/zscore_avg_method.py
-drwxr-xr-x   0 c3336955   (503) staff       (20)        0 2023-07-11 01:49:03.190939 neuroshape-0.0.4.6.6/neuroshape.egg-info/
--rw-r--r--   0 c3336955   (503) staff       (20)     6795 2023-07-11 01:49:03.000000 neuroshape-0.0.4.6.6/neuroshape.egg-info/PKG-INFO
--rw-r--r--   0 c3336955   (503) staff       (20)     1383 2023-07-11 01:49:03.000000 neuroshape-0.0.4.6.6/neuroshape.egg-info/SOURCES.txt
--rw-r--r--   0 c3336955   (503) staff       (20)        1 2023-07-11 01:49:03.000000 neuroshape-0.0.4.6.6/neuroshape.egg-info/dependency_links.txt
--rw-r--r--   0 c3336955   (503) staff       (20)       11 2023-07-11 01:49:03.000000 neuroshape-0.0.4.6.6/neuroshape.egg-info/top_level.txt
--rw-r--r--   0 c3336955   (503) staff       (20)      670 2023-07-11 01:48:59.000000 neuroshape-0.0.4.6.6/pyproject.toml
--rw-r--r--   0 c3336955   (503) staff       (20)       38 2023-07-11 01:49:03.211550 neuroshape-0.0.4.6.6/setup.cfg
--rw-r--r--   0 c3336955   (503) staff       (20)     1048 2023-07-11 01:48:48.000000 neuroshape-0.0.4.6.6/setup.py
-drwxr-xr-x   0 c3336955   (503) staff       (20)        0 2023-07-11 01:49:03.210321 neuroshape-0.0.4.6.6/src/
--rw-r--r--   0 c3336955   (503) staff       (20)     5389 2023-06-16 11:25:08.000000 neuroshape-0.0.4.6.6/src/eta_squared.c
--rw-r--r--   0 c3336955   (503) staff       (20)     2545 2023-06-06 10:51:35.000000 neuroshape-0.0.4.6.6/src/euler_threshold.c
--rw-r--r--   0 c3336955   (503) staff       (20)     5946 2023-06-06 05:46:53.000000 neuroshape-0.0.4.6.6/src/glmfit.c
+drwxr-xr-x   0 c3336955   (503) staff       (20)        0 2023-08-01 04:57:41.333825 neuroshape-0.0.4.6.7/
+-rw-r--r--   0 c3336955   (503) staff       (20)     1501 2023-06-07 11:17:25.000000 neuroshape-0.0.4.6.7/LICENSE
+-rw-r--r--   0 c3336955   (503) staff       (20)     6795 2023-08-01 04:57:41.333109 neuroshape-0.0.4.6.7/PKG-INFO
+-rw-r--r--   0 c3336955   (503) staff       (20)     4445 2023-06-08 03:48:59.000000 neuroshape-0.0.4.6.7/README.rst
+drwxr-xr-x   0 c3336955   (503) staff       (20)        0 2023-08-01 04:57:41.102579 neuroshape-0.0.4.6.7/neuroshape/
+-rw-r--r--   0 c3336955   (503) staff       (20)        0 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.7/neuroshape/__init__.py
+-rw-r--r--   0 c3336955   (503) staff       (20)    22407 2023-06-16 11:25:08.000000 neuroshape-0.0.4.6.7/neuroshape/connectopic_laplacian.py
+-rw-r--r--   0 c3336955   (503) staff       (20)    22798 2023-08-01 04:50:52.000000 neuroshape-0.0.4.6.7/neuroshape/eigenmodes.py
+drwxr-xr-x   0 c3336955   (503) staff       (20)        0 2023-08-01 04:57:41.162879 neuroshape-0.0.4.6.7/neuroshape/nulls/
+-rw-r--r--   0 c3336955   (503) staff       (20)       44 2023-06-08 03:48:59.000000 neuroshape-0.0.4.6.7/neuroshape/nulls/__init__.py
+-rw-r--r--   0 c3336955   (503) staff       (20)     5351 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.7/neuroshape/nulls/burt.py
+-rw-r--r--   0 c3336955   (503) staff       (20)    20808 2023-06-13 01:26:03.000000 neuroshape-0.0.4.6.7/neuroshape/nulls/eigenshuff.py
+-rw-r--r--   0 c3336955   (503) staff       (20)    16743 2023-07-14 03:25:36.000000 neuroshape-0.0.4.6.7/neuroshape/nulls/eigensphere.py
+-rw-r--r--   0 c3336955   (503) staff       (20)    25239 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.7/neuroshape/nulls/nulls.py
+-rw-r--r--   0 c3336955   (503) staff       (20)    27669 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.7/neuroshape/nulls/spins.py
+drwxr-xr-x   0 c3336955   (503) staff       (20)        0 2023-08-01 04:57:41.198375 neuroshape-0.0.4.6.7/neuroshape/nulls/tests/
+-rw-r--r--   0 c3336955   (503) staff       (20)        0 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.7/neuroshape/nulls/tests/__init__.py
+-rw-r--r--   0 c3336955   (503) staff       (20)     5042 2023-06-19 22:07:48.000000 neuroshape-0.0.4.6.7/neuroshape/nulls/tests/eigenmode_replication.py
+-rw-r--r--   0 c3336955   (503) staff       (20)      530 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.7/neuroshape/nulls/tests/test_burt.py
+-rw-r--r--   0 c3336955   (503) staff       (20)     4137 2023-06-19 22:07:48.000000 neuroshape-0.0.4.6.7/neuroshape/nulls/tests/test_eigenresamp.py
+-rw-r--r--   0 c3336955   (503) staff       (20)      695 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.7/neuroshape/nulls/tests/test_nulls.py
+-rw-r--r--   0 c3336955   (503) staff       (20)      814 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.7/neuroshape/nulls/tests/test_spins.py
+-rw-r--r--   0 c3336955   (503) staff       (20)    12845 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.7/neuroshape/nulls/waveshuff.py
+-rw-r--r--   0 c3336955   (503) staff       (20)     4078 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.7/neuroshape/permutation.py
+-rw-r--r--   0 c3336955   (503) staff       (20)    13180 2023-06-18 23:49:14.000000 neuroshape-0.0.4.6.7/neuroshape/recon.py
+-rw-r--r--   0 c3336955   (503) staff       (20)     5400 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.7/neuroshape/stats.py
+drwxr-xr-x   0 c3336955   (503) staff       (20)        0 2023-08-01 04:57:41.310392 neuroshape-0.0.4.6.7/neuroshape/utils/
+-rw-r--r--   0 c3336955   (503) staff       (20)       25 2023-06-07 11:17:25.000000 neuroshape-0.0.4.6.7/neuroshape/utils/__init__.py
+-rw-r--r--   0 c3336955   (503) staff       (20)     1345 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.7/neuroshape/utils/check_fs_subjid.py
+-rw-r--r--   0 c3336955   (503) staff       (20)      616 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.7/neuroshape/utils/check_map.py
+-rw-r--r--   0 c3336955   (503) staff       (20)     6553 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.7/neuroshape/utils/checks.py
+-rw-r--r--   0 c3336955   (503) staff       (20)      917 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.7/neuroshape/utils/compare_parallel.py
+-rw-r--r--   0 c3336955   (503) staff       (20)     3501 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.7/neuroshape/utils/compute_geodesic_distance.py
+-rw-r--r--   0 c3336955   (503) staff       (20)     6248 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.7/neuroshape/utils/concavehull.py
+-rw-r--r--   0 c3336955   (503) staff       (20)    11555 2023-07-13 07:08:59.000000 neuroshape-0.0.4.6.7/neuroshape/utils/eigen.py
+-rw-r--r--   0 c3336955   (503) staff       (20)      763 2023-06-13 01:26:03.000000 neuroshape-0.0.4.6.7/neuroshape/utils/fetch_atlas.py
+-rw-r--r--   0 c3336955   (503) staff       (20)    25397 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.7/neuroshape/utils/fs_shapeDNA.py
+-rw-r--r--   0 c3336955   (503) staff       (20)    32940 2023-06-28 10:54:36.000000 neuroshape-0.0.4.6.7/neuroshape/utils/geometry.py
+-rw-r--r--   0 c3336955   (503) staff       (20)      348 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.7/neuroshape/utils/load_mesh_vertices.py
+-rw-r--r--   0 c3336955   (503) staff       (20)     2580 2023-07-01 22:04:11.000000 neuroshape-0.0.4.6.7/neuroshape/utils/meshtransforms.py
+-rw-r--r--   0 c3336955   (503) staff       (20)      222 2023-06-13 01:26:03.000000 neuroshape-0.0.4.6.7/neuroshape/utils/normalize_data.py
+-rw-r--r--   0 c3336955   (503) staff       (20)      201 2023-06-11 10:05:42.000000 neuroshape-0.0.4.6.7/neuroshape/utils/swap_single_row.py
+-rw-r--r--   0 c3336955   (503) staff       (20)      540 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.7/neuroshape/utils/tmpname.py
+-rw-r--r--   0 c3336955   (503) staff       (20)      193 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.7/neuroshape/utils/zscore_avg_method.py
+drwxr-xr-x   0 c3336955   (503) staff       (20)        0 2023-08-01 04:57:41.114404 neuroshape-0.0.4.6.7/neuroshape.egg-info/
+-rw-r--r--   0 c3336955   (503) staff       (20)     6795 2023-08-01 04:57:40.000000 neuroshape-0.0.4.6.7/neuroshape.egg-info/PKG-INFO
+-rw-r--r--   0 c3336955   (503) staff       (20)     1383 2023-08-01 04:57:41.000000 neuroshape-0.0.4.6.7/neuroshape.egg-info/SOURCES.txt
+-rw-r--r--   0 c3336955   (503) staff       (20)        1 2023-08-01 04:57:40.000000 neuroshape-0.0.4.6.7/neuroshape.egg-info/dependency_links.txt
+-rw-r--r--   0 c3336955   (503) staff       (20)       11 2023-08-01 04:57:40.000000 neuroshape-0.0.4.6.7/neuroshape.egg-info/top_level.txt
+-rw-r--r--   0 c3336955   (503) staff       (20)      670 2023-08-01 04:56:05.000000 neuroshape-0.0.4.6.7/pyproject.toml
+-rw-r--r--   0 c3336955   (503) staff       (20)       38 2023-08-01 04:57:41.334092 neuroshape-0.0.4.6.7/setup.cfg
+-rw-r--r--   0 c3336955   (503) staff       (20)     1048 2023-08-01 04:55:53.000000 neuroshape-0.0.4.6.7/setup.py
+drwxr-xr-x   0 c3336955   (503) staff       (20)        0 2023-08-01 04:57:41.332080 neuroshape-0.0.4.6.7/src/
+-rw-r--r--   0 c3336955   (503) staff       (20)     5389 2023-06-16 11:25:08.000000 neuroshape-0.0.4.6.7/src/eta_squared.c
+-rw-r--r--   0 c3336955   (503) staff       (20)     2545 2023-06-06 10:51:35.000000 neuroshape-0.0.4.6.7/src/euler_threshold.c
+-rw-r--r--   0 c3336955   (503) staff       (20)     5946 2023-06-06 05:46:53.000000 neuroshape-0.0.4.6.7/src/glmfit.c
```

### Comparing `neuroshape-0.0.4.6.6/LICENSE` & `neuroshape-0.0.4.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.6/PKG-INFO` & `neuroshape-0.0.4.6.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuroshape
-Version: 0.0.4.6.6
+Version: 0.0.4.6.7
 Summary: For computing connectopic and geometric Laplacian eigenmodes and performing null hypothesis testing. As implementation is ongoing, this description is subject to rapid change.
 Home-page: https://github.com/nikitas-k/neuroshape-dev
 Author: Nikitas C. Koussis, Systems Neuroscience Group Newcastle
 Author-email: "Nikitas C. Koussis" <nikitas.koussis@gmail.com>
 License: Copyright 2023 Systems Neuroscience Group Newcastle
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `neuroshape-0.0.4.6.6/README.rst` & `neuroshape-0.0.4.6.7/README.rst`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.6/neuroshape/connectopic_laplacian.py` & `neuroshape-0.0.4.6.7/neuroshape/connectopic_laplacian.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.6/neuroshape/eigenmodes.py` & `neuroshape-0.0.4.6.7/neuroshape/eigenmodes.py`

 * *Files 4% similar despite different names*

```diff
@@ -364,27 +364,27 @@
     hemi = splitsurf[0]
     surf = splitsurf[1]
     # map label if necessary
     mappedlabel = label
     if (source != sid):
         mappedlabel = os.path.join(outdir, os.path.basename(label) + '.' + str(uuid.uuid4()) + '.label')
         cmd = 'mri_label2label --sd ' + sdir + ' --srclabel ' + label + ' --srcsubject ' + source + ' --trgsubject ' + sid + ' --trglabel ' + mappedlabel + ' --hemi ' + hemi + ' --regmethod surface'
-        subprocess.run(cmd)     
+        os.system(cmd)     
     # make surface path (make sure output is stl, this currently needs fsdev, will probably be in 6.0)
     cmd = 'label2patch -writesurf -sdir ' + sdir + ' -surf ' + surf + ' ' + sid + ' ' + hemi + ' ' + mappedlabel + ' ' + stlsurf
-    subprocess.run(cmd)     
+    os.system(cmd)     
     cmd = 'mris_convert ' + stlsurf + ' ' + outsurf
-    subprocess.run(cmd)
+    os.system(cmd)
     
     # cleanup map label if necessary
     if (source != sid):
         cmd ='rm ' + mappedlabel
-        subprocess.run(cmd)     
+        os.system(cmd)     
     cmd = 'rm ' + stlsurf
-    subprocess.run(cmd)
+    os.system(cmd)
     
     # make and write surface
     outsurf = make_surf(sdir, sid, surf, outdir, outsurf)
     
     # return surf name
     return outsurf
 
@@ -404,38 +404,38 @@
     segsurf  = os.path.join(outdir, tmpname + '.vtk')
     # binarize on selected labels (creates temp segf)
     ptinput = aseg
     ptlabel = str(asegid[0])
     #if len(asegid) > 1:
     # always binarize first, otherwise pretess may scale aseg if labels are larger than 255 (e.g. aseg+aparc, bug in mri_pretess?)
     cmd ='mri_binarize --i ' + aseg + ' --match ' + astring2 + ' --o ' + segf
-    subprocess.run(cmd) 
+    os.system(cmd) 
     ptinput = segf
     ptlabel = '1'
     # if norm exist, fix label (pretess)
     if os.path.isfile(norm):
         cmd ='mri_pretess ' + ptinput + ' ' + ptlabel + ' ' + norm + ' ' + segf
-        subprocess.run(cmd) 
+        os.system(cmd) 
     else:
         if not os.path.isfile(segf):
             # cp segf if not exist yet
             # (it exists already if we combined labels above)
             cmd = 'cp ' + ptinput + ' ' + segf
-            subprocess.run(cmd) 
+            os.system(cmd) 
     # runs marching cube to extract surface
     cmd ='mri_mc ' + segf + ' ' + ptlabel + ' ' + segsurf
-    subprocess.run(cmd) 
+    os.system(cmd) 
     # convert to stl
     cmd ='mris_convert ' + segsurf + ' ' + outsurf
-    subprocess.run(cmd)
+    os.system(cmd)
     # cleanup temp files
     cmd ='rm ' + segf
-    subprocess.run(cmd) 
+    os.system(cmd) 
     cmd ='rm ' + segsurf
-    subprocess.run(cmd)
+    os.system(cmd)
     
     
     # return surf name
     return outsurf
 
 
 def get_aparc_surf(sdir, sid, surf, aparcid, outsurf):
@@ -451,49 +451,49 @@
     hemi = surf.split(".", 1)[0]
     # convert annotation id to label:
     alllabels = ''
     for aid in aparcid:
         # create label of this id
         outlabelpre = os.path.join(outdir, hemi + '.aparc.' + rndname)
         cmd = 'mri_annotation2label --sd ' + sdir + ' --subject ' + sid + ' --hemi ' + hemi + ' --label ' + str(aid) + ' --labelbase ' + outlabelpre 
-        subprocess.run(cmd) 
+        os.system(cmd) 
         alllabels = alllabels + '-i ' + outlabelpre + "-%03d.label" % int(aid) + ' ' 
     # merge labels (if more than 1)
     mergedlabel = outlabelpre + "-%03d.label" % int(aid)
     if len(aparcid) > 1:
         mergedlabel = os.path.join(outdir, hemi + '.aparc.all.' + rndname + '.label')
         cmd = 'mri_mergelabels ' + alllabels + ' -o ' + mergedlabel
-        subprocess.run(cmd) 
+        os.system(cmd) 
     # make to surface (call subfunction above)
     get_label_surf(sdir, sid, mergedlabel, surf, sid, outsurf)
     # cleanup
     if len(aparcid) > 1:
         cmd ='rm ' + mergedlabel
-        subprocess.run(cmd)
+        os.system(cmd)
     for aid in aparcid:
         outlabelpre = os.path.join(outdir, hemi + '.aparc.' + rndname + "-%03d.label" % int(aid))
         cmd ='rm ' + outlabelpre
-        subprocess.run(cmd)
+        os.system(cmd)
     # return surf name
     return outsurf
 
 def get_tetmesh(sdir, sid, surf, outtet, norm_type, norm_factor=1):
     # TODO FIX nonfunctional for now 
     surfbase  = os.path.basename(surf)
     outdir    = os.path.dirname(outtet)    
     surftemp_stl = os.path.join(outdir, surfbase + '.temp.stl')
     
     # make surface mesh
     cmd = 'mris_convert ' + surf + ' ' + surftemp_stl
-    subprocess.run(cmd)
+    os.system(cmd)
     
     # marching cubes
     tria_file = 'tmp_surface.vtk'
     cmd = 'mri_mc ' + surftemp_stl + ' 1 ' + outdir + '/' + tria_file
-    subprocess.run(cmd)
+    os.system(cmd)
       
     # write gmsh geofile
     geofile  = os.path.join(outdir,'gmsh.'+str(uuid.uuid4())+'.geo')
     
     with open(geofile, 'w') as g:
         g.write("Mesh.Algorithm3D=4;\n")
         g.write("Mesh.Optimize=1;\n")
@@ -501,18 +501,18 @@
         g.write("Merge \""+surfbase+'.temp.stl'+"\";\n")
         g.write("Surface Loop(1) = {1};\n")
         g.write("Volume(1) = {1};\n")
         g.write("Physical Volume(1) = {1};\n")
         
     # use gmsh to create tet mesh
     cmd = 'gmsh -3 -o ' + outtet + ' ' + geofile
-    subprocess.run(cmd)
+    os.system(cmd)
     
     cmd = "sed 's/double/float/g;s/UNSTRUCTURED_GRID/POLYDATA/g;s/CELLS/POLYGONS/g;/CELL_TYPES/,$d' " + outtet + " > " + outtet + "'_fixed'"
-    subprocess.run(cmd)
+    os.system(cmd)
     
     # get volume and number of non-zero voxels in ROI
     brainmask_path = os.path.join(sdir, sid, 'mri', 'brainmask.mgz')
     
     # normalize surface
     tet = TetIO.import_gmsh(outtet)
     tet_norm = tet
@@ -528,19 +528,19 @@
     # elif norm_type == 'constant':
     #     tet_norm.v = tet.v/(norm_factor ** (1/3))
     
     
     
     # cleanup
     cmd ='rm ' + geofile
-    subprocess.run(cmd) 
+    os.system(cmd) 
     cmd='rm ' + surftemp_stl
-    subprocess.run(cmd)
+    os.system(cmd)
     cmd = 'rm '+ '/tmp_surface.vtk'
-    subprocess.run(cmd)
+    os.system(cmd)
 
     # return tetmesh filename
     return outtet
 
 def calc_eigenmodes(sdir, sid, surf_file, outdir, outevec=None, num_modes=2):
     """
     Calculate the eigenmodes of a mesh
```

### Comparing `neuroshape-0.0.4.6.6/neuroshape/nulls/burt.py` & `neuroshape-0.0.4.6.7/neuroshape/nulls/burt.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.6/neuroshape/nulls/eigenshuff.py` & `neuroshape-0.0.4.6.7/neuroshape/nulls/eigenshuff.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.6/neuroshape/nulls/eigensphere.py` & `neuroshape-0.0.4.6.7/neuroshape/nulls/eigensphere.py`

 * *Files 7% similar despite different names*

```diff
@@ -87,19 +87,18 @@
         - find the unit vectors of the points `p` by dividing by the 
             Euclidean norm (equivalent to the eigenmodes)
         - make the new unit vectors orthonormal using Gram-Schmidt process
         - return the new eigenmodes of that eigengroup until all eigengroups
             are computed
         - reconstruct the null data by multiplying the original coefficients
             by the new eigenmodes
-        - resamples the original data to the new distribution by performing
-            a rank order of both the surrogate and the empirical data and
-            subsitutes the empirical data into the new array, then returns the
-            original distribution of the data. This preserves the values,
-            but results in a new map
+        - resamples the null data by performing rank-ordering to replicate
+            the reconstructed data term, then adds the noise term back into the
+            null data to produce a surrogate that replicates the original
+            variance of the empirical data.
             * Only performed if `resample` = True.
     
     References
     ----------
         1. Robinson, P. A. et al., (2016), Eigenmodes of brain activity: Neural field 
         theory predictions and comparison with experiment. NeuroImage 142, 79-98.
         <https://dx.doi.org/10.1016/j.neuroimage.2016.04.050>
@@ -249,89 +248,109 @@
     medial_wall = medial_wall.astype(bool)
     
     medial_mask = np.logical_not(medial_wall)
     data_copy = copy.deepcopy(data) # deepcopy original data so it's not modified
     data_copy = data_copy[medial_mask]
     emodes_copy = copy.deepcopy(emodes)
     emodes_copy = emodes_copy[medial_mask]
+    #emodes_copy = gram_schmidt(emodes_copy)
     
     # find eigengroups
     groups = _get_eigengroups(emodes_copy)
     
     # if not given angles
     if angles is None:
         angles = np.random.randn(len(groups) + 1) * np.pi
     
     # initialize the new modes
-    new_modes = np.zeros_like(emodes_copy)
+    new_modes = copy.deepcopy(np.zeros_like(emodes_copy))
     
     m = 0 #index of angles
     # resample the hypersphere (except for groups 1 and 2)
     for idx in range(1, len(groups)):
         group_modes = emodes_copy[:, groups[idx]]
         group_evals = evals[groups[idx]]
         
         if len(groups[idx]) == 3:
             # do simple rotation
-            # initialize the points
+            # initialize thße points
             p = group_modes / np.sqrt(group_evals)
+            #p /= np.linalg.norm(p, axis=0)
             p *= np.cos(angles[m])
             
             # ensure orthonormal
-            group_new_modes = gram_schmidt(p)
+            group_new_modes = gram_schmidt(p * np.sqrt(group_evals))
              # get the index for the angles
             new_modes[:, groups[idx]] = group_new_modes
         
         m += 1
         # else, transform to spheroid and index the angles properly
         group_new_modes = transform_to_spheroid(group_evals, group_modes)
         group_spherical_modes = resample_spheroid(group_new_modes, angles[m])
         
         # ensure orthonormal
-        group_spherical_modes = gram_schmidt(group_spherical_modes)
+        #group_spherical_modes = gram_schmidt(group_spherical_modes)
         
         # transform back to ellipsoid
         group_ellipsoid_modes = transform_to_ellipsoid(group_evals, group_spherical_modes)
         
         new_modes[:, groups[idx]] = gram_schmidt(group_ellipsoid_modes) #/ np.linalg.norm(group_ellipsoid_modes)
      
     #new_modes = gram_schmidt(new_modes) #/ np.linalg.norm(new_modes)
     # find the coefficents of the modes to the data by solving the OLS
     # decomposition, either through the normal equation solution or regression    
     coeffs = eigen_decomposition(data_copy, emodes_copy, method=method)
+    reconstructed_data = coeffs @ emodes_copy.T
     
     # matrix multiply the estimated coefficients by the new modes
     surrogate_data = np.zeros_like(data)
     
     if randomize is True:
         for i in range(len(groups)):
             coeffs[groups[i]] = np.random.permutation(coeffs[groups[i]])
     
     surrogate_data[medial_mask] = reconstruct_data(coeffs, new_modes)
     
     # mask out medial wall from surrogate
     #surrogate_data[medial_wall] = 0.0
+    mask = np.logical_not(medial_wall)
+
+    # Mask the data and surrogate_data excluding the medial wall
+    surr_no_mwall = copy.deepcopy(surrogate_data)
+    surr_no_mwall = surr_no_mwall[mask]
     
     if resample is True:
-        mask = np.logical_not(medial_wall)
-
-        # Mask the data and surrogate_data excluding the medial wall
-        data_no_mwall = data[mask]
-        surr_no_mwall = copy.deepcopy(surrogate_data)
-        surr_no_mwall = surr_no_mwall[mask]
-        
         # Get the rank ordered indices
-        data_ranks = data_no_mwall.argsort()[::-1]
+        data_ranks = reconstructed_data.argsort()[::-1]
         surr_ranks = surr_no_mwall.argsort()[::-1]
         
         # Resample surr_no_mwall according to the rank ordering of data_no_mwall
-        surr_no_mwall[surr_ranks] = data_no_mwall[data_ranks]
-        output_surr = np.zeros_like(surrogate_data)
-        output_surr[mask] = surr_no_mwall
-        surrogate_data = output_surr
+        surr_no_mwall[surr_ranks] = reconstructed_data[data_ranks]
+        
+    else: # force match the minima
+        surr_no_mwall /= np.sqrt(np.mean(surr_no_mwall**2))
+        surr_no_mwall *= np.sqrt(np.mean(data_copy**2))        
+    
+    # now add the residuals of the original data
+    residuals = data_copy - reconstructed_data
+
+    # slightly permute the original residuals
+    #window_size = 50  # size of the local section to shuffle
+    
+    # Loop over the array with a stride of window_size
+    #for i in range(0, len(residuals), window_size):
+        # Randomly permute a small section of the array
+        #residuals[i:i+window_size] = np.random.permutation(residuals[i:i+window_size])
+    
+    surr_no_mwall = surr_no_mwall + residuals
+    
+    output_surr = np.zeros_like(surrogate_data)
+    output_surr[mask] = surr_no_mwall
+    
+    surrogate_data = output_surr
     
     return surrogate_data
 
 
 def plot_data(surface, data, hemi='left', view='lateral', cmap='gray', show=True):
     """
     Plots a data map using nilearn.plotting, returns fig and ax handles
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `neuroshape-0.0.4.6.6/neuroshape/nulls/nulls.py` & `neuroshape-0.0.4.6.7/neuroshape/nulls/nulls.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.6/neuroshape/nulls/spins.py` & `neuroshape-0.0.4.6.7/neuroshape/nulls/spins.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.6/neuroshape/nulls/tests/eigenmode_replication.py` & `neuroshape-0.0.4.6.7/neuroshape/nulls/tests/eigenmode_replication.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.6/neuroshape/nulls/tests/test_burt.py` & `neuroshape-0.0.4.6.7/neuroshape/nulls/tests/test_burt.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.6/neuroshape/nulls/tests/test_eigenresamp.py` & `neuroshape-0.0.4.6.7/neuroshape/nulls/tests/test_eigenresamp.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.6/neuroshape/nulls/tests/test_nulls.py` & `neuroshape-0.0.4.6.7/neuroshape/nulls/tests/test_nulls.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.6/neuroshape/nulls/tests/test_spins.py` & `neuroshape-0.0.4.6.7/neuroshape/nulls/tests/test_spins.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.6/neuroshape/nulls/waveshuff.py` & `neuroshape-0.0.4.6.7/neuroshape/nulls/waveshuff.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.6/neuroshape/permutation.py` & `neuroshape-0.0.4.6.7/neuroshape/permutation.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.6/neuroshape/recon.py` & `neuroshape-0.0.4.6.7/neuroshape/recon.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.6/neuroshape/stats.py` & `neuroshape-0.0.4.6.7/neuroshape/stats.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.6/neuroshape/utils/check_fs_subjid.py` & `neuroshape-0.0.4.6.7/neuroshape/utils/check_fs_subjid.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.6/neuroshape/utils/check_map.py` & `neuroshape-0.0.4.6.7/neuroshape/utils/check_map.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.6/neuroshape/utils/checks.py` & `neuroshape-0.0.4.6.7/neuroshape/utils/checks.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.6/neuroshape/utils/compare_parallel.py` & `neuroshape-0.0.4.6.7/neuroshape/utils/compare_parallel.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.6/neuroshape/utils/compute_geodesic_distance.py` & `neuroshape-0.0.4.6.7/neuroshape/utils/compute_geodesic_distance.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.6/neuroshape/utils/concavehull.py` & `neuroshape-0.0.4.6.7/neuroshape/utils/concavehull.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.6/neuroshape/utils/eigen.py` & `neuroshape-0.0.4.6.7/neuroshape/utils/eigen.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,15 +105,15 @@
             return eigs_.T
     except:
         return eigs_.T
     eigs_ = eigs_swapped
     previous_corr = next_corr
     
 
-def reconstruct_data(coeffs, eigenmodes, pv=100.0):
+def reconstruct_data(coeffs, eigenmodes):
     """
     Reconstruct a dataset of `n_vertices` given a set of eigenmodes and coeffs
     conditioned on data using ordinary least squares (OLS)
 
     Parameters
     ----------
     coeffs : np.ndarray of shape (M,)
@@ -126,24 +126,17 @@
     Returns
     -------
     new_data : np.ndarray of (n_vertices,)
         Reconstructed data
 
     """
     
-    if pv == 0.0:
-        raise ValueError("Percentage of modes to use for reconstruction must be greater than 1")
-        
-    _, M = eigenmodes.shape
-    n = int(np.ceil(M * pv / 100))
-    
-    eigenmodes = eigenmodes[:,:n]
-    coeffs = coeffs[:n].reshape(-1, 1)
+    coeffs = coeffs.reshape(-1, 1)
     
-    new_data = coeffs.T @ eigenmodes.T
+    new_data = eigenmodes @ coeffs
     
     return new_data.squeeze()
     
 
 def reconstruct_surface(surface, eigenmodes, n=100, normalize='area', norm_factor=1, method='matrix'):
     """
     Reconstruct a surface of `n_vertices` given a set of eigenmodes
@@ -317,19 +310,19 @@
     # ensure the eigenmodes are normalized on the unit hypersphere
     spheroid_eigenmodes = spheroid_eigenmodes #/ np.linalg.norm(spheroid_eigenmodes, axis=0)
     
     # length of group to determine evenness or oddness of dimensions
     #dims = spheroid_eigenmodes.shape[0]
     
     # initialize the new points p
-    p = spheroid_eigenmodes
+    p = spheroid_eigenmodes * np.cos(angle)
     
     # compute the coordinates for the new points
-    for i in range(1, spheroid_eigenmodes.shape[1]):
-        p[:, i] *= np.cos(angle)
+    # for i in range(0, spheroid_eigenmodes.shape[1]):
+    #     p[:, i] *= np.cos(angle)
     
     # Compute the coordinates for new points p
     # print("Computing the coordinates for each dimension, multiplying by single angle per group")
     # if dims % 2 == 0: # EVEN
     #     p *= np.cos(angle)
     # else: #dims % 2 == 1 ODD
     #     p *= np.sin(angle)
```

### Comparing `neuroshape-0.0.4.6.6/neuroshape/utils/fetch_atlas.py` & `neuroshape-0.0.4.6.7/neuroshape/utils/fetch_atlas.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.6/neuroshape/utils/fs_shapeDNA.py` & `neuroshape-0.0.4.6.7/neuroshape/utils/fs_shapeDNA.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.6/neuroshape/utils/geometry.py` & `neuroshape-0.0.4.6.7/neuroshape/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.6/neuroshape/utils/meshtransforms.py` & `neuroshape-0.0.4.6.7/neuroshape/utils/meshtransforms.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.6/neuroshape/utils/tmpname.py` & `neuroshape-0.0.4.6.7/neuroshape/utils/tmpname.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.6/neuroshape.egg-info/PKG-INFO` & `neuroshape-0.0.4.6.7/neuroshape.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuroshape
-Version: 0.0.4.6.6
+Version: 0.0.4.6.7
 Summary: For computing connectopic and geometric Laplacian eigenmodes and performing null hypothesis testing. As implementation is ongoing, this description is subject to rapid change.
 Home-page: https://github.com/nikitas-k/neuroshape-dev
 Author: Nikitas C. Koussis, Systems Neuroscience Group Newcastle
 Author-email: "Nikitas C. Koussis" <nikitas.koussis@gmail.com>
 License: Copyright 2023 Systems Neuroscience Group Newcastle
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `neuroshape-0.0.4.6.6/neuroshape.egg-info/SOURCES.txt` & `neuroshape-0.0.4.6.7/neuroshape.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.6/pyproject.toml` & `neuroshape-0.0.4.6.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     "setuptools>=42",
     "wheel",
 ]
 
 
 [project]
 name = "neuroshape"
-version = "0.0.4.6.6"
+version = "0.0.4.6.7"
 description = "For computing connectopic and geometric Laplacian eigenmodes and performing null hypothesis testing. As implementation is ongoing, this description is subject to rapid change."
 readme = "README.rst"
 authors = [
     {name = "Nikitas C. Koussis", email = "nikitas.koussis@gmail.com"},
 ]
 license = { file = "LICENSE" }
```

### Comparing `neuroshape-0.0.4.6.6/setup.py` & `neuroshape-0.0.4.6.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,14 +13,14 @@
 #                   include_dirs=[numpy.get_include()])
 
 #euler = Extension('neuroshape.euler', sources=['src/euler_threshold.c'],
 #                  include_dirs=[numpy.get_include()])
 
 # run the setup
 setup(name='neuroshape',
-      version='0.0.4.6.6',
+      version='0.0.4.6.7',
       description="For computing connectopic and geometric Laplacian eigenmodes and performing null hypothesis testing. As implementation is ongoing, this description is subject to rapid change.",
       author='Nikitas C. Koussis, Systems Neuroscience Group Newcastle',
       author_email='nikitas.koussis@gmail.com',
       url='https://github.com/nikitas-k/neuroshape-dev',
       packages=find_packages())
       #ext_modules=[eta, glmfit, euler])
```

### Comparing `neuroshape-0.0.4.6.6/src/eta_squared.c` & `neuroshape-0.0.4.6.7/src/eta_squared.c`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.6/src/euler_threshold.c` & `neuroshape-0.0.4.6.7/src/euler_threshold.c`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.6/src/glmfit.c` & `neuroshape-0.0.4.6.7/src/glmfit.c`

 * *Files identical despite different names*

