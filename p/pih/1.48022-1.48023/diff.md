# Comparing `tmp/pih-1.48022.tar.gz` & `tmp/pih-1.48023.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-1.48022.tar", last modified: Tue Aug  1 03:14:24 2023, max compression
+gzip compressed data, was "pih-1.48023.tar", last modified: Tue Aug  1 03:17:21 2023, max compression
```

## Comparing `pih-1.48022.tar` & `pih-1.48023.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 03:14:23.495849 pih-1.48022/
--rw-rw-rw-   0        0        0      261 2023-08-01 03:14:24.292715 pih-1.48022/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-01 03:14:24.120844 pih-1.48022/pih/
--rw-rw-rw-   0        0        0      157 2022-12-03 14:38:35.000000 pih-1.48022/pih/__init__.py
--rw-rw-rw-   0        0        0    20482 2023-07-25 14:36:49.000000 pih-1.48022/pih/collection.py
--rw-rw-rw-   0        0        0    61125 2023-08-01 03:14:05.000000 pih-1.48022/pih/console_api.py
--rw-rw-rw-   0        0        0   111144 2023-08-01 00:39:59.000000 pih-1.48022/pih/const.py
--rw-rw-rw-   0        0        0   317177 2023-08-01 03:14:16.000000 pih-1.48022/pih/pih.py
--rw-rw-rw-   0        0        0    24697 2023-07-28 13:13:08.000000 pih-1.48022/pih/rpc.py
--rw-rw-rw-   0        0        0     1941 2022-07-31 10:55:18.000000 pih-1.48022/pih/rpcCommandCall_pb2.py
--rw-rw-rw-   0        0        0     2465 2022-08-05 02:38:47.000000 pih-1.48022/pih/rpcCommandCall_pb2_grpc.py
--rw-rw-rw-   0        0        0     2576 2023-07-31 23:11:58.000000 pih-1.48022/pih/rpc_collection.py
--rw-rw-rw-   0        0        0     6453 2023-07-24 14:50:22.000000 pih-1.48022/pih/rpc_const.py
--rw-rw-rw-   0        0        0      635 2023-06-11 13:35:46.000000 pih-1.48022/pih/service_example.py
--rw-rw-rw-   0        0        0    38229 2023-08-01 02:41:41.000000 pih-1.48022/pih/tools.py
--rw-rw-rw-   0        0        0     2280 2023-06-30 04:39:52.000000 pih-1.48022/pih/widgets.py
-drwxrwxrwx   0        0        0        0 2023-08-01 03:14:24.277090 pih-1.48022/pih.egg-info/
--rw-rw-rw-   0        0        0      261 2023-08-01 03:14:22.000000 pih-1.48022/pih.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      381 2023-08-01 03:14:23.000000 pih-1.48022/pih.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 03:14:22.000000 pih-1.48022/pih.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-08-01 03:14:23.000000 pih-1.48022/pih.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-08-01 03:14:23.000000 pih-1.48022/pih.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2009 2023-08-01 00:47:12.000000 pih-1.48022/pih_setup.py
--rw-rw-rw-   0        0        0       42 2023-08-01 03:14:24.308339 pih-1.48022/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-01 03:17:22.011976 pih-1.48023/
+-rw-rw-rw-   0        0        0      261 2023-08-01 03:17:21.996351 pih-1.48023/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-01 03:17:21.746354 pih-1.48023/pih/
+-rw-rw-rw-   0        0        0      157 2022-12-03 14:38:35.000000 pih-1.48023/pih/__init__.py
+-rw-rw-rw-   0        0        0    20482 2023-07-25 14:36:49.000000 pih-1.48023/pih/collection.py
+-rw-rw-rw-   0        0        0    61125 2023-08-01 03:14:05.000000 pih-1.48023/pih/console_api.py
+-rw-rw-rw-   0        0        0   111144 2023-08-01 00:39:59.000000 pih-1.48023/pih/const.py
+-rw-rw-rw-   0        0        0   317173 2023-08-01 03:17:06.000000 pih-1.48023/pih/pih.py
+-rw-rw-rw-   0        0        0    24697 2023-07-28 13:13:08.000000 pih-1.48023/pih/rpc.py
+-rw-rw-rw-   0        0        0     1941 2022-07-31 10:55:18.000000 pih-1.48023/pih/rpcCommandCall_pb2.py
+-rw-rw-rw-   0        0        0     2465 2022-08-05 02:38:47.000000 pih-1.48023/pih/rpcCommandCall_pb2_grpc.py
+-rw-rw-rw-   0        0        0     2576 2023-07-31 23:11:58.000000 pih-1.48023/pih/rpc_collection.py
+-rw-rw-rw-   0        0        0     6453 2023-07-24 14:50:22.000000 pih-1.48023/pih/rpc_const.py
+-rw-rw-rw-   0        0        0      635 2023-06-11 13:35:46.000000 pih-1.48023/pih/service_example.py
+-rw-rw-rw-   0        0        0    38229 2023-08-01 02:41:41.000000 pih-1.48023/pih/tools.py
+-rw-rw-rw-   0        0        0     2280 2023-06-30 04:39:52.000000 pih-1.48023/pih/widgets.py
+drwxrwxrwx   0        0        0        0 2023-08-01 03:17:21.965101 pih-1.48023/pih.egg-info/
+-rw-rw-rw-   0        0        0      261 2023-08-01 03:17:19.000000 pih-1.48023/pih.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2023-08-01 03:17:20.000000 pih-1.48023/pih.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 03:17:19.000000 pih-1.48023/pih.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-08-01 03:17:20.000000 pih-1.48023/pih.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-08-01 03:17:20.000000 pih-1.48023/pih.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2009 2023-08-01 00:47:12.000000 pih-1.48023/pih_setup.py
+-rw-rw-rw-   0        0        0       42 2023-08-01 03:17:22.027605 pih-1.48023/setup.cfg
```

### Comparing `pih-1.48022/pih/collection.py` & `pih-1.48023/pih/collection.py`

 * *Files identical despite different names*

### Comparing `pih-1.48022/pih/console_api.py` & `pih-1.48023/pih/console_api.py`

 * *Files identical despite different names*

### Comparing `pih-1.48022/pih/const.py` & `pih-1.48023/pih/const.py`

 * *Files identical despite different names*

### Comparing `pih-1.48022/pih/pih.py` & `pih-1.48023/pih/pih.py`

 * *Files 0% similar despite different names*

```diff
@@ -1637,15 +1637,15 @@
             
             @staticmethod
             def local() -> str:
                 return "1.48020"  
 
         @staticmethod
         def local() -> str:
-            return "1.48022"
+            return "1.48023"
 
         @staticmethod
         def need_update() -> bool:
             return False
             #return importlib.util.find_spec(PIH.NAME) is not None and PIH.VERSION.local() < PIH.VERSION.remote()
     
     class INPUT_WAIT:
@@ -2828,15 +2828,15 @@
 
             @staticmethod
             def get_file_path(name: str) -> str:
                 return PIH.PATH.adapt_if_linux(PATH_STATISTICS.get_file_path(name))
 
         @staticmethod
         def adapt_if_linux(path: str) -> str:
-            if not PIH.OS.is_linux():
+            if PIH.OS.is_linux():
                 path = PIH.PATH.convert_for_unix(path)
                 alias: str = PIH.PATH.convert_for_unix(PATH_FACADE.PATH)
                 if path.find(alias) == 0:
                     path = path[len(alias):]
                     path = PATHS.FACADE.LINUX_MOUNT_POINT_PATH + path
             return path
```

### Comparing `pih-1.48022/pih/rpc.py` & `pih-1.48023/pih/rpc.py`

 * *Files identical despite different names*

### Comparing `pih-1.48022/pih/rpcCommandCall_pb2.py` & `pih-1.48023/pih/rpcCommandCall_pb2.py`

 * *Files identical despite different names*

### Comparing `pih-1.48022/pih/rpcCommandCall_pb2_grpc.py` & `pih-1.48023/pih/rpcCommandCall_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pih-1.48022/pih/rpc_collection.py` & `pih-1.48023/pih/rpc_collection.py`

 * *Files identical despite different names*

### Comparing `pih-1.48022/pih/rpc_const.py` & `pih-1.48023/pih/rpc_const.py`

 * *Files identical despite different names*

### Comparing `pih-1.48022/pih/service_example.py` & `pih-1.48023/pih/service_example.py`

 * *Files identical despite different names*

### Comparing `pih-1.48022/pih/tools.py` & `pih-1.48023/pih/tools.py`

 * *Files identical despite different names*

### Comparing `pih-1.48022/pih/widgets.py` & `pih-1.48023/pih/widgets.py`

 * *Files identical despite different names*

### Comparing `pih-1.48022/pih_setup.py` & `pih-1.48023/pih_setup.py`

 * *Files identical despite different names*

