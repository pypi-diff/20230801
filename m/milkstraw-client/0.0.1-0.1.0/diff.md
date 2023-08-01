# Comparing `tmp/milkstraw-client-0.0.1.tar.gz` & `tmp/milkstraw-client-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "milkstraw-client-0.0.1.tar", last modified: Mon Jun 26 21:32:31 2023, max compression
+gzip compressed data, was "milkstraw-client-0.1.0.tar", last modified: Tue Aug  1 13:15:22 2023, max compression
```

## Comparing `milkstraw-client-0.0.1.tar` & `milkstraw-client-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 ibraheem  (1000) ibraheem  (1000)        0 2023-06-26 21:32:31.680545 milkstraw-client-0.0.1/
--rw-rw-r--   0 ibraheem  (1000) ibraheem  (1000)    11357 2023-06-26 21:30:06.000000 milkstraw-client-0.0.1/LICENSE
--rw-rw-r--   0 ibraheem  (1000) ibraheem  (1000)    17718 2023-06-26 21:32:31.680545 milkstraw-client-0.0.1/PKG-INFO
--rw-rw-r--   0 ibraheem  (1000) ibraheem  (1000)     3989 2023-06-26 21:30:06.000000 milkstraw-client-0.0.1/README.md
--rw-rw-r--   0 ibraheem  (1000) ibraheem  (1000)      889 2023-06-26 21:30:06.000000 milkstraw-client-0.0.1/pyproject.toml
--rw-rw-r--   0 ibraheem  (1000) ibraheem  (1000)       38 2023-06-26 21:32:31.680545 milkstraw-client-0.0.1/setup.cfg
-drwxrwxr-x   0 ibraheem  (1000) ibraheem  (1000)        0 2023-06-26 21:32:31.680545 milkstraw-client-0.0.1/src/
-drwxrwxr-x   0 ibraheem  (1000) ibraheem  (1000)        0 2023-06-26 21:32:31.680545 milkstraw-client-0.0.1/src/milkstraw_client/
--rw-rw-r--   0 ibraheem  (1000) ibraheem  (1000)      474 2023-06-26 21:30:06.000000 milkstraw-client-0.0.1/src/milkstraw_client/__init__.py
--rw-rw-r--   0 ibraheem  (1000) ibraheem  (1000)     1969 2023-06-26 21:30:06.000000 milkstraw-client-0.0.1/src/milkstraw_client/api_client.py
--rw-rw-r--   0 ibraheem  (1000) ibraheem  (1000)     1802 2023-06-26 21:30:06.000000 milkstraw-client-0.0.1/src/milkstraw_client/generated_data.py
--rw-rw-r--   0 ibraheem  (1000) ibraheem  (1000)     1709 2023-06-26 21:30:06.000000 milkstraw-client-0.0.1/src/milkstraw_client/model.py
--rw-rw-r--   0 ibraheem  (1000) ibraheem  (1000)     1441 2023-06-26 21:30:06.000000 milkstraw-client-0.0.1/src/milkstraw_client/source_data.py
-drwxrwxr-x   0 ibraheem  (1000) ibraheem  (1000)        0 2023-06-26 21:32:31.680545 milkstraw-client-0.0.1/src/milkstraw_client.egg-info/
--rw-rw-r--   0 ibraheem  (1000) ibraheem  (1000)    17718 2023-06-26 21:32:31.000000 milkstraw-client-0.0.1/src/milkstraw_client.egg-info/PKG-INFO
--rw-rw-r--   0 ibraheem  (1000) ibraheem  (1000)      424 2023-06-26 21:32:31.000000 milkstraw-client-0.0.1/src/milkstraw_client.egg-info/SOURCES.txt
--rw-rw-r--   0 ibraheem  (1000) ibraheem  (1000)        1 2023-06-26 21:32:31.000000 milkstraw-client-0.0.1/src/milkstraw_client.egg-info/dependency_links.txt
--rw-rw-r--   0 ibraheem  (1000) ibraheem  (1000)       17 2023-06-26 21:32:31.000000 milkstraw-client-0.0.1/src/milkstraw_client.egg-info/requires.txt
--rw-rw-r--   0 ibraheem  (1000) ibraheem  (1000)       17 2023-06-26 21:32:31.000000 milkstraw-client-0.0.1/src/milkstraw_client.egg-info/top_level.txt
+drwxrwxr-x   0 ibraheem  (1000) ibraheem  (1000)        0 2023-08-01 13:15:22.403707 milkstraw-client-0.1.0/
+-rw-rw-r--   0 ibraheem  (1000) ibraheem  (1000)    11357 2023-08-01 12:46:35.000000 milkstraw-client-0.1.0/LICENSE
+-rw-rw-r--   0 ibraheem  (1000) ibraheem  (1000)    17804 2023-08-01 13:15:22.403707 milkstraw-client-0.1.0/PKG-INFO
+-rw-rw-r--   0 ibraheem  (1000) ibraheem  (1000)     4075 2023-08-01 12:46:35.000000 milkstraw-client-0.1.0/README.md
+-rw-rw-r--   0 ibraheem  (1000) ibraheem  (1000)      889 2023-08-01 13:10:57.000000 milkstraw-client-0.1.0/pyproject.toml
+-rw-rw-r--   0 ibraheem  (1000) ibraheem  (1000)       38 2023-08-01 13:15:22.403707 milkstraw-client-0.1.0/setup.cfg
+drwxrwxr-x   0 ibraheem  (1000) ibraheem  (1000)        0 2023-08-01 13:15:22.403707 milkstraw-client-0.1.0/src/
+drwxrwxr-x   0 ibraheem  (1000) ibraheem  (1000)        0 2023-08-01 13:15:22.403707 milkstraw-client-0.1.0/src/milkstraw_client/
+-rw-rw-r--   0 ibraheem  (1000) ibraheem  (1000)      474 2023-08-01 12:46:35.000000 milkstraw-client-0.1.0/src/milkstraw_client/__init__.py
+-rw-rw-r--   0 ibraheem  (1000) ibraheem  (1000)     1969 2023-08-01 12:46:35.000000 milkstraw-client-0.1.0/src/milkstraw_client/api_client.py
+-rw-rw-r--   0 ibraheem  (1000) ibraheem  (1000)     1802 2023-08-01 12:46:35.000000 milkstraw-client-0.1.0/src/milkstraw_client/generated_data.py
+-rw-rw-r--   0 ibraheem  (1000) ibraheem  (1000)     1709 2023-08-01 12:46:35.000000 milkstraw-client-0.1.0/src/milkstraw_client/model.py
+-rw-rw-r--   0 ibraheem  (1000) ibraheem  (1000)     1796 2023-08-01 13:10:57.000000 milkstraw-client-0.1.0/src/milkstraw_client/source_data.py
+drwxrwxr-x   0 ibraheem  (1000) ibraheem  (1000)        0 2023-08-01 13:15:22.403707 milkstraw-client-0.1.0/src/milkstraw_client.egg-info/
+-rw-rw-r--   0 ibraheem  (1000) ibraheem  (1000)    17804 2023-08-01 13:15:22.000000 milkstraw-client-0.1.0/src/milkstraw_client.egg-info/PKG-INFO
+-rw-rw-r--   0 ibraheem  (1000) ibraheem  (1000)      424 2023-08-01 13:15:22.000000 milkstraw-client-0.1.0/src/milkstraw_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 ibraheem  (1000) ibraheem  (1000)        1 2023-08-01 13:15:22.000000 milkstraw-client-0.1.0/src/milkstraw_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 ibraheem  (1000) ibraheem  (1000)       17 2023-08-01 13:15:22.000000 milkstraw-client-0.1.0/src/milkstraw_client.egg-info/requires.txt
+-rw-rw-r--   0 ibraheem  (1000) ibraheem  (1000)       17 2023-08-01 13:15:22.000000 milkstraw-client-0.1.0/src/milkstraw_client.egg-info/top_level.txt
```

### Comparing `milkstraw-client-0.0.1/LICENSE` & `milkstraw-client-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `milkstraw-client-0.0.1/PKG-INFO` & `milkstraw-client-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: milkstraw-client
-Version: 0.0.1
+Version: 0.1.0
 Summary: Generate synthetic data with a simple python client for milkstraw.ai
 Author-email: "Milkstraw AI, Inc." <admin@milkstraw.ai>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -293,7 +293,10 @@
 report_file_path = GeneratedData.download_report(my_generated_data.id, "data/generated_data_report.zip")
 ```
 Instead, you can setup credentials from environment variables:
 ``` shell
 export MILKSTRAW_USER_EMAIL="[YOUR_EMAIL]"
 export MILKSTRAW_USER_PASS="[YOUR_PASSWORD]"
 ```
+
+## Examples
+Please checkout our demo notebooks in the [examples](./examples) folder.
```

### Comparing `milkstraw-client-0.0.1/README.md` & `milkstraw-client-0.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -74,7 +74,10 @@
 report_file_path = GeneratedData.download_report(my_generated_data.id, "data/generated_data_report.zip")
 ```
 Instead, you can setup credentials from environment variables:
 ``` shell
 export MILKSTRAW_USER_EMAIL="[YOUR_EMAIL]"
 export MILKSTRAW_USER_PASS="[YOUR_PASSWORD]"
 ```
+
+## Examples
+Please checkout our demo notebooks in the [examples](./examples) folder.
```

#### html2text {}

```diff
@@ -47,8 +47,9 @@
 GeneratedData.generate(my_model.id, records_num=10000) # Download generated
 data (After `my_generated_data` status becomes `done`) data_file_path =
 GeneratedData.download(my_generated_data.id, "data/generated_data.csv") #
 Download generated data report report_file_path = GeneratedData.download_report
 (my_generated_data.id, "data/generated_data_report.zip") ``` Instead, you can
 setup credentials from environment variables: ``` shell export
 MILKSTRAW_USER_EMAIL="[YOUR_EMAIL]" export MILKSTRAW_USER_PASS="
-[YOUR_PASSWORD]" ```
+[YOUR_PASSWORD]" ``` ## Examples Please checkout our demo notebooks in the
+[examples](./examples) folder.
```

### Comparing `milkstraw-client-0.0.1/pyproject.toml` & `milkstraw-client-0.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "milkstraw-client"
-version = "0.0.1"
+version = "0.1.0"
 description = "Generate synthetic data with a simple python client for milkstraw.ai"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3 :: Only",
     "License :: OSI Approved :: Apache Software License",
```

### Comparing `milkstraw-client-0.0.1/src/milkstraw_client/api_client.py` & `milkstraw-client-0.1.0/src/milkstraw_client/api_client.py`

 * *Files identical despite different names*

### Comparing `milkstraw-client-0.0.1/src/milkstraw_client/generated_data.py` & `milkstraw-client-0.1.0/src/milkstraw_client/generated_data.py`

 * *Files identical despite different names*

### Comparing `milkstraw-client-0.0.1/src/milkstraw_client/model.py` & `milkstraw-client-0.1.0/src/milkstraw_client/model.py`

 * *Files identical despite different names*

### Comparing `milkstraw-client-0.0.1/src/milkstraw_client/source_data.py` & `milkstraw-client-0.1.0/src/milkstraw_client/source_data.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from __future__ import annotations
 
+from typing import Optional
+
 import milkstraw_client
 from milkstraw_client import APIClient
 
 
 class SourceData:
     def __init__(self, id: str, name: str, status: str):
         self.id = id
@@ -11,17 +13,26 @@
         self.status = status
 
     def __repr__(self) -> str:
         attributes = ", ".join(f"{key}='{value}'" for key, value in vars(self).items())
         return f"{self.__class__.__name__}({attributes})"
 
     @staticmethod
-    def upload(name: str, file_path: str) -> SourceData:
+    def upload(
+        name: str,
+        file_path: str,
+        auto_primary_key: Optional[bool] = None,
+        primary_key_column: Optional[str] = None,
+    ) -> SourceData:
         url = f"{milkstraw_client.edge_service_url}/source-data/"
         params = {"name": name}
+        if auto_primary_key is not None:
+            params["auto_primary_key"] = auto_primary_key
+        if primary_key_column is not None:
+            params["primary_key_column"] = primary_key_column
         file_paths = {"file": file_path}
         response = APIClient.request("post", url, params=params, file_paths=file_paths)
         return SourceData(**response)
 
     @staticmethod
     def get(id: str) -> SourceData:
         url = f"{milkstraw_client.edge_service_url}/source-data/{id}"
```

### Comparing `milkstraw-client-0.0.1/src/milkstraw_client.egg-info/PKG-INFO` & `milkstraw-client-0.1.0/src/milkstraw_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: milkstraw-client
-Version: 0.0.1
+Version: 0.1.0
 Summary: Generate synthetic data with a simple python client for milkstraw.ai
 Author-email: "Milkstraw AI, Inc." <admin@milkstraw.ai>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -293,7 +293,10 @@
 report_file_path = GeneratedData.download_report(my_generated_data.id, "data/generated_data_report.zip")
 ```
 Instead, you can setup credentials from environment variables:
 ``` shell
 export MILKSTRAW_USER_EMAIL="[YOUR_EMAIL]"
 export MILKSTRAW_USER_PASS="[YOUR_PASSWORD]"
 ```
+
+## Examples
+Please checkout our demo notebooks in the [examples](./examples) folder.
```

