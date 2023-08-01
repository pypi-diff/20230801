# Comparing `tmp/Dager-0.1.tar.gz` & `tmp/Dager-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Dager-0.1.tar", last modified: Fri Jul 21 11:56:00 2023, max compression
+gzip compressed data, was "Dager-0.2.tar", last modified: Tue Aug  1 07:45:37 2023, max compression
```

## Comparing `Dager-0.1.tar` & `Dager-0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 11:56:00.642374 Dager-0.1/
-drwxrwxrwx   0        0        0        0 2023-07-21 11:56:00.606373 Dager-0.1/Dager/
--rw-rw-rw-   0        0        0       32 2023-07-21 11:50:21.000000 Dager-0.1/Dager/__init__.py
--rw-rw-rw-   0        0        0     1897 2023-07-21 11:50:03.000000 Dager-0.1/Dager/dager_data.py
-drwxrwxrwx   0        0        0        0 2023-07-21 11:56:00.638372 Dager-0.1/Dager.egg-info/
--rw-rw-rw-   0        0        0      536 2023-07-21 11:56:00.000000 Dager-0.1/Dager.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      208 2023-07-21 11:56:00.000000 Dager-0.1/Dager.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 11:56:00.000000 Dager-0.1/Dager.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      230 2023-07-21 11:56:00.000000 Dager-0.1/Dager.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-21 11:56:00.000000 Dager-0.1/Dager.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1065 2023-07-21 10:54:19.000000 Dager-0.1/LICENSE
--rw-rw-rw-   0        0        0      536 2023-07-21 11:56:00.641372 Dager-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       60 2023-07-21 11:48:01.000000 Dager-0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-21 11:56:00.643371 Dager-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1079 2023-07-21 11:52:38.000000 Dager-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 07:45:37.658624 Dager-0.2/
+drwxrwxrwx   0        0        0        0 2023-08-01 07:45:37.627624 Dager-0.2/Dager/
+-rw-rw-rw-   0        0        0       32 2023-07-21 11:50:21.000000 Dager-0.2/Dager/__init__.py
+-rw-rw-rw-   0        0        0     1908 2023-07-26 14:57:29.000000 Dager-0.2/Dager/dager_data.py
+drwxrwxrwx   0        0        0        0 2023-08-01 07:45:37.651625 Dager-0.2/Dager.egg-info/
+-rw-rw-rw-   0        0        0      536 2023-08-01 07:45:37.000000 Dager-0.2/Dager.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      208 2023-08-01 07:45:37.000000 Dager-0.2/Dager.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 07:45:37.000000 Dager-0.2/Dager.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      230 2023-08-01 07:45:37.000000 Dager-0.2/Dager.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-08-01 07:45:37.000000 Dager-0.2/Dager.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1065 2023-07-21 10:54:19.000000 Dager-0.2/LICENSE
+-rw-rw-rw-   0        0        0      536 2023-08-01 07:45:37.657623 Dager-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       60 2023-07-21 11:48:01.000000 Dager-0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-01 07:45:37.659626 Dager-0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1079 2023-08-01 07:45:26.000000 Dager-0.2/setup.py
```

### Comparing `Dager-0.1/Dager/dager_data.py` & `Dager-0.2/Dager/dager_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 Dager_client = "mongodb://DaggerData_rw:eEsQcKvMgKfH5Di@p1ir1mon019.ger.corp.intel.com:7174,p2ir1mon019.ger.corp.intel.com:7174,p3ir1mon019.ger.corp.intel.com:7174/DaggerData?ssl=true&replicaSet=mongo7174"
 Dager_conn = 'DaggerData'
 
 ConnectionStringDager = pymongo.MongoClient(Dager_client)
 DatabaseDager = ConnectionStringDager[Dager_conn]
 
 class Database:
-    def pull_data(self, lot, indicator, operation, output_format='json', file_path=None):
+    def pull_data(self, lot, indicator, operation, wfr, output_format='json', file_path=None):
         """ Pull Data e.g.lot_indicator_operation 422200000_132324_Binning"""
 
-        name = f"{lot}_{operation}_{indicator}"
+        name = f"{lot}_{operation}_{wfr}_{indicator}"
         db = DatabaseDager
         fs = gridfs.GridFS(db)
 
         # download
         data = db.fs.files.find_one({'filename':name})
         if data:
             pulled_data = fs.get(data['_id']).read().decode()
```

### Comparing `Dager-0.1/Dager.egg-info/PKG-INFO` & `Dager-0.2/Dager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Dager
-Version: 0.1
+Version: 0.2
 Summary: Data Acquisition and Generation Engine for Reporting
 Home-page: https://github.com/iddy-ani/Dager_data
 Author: Idriss Animashaun
 Author-email: idriss.animashaun@intel.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Dager-0.1/LICENSE` & `Dager-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Dager-0.1/PKG-INFO` & `Dager-0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Dager
-Version: 0.1
+Version: 0.2
 Summary: Data Acquisition and Generation Engine for Reporting
 Home-page: https://github.com/iddy-ani/Dager_data
 Author: Idriss Animashaun
 Author-email: idriss.animashaun@intel.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Dager-0.1/setup.py` & `Dager-0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="Dager",
-    version="0.1",
+    version="0.2",
     packages=find_packages(),
     author="Idriss Animashaun",
     author_email="idriss.animashaun@intel.com",
     description="Data Acquisition and Generation Engine for Reporting",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/iddy-ani/Dager_data",
```

