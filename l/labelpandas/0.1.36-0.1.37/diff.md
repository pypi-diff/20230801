# Comparing `tmp/labelpandas-0.1.36.tar.gz` & `tmp/labelpandas-0.1.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labelpandas-0.1.36.tar", last modified: Tue Aug  1 14:34:05 2023, max compression
+gzip compressed data, was "labelpandas-0.1.37.tar", last modified: Tue Aug  1 21:27:20 2023, max compression
```

## Comparing `labelpandas-0.1.36.tar` & `labelpandas-0.1.37.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:34:05.050164 labelpandas-0.1.36/
--rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-08-01 14:34:05.050164 labelpandas-0.1.36/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-08-01 14:33:51.000000 labelpandas-0.1.36/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:34:05.050164 labelpandas-0.1.36/labelpandas/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-08-01 14:33:53.000000 labelpandas-0.1.36/labelpandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24237 2023-08-01 14:33:53.000000 labelpandas-0.1.36/labelpandas/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-08-01 14:33:53.000000 labelpandas-0.1.36/labelpandas/connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-08-01 14:33:53.000000 labelpandas-0.1.36/labelpandas/load_local_files.py
--rw-r--r--   0 runner    (1001) docker     (123)    17044 2023-08-01 14:33:53.000000 labelpandas-0.1.36/labelpandas/uploader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:34:05.050164 labelpandas-0.1.36/labelpandas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-08-01 14:34:05.000000 labelpandas-0.1.36/labelpandas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-08-01 14:34:05.000000 labelpandas-0.1.36/labelpandas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 14:34:05.000000 labelpandas-0.1.36/labelpandas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-01 14:34:05.000000 labelpandas-0.1.36/labelpandas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-01 14:34:05.000000 labelpandas-0.1.36/labelpandas.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 14:34:05.050164 labelpandas-0.1.36/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-08-01 14:33:53.000000 labelpandas-0.1.36/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:27:20.431673 labelpandas-0.1.37/
+-rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-08-01 21:27:20.431673 labelpandas-0.1.37/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-08-01 21:27:06.000000 labelpandas-0.1.37/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:27:20.431673 labelpandas-0.1.37/labelpandas/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-08-01 21:27:09.000000 labelpandas-0.1.37/labelpandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24267 2023-08-01 21:27:09.000000 labelpandas-0.1.37/labelpandas/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-08-01 21:27:09.000000 labelpandas-0.1.37/labelpandas/connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-08-01 21:27:09.000000 labelpandas-0.1.37/labelpandas/load_local_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17044 2023-08-01 21:27:09.000000 labelpandas-0.1.37/labelpandas/uploader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:27:20.431673 labelpandas-0.1.37/labelpandas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-08-01 21:27:20.000000 labelpandas-0.1.37/labelpandas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-08-01 21:27:20.000000 labelpandas-0.1.37/labelpandas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 21:27:20.000000 labelpandas-0.1.37/labelpandas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-01 21:27:20.000000 labelpandas-0.1.37/labelpandas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-01 21:27:20.000000 labelpandas-0.1.37/labelpandas.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 21:27:20.431673 labelpandas-0.1.37/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-08-01 21:27:09.000000 labelpandas-0.1.37/setup.py
```

### Comparing `labelpandas-0.1.36/PKG-INFO` & `labelpandas-0.1.37/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labelpandas
-Version: 0.1.36
+Version: 0.1.37
 Summary: Labelbox Connector for Pandas
 Home-page: https://github.com/Labelbox/labelpandas
 Author: Labelbox
 Author-email: raphael@labelbox.com
 Description-Content-Type: text/markdown
 
 # The Official Open-Source Labelbox <> Pandas Python Integration
```

### Comparing `labelpandas-0.1.36/README.md` & `labelpandas-0.1.37/README.md`

 * *Files identical despite different names*

### Comparing `labelpandas-0.1.36/labelpandas/client.py` & `labelpandas-0.1.37/labelpandas/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,15 +138,15 @@
             client=self.lb_client, table=table, table_dict=table_dict, 
             row_data_col=x["row_data_col"], global_key_col=x["global_key_col"], external_id_col=x["external_id_col"], 
             dataset_id_col=x["dataset_id_col"], dataset_id=dataset_id, 
             project_id_col=x["project_id_col"], project_id=project_id,
             model_id_col=x["model_id_col"], model_id=model_id, 
             model_run_id_col=x["model_run_id_col"], model_run_id=model_run_id,
             metadata_index=x["metadata_index"], attachment_index=x["attachment_index"], 
-            annotation_index=x["annotation_index"], prediction_index=x["prediction_index"], 
+            annotation_index=x["annotation_index"], prediction_index=x["prediction_index"], batch_action=actions['batch'],
             create_action=actions["create"], annotate_action=actions["annotate"], prediction_action=actions["predictions"],
             upload_method=upload_method, mask_method=mask_method, divider=divider, verbose=verbose
         )
                 
         # Upload your data rows to Labelbox, updating upload_dict if global keys are modified during upload using labelbase.uploader.batch_create_data_rows
         data_row_upload_results, upload_dict = batch_create_data_rows(
             client=self.lb_client, upload_dict=upload_dict,
```

### Comparing `labelpandas-0.1.36/labelpandas/connector.py` & `labelpandas-0.1.37/labelpandas/connector.py`

 * *Files identical despite different names*

### Comparing `labelpandas-0.1.36/labelpandas/load_local_files.py` & `labelpandas-0.1.37/labelpandas/load_local_files.py`

 * *Files identical despite different names*

### Comparing `labelpandas-0.1.36/labelpandas/uploader.py` & `labelpandas-0.1.37/labelpandas/uploader.py`

 * *Files identical despite different names*

### Comparing `labelpandas-0.1.36/labelpandas.egg-info/PKG-INFO` & `labelpandas-0.1.37/labelpandas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labelpandas
-Version: 0.1.36
+Version: 0.1.37
 Summary: Labelbox Connector for Pandas
 Home-page: https://github.com/Labelbox/labelpandas
 Author: Labelbox
 Author-email: raphael@labelbox.com
 Description-Content-Type: text/markdown
 
 # The Official Open-Source Labelbox <> Pandas Python Integration
```

### Comparing `labelpandas-0.1.36/setup.py` & `labelpandas-0.1.37/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='labelpandas',
-    version='0.1.36',
+    version='0.1.37',
     author='Labelbox',
     author_email="raphael@labelbox.com",
     description='Labelbox Connector for Pandas',
     long_description=long_description,
     long_description_content_type="text/markdown",    
     url='https://github.com/Labelbox/labelpandas',    
     packages=find_packages(),
```

