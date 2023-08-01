# Comparing `tmp/labelpandas-0.1.35.tar.gz` & `tmp/labelpandas-0.1.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labelpandas-0.1.35.tar", last modified: Tue Aug  1 14:32:18 2023, max compression
+gzip compressed data, was "labelpandas-0.1.36.tar", last modified: Tue Aug  1 14:34:05 2023, max compression
```

## Comparing `labelpandas-0.1.35.tar` & `labelpandas-0.1.36.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:32:18.712515 labelpandas-0.1.35/
--rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-08-01 14:32:18.712515 labelpandas-0.1.35/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-08-01 14:31:46.000000 labelpandas-0.1.35/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:32:18.712515 labelpandas-0.1.35/labelpandas/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-08-01 14:31:49.000000 labelpandas-0.1.35/labelpandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24237 2023-08-01 14:31:49.000000 labelpandas-0.1.35/labelpandas/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-08-01 14:31:49.000000 labelpandas-0.1.35/labelpandas/connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-08-01 14:31:49.000000 labelpandas-0.1.35/labelpandas/load_local_files.py
--rw-r--r--   0 runner    (1001) docker     (123)    17044 2023-08-01 14:31:49.000000 labelpandas-0.1.35/labelpandas/uploader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:32:18.712515 labelpandas-0.1.35/labelpandas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-08-01 14:32:18.000000 labelpandas-0.1.35/labelpandas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-08-01 14:32:18.000000 labelpandas-0.1.35/labelpandas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 14:32:18.000000 labelpandas-0.1.35/labelpandas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-01 14:32:18.000000 labelpandas-0.1.35/labelpandas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-01 14:32:18.000000 labelpandas-0.1.35/labelpandas.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 14:32:18.712515 labelpandas-0.1.35/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-08-01 14:31:49.000000 labelpandas-0.1.35/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:34:05.050164 labelpandas-0.1.36/
+-rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-08-01 14:34:05.050164 labelpandas-0.1.36/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-08-01 14:33:51.000000 labelpandas-0.1.36/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:34:05.050164 labelpandas-0.1.36/labelpandas/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-08-01 14:33:53.000000 labelpandas-0.1.36/labelpandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24237 2023-08-01 14:33:53.000000 labelpandas-0.1.36/labelpandas/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-08-01 14:33:53.000000 labelpandas-0.1.36/labelpandas/connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-08-01 14:33:53.000000 labelpandas-0.1.36/labelpandas/load_local_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17044 2023-08-01 14:33:53.000000 labelpandas-0.1.36/labelpandas/uploader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:34:05.050164 labelpandas-0.1.36/labelpandas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-08-01 14:34:05.000000 labelpandas-0.1.36/labelpandas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-08-01 14:34:05.000000 labelpandas-0.1.36/labelpandas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 14:34:05.000000 labelpandas-0.1.36/labelpandas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-01 14:34:05.000000 labelpandas-0.1.36/labelpandas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-01 14:34:05.000000 labelpandas-0.1.36/labelpandas.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 14:34:05.050164 labelpandas-0.1.36/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-08-01 14:33:53.000000 labelpandas-0.1.36/setup.py
```

### Comparing `labelpandas-0.1.35/PKG-INFO` & `labelpandas-0.1.36/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labelpandas
-Version: 0.1.35
+Version: 0.1.36
 Summary: Labelbox Connector for Pandas
 Home-page: https://github.com/Labelbox/labelpandas
 Author: Labelbox
 Author-email: raphael@labelbox.com
 Description-Content-Type: text/markdown
 
 # The Official Open-Source Labelbox <> Pandas Python Integration
```

### Comparing `labelpandas-0.1.35/README.md` & `labelpandas-0.1.36/README.md`

 * *Files identical despite different names*

### Comparing `labelpandas-0.1.35/labelpandas/client.py` & `labelpandas-0.1.36/labelpandas/client.py`

 * *Files identical despite different names*

### Comparing `labelpandas-0.1.35/labelpandas/connector.py` & `labelpandas-0.1.36/labelpandas/connector.py`

 * *Files identical despite different names*

### Comparing `labelpandas-0.1.35/labelpandas/load_local_files.py` & `labelpandas-0.1.36/labelpandas/load_local_files.py`

 * *Files identical despite different names*

### Comparing `labelpandas-0.1.35/labelpandas/uploader.py` & `labelpandas-0.1.36/labelpandas/uploader.py`

 * *Files identical despite different names*

### Comparing `labelpandas-0.1.35/labelpandas.egg-info/PKG-INFO` & `labelpandas-0.1.36/labelpandas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labelpandas
-Version: 0.1.35
+Version: 0.1.36
 Summary: Labelbox Connector for Pandas
 Home-page: https://github.com/Labelbox/labelpandas
 Author: Labelbox
 Author-email: raphael@labelbox.com
 Description-Content-Type: text/markdown
 
 # The Official Open-Source Labelbox <> Pandas Python Integration
```

### Comparing `labelpandas-0.1.35/setup.py` & `labelpandas-0.1.36/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='labelpandas',
-    version='0.1.35',
+    version='0.1.36',
     author='Labelbox',
     author_email="raphael@labelbox.com",
     description='Labelbox Connector for Pandas',
     long_description=long_description,
     long_description_content_type="text/markdown",    
     url='https://github.com/Labelbox/labelpandas',    
     packages=find_packages(),
```

