# Comparing `tmp/pyseat-0.0.1.3.tar.gz` & `tmp/pyseat-0.0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyseat-0.0.1.3.tar", last modified: Tue Oct 18 15:33:22 2022, max compression
+gzip compressed data, was "pyseat-0.0.1.4.tar", last modified: Tue Aug  1 04:08:11 2023, max compression
```

## Comparing `pyseat-0.0.1.3.tar` & `pyseat-0.0.1.4.tar`

### file list

```diff
@@ -1,51 +1,16 @@
-drwxrwxrwx   0 chenlingxi  (1000) chenlingxi  (1000)        0 2022-10-18 15:33:22.477481 pyseat-0.0.1.3/
--rwxrwxrwx   0 chenlingxi  (1000) chenlingxi  (1000)      344 2022-10-18 15:33:22.476483 pyseat-0.0.1.3/PKG-INFO
-drwxrwxrwx   0 chenlingxi  (1000) chenlingxi  (1000)        0 2022-10-18 15:33:22.316020 pyseat-0.0.1.3/pyseat/
--rwxrwxrwx   0 chenlingxi  (1000) chenlingxi  (1000)     8127 2022-10-18 15:30:35.000000 pyseat-0.0.1.3/pyseat/HierachicalEmbedding.py
--rwxrwxrwx   0 chenlingxi  (1000) chenlingxi  (1000)    38331 2022-10-18 15:30:42.000000 pyseat-0.0.1.3/pyseat/SEAT.py
--rwxrwxrwx   0 chenlingxi  (1000) chenlingxi  (1000)        0 2022-09-15 07:06:40.000000 pyseat-0.0.1.3/pyseat/__init__.py
--rwxrwxrwx   0 chenlingxi  (1000) chenlingxi  (1000)     4208 2022-09-15 07:13:25.000000 pyseat-0.0.1.3/pyseat/graph_metric.py
--rwxrwxrwx   0 chenlingxi  (1000) chenlingxi  (1000)       24 2022-10-18 15:32:16.000000 pyseat-0.0.1.3/pyseat/version.py
-drwxrwxrwx   0 chenlingxi  (1000) chenlingxi  (1000)        0 2022-10-18 15:33:22.322001 pyseat-0.0.1.3/pyseat.egg-info/
--rwxrwxrwx   0 chenlingxi  (1000) chenlingxi  (1000)      344 2022-10-18 15:33:22.000000 pyseat-0.0.1.3/pyseat.egg-info/PKG-INFO
--rwxrwxrwx   0 chenlingxi  (1000) chenlingxi  (1000)     1278 2022-10-18 15:33:22.000000 pyseat-0.0.1.3/pyseat.egg-info/SOURCES.txt
--rwxrwxrwx   0 chenlingxi  (1000) chenlingxi  (1000)        1 2022-10-18 15:33:22.000000 pyseat-0.0.1.3/pyseat.egg-info/dependency_links.txt
--rwxrwxrwx   0 chenlingxi  (1000) chenlingxi  (1000)      362 2022-10-18 15:33:22.000000 pyseat-0.0.1.3/pyseat.egg-info/requires.txt
--rwxrwxrwx   0 chenlingxi  (1000) chenlingxi  (1000)       38 2022-10-18 15:33:22.000000 pyseat-0.0.1.3/pyseat.egg-info/top_level.txt
-drwxrwxrwx   0 chenlingxi  (1000) chenlingxi  (1000)        0 2022-10-18 15:33:22.353894 pyseat-0.0.1.3/pyseat_backup/
--rwxrwxrwx   0 chenlingxi  (1000) chenlingxi  (1000)     9723 2021-11-03 13:44:55.000000 pyseat-0.0.1.3/pyseat_backup/KR_norm_juicer.py
--rwxrwxrwx   0 chenlingxi  (1000) chenlingxi  (1000)     6320 2022-04-28 07:08:31.000000 pyseat-0.0.1.3/pyseat_backup/SEAT.py
--rwxrwxrwx   0 chenlingxi  (1000) chenlingxi  (1000)    38846 2021-12-27 13:12:42.000000 pyseat-0.0.1.3/pyseat_backup/SEAT_queue.py
--rwxrwxrwx   0 chenlingxi  (1000) chenlingxi  (1000)        0 2021-10-07 03:28:34.000000 pyseat-0.0.1.3/pyseat_backup/__init__.py
--rwxrwxrwx   0 chenlingxi  (1000) chenlingxi  (1000)      435 2021-10-01 03:33:54.000000 pyseat-0.0.1.3/pyseat_backup/graph.py
--rwxrwxrwx   0 chenlingxi  (1000) chenlingxi  (1000)     3274 2021-11-17 05:11:41.000000 pyseat-0.0.1.3/pyseat_backup/se.py
--rwxrwxrwx   0 chenlingxi  (1000) chenlingxi  (1000)       24 2021-10-07 03:44:30.000000 pyseat-0.0.1.3/pyseat_backup/version.py
-drwxrwxrwx   0 chenlingxi  (1000) chenlingxi  (1000)        0 2022-10-18 15:33:22.423660 pyseat-0.0.1.3/pyseat_workspace/
--rwxrwxrwx   0 chenlingxi  (1000) chenlingxi  (1000)     3364 2022-06-14 14:41:06.000000 pyseat-0.0.1.3/pyseat_workspace/HE_recursive_demo.py
--rwxrwxrwx   0 chenlingxi  (1000) chenlingxi  (1000)     8127 2022-10-18 15:28:16.000000 pyseat-0.0.1.3/pyseat_workspace/HierachicalEmbedding.py
--rwxrwxrwx   0 chenlingxi  (1000) chenlingxi  (1000)     9723 2022-04-03 07:31:01.000000 pyseat-0.0.1.3/pyseat_workspace/KR_norm_juicer.py
--rwxrwxrwx   0 chenlingxi  (1000) chenlingxi  (1000)    35134 2022-04-30 14:09:38.000000 pyseat-0.0.1.3/pyseat_workspace/SEAT - Copy.py
--rwxrwxrwx   0 chenlingxi  (1000) chenlingxi  (1000)    38331 2022-10-18 15:28:14.000000 pyseat-0.0.1.3/pyseat_workspace/SEAT.py
--rwxrwxrwx   0 chenlingxi  (1000) chenlingxi  (1000)    33405 2022-05-26 10:19:21.000000 pyseat-0.0.1.3/pyseat_workspace/SEAT_20220526.py
--rwxrwxrwx   0 chenlingxi  (1000) chenlingxi  (1000)    44482 2022-04-30 06:48:44.000000 pyseat-0.0.1.3/pyseat_workspace/SEAT_ms_backup.py
--rwxrwxrwx   0 chenlingxi  (1000) chenlingxi  (1000)    38846 2022-04-03 07:31:01.000000 pyseat-0.0.1.3/pyseat_workspace/SEAT_queue.py
--rwxrwxrwx   0 chenlingxi  (1000) chenlingxi  (1000)        0 2022-04-03 07:31:01.000000 pyseat-0.0.1.3/pyseat_workspace/__init__.py
--rwxrwxrwx   0 chenlingxi  (1000) chenlingxi  (1000)    10125 2022-04-28 10:34:12.000000 pyseat-0.0.1.3/pyseat_workspace/call_cn.py
--rwxrwxrwx   0 chenlingxi  (1000) chenlingxi  (1000)      435 2022-04-03 07:31:01.000000 pyseat-0.0.1.3/pyseat_workspace/graph.py
--rwxrwxrwx   0 chenlingxi  (1000) chenlingxi  (1000)     4022 2022-05-27 02:28:01.000000 pyseat-0.0.1.3/pyseat_workspace/graph_metric.py
--rwxrwxrwx   0 chenlingxi  (1000) chenlingxi  (1000)     3122 2022-05-06 13:10:37.000000 pyseat-0.0.1.3/pyseat_workspace/se_20220526.py
-drwxrwxrwx   0 chenlingxi  (1000) chenlingxi  (1000)        0 2022-10-18 15:33:22.475487 pyseat-0.0.1.3/pyseat_workspace/smurf/
--rwxrwxrwx   0 chenlingxi  (1000) chenlingxi  (1000)      271 2022-05-02 07:11:33.000000 pyseat-0.0.1.3/pyseat_workspace/smurf/__init__.py
--rwxrwxrwx   0 chenlingxi  (1000) chenlingxi  (1000)     1677 2022-05-02 07:11:33.000000 pyseat-0.0.1.3/pyseat_workspace/smurf/cell_circle.py
--rwxrwxrwx   0 chenlingxi  (1000) chenlingxi  (1000)     1470 2022-05-02 07:11:33.000000 pyseat-0.0.1.3/pyseat_workspace/smurf/distance.py
--rwxrwxrwx   0 chenlingxi  (1000) chenlingxi  (1000)     3853 2022-05-02 07:11:33.000000 pyseat-0.0.1.3/pyseat_workspace/smurf/initialParams.py
--rwxrwxrwx   0 chenlingxi  (1000) chenlingxi  (1000)     2006 2022-05-02 07:11:33.000000 pyseat-0.0.1.3/pyseat_workspace/smurf/lossFunc.py
--rwxrwxrwx   0 chenlingxi  (1000) chenlingxi  (1000)     2244 2022-05-02 07:11:33.000000 pyseat-0.0.1.3/pyseat_workspace/smurf/lossFunc_sym.py
--rwxrwxrwx   0 chenlingxi  (1000) chenlingxi  (1000)    14345 2022-05-02 07:11:33.000000 pyseat-0.0.1.3/pyseat_workspace/smurf/model.py
--rwxrwxrwx   0 chenlingxi  (1000) chenlingxi  (1000)    12941 2022-05-02 07:11:33.000000 pyseat-0.0.1.3/pyseat_workspace/smurf/model_sym.py
--rwxrwxrwx   0 chenlingxi  (1000) chenlingxi  (1000)    11181 2022-05-02 07:11:33.000000 pyseat-0.0.1.3/pyseat_workspace/smurf/optimize.py
--rwxrwxrwx   0 chenlingxi  (1000) chenlingxi  (1000)     2785 2022-05-02 07:11:33.000000 pyseat-0.0.1.3/pyseat_workspace/smurf/utiles.py
--rwxrwxrwx   0 chenlingxi  (1000) chenlingxi  (1000)      165 2022-05-02 07:11:33.000000 pyseat-0.0.1.3/pyseat_workspace/smurf/version.py
--rwxrwxrwx   0 chenlingxi  (1000) chenlingxi  (1000)       24 2022-04-03 07:31:01.000000 pyseat-0.0.1.3/pyseat_workspace/version.py
--rwxrwxrwx   0 chenlingxi  (1000) chenlingxi  (1000)       38 2022-10-18 15:33:22.477481 pyseat-0.0.1.3/setup.cfg
--rwxrwxrwx   0 chenlingxi  (1000) chenlingxi  (1000)     1299 2022-10-02 14:02:59.000000 pyseat-0.0.1.3/setup.py
+drwxr-xr-x   0 chenlingxi   (501) staff       (20)        0 2023-08-01 04:08:11.814295 pyseat-0.0.1.4/
+-rw-r--r--   0 chenlingxi   (501) staff       (20)      389 2023-08-01 04:08:11.814162 pyseat-0.0.1.4/PKG-INFO
+drwxr-xr-x   0 chenlingxi   (501) staff       (20)        0 2023-08-01 04:08:11.813377 pyseat-0.0.1.4/pyseat/
+-rw-r--r--   0 chenlingxi   (501) staff       (20)     8127 2022-09-15 07:06:40.000000 pyseat-0.0.1.4/pyseat/HierachicalEmbedding.py
+-rw-r--r--   0 chenlingxi   (501) staff       (20)    38331 2022-10-18 15:30:42.000000 pyseat-0.0.1.4/pyseat/SEAT.py
+-rw-r--r--   0 chenlingxi   (501) staff       (20)        0 2022-09-15 07:06:40.000000 pyseat-0.0.1.4/pyseat/__init__.py
+-rw-r--r--   0 chenlingxi   (501) staff       (20)     4208 2022-09-15 07:13:25.000000 pyseat-0.0.1.4/pyseat/graph_metric.py
+-rw-r--r--   0 chenlingxi   (501) staff       (20)       24 2023-08-01 04:04:36.000000 pyseat-0.0.1.4/pyseat/version.py
+drwxr-xr-x   0 chenlingxi   (501) staff       (20)        0 2023-08-01 04:08:11.814007 pyseat-0.0.1.4/pyseat.egg-info/
+-rw-r--r--   0 chenlingxi   (501) staff       (20)      389 2023-08-01 04:08:11.000000 pyseat-0.0.1.4/pyseat.egg-info/PKG-INFO
+-rw-r--r--   0 chenlingxi   (501) staff       (20)      263 2023-08-01 04:08:11.000000 pyseat-0.0.1.4/pyseat.egg-info/SOURCES.txt
+-rw-r--r--   0 chenlingxi   (501) staff       (20)        1 2023-08-01 04:08:11.000000 pyseat-0.0.1.4/pyseat.egg-info/dependency_links.txt
+-rw-r--r--   0 chenlingxi   (501) staff       (20)      367 2023-08-01 04:08:11.000000 pyseat-0.0.1.4/pyseat.egg-info/requires.txt
+-rw-r--r--   0 chenlingxi   (501) staff       (20)        7 2023-08-01 04:08:11.000000 pyseat-0.0.1.4/pyseat.egg-info/top_level.txt
+-rw-r--r--   0 chenlingxi   (501) staff       (20)       38 2023-08-01 04:08:11.814355 pyseat-0.0.1.4/setup.cfg
+-rw-r--r--   0 chenlingxi   (501) staff       (20)     1304 2023-08-01 04:03:55.000000 pyseat-0.0.1.4/setup.py
```

### Comparing `pyseat-0.0.1.3/pyseat/HierachicalEmbedding.py` & `pyseat-0.0.1.4/pyseat/HierachicalEmbedding.py`

 * *Files identical despite different names*

### Comparing `pyseat-0.0.1.3/pyseat/SEAT.py` & `pyseat-0.0.1.4/pyseat/SEAT.py`

 * *Files identical despite different names*

### Comparing `pyseat-0.0.1.3/pyseat/graph_metric.py` & `pyseat-0.0.1.4/pyseat/graph_metric.py`

 * *Files identical despite different names*

### Comparing `pyseat-0.0.1.3/setup.py` & `pyseat-0.0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,13 +34,13 @@
         'pyparsing>=3.0.9',
         'python-dateutil>=2.8.2',
         'pytz>=2022.2.1',
         'scikit-learn>=1.1.2',
         'scipy>=1.9.1',
         'seaborn>=0.12.0',
         'six>=1.16.0',
-        'sklearn>=0.0',
+        'scikit-learn>=0.0',
         'threadpoolctl>=3.1.0',
         'torch>=1.12.1',
         'typing_extensions>=4.3.0'
     ]
 )
```

