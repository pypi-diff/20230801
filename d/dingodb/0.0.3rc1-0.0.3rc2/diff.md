# Comparing `tmp/dingodb-0.0.3rc1.tar.gz` & `tmp/dingodb-0.0.3rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dingodb-0.0.3rc1.tar", last modified: Tue Jul 25 09:10:32 2023, max compression
+gzip compressed data, was "dingodb-0.0.3rc2.tar", last modified: Tue Aug  1 03:33:49 2023, max compression
```

## Comparing `dingodb-0.0.3rc1.tar` & `dingodb-0.0.3rc2.tar`

### file list

```diff
@@ -1,24 +1,20 @@
-drwxrwxr-x   0 gary      (1000) gary      (1000)        0 2023-07-25 09:10:32.947487 dingodb-0.0.3rc1/
--rw-rw-r--   0 gary      (1000) gary      (1000)      139 2023-07-18 06:02:01.000000 dingodb-0.0.3rc1/.gitignore
--rw-rw-r--   0 gary      (1000) gary      (1000)       72 2023-07-20 09:31:54.000000 dingodb-0.0.3rc1/MANIFEST.in
--rw-rw-r--   0 gary      (1000) gary      (1000)     5724 2023-07-25 09:10:32.943488 dingodb-0.0.3rc1/PKG-INFO
--rw-rw-r--   0 gary      (1000) gary      (1000)     4317 2023-07-20 09:40:52.000000 dingodb-0.0.3rc1/README.md
-drwxrwxr-x   0 gary      (1000) gary      (1000)        0 2023-07-25 09:10:32.943488 dingodb-0.0.3rc1/dingodb/
--rw-rw-r--   0 gary      (1000) gary      (1000)       60 2023-07-20 09:31:54.000000 dingodb-0.0.3rc1/dingodb/__init__.py
--rw-rw-r--   0 gary      (1000) gary      (1000)       10 2023-07-25 09:10:25.000000 dingodb-0.0.3rc1/dingodb/__version__
--rw-rw-r--   0 gary      (1000) gary      (1000)     1600 2023-07-24 17:07:31.000000 dingodb-0.0.3rc1/dingodb/config.py
--rw-rw-r--   0 gary      (1000) gary      (1000)    14301 2023-07-25 07:10:40.000000 dingodb-0.0.3rc1/dingodb/db.py
--rw-rw-r--   0 gary      (1000) gary      (1000)     7393 2023-07-25 07:10:40.000000 dingodb-0.0.3rc1/dingodb/dingo_param.py
-drwxrwxr-x   0 gary      (1000) gary      (1000)        0 2023-07-25 09:10:32.943488 dingodb-0.0.3rc1/dingodb.egg-info/
--rw-rw-r--   0 gary      (1000) gary      (1000)     5724 2023-07-25 09:10:32.000000 dingodb-0.0.3rc1/dingodb.egg-info/PKG-INFO
--rw-rw-r--   0 gary      (1000) gary      (1000)      350 2023-07-25 09:10:32.000000 dingodb-0.0.3rc1/dingodb.egg-info/SOURCES.txt
--rw-rw-r--   0 gary      (1000) gary      (1000)        1 2023-07-25 09:10:32.000000 dingodb-0.0.3rc1/dingodb.egg-info/dependency_links.txt
--rw-rw-r--   0 gary      (1000) gary      (1000)       62 2023-07-25 09:10:32.000000 dingodb-0.0.3rc1/dingodb.egg-info/requires.txt
--rw-rw-r--   0 gary      (1000) gary      (1000)        8 2023-07-25 09:10:32.000000 dingodb-0.0.3rc1/dingodb.egg-info/top_level.txt
-drwxrwxr-x   0 gary      (1000) gary      (1000)        0 2023-07-25 09:10:32.943488 dingodb-0.0.3rc1/examples/
--rw-rw-r--   0 gary      (1000) gary      (1000)     6413 2023-07-24 17:07:31.000000 dingodb-0.0.3rc1/examples/example.py
--rw-rw-r--   0 gary      (1000) gary      (1000)        0 2023-07-13 06:19:14.000000 dingodb-0.0.3rc1/pyproject.toml
--rw-rw-r--   0 gary      (1000) gary      (1000)       70 2023-07-24 17:07:31.000000 dingodb-0.0.3rc1/requirements.txt
--rw-rw-r--   0 gary      (1000) gary      (1000)       38 2023-07-25 09:10:32.947487 dingodb-0.0.3rc1/setup.cfg
--rw-rw-r--   0 gary      (1000) gary      (1000)     2006 2023-07-20 09:31:54.000000 dingodb-0.0.3rc1/setup.py
--rw-rw-r--   0 gary      (1000) gary      (1000)        0 2023-07-13 05:53:08.000000 dingodb-0.0.3rc1/tox.ini
+drwxrwxr-x   0 gary      (1000) gary      (1000)        0 2023-08-01 03:33:49.360584 dingodb-0.0.3rc2/
+-rw-rw-r--   0 gary      (1000) gary      (1000)       72 2023-07-20 09:31:54.000000 dingodb-0.0.3rc2/MANIFEST.in
+-rw-rw-r--   0 gary      (1000) gary      (1000)     5724 2023-08-01 03:33:49.360584 dingodb-0.0.3rc2/PKG-INFO
+-rw-rw-r--   0 gary      (1000) gary      (1000)     4317 2023-07-20 09:40:52.000000 dingodb-0.0.3rc2/README.md
+drwxrwxr-x   0 gary      (1000) gary      (1000)        0 2023-08-01 03:33:49.360584 dingodb-0.0.3rc2/dingodb/
+-rw-rw-r--   0 gary      (1000) gary      (1000)       60 2023-07-20 09:31:54.000000 dingodb-0.0.3rc2/dingodb/__init__.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)        9 2023-08-01 03:33:33.000000 dingodb-0.0.3rc2/dingodb/__version__
+-rw-rw-r--   0 gary      (1000) gary      (1000)     1636 2023-08-01 03:23:27.000000 dingodb-0.0.3rc2/dingodb/config.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)    14268 2023-08-01 03:23:27.000000 dingodb-0.0.3rc2/dingodb/db.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)     7379 2023-08-01 03:23:27.000000 dingodb-0.0.3rc2/dingodb/dingo_param.py
+drwxrwxr-x   0 gary      (1000) gary      (1000)        0 2023-08-01 03:33:49.360584 dingodb-0.0.3rc2/dingodb.egg-info/
+-rw-rw-r--   0 gary      (1000) gary      (1000)     5724 2023-08-01 03:33:49.000000 dingodb-0.0.3rc2/dingodb.egg-info/PKG-INFO
+-rw-rw-r--   0 gary      (1000) gary      (1000)      311 2023-08-01 03:33:49.000000 dingodb-0.0.3rc2/dingodb.egg-info/SOURCES.txt
+-rw-rw-r--   0 gary      (1000) gary      (1000)        1 2023-08-01 03:33:49.000000 dingodb-0.0.3rc2/dingodb.egg-info/dependency_links.txt
+-rw-rw-r--   0 gary      (1000) gary      (1000)       62 2023-08-01 03:33:49.000000 dingodb-0.0.3rc2/dingodb.egg-info/requires.txt
+-rw-rw-r--   0 gary      (1000) gary      (1000)        8 2023-08-01 03:33:49.000000 dingodb-0.0.3rc2/dingodb.egg-info/top_level.txt
+-rw-rw-r--   0 gary      (1000) gary      (1000)        0 2023-07-13 06:19:14.000000 dingodb-0.0.3rc2/pyproject.toml
+-rw-rw-r--   0 gary      (1000) gary      (1000)       70 2023-07-25 09:23:58.000000 dingodb-0.0.3rc2/requirements.txt
+-rw-rw-r--   0 gary      (1000) gary      (1000)       38 2023-08-01 03:33:49.360584 dingodb-0.0.3rc2/setup.cfg
+-rw-rw-r--   0 gary      (1000) gary      (1000)     2006 2023-07-20 09:31:54.000000 dingodb-0.0.3rc2/setup.py
```

### Comparing `dingodb-0.0.3rc1/PKG-INFO` & `dingodb-0.0.3rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dingodb
-Version: 0.0.3rc1
+Version: 0.0.3rc2
 Summary: dingodb is dingodb sdk
 Home-page: https://www.dingodb.com/
 Author: DingoDB
 Author-email: dingodb@zetyun.com
 License: Proprietary License
 Project-URL: Homepage, https://www.dingodb.com/
 Project-URL: Documentation, https://dingodb.readthedocs.io/en/latest/
```

### Comparing `dingodb-0.0.3rc1/README.md` & `dingodb-0.0.3rc2/README.md`

 * *Files identical despite different names*

### Comparing `dingodb-0.0.3rc1/dingodb/config.py` & `dingodb-0.0.3rc2/dingodb/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 metric_type = {
     "euclidean": "METRIC_TYPE_L2",
-    "dotproduct": "METRIC_TYPE_INNER_PRODUCT"
+    "dotproduct": "METRIC_TYPE_INNER_PRODUCT",
+    "cosine": "METRIC_TYPE_COSINE"
 }
 
 
 # proto
 index_config = {
     "flat": {
                 "flatParam": {
```

### Comparing `dingodb-0.0.3rc1/dingodb/db.py` & `dingodb-0.0.3rc2/dingodb/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,26 +49,26 @@
         res = self.session.get(f"{self.requestProto}{self.host[0]}{self.indexApi}{index_name}", headers=self.headers)
         
         if res.status_code == 200:
             return res.json()
         else:
             raise RuntimeError(res.json())
 
-    def create_index(self,  index_name: str, dimension: int, index_type: str = "hnsw", metric_type: str = "euclidean",
+    def create_index(self,  index_name: str, dimension: int, index_type: str = "hnsw", metric_type: str = "cosine",
                      replicas: int = 3, index_config: dict = None, metadata_config: dict = None,
                      partition_rule: dict = None, operand: list = None, auto_id: bool = True,
                      start_id: int = 1) -> bool:
         """
         create_index create index
 
         Args:
             index_name (str): the name of index
             dimension (int): dimension of vector
             index_type (str, optional): index type, one of {"flat", "hnsw"}. Defaults to "hnsw".
-            metric_type (str, optional): metric type, one of {"dotproduct", "euclidean"}. Defaults to "euclidean".
+            metric_type (str, optional): metric type, one of {"dotproduct", "euclidean", "cosine"}. Defaults to "cosine"
             replicas (int, optional): dingoDB store replicas. Defaults to 3.
             index_config (dict, optional): Advanced configuration options for the index. Defaults to None.
             metadata_config (dict, optional): metadata. Defaults to None.
             partition_rule (dict, optional): partition rule. Defaults to None.
             operand (list, optional): operand. Defaults to None.
             auto_id (bool, optional): isAutoIncrement or not isAutoIncrement. Defaults to True.
             start_id (int, optional): autoIncrement start id. Defaults to 1.
@@ -222,42 +222,42 @@
             records = res.json()
             return records.get("currentCount") - records.get("deletedCount")
         else:
             raise RuntimeError(res.json())
         
     def vector_scan(self, index_name: str, start_id: int, max_count: int = 1000, is_reverse: bool = False,
                     with_scalar_data: bool = True, with_table_data: bool = True, without_vector_data: bool = False,
-                    filter_scalar: list = None) -> list:
+                    fields: list = None) -> list:
         """
         vector_scan scan with start_id
 
         Args:
             index_name (str): the name of in index
             start_id (int): start id
             max_count (int, optional): max scan count. Defaults to 1000.
             is_reverse (bool, optional): whether or not reverse. Defaults to False.
             with_scalar_data (bool, optional): whether  with scalar info. Defaults to True.
             with_table_data (bool, optional): whether  with table info. Defaults to True.
             without_vector_data (bool, optional): whether with vector info. Defaults to False.
-            filter_scalar (list, optional): scalar filter filed. Defaults to [].
+            fields (list, optional): fields for return . Defaults to [].
 
         Raises:
             RuntimeError: return error
 
         Returns:
             list:  scan info list
         """
         params = CheckVectorScanParam(index_name=index_name, start_id=start_id, max_count=max_count,
                                       is_reverse=is_reverse, with_scalar_data=with_scalar_data,
                                       with_table_data=with_table_data, without_vector_data=without_vector_data,
-                                      filter_scalar=filter_scalar)
+                                      fields=fields)
         payload = {
             "isReverseScan": params.is_reverse,
             "maxScanCount": params.max_count,
-            "selectedKeys": params.filter_scalar,
+            "selectedKeys": params.fields,
             "startId": params.start_id,
             "withScalarData": params.with_scalar_data,
             "withTableData": params.with_table_data,
             "withoutVectorData": params.without_vector_data
         }
         res = self.session.post(f"{self.requestProto}{self.host[0]}{self.vectorApi}{params.index_name}/scan",
                                 headers=self.headers, data=json.dumps(payload))
```

### Comparing `dingodb-0.0.3rc1/dingodb/dingo_param.py` & `dingodb-0.0.3rc2/dingodb/dingo_param.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,28 +106,28 @@
     index_name: str
     start_id: int
     max_count: int = 1000
     is_reverse: bool = False
     with_scalar_data: bool = True
     with_table_data: bool = True
     without_vector_data: bool = False
-    filter_scalar: list = None
+    fields: list = None
     
     @validator("*", always=True)
     def check_input(cls, value, field):
         if field.name == "start_id":
             if not value > 0:
                 raise Exception("start_id must > 0")   
         if field.name == "max_count":
             if not value > 0:
                 raise Exception("max_count must > 0")
         if field.name == "is_reverse" or field.name == "with_scalar_data" or field.name == "with_table_data" or \
                 field.name == "without_vector_data":
             value = "true" if value else "false"
-        if field.name == "filter_scalar":
+        if field.name == "fields":
             if value is None:
                 value = []
 
         return value
 
 
 class CheckVectorSearchParam(BaseModel):
```

### Comparing `dingodb-0.0.3rc1/dingodb.egg-info/PKG-INFO` & `dingodb-0.0.3rc2/dingodb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dingodb
-Version: 0.0.3rc1
+Version: 0.0.3rc2
 Summary: dingodb is dingodb sdk
 Home-page: https://www.dingodb.com/
 Author: DingoDB
 Author-email: dingodb@zetyun.com
 License: Proprietary License
 Project-URL: Homepage, https://www.dingodb.com/
 Project-URL: Documentation, https://dingodb.readthedocs.io/en/latest/
```

### Comparing `dingodb-0.0.3rc1/setup.py` & `dingodb-0.0.3rc2/setup.py`

 * *Files identical despite different names*

