# Comparing `tmp/pih-1.48023.tar.gz` & `tmp/pih-1.48024.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-1.48023.tar", last modified: Tue Aug  1 03:17:21 2023, max compression
+gzip compressed data, was "pih-1.48024.tar", last modified: Tue Aug  1 03:21:13 2023, max compression
```

## Comparing `pih-1.48023.tar` & `pih-1.48024.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 03:17:22.011976 pih-1.48023/
--rw-rw-rw-   0        0        0      261 2023-08-01 03:17:21.996351 pih-1.48023/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-01 03:17:21.746354 pih-1.48023/pih/
--rw-rw-rw-   0        0        0      157 2022-12-03 14:38:35.000000 pih-1.48023/pih/__init__.py
--rw-rw-rw-   0        0        0    20482 2023-07-25 14:36:49.000000 pih-1.48023/pih/collection.py
--rw-rw-rw-   0        0        0    61125 2023-08-01 03:14:05.000000 pih-1.48023/pih/console_api.py
--rw-rw-rw-   0        0        0   111144 2023-08-01 00:39:59.000000 pih-1.48023/pih/const.py
--rw-rw-rw-   0        0        0   317173 2023-08-01 03:17:06.000000 pih-1.48023/pih/pih.py
--rw-rw-rw-   0        0        0    24697 2023-07-28 13:13:08.000000 pih-1.48023/pih/rpc.py
--rw-rw-rw-   0        0        0     1941 2022-07-31 10:55:18.000000 pih-1.48023/pih/rpcCommandCall_pb2.py
--rw-rw-rw-   0        0        0     2465 2022-08-05 02:38:47.000000 pih-1.48023/pih/rpcCommandCall_pb2_grpc.py
--rw-rw-rw-   0        0        0     2576 2023-07-31 23:11:58.000000 pih-1.48023/pih/rpc_collection.py
--rw-rw-rw-   0        0        0     6453 2023-07-24 14:50:22.000000 pih-1.48023/pih/rpc_const.py
--rw-rw-rw-   0        0        0      635 2023-06-11 13:35:46.000000 pih-1.48023/pih/service_example.py
--rw-rw-rw-   0        0        0    38229 2023-08-01 02:41:41.000000 pih-1.48023/pih/tools.py
--rw-rw-rw-   0        0        0     2280 2023-06-30 04:39:52.000000 pih-1.48023/pih/widgets.py
-drwxrwxrwx   0        0        0        0 2023-08-01 03:17:21.965101 pih-1.48023/pih.egg-info/
--rw-rw-rw-   0        0        0      261 2023-08-01 03:17:19.000000 pih-1.48023/pih.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      381 2023-08-01 03:17:20.000000 pih-1.48023/pih.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 03:17:19.000000 pih-1.48023/pih.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-08-01 03:17:20.000000 pih-1.48023/pih.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-08-01 03:17:20.000000 pih-1.48023/pih.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2009 2023-08-01 00:47:12.000000 pih-1.48023/pih_setup.py
--rw-rw-rw-   0        0        0       42 2023-08-01 03:17:22.027605 pih-1.48023/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-01 03:21:14.037731 pih-1.48024/
+-rw-rw-rw-   0        0        0      261 2023-08-01 03:21:14.037731 pih-1.48024/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-01 03:21:13.662732 pih-1.48024/pih/
+-rw-rw-rw-   0        0        0      157 2022-12-03 14:38:35.000000 pih-1.48024/pih/__init__.py
+-rw-rw-rw-   0        0        0    20482 2023-07-25 14:36:49.000000 pih-1.48024/pih/collection.py
+-rw-rw-rw-   0        0        0    60803 2023-08-01 03:20:53.000000 pih-1.48024/pih/console_api.py
+-rw-rw-rw-   0        0        0   111144 2023-08-01 00:39:59.000000 pih-1.48024/pih/const.py
+-rw-rw-rw-   0        0        0   317173 2023-08-01 03:21:04.000000 pih-1.48024/pih/pih.py
+-rw-rw-rw-   0        0        0    24697 2023-07-28 13:13:08.000000 pih-1.48024/pih/rpc.py
+-rw-rw-rw-   0        0        0     1941 2022-07-31 10:55:18.000000 pih-1.48024/pih/rpcCommandCall_pb2.py
+-rw-rw-rw-   0        0        0     2465 2022-08-05 02:38:47.000000 pih-1.48024/pih/rpcCommandCall_pb2_grpc.py
+-rw-rw-rw-   0        0        0     2576 2023-07-31 23:11:58.000000 pih-1.48024/pih/rpc_collection.py
+-rw-rw-rw-   0        0        0     6453 2023-07-24 14:50:22.000000 pih-1.48024/pih/rpc_const.py
+-rw-rw-rw-   0        0        0      635 2023-06-11 13:35:46.000000 pih-1.48024/pih/service_example.py
+-rw-rw-rw-   0        0        0    38229 2023-08-01 02:41:41.000000 pih-1.48024/pih/tools.py
+-rw-rw-rw-   0        0        0     2280 2023-06-30 04:39:52.000000 pih-1.48024/pih/widgets.py
+drwxrwxrwx   0        0        0        0 2023-08-01 03:21:13.990851 pih-1.48024/pih.egg-info/
+-rw-rw-rw-   0        0        0      261 2023-08-01 03:21:11.000000 pih-1.48024/pih.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2023-08-01 03:21:12.000000 pih-1.48024/pih.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 03:21:11.000000 pih-1.48024/pih.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-08-01 03:21:12.000000 pih-1.48024/pih.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-08-01 03:21:12.000000 pih-1.48024/pih.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2009 2023-08-01 00:47:12.000000 pih-1.48024/pih_setup.py
+-rw-rw-rw-   0        0        0       42 2023-08-01 03:21:14.053351 pih-1.48024/setup.cfg
```

### Comparing `pih-1.48023/pih/collection.py` & `pih-1.48024/pih/collection.py`

 * *Files identical despite different names*

### Comparing `pih-1.48023/pih/console_api.py` & `pih-1.48024/pih/console_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,37 +121,36 @@
                         if self.is_mobile:
                             self.output.new_line()
                         if all:
                             self.output.write_line(" ".join((A.CT_V.BULLET, self.bold(A.D.check(checkable_section == CheckableSections.RESOURCES, "Основные ресурсы", A.D.check(checkable_section == CheckableSections.WS, "Наблюдаемые компьютеры", "Сервера"))))))
                         with self.output.make_indent(2, True):
                             self.output.write_result(A.R_R.get_status_list([checkable_section], force_update, all if len(checkable_section_list) == 1 and CheckableSections.WS in checkable_section_list else False), False, label_function=label_function, separated_result_item=self.is_mobile)
             if CheckableSections.INDICATIONS in checkable_section_list:
-                #self.output.separated_line()
-                #self.output.write_line(f"Показания доступны по адрессу:\n{self.bold('http://indications')}, если заходить с рабочего компьютера\nили\n{self.bold('http://192.168.100.138')}, если заходить с мобильного телефона, подключенного к корпоративной wifi сети")
-                if self.is_mobile:
-                    self.output.new_line()
-                self.output.write_line(self.bold(f"{A.CT_V.BULLET} Показания в помещении КТ"))
-                with self.output.make_indent(2, True):
-                    self.output.write_result(A.R_I.last_ct_value_containers(True))
-                    path: str =  A.PTH.STATISTICS.get_file_path(A.D.get(A.CT_STATISTICS.TYPES.CT))
+                with A.ER.detect():
+                    if self.is_mobile:
+                        self.output.new_line()
+                    self.output.write_line(self.bold(f"{A.CT_V.BULLET} Показания в помещении КТ"))
+                    with self.output.make_indent(2, True):
+                        self.output.write_result(A.R_I.last_ct_value_containers(True))
+                        path: str =  A.PTH.STATISTICS.get_file_path(A.D.get(A.CT_STATISTICS.TYPES.CT))
+                        self.output.write_image(j(("   ", A.CT_V.BULLET, " ", self.output.bold("График показаний"))), A.D_CO.file_to_base64(path))
+                    self.output.separated_line()
+                    self.output.write_line(self.bold(f"{A.CT_V.BULLET} Показания в техническом помещении МРТ"))
+                    chiller_indications_value_container_result: Result[list[ChillerIndicationsValueContainer]] = A.R_I.last_chiller_value_containers(True)
+                    chiller_indications_value_container: ChillerIndicationsValueContainer = A.R.get_first_item(chiller_indications_value_container_result)
+                    path: str = A.PTH.adapt_if_linux(A.PTH_I.CHILLER_DATA_IMAGE_LAST)
                     A.O.write_line(f"path: {path}")
-                    self.output.write_image(j(("   ", A.CT_V.BULLET, " ", self.output.bold("График показаний"))), A.D_CO.file_to_base64(path))
-                self.output.separated_line()
-                self.output.write_line(self.bold(f"{A.CT_V.BULLET} Показания в техническом помещении МРТ"))
-                chiller_indications_value_container_result: Result[list[ChillerIndicationsValueContainer]] = A.R_I.last_chiller_value_containers(True)
-                chiller_indications_value_container: ChillerIndicationsValueContainer = A.R.get_first_item(chiller_indications_value_container_result)
-                path: str = A.PTH.adapt_if_linux(A.PTH_I.CHILLER_DATA_IMAGE_LAST)
-                modification_timstamp: float = os.path.getmtime(path)
-                file_creating_datetime: datetime | None = datetime.fromtimestamp(modification_timstamp if modification_timstamp > 0 else os.path.getctime(path))
-                with self.output.make_indent(2, True):
-                    if A.C_E.has(A.E_B.chiller_was_turned_off()):
-                        self.output.write_line(j((A.CT_V.WARNING, "Чиллер выключен!", A.CT_V.WARNING)))
-                    else:
-                        self.output.write_result(chiller_indications_value_container_result, title="Показания чиллера\n" if A.D_C.INDICATIONS.chiller_value_actual(chiller_indications_value_container) else f"{self.bold('Внимание!')}: Показания чиллера неактуальны\n", separated_result_item=False)
-                        self.output.write_image(f"    Изображение дисплея чиллера\nВремя снятия: {A.D_F.datetime(file_creating_datetime)}", A.D_CO.file_to_base64(A.PTH_I.CHILLER_DATA_IMAGE_LAST_RESULT))
+                    modification_timstamp: float = os.path.getmtime(path)
+                    file_creating_datetime: datetime | None = datetime.fromtimestamp(modification_timstamp if modification_timstamp > 0 else os.path.getctime(path))
+                    with self.output.make_indent(2, True):
+                        if A.C_E.has(A.E_B.chiller_was_turned_off()):
+                            self.output.write_line(j((A.CT_V.WARNING, "Чиллер выключен!", A.CT_V.WARNING)))
+                        else:
+                            self.output.write_result(chiller_indications_value_container_result, title="Показания чиллера\n" if A.D_C.INDICATIONS.chiller_value_actual(chiller_indications_value_container) else f"{self.bold('Внимание!')}: Показания чиллера неактуальны\n", separated_result_item=False)
+                            self.output.write_image(f"    Изображение дисплея чиллера\nВремя снятия: {A.D_F.datetime(file_creating_datetime)}", A.D_CO.file_to_base64(A.PTH_I.CHILLER_DATA_IMAGE_LAST_RESULT))
             if CheckableSections.MATERIALIZED_RESOURCES in checkable_section_list:
                 if self.is_mobile:
                     self.output.new_line()
                 self.output.separated_line()
                 self.output.write_line(
                     self.bold(f"{A.CT_V.BULLET} Материальные ресурсы"))
                 with self.output.make_indent(2, True):
```

### Comparing `pih-1.48023/pih/const.py` & `pih-1.48024/pih/const.py`

 * *Files identical despite different names*

### Comparing `pih-1.48023/pih/pih.py` & `pih-1.48024/pih/pih.py`

 * *Files 0% similar despite different names*

```diff
@@ -1637,15 +1637,15 @@
             
             @staticmethod
             def local() -> str:
                 return "1.48020"  
 
         @staticmethod
         def local() -> str:
-            return "1.48023"
+            return "1.48024"
 
         @staticmethod
         def need_update() -> bool:
             return False
             #return importlib.util.find_spec(PIH.NAME) is not None and PIH.VERSION.local() < PIH.VERSION.remote()
     
     class INPUT_WAIT:
```

### Comparing `pih-1.48023/pih/rpc.py` & `pih-1.48024/pih/rpc.py`

 * *Files identical despite different names*

### Comparing `pih-1.48023/pih/rpcCommandCall_pb2.py` & `pih-1.48024/pih/rpcCommandCall_pb2.py`

 * *Files identical despite different names*

### Comparing `pih-1.48023/pih/rpcCommandCall_pb2_grpc.py` & `pih-1.48024/pih/rpcCommandCall_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pih-1.48023/pih/rpc_collection.py` & `pih-1.48024/pih/rpc_collection.py`

 * *Files identical despite different names*

### Comparing `pih-1.48023/pih/rpc_const.py` & `pih-1.48024/pih/rpc_const.py`

 * *Files identical despite different names*

### Comparing `pih-1.48023/pih/service_example.py` & `pih-1.48024/pih/service_example.py`

 * *Files identical despite different names*

### Comparing `pih-1.48023/pih/tools.py` & `pih-1.48024/pih/tools.py`

 * *Files identical despite different names*

### Comparing `pih-1.48023/pih/widgets.py` & `pih-1.48024/pih/widgets.py`

 * *Files identical despite different names*

### Comparing `pih-1.48023/pih_setup.py` & `pih-1.48024/pih_setup.py`

 * *Files identical despite different names*

