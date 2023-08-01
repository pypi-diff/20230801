# Comparing `tmp/pih-1.47207.tar.gz` & `tmp/pih-1.47208.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-1.47207.tar", last modified: Mon Jul 31 23:48:38 2023, max compression
+gzip compressed data, was "pih-1.47208.tar", last modified: Tue Aug  1 00:20:19 2023, max compression
```

## Comparing `pih-1.47207.tar` & `pih-1.47208.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 23:48:37.270377 pih-1.47207/
-drwxrwxrwx   0        0        0        0 2023-07-31 23:48:37.521471 pih-1.47207/MobileHelperCore/
--rw-rw-rw-   0        0        0        0 2023-03-23 02:22:16.000000 pih-1.47207/MobileHelperCore/__init__.py
--rw-rw-rw-   0        0        0   165320 2023-07-31 03:28:09.000000 pih-1.47207/MobileHelperCore/api.py
--rw-rw-rw-   0        0        0      718 2023-07-28 13:36:37.000000 pih-1.47207/MobileHelperCore/service.py
--rw-rw-rw-   0        0        0     9431 2023-07-28 13:39:51.000000 pih-1.47207/MobileHelperCore/service_api.py
--rw-rw-rw-   0        0        0      986 2023-06-21 05:38:40.000000 pih-1.47207/MobileHelperCore/tools.py
--rw-rw-rw-   0        0        0      261 2023-07-31 23:48:38.591880 pih-1.47207/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-31 23:48:38.326259 pih-1.47207/pih/
--rw-rw-rw-   0        0        0      157 2022-12-03 14:38:35.000000 pih-1.47207/pih/__init__.py
--rw-rw-rw-   0        0        0    20482 2023-07-25 14:36:49.000000 pih-1.47207/pih/collection.py
--rw-rw-rw-   0        0        0    61070 2023-07-31 13:45:05.000000 pih-1.47207/pih/console_api.py
--rw-rw-rw-   0        0        0   111143 2023-07-31 23:11:49.000000 pih-1.47207/pih/const.py
--rw-rw-rw-   0        0        0   316482 2023-07-31 23:48:13.000000 pih-1.47207/pih/pih.py
--rw-rw-rw-   0        0        0    24697 2023-07-28 13:13:08.000000 pih-1.47207/pih/rpc.py
--rw-rw-rw-   0        0        0     1941 2022-07-31 10:55:18.000000 pih-1.47207/pih/rpcCommandCall_pb2.py
--rw-rw-rw-   0        0        0     2465 2022-08-05 02:38:47.000000 pih-1.47207/pih/rpcCommandCall_pb2_grpc.py
--rw-rw-rw-   0        0        0     2576 2023-07-31 23:11:58.000000 pih-1.47207/pih/rpc_collection.py
--rw-rw-rw-   0        0        0     6453 2023-07-24 14:50:22.000000 pih-1.47207/pih/rpc_const.py
--rw-rw-rw-   0        0        0      635 2023-06-11 13:35:46.000000 pih-1.47207/pih/service_example.py
--rw-rw-rw-   0        0        0    38229 2023-07-31 13:41:04.000000 pih-1.47207/pih/tools.py
--rw-rw-rw-   0        0        0     2280 2023-06-30 04:39:52.000000 pih-1.47207/pih/widgets.py
-drwxrwxrwx   0        0        0        0 2023-07-31 23:48:38.560630 pih-1.47207/pih.egg-info/
--rw-rw-rw-   0        0        0      261 2023-07-31 23:48:36.000000 pih-1.47207/pih.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      537 2023-07-31 23:48:36.000000 pih-1.47207/pih.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 23:48:36.000000 pih-1.47207/pih.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-07-31 23:48:36.000000 pih-1.47207/pih.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-31 23:48:36.000000 pih-1.47207/pih.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1644 2023-07-28 12:42:15.000000 pih-1.47207/pih_mio_setup.py
--rw-rw-rw-   0        0        0     2009 2023-07-27 14:02:40.000000 pih-1.47207/pih_setup.py
--rw-rw-rw-   0        0        0       42 2023-07-31 23:48:38.607504 pih-1.47207/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-01 00:20:18.027718 pih-1.47208/
+drwxrwxrwx   0        0        0        0 2023-08-01 00:20:18.308965 pih-1.47208/MobileHelperCore/
+-rw-rw-rw-   0        0        0        0 2023-03-23 02:22:16.000000 pih-1.47208/MobileHelperCore/__init__.py
+-rw-rw-rw-   0        0        0   165320 2023-07-31 03:28:09.000000 pih-1.47208/MobileHelperCore/api.py
+-rw-rw-rw-   0        0        0      718 2023-07-28 13:36:37.000000 pih-1.47208/MobileHelperCore/service.py
+-rw-rw-rw-   0        0        0     9431 2023-07-28 13:39:51.000000 pih-1.47208/MobileHelperCore/service_api.py
+-rw-rw-rw-   0        0        0      986 2023-06-21 05:38:40.000000 pih-1.47208/MobileHelperCore/tools.py
+-rw-rw-rw-   0        0        0      261 2023-08-01 00:20:19.418329 pih-1.47208/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-01 00:20:19.168326 pih-1.47208/pih/
+-rw-rw-rw-   0        0        0      157 2022-12-03 14:38:35.000000 pih-1.47208/pih/__init__.py
+-rw-rw-rw-   0        0        0    20482 2023-07-25 14:36:49.000000 pih-1.47208/pih/collection.py
+-rw-rw-rw-   0        0        0    61070 2023-08-01 00:19:29.000000 pih-1.47208/pih/console_api.py
+-rw-rw-rw-   0        0        0   111143 2023-07-31 23:11:49.000000 pih-1.47208/pih/const.py
+-rw-rw-rw-   0        0        0   316737 2023-08-01 00:20:11.000000 pih-1.47208/pih/pih.py
+-rw-rw-rw-   0        0        0    24697 2023-07-28 13:13:08.000000 pih-1.47208/pih/rpc.py
+-rw-rw-rw-   0        0        0     1941 2022-07-31 10:55:18.000000 pih-1.47208/pih/rpcCommandCall_pb2.py
+-rw-rw-rw-   0        0        0     2465 2022-08-05 02:38:47.000000 pih-1.47208/pih/rpcCommandCall_pb2_grpc.py
+-rw-rw-rw-   0        0        0     2576 2023-07-31 23:11:58.000000 pih-1.47208/pih/rpc_collection.py
+-rw-rw-rw-   0        0        0     6453 2023-07-24 14:50:22.000000 pih-1.47208/pih/rpc_const.py
+-rw-rw-rw-   0        0        0      635 2023-06-11 13:35:46.000000 pih-1.47208/pih/service_example.py
+-rw-rw-rw-   0        0        0    38229 2023-07-31 13:41:04.000000 pih-1.47208/pih/tools.py
+-rw-rw-rw-   0        0        0     2280 2023-06-30 04:39:52.000000 pih-1.47208/pih/widgets.py
+drwxrwxrwx   0        0        0        0 2023-08-01 00:20:19.371450 pih-1.47208/pih.egg-info/
+-rw-rw-rw-   0        0        0      261 2023-08-01 00:20:16.000000 pih-1.47208/pih.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      537 2023-08-01 00:20:17.000000 pih-1.47208/pih.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 00:20:17.000000 pih-1.47208/pih.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-08-01 00:20:17.000000 pih-1.47208/pih.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-08-01 00:20:17.000000 pih-1.47208/pih.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1644 2023-07-28 12:42:15.000000 pih-1.47208/pih_mio_setup.py
+-rw-rw-rw-   0        0        0     2009 2023-07-27 14:02:40.000000 pih-1.47208/pih_setup.py
+-rw-rw-rw-   0        0        0       42 2023-08-01 00:20:19.465197 pih-1.47208/setup.cfg
```

### Comparing `pih-1.47207/MobileHelperCore/api.py` & `pih-1.47208/MobileHelperCore/api.py`

 * *Files identical despite different names*

### Comparing `pih-1.47207/MobileHelperCore/service.py` & `pih-1.47208/MobileHelperCore/service.py`

 * *Files identical despite different names*

### Comparing `pih-1.47207/MobileHelperCore/service_api.py` & `pih-1.47208/MobileHelperCore/service_api.py`

 * *Files identical despite different names*

### Comparing `pih-1.47207/MobileHelperCore/tools.py` & `pih-1.47208/MobileHelperCore/tools.py`

 * *Files identical despite different names*

### Comparing `pih-1.47207/pih/collection.py` & `pih-1.47208/pih/collection.py`

 * *Files identical despite different names*

### Comparing `pih-1.47207/pih/console_api.py` & `pih-1.47208/pih/console_api.py`

 * *Files identical despite different names*

### Comparing `pih-1.47207/pih/const.py` & `pih-1.47208/pih/const.py`

 * *Files identical despite different names*

### Comparing `pih-1.47207/pih/pih.py` & `pih-1.47208/pih/pih.py`

 * *Files 0% similar despite different names*

```diff
@@ -1636,15 +1636,15 @@
             
             @staticmethod
             def local() -> str:
                 return "1.48016"  
 
         @staticmethod
         def local() -> str:
-            return "1.47207"
+            return "1.47208"
 
         @staticmethod
         def need_update() -> bool:
             return False
             #return importlib.util.find_spec(PIH.NAME) is not None and PIH.VERSION.local() < PIH.VERSION.remote()
     
     class INPUT_WAIT:
@@ -2651,30 +2651,31 @@
                       call_handler: Callable[[ServiceCommands, ParameterList], Any] | None = None, 
                       starts_handler: Callable[[IService | None], None] | None = None, 
                       max_workers: int | None = None, 
                       stop_before: bool = True, 
                       depends_on_list: list[ServiceDescription | ServiceRoles] | None = None, 
                       isolate: bool = False,
                       show_output: bool = True) -> None:
+                host: str = A.OS.host()
                 service_description: ServiceInformationBase = A.CT_SR.description(role_or_information)
                 if isolate:
                      PIH.SERVICE.ADMIN.isolate(service_description)
                 else:
-                    if not A.D.contains(A.OS.host(), service_description.host):
+                    if not A.D.contains(host, service_description.host):
                         if service_description.host_changeable:
                             PIH.SERVICE.ADMIN.change_host_on_local(service_description)
                         else:
                             pass
                     if stop_before:
                         if PIH.SERVICE.check_accessibility(service_description):
                             PIH.SERVICE.ADMIN.stop(service_description)
                 def internal_start_handler(service: IService) -> None:
                     if PIH.OS.is_linux():
-                        PIH.PATH.make_directory_if_not_exists(PATHS.FACADE.LINUX_MOUNT_POINT_PATH)
-                        PIH.PATH.mount_facade_storage_on_linux_host()
+                        PIH.PATH.make_directory_if_not_exists(PATHS.FACADE.LINUX_MOUNT_POINT_PATH, host)
+                        PIH.PATH.mount_facade_storage_on_linux_host(host)
                     if starts_handler is not None:
                         if starts_handler.__code__.co_argcount == 1:
                             starts_handler(service)
                         else:
                             starts_handler()
                 service: IService = RPC.create_service()
                 from inspect import signature, Signature
@@ -2856,17 +2857,19 @@
                     lambda: PIH.RESULT.SSH.execute(commnad, linux_host)
                 )
                 return True
             return False
                  
         @staticmethod
         def make_directory_if_not_exists(path: str, host: str | None = None) -> bool:
+            command: str = f"mkdir {path}"
             if DataTool.is_none(host):
                 return PathTool.make_directory_if_not_exists(path)
-            PIH.RESULT.SSH.execute(f"mkdir {path}", host, use_sudo=True)
+            else:
+                PIH.RESULT.SSH.execute(command, host, use_sudo=True)
             return True
 
         @staticmethod
         def get_command_for_mount_facade_storage_on_linux_host() -> str:
             return PIH.PATH.get_command_for_mount_storage_on_linux_host(PATHS.FACADE.STORAGE_PATH(), 
                                                                         PATHS.FACADE.LINUX_MOUNT_POINT_PATH, 
                                                                         PIH.DATA.get_variable_value(HOSTS.SERVICES.PASSWORD_ALIAS), 
@@ -2915,14 +2918,18 @@
             def mobile_helper_command(name: str) -> str:
                 name = PIH.DATA.FORMAT.mobile_helper_command(name)
                 return os.path.join(PATHS.MOBILE_HELPER.QR_CODE_FOLDER, PathTool.replace_prohibited_symbols_from_path_with_symbol(PathTool.add_extension(name, FILE.EXTENSION.PNG)))
 
     class DATA(DataTool, StringTool, ListTool, DateTimeTool, EnumTool, FullNameTool):
 
         @staticmethod
+        def make_sudo(command: str, password: str) -> str:
+            return f"echo -e '{password}\n' | sudo -S " + command
+
+        @staticmethod
         def translit(value, language_code=None, reversed=False, strict=False):
             return translit(value, language_code, reversed, strict)
 
         @staticmethod
         def find_variables(name: str | None) -> list[StorageValue]:
             return PIH.DATA.MATERIALIZED_RESOURCES.find(name) + PIH.SETTINGS.find(name)
```

### Comparing `pih-1.47207/pih/rpc.py` & `pih-1.47208/pih/rpc.py`

 * *Files identical despite different names*

### Comparing `pih-1.47207/pih/rpcCommandCall_pb2.py` & `pih-1.47208/pih/rpcCommandCall_pb2.py`

 * *Files identical despite different names*

### Comparing `pih-1.47207/pih/rpcCommandCall_pb2_grpc.py` & `pih-1.47208/pih/rpcCommandCall_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pih-1.47207/pih/rpc_collection.py` & `pih-1.47208/pih/rpc_collection.py`

 * *Files identical despite different names*

### Comparing `pih-1.47207/pih/rpc_const.py` & `pih-1.47208/pih/rpc_const.py`

 * *Files identical despite different names*

### Comparing `pih-1.47207/pih/service_example.py` & `pih-1.47208/pih/service_example.py`

 * *Files identical despite different names*

### Comparing `pih-1.47207/pih/tools.py` & `pih-1.47208/pih/tools.py`

 * *Files identical despite different names*

### Comparing `pih-1.47207/pih/widgets.py` & `pih-1.47208/pih/widgets.py`

 * *Files identical despite different names*

### Comparing `pih-1.47207/pih.egg-info/SOURCES.txt` & `pih-1.47208/pih.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pih-1.47207/pih_mio_setup.py` & `pih-1.47208/pih_mio_setup.py`

 * *Files identical despite different names*

### Comparing `pih-1.47207/pih_setup.py` & `pih-1.47208/pih_setup.py`

 * *Files identical despite different names*

