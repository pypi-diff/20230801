# Comparing `tmp/pih-1.48024.tar.gz` & `tmp/pih-1.48026.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-1.48024.tar", last modified: Tue Aug  1 03:21:13 2023, max compression
+gzip compressed data, was "pih-1.48026.tar", last modified: Tue Aug  1 04:09:28 2023, max compression
```

## Comparing `pih-1.48024.tar` & `pih-1.48026.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 03:21:14.037731 pih-1.48024/
--rw-rw-rw-   0        0        0      261 2023-08-01 03:21:14.037731 pih-1.48024/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-01 03:21:13.662732 pih-1.48024/pih/
--rw-rw-rw-   0        0        0      157 2022-12-03 14:38:35.000000 pih-1.48024/pih/__init__.py
--rw-rw-rw-   0        0        0    20482 2023-07-25 14:36:49.000000 pih-1.48024/pih/collection.py
--rw-rw-rw-   0        0        0    60803 2023-08-01 03:20:53.000000 pih-1.48024/pih/console_api.py
--rw-rw-rw-   0        0        0   111144 2023-08-01 00:39:59.000000 pih-1.48024/pih/const.py
--rw-rw-rw-   0        0        0   317173 2023-08-01 03:21:04.000000 pih-1.48024/pih/pih.py
--rw-rw-rw-   0        0        0    24697 2023-07-28 13:13:08.000000 pih-1.48024/pih/rpc.py
--rw-rw-rw-   0        0        0     1941 2022-07-31 10:55:18.000000 pih-1.48024/pih/rpcCommandCall_pb2.py
--rw-rw-rw-   0        0        0     2465 2022-08-05 02:38:47.000000 pih-1.48024/pih/rpcCommandCall_pb2_grpc.py
--rw-rw-rw-   0        0        0     2576 2023-07-31 23:11:58.000000 pih-1.48024/pih/rpc_collection.py
--rw-rw-rw-   0        0        0     6453 2023-07-24 14:50:22.000000 pih-1.48024/pih/rpc_const.py
--rw-rw-rw-   0        0        0      635 2023-06-11 13:35:46.000000 pih-1.48024/pih/service_example.py
--rw-rw-rw-   0        0        0    38229 2023-08-01 02:41:41.000000 pih-1.48024/pih/tools.py
--rw-rw-rw-   0        0        0     2280 2023-06-30 04:39:52.000000 pih-1.48024/pih/widgets.py
-drwxrwxrwx   0        0        0        0 2023-08-01 03:21:13.990851 pih-1.48024/pih.egg-info/
--rw-rw-rw-   0        0        0      261 2023-08-01 03:21:11.000000 pih-1.48024/pih.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      381 2023-08-01 03:21:12.000000 pih-1.48024/pih.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 03:21:11.000000 pih-1.48024/pih.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-08-01 03:21:12.000000 pih-1.48024/pih.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-08-01 03:21:12.000000 pih-1.48024/pih.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2009 2023-08-01 00:47:12.000000 pih-1.48024/pih_setup.py
--rw-rw-rw-   0        0        0       42 2023-08-01 03:21:14.053351 pih-1.48024/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-01 04:09:28.102432 pih-1.48026/
+-rw-rw-rw-   0        0        0      261 2023-08-01 04:09:28.102432 pih-1.48026/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-01 04:09:27.539938 pih-1.48026/pih/
+-rw-rw-rw-   0        0        0      157 2022-12-03 14:38:35.000000 pih-1.48026/pih/__init__.py
+-rw-rw-rw-   0        0        0    20482 2023-07-25 14:36:49.000000 pih-1.48026/pih/collection.py
+-rw-rw-rw-   0        0        0    60753 2023-08-01 04:09:10.000000 pih-1.48026/pih/console_api.py
+-rw-rw-rw-   0        0        0   111144 2023-08-01 00:39:59.000000 pih-1.48026/pih/const.py
+-rw-rw-rw-   0        0        0   317307 2023-08-01 04:09:20.000000 pih-1.48026/pih/pih.py
+-rw-rw-rw-   0        0        0    24697 2023-07-28 13:13:08.000000 pih-1.48026/pih/rpc.py
+-rw-rw-rw-   0        0        0     1941 2022-07-31 10:55:18.000000 pih-1.48026/pih/rpcCommandCall_pb2.py
+-rw-rw-rw-   0        0        0     2465 2022-08-05 02:38:47.000000 pih-1.48026/pih/rpcCommandCall_pb2_grpc.py
+-rw-rw-rw-   0        0        0     2576 2023-07-31 23:11:58.000000 pih-1.48026/pih/rpc_collection.py
+-rw-rw-rw-   0        0        0     6453 2023-07-24 14:50:22.000000 pih-1.48026/pih/rpc_const.py
+-rw-rw-rw-   0        0        0      635 2023-06-11 13:35:46.000000 pih-1.48026/pih/service_example.py
+-rw-rw-rw-   0        0        0    38229 2023-08-01 02:41:41.000000 pih-1.48026/pih/tools.py
+-rw-rw-rw-   0        0        0     2280 2023-06-30 04:39:52.000000 pih-1.48026/pih/widgets.py
+drwxrwxrwx   0        0        0        0 2023-08-01 04:09:28.071182 pih-1.48026/pih.egg-info/
+-rw-rw-rw-   0        0        0      261 2023-08-01 04:09:25.000000 pih-1.48026/pih.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2023-08-01 04:09:26.000000 pih-1.48026/pih.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 04:09:25.000000 pih-1.48026/pih.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-08-01 04:09:26.000000 pih-1.48026/pih.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-08-01 04:09:26.000000 pih-1.48026/pih.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2009 2023-08-01 00:47:12.000000 pih-1.48026/pih_setup.py
+-rw-rw-rw-   0        0        0       42 2023-08-01 04:09:28.118057 pih-1.48026/setup.cfg
```

### Comparing `pih-1.48024/pih/collection.py` & `pih-1.48026/pih/collection.py`

 * *Files identical despite different names*

### Comparing `pih-1.48024/pih/console_api.py` & `pih-1.48026/pih/console_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,18 +133,17 @@
                         self.output.write_result(A.R_I.last_ct_value_containers(True))
                         path: str =  A.PTH.STATISTICS.get_file_path(A.D.get(A.CT_STATISTICS.TYPES.CT))
                         self.output.write_image(j(("   ", A.CT_V.BULLET, " ", self.output.bold("График показаний"))), A.D_CO.file_to_base64(path))
                     self.output.separated_line()
                     self.output.write_line(self.bold(f"{A.CT_V.BULLET} Показания в техническом помещении МРТ"))
                     chiller_indications_value_container_result: Result[list[ChillerIndicationsValueContainer]] = A.R_I.last_chiller_value_containers(True)
                     chiller_indications_value_container: ChillerIndicationsValueContainer = A.R.get_first_item(chiller_indications_value_container_result)
-                    path: str = A.PTH.adapt_if_linux(A.PTH_I.CHILLER_DATA_IMAGE_LAST)
-                    A.O.write_line(f"path: {path}")
-                    modification_timstamp: float = os.path.getmtime(path)
-                    file_creating_datetime: datetime | None = datetime.fromtimestamp(modification_timstamp if modification_timstamp > 0 else os.path.getctime(path))
+                    path: str = A.PTH_I.CHILLER_DATA_IMAGE_LAST
+                    modification_timstamp: float = A.PTH.get_modification_time(path)
+                    file_creating_datetime: datetime | None = datetime.fromtimestamp(modification_timstamp if modification_timstamp > 0 else A.PTH.get_creation_time(path))
                     with self.output.make_indent(2, True):
                         if A.C_E.has(A.E_B.chiller_was_turned_off()):
                             self.output.write_line(j((A.CT_V.WARNING, "Чиллер выключен!", A.CT_V.WARNING)))
                         else:
                             self.output.write_result(chiller_indications_value_container_result, title="Показания чиллера\n" if A.D_C.INDICATIONS.chiller_value_actual(chiller_indications_value_container) else f"{self.bold('Внимание!')}: Показания чиллера неактуальны\n", separated_result_item=False)
                             self.output.write_image(f"    Изображение дисплея чиллера\nВремя снятия: {A.D_F.datetime(file_creating_datetime)}", A.D_CO.file_to_base64(A.PTH_I.CHILLER_DATA_IMAGE_LAST_RESULT))
             if CheckableSections.MATERIALIZED_RESOURCES in checkable_section_list:
@@ -169,15 +168,15 @@
                     self.output.new_line()
                 self.output.separated_line()
                 self.output.write_line(
                     self.bold(f"{A.CT_V.BULLET} Новые исследования в Валенте: " + ("Нет" if count == 0 else f"Да ({count})")))    
                 if count > 0:
                     if self.input.yes_no("Показать отсканированные изображения"):
                         for scanned_file_path in scanned_file_path_list:
-                            self.output.write_image(j(("Дата создания файла: ", A.D_F.datetime(datetime.fromtimestamp(os.path.getctime(scanned_file_path))))),
+                            self.output.write_image(j(("Дата создания файла: ", A.D_F.datetime(datetime.fromtimestamp(A.PTH.get_creation_time(scanned_file_path))))),
                                 A.D_CO.file_to_base64(scanned_file_path))
                     if self.input.yes_no("Синхронизировать Валенту"):
                         A.A_ACT.was_done(A.CT_ACT.VALENTA_SYNCHRONIZATION, self.session.user)
             if CheckableSections.PRINTERS in checkable_section_list:
                 def printer_report(printer_report: PrinterReport) -> str:
                     report_list: list[str] = []
                     admin_description_list: list[str] = ("" or printer_report.adminDescription).split(",")
```

### Comparing `pih-1.48024/pih/const.py` & `pih-1.48026/pih/const.py`

 * *Files identical despite different names*

### Comparing `pih-1.48024/pih/pih.py` & `pih-1.48026/pih/pih.py`

 * *Files 0% similar despite different names*

```diff
@@ -1637,15 +1637,15 @@
             
             @staticmethod
             def local() -> str:
                 return "1.48020"  
 
         @staticmethod
         def local() -> str:
-            return "1.48024"
+            return "1.48026"
 
         @staticmethod
         def need_update() -> bool:
             return False
             #return importlib.util.find_spec(PIH.NAME) is not None and PIH.VERSION.local() < PIH.VERSION.remote()
     
     class INPUT_WAIT:
@@ -2820,19 +2820,21 @@
             description: ServiceDescription = ServiceRoles.description(role_or_information)
             return PIH.OS.host() if description.isolated or DataTool.is_empty(description.host) else description.host
 
     class PATH(PATHS, PathTool):
 
         DIRECTORY_INFO_PREFIX: str = "directory_info_"
 
-        class STATISTICS(PATH_STATISTICS):
+        @staticmethod
+        def get_modification_time(path: str) -> str:
+            return os.path.getmtime(PIH.PATH.adapt_if_linux(path))
 
-            @staticmethod
-            def get_file_path(name: str) -> str:
-                return PIH.PATH.adapt_if_linux(PATH_STATISTICS.get_file_path(name))
+        @staticmethod
+        def get_creation_time(path: str) -> str:
+            return os.path.getctime(PIH.PATH.adapt_if_linux(path))
 
         @staticmethod
         def adapt_if_linux(path: str) -> str:
             if PIH.OS.is_linux():
                 path = PIH.PATH.convert_for_unix(path)
                 alias: str = PIH.PATH.convert_for_unix(PATH_FACADE.PATH)
                 if path.find(alias) == 0:
@@ -3286,14 +3288,15 @@
             
             @staticmethod
             def settings_to_datetime_list(item: SETTINGS, format: str = CONST.SECONDLESS_TIME_FORMAT) -> list[datetime]:
                 return list(map(lambda item: DateTimeTool.datetime_from_string(item, format), PIH.SETTINGS.get(item)))
 
             @staticmethod
             def file_to_base64(path: str) -> str | None:
+                path = PIH.PATH.adapt_if_linux(path)
                 while True:
                     try:
                         with open(path, "rb") as file:
                             return PIH.DATA.CONVERT.bytes_to_base64(file.read())
                     except Exception:
                         pass
                 return None
```

### Comparing `pih-1.48024/pih/rpc.py` & `pih-1.48026/pih/rpc.py`

 * *Files identical despite different names*

### Comparing `pih-1.48024/pih/rpcCommandCall_pb2.py` & `pih-1.48026/pih/rpcCommandCall_pb2.py`

 * *Files identical despite different names*

### Comparing `pih-1.48024/pih/rpcCommandCall_pb2_grpc.py` & `pih-1.48026/pih/rpcCommandCall_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pih-1.48024/pih/rpc_collection.py` & `pih-1.48026/pih/rpc_collection.py`

 * *Files identical despite different names*

### Comparing `pih-1.48024/pih/rpc_const.py` & `pih-1.48026/pih/rpc_const.py`

 * *Files identical despite different names*

### Comparing `pih-1.48024/pih/service_example.py` & `pih-1.48026/pih/service_example.py`

 * *Files identical despite different names*

### Comparing `pih-1.48024/pih/tools.py` & `pih-1.48026/pih/tools.py`

 * *Files identical despite different names*

### Comparing `pih-1.48024/pih/widgets.py` & `pih-1.48026/pih/widgets.py`

 * *Files identical despite different names*

### Comparing `pih-1.48024/pih_setup.py` & `pih-1.48026/pih_setup.py`

 * *Files identical despite different names*

