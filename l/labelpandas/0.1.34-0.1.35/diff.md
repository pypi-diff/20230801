# Comparing `tmp/labelpandas-0.1.34.tar.gz` & `tmp/labelpandas-0.1.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labelpandas-0.1.34.tar", last modified: Mon Apr  3 18:19:23 2023, max compression
+gzip compressed data, was "labelpandas-0.1.35.tar", last modified: Tue Aug  1 14:32:18 2023, max compression
```

## Comparing `labelpandas-0.1.34.tar` & `labelpandas-0.1.35.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 18:19:23.084304 labelpandas-0.1.34/
--rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-04-03 18:19:23.084304 labelpandas-0.1.34/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-04-03 18:19:11.000000 labelpandas-0.1.34/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 18:19:23.084304 labelpandas-0.1.34/labelpandas/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-03 18:19:11.000000 labelpandas-0.1.34/labelpandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12262 2023-04-03 18:19:11.000000 labelpandas-0.1.34/labelpandas/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-04-03 18:19:11.000000 labelpandas-0.1.34/labelpandas/connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-03 18:19:11.000000 labelpandas-0.1.34/labelpandas/load_local_files.py
--rw-r--r--   0 runner    (1001) docker     (123)    11069 2023-04-03 18:19:11.000000 labelpandas-0.1.34/labelpandas/uploader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 18:19:23.084304 labelpandas-0.1.34/labelpandas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-04-03 18:19:23.000000 labelpandas-0.1.34/labelpandas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-03 18:19:23.000000 labelpandas-0.1.34/labelpandas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 18:19:23.000000 labelpandas-0.1.34/labelpandas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-03 18:19:23.000000 labelpandas-0.1.34/labelpandas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-03 18:19:23.000000 labelpandas-0.1.34/labelpandas.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 18:19:23.084304 labelpandas-0.1.34/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-03 18:19:11.000000 labelpandas-0.1.34/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:32:18.712515 labelpandas-0.1.35/
+-rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-08-01 14:32:18.712515 labelpandas-0.1.35/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-08-01 14:31:46.000000 labelpandas-0.1.35/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:32:18.712515 labelpandas-0.1.35/labelpandas/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-08-01 14:31:49.000000 labelpandas-0.1.35/labelpandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24237 2023-08-01 14:31:49.000000 labelpandas-0.1.35/labelpandas/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-08-01 14:31:49.000000 labelpandas-0.1.35/labelpandas/connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-08-01 14:31:49.000000 labelpandas-0.1.35/labelpandas/load_local_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17044 2023-08-01 14:31:49.000000 labelpandas-0.1.35/labelpandas/uploader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:32:18.712515 labelpandas-0.1.35/labelpandas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-08-01 14:32:18.000000 labelpandas-0.1.35/labelpandas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-08-01 14:32:18.000000 labelpandas-0.1.35/labelpandas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 14:32:18.000000 labelpandas-0.1.35/labelpandas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-01 14:32:18.000000 labelpandas-0.1.35/labelpandas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-01 14:32:18.000000 labelpandas-0.1.35/labelpandas.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 14:32:18.712515 labelpandas-0.1.35/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-08-01 14:31:49.000000 labelpandas-0.1.35/setup.py
```

### Comparing `labelpandas-0.1.34/PKG-INFO` & `labelpandas-0.1.35/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labelpandas
-Version: 0.1.34
+Version: 0.1.35
 Summary: Labelbox Connector for Pandas
 Home-page: https://github.com/Labelbox/labelpandas
 Author: Labelbox
 Author-email: raphael@labelbox.com
 Description-Content-Type: text/markdown
 
 # The Official Open-Source Labelbox <> Pandas Python Integration
```

### Comparing `labelpandas-0.1.34/README.md` & `labelpandas-0.1.35/README.md`

 * *Files identical despite different names*

### Comparing `labelpandas-0.1.34/labelpandas/connector.py` & `labelpandas-0.1.35/labelpandas/connector.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 - get_unique_values(table, col)                           : Gets all unique values in a given column
 - add_col(table, col, default)                            : Creates a column where all values equal the default value
 - get_table_length(table)                                 : Gets the length of a DataFrame
 - rename_col(table, col, to)                              : Renames a given column
 
 """
 import pandas   
-from labelbase.connector import validate_column_name_change
   
 def get_col_names(table:pandas.core.frame.DataFrame, extra_client=None):
     """Grabs all column names from a Pandas DataFrame
     Args:
         table           :   Required (pandas.core.frame.DataFrame) - Pandas DataFrame
         extra_client    :   Ignore this value - necessary for other labelbase integrations
     Returns:
@@ -51,21 +50,7 @@
     Args:
         table           :   Required (pandas.core.frame.DataFrame) - Pandas DataFrame
         extra_client    :   Ignore this value - necessary for other labelbase integrations        
     Returns:
         The length of your table as an integer
     """  
     return len(table)
-
-def rename_col(table: pandas.core.frame.DataFrame, col:str, to:str):
-    """ Renames columns into the Labelpandas format    
-    Args:
-        table           :   Required (pandas.core.frame.DataFrame) - Pandas DataFrame
-        col             :   Required (str) - Existing column name to-be-changed
-        to              :   Required (str) - What to rename the column as       
-    Returns:
-        Updated `table` object with renamed column
-    """
-    existing_cols = get_col_names(table, extra_client=False)
-    validate_column_name_change(old_col_name=col, new_col_name=to, existing_col_names=existing_cols)
-    table = table.rename(columns={col:to})
-    return table
```

### Comparing `labelpandas-0.1.34/labelpandas/load_local_files.py` & `labelpandas-0.1.35/labelpandas/load_local_files.py`

 * *Files identical despite different names*

### Comparing `labelpandas-0.1.34/labelpandas.egg-info/PKG-INFO` & `labelpandas-0.1.35/labelpandas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labelpandas
-Version: 0.1.34
+Version: 0.1.35
 Summary: Labelbox Connector for Pandas
 Home-page: https://github.com/Labelbox/labelpandas
 Author: Labelbox
 Author-email: raphael@labelbox.com
 Description-Content-Type: text/markdown
 
 # The Official Open-Source Labelbox <> Pandas Python Integration
```

### Comparing `labelpandas-0.1.34/setup.py` & `labelpandas-0.1.35/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='labelpandas',
-    version='0.1.34',
+    version='0.1.35',
     author='Labelbox',
     author_email="raphael@labelbox.com",
     description='Labelbox Connector for Pandas',
     long_description=long_description,
     long_description_content_type="text/markdown",    
     url='https://github.com/Labelbox/labelpandas',    
     packages=find_packages(),
```

