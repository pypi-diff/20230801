# Comparing `tmp/pheno-utils-0.3.8.2.tar.gz` & `tmp/pheno-utils-0.3.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pheno-utils-0.3.8.2.tar", last modified: Tue Aug  1 14:14:30 2023, max compression
+gzip compressed data, was "pheno-utils-0.3.8.3.tar", last modified: Tue Aug  1 14:17:56 2023, max compression
```

## Comparing `pheno-utils-0.3.8.2.tar` & `pheno-utils-0.3.8.3.tar`

### file list

```diff
@@ -1,32 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 14:14:30.164953 pheno-utils-0.3.8.2/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-06-21 16:13:16.000000 pheno-utils-0.3.8.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      131 2023-08-01 14:12:49.000000 pheno-utils-0.3.8.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2361 2023-08-01 14:14:30.164071 pheno-utils-0.3.8.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1583 2023-07-26 07:07:45.000000 pheno-utils-0.3.8.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 14:14:30.121382 pheno-utils-0.3.8.2/pheno_utils/
--rw-r--r--   0 root         (0) root         (0)      344 2023-08-01 14:14:12.000000 pheno-utils-0.3.8.2/pheno_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19682 2023-08-01 14:14:12.000000 pheno-utils-0.3.8.2/pheno_utils/_modidx.py
--rw-r--r--   0 root         (0) root         (0)    16533 2023-08-01 14:14:12.000000 pheno-utils-0.3.8.2/pheno_utils/age_reference_plots.py
--rw-r--r--   0 root         (0) root         (0)     5530 2023-08-01 14:14:12.000000 pheno-utils-0.3.8.2/pheno_utils/basic_analysis.py
--rw-r--r--   0 root         (0) root         (0)    11559 2023-08-01 14:14:12.000000 pheno-utils-0.3.8.2/pheno_utils/basic_plots.py
--rw-r--r--   0 root         (0) root         (0)     2672 2023-08-01 14:14:12.000000 pheno-utils-0.3.8.2/pheno_utils/blandaltman_plots.py
--rw-r--r--   0 root         (0) root         (0)     7865 2023-08-01 14:14:12.000000 pheno-utils-0.3.8.2/pheno_utils/cgm_plots.py
--rw-r--r--   0 root         (0) root         (0)     3036 2023-08-01 14:14:12.000000 pheno-utils-0.3.8.2/pheno_utils/cohort_selector.py
--rw-r--r--   0 root         (0) root         (0)     4638 2023-08-01 14:14:12.000000 pheno-utils-0.3.8.2/pheno_utils/config.py
--rw-r--r--   0 root         (0) root         (0)     2825 2023-08-01 14:14:12.000000 pheno-utils-0.3.8.2/pheno_utils/dates_plots.py
--rw-r--r--   0 root         (0) root         (0)     2113 2023-08-01 14:14:12.000000 pheno-utils-0.3.8.2/pheno_utils/ecg_analysis.py
--rw-r--r--   0 root         (0) root         (0)     7781 2023-08-01 14:14:12.000000 pheno-utils-0.3.8.2/pheno_utils/meta_loader.py
--rw-r--r--   0 root         (0) root         (0)    20194 2023-08-01 14:14:12.000000 pheno-utils-0.3.8.2/pheno_utils/pheno_loader.py
--rw-r--r--   0 root         (0) root         (0)     1444 2023-08-01 14:14:12.000000 pheno-utils-0.3.8.2/pheno_utils/questionnaires_handler.py
--rw-r--r--   0 root         (0) root         (0)    13188 2023-08-01 14:14:12.000000 pheno-utils-0.3.8.2/pheno_utils/sleep_plots.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 14:14:30.159879 pheno-utils-0.3.8.2/pheno_utils.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2361 2023-08-01 14:14:29.000000 pheno-utils-0.3.8.2/pheno_utils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      722 2023-08-01 14:14:29.000000 pheno-utils-0.3.8.2/pheno_utils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 14:14:29.000000 pheno-utils-0.3.8.2/pheno_utils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-08-01 14:14:29.000000 pheno-utils-0.3.8.2/pheno_utils.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 16:16:15.000000 pheno-utils-0.3.8.2/pheno_utils.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      132 2023-08-01 14:14:29.000000 pheno-utils-0.3.8.2/pheno_utils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-08-01 14:14:29.000000 pheno-utils-0.3.8.2/pheno_utils.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      944 2023-08-01 14:14:09.000000 pheno-utils-0.3.8.2/settings.ini
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-01 14:14:30.165394 pheno-utils-0.3.8.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2591 2023-07-26 08:46:36.000000 pheno-utils-0.3.8.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 14:17:56.567335 pheno-utils-0.3.8.3/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-06-21 16:13:16.000000 pheno-utils-0.3.8.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      143 2023-08-01 14:17:35.000000 pheno-utils-0.3.8.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2361 2023-08-01 14:17:56.566128 pheno-utils-0.3.8.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1583 2023-07-26 07:07:45.000000 pheno-utils-0.3.8.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 14:17:56.430590 pheno-utils-0.3.8.3/config_setup/
+-rw-r--r--   0 root         (0) root         (0)      447 2023-07-25 08:54:34.000000 pheno-utils-0.3.8.3/config_setup/config_tre.json
+-rw-r--r--   0 root         (0) root         (0)     2696 2023-07-26 08:11:20.000000 pheno-utils-0.3.8.3/config_setup/create_default_config.py
+-rw-r--r--   0 root         (0) root         (0)      260 2023-07-20 12:24:23.000000 pheno-utils-0.3.8.3/config_setup/example_config.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 14:17:56.514035 pheno-utils-0.3.8.3/pheno_utils/
+-rw-r--r--   0 root         (0) root         (0)      344 2023-08-01 14:17:45.000000 pheno-utils-0.3.8.3/pheno_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19682 2023-08-01 14:17:45.000000 pheno-utils-0.3.8.3/pheno_utils/_modidx.py
+-rw-r--r--   0 root         (0) root         (0)    16533 2023-08-01 14:17:45.000000 pheno-utils-0.3.8.3/pheno_utils/age_reference_plots.py
+-rw-r--r--   0 root         (0) root         (0)     5530 2023-08-01 14:17:45.000000 pheno-utils-0.3.8.3/pheno_utils/basic_analysis.py
+-rw-r--r--   0 root         (0) root         (0)    11559 2023-08-01 14:17:45.000000 pheno-utils-0.3.8.3/pheno_utils/basic_plots.py
+-rw-r--r--   0 root         (0) root         (0)     2672 2023-08-01 14:17:45.000000 pheno-utils-0.3.8.3/pheno_utils/blandaltman_plots.py
+-rw-r--r--   0 root         (0) root         (0)     7865 2023-08-01 14:17:45.000000 pheno-utils-0.3.8.3/pheno_utils/cgm_plots.py
+-rw-r--r--   0 root         (0) root         (0)     3036 2023-08-01 14:17:45.000000 pheno-utils-0.3.8.3/pheno_utils/cohort_selector.py
+-rw-r--r--   0 root         (0) root         (0)     4638 2023-08-01 14:17:45.000000 pheno-utils-0.3.8.3/pheno_utils/config.py
+-rw-r--r--   0 root         (0) root         (0)     2825 2023-08-01 14:17:45.000000 pheno-utils-0.3.8.3/pheno_utils/dates_plots.py
+-rw-r--r--   0 root         (0) root         (0)     2113 2023-08-01 14:17:45.000000 pheno-utils-0.3.8.3/pheno_utils/ecg_analysis.py
+-rw-r--r--   0 root         (0) root         (0)     7781 2023-08-01 14:17:45.000000 pheno-utils-0.3.8.3/pheno_utils/meta_loader.py
+-rw-r--r--   0 root         (0) root         (0)    20194 2023-08-01 14:17:45.000000 pheno-utils-0.3.8.3/pheno_utils/pheno_loader.py
+-rw-r--r--   0 root         (0) root         (0)     1444 2023-08-01 14:17:45.000000 pheno-utils-0.3.8.3/pheno_utils/questionnaires_handler.py
+-rw-r--r--   0 root         (0) root         (0)    13188 2023-08-01 14:17:45.000000 pheno-utils-0.3.8.3/pheno_utils/sleep_plots.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 14:17:56.559769 pheno-utils-0.3.8.3/pheno_utils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2361 2023-08-01 14:17:56.000000 pheno-utils-0.3.8.3/pheno_utils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      822 2023-08-01 14:17:56.000000 pheno-utils-0.3.8.3/pheno_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 14:17:56.000000 pheno-utils-0.3.8.3/pheno_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-08-01 14:17:56.000000 pheno-utils-0.3.8.3/pheno_utils.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 16:16:15.000000 pheno-utils-0.3.8.3/pheno_utils.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      132 2023-08-01 14:17:56.000000 pheno-utils-0.3.8.3/pheno_utils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-08-01 14:17:56.000000 pheno-utils-0.3.8.3/pheno_utils.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      944 2023-08-01 14:17:41.000000 pheno-utils-0.3.8.3/settings.ini
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-01 14:17:56.567912 pheno-utils-0.3.8.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2591 2023-07-26 08:46:36.000000 pheno-utils-0.3.8.3/setup.py
```

### Comparing `pheno-utils-0.3.8.2/LICENSE` & `pheno-utils-0.3.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.8.2/PKG-INFO` & `pheno-utils-0.3.8.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pheno-utils
-Version: 0.3.8.2
+Version: 0.3.8.3
 Summary: Pheno data utils - viz, loaders, mergers
 Home-page: https://github.com/pheno-ai/pheno-utils
 Author: pheno.ai
 Author-email: hagai@pheno.ai
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pheno-utils-0.3.8.2/README.md` & `pheno-utils-0.3.8.3/README.md`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.8.2/pheno_utils/_modidx.py` & `pheno-utils-0.3.8.3/pheno_utils/_modidx.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.8.2/pheno_utils/age_reference_plots.py` & `pheno-utils-0.3.8.3/pheno_utils/age_reference_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.8.2/pheno_utils/basic_analysis.py` & `pheno-utils-0.3.8.3/pheno_utils/basic_analysis.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.8.2/pheno_utils/basic_plots.py` & `pheno-utils-0.3.8.3/pheno_utils/basic_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.8.2/pheno_utils/blandaltman_plots.py` & `pheno-utils-0.3.8.3/pheno_utils/blandaltman_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.8.2/pheno_utils/cgm_plots.py` & `pheno-utils-0.3.8.3/pheno_utils/cgm_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.8.2/pheno_utils/cohort_selector.py` & `pheno-utils-0.3.8.3/pheno_utils/cohort_selector.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.8.2/pheno_utils/config.py` & `pheno-utils-0.3.8.3/pheno_utils/config.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.8.2/pheno_utils/dates_plots.py` & `pheno-utils-0.3.8.3/pheno_utils/dates_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.8.2/pheno_utils/ecg_analysis.py` & `pheno-utils-0.3.8.3/pheno_utils/ecg_analysis.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.8.2/pheno_utils/meta_loader.py` & `pheno-utils-0.3.8.3/pheno_utils/meta_loader.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.8.2/pheno_utils/pheno_loader.py` & `pheno-utils-0.3.8.3/pheno_utils/pheno_loader.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.8.2/pheno_utils/questionnaires_handler.py` & `pheno-utils-0.3.8.3/pheno_utils/questionnaires_handler.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.8.2/pheno_utils/sleep_plots.py` & `pheno-utils-0.3.8.3/pheno_utils/sleep_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.8.2/pheno_utils.egg-info/PKG-INFO` & `pheno-utils-0.3.8.3/pheno_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pheno-utils
-Version: 0.3.8.2
+Version: 0.3.8.3
 Summary: Pheno data utils - viz, loaders, mergers
 Home-page: https://github.com/pheno-ai/pheno-utils
 Author: pheno.ai
 Author-email: hagai@pheno.ai
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pheno-utils-0.3.8.2/pheno_utils.egg-info/SOURCES.txt` & `pheno-utils-0.3.8.3/pheno_utils.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 LICENSE
 MANIFEST.in
 README.md
 settings.ini
 setup.py
+config_setup/config_tre.json
+config_setup/create_default_config.py
+config_setup/example_config.json
 pheno_utils/__init__.py
 pheno_utils/_modidx.py
 pheno_utils/age_reference_plots.py
 pheno_utils/basic_analysis.py
 pheno_utils/basic_plots.py
 pheno_utils/blandaltman_plots.py
 pheno_utils/cgm_plots.py
```

### Comparing `pheno-utils-0.3.8.2/settings.ini` & `pheno-utils-0.3.8.3/settings.ini`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = pheno-utils
 lib_name = pheno-utils
-version = 0.3.8.2
+version = 0.3.8.3
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = pheno_utils
 nbs_path = nbs
 recursive = True
```

### Comparing `pheno-utils-0.3.8.2/setup.py` & `pheno-utils-0.3.8.3/setup.py`

 * *Files identical despite different names*

