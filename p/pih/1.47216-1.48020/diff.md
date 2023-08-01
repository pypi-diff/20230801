# Comparing `tmp/pih-1.47216.tar.gz` & `tmp/pih-1.48020.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-1.47216.tar", last modified: Tue Aug  1 02:44:53 2023, max compression
+gzip compressed data, was "pih-1.48020.tar", last modified: Tue Aug  1 03:00:38 2023, max compression
```

## Comparing `pih-1.47216.tar` & `pih-1.48020.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 02:44:53.910902 pih-1.47216/
--rw-rw-rw-   0        0        0      261 2023-08-01 02:44:53.926512 pih-1.47216/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-01 02:44:53.692170 pih-1.47216/pih/
--rw-rw-rw-   0        0        0      157 2022-12-03 14:38:35.000000 pih-1.47216/pih/__init__.py
--rw-rw-rw-   0        0        0    20482 2023-07-25 14:36:49.000000 pih-1.47216/pih/collection.py
--rw-rw-rw-   0        0        0    61053 2023-08-01 02:43:31.000000 pih-1.47216/pih/console_api.py
--rw-rw-rw-   0        0        0   111144 2023-08-01 00:39:59.000000 pih-1.47216/pih/const.py
--rw-rw-rw-   0        0        0   317177 2023-08-01 02:44:45.000000 pih-1.47216/pih/pih.py
--rw-rw-rw-   0        0        0    24697 2023-07-28 13:13:08.000000 pih-1.47216/pih/rpc.py
--rw-rw-rw-   0        0        0     1941 2022-07-31 10:55:18.000000 pih-1.47216/pih/rpcCommandCall_pb2.py
--rw-rw-rw-   0        0        0     2465 2022-08-05 02:38:47.000000 pih-1.47216/pih/rpcCommandCall_pb2_grpc.py
--rw-rw-rw-   0        0        0     2576 2023-07-31 23:11:58.000000 pih-1.47216/pih/rpc_collection.py
--rw-rw-rw-   0        0        0     6453 2023-07-24 14:50:22.000000 pih-1.47216/pih/rpc_const.py
--rw-rw-rw-   0        0        0      635 2023-06-11 13:35:46.000000 pih-1.47216/pih/service_example.py
--rw-rw-rw-   0        0        0    38229 2023-08-01 02:41:41.000000 pih-1.47216/pih/tools.py
--rw-rw-rw-   0        0        0     2280 2023-06-30 04:39:52.000000 pih-1.47216/pih/widgets.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:44:53.879652 pih-1.47216/pih.egg-info/
--rw-rw-rw-   0        0        0      261 2023-08-01 02:44:51.000000 pih-1.47216/pih.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      381 2023-08-01 02:44:52.000000 pih-1.47216/pih.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 02:44:51.000000 pih-1.47216/pih.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-08-01 02:44:52.000000 pih-1.47216/pih.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-08-01 02:44:52.000000 pih-1.47216/pih.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2009 2023-08-01 00:47:12.000000 pih-1.47216/pih_setup.py
--rw-rw-rw-   0        0        0       42 2023-08-01 02:44:53.942144 pih-1.47216/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-01 03:00:38.498666 pih-1.48020/
+-rw-rw-rw-   0        0        0      261 2023-08-01 03:00:38.451792 pih-1.48020/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-01 03:00:37.309183 pih-1.48020/pih/
+-rw-rw-rw-   0        0        0      157 2022-12-03 14:38:35.000000 pih-1.48020/pih/__init__.py
+-rw-rw-rw-   0        0        0    20482 2023-07-25 14:36:49.000000 pih-1.48020/pih/collection.py
+-rw-rw-rw-   0        0        0    61053 2023-08-01 02:43:31.000000 pih-1.48020/pih/console_api.py
+-rw-rw-rw-   0        0        0   111144 2023-08-01 00:39:59.000000 pih-1.48020/pih/const.py
+-rw-rw-rw-   0        0        0   317177 2023-08-01 02:58:15.000000 pih-1.48020/pih/pih.py
+-rw-rw-rw-   0        0        0    24697 2023-07-28 13:13:08.000000 pih-1.48020/pih/rpc.py
+-rw-rw-rw-   0        0        0     1941 2022-07-31 10:55:18.000000 pih-1.48020/pih/rpcCommandCall_pb2.py
+-rw-rw-rw-   0        0        0     2465 2022-08-05 02:38:47.000000 pih-1.48020/pih/rpcCommandCall_pb2_grpc.py
+-rw-rw-rw-   0        0        0     2576 2023-07-31 23:11:58.000000 pih-1.48020/pih/rpc_collection.py
+-rw-rw-rw-   0        0        0     6453 2023-07-24 14:50:22.000000 pih-1.48020/pih/rpc_const.py
+-rw-rw-rw-   0        0        0      635 2023-06-11 13:35:46.000000 pih-1.48020/pih/service_example.py
+-rw-rw-rw-   0        0        0    38229 2023-08-01 02:41:41.000000 pih-1.48020/pih/tools.py
+-rw-rw-rw-   0        0        0     2280 2023-06-30 04:39:52.000000 pih-1.48020/pih/widgets.py
+drwxrwxrwx   0        0        0        0 2023-08-01 03:00:38.248674 pih-1.48020/pih.egg-info/
+-rw-rw-rw-   0        0        0      261 2023-08-01 03:00:31.000000 pih-1.48020/pih.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2023-08-01 03:00:33.000000 pih-1.48020/pih.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 03:00:31.000000 pih-1.48020/pih.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-08-01 03:00:32.000000 pih-1.48020/pih.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-08-01 03:00:32.000000 pih-1.48020/pih.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2009 2023-08-01 00:47:12.000000 pih-1.48020/pih_setup.py
+-rw-rw-rw-   0        0        0       42 2023-08-01 03:00:38.623702 pih-1.48020/setup.cfg
```

### Comparing `pih-1.47216/pih/collection.py` & `pih-1.48020/pih/collection.py`

 * *Files identical despite different names*

### Comparing `pih-1.47216/pih/console_api.py` & `pih-1.48020/pih/console_api.py`

 * *Files identical despite different names*

### Comparing `pih-1.47216/pih/const.py` & `pih-1.48020/pih/const.py`

 * *Files identical despite different names*

### Comparing `pih-1.47216/pih/pih.py` & `pih-1.48020/pih/pih.py`

 * *Files 0% similar despite different names*

```diff
@@ -1633,19 +1633,19 @@
 
     class VERSION:
 
         class MIO:
             
             @staticmethod
             def local() -> str:
-                return "1.48016"  
+                return "1.48020"  
 
         @staticmethod
         def local() -> str:
-            return "1.47216"
+            return "1.48020"
 
         @staticmethod
         def need_update() -> bool:
             return False
             #return importlib.util.find_spec(PIH.NAME) is not None and PIH.VERSION.local() < PIH.VERSION.remote()
     
     class INPUT_WAIT:
```

### Comparing `pih-1.47216/pih/rpc.py` & `pih-1.48020/pih/rpc.py`

 * *Files identical despite different names*

### Comparing `pih-1.47216/pih/rpcCommandCall_pb2.py` & `pih-1.48020/pih/rpcCommandCall_pb2.py`

 * *Files identical despite different names*

### Comparing `pih-1.47216/pih/rpcCommandCall_pb2_grpc.py` & `pih-1.48020/pih/rpcCommandCall_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pih-1.47216/pih/rpc_collection.py` & `pih-1.48020/pih/rpc_collection.py`

 * *Files identical despite different names*

### Comparing `pih-1.47216/pih/rpc_const.py` & `pih-1.48020/pih/rpc_const.py`

 * *Files identical despite different names*

### Comparing `pih-1.47216/pih/service_example.py` & `pih-1.48020/pih/service_example.py`

 * *Files identical despite different names*

### Comparing `pih-1.47216/pih/tools.py` & `pih-1.48020/pih/tools.py`

 * *Files identical despite different names*

### Comparing `pih-1.47216/pih/widgets.py` & `pih-1.48020/pih/widgets.py`

 * *Files identical despite different names*

### Comparing `pih-1.47216/pih_setup.py` & `pih-1.48020/pih_setup.py`

 * *Files identical despite different names*

