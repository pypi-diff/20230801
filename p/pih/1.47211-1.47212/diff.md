# Comparing `tmp/pih-1.47211.tar.gz` & `tmp/pih-1.47212.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-1.47211.tar", last modified: Tue Aug  1 00:59:46 2023, max compression
+gzip compressed data, was "pih-1.47212.tar", last modified: Tue Aug  1 02:05:57 2023, max compression
```

## Comparing `pih-1.47211.tar` & `pih-1.47212.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 00:59:46.324914 pih-1.47211/
--rw-rw-rw-   0        0        0      261 2023-08-01 00:59:46.340539 pih-1.47211/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-01 00:59:46.059295 pih-1.47211/pih/
--rw-rw-rw-   0        0        0      157 2022-12-03 14:38:35.000000 pih-1.47211/pih/__init__.py
--rw-rw-rw-   0        0        0    20482 2023-07-25 14:36:49.000000 pih-1.47211/pih/collection.py
--rw-rw-rw-   0        0        0    61071 2023-08-01 00:38:40.000000 pih-1.47211/pih/console_api.py
--rw-rw-rw-   0        0        0   111144 2023-08-01 00:39:59.000000 pih-1.47211/pih/const.py
--rw-rw-rw-   0        0        0   317176 2023-08-01 00:59:39.000000 pih-1.47211/pih/pih.py
--rw-rw-rw-   0        0        0    24697 2023-07-28 13:13:08.000000 pih-1.47211/pih/rpc.py
--rw-rw-rw-   0        0        0     1941 2022-07-31 10:55:18.000000 pih-1.47211/pih/rpcCommandCall_pb2.py
--rw-rw-rw-   0        0        0     2465 2022-08-05 02:38:47.000000 pih-1.47211/pih/rpcCommandCall_pb2_grpc.py
--rw-rw-rw-   0        0        0     2576 2023-07-31 23:11:58.000000 pih-1.47211/pih/rpc_collection.py
--rw-rw-rw-   0        0        0     6453 2023-07-24 14:50:22.000000 pih-1.47211/pih/rpc_const.py
--rw-rw-rw-   0        0        0      635 2023-06-11 13:35:46.000000 pih-1.47211/pih/service_example.py
--rw-rw-rw-   0        0        0    38229 2023-07-31 13:41:04.000000 pih-1.47211/pih/tools.py
--rw-rw-rw-   0        0        0     2280 2023-06-30 04:39:52.000000 pih-1.47211/pih/widgets.py
-drwxrwxrwx   0        0        0        0 2023-08-01 00:59:46.309291 pih-1.47211/pih.egg-info/
--rw-rw-rw-   0        0        0      261 2023-08-01 00:59:44.000000 pih-1.47211/pih.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      381 2023-08-01 00:59:45.000000 pih-1.47211/pih.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 00:59:44.000000 pih-1.47211/pih.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-08-01 00:59:44.000000 pih-1.47211/pih.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-08-01 00:59:44.000000 pih-1.47211/pih.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2009 2023-08-01 00:47:12.000000 pih-1.47211/pih_setup.py
--rw-rw-rw-   0        0        0       42 2023-08-01 00:59:46.356166 pih-1.47211/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-01 02:05:55.862630 pih-1.47212/
+-rw-rw-rw-   0        0        0      261 2023-08-01 02:05:57.189502 pih-1.47212/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-01 02:05:56.892659 pih-1.47212/pih/
+-rw-rw-rw-   0        0        0      157 2022-12-03 14:38:35.000000 pih-1.47212/pih/__init__.py
+-rw-rw-rw-   0        0        0    20482 2023-07-25 14:36:49.000000 pih-1.47212/pih/collection.py
+-rw-rw-rw-   0        0        0    61071 2023-08-01 00:38:40.000000 pih-1.47212/pih/console_api.py
+-rw-rw-rw-   0        0        0   111144 2023-08-01 00:39:59.000000 pih-1.47212/pih/const.py
+-rw-rw-rw-   0        0        0   317185 2023-08-01 02:05:49.000000 pih-1.47212/pih/pih.py
+-rw-rw-rw-   0        0        0    24697 2023-07-28 13:13:08.000000 pih-1.47212/pih/rpc.py
+-rw-rw-rw-   0        0        0     1941 2022-07-31 10:55:18.000000 pih-1.47212/pih/rpcCommandCall_pb2.py
+-rw-rw-rw-   0        0        0     2465 2022-08-05 02:38:47.000000 pih-1.47212/pih/rpcCommandCall_pb2_grpc.py
+-rw-rw-rw-   0        0        0     2576 2023-07-31 23:11:58.000000 pih-1.47212/pih/rpc_collection.py
+-rw-rw-rw-   0        0        0     6453 2023-07-24 14:50:22.000000 pih-1.47212/pih/rpc_const.py
+-rw-rw-rw-   0        0        0      635 2023-06-11 13:35:46.000000 pih-1.47212/pih/service_example.py
+-rw-rw-rw-   0        0        0    38229 2023-07-31 13:41:04.000000 pih-1.47212/pih/tools.py
+-rw-rw-rw-   0        0        0     2280 2023-06-30 04:39:52.000000 pih-1.47212/pih/widgets.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:05:57.142625 pih-1.47212/pih.egg-info/
+-rw-rw-rw-   0        0        0      261 2023-08-01 02:05:54.000000 pih-1.47212/pih.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2023-08-01 02:05:55.000000 pih-1.47212/pih.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 02:05:55.000000 pih-1.47212/pih.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-08-01 02:05:55.000000 pih-1.47212/pih.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-08-01 02:05:55.000000 pih-1.47212/pih.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2009 2023-08-01 00:47:12.000000 pih-1.47212/pih_setup.py
+-rw-rw-rw-   0        0        0       42 2023-08-01 02:05:57.205181 pih-1.47212/setup.cfg
```

### Comparing `pih-1.47211/pih/collection.py` & `pih-1.47212/pih/collection.py`

 * *Files identical despite different names*

### Comparing `pih-1.47211/pih/console_api.py` & `pih-1.47212/pih/console_api.py`

 * *Files identical despite different names*

### Comparing `pih-1.47211/pih/const.py` & `pih-1.47212/pih/const.py`

 * *Files identical despite different names*

### Comparing `pih-1.47211/pih/pih.py` & `pih-1.47212/pih/pih.py`

 * *Files 0% similar despite different names*

```diff
@@ -1637,15 +1637,15 @@
             
             @staticmethod
             def local() -> str:
                 return "1.48016"  
 
         @staticmethod
         def local() -> str:
-            return "1.47211"
+            return "1.47212"
 
         @staticmethod
         def need_update() -> bool:
             return False
             #return importlib.util.find_spec(PIH.NAME) is not None and PIH.VERSION.local() < PIH.VERSION.remote()
     
     class INPUT_WAIT:
@@ -2653,15 +2653,15 @@
                       starts_handler: Callable[[IService | None], None] | None = None, 
                       max_workers: int | None = None, 
                       stop_before: bool = True, 
                       depends_on_list: list[ServiceDescription | ServiceRoles] | None = None, 
                       isolate: bool = False,
                       show_output: bool = True) -> None:
                 host: str = PIH.OS.host()
-                service_description: ServiceInformationBase = ServiceDescription.description(role_or_information)
+                service_description: ServiceInformationBase = ServiceRoles.description(role_or_information)
                 if isolate:
                      PIH.SERVICE.ADMIN.isolate(service_description)
                 else:
                     if not PIH.DATA.contains(host, service_description.host):
                         if service_description.host_changeable:
                             PIH.SERVICE.ADMIN.change_host_on_local(service_description)
                         else:
@@ -2851,15 +2851,15 @@
             
         @staticmethod
         def mount_facade_storage_on_linux_host(linux_host: str | None = None) -> bool:
             if PIH.OS.is_linux():
                 commnad: str = PIH.PATH.get_command_for_mount_facade_storage_on_linux_host()
                 if_else(DataTool.is_none(linux_host),
                         lambda: PIH.PSTOOLS.execute_command_list(commnad, True, as_shell=True),
-                    lambda: PIH.RESULT.SSH.execute(commnad, linux_host)
+                    lambda: PIH.RESULT.SSH.execute(commnad, linux_host, use_sudo=True)
                 )
                 return True
             return False
                  
         @staticmethod
         def make_directory_if_not_exists(path: str, host: str | None = None) -> bool:
             command: str = f"mkdir {path}"
```

### Comparing `pih-1.47211/pih/rpc.py` & `pih-1.47212/pih/rpc.py`

 * *Files identical despite different names*

### Comparing `pih-1.47211/pih/rpcCommandCall_pb2.py` & `pih-1.47212/pih/rpcCommandCall_pb2.py`

 * *Files identical despite different names*

### Comparing `pih-1.47211/pih/rpcCommandCall_pb2_grpc.py` & `pih-1.47212/pih/rpcCommandCall_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pih-1.47211/pih/rpc_collection.py` & `pih-1.47212/pih/rpc_collection.py`

 * *Files identical despite different names*

### Comparing `pih-1.47211/pih/rpc_const.py` & `pih-1.47212/pih/rpc_const.py`

 * *Files identical despite different names*

### Comparing `pih-1.47211/pih/service_example.py` & `pih-1.47212/pih/service_example.py`

 * *Files identical despite different names*

### Comparing `pih-1.47211/pih/tools.py` & `pih-1.47212/pih/tools.py`

 * *Files identical despite different names*

### Comparing `pih-1.47211/pih/widgets.py` & `pih-1.47212/pih/widgets.py`

 * *Files identical despite different names*

### Comparing `pih-1.47211/pih_setup.py` & `pih-1.47212/pih_setup.py`

 * *Files identical despite different names*

