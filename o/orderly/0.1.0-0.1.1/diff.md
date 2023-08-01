# Comparing `tmp/orderly-0.1.0.tar.gz` & `tmp/orderly-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orderly-0.1.0.tar", last modified: Tue Aug  1 12:38:57 2023, max compression
+gzip compressed data, was "orderly-0.1.1.tar", last modified: Tue Aug  1 16:00:38 2023, max compression
```

## Comparing `orderly-0.1.0.tar` & `orderly-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,46 @@
-drwxr-xr-x   0 dsw46      (502) staff       (20)        0 2023-08-01 12:38:57.450646 orderly-0.1.0/
--rw-r--r--   0 dsw46      (502) staff       (20)      390 2023-04-14 18:37:02.000000 orderly-0.1.0/AUTHORS
--rw-r--r--   0 dsw46      (502) staff       (20)     1079 2023-07-03 14:56:10.000000 orderly-0.1.0/LICENSE
--rw-r--r--   0 dsw46      (502) staff       (20)     8971 2023-08-01 12:38:57.450365 orderly-0.1.0/PKG-INFO
--rw-r--r--   0 dsw46      (502) staff       (20)     8718 2023-08-01 12:20:44.000000 orderly-0.1.0/README.md
-drwxr-xr-x   0 dsw46      (502) staff       (20)        0 2023-08-01 12:38:57.447829 orderly-0.1.0/orderly/
--rw-r--r--   0 dsw46      (502) staff       (20)      315 2023-07-31 10:25:49.000000 orderly-0.1.0/orderly/__init__.py
--rw-r--r--   0 dsw46      (502) staff       (20)     1934 2023-05-02 14:22:54.000000 orderly-0.1.0/orderly/types.py
-drwxr-xr-x   0 dsw46      (502) staff       (20)        0 2023-08-01 12:38:57.448798 orderly-0.1.0/orderly.egg-info/
--rw-r--r--   0 dsw46      (502) staff       (20)     8971 2023-08-01 12:38:57.000000 orderly-0.1.0/orderly.egg-info/PKG-INFO
--rw-r--r--   0 dsw46      (502) staff       (20)      271 2023-08-01 12:38:57.000000 orderly-0.1.0/orderly.egg-info/SOURCES.txt
--rw-r--r--   0 dsw46      (502) staff       (20)        1 2023-08-01 12:38:57.000000 orderly-0.1.0/orderly.egg-info/dependency_links.txt
--rw-r--r--   0 dsw46      (502) staff       (20)        8 2023-08-01 12:38:57.000000 orderly-0.1.0/orderly.egg-info/top_level.txt
--rw-r--r--   0 dsw46      (502) staff       (20)     1140 2023-07-03 14:56:10.000000 orderly-0.1.0/pyproject.toml
--rw-r--r--   0 dsw46      (502) staff       (20)       38 2023-08-01 12:38:57.450690 orderly-0.1.0/setup.cfg
--rw-r--r--   0 dsw46      (502) staff       (20)      655 2023-08-01 12:38:05.000000 orderly-0.1.0/setup.py
-drwxr-xr-x   0 dsw46      (502) staff       (20)        0 2023-08-01 12:38:57.449899 orderly-0.1.0/tests/
--rw-r--r--   0 dsw46      (502) staff       (20)    44246 2023-07-03 14:56:10.000000 orderly-0.1.0/tests/test_clean.py
--rw-r--r--   0 dsw46      (502) staff       (20)     1548 2023-04-14 18:37:02.000000 orderly-0.1.0/tests/test_data.py
--rw-r--r--   0 dsw46      (502) staff       (20)    60769 2023-07-03 14:56:10.000000 orderly-0.1.0/tests/test_extract.py
+drwxr-xr-x   0 dsw46      (502) staff       (20)        0 2023-08-01 16:00:38.764308 orderly-0.1.1/
+-rw-r--r--   0 dsw46      (502) staff       (20)      390 2023-04-14 18:37:02.000000 orderly-0.1.1/AUTHORS
+-rw-r--r--   0 dsw46      (502) staff       (20)     1079 2023-07-03 14:56:10.000000 orderly-0.1.1/LICENSE
+-rw-r--r--   0 dsw46      (502) staff       (20)     8988 2023-08-01 16:00:38.763792 orderly-0.1.1/PKG-INFO
+-rw-r--r--   0 dsw46      (502) staff       (20)     8735 2023-08-01 13:33:37.000000 orderly-0.1.1/README.md
+drwxr-xr-x   0 dsw46      (502) staff       (20)        0 2023-08-01 16:00:38.757957 orderly-0.1.1/orderly/
+-rw-r--r--   0 dsw46      (502) staff       (20)      303 2023-08-01 14:43:23.000000 orderly-0.1.1/orderly/__init__.py
+drwxr-xr-x   0 dsw46      (502) staff       (20)        0 2023-08-01 16:00:38.758894 orderly-0.1.1/orderly/clean/
+-rw-r--r--   0 dsw46      (502) staff       (20)        0 2023-04-07 16:58:29.000000 orderly-0.1.1/orderly/clean/__init__.py
+-rw-r--r--   0 dsw46      (502) staff       (20)       60 2023-07-31 10:30:36.000000 orderly-0.1.1/orderly/clean/__main__.py
+-rw-r--r--   0 dsw46      (502) staff       (20)    59481 2023-07-31 09:04:20.000000 orderly-0.1.1/orderly/clean/cleaner.py
+drwxr-xr-x   0 dsw46      (502) staff       (20)        0 2023-08-01 16:00:38.760100 orderly-0.1.1/orderly/data/
+-rw-r--r--   0 dsw46      (502) staff       (20)      187 2023-04-07 16:58:29.000000 orderly-0.1.1/orderly/data/__init__.py
+-rw-r--r--   0 dsw46      (502) staff       (20)    68519 2023-07-03 14:56:10.000000 orderly-0.1.1/orderly/data/solvents.csv
+-rw-r--r--   0 dsw46      (502) staff       (20)     2151 2023-05-10 22:43:33.000000 orderly-0.1.1/orderly/data/solvents.py
+-rw-r--r--   0 dsw46      (502) staff       (20)     1201 2023-04-18 12:10:09.000000 orderly-0.1.1/orderly/data/test_data.py
+-rw-r--r--   0 dsw46      (502) staff       (20)      570 2023-04-18 12:10:09.000000 orderly-0.1.1/orderly/data/util.py
+drwxr-xr-x   0 dsw46      (502) staff       (20)        0 2023-08-01 16:00:38.761989 orderly-0.1.1/orderly/extract/
+-rw-r--r--   0 dsw46      (502) staff       (20)        0 2023-04-07 16:58:29.000000 orderly-0.1.1/orderly/extract/__init__.py
+-rw-r--r--   0 dsw46      (502) staff       (20)       59 2023-04-16 19:08:44.000000 orderly-0.1.1/orderly/extract/__main__.py
+-rw-r--r--   0 dsw46      (502) staff       (20)     2733 2023-05-10 22:43:33.000000 orderly-0.1.1/orderly/extract/canonicalise.py
+-rw-r--r--   0 dsw46      (502) staff       (20)     7091 2023-05-10 22:43:33.000000 orderly-0.1.1/orderly/extract/defaults.py
+-rw-r--r--   0 dsw46      (502) staff       (20)    54067 2023-07-03 14:56:10.000000 orderly-0.1.1/orderly/extract/extractor.py
+-rw-r--r--   0 dsw46      (502) staff       (20)    32943 2023-07-03 14:56:10.000000 orderly-0.1.1/orderly/extract/main.py
+drwxr-xr-x   0 dsw46      (502) staff       (20)        0 2023-08-01 16:00:38.762504 orderly-0.1.1/orderly/gen_fp/
+-rw-r--r--   0 dsw46      (502) staff       (20)        0 2023-05-21 10:18:04.000000 orderly-0.1.1/orderly/gen_fp/__init__.py
+-rw-r--r--   0 dsw46      (502) staff       (20)       70 2023-05-21 10:18:04.000000 orderly-0.1.1/orderly/gen_fp/__main__.py
+-rw-r--r--   0 dsw46      (502) staff       (20)     6592 2023-07-03 14:56:10.000000 orderly-0.1.1/orderly/gen_fp/fingerprints.py
+drwxr-xr-x   0 dsw46      (502) staff       (20)        0 2023-08-01 16:00:38.762889 orderly-0.1.1/orderly/plot/
+-rw-r--r--   0 dsw46      (502) staff       (20)        0 2023-05-16 18:30:48.000000 orderly-0.1.1/orderly/plot/__init__.py
+-rw-r--r--   0 dsw46      (502) staff       (20)       63 2023-05-16 18:30:48.000000 orderly-0.1.1/orderly/plot/__main__.py
+-rw-r--r--   0 dsw46      (502) staff       (20)    18069 2023-07-03 14:56:10.000000 orderly-0.1.1/orderly/plot/plotter.py
+-rw-r--r--   0 dsw46      (502) staff       (20)     1934 2023-05-02 14:22:54.000000 orderly-0.1.1/orderly/types.py
+drwxr-xr-x   0 dsw46      (502) staff       (20)        0 2023-08-01 16:00:38.758515 orderly-0.1.1/orderly.egg-info/
+-rw-r--r--   0 dsw46      (502) staff       (20)     8988 2023-08-01 16:00:38.000000 orderly-0.1.1/orderly.egg-info/PKG-INFO
+-rw-r--r--   0 dsw46      (502) staff       (20)      817 2023-08-01 16:00:38.000000 orderly-0.1.1/orderly.egg-info/SOURCES.txt
+-rw-r--r--   0 dsw46      (502) staff       (20)        1 2023-08-01 16:00:38.000000 orderly-0.1.1/orderly.egg-info/dependency_links.txt
+-rw-r--r--   0 dsw46      (502) staff       (20)       14 2023-08-01 16:00:38.000000 orderly-0.1.1/orderly.egg-info/top_level.txt
+-rw-r--r--   0 dsw46      (502) staff       (20)     1140 2023-07-03 14:56:10.000000 orderly-0.1.1/pyproject.toml
+-rw-r--r--   0 dsw46      (502) staff       (20)       38 2023-08-01 16:00:38.764365 orderly-0.1.1/setup.cfg
+-rw-r--r--   0 dsw46      (502) staff       (20)      728 2023-08-01 15:59:09.000000 orderly-0.1.1/setup.py
+drwxr-xr-x   0 dsw46      (502) staff       (20)        0 2023-08-01 16:00:38.763450 orderly-0.1.1/tests/
+-rw-r--r--   0 dsw46      (502) staff       (20)        0 2023-04-07 16:58:29.000000 orderly-0.1.1/tests/__init__.py
+-rw-r--r--   0 dsw46      (502) staff       (20)    44246 2023-07-03 14:56:10.000000 orderly-0.1.1/tests/test_clean.py
+-rw-r--r--   0 dsw46      (502) staff       (20)     1548 2023-04-14 18:37:02.000000 orderly-0.1.1/tests/test_data.py
+-rw-r--r--   0 dsw46      (502) staff       (20)    60769 2023-07-03 14:56:10.000000 orderly-0.1.1/tests/test_extract.py
```

### Comparing `orderly-0.1.0/LICENSE` & `orderly-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `orderly-0.1.0/PKG-INFO` & `orderly-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orderly
-Version: 0.1.0
+Version: 0.1.1
 Summary: A wrapper for downloading ORD-schema data, extracting and cleaning the data
 Author: ['Daniel S. Wigh <dsw46@cam.ac.uk>', 'Joe Arrowsmith <joearrowsmith0@gmail.com>', 'Alexander Pomberger <ap2153@cam.ac.uk>', 'Kobi C. Felton <kcmf2@cam.ac.uk>', 'Alexei A. Lapkin <aal35@cam.ac.uk>']
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
 
@@ -24,17 +24,17 @@
 -----------------
 
 Machine learning has the potential to provide tremendous value to chemistry. However, large amounts of clean high-quality data are needed to train models
 
 ORDerly cleans chemical reaction data from the growing [Open Reaction Database (ORD)](https://docs.open-reaction-database.org/en/latest/).
 
 Use ORDerly to:
-- Extract and clean your own dataset from ORD
+- Extract and clean your own datasets.
 - Access the [ORDerly condition prediction benchmark dataset](https://figshare.com/articles/dataset/ORDerly_chemical_reactions_condition_benchmarks/23298467) for reaction condition prediction.
-- Reproduce results from our paper including training a ML model to predict reaction conditions
+- Reproduce results from our paper including training a ML model to predict reaction conditions.
 
 <img src="images/abstract_fig.png" alt="Abstract Figure" width="300">
 
 
 <!-- Section on extracting and cleaning a dataset-->
 
 📖 Extract and clean a dataset
@@ -44,15 +44,15 @@
 
 <!-- ```python -m orderly.download.ord```
 
 This will create a folder called ```/data/ord/``` in your current directory, and download the data into ```ord/``` -->
 
 Data in ORD format should be placed in a folder called ```/data/ord/```. You can either use your own data, or the open-source ORD data.
 
-To download the ORD data follow the instructions on the [official website](https://github.com/open-reaction-database/ord-data) (i.e. download GitLFS and clone their repository) and then place it within a folder called ```/data/ord/```.
+To download the ORD data follow the instructions in the [ORD repository](https://github.com/open-reaction-database/ord-data) (i.e. download [Git LFS](https://git-lfs.com/) and clone their repository) and then place it within a folder called ```/data/ord/```.
 
 ### Extract data from the ORD files
 
 ```python -m orderly.extract```
 
 If you want to run ORDerly on your own data, and want to specify the input and output path:
```

### Comparing `orderly-0.1.0/README.md` & `orderly-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 -----------------
 
 Machine learning has the potential to provide tremendous value to chemistry. However, large amounts of clean high-quality data are needed to train models
 
 ORDerly cleans chemical reaction data from the growing [Open Reaction Database (ORD)](https://docs.open-reaction-database.org/en/latest/).
 
 Use ORDerly to:
-- Extract and clean your own dataset from ORD
+- Extract and clean your own datasets.
 - Access the [ORDerly condition prediction benchmark dataset](https://figshare.com/articles/dataset/ORDerly_chemical_reactions_condition_benchmarks/23298467) for reaction condition prediction.
-- Reproduce results from our paper including training a ML model to predict reaction conditions
+- Reproduce results from our paper including training a ML model to predict reaction conditions.
 
 <img src="images/abstract_fig.png" alt="Abstract Figure" width="300">
 
 
 <!-- Section on extracting and cleaning a dataset-->
 
 📖 Extract and clean a dataset
@@ -34,15 +34,15 @@
 
 <!-- ```python -m orderly.download.ord```
 
 This will create a folder called ```/data/ord/``` in your current directory, and download the data into ```ord/``` -->
 
 Data in ORD format should be placed in a folder called ```/data/ord/```. You can either use your own data, or the open-source ORD data.
 
-To download the ORD data follow the instructions on the [official website](https://github.com/open-reaction-database/ord-data) (i.e. download GitLFS and clone their repository) and then place it within a folder called ```/data/ord/```.
+To download the ORD data follow the instructions in the [ORD repository](https://github.com/open-reaction-database/ord-data) (i.e. download [Git LFS](https://git-lfs.com/) and clone their repository) and then place it within a folder called ```/data/ord/```.
 
 ### Extract data from the ORD files
 
 ```python -m orderly.extract```
 
 If you want to run ORDerly on your own data, and want to specify the input and output path:
```

### Comparing `orderly-0.1.0/orderly/types.py` & `orderly-0.1.1/orderly/types.py`

 * *Files identical despite different names*

### Comparing `orderly-0.1.0/orderly.egg-info/PKG-INFO` & `orderly-0.1.1/orderly.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orderly
-Version: 0.1.0
+Version: 0.1.1
 Summary: A wrapper for downloading ORD-schema data, extracting and cleaning the data
 Author: ['Daniel S. Wigh <dsw46@cam.ac.uk>', 'Joe Arrowsmith <joearrowsmith0@gmail.com>', 'Alexander Pomberger <ap2153@cam.ac.uk>', 'Kobi C. Felton <kcmf2@cam.ac.uk>', 'Alexei A. Lapkin <aal35@cam.ac.uk>']
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
 
@@ -24,17 +24,17 @@
 -----------------
 
 Machine learning has the potential to provide tremendous value to chemistry. However, large amounts of clean high-quality data are needed to train models
 
 ORDerly cleans chemical reaction data from the growing [Open Reaction Database (ORD)](https://docs.open-reaction-database.org/en/latest/).
 
 Use ORDerly to:
-- Extract and clean your own dataset from ORD
+- Extract and clean your own datasets.
 - Access the [ORDerly condition prediction benchmark dataset](https://figshare.com/articles/dataset/ORDerly_chemical_reactions_condition_benchmarks/23298467) for reaction condition prediction.
-- Reproduce results from our paper including training a ML model to predict reaction conditions
+- Reproduce results from our paper including training a ML model to predict reaction conditions.
 
 <img src="images/abstract_fig.png" alt="Abstract Figure" width="300">
 
 
 <!-- Section on extracting and cleaning a dataset-->
 
 📖 Extract and clean a dataset
@@ -44,15 +44,15 @@
 
 <!-- ```python -m orderly.download.ord```
 
 This will create a folder called ```/data/ord/``` in your current directory, and download the data into ```ord/``` -->
 
 Data in ORD format should be placed in a folder called ```/data/ord/```. You can either use your own data, or the open-source ORD data.
 
-To download the ORD data follow the instructions on the [official website](https://github.com/open-reaction-database/ord-data) (i.e. download GitLFS and clone their repository) and then place it within a folder called ```/data/ord/```.
+To download the ORD data follow the instructions in the [ORD repository](https://github.com/open-reaction-database/ord-data) (i.e. download [Git LFS](https://git-lfs.com/) and clone their repository) and then place it within a folder called ```/data/ord/```.
 
 ### Extract data from the ORD files
 
 ```python -m orderly.extract```
 
 If you want to run ORDerly on your own data, and want to specify the input and output path:
```

### Comparing `orderly-0.1.0/pyproject.toml` & `orderly-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `orderly-0.1.0/tests/test_clean.py` & `orderly-0.1.1/tests/test_clean.py`

 * *Files identical despite different names*

### Comparing `orderly-0.1.0/tests/test_data.py` & `orderly-0.1.1/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `orderly-0.1.0/tests/test_extract.py` & `orderly-0.1.1/tests/test_extract.py`

 * *Files identical despite different names*

