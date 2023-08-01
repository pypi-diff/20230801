# Comparing `tmp/pih-1.47214.tar.gz` & `tmp/pih-1.47215.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-1.47214.tar", last modified: Tue Aug  1 02:23:13 2023, max compression
+gzip compressed data, was "pih-1.47215.tar", last modified: Tue Aug  1 02:33:28 2023, max compression
```

## Comparing `pih-1.47214.tar` & `pih-1.47215.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 02:23:12.616200 pih-1.47214/
--rw-rw-rw-   0        0        0      261 2023-08-01 02:23:13.569297 pih-1.47214/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-01 02:23:13.366178 pih-1.47214/pih/
--rw-rw-rw-   0        0        0      157 2022-12-03 14:38:35.000000 pih-1.47214/pih/__init__.py
--rw-rw-rw-   0        0        0    20482 2023-07-25 14:36:49.000000 pih-1.47214/pih/collection.py
--rw-rw-rw-   0        0        0    61053 2023-08-01 02:15:39.000000 pih-1.47214/pih/console_api.py
--rw-rw-rw-   0        0        0   111144 2023-08-01 00:39:59.000000 pih-1.47214/pih/const.py
--rw-rw-rw-   0        0        0   317186 2023-08-01 02:23:06.000000 pih-1.47214/pih/pih.py
--rw-rw-rw-   0        0        0    24697 2023-07-28 13:13:08.000000 pih-1.47214/pih/rpc.py
--rw-rw-rw-   0        0        0     1941 2022-07-31 10:55:18.000000 pih-1.47214/pih/rpcCommandCall_pb2.py
--rw-rw-rw-   0        0        0     2465 2022-08-05 02:38:47.000000 pih-1.47214/pih/rpcCommandCall_pb2_grpc.py
--rw-rw-rw-   0        0        0     2576 2023-07-31 23:11:58.000000 pih-1.47214/pih/rpc_collection.py
--rw-rw-rw-   0        0        0     6453 2023-07-24 14:50:22.000000 pih-1.47214/pih/rpc_const.py
--rw-rw-rw-   0        0        0      635 2023-06-11 13:35:46.000000 pih-1.47214/pih/service_example.py
--rw-rw-rw-   0        0        0    38229 2023-07-31 13:41:04.000000 pih-1.47214/pih/tools.py
--rw-rw-rw-   0        0        0     2280 2023-06-30 04:39:52.000000 pih-1.47214/pih/widgets.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:23:13.538052 pih-1.47214/pih.egg-info/
--rw-rw-rw-   0        0        0      261 2023-08-01 02:23:11.000000 pih-1.47214/pih.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      381 2023-08-01 02:23:12.000000 pih-1.47214/pih.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 02:23:11.000000 pih-1.47214/pih.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-08-01 02:23:12.000000 pih-1.47214/pih.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-08-01 02:23:12.000000 pih-1.47214/pih.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2009 2023-08-01 00:47:12.000000 pih-1.47214/pih_setup.py
--rw-rw-rw-   0        0        0       42 2023-08-01 02:23:13.569297 pih-1.47214/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-01 02:33:28.806602 pih-1.47215/
+-rw-rw-rw-   0        0        0      261 2023-08-01 02:33:28.790958 pih-1.47215/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-01 02:33:28.572224 pih-1.47215/pih/
+-rw-rw-rw-   0        0        0      157 2022-12-03 14:38:35.000000 pih-1.47215/pih/__init__.py
+-rw-rw-rw-   0        0        0    20482 2023-07-25 14:36:49.000000 pih-1.47215/pih/collection.py
+-rw-rw-rw-   0        0        0    61053 2023-08-01 02:15:39.000000 pih-1.47215/pih/console_api.py
+-rw-rw-rw-   0        0        0   111144 2023-08-01 00:39:59.000000 pih-1.47215/pih/const.py
+-rw-rw-rw-   0        0        0   317177 2023-08-01 02:33:19.000000 pih-1.47215/pih/pih.py
+-rw-rw-rw-   0        0        0    24697 2023-07-28 13:13:08.000000 pih-1.47215/pih/rpc.py
+-rw-rw-rw-   0        0        0     1941 2022-07-31 10:55:18.000000 pih-1.47215/pih/rpcCommandCall_pb2.py
+-rw-rw-rw-   0        0        0     2465 2022-08-05 02:38:47.000000 pih-1.47215/pih/rpcCommandCall_pb2_grpc.py
+-rw-rw-rw-   0        0        0     2576 2023-07-31 23:11:58.000000 pih-1.47215/pih/rpc_collection.py
+-rw-rw-rw-   0        0        0     6453 2023-07-24 14:50:22.000000 pih-1.47215/pih/rpc_const.py
+-rw-rw-rw-   0        0        0      635 2023-06-11 13:35:46.000000 pih-1.47215/pih/service_example.py
+-rw-rw-rw-   0        0        0    38229 2023-07-31 13:41:04.000000 pih-1.47215/pih/tools.py
+-rw-rw-rw-   0        0        0     2280 2023-06-30 04:39:52.000000 pih-1.47215/pih/widgets.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:33:28.728536 pih-1.47215/pih.egg-info/
+-rw-rw-rw-   0        0        0      261 2023-08-01 02:33:25.000000 pih-1.47215/pih.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2023-08-01 02:33:26.000000 pih-1.47215/pih.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 02:33:25.000000 pih-1.47215/pih.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-08-01 02:33:25.000000 pih-1.47215/pih.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-08-01 02:33:25.000000 pih-1.47215/pih.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2009 2023-08-01 00:47:12.000000 pih-1.47215/pih_setup.py
+-rw-rw-rw-   0        0        0       42 2023-08-01 02:33:28.806602 pih-1.47215/setup.cfg
```

### Comparing `pih-1.47214/pih/collection.py` & `pih-1.47215/pih/collection.py`

 * *Files identical despite different names*

### Comparing `pih-1.47214/pih/console_api.py` & `pih-1.47215/pih/console_api.py`

 * *Files identical despite different names*

### Comparing `pih-1.47214/pih/const.py` & `pih-1.47215/pih/const.py`

 * *Files identical despite different names*

### Comparing `pih-1.47214/pih/pih.py` & `pih-1.47215/pih/pih.py`

 * *Files 0% similar despite different names*

```diff
@@ -1637,15 +1637,15 @@
             
             @staticmethod
             def local() -> str:
                 return "1.48016"  
 
         @staticmethod
         def local() -> str:
-            return "1.47214"
+            return "1.47215"
 
         @staticmethod
         def need_update() -> bool:
             return False
             #return importlib.util.find_spec(PIH.NAME) is not None and PIH.VERSION.local() < PIH.VERSION.remote()
     
     class INPUT_WAIT:
@@ -2828,20 +2828,20 @@
 
             @staticmethod
             def get_file_path(name: str) -> str:
                 return PIH.PATH.adapt_if_linux(PATH_STATISTICS.get_file_path(name))
 
         @staticmethod
         def adapt_if_linux(path: str) -> str:
-            if PIH.OS.is_linux():
+            if not PIH.OS.is_linux():
                 path = PIH.PATH.convert_for_unix(path)
                 alias: str = PIH.PATH.convert_for_unix(PATH_FACADE.PATH)
                 if path.find(alias) == 0:
                     path = path[len(alias):]
-                    path = os.path.join(PATHS.FACADE.LINUX_MOUNT_POINT_PATH, path)
+                    path = PATHS.FACADE.LINUX_MOUNT_POINT_PATH + path
             return path
 
         @staticmethod
         def get_command_for_mount_storage_on_linux_host(storage_path: str, linux_mount_point: str, linux_host_user_password: str, storage_host_user_login: str, storage_host_user_password: str) -> str:
             return f"mount -t cifs {PIH.PATH.convert_for_unix(storage_path)} {linux_mount_point} -o username={storage_host_user_login},password={storage_host_user_password}"
 
         @staticmethod
```

### Comparing `pih-1.47214/pih/rpc.py` & `pih-1.47215/pih/rpc.py`

 * *Files identical despite different names*

### Comparing `pih-1.47214/pih/rpcCommandCall_pb2.py` & `pih-1.47215/pih/rpcCommandCall_pb2.py`

 * *Files identical despite different names*

### Comparing `pih-1.47214/pih/rpcCommandCall_pb2_grpc.py` & `pih-1.47215/pih/rpcCommandCall_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pih-1.47214/pih/rpc_collection.py` & `pih-1.47215/pih/rpc_collection.py`

 * *Files identical despite different names*

### Comparing `pih-1.47214/pih/rpc_const.py` & `pih-1.47215/pih/rpc_const.py`

 * *Files identical despite different names*

### Comparing `pih-1.47214/pih/service_example.py` & `pih-1.47215/pih/service_example.py`

 * *Files identical despite different names*

### Comparing `pih-1.47214/pih/tools.py` & `pih-1.47215/pih/tools.py`

 * *Files identical despite different names*

### Comparing `pih-1.47214/pih/widgets.py` & `pih-1.47215/pih/widgets.py`

 * *Files identical despite different names*

### Comparing `pih-1.47214/pih_setup.py` & `pih-1.47215/pih_setup.py`

 * *Files identical despite different names*

