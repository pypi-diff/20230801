# Comparing `tmp/redvox-pandas-1.4.3.tar.gz` & `tmp/redvox-pandas-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redvox-pandas-1.4.3.tar", last modified: Tue Aug  1 18:59:35 2023, max compression
+gzip compressed data, was "redvox-pandas-1.4.4.tar", last modified: Tue Aug  1 19:56:54 2023, max compression
```

## Comparing `redvox-pandas-1.4.3.tar` & `redvox-pandas-1.4.4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-08-01 18:59:35.707134 redvox-pandas-1.4.3/
--rw-rw-r--   0 opq       (1000) opq       (1000)    11359 2021-07-02 00:27:05.000000 redvox-pandas-1.4.3/LICENSE
--rw-r--r--   0 opq       (1000) opq       (1000)    15648 2023-08-01 18:59:35.707134 redvox-pandas-1.4.3/PKG-INFO
--rw-r--r--   0 opq       (1000) opq       (1000)     2266 2023-04-27 21:26:24.000000 redvox-pandas-1.4.3/README.md
--rw-r--r--   0 opq       (1000) opq       (1000)      882 2023-08-01 18:47:31.000000 redvox-pandas-1.4.3/pyproject.toml
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-08-01 18:59:35.705134 redvox-pandas-1.4.3/redpandas/
--rw-rw-r--   0 opq       (1000) opq       (1000)      305 2022-07-07 20:44:53.000000 redvox-pandas-1.4.3/redpandas/__init__.py
--rw-r--r--   0 opq       (1000) opq       (1000)    19300 2023-04-27 21:26:25.000000 redvox-pandas-1.4.3/redpandas/redpd_build_station.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    15456 2022-07-07 20:44:53.000000 redvox-pandas-1.4.3/redpandas/redpd_cohere.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     6751 2021-08-03 22:13:07.000000 redvox-pandas-1.4.3/redpandas/redpd_config.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     4051 2022-07-07 20:44:53.000000 redvox-pandas-1.4.3/redpandas/redpd_datawin.py
--rw-r--r--   0 opq       (1000) opq       (1000)     4981 2023-04-27 21:26:25.000000 redvox-pandas-1.4.3/redpandas/redpd_df.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    14773 2022-07-07 20:44:53.000000 redvox-pandas-1.4.3/redpandas/redpd_dq.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    16853 2021-08-03 22:13:07.000000 redvox-pandas-1.4.3/redpandas/redpd_ensonify.py
--rw-rw-r--   0 opq       (1000) opq       (1000)      403 2021-10-18 19:57:34.000000 redvox-pandas-1.4.3/redpandas/redpd_errors.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    26898 2021-10-18 19:57:34.000000 redvox-pandas-1.4.3/redpandas/redpd_filter.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     8524 2022-07-07 20:44:53.000000 redvox-pandas-1.4.3/redpandas/redpd_geospatial.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     4200 2022-07-07 20:44:53.000000 redvox-pandas-1.4.3/redpandas/redpd_gravity.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     3790 2022-07-07 20:44:53.000000 redvox-pandas-1.4.3/redpandas/redpd_iterator.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     7874 2022-07-07 20:44:53.000000 redvox-pandas-1.4.3/redpandas/redpd_orientation.py
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-08-01 18:59:35.706134 redvox-pandas-1.4.3/redpandas/redpd_plot/
--rw-rw-r--   0 opq       (1000) opq       (1000)        0 2021-08-03 22:13:07.000000 redvox-pandas-1.4.3/redpandas/redpd_plot/__init__.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     4423 2021-08-03 22:13:07.000000 redvox-pandas-1.4.3/redpandas/redpd_plot/coherence.py
--rw-r--r--   0 opq       (1000) opq       (1000)    33263 2023-04-27 21:26:25.000000 redvox-pandas-1.4.3/redpandas/redpd_plot/mesh.py
--rw-rw-r--   0 opq       (1000) opq       (1000)      467 2021-10-18 19:57:34.000000 redvox-pandas-1.4.3/redpandas/redpd_plot/parameters.py
--rw-r--r--   0 opq       (1000) opq       (1000)    35442 2023-04-27 21:26:25.000000 redvox-pandas-1.4.3/redpandas/redpd_plot/wiggles.py
--rw-r--r--   0 opq       (1000) opq       (1000)    15627 2023-04-27 21:26:25.000000 redvox-pandas-1.4.3/redpandas/redpd_preprocess.py
--rw-r--r--   0 opq       (1000) opq       (1000)     8703 2023-04-27 21:26:25.000000 redvox-pandas-1.4.3/redpandas/redpd_report.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     1482 2022-07-07 20:44:53.000000 redvox-pandas-1.4.3/redpandas/redpd_scales.py
--rw-rw-r--   0 opq       (1000) opq       (1000)       80 2022-07-07 20:44:53.000000 redvox-pandas-1.4.3/redpandas/redpd_state.py
--rw-r--r--   0 opq       (1000) opq       (1000)    15899 2023-04-27 21:26:25.000000 redvox-pandas-1.4.3/redpandas/redpd_tfr.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    21018 2022-07-07 20:44:53.000000 redvox-pandas-1.4.3/redpandas/redpd_xcorr.py
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-08-01 18:59:35.706134 redvox-pandas-1.4.3/redvox_pandas.egg-info/
--rw-rw-r--   0 opq       (1000) opq       (1000)    15648 2023-08-01 18:59:35.000000 redvox-pandas-1.4.3/redvox_pandas.egg-info/PKG-INFO
--rw-rw-r--   0 opq       (1000) opq       (1000)      908 2023-08-01 18:59:35.000000 redvox-pandas-1.4.3/redvox_pandas.egg-info/SOURCES.txt
--rw-rw-r--   0 opq       (1000) opq       (1000)        1 2023-08-01 18:59:35.000000 redvox-pandas-1.4.3/redvox_pandas.egg-info/dependency_links.txt
--rw-rw-r--   0 opq       (1000) opq       (1000)       96 2023-08-01 18:59:35.000000 redvox-pandas-1.4.3/redvox_pandas.egg-info/requires.txt
--rw-rw-r--   0 opq       (1000) opq       (1000)       10 2023-08-01 18:59:35.000000 redvox-pandas-1.4.3/redvox_pandas.egg-info/top_level.txt
--rw-r--r--   0 opq       (1000) opq       (1000)       38 2023-08-01 18:59:35.707134 redvox-pandas-1.4.3/setup.cfg
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-08-01 19:56:54.350568 redvox-pandas-1.4.4/
+-rw-rw-r--   0 opq       (1000) opq       (1000)    11359 2021-07-02 00:27:05.000000 redvox-pandas-1.4.4/LICENSE
+-rw-r--r--   0 opq       (1000) opq       (1000)    15648 2023-08-01 19:56:54.350568 redvox-pandas-1.4.4/PKG-INFO
+-rw-r--r--   0 opq       (1000) opq       (1000)     2266 2023-04-27 21:26:24.000000 redvox-pandas-1.4.4/README.md
+-rw-r--r--   0 opq       (1000) opq       (1000)      910 2023-08-01 19:55:46.000000 redvox-pandas-1.4.4/pyproject.toml
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-08-01 19:56:54.349568 redvox-pandas-1.4.4/redpandas/
+-rw-rw-r--   0 opq       (1000) opq       (1000)      305 2022-07-07 20:44:53.000000 redvox-pandas-1.4.4/redpandas/__init__.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    19300 2023-04-27 21:26:25.000000 redvox-pandas-1.4.4/redpandas/redpd_build_station.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    15456 2022-07-07 20:44:53.000000 redvox-pandas-1.4.4/redpandas/redpd_cohere.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     6751 2021-08-03 22:13:07.000000 redvox-pandas-1.4.4/redpandas/redpd_config.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     4051 2022-07-07 20:44:53.000000 redvox-pandas-1.4.4/redpandas/redpd_datawin.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     4981 2023-04-27 21:26:25.000000 redvox-pandas-1.4.4/redpandas/redpd_df.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    14773 2022-07-07 20:44:53.000000 redvox-pandas-1.4.4/redpandas/redpd_dq.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    16853 2021-08-03 22:13:07.000000 redvox-pandas-1.4.4/redpandas/redpd_ensonify.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)      403 2021-10-18 19:57:34.000000 redvox-pandas-1.4.4/redpandas/redpd_errors.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    26898 2021-10-18 19:57:34.000000 redvox-pandas-1.4.4/redpandas/redpd_filter.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     8524 2022-07-07 20:44:53.000000 redvox-pandas-1.4.4/redpandas/redpd_geospatial.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     4200 2022-07-07 20:44:53.000000 redvox-pandas-1.4.4/redpandas/redpd_gravity.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     3790 2022-07-07 20:44:53.000000 redvox-pandas-1.4.4/redpandas/redpd_iterator.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     7874 2022-07-07 20:44:53.000000 redvox-pandas-1.4.4/redpandas/redpd_orientation.py
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-08-01 19:56:54.350568 redvox-pandas-1.4.4/redpandas/redpd_plot/
+-rw-rw-r--   0 opq       (1000) opq       (1000)        0 2021-08-03 22:13:07.000000 redvox-pandas-1.4.4/redpandas/redpd_plot/__init__.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     4423 2021-08-03 22:13:07.000000 redvox-pandas-1.4.4/redpandas/redpd_plot/coherence.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    33263 2023-04-27 21:26:25.000000 redvox-pandas-1.4.4/redpandas/redpd_plot/mesh.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)      467 2021-10-18 19:57:34.000000 redvox-pandas-1.4.4/redpandas/redpd_plot/parameters.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    35442 2023-04-27 21:26:25.000000 redvox-pandas-1.4.4/redpandas/redpd_plot/wiggles.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    15627 2023-04-27 21:26:25.000000 redvox-pandas-1.4.4/redpandas/redpd_preprocess.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     8703 2023-04-27 21:26:25.000000 redvox-pandas-1.4.4/redpandas/redpd_report.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     1482 2022-07-07 20:44:53.000000 redvox-pandas-1.4.4/redpandas/redpd_scales.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)       80 2022-07-07 20:44:53.000000 redvox-pandas-1.4.4/redpandas/redpd_state.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    15899 2023-04-27 21:26:25.000000 redvox-pandas-1.4.4/redpandas/redpd_tfr.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    21018 2022-07-07 20:44:53.000000 redvox-pandas-1.4.4/redpandas/redpd_xcorr.py
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-08-01 19:56:54.350568 redvox-pandas-1.4.4/redvox_pandas.egg-info/
+-rw-rw-r--   0 opq       (1000) opq       (1000)    15648 2023-08-01 19:56:54.000000 redvox-pandas-1.4.4/redvox_pandas.egg-info/PKG-INFO
+-rw-rw-r--   0 opq       (1000) opq       (1000)      908 2023-08-01 19:56:54.000000 redvox-pandas-1.4.4/redvox_pandas.egg-info/SOURCES.txt
+-rw-rw-r--   0 opq       (1000) opq       (1000)        1 2023-08-01 19:56:54.000000 redvox-pandas-1.4.4/redvox_pandas.egg-info/dependency_links.txt
+-rw-rw-r--   0 opq       (1000) opq       (1000)      102 2023-08-01 19:56:54.000000 redvox-pandas-1.4.4/redvox_pandas.egg-info/requires.txt
+-rw-rw-r--   0 opq       (1000) opq       (1000)       10 2023-08-01 19:56:54.000000 redvox-pandas-1.4.4/redvox_pandas.egg-info/top_level.txt
+-rw-r--r--   0 opq       (1000) opq       (1000)       38 2023-08-01 19:56:54.351568 redvox-pandas-1.4.4/setup.cfg
```

### Comparing `redvox-pandas-1.4.3/LICENSE` & `redvox-pandas-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `redvox-pandas-1.4.3/PKG-INFO` & `redvox-pandas-1.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redvox-pandas
-Version: 1.4.3
+Version: 1.4.4
 Summary: Library to streamline preprocessing of RedVox API 900 and API 1000 data
 Author-email: "RedVox, Inc" <support@redvox.io>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `redvox-pandas-1.4.3/README.md` & `redvox-pandas-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `redvox-pandas-1.4.3/pyproject.toml` & `redvox-pandas-1.4.4/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 # See:
 # - https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html
 # - https://packaging.python.org/en/latest/specifications/declaring-project-metadata/
 
 [project]
 name = "redvox-pandas"
-version = "1.4.3"
+version = "1.4.4"
 authors = [
     { name = "RedVox, Inc", email = "support@redvox.io" }
 ]
 description = "Library to streamline preprocessing of RedVox API 900 and API 1000 data"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 
 dependencies = [
+    "matplotlib==3.7.1",
+    "numpy==1.23.5",
     "obspy==1.4.0",
+    "pandas==2.0.1",
     "pymap3d==3.0.1",
-    "redvox==3.5.1",
-    "redvox-base[matplotlib,numpy,pandas,scipy]==2023.4.27"
+    "redvox==3.5.2",
+    "scipy==1.10.1",
 ]
 
 [project.urls]
 homepage = "https://github.com/RedVoxInc/redpandas"
 PyPI = "https://pypi.org/project/redpandas/"
 
 [build-system]
```

### Comparing `redvox-pandas-1.4.3/redpandas/redpd_build_station.py` & `redvox-pandas-1.4.4/redpandas/redpd_build_station.py`

 * *Files identical despite different names*

### Comparing `redvox-pandas-1.4.3/redpandas/redpd_cohere.py` & `redvox-pandas-1.4.4/redpandas/redpd_cohere.py`

 * *Files identical despite different names*

### Comparing `redvox-pandas-1.4.3/redpandas/redpd_config.py` & `redvox-pandas-1.4.4/redpandas/redpd_config.py`

 * *Files identical despite different names*

### Comparing `redvox-pandas-1.4.3/redpandas/redpd_datawin.py` & `redvox-pandas-1.4.4/redpandas/redpd_datawin.py`

 * *Files identical despite different names*

### Comparing `redvox-pandas-1.4.3/redpandas/redpd_df.py` & `redvox-pandas-1.4.4/redpandas/redpd_df.py`

 * *Files identical despite different names*

### Comparing `redvox-pandas-1.4.3/redpandas/redpd_dq.py` & `redvox-pandas-1.4.4/redpandas/redpd_dq.py`

 * *Files identical despite different names*

### Comparing `redvox-pandas-1.4.3/redpandas/redpd_ensonify.py` & `redvox-pandas-1.4.4/redpandas/redpd_ensonify.py`

 * *Files identical despite different names*

### Comparing `redvox-pandas-1.4.3/redpandas/redpd_filter.py` & `redvox-pandas-1.4.4/redpandas/redpd_filter.py`

 * *Files identical despite different names*

### Comparing `redvox-pandas-1.4.3/redpandas/redpd_geospatial.py` & `redvox-pandas-1.4.4/redpandas/redpd_geospatial.py`

 * *Files identical despite different names*

### Comparing `redvox-pandas-1.4.3/redpandas/redpd_gravity.py` & `redvox-pandas-1.4.4/redpandas/redpd_gravity.py`

 * *Files identical despite different names*

### Comparing `redvox-pandas-1.4.3/redpandas/redpd_iterator.py` & `redvox-pandas-1.4.4/redpandas/redpd_iterator.py`

 * *Files identical despite different names*

### Comparing `redvox-pandas-1.4.3/redpandas/redpd_orientation.py` & `redvox-pandas-1.4.4/redpandas/redpd_orientation.py`

 * *Files identical despite different names*

### Comparing `redvox-pandas-1.4.3/redpandas/redpd_plot/coherence.py` & `redvox-pandas-1.4.4/redpandas/redpd_plot/coherence.py`

 * *Files identical despite different names*

### Comparing `redvox-pandas-1.4.3/redpandas/redpd_plot/mesh.py` & `redvox-pandas-1.4.4/redpandas/redpd_plot/mesh.py`

 * *Files identical despite different names*

### Comparing `redvox-pandas-1.4.3/redpandas/redpd_plot/wiggles.py` & `redvox-pandas-1.4.4/redpandas/redpd_plot/wiggles.py`

 * *Files identical despite different names*

### Comparing `redvox-pandas-1.4.3/redpandas/redpd_preprocess.py` & `redvox-pandas-1.4.4/redpandas/redpd_preprocess.py`

 * *Files identical despite different names*

### Comparing `redvox-pandas-1.4.3/redpandas/redpd_report.py` & `redvox-pandas-1.4.4/redpandas/redpd_report.py`

 * *Files identical despite different names*

### Comparing `redvox-pandas-1.4.3/redpandas/redpd_scales.py` & `redvox-pandas-1.4.4/redpandas/redpd_scales.py`

 * *Files identical despite different names*

### Comparing `redvox-pandas-1.4.3/redpandas/redpd_tfr.py` & `redvox-pandas-1.4.4/redpandas/redpd_tfr.py`

 * *Files identical despite different names*

### Comparing `redvox-pandas-1.4.3/redpandas/redpd_xcorr.py` & `redvox-pandas-1.4.4/redpandas/redpd_xcorr.py`

 * *Files identical despite different names*

### Comparing `redvox-pandas-1.4.3/redvox_pandas.egg-info/PKG-INFO` & `redvox-pandas-1.4.4/redvox_pandas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redvox-pandas
-Version: 1.4.3
+Version: 1.4.4
 Summary: Library to streamline preprocessing of RedVox API 900 and API 1000 data
 Author-email: "RedVox, Inc" <support@redvox.io>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `redvox-pandas-1.4.3/redvox_pandas.egg-info/SOURCES.txt` & `redvox-pandas-1.4.4/redvox_pandas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

