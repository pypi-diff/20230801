# Comparing `tmp/aws_feature_store-0.0.8.tar.gz` & `tmp/aws_feature_store-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/ihor/Documents/Py/Yay/ml_services/aws_feature_store/dist/tmpfs3i57mz/aws_feature_store-0.0.8.tar", last modified: Wed Nov 23 11:39:41 2022, max compression
+gzip compressed data, was "/Users/ihor/Documents/Py/Yay/ml_services/aws_feature_store/dist/.tmp-g1fczkbc/aws_feature_store-0.0.9.tar", last modified: Wed Nov 23 18:58:26 2022, max compression
```

## Comparing `aws_feature_store-0.0.8.tar` & `aws_feature_store-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 ihor       (501) staff       (20)        0 2022-11-23 11:39:41.684768 aws_feature_store-0.0.8/
--rw-r--r--   0 ihor       (501) staff       (20)    11357 2022-11-22 14:06:42.000000 aws_feature_store-0.0.8/LICENSE
--rw-r--r--   0 ihor       (501) staff       (20)      748 2022-11-23 11:39:41.684294 aws_feature_store-0.0.8/PKG-INFO
--rw-r--r--   0 ihor       (501) staff       (20)     1316 2022-11-22 15:32:09.000000 aws_feature_store-0.0.8/README.md
-drwxr-xr-x   0 ihor       (501) staff       (20)        0 2022-11-23 11:39:41.680402 aws_feature_store-0.0.8/aws_feature_store/
--rw-r--r--   0 ihor       (501) staff       (20)       29 2022-11-22 18:47:39.000000 aws_feature_store-0.0.8/aws_feature_store/__init__.py
--rw-r--r--   0 ihor       (501) staff       (20)      964 2022-11-22 18:49:06.000000 aws_feature_store-0.0.8/aws_feature_store/feature_definition.py
--rw-r--r--   0 ihor       (501) staff       (20)     8105 2022-11-23 11:39:12.000000 aws_feature_store-0.0.8/aws_feature_store/feature_group.py
--rw-r--r--   0 ihor       (501) staff       (20)     6319 2022-11-22 14:57:16.000000 aws_feature_store-0.0.8/aws_feature_store/inputs.py
-drwxr-xr-x   0 ihor       (501) staff       (20)        0 2022-11-23 11:39:41.683732 aws_feature_store-0.0.8/aws_feature_store.egg-info/
--rw-r--r--   0 ihor       (501) staff       (20)      748 2022-11-23 11:39:41.000000 aws_feature_store-0.0.8/aws_feature_store.egg-info/PKG-INFO
--rw-r--r--   0 ihor       (501) staff       (20)      363 2022-11-23 11:39:41.000000 aws_feature_store-0.0.8/aws_feature_store.egg-info/SOURCES.txt
--rw-r--r--   0 ihor       (501) staff       (20)        1 2022-11-23 11:39:41.000000 aws_feature_store-0.0.8/aws_feature_store.egg-info/dependency_links.txt
--rw-r--r--   0 ihor       (501) staff       (20)       27 2022-11-23 11:39:41.000000 aws_feature_store-0.0.8/aws_feature_store.egg-info/requires.txt
--rw-r--r--   0 ihor       (501) staff       (20)       67 2022-11-23 11:39:41.000000 aws_feature_store-0.0.8/aws_feature_store.egg-info/top_level.txt
--rw-r--r--   0 ihor       (501) staff       (20)       38 2022-11-23 11:39:41.684911 aws_feature_store-0.0.8/setup.cfg
--rw-r--r--   0 ihor       (501) staff       (20)     1336 2022-11-23 11:39:29.000000 aws_feature_store-0.0.8/setup.py
+drwxr-xr-x   0 ihor       (501) staff       (20)        0 2022-11-23 18:58:26.004154 aws_feature_store-0.0.9/
+-rw-r--r--   0 ihor       (501) staff       (20)    11357 2022-11-22 14:06:42.000000 aws_feature_store-0.0.9/LICENSE
+-rw-r--r--   0 ihor       (501) staff       (20)      748 2022-11-23 18:58:26.003828 aws_feature_store-0.0.9/PKG-INFO
+-rw-r--r--   0 ihor       (501) staff       (20)     1316 2022-11-22 15:32:09.000000 aws_feature_store-0.0.9/README.md
+drwxr-xr-x   0 ihor       (501) staff       (20)        0 2022-11-23 18:58:25.998789 aws_feature_store-0.0.9/aws_feature_store/
+-rw-r--r--   0 ihor       (501) staff       (20)       29 2022-11-22 18:47:39.000000 aws_feature_store-0.0.9/aws_feature_store/__init__.py
+-rw-r--r--   0 ihor       (501) staff       (20)      964 2022-11-22 18:49:06.000000 aws_feature_store-0.0.9/aws_feature_store/feature_definition.py
+-rw-r--r--   0 ihor       (501) staff       (20)     8421 2022-11-23 18:54:27.000000 aws_feature_store-0.0.9/aws_feature_store/feature_group.py
+-rw-r--r--   0 ihor       (501) staff       (20)     6319 2022-11-22 14:57:16.000000 aws_feature_store-0.0.9/aws_feature_store/inputs.py
+drwxr-xr-x   0 ihor       (501) staff       (20)        0 2022-11-23 18:58:26.003414 aws_feature_store-0.0.9/aws_feature_store.egg-info/
+-rw-r--r--   0 ihor       (501) staff       (20)      748 2022-11-23 18:58:25.000000 aws_feature_store-0.0.9/aws_feature_store.egg-info/PKG-INFO
+-rw-r--r--   0 ihor       (501) staff       (20)      363 2022-11-23 18:58:25.000000 aws_feature_store-0.0.9/aws_feature_store.egg-info/SOURCES.txt
+-rw-r--r--   0 ihor       (501) staff       (20)        1 2022-11-23 18:58:25.000000 aws_feature_store-0.0.9/aws_feature_store.egg-info/dependency_links.txt
+-rw-r--r--   0 ihor       (501) staff       (20)       27 2022-11-23 18:58:25.000000 aws_feature_store-0.0.9/aws_feature_store.egg-info/requires.txt
+-rw-r--r--   0 ihor       (501) staff       (20)       67 2022-11-23 18:58:25.000000 aws_feature_store-0.0.9/aws_feature_store.egg-info/top_level.txt
+-rw-r--r--   0 ihor       (501) staff       (20)       38 2022-11-23 18:58:26.004253 aws_feature_store-0.0.9/setup.cfg
+-rw-r--r--   0 ihor       (501) staff       (20)     1336 2022-11-23 18:56:39.000000 aws_feature_store-0.0.9/setup.py
```

### Comparing `aws_feature_store-0.0.8/LICENSE` & `aws_feature_store-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aws_feature_store-0.0.8/PKG-INFO` & `aws_feature_store-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws_feature_store
-Version: 0.0.8
+Version: 0.0.9
 Summary: Simplified SageMaker Feature Store
 Home-page: https://github.com/bilykigor/aws_feature_store
 Author: Ihor Bilyk
 License: Apache License 2.0
 Keywords: Simplified SageMaker Feature Store
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `aws_feature_store-0.0.8/README.md` & `aws_feature_store-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `aws_feature_store-0.0.8/aws_feature_store/feature_definition.py` & `aws_feature_store-0.0.9/aws_feature_store/feature_definition.py`

 * *Files identical despite different names*

### Comparing `aws_feature_store-0.0.8/aws_feature_store/feature_group.py` & `aws_feature_store-0.0.9/aws_feature_store/feature_group.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import pandas as pd
 from pandas import DataFrame
 from time import gmtime, strftime
 import awswrangler as wr
 import json
 import boto3
+import logging
+
 from boto3.session import Session
 
 from aws_feature_store.feature_definition import (
     FeatureDefinition,
     FeatureTypeEnum,
 )
 
@@ -43,72 +45,84 @@
         name: str,
         s3_uri: str,
         boto3_session: Session):
         
         self.name = name
         self.s3_uri = s3_uri
         self.boto3_session = boto3_session
-        
+        #==========================================
+        print('debug')
         #==========================================
         
         bucket_name = s3_uri.replace('s3://','').split('/')[0]
         s3_folder = s3_uri.replace(f's3://{bucket_name}/','')
         
         if len(s3_folder)==0:
             raise
         
         if s3_folder[-1]=='/':
             s3_folder = s3_folder[:-1]
         
         self.s3_folder = s3_folder
+        self.bucket_name = bucket_name
         self.bucket = boto3_session.resource('s3').Bucket(bucket_name)
         
+        #===set up utils functions ================
         json.load_s3 = lambda f: json.load(self.bucket.Object(key=f).get()["Body"])
         json.dump_s3 = lambda obj, f: self.bucket.Object(key=f).put(Body=json.dumps(obj))
         
         #===check bucket existance=================
         folder_exists=False
-        for folder_exists in self.bucket.objects.filter(Prefix=f'{s3_folder}/'):
+        for folder_exists in self.bucket.objects.filter(Prefix=f'{self.s3_folder}/'):
             break
         if not folder_exists:
             logging.error(f'Folder {s3_folder}/ does not exist.')
             raise
                 
         for folder in ['data','meta_data']:
             folder_exists=False
-            for folder_exists in self.bucket.objects.filter(Prefix=f'{s3_folder}/{folder}/'):
+            for folder_exists in self.bucket.objects.filter(Prefix=f'{self.s3_folder}/{folder}/'):
                 break
             if not folder_exists:
                 logging.warn(f'Folder {s3_folder}/{folder}/ does not exist. Will be created')
                 status = self.bucket.put_object(Key=f'{s3_folder}/{folder}/')
                  
-        
         #===check if feature_group_exists===========
-        if self.exists():
-            objs = [o for o in self.bucket.objects.filter(Prefix=f'{s3_folder}/meta_data/{self.name}/')]
-            self.create_feature_store_args = json.load_s3(objs[-1].key)
+        exists_name = self.exists()
+        if exists_name is not None:
+            print(f'Found feature group {exists_name}')
+            self.create_feature_store_args = json.load_s3(exists_name)
+            self.name = exists_name.replace('/config.json','').replace(f'{s3_folder}/{folder}/','')
     
     
     def exists(self):
         #===check if feature_group_exists===========
-        for folder in ['data','meta_data']:
-            feature_group_exists=False
-            for feature_group_exists in self.bucket.objects.filter(Prefix=f'{s3_folder}/{folder}/{self.name}/'):
-                break
-            if not feature_group_exists:
-                return False
-            
+        s3=self.boto3_session.client('s3')
+        rsp = s3.list_objects_v2(Bucket=self.bucket_name, Prefix=f'{self.s3_folder}/data/{self.name}', Delimiter="/")
+        if rsp['KeyCount']==0:
+            return None
+        
+        objs=list(obj["Prefix"] for obj in rsp["CommonPrefixes"])
+        
+        #get last oblect
+        key = objs[-1]
+        key=key.replace('/data/','/meta_data/')
+        
+        objs = [o for o in self.bucket.objects.filter(Prefix=key)]
+        if len(objs)==0:
+            return None
+        
         try:
-            objs = [o for o in self.bucket.objects.filter(Prefix=f'{s3_folder}/meta_data/{self.name}/')]
-            self.create_feature_store_args = json.load_s3(objs[-1].key)
+            #print(f'Read config from {objs[-1].key}')
+            json.load_s3(objs[-1].key)
         except Exception as e:
-            logging.war('Failed to read config for {self.name}')
-            return False
+            print(f'Failed to read config for {self.name}\n{e}')
+            return None
         
-        return True
+        return objs[-1].key
         
 
     def create(
         self,
         event_time_feature_name: str,
         record_identifier_name: str = None,
         description: str = None,
@@ -142,39 +156,38 @@
             data_source=data_source,
             tags=tags,
         )
 
         s3_uri = self.s3_uri
         
         #===check feature_group_exists===========
-        feature_group_exists=False
-        for feature_group_exists in self.bucket.objects.filter(Prefix=f'{self.s3_folder}/data/{self.name}/'):
-            break
-        if feature_group_exists:
+        if self.exists() is not None:
             raise
         #========================================
         
+        fg_time = gmtime()
+        fg_timestamp = strftime("%Y-%m-%d'T'%H:%M:%SZ", fg_time)
+        
         #===create folder =======================
+        self.name = f'{self.name}_{fg_timestamp}'
         status = self.bucket.put_object(Key=f'{self.s3_folder}/data/{self.name}/')
     
         #===create config =======================
         s3_storage_config = S3StorageConfig(s3_uri=s3_uri)
         offline_store_config = OfflineStoreConfig(
             s3_storage_config=s3_storage_config,
             data_catalog_config=None,
         )
         create_feature_store_args.update(
             {"offline_store_config": offline_store_config.to_dict()}
         )
         self.create_feature_store_args = create_feature_store_args
         
         #===record config to meta_data==========
-        fg_time = gmtime()
-        fg_timestamp = strftime("%Y-%m-%d'T'%H:%M:%SZ", fg_time)
-        key = f'{self.s3_folder}/meta_data/{self.name}/{fg_timestamp}.json'
+        key = f'{self.s3_folder}/meta_data/{self.name}/config.json'
         json.dump_s3(create_feature_store_args, key)
         
         return create_feature_store_args
             
     def describe(
         self,
     ):
```

### Comparing `aws_feature_store-0.0.8/aws_feature_store/inputs.py` & `aws_feature_store-0.0.9/aws_feature_store/inputs.py`

 * *Files identical despite different names*

### Comparing `aws_feature_store-0.0.8/aws_feature_store.egg-info/PKG-INFO` & `aws_feature_store-0.0.9/aws_feature_store.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-feature-store
-Version: 0.0.8
+Version: 0.0.9
 Summary: Simplified SageMaker Feature Store
 Home-page: https://github.com/bilykigor/aws_feature_store
 Author: Ihor Bilyk
 License: Apache License 2.0
 Keywords: Simplified SageMaker Feature Store
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `aws_feature_store-0.0.8/setup.py` & `aws_feature_store-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 required_packages = [
     "boto3>=1.20.21,<2.0",
     "pandas",
 ]
 
 setup(
     name="aws_feature_store",
-    version="0.0.8",
+    version="0.0.9",
     description="Simplified SageMaker Feature Store",
     packages=find_packages(),
     py_modules=[os.path.splitext(os.path.basename(path))[0] for path in glob("aws_feature_store/*.py")],
     include_package_data=True,
     author="Ihor Bilyk",
     url="https://github.com/bilykigor/aws_feature_store",
     license="Apache License 2.0",
```

