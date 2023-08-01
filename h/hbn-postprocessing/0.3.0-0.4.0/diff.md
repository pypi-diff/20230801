# Comparing `tmp/hbn_postprocessing-0.3.0.tar.gz` & `tmp/hbn_postprocessing-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hbn_postprocessing-0.3.0.tar", max compression
+gzip compressed data, was "hbn_postprocessing-0.4.0.tar", max compression
```

## Comparing `hbn_postprocessing-0.3.0.tar` & `hbn_postprocessing-0.4.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       70 2023-05-11 19:33:07.365330 hbn_postprocessing-0.3.0/README.md
--rw-r--r--   0        0        0       38 2023-05-12 16:53:18.721105 hbn_postprocessing-0.3.0/hbn_postprocessing/__init__.py
--rw-r--r--   0        0        0     2697 2023-08-01 15:11:54.300990 hbn_postprocessing-0.3.0/hbn_postprocessing/file_count.py
--rw-r--r--   0        0        0     1158 2023-08-01 15:11:54.300990 hbn_postprocessing-0.3.0/hbn_postprocessing/html.py
--rw-r--r--   0        0        0     2058 2023-08-01 15:11:54.300990 hbn_postprocessing-0.3.0/hbn_postprocessing/jobs.py
--rw-r--r--   0        0        0     1914 2023-08-01 19:24:25.046071 hbn_postprocessing-0.3.0/hbn_postprocessing/main.py
--rw-r--r--   0        0        0     2199 2023-08-01 15:11:54.304990 hbn_postprocessing-0.3.0/hbn_postprocessing/motion.py
--rw-r--r--   0        0        0      833 2023-05-12 19:00:23.976893 hbn_postprocessing-0.3.0/hbn_postprocessing/utils.py
--rw-r--r--   0        0        0     1265 2023-08-01 19:24:31.550202 hbn_postprocessing-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      627 1970-01-01 00:00:00.000000 hbn_postprocessing-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0       70 2023-05-11 19:33:07.365330 hbn_postprocessing-0.4.0/README.md
+-rw-r--r--   0        0        0       38 2023-05-12 16:53:18.721105 hbn_postprocessing-0.4.0/hbn_postprocessing/__init__.py
+-rw-r--r--   0        0        0     2697 2023-08-01 15:11:54.300990 hbn_postprocessing-0.4.0/hbn_postprocessing/file_count.py
+-rw-r--r--   0        0        0     1116 2023-08-01 19:26:48.772972 hbn_postprocessing-0.4.0/hbn_postprocessing/html.py
+-rw-r--r--   0        0        0     2058 2023-08-01 15:11:54.300990 hbn_postprocessing-0.4.0/hbn_postprocessing/jobs.py
+-rw-r--r--   0        0        0     1914 2023-08-01 19:24:25.046071 hbn_postprocessing-0.4.0/hbn_postprocessing/main.py
+-rw-r--r--   0        0        0     2199 2023-08-01 15:11:54.304990 hbn_postprocessing-0.4.0/hbn_postprocessing/motion.py
+-rw-r--r--   0        0        0      833 2023-05-12 19:00:23.976893 hbn_postprocessing-0.4.0/hbn_postprocessing/utils.py
+-rw-r--r--   0        0        0     1265 2023-08-01 19:27:01.553231 hbn_postprocessing-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      627 1970-01-01 00:00:00.000000 hbn_postprocessing-0.4.0/PKG-INFO
```

### Comparing `hbn_postprocessing-0.3.0/hbn_postprocessing/file_count.py` & `hbn_postprocessing-0.4.0/hbn_postprocessing/file_count.py`

 * *Files identical despite different names*

### Comparing `hbn_postprocessing-0.3.0/hbn_postprocessing/html.py` & `hbn_postprocessing-0.4.0/hbn_postprocessing/html.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,15 +25,13 @@
         .replace([True, False], ["yes", "no"]),
     ).set_index("participant_id")
     out_path = Path(out_dir)
     matches.to_csv(out_path / "html-check_all.csv", sep=",")
     matches[matches["html"] == "no"].to_csv(
         out_path / "html-check_no.csv",
         sep=",",
-        index=False,
     )
     matches[matches["html"] == "yes"].to_csv(
         out_path / "html-check_yes.csv",
         sep=",",
-        index=False,
     )
     return matches
```

### Comparing `hbn_postprocessing-0.3.0/hbn_postprocessing/jobs.py` & `hbn_postprocessing-0.4.0/hbn_postprocessing/jobs.py`

 * *Files identical despite different names*

### Comparing `hbn_postprocessing-0.3.0/hbn_postprocessing/main.py` & `hbn_postprocessing-0.4.0/hbn_postprocessing/main.py`

 * *Files identical despite different names*

### Comparing `hbn_postprocessing-0.3.0/hbn_postprocessing/motion.py` & `hbn_postprocessing-0.4.0/hbn_postprocessing/motion.py`

 * *Files identical despite different names*

### Comparing `hbn_postprocessing-0.3.0/hbn_postprocessing/utils.py` & `hbn_postprocessing-0.4.0/hbn_postprocessing/utils.py`

 * *Files identical despite different names*

### Comparing `hbn_postprocessing-0.3.0/pyproject.toml` & `hbn_postprocessing-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hbn-postprocessing"
-version = "0.3.0"
+version = "0.4.0"
 description = "Postprocessing workflow for HBN data"
 authors = ["Tristan Kuehn <tkuehn@uwo.ca>", "Jessica Lammert <jlammert@uwo.ca>"]
 readme = "README.md"
 packages = [{include = "hbn_postprocessing"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
```

### Comparing `hbn_postprocessing-0.3.0/PKG-INFO` & `hbn_postprocessing-0.4.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hbn-postprocessing
-Version: 0.3.0
+Version: 0.4.0
 Summary: Postprocessing workflow for HBN data
 Author: Tristan Kuehn
 Author-email: tkuehn@uwo.ca
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

