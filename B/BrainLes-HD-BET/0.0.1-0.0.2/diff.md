# Comparing `tmp/BrainLes_HD-BET-0.0.1.tar.gz` & `tmp/BrainLes_HD-BET-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BrainLes_HD-BET-0.0.1.tar", last modified: Tue Aug  1 09:46:17 2023, max compression
+gzip compressed data, was "BrainLes_HD-BET-0.0.2.tar", last modified: Tue Aug  1 10:13:10 2023, max compression
```

## Comparing `BrainLes_HD-BET-0.0.1.tar` & `BrainLes_HD-BET-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 florian   (1001) florian   (1001)        0 2023-08-01 09:46:17.324365 BrainLes_HD-BET-0.0.1/
-drwxrwxr-x   0 florian   (1001) florian   (1001)        0 2023-08-01 09:46:17.324365 BrainLes_HD-BET-0.0.1/BrainLes_HD_BET.egg-info/
--rw-rw-r--   0 florian   (1001) florian   (1001)      662 2023-08-01 09:46:17.000000 BrainLes_HD-BET-0.0.1/BrainLes_HD_BET.egg-info/PKG-INFO
--rw-rw-r--   0 florian   (1001) florian   (1001)      490 2023-08-01 09:46:17.000000 BrainLes_HD-BET-0.0.1/BrainLes_HD_BET.egg-info/SOURCES.txt
--rw-rw-r--   0 florian   (1001) florian   (1001)        1 2023-08-01 09:46:17.000000 BrainLes_HD-BET-0.0.1/BrainLes_HD_BET.egg-info/dependency_links.txt
--rw-rw-r--   0 florian   (1001) florian   (1001)       55 2023-08-01 09:46:17.000000 BrainLes_HD-BET-0.0.1/BrainLes_HD_BET.egg-info/entry_points.txt
--rw-rw-r--   0 florian   (1001) florian   (1001)       56 2023-08-01 09:46:17.000000 BrainLes_HD-BET-0.0.1/BrainLes_HD_BET.egg-info/requires.txt
--rw-rw-r--   0 florian   (1001) florian   (1001)       16 2023-08-01 09:46:17.000000 BrainLes_HD-BET-0.0.1/BrainLes_HD_BET.egg-info/top_level.txt
--rw-rw-r--   0 florian   (1001) florian   (1001)    11356 2023-08-01 08:40:39.000000 BrainLes_HD-BET-0.0.1/LICENSE
--rw-rw-r--   0 florian   (1001) florian   (1001)      662 2023-08-01 09:46:17.324365 BrainLes_HD-BET-0.0.1/PKG-INFO
-drwxrwxr-x   0 florian   (1001) florian   (1001)        0 2023-08-01 09:46:17.324365 BrainLes_HD-BET-0.0.1/brainles_hd_bet/
--rw-rw-r--   0 florian   (1001) florian   (1001)        0 2023-08-01 08:40:39.000000 BrainLes_HD-BET-0.0.1/brainles_hd_bet/__init__.py
--rwxrwxr-x   0 florian   (1001) florian   (1001)     3765 2023-08-01 08:40:55.000000 BrainLes_HD-BET-0.0.1/brainles_hd_bet/config.py
--rwxrwxr-x   0 florian   (1001) florian   (1001)     4798 2023-08-01 08:40:39.000000 BrainLes_HD-BET-0.0.1/brainles_hd_bet/data_loading.py
--rwxrwxr-x   0 florian   (1001) florian   (1001)     5832 2023-08-01 09:16:51.000000 BrainLes_HD-BET-0.0.1/brainles_hd_bet/hd_bet.py
--rwxrwxr-x   0 florian   (1001) florian   (1001)    10665 2023-08-01 08:40:55.000000 BrainLes_HD-BET-0.0.1/brainles_hd_bet/network_architecture.py
--rwxrwxr-x   0 florian   (1001) florian   (1001)     5558 2023-08-01 08:40:39.000000 BrainLes_HD-BET-0.0.1/brainles_hd_bet/predict_case.py
--rwxrwxr-x   0 florian   (1001) florian   (1001)     4615 2023-08-01 09:12:46.000000 BrainLes_HD-BET-0.0.1/brainles_hd_bet/run.py
--rwxrwxr-x   0 florian   (1001) florian   (1001)     4067 2023-08-01 09:44:48.000000 BrainLes_HD-BET-0.0.1/brainles_hd_bet/utils.py
--rw-rw-r--   0 florian   (1001) florian   (1001)     1260 2023-08-01 09:23:29.000000 BrainLes_HD-BET-0.0.1/pyproject.toml
--rw-rw-r--   0 florian   (1001) florian   (1001)       38 2023-08-01 09:46:17.324365 BrainLes_HD-BET-0.0.1/setup.cfg
+drwxrwxr-x   0 florian   (1001) florian   (1001)        0 2023-08-01 10:13:10.424228 BrainLes_HD-BET-0.0.2/
+drwxrwxr-x   0 florian   (1001) florian   (1001)        0 2023-08-01 10:13:10.424228 BrainLes_HD-BET-0.0.2/BrainLes_HD_BET.egg-info/
+-rw-rw-r--   0 florian   (1001) florian   (1001)      662 2023-08-01 10:13:10.000000 BrainLes_HD-BET-0.0.2/BrainLes_HD_BET.egg-info/PKG-INFO
+-rw-rw-r--   0 florian   (1001) florian   (1001)      490 2023-08-01 10:13:10.000000 BrainLes_HD-BET-0.0.2/BrainLes_HD_BET.egg-info/SOURCES.txt
+-rw-rw-r--   0 florian   (1001) florian   (1001)        1 2023-08-01 10:13:10.000000 BrainLes_HD-BET-0.0.2/BrainLes_HD_BET.egg-info/dependency_links.txt
+-rw-rw-r--   0 florian   (1001) florian   (1001)       55 2023-08-01 10:13:10.000000 BrainLes_HD-BET-0.0.2/BrainLes_HD_BET.egg-info/entry_points.txt
+-rw-rw-r--   0 florian   (1001) florian   (1001)       79 2023-08-01 10:13:10.000000 BrainLes_HD-BET-0.0.2/BrainLes_HD_BET.egg-info/requires.txt
+-rw-rw-r--   0 florian   (1001) florian   (1001)       16 2023-08-01 10:13:10.000000 BrainLes_HD-BET-0.0.2/BrainLes_HD_BET.egg-info/top_level.txt
+-rw-rw-r--   0 florian   (1001) florian   (1001)    11356 2023-08-01 08:40:39.000000 BrainLes_HD-BET-0.0.2/LICENSE
+-rw-rw-r--   0 florian   (1001) florian   (1001)      662 2023-08-01 10:13:10.424228 BrainLes_HD-BET-0.0.2/PKG-INFO
+drwxrwxr-x   0 florian   (1001) florian   (1001)        0 2023-08-01 10:13:10.424228 BrainLes_HD-BET-0.0.2/brainles_hd_bet/
+-rw-rw-r--   0 florian   (1001) florian   (1001)        0 2023-08-01 08:40:39.000000 BrainLes_HD-BET-0.0.2/brainles_hd_bet/__init__.py
+-rwxrwxr-x   0 florian   (1001) florian   (1001)     3765 2023-08-01 08:40:55.000000 BrainLes_HD-BET-0.0.2/brainles_hd_bet/config.py
+-rwxrwxr-x   0 florian   (1001) florian   (1001)     4798 2023-08-01 08:40:39.000000 BrainLes_HD-BET-0.0.2/brainles_hd_bet/data_loading.py
+-rwxrwxr-x   0 florian   (1001) florian   (1001)     5832 2023-08-01 09:16:51.000000 BrainLes_HD-BET-0.0.2/brainles_hd_bet/hd_bet.py
+-rwxrwxr-x   0 florian   (1001) florian   (1001)    10665 2023-08-01 08:40:55.000000 BrainLes_HD-BET-0.0.2/brainles_hd_bet/network_architecture.py
+-rwxrwxr-x   0 florian   (1001) florian   (1001)     5558 2023-08-01 08:40:39.000000 BrainLes_HD-BET-0.0.2/brainles_hd_bet/predict_case.py
+-rwxrwxr-x   0 florian   (1001) florian   (1001)     4615 2023-08-01 09:12:46.000000 BrainLes_HD-BET-0.0.2/brainles_hd_bet/run.py
+-rwxrwxr-x   0 florian   (1001) florian   (1001)     4067 2023-08-01 09:44:48.000000 BrainLes_HD-BET-0.0.2/brainles_hd_bet/utils.py
+-rw-rw-r--   0 florian   (1001) florian   (1001)     1294 2023-08-01 10:13:01.000000 BrainLes_HD-BET-0.0.2/pyproject.toml
+-rw-rw-r--   0 florian   (1001) florian   (1001)       38 2023-08-01 10:13:10.424228 BrainLes_HD-BET-0.0.2/setup.cfg
```

### Comparing `BrainLes_HD-BET-0.0.1/BrainLes_HD_BET.egg-info/PKG-INFO` & `BrainLes_HD-BET-0.0.2/BrainLes_HD_BET.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BrainLes-HD-BET
-Version: 0.0.1
+Version: 0.0.2
 Summary: TODO.
 Author-email: Florian Kofler <florian.kofler@tum.de>, Isra Mekki <isra.mekki@helmholtz-muenchen.de>
 Maintainer-email: Florian Kofler <florian.kofler@tum.de>, Isra Mekki <isra.mekki@helmholtz-muenchen.de>
 Project-URL: repository, https://github.com/neuronflow/BrainLes
 Keywords: Brain extraction, skull stripping
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `BrainLes_HD-BET-0.0.1/LICENSE` & `BrainLes_HD-BET-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `BrainLes_HD-BET-0.0.1/PKG-INFO` & `BrainLes_HD-BET-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BrainLes_HD-BET
-Version: 0.0.1
+Version: 0.0.2
 Summary: TODO.
 Author-email: Florian Kofler <florian.kofler@tum.de>, Isra Mekki <isra.mekki@helmholtz-muenchen.de>
 Maintainer-email: Florian Kofler <florian.kofler@tum.de>, Isra Mekki <isra.mekki@helmholtz-muenchen.de>
 Project-URL: repository, https://github.com/neuronflow/BrainLes
 Keywords: Brain extraction, skull stripping
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `BrainLes_HD-BET-0.0.1/brainles_hd_bet/config.py` & `BrainLes_HD-BET-0.0.2/brainles_hd_bet/config.py`

 * *Files identical despite different names*

### Comparing `BrainLes_HD-BET-0.0.1/brainles_hd_bet/data_loading.py` & `BrainLes_HD-BET-0.0.2/brainles_hd_bet/data_loading.py`

 * *Files identical despite different names*

### Comparing `BrainLes_HD-BET-0.0.1/brainles_hd_bet/hd_bet.py` & `BrainLes_HD-BET-0.0.2/brainles_hd_bet/hd_bet.py`

 * *Files identical despite different names*

### Comparing `BrainLes_HD-BET-0.0.1/brainles_hd_bet/network_architecture.py` & `BrainLes_HD-BET-0.0.2/brainles_hd_bet/network_architecture.py`

 * *Files identical despite different names*

### Comparing `BrainLes_HD-BET-0.0.1/brainles_hd_bet/predict_case.py` & `BrainLes_HD-BET-0.0.2/brainles_hd_bet/predict_case.py`

 * *Files identical despite different names*

### Comparing `BrainLes_HD-BET-0.0.1/brainles_hd_bet/run.py` & `BrainLes_HD-BET-0.0.2/brainles_hd_bet/run.py`

 * *Files identical despite different names*

### Comparing `BrainLes_HD-BET-0.0.1/brainles_hd_bet/utils.py` & `BrainLes_HD-BET-0.0.2/brainles_hd_bet/utils.py`

 * *Files identical despite different names*

### Comparing `BrainLes_HD-BET-0.0.1/pyproject.toml` & `BrainLes_HD-BET-0.0.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 [tool.setuptools_scm]
 write_to = "brainles_hd_bet/_version.py"
 
 [project]
 name = "BrainLes_HD-BET"
 requires-python = ">=3.5"
 # dynamic = ["version"]
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name = "Florian Kofler", email = "florian.kofler@tum.de" },
   { name = "Isra Mekki", email = "isra.mekki@helmholtz-muenchen.de" },
 ]
 maintainers = [
   { name = "Florian Kofler", email = "florian.kofler@tum.de" },
   { name = "Isra Mekki", email = "isra.mekki@helmholtz-muenchen.de" },
@@ -30,15 +30,20 @@
 # requires-python = "==3.10"
 classifiers = [
   "Programming Language :: Python :: 3",
   # TODO check license issues
   "License :: OSI Approved :: GNU Affero General Public License v3",
   "Operating System :: OS Independent",
 ]
-dependencies = ['numpy', 'torch>=0.4.1', 'scikit-image', 'SimpleITK']
+dependencies = [
+  'numpy==1.24.0',
+  'torch>=0.4.1',
+  'scikit-image==0.21.0',
+  'SimpleITK==2.2.1',
+]
 
 [project.scripts]
 hd-bet = "brainles_hd_bet:hd_bet.main"
 
 [project.optional-dependencies]
 dev = ["pytest"]
```

