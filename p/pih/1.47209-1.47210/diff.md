# Comparing `tmp/pih-1.47209.tar.gz` & `tmp/pih-1.47210.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-1.47209.tar", last modified: Tue Aug  1 00:43:39 2023, max compression
+gzip compressed data, was "pih-1.47210.tar", last modified: Tue Aug  1 00:58:24 2023, max compression
```

## Comparing `pih-1.47209.tar` & `pih-1.47210.tar`

### file list

```diff
@@ -1,31 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 00:43:39.335830 pih-1.47209/
-drwxrwxrwx   0        0        0        0 2023-08-01 00:43:26.379178 pih-1.47209/MobileHelperCore/
--rw-rw-rw-   0        0        0        0 2023-03-23 02:22:16.000000 pih-1.47209/MobileHelperCore/__init__.py
--rw-rw-rw-   0        0        0   165320 2023-07-31 03:28:09.000000 pih-1.47209/MobileHelperCore/api.py
--rw-rw-rw-   0        0        0      718 2023-07-28 13:36:37.000000 pih-1.47209/MobileHelperCore/service.py
--rw-rw-rw-   0        0        0     9434 2023-08-01 00:38:40.000000 pih-1.47209/MobileHelperCore/service_api.py
--rw-rw-rw-   0        0        0      986 2023-06-21 05:38:40.000000 pih-1.47209/MobileHelperCore/tools.py
--rw-rw-rw-   0        0        0      261 2023-08-01 00:43:39.288938 pih-1.47209/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-01 00:43:37.169285 pih-1.47209/pih/
--rw-rw-rw-   0        0        0      157 2022-12-03 14:38:35.000000 pih-1.47209/pih/__init__.py
--rw-rw-rw-   0        0        0    20482 2023-07-25 14:36:49.000000 pih-1.47209/pih/collection.py
--rw-rw-rw-   0        0        0    61071 2023-08-01 00:38:40.000000 pih-1.47209/pih/console_api.py
--rw-rw-rw-   0        0        0   111144 2023-08-01 00:39:59.000000 pih-1.47209/pih/const.py
--rw-rw-rw-   0        0        0   317174 2023-08-01 00:40:47.000000 pih-1.47209/pih/pih.py
--rw-rw-rw-   0        0        0    24697 2023-07-28 13:13:08.000000 pih-1.47209/pih/rpc.py
--rw-rw-rw-   0        0        0     1941 2022-07-31 10:55:18.000000 pih-1.47209/pih/rpcCommandCall_pb2.py
--rw-rw-rw-   0        0        0     2465 2022-08-05 02:38:47.000000 pih-1.47209/pih/rpcCommandCall_pb2_grpc.py
--rw-rw-rw-   0        0        0     2576 2023-07-31 23:11:58.000000 pih-1.47209/pih/rpc_collection.py
--rw-rw-rw-   0        0        0     6453 2023-07-24 14:50:22.000000 pih-1.47209/pih/rpc_const.py
--rw-rw-rw-   0        0        0      635 2023-06-11 13:35:46.000000 pih-1.47209/pih/service_example.py
--rw-rw-rw-   0        0        0    38229 2023-07-31 13:41:04.000000 pih-1.47209/pih/tools.py
--rw-rw-rw-   0        0        0     2280 2023-06-30 04:39:52.000000 pih-1.47209/pih/widgets.py
-drwxrwxrwx   0        0        0        0 2023-08-01 00:43:38.897071 pih-1.47209/pih.egg-info/
--rw-rw-rw-   0        0        0      261 2023-08-01 00:43:16.000000 pih-1.47209/pih.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      537 2023-08-01 00:43:23.000000 pih-1.47209/pih.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 00:43:16.000000 pih-1.47209/pih.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-08-01 00:43:16.000000 pih-1.47209/pih.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-08-01 00:43:16.000000 pih-1.47209/pih.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1644 2023-07-28 12:42:15.000000 pih-1.47209/pih_mio_setup.py
--rw-rw-rw-   0        0        0     2009 2023-07-27 14:02:40.000000 pih-1.47209/pih_setup.py
--rw-rw-rw-   0        0        0       42 2023-08-01 00:43:39.367074 pih-1.47209/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-01 00:58:23.785543 pih-1.47210/
+-rw-rw-rw-   0        0        0      261 2023-08-01 00:58:24.818693 pih-1.47210/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-01 00:58:24.584322 pih-1.47210/pih/
+-rw-rw-rw-   0        0        0      157 2022-12-03 14:38:35.000000 pih-1.47210/pih/__init__.py
+-rw-rw-rw-   0        0        0    20482 2023-07-25 14:36:49.000000 pih-1.47210/pih/collection.py
+-rw-rw-rw-   0        0        0    61071 2023-08-01 00:38:40.000000 pih-1.47210/pih/console_api.py
+-rw-rw-rw-   0        0        0   111144 2023-08-01 00:39:59.000000 pih-1.47210/pih/const.py
+-rw-rw-rw-   0        0        0   317176 2023-08-01 00:58:06.000000 pih-1.47210/pih/pih.py
+-rw-rw-rw-   0        0        0    24697 2023-07-28 13:13:08.000000 pih-1.47210/pih/rpc.py
+-rw-rw-rw-   0        0        0     1941 2022-07-31 10:55:18.000000 pih-1.47210/pih/rpcCommandCall_pb2.py
+-rw-rw-rw-   0        0        0     2465 2022-08-05 02:38:47.000000 pih-1.47210/pih/rpcCommandCall_pb2_grpc.py
+-rw-rw-rw-   0        0        0     2576 2023-07-31 23:11:58.000000 pih-1.47210/pih/rpc_collection.py
+-rw-rw-rw-   0        0        0     6453 2023-07-24 14:50:22.000000 pih-1.47210/pih/rpc_const.py
+-rw-rw-rw-   0        0        0      635 2023-06-11 13:35:46.000000 pih-1.47210/pih/service_example.py
+-rw-rw-rw-   0        0        0    38229 2023-07-31 13:41:04.000000 pih-1.47210/pih/tools.py
+-rw-rw-rw-   0        0        0     2280 2023-06-30 04:39:52.000000 pih-1.47210/pih/widgets.py
+drwxrwxrwx   0        0        0        0 2023-08-01 00:58:24.771818 pih-1.47210/pih.egg-info/
+-rw-rw-rw-   0        0        0      261 2023-08-01 00:58:22.000000 pih-1.47210/pih.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2023-08-01 00:58:23.000000 pih-1.47210/pih.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 00:58:23.000000 pih-1.47210/pih.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-08-01 00:58:23.000000 pih-1.47210/pih.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-08-01 00:58:23.000000 pih-1.47210/pih.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2009 2023-08-01 00:47:12.000000 pih-1.47210/pih_setup.py
+-rw-rw-rw-   0        0        0       42 2023-08-01 00:58:24.834324 pih-1.47210/setup.cfg
```

### Comparing `pih-1.47209/pih/collection.py` & `pih-1.47210/pih/collection.py`

 * *Files identical despite different names*

### Comparing `pih-1.47209/pih/console_api.py` & `pih-1.47210/pih/console_api.py`

 * *Files identical despite different names*

### Comparing `pih-1.47209/pih/const.py` & `pih-1.47210/pih/const.py`

 * *Files identical despite different names*

### Comparing `pih-1.47209/pih/pih.py` & `pih-1.47210/pih/pih.py`

 * *Files 0% similar despite different names*

```diff
@@ -1614,14 +1614,15 @@
             session.output = output
             if say_hello and not recipient_as_whatsapp_group:
                 session.say_hello()
             if not recipient_as_whatsapp_group:
                 output.user.get_formatted_given_name = lambda: format_given_name(session, output)
             return output
 
+
         @staticmethod
         def waiting_for_input_from(recipient: str, handler: Callable[[str, Callable[[None], None]], None] | None = None) -> str | None:
             def internal_handler(message: str, close_handler: Callable[[None], None]) -> None:
                 PIH.MIO.ANSWER[recipient].append(message)
                 if DataTool.is_empty(handler):
                     close_handler()
                 else:
@@ -1636,15 +1637,15 @@
             
             @staticmethod
             def local() -> str:
                 return "1.48016"  
 
         @staticmethod
         def local() -> str:
-            return "1.47209"
+            return "1.47210"
 
         @staticmethod
         def need_update() -> bool:
             return False
             #return importlib.util.find_spec(PIH.NAME) is not None and PIH.VERSION.local() < PIH.VERSION.remote()
     
     class INPUT_WAIT:
```

### Comparing `pih-1.47209/pih/rpc.py` & `pih-1.47210/pih/rpc.py`

 * *Files identical despite different names*

### Comparing `pih-1.47209/pih/rpcCommandCall_pb2.py` & `pih-1.47210/pih/rpcCommandCall_pb2.py`

 * *Files identical despite different names*

### Comparing `pih-1.47209/pih/rpcCommandCall_pb2_grpc.py` & `pih-1.47210/pih/rpcCommandCall_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pih-1.47209/pih/rpc_collection.py` & `pih-1.47210/pih/rpc_collection.py`

 * *Files identical despite different names*

### Comparing `pih-1.47209/pih/rpc_const.py` & `pih-1.47210/pih/rpc_const.py`

 * *Files identical despite different names*

### Comparing `pih-1.47209/pih/service_example.py` & `pih-1.47210/pih/service_example.py`

 * *Files identical despite different names*

### Comparing `pih-1.47209/pih/tools.py` & `pih-1.47210/pih/tools.py`

 * *Files identical despite different names*

### Comparing `pih-1.47209/pih/widgets.py` & `pih-1.47210/pih/widgets.py`

 * *Files identical despite different names*

### Comparing `pih-1.47209/pih_setup.py` & `pih-1.47210/pih_setup.py`

 * *Files identical despite different names*

