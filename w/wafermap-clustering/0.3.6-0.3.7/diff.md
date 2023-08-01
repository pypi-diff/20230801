# Comparing `tmp/wafermap-clustering-0.3.6.tar.gz` & `tmp/wafermap-clustering-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wafermap-clustering-0.3.6.tar", last modified: Thu Jul 27 09:16:19 2023, max compression
+gzip compressed data, was "wafermap-clustering-0.3.7.tar", last modified: Tue Aug  1 08:04:48 2023, max compression
```

## Comparing `wafermap-clustering-0.3.6.tar` & `wafermap-clustering-0.3.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 09:16:19.234962 wafermap-clustering-0.3.6/
--rw-rw-rw-   0        0        0     1077 2023-01-23 09:00:52.000000 wafermap-clustering-0.3.6/LICENSE.txt
--rw-rw-rw-   0        0        0      568 2023-07-27 09:16:19.232898 wafermap-clustering-0.3.6/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-01-27 14:30:27.000000 wafermap-clustering-0.3.6/README.md
--rw-rw-rw-   0        0        0       42 2023-07-27 09:16:19.235696 wafermap-clustering-0.3.6/setup.cfg
--rw-rw-rw-   0        0        0      960 2023-07-27 09:15:51.000000 wafermap-clustering-0.3.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-27 09:16:19.188587 wafermap-clustering-0.3.6/tests/
--rw-rw-rw-   0        0        0    12755 2023-07-26 14:59:03.000000 wafermap-clustering-0.3.6/tests/test_clustering.py
-drwxrwxrwx   0        0        0        0 2023-07-27 09:16:19.194041 wafermap-clustering-0.3.6/wafermap_clustering/
-drwxrwxrwx   0        0        0        0 2023-07-27 09:16:19.217190 wafermap-clustering-0.3.6/wafermap_clustering/configs/
--rw-rw-rw-   0        0        0     3472 2023-06-27 08:34:33.000000 wafermap-clustering-0.3.6/wafermap_clustering/configs/config.py
-drwxrwxrwx   0        0        0        0 2023-07-27 09:16:19.219694 wafermap-clustering-0.3.6/wafermap_clustering/libs/
--rw-rw-rw-   0        0        0     4572 2023-07-26 14:53:07.000000 wafermap-clustering-0.3.6/wafermap_clustering/libs/klarf_lib.py
-drwxrwxrwx   0        0        0        0 2023-07-27 09:16:19.229390 wafermap-clustering-0.3.6/wafermap_clustering/models/
--rw-rw-rw-   0        0        0      125 2023-03-09 12:31:13.000000 wafermap-clustering-0.3.6/wafermap_clustering/models/clustered_defect.py
--rw-rw-rw-   0        0        0      468 2023-07-19 09:50:06.000000 wafermap-clustering-0.3.6/wafermap_clustering/models/clustering_performance.py
--rw-rw-rw-   0        0        0      854 2023-06-27 08:43:17.000000 wafermap-clustering-0.3.6/wafermap_clustering/models/clustering_result.py
--rw-rw-rw-   0        0        0     7008 2023-07-27 09:15:39.000000 wafermap-clustering-0.3.6/wafermap_clustering/wafermap_clustering.py
-drwxrwxrwx   0        0        0        0 2023-07-27 09:16:19.213862 wafermap-clustering-0.3.6/wafermap_clustering.egg-info/
--rw-rw-rw-   0        0        0      568 2023-07-27 09:16:19.000000 wafermap-clustering-0.3.6/wafermap_clustering.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      536 2023-07-27 09:16:19.000000 wafermap-clustering-0.3.6/wafermap_clustering.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 09:16:19.000000 wafermap-clustering-0.3.6/wafermap_clustering.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-07-27 09:16:19.000000 wafermap-clustering-0.3.6/wafermap_clustering.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-07-27 09:16:19.000000 wafermap-clustering-0.3.6/wafermap_clustering.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 08:04:48.306181 wafermap-clustering-0.3.7/
+-rw-rw-rw-   0        0        0     1077 2023-01-23 09:00:52.000000 wafermap-clustering-0.3.7/LICENSE.txt
+-rw-rw-rw-   0        0        0      568 2023-08-01 08:04:48.304739 wafermap-clustering-0.3.7/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-01-27 14:30:27.000000 wafermap-clustering-0.3.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-01 08:04:48.306703 wafermap-clustering-0.3.7/setup.cfg
+-rw-rw-rw-   0        0        0      960 2023-08-01 08:04:24.000000 wafermap-clustering-0.3.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 08:04:48.242053 wafermap-clustering-0.3.7/tests/
+-rw-rw-rw-   0        0        0    12755 2023-07-26 14:59:03.000000 wafermap-clustering-0.3.7/tests/test_clustering.py
+drwxrwxrwx   0        0        0        0 2023-08-01 08:04:48.246053 wafermap-clustering-0.3.7/wafermap_clustering/
+drwxrwxrwx   0        0        0        0 2023-08-01 08:04:48.276706 wafermap-clustering-0.3.7/wafermap_clustering/configs/
+-rw-rw-rw-   0        0        0     3472 2023-06-27 08:34:33.000000 wafermap-clustering-0.3.7/wafermap_clustering/configs/config.py
+drwxrwxrwx   0        0        0        0 2023-08-01 08:04:48.281376 wafermap-clustering-0.3.7/wafermap_clustering/libs/
+-rw-rw-rw-   0        0        0     4572 2023-07-26 14:53:07.000000 wafermap-clustering-0.3.7/wafermap_clustering/libs/klarf_lib.py
+drwxrwxrwx   0        0        0        0 2023-08-01 08:04:48.299248 wafermap-clustering-0.3.7/wafermap_clustering/models/
+-rw-rw-rw-   0        0        0      125 2023-03-09 12:31:13.000000 wafermap-clustering-0.3.7/wafermap_clustering/models/clustered_defect.py
+-rw-rw-rw-   0        0        0      468 2023-07-19 09:50:06.000000 wafermap-clustering-0.3.7/wafermap_clustering/models/clustering_performance.py
+-rw-rw-rw-   0        0        0      854 2023-06-27 08:43:17.000000 wafermap-clustering-0.3.7/wafermap_clustering/models/clustering_result.py
+-rw-rw-rw-   0        0        0     7826 2023-08-01 08:03:39.000000 wafermap-clustering-0.3.7/wafermap_clustering/wafermap_clustering.py
+drwxrwxrwx   0        0        0        0 2023-08-01 08:04:48.272700 wafermap-clustering-0.3.7/wafermap_clustering.egg-info/
+-rw-rw-rw-   0        0        0      568 2023-08-01 08:04:48.000000 wafermap-clustering-0.3.7/wafermap_clustering.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      536 2023-08-01 08:04:48.000000 wafermap-clustering-0.3.7/wafermap_clustering.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 08:04:48.000000 wafermap-clustering-0.3.7/wafermap_clustering.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-08-01 08:04:48.000000 wafermap-clustering-0.3.7/wafermap_clustering.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-08-01 08:04:48.000000 wafermap-clustering-0.3.7/wafermap_clustering.egg-info/top_level.txt
```

### Comparing `wafermap-clustering-0.3.6/LICENSE.txt` & `wafermap-clustering-0.3.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wafermap-clustering-0.3.6/PKG-INFO` & `wafermap-clustering-0.3.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: wafermap-clustering
-Version: 0.3.6
+Version: 0.3.7
 Summary: A project to apply clustering on wafermaps
 Home-page: https://github.com/Impro02/wafermap-clustering
-Download-URL: https://github.com/Impro02/wafermap-clustering/archive/refs/tags/0.3.6.tar.gz
+Download-URL: https://github.com/Impro02/wafermap-clustering/archive/refs/tags/0.3.7.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `wafermap-clustering-0.3.6/setup.py` & `wafermap-clustering-0.3.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = "0.3.6"
+version = "0.3.7"
 
 setup(
     name="wafermap-clustering",
     version=version,
     packages=[
         "wafermap_clustering",
         "wafermap_clustering.configs",
```

### Comparing `wafermap-clustering-0.3.6/tests/test_clustering.py` & `wafermap-clustering-0.3.7/tests/test_clustering.py`

 * *Files identical despite different names*

### Comparing `wafermap-clustering-0.3.6/wafermap_clustering/configs/config.py` & `wafermap-clustering-0.3.7/wafermap_clustering/configs/config.py`

 * *Files identical despite different names*

### Comparing `wafermap-clustering-0.3.6/wafermap_clustering/libs/klarf_lib.py` & `wafermap-clustering-0.3.7/wafermap_clustering/libs/klarf_lib.py`

 * *Files identical despite different names*

### Comparing `wafermap-clustering-0.3.6/wafermap_clustering/models/clustering_result.py` & `wafermap-clustering-0.3.7/wafermap_clustering/models/clustering_result.py`

 * *Files identical despite different names*

### Comparing `wafermap-clustering-0.3.6/wafermap_clustering/wafermap_clustering.py` & `wafermap-clustering-0.3.7/wafermap_clustering/wafermap_clustering.py`

 * *Files 7% similar despite different names*

```diff
@@ -59,35 +59,52 @@
                 clustering = HDBSCAN(
                     min_samples=self.config.clustering.hdbscan.min_samples,
                     min_cluster_size=self.config.clustering.hdbscan.min_cluster_size,
                 )
             case _:
                 raise ValueError(f"{clustering_mode=} is not supported")
 
+        self.logger.info(f"Prepare to cluster {len(klarf_content.wafers)} wafers")
+
         results: List[ClusteringResult] = []
         for index, wafer in enumerate(klarf_content.wafers):
             tic = time.time()
 
             single_klarf = klarf_convert.convert_to_single_klarf_content(
                 klarf_content=klarf_content, wafer_index=index
             )
 
+            lot = single_klarf.lot_id
+            wafer_id = single_klarf.wafer.id
+
+            self.logger.info(
+                f"Preparing to perform clustering for {lot=} and {wafer_id=} using {clustering_mode=}"
+            )
+
             if len(wafer.defects) == 0:
                 clusters = 0
                 clustered_defects = []
                 clustering_timestamp = 0
+
+                self.logger.info(f"{lot=} and {wafer_id=} do not have any defects")
             else:
                 defect_ids = np.array([defect.id for defect in wafer.defects])
                 defect_points = np.array(
                     [
                         (defect.point[0] / 1000, defect.point[1] / 1000)
                         for defect in wafer.defects
                     ]
                 )
 
+                self.logger.info(
+                    f"Starting clustering process for {lot=} and {wafer_id=} on {len(defect_points)} defects"
+                )
+
+                self.logger.info(f"{lot=} and {wafer_id=} do not have any defects")
+
                 labels = clustering.fit_predict(defect_points)
 
                 clustering_values = np.column_stack((defect_ids, labels))
                 clusters = len(np.unique(labels, axis=0))
 
                 clustered_defects = [
                     ClusteredDefect(
@@ -109,14 +126,18 @@
                 clusters=clusters,
                 clustered_defects=clustered_defects,
                 performance=ClusteringPerformance(
                     clustering_timestamp=round(clustering_timestamp, 3)
                 ),
             )
 
+            self.logger.info(
+                f"Clustering complete. Found {clusters} clusters on {len(clustered_defects)} defects."
+            )
+
             output_timestamp = None
             if klarf_format == KlarfFormat.BABY.value and output_directory is not None:
                 output_filename = (
                     output_directory
                     / f"{single_klarf.lot_id}_{single_klarf.step_id}_{single_klarf.wafer.id}_{clustering_mode}.000"
                 )
```

### Comparing `wafermap-clustering-0.3.6/wafermap_clustering.egg-info/PKG-INFO` & `wafermap-clustering-0.3.7/wafermap_clustering.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: wafermap-clustering
-Version: 0.3.6
+Version: 0.3.7
 Summary: A project to apply clustering on wafermaps
 Home-page: https://github.com/Impro02/wafermap-clustering
-Download-URL: https://github.com/Impro02/wafermap-clustering/archive/refs/tags/0.3.6.tar.gz
+Download-URL: https://github.com/Impro02/wafermap-clustering/archive/refs/tags/0.3.7.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `wafermap-clustering-0.3.6/wafermap_clustering.egg-info/SOURCES.txt` & `wafermap-clustering-0.3.7/wafermap_clustering.egg-info/SOURCES.txt`

 * *Files identical despite different names*

