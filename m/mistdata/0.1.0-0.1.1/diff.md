# Comparing `tmp/mistdata-0.1.0.tar.gz` & `tmp/mistdata-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mistdata-0.1.0.tar", max compression
+gzip compressed data, was "mistdata-0.1.1.tar", max compression
```

## Comparing `mistdata-0.1.0.tar` & `mistdata-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rwxr-xr-x   0        0        0      492 2023-08-01 19:10:48.556361 mistdata-0.1.0/pyproject.toml
--rwxr-xr-x   0        0        0     5140 2023-08-01 17:24:24.208711 mistdata-0.1.0/src/mistdata/DUTLNA.py
--rwxr-xr-x   0        0        0     7141 2023-08-01 17:24:18.076926 mistdata-0.1.0/src/mistdata/DUTRecIn.py
--rwxr-xr-x   0        0        0    15403 2023-07-27 18:26:10.520310 mistdata-0.1.0/src/mistdata/LSTBinnedSpectra.py
--rwxr-xr-x   0        0        0    14434 2023-08-01 18:21:42.707859 mistdata-0.1.0/src/mistdata/MISTData.py
--rwxr-xr-x   0        0        0     6714 2023-03-14 16:00:54.080090 mistdata-0.1.0/src/mistdata/MISTData_methods/plotting_raw.py
--rwxr-xr-x   0        0        0    10889 2023-08-01 18:21:42.711860 mistdata-0.1.0/src/mistdata/Spectrum.py
--rwxr-xr-x   0        0        0     4853 2023-08-01 17:24:14.769042 mistdata-0.1.0/src/mistdata/Thermistors.py
--rwxr-xr-x   0        0        0      220 2023-05-31 19:42:31.918863 mistdata-0.1.0/src/mistdata/__init__.py
--rwxr-xr-x   0        0        0     4144 2023-08-01 18:54:05.611076 mistdata-0.1.0/src/mistdata/plotting.py
--rwxr-xr-x   0        0        0     2626 2023-07-27 18:22:17.953544 mistdata-0.1.0/src/mistdata/utils.py
--rw-r--r--   0        0        0      619 1970-01-01 00:00:00.000000 mistdata-0.1.0/PKG-INFO
+-rwxr-xr-x   0        0        0      492 2023-08-01 19:22:08.194503 mistdata-0.1.1/pyproject.toml
+-rwxr-xr-x   0        0        0     5140 2023-08-01 17:24:24.208711 mistdata-0.1.1/src/mistdata/DUTLNA.py
+-rwxr-xr-x   0        0        0     7141 2023-08-01 17:24:18.076926 mistdata-0.1.1/src/mistdata/DUTRecIn.py
+-rwxr-xr-x   0        0        0    15403 2023-07-27 18:26:10.520310 mistdata-0.1.1/src/mistdata/LSTBinnedSpectra.py
+-rwxr-xr-x   0        0        0    14434 2023-08-01 18:21:42.707859 mistdata-0.1.1/src/mistdata/MISTData.py
+-rwxr-xr-x   0        0        0     6714 2023-03-14 16:00:54.080090 mistdata-0.1.1/src/mistdata/MISTData_methods/plotting_raw.py
+-rwxr-xr-x   0        0        0    10889 2023-08-01 18:21:42.711860 mistdata-0.1.1/src/mistdata/Spectrum.py
+-rwxr-xr-x   0        0        0     4853 2023-08-01 17:24:14.769042 mistdata-0.1.1/src/mistdata/Thermistors.py
+-rwxr-xr-x   0        0        0      220 2023-05-31 19:42:31.918863 mistdata-0.1.1/src/mistdata/__init__.py
+-rwxr-xr-x   0        0        0     4144 2023-08-01 18:54:05.611076 mistdata-0.1.1/src/mistdata/plotting.py
+-rwxr-xr-x   0        0        0     2626 2023-07-27 18:22:17.953544 mistdata-0.1.1/src/mistdata/utils.py
+-rw-r--r--   0        0        0      619 1970-01-01 00:00:00.000000 mistdata-0.1.1/PKG-INFO
```

### Comparing `mistdata-0.1.0/src/mistdata/DUTLNA.py` & `mistdata-0.1.1/src/mistdata/DUTLNA.py`

 * *Files identical despite different names*

### Comparing `mistdata-0.1.0/src/mistdata/DUTRecIn.py` & `mistdata-0.1.1/src/mistdata/DUTRecIn.py`

 * *Files identical despite different names*

### Comparing `mistdata-0.1.0/src/mistdata/LSTBinnedSpectra.py` & `mistdata-0.1.1/src/mistdata/LSTBinnedSpectra.py`

 * *Files identical despite different names*

### Comparing `mistdata-0.1.0/src/mistdata/MISTData.py` & `mistdata-0.1.1/src/mistdata/MISTData.py`

 * *Files identical despite different names*

### Comparing `mistdata-0.1.0/src/mistdata/MISTData_methods/plotting_raw.py` & `mistdata-0.1.1/src/mistdata/MISTData_methods/plotting_raw.py`

 * *Files identical despite different names*

### Comparing `mistdata-0.1.0/src/mistdata/Spectrum.py` & `mistdata-0.1.1/src/mistdata/Spectrum.py`

 * *Files identical despite different names*

### Comparing `mistdata-0.1.0/src/mistdata/Thermistors.py` & `mistdata-0.1.1/src/mistdata/Thermistors.py`

 * *Files identical despite different names*

### Comparing `mistdata-0.1.0/src/mistdata/plotting.py` & `mistdata-0.1.1/src/mistdata/plotting.py`

 * *Files identical despite different names*

### Comparing `mistdata-0.1.0/src/mistdata/utils.py` & `mistdata-0.1.1/src/mistdata/utils.py`

 * *Files identical despite different names*

### Comparing `mistdata-0.1.0/PKG-INFO` & `mistdata-0.1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mistdata
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Vadym Bidula
 Author-email: vadym.bidula@gmail.com
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

