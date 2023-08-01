# Comparing `tmp/nids_datasets-0.1.3.tar.gz` & `tmp/nids_datasets-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nids_datasets-0.1.3.tar", last modified: Fri Jul 21 03:51:26 2023, max compression
+gzip compressed data, was "nids_datasets-0.1.4.tar", last modified: Tue Aug  1 15:52:18 2023, max compression
```

## Comparing `nids_datasets-0.1.3.tar` & `nids_datasets-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-21 03:51:26.465011 nids_datasets-0.1.3/
--rw-r--r--   0 rdp        (501) staff       (20)     8083 2023-07-21 03:51:26.464767 nids_datasets-0.1.3/PKG-INFO
--rw-r--r--   0 rdp        (501) staff       (20)     7489 2023-07-21 03:51:07.000000 nids_datasets-0.1.3/README.md
-drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-21 03:51:26.463674 nids_datasets-0.1.3/nids_datasets/
--rw-r--r--   0 rdp        (501) staff       (20)       41 2023-07-17 06:28:22.000000 nids_datasets-0.1.3/nids_datasets/__init__.py
--rw-r--r--   0 rdp        (501) staff       (20)    12833 2023-07-21 01:00:33.000000 nids_datasets-0.1.3/nids_datasets/dataset.py
-drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-21 03:51:26.464555 nids_datasets-0.1.3/nids_datasets.egg-info/
--rw-r--r--   0 rdp        (501) staff       (20)     8083 2023-07-21 03:51:26.000000 nids_datasets-0.1.3/nids_datasets.egg-info/PKG-INFO
--rw-r--r--   0 rdp        (501) staff       (20)      253 2023-07-21 03:51:26.000000 nids_datasets-0.1.3/nids_datasets.egg-info/SOURCES.txt
--rw-r--r--   0 rdp        (501) staff       (20)        1 2023-07-21 03:51:26.000000 nids_datasets-0.1.3/nids_datasets.egg-info/dependency_links.txt
--rw-r--r--   0 rdp        (501) staff       (20)       98 2023-07-21 03:51:26.000000 nids_datasets-0.1.3/nids_datasets.egg-info/requires.txt
--rw-r--r--   0 rdp        (501) staff       (20)       14 2023-07-21 03:51:26.000000 nids_datasets-0.1.3/nids_datasets.egg-info/top_level.txt
--rw-r--r--   0 rdp        (501) staff       (20)       38 2023-07-21 03:51:26.465061 nids_datasets-0.1.3/setup.cfg
--rw-r--r--   0 rdp        (501) staff       (20)      967 2023-07-21 03:51:14.000000 nids_datasets-0.1.3/setup.py
+drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-08-01 15:52:18.739567 nids_datasets-0.1.4/
+-rw-r--r--   0 rdp        (501) staff       (20)     8083 2023-08-01 15:52:18.739398 nids_datasets-0.1.4/PKG-INFO
+-rw-r--r--   0 rdp        (501) staff       (20)     7489 2023-07-21 03:51:07.000000 nids_datasets-0.1.4/README.md
+drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-08-01 15:52:18.738392 nids_datasets-0.1.4/nids_datasets/
+-rw-r--r--   0 rdp        (501) staff       (20)       41 2023-07-17 06:28:22.000000 nids_datasets-0.1.4/nids_datasets/__init__.py
+-rw-r--r--   0 rdp        (501) staff       (20)    12966 2023-08-01 15:34:32.000000 nids_datasets-0.1.4/nids_datasets/dataset.py
+drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-08-01 15:52:18.739195 nids_datasets-0.1.4/nids_datasets.egg-info/
+-rw-r--r--   0 rdp        (501) staff       (20)     8083 2023-08-01 15:52:18.000000 nids_datasets-0.1.4/nids_datasets.egg-info/PKG-INFO
+-rw-r--r--   0 rdp        (501) staff       (20)      253 2023-08-01 15:52:18.000000 nids_datasets-0.1.4/nids_datasets.egg-info/SOURCES.txt
+-rw-r--r--   0 rdp        (501) staff       (20)        1 2023-08-01 15:52:18.000000 nids_datasets-0.1.4/nids_datasets.egg-info/dependency_links.txt
+-rw-r--r--   0 rdp        (501) staff       (20)       98 2023-08-01 15:52:18.000000 nids_datasets-0.1.4/nids_datasets.egg-info/requires.txt
+-rw-r--r--   0 rdp        (501) staff       (20)       14 2023-08-01 15:52:18.000000 nids_datasets-0.1.4/nids_datasets.egg-info/top_level.txt
+-rw-r--r--   0 rdp        (501) staff       (20)       38 2023-08-01 15:52:18.739616 nids_datasets-0.1.4/setup.cfg
+-rw-r--r--   0 rdp        (501) staff       (20)      967 2023-08-01 15:52:04.000000 nids_datasets-0.1.4/setup.py
```

### Comparing `nids_datasets-0.1.3/PKG-INFO` & `nids_datasets-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nids_datasets
-Version: 0.1.3
+Version: 0.1.4
 Summary: Download and utilize specially curated and extracted datasets from the original UNSW-NB15 and CIC-IDS2017 datasets
 Home-page: https://github.com/rdpahalavan/nids-datasets
 Author: Pahalavan R D
 Author-email: rdpahalavan24@gmail.com
 License: Apache License 2.0
 Keywords: Dataset NIDS UNSW-NB15 CIC-IDS2017
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nids_datasets-0.1.3/README.md` & `nids_datasets-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `nids_datasets-0.1.3/nids_datasets/dataset.py` & `nids_datasets-0.1.4/nids_datasets/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,17 +22,21 @@
 
 
 class Dataset:
     def __init__(self, dataset=None, subset=None, files=None):
         self.dataset = dataset
         if subset == 'all':
             subset = ['Network-Flows', 'Packet-Fields', 'Packet-Bytes', 'Payload-Bytes']
+        elif isinstance(subset, str):
+            subset = [subset]
         self.subset = subset
         if files == 'all':
             files = [i for i in range(1, 19)]
+        elif isinstance(files, str):
+            files = [files]
         self.files = files
         if self.dataset == 'UNSW-NB15':
             self.flow_file = "UNSW_Flow"
         else:
             self.flow_file = "CICIDS_Flow"
 
     def download(self, use_cache=True):
```

### Comparing `nids_datasets-0.1.3/nids_datasets.egg-info/PKG-INFO` & `nids_datasets-0.1.4/nids_datasets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nids-datasets
-Version: 0.1.3
+Version: 0.1.4
 Summary: Download and utilize specially curated and extracted datasets from the original UNSW-NB15 and CIC-IDS2017 datasets
 Home-page: https://github.com/rdpahalavan/nids-datasets
 Author: Pahalavan R D
 Author-email: rdpahalavan24@gmail.com
 License: Apache License 2.0
 Keywords: Dataset NIDS UNSW-NB15 CIC-IDS2017
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nids_datasets-0.1.3/setup.py` & `nids_datasets-0.1.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = f.read().splitlines()
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name='nids_datasets',
-    version='0.1.3',
+    version='0.1.4',
     description="Download and utilize specially curated and extracted datasets from the original UNSW-NB15 and CIC-IDS2017 datasets",
     keywords="Dataset NIDS UNSW-NB15 CIC-IDS2017",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='Apache License 2.0',
     author="Pahalavan R D",
     author_email='rdpahalavan24@gmail.com',
```

