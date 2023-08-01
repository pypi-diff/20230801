# Comparing `tmp/shaku-database-1.1.7.tar.gz` & `tmp/shaku-database-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shaku-database-1.1.7.tar", last modified: Mon Jul 31 07:34:55 2023, max compression
+gzip compressed data, was "shaku-database-1.1.8.tar", last modified: Tue Aug  1 01:27:23 2023, max compression
```

## Comparing `shaku-database-1.1.7.tar` & `shaku-database-1.1.8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-31 07:34:55.170714 shaku-database-1.1.7/
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1069 2023-06-15 08:18:42.000000 shaku-database-1.1.7/LICENSE
--rw-r--r--   0 tongyuhao   (501) staff       (20)     7323 2023-07-31 07:34:55.170231 shaku-database-1.1.7/PKG-INFO
--rw-r--r--   0 tongyuhao   (501) staff       (20)     6192 2023-06-15 08:05:19.000000 shaku-database-1.1.7/README.md
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-31 07:34:55.164468 shaku-database-1.1.7/database/
--rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.1.7/database/__init__.py
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-31 07:34:55.165020 shaku-database-1.1.7/database/bigquery/
--rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.1.7/database/bigquery/__init__.py
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1452 2023-07-07 09:40:34.000000 shaku-database-1.1.7/database/bigquery/bq_sql_parser.py
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1683 2023-06-20 03:32:33.000000 shaku-database-1.1.7/database/bigquery/util.py
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-31 07:34:55.165408 shaku-database-1.1.7/database/cloud_sql/
--rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.1.7/database/cloud_sql/__init__.py
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1139 2023-06-16 06:51:48.000000 shaku-database-1.1.7/database/cloud_sql/crud.py
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-31 07:34:55.165770 shaku-database-1.1.7/database/cloud_storage/
--rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-07-11 09:09:30.000000 shaku-database-1.1.7/database/cloud_storage/__init__.py
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1580 2023-07-11 09:00:21.000000 shaku-database-1.1.7/database/cloud_storage/util.py
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-31 07:34:55.166033 shaku-database-1.1.7/gdrive_gcs_toolkit/
--rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-07-07 09:40:26.000000 shaku-database-1.1.7/gdrive_gcs_toolkit/__init__.py
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-31 07:34:55.166371 shaku-database-1.1.7/gdrive_gcs_toolkit/cloud_storage/
--rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-07-07 09:40:26.000000 shaku-database-1.1.7/gdrive_gcs_toolkit/cloud_storage/__init__.py
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1183 2023-07-07 09:40:26.000000 shaku-database-1.1.7/gdrive_gcs_toolkit/cloud_storage/util.py
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-31 07:34:55.168373 shaku-database-1.1.7/gdrive_gcs_toolkit/google_shared_drive/
--rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-07-07 09:40:26.000000 shaku-database-1.1.7/gdrive_gcs_toolkit/google_shared_drive/__init__.py
--rw-r--r--   0 tongyuhao   (501) staff       (20)    17404 2023-07-31 07:32:41.000000 shaku-database-1.1.7/gdrive_gcs_toolkit/google_shared_drive/util.py
--rw-r--r--   0 tongyuhao   (501) staff       (20)       38 2023-07-31 07:34:55.170955 shaku-database-1.1.7/setup.cfg
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1169 2023-07-31 07:33:01.000000 shaku-database-1.1.7/setup.py
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-31 07:34:55.169690 shaku-database-1.1.7/shaku_database.egg-info/
--rw-r--r--   0 tongyuhao   (501) staff       (20)     7323 2023-07-31 07:34:55.000000 shaku-database-1.1.7/shaku_database.egg-info/PKG-INFO
--rw-r--r--   0 tongyuhao   (501) staff       (20)      666 2023-07-31 07:34:55.000000 shaku-database-1.1.7/shaku_database.egg-info/SOURCES.txt
--rw-r--r--   0 tongyuhao   (501) staff       (20)        1 2023-07-31 07:34:55.000000 shaku-database-1.1.7/shaku_database.egg-info/dependency_links.txt
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1044 2023-07-31 07:34:55.000000 shaku-database-1.1.7/shaku_database.egg-info/requires.txt
--rw-r--r--   0 tongyuhao   (501) staff       (20)       28 2023-07-31 07:34:55.000000 shaku-database-1.1.7/shaku_database.egg-info/top_level.txt
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-08-01 01:27:23.388624 shaku-database-1.1.8/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1069 2023-06-15 08:18:42.000000 shaku-database-1.1.8/LICENSE
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     7323 2023-08-01 01:27:23.388401 shaku-database-1.1.8/PKG-INFO
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     6192 2023-06-15 08:05:19.000000 shaku-database-1.1.8/README.md
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-08-01 01:27:23.386004 shaku-database-1.1.8/database/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.1.8/database/__init__.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-08-01 01:27:23.386366 shaku-database-1.1.8/database/bigquery/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.1.8/database/bigquery/__init__.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1452 2023-07-07 09:40:34.000000 shaku-database-1.1.8/database/bigquery/bq_sql_parser.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1683 2023-06-20 03:32:33.000000 shaku-database-1.1.8/database/bigquery/util.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-08-01 01:27:23.386616 shaku-database-1.1.8/database/cloud_sql/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.1.8/database/cloud_sql/__init__.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1139 2023-06-16 06:51:48.000000 shaku-database-1.1.8/database/cloud_sql/crud.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-08-01 01:27:23.386864 shaku-database-1.1.8/database/cloud_storage/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-07-11 09:09:30.000000 shaku-database-1.1.8/database/cloud_storage/__init__.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1580 2023-07-11 09:00:21.000000 shaku-database-1.1.8/database/cloud_storage/util.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-08-01 01:27:23.386997 shaku-database-1.1.8/gdrive_gcs_toolkit/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-07-07 09:40:26.000000 shaku-database-1.1.8/gdrive_gcs_toolkit/__init__.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-08-01 01:27:23.387227 shaku-database-1.1.8/gdrive_gcs_toolkit/cloud_storage/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-07-07 09:40:26.000000 shaku-database-1.1.8/gdrive_gcs_toolkit/cloud_storage/__init__.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1183 2023-07-07 09:40:26.000000 shaku-database-1.1.8/gdrive_gcs_toolkit/cloud_storage/util.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-08-01 01:27:23.387484 shaku-database-1.1.8/gdrive_gcs_toolkit/google_shared_drive/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-07-07 09:40:26.000000 shaku-database-1.1.8/gdrive_gcs_toolkit/google_shared_drive/__init__.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)    17515 2023-08-01 01:26:48.000000 shaku-database-1.1.8/gdrive_gcs_toolkit/google_shared_drive/util.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)       38 2023-08-01 01:27:23.388667 shaku-database-1.1.8/setup.cfg
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1169 2023-08-01 01:26:50.000000 shaku-database-1.1.8/setup.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-08-01 01:27:23.388177 shaku-database-1.1.8/shaku_database.egg-info/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     7323 2023-08-01 01:27:23.000000 shaku-database-1.1.8/shaku_database.egg-info/PKG-INFO
+-rw-r--r--   0 tongyuhao   (501) staff       (20)      666 2023-08-01 01:27:23.000000 shaku-database-1.1.8/shaku_database.egg-info/SOURCES.txt
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        1 2023-08-01 01:27:23.000000 shaku-database-1.1.8/shaku_database.egg-info/dependency_links.txt
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1044 2023-08-01 01:27:23.000000 shaku-database-1.1.8/shaku_database.egg-info/requires.txt
+-rw-r--r--   0 tongyuhao   (501) staff       (20)       28 2023-08-01 01:27:23.000000 shaku-database-1.1.8/shaku_database.egg-info/top_level.txt
```

### Comparing `shaku-database-1.1.7/LICENSE` & `shaku-database-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `shaku-database-1.1.7/PKG-INFO` & `shaku-database-1.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shaku-database
-Version: 1.1.7
+Version: 1.1.8
 Summary: Shaku Database util
 Home-page: https://gitlab.com/hawktorng1/test_shaku
 Author: hawktorng
 Author-email: hawktorng@shaku.com.tw
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `shaku-database-1.1.7/README.md` & `shaku-database-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `shaku-database-1.1.7/database/bigquery/bq_sql_parser.py` & `shaku-database-1.1.8/database/bigquery/bq_sql_parser.py`

 * *Files identical despite different names*

### Comparing `shaku-database-1.1.7/database/bigquery/util.py` & `shaku-database-1.1.8/database/bigquery/util.py`

 * *Files identical despite different names*

### Comparing `shaku-database-1.1.7/database/cloud_sql/crud.py` & `shaku-database-1.1.8/database/cloud_sql/crud.py`

 * *Files identical despite different names*

### Comparing `shaku-database-1.1.7/database/cloud_storage/util.py` & `shaku-database-1.1.8/database/cloud_storage/util.py`

 * *Files identical despite different names*

### Comparing `shaku-database-1.1.7/gdrive_gcs_toolkit/cloud_storage/util.py` & `shaku-database-1.1.8/gdrive_gcs_toolkit/cloud_storage/util.py`

 * *Files identical despite different names*

### Comparing `shaku-database-1.1.7/gdrive_gcs_toolkit/google_shared_drive/util.py` & `shaku-database-1.1.8/gdrive_gcs_toolkit/google_shared_drive/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,15 +176,15 @@
         folder_info = self.__get_path_info(path)
 
         path_parts = Path(path)
 
         folder_name = path_parts.parent.name
         file_name = path_parts.name
 
-        folder_id = folder_info[folder_name]
+        folder_id = folder_info[folder_name]['id']
 
         # if the last part is file, read the file
         # if len(file_name) > 0:
         file = pd.DataFrame()
         dataframes = self.__file_loader(file_name, folder_id)
         for key in dataframes.keys():
             if file_name in key:
@@ -305,15 +305,15 @@
 
         folder_info = self.__get_path_info(path)
 
         path_parts = Path(path)
 
         folder_name = path_parts.name
 
-        folder_id = folder_info[folder_name]
+        folder_id = folder_info[folder_name]['id']
 
         file_extension = Path(file_name).suffix
 
         try:
 
             if file_extension == ".csv":
                 # .csv is textual data so use StringIO
@@ -391,14 +391,17 @@
                     'mimeType': 'application/vnd.google-apps.folder',
                     'parents': [parent_id]
                 }
                 try:
                     new_folder = self.service.files().create(body=file_metadata, fields="id",
                                                              supportsAllDrives=True).execute()
                     current_dict[path_part] = {"id": new_folder['id']}
+                    path_id = None
+                    current_dict = current_dict[path_part]
                     print(f"folder {path_part} is not existed and has been created.")
                 except HttpError as error:
                     raise f'An error occurred:{error}'
 
         if flag:
-            self.folder_dict = self.__partial_traversal(self.shared_drive_id, self.root_list)
+            self.folder_dict = self.__partial_traversal(self.shared_drive_id, self.root_list[1:])
             print("some folders are not existed and have been created.")
+
```

### Comparing `shaku-database-1.1.7/setup.py` & `shaku-database-1.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 HERE = pathlib.Path(__file__).parent.resolve()
 requirements = (HERE / "requirements.txt").read_text(encoding="utf8")
 EX_INSTALL_REQUIRES = {s.strip().split('==')[0]: s.strip().split('==')[1] if len(s.strip().split('==')) > 1 else ""
                        for s in requirements.split("\n")}
 INSTALL_REQUIRES = [s.strip() for s in requirements.split("\n")]
 setup(
     name="shaku-database",
-    version="1.1.7",
+    version="1.1.8",
     author="hawktorng",
     author_email="hawktorng@shaku.com.tw",
     description="Shaku Database util",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/hawktorng1/test_shaku",
     packages=find_packages(),
```

### Comparing `shaku-database-1.1.7/shaku_database.egg-info/PKG-INFO` & `shaku-database-1.1.8/shaku_database.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shaku-database
-Version: 1.1.7
+Version: 1.1.8
 Summary: Shaku Database util
 Home-page: https://gitlab.com/hawktorng1/test_shaku
 Author: hawktorng
 Author-email: hawktorng@shaku.com.tw
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `shaku-database-1.1.7/shaku_database.egg-info/SOURCES.txt` & `shaku-database-1.1.8/shaku_database.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shaku-database-1.1.7/shaku_database.egg-info/requires.txt` & `shaku-database-1.1.8/shaku_database.egg-info/requires.txt`

 * *Files identical despite different names*

