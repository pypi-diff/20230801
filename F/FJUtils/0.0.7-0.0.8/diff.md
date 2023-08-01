# Comparing `tmp/FJUtils-0.0.7.tar.gz` & `tmp/FJUtils-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FJUtils-0.0.7.tar", last modified: Mon Jul 31 09:46:42 2023, max compression
+gzip compressed data, was "FJUtils-0.0.8.tar", last modified: Tue Aug  1 09:19:41 2023, max compression
```

## Comparing `FJUtils-0.0.7.tar` & `FJUtils-0.0.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-31 09:46:42.471868 FJUtils-0.0.7/
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-31 09:46:42.471868 FJUtils-0.0.7/FJUtils.egg-info/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     3670 2023-07-31 09:46:42.000000 FJUtils-0.0.7/FJUtils.egg-info/PKG-INFO
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      362 2023-07-31 09:46:42.000000 FJUtils-0.0.7/FJUtils.egg-info/SOURCES.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)        1 2023-07-31 09:46:42.000000 FJUtils-0.0.7/FJUtils.egg-info/dependency_links.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      116 2023-07-31 09:46:42.000000 FJUtils-0.0.7/FJUtils.egg-info/requires.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)        8 2023-07-31 09:46:42.000000 FJUtils-0.0.7/FJUtils.egg-info/top_level.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    11357 2023-06-06 11:02:09.000000 FJUtils-0.0.7/LICENSE
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     3670 2023-07-31 09:46:42.471868 FJUtils-0.0.7/PKG-INFO
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     2911 2023-06-06 11:02:09.000000 FJUtils-0.0.7/README.md
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-31 09:46:42.471868 FJUtils-0.0.7/fjutils/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      885 2023-07-31 09:42:46.000000 FJUtils-0.0.7/fjutils/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     8332 2023-06-17 08:26:17.000000 FJUtils-0.0.7/fjutils/checkpointing.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     9956 2023-07-22 12:20:22.000000 FJUtils-0.0.7/fjutils/easylm.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    25511 2023-07-31 09:40:02.000000 FJUtils-0.0.7/fjutils/flash_attention.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1800 2023-06-06 11:02:09.000000 FJUtils-0.0.7/fjutils/load.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1931 2023-07-26 09:37:29.000000 FJUtils-0.0.7/fjutils/loss_funcs.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     9724 2023-06-24 10:11:24.000000 FJUtils-0.0.7/fjutils/optimizers.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     7278 2023-07-22 12:19:47.000000 FJUtils-0.0.7/fjutils/utils.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      533 2023-06-06 11:02:09.000000 FJUtils-0.0.7/pyproject.toml
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       38 2023-07-31 09:46:42.471868 FJUtils-0.0.7/setup.cfg
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1209 2023-07-31 09:41:53.000000 FJUtils-0.0.7/setup.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-08-01 09:19:41.482348 FJUtils-0.0.8/
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-08-01 09:19:41.478348 FJUtils-0.0.8/FJUtils.egg-info/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     3670 2023-08-01 09:19:41.000000 FJUtils-0.0.8/FJUtils.egg-info/PKG-INFO
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      362 2023-08-01 09:19:41.000000 FJUtils-0.0.8/FJUtils.egg-info/SOURCES.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)        1 2023-08-01 09:19:41.000000 FJUtils-0.0.8/FJUtils.egg-info/dependency_links.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      116 2023-08-01 09:19:41.000000 FJUtils-0.0.8/FJUtils.egg-info/requires.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)        8 2023-08-01 09:19:41.000000 FJUtils-0.0.8/FJUtils.egg-info/top_level.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    11357 2023-06-06 11:02:09.000000 FJUtils-0.0.8/LICENSE
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     3670 2023-08-01 09:19:41.482348 FJUtils-0.0.8/PKG-INFO
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     2911 2023-06-06 11:02:09.000000 FJUtils-0.0.8/README.md
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-08-01 09:19:41.482348 FJUtils-0.0.8/fjutils/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      885 2023-07-31 09:42:46.000000 FJUtils-0.0.8/fjutils/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     8332 2023-06-17 08:26:17.000000 FJUtils-0.0.8/fjutils/checkpointing.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     9956 2023-07-22 12:20:22.000000 FJUtils-0.0.8/fjutils/easylm.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    25511 2023-07-31 09:40:02.000000 FJUtils-0.0.8/fjutils/flash_attention.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1800 2023-06-06 11:02:09.000000 FJUtils-0.0.8/fjutils/load.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1931 2023-07-26 09:37:29.000000 FJUtils-0.0.8/fjutils/loss_funcs.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    15184 2023-08-01 09:19:08.000000 FJUtils-0.0.8/fjutils/optimizers.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     7278 2023-07-22 12:19:47.000000 FJUtils-0.0.8/fjutils/utils.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      533 2023-06-06 11:02:09.000000 FJUtils-0.0.8/pyproject.toml
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       38 2023-08-01 09:19:41.482348 FJUtils-0.0.8/setup.cfg
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1209 2023-08-01 09:19:08.000000 FJUtils-0.0.8/setup.py
```

### Comparing `FJUtils-0.0.7/FJUtils.egg-info/PKG-INFO` & `FJUtils-0.0.8/FJUtils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FJUtils
-Version: 0.0.7
+Version: 0.0.8
 Summary: UNKNOWN
 Home-page: https://github.com/erfanzar/
 Author: Erfan Zare Chavoshi
 Author-email: erfanzare82@yahoo.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `FJUtils-0.0.7/LICENSE` & `FJUtils-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `FJUtils-0.0.7/PKG-INFO` & `FJUtils-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FJUtils
-Version: 0.0.7
+Version: 0.0.8
 Summary: UNKNOWN
 Home-page: https://github.com/erfanzar/
 Author: Erfan Zare Chavoshi
 Author-email: erfanzare82@yahoo.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `FJUtils-0.0.7/README.md` & `FJUtils-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `FJUtils-0.0.7/fjutils/__init__.py` & `FJUtils-0.0.8/fjutils/__init__.py`

 * *Files identical despite different names*

### Comparing `FJUtils-0.0.7/fjutils/checkpointing.py` & `FJUtils-0.0.8/fjutils/checkpointing.py`

 * *Files identical despite different names*

### Comparing `FJUtils-0.0.7/fjutils/easylm.py` & `FJUtils-0.0.8/fjutils/easylm.py`

 * *Files identical despite different names*

### Comparing `FJUtils-0.0.7/fjutils/flash_attention.py` & `FJUtils-0.0.8/fjutils/flash_attention.py`

 * *Files identical despite different names*

### Comparing `FJUtils-0.0.7/fjutils/load.py` & `FJUtils-0.0.8/fjutils/load.py`

 * *Files identical despite different names*

### Comparing `FJUtils-0.0.7/fjutils/loss_funcs.py` & `FJUtils-0.0.8/fjutils/loss_funcs.py`

 * *Files identical despite different names*

### Comparing `FJUtils-0.0.7/fjutils/utils.py` & `FJUtils-0.0.8/fjutils/utils.py`

 * *Files identical despite different names*

### Comparing `FJUtils-0.0.7/pyproject.toml` & `FJUtils-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `FJUtils-0.0.7/setup.py` & `FJUtils-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="FJUtils",
-    version='0.0.7',
+    version='0.0.8',
     author="Erfan Zare Chavoshi",
     author_email="erfanzare82@yahoo.com",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/erfanzar/",
     packages=setuptools.find_packages(),
     install_requires=[
```

