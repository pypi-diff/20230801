# Comparing `tmp/hypergo-0.1.4.tar.gz` & `tmp/hypergo-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypergo-0.1.4.tar", last modified: Mon Jul 31 14:49:18 2023, max compression
+gzip compressed data, was "hypergo-0.1.5.tar", last modified: Tue Aug  1 18:13:56 2023, max compression
```

## Comparing `hypergo-0.1.4.tar` & `hypergo-0.1.5.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:49:18.435377 hypergo-0.1.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:49:18.427377 hypergo-0.1.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:49:18.427377 hypergo-0.1.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-31 14:49:08.000000 hypergo-0.1.4/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6232 2023-07-31 14:49:08.000000 hypergo-0.1.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-31 14:49:08.000000 hypergo-0.1.4/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-07-31 14:49:08.000000 hypergo-0.1.4/BACKLOG.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:49:08.000000 hypergo-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-31 14:49:18.435377 hypergo-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-31 14:49:08.000000 hypergo-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    12636 2023-07-31 14:49:08.000000 hypergo-0.1.4/RELEASE_NOTES.md
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-31 14:49:08.000000 hypergo-0.1.4/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:49:18.431378 hypergo-0.1.4/hypergo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:49:08.000000 hypergo-0.1.4/hypergo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-31 14:49:08.000000 hypergo-0.1.4/hypergo/azure_service_bus_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-31 14:49:08.000000 hypergo-0.1.4/hypergo/azure_service_bus_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-31 14:49:08.000000 hypergo-0.1.4/hypergo/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-31 14:49:08.000000 hypergo-0.1.4/hypergo/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-31 14:49:08.000000 hypergo-0.1.4/hypergo/custom_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-07-31 14:49:08.000000 hypergo-0.1.4/hypergo/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-07-31 14:49:08.000000 hypergo-0.1.4/hypergo/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-07-31 14:49:08.000000 hypergo-0.1.4/hypergo/hypergo_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-31 14:49:08.000000 hypergo-0.1.4/hypergo/hypergo_click.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-07-31 14:49:08.000000 hypergo-0.1.4/hypergo/hypergo_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-31 14:49:08.000000 hypergo-0.1.4/hypergo/key_value_store.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-31 14:49:08.000000 hypergo-0.1.4/hypergo/local_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-07-31 14:49:08.000000 hypergo-0.1.4/hypergo/message.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-31 14:49:08.000000 hypergo-0.1.4/hypergo/service_bus_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-31 14:49:08.000000 hypergo-0.1.4/hypergo/stdio_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-31 14:49:08.000000 hypergo-0.1.4/hypergo/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-31 14:49:08.000000 hypergo-0.1.4/hypergo/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-07-31 14:49:08.000000 hypergo-0.1.4/hypergo/utility.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-07-31 14:49:08.000000 hypergo-0.1.4/hypergo/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:49:18.431378 hypergo-0.1.4/hypergo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-31 14:49:18.000000 hypergo-0.1.4/hypergo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-31 14:49:18.000000 hypergo-0.1.4/hypergo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 14:49:18.000000 hypergo-0.1.4/hypergo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-31 14:49:18.000000 hypergo-0.1.4/hypergo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-31 14:49:18.000000 hypergo-0.1.4/hypergo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-31 14:49:18.000000 hypergo-0.1.4/hypergo.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     2830 2023-07-31 14:49:08.000000 hypergo-0.1.4/lint.sh
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-31 14:49:08.000000 hypergo-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-31 14:49:18.435377 hypergo-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-31 14:49:08.000000 hypergo-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:49:18.435377 hypergo-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-07-31 14:49:08.000000 hypergo-0.1.4/tests/test.json
--rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-07-31 14:49:08.000000 hypergo-0.1.4/tests/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-31 14:49:08.000000 hypergo-0.1.4/tests/test_dynamic_input_bindings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-07-31 14:49:08.000000 hypergo-0.1.4/tests/test_dynamic_routing_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-07-31 14:49:08.000000 hypergo-0.1.4/tests/test_local_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-31 14:49:08.000000 hypergo-0.1.4/tests/test_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-07-31 14:49:08.000000 hypergo-0.1.4/tests/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-07-31 14:49:08.000000 hypergo-0.1.4/tests/test_utility.py
--rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-07-31 14:49:08.000000 hypergo-0.1.4/tests/test_utility_serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:13:56.580047 hypergo-0.1.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:13:56.568047 hypergo-0.1.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:13:56.572047 hypergo-0.1.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-08-01 18:13:44.000000 hypergo-0.1.5/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6232 2023-08-01 18:13:44.000000 hypergo-0.1.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-01 18:13:44.000000 hypergo-0.1.5/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-08-01 18:13:44.000000 hypergo-0.1.5/BACKLOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 18:13:44.000000 hypergo-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-08-01 18:13:56.580047 hypergo-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-08-01 18:13:44.000000 hypergo-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12636 2023-08-01 18:13:44.000000 hypergo-0.1.5/RELEASE_NOTES.md
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-08-01 18:13:44.000000 hypergo-0.1.5/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:13:56.576047 hypergo-0.1.5/hypergo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 18:13:44.000000 hypergo-0.1.5/hypergo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-08-01 18:13:44.000000 hypergo-0.1.5/hypergo/azure_service_bus_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-01 18:13:44.000000 hypergo-0.1.5/hypergo/azure_service_bus_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-08-01 18:13:44.000000 hypergo-0.1.5/hypergo/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-08-01 18:13:44.000000 hypergo-0.1.5/hypergo/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-08-01 18:13:44.000000 hypergo-0.1.5/hypergo/custom_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-08-01 18:13:44.000000 hypergo-0.1.5/hypergo/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-08-01 18:13:44.000000 hypergo-0.1.5/hypergo/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-08-01 18:13:44.000000 hypergo-0.1.5/hypergo/hypergo_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-08-01 18:13:44.000000 hypergo-0.1.5/hypergo/hypergo_click.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-08-01 18:13:44.000000 hypergo-0.1.5/hypergo/hypergo_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-08-01 18:13:44.000000 hypergo-0.1.5/hypergo/key_value_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-08-01 18:13:44.000000 hypergo-0.1.5/hypergo/local_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-08-01 18:13:44.000000 hypergo-0.1.5/hypergo/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-08-01 18:13:44.000000 hypergo-0.1.5/hypergo/service_bus_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-08-01 18:13:44.000000 hypergo-0.1.5/hypergo/stdio_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-08-01 18:13:44.000000 hypergo-0.1.5/hypergo/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-08-01 18:13:44.000000 hypergo-0.1.5/hypergo/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-08-01 18:13:44.000000 hypergo-0.1.5/hypergo/utility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-08-01 18:13:44.000000 hypergo-0.1.5/hypergo/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:13:56.576047 hypergo-0.1.5/hypergo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-08-01 18:13:56.000000 hypergo-0.1.5/hypergo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-01 18:13:56.000000 hypergo-0.1.5/hypergo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 18:13:56.000000 hypergo-0.1.5/hypergo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-01 18:13:56.000000 hypergo-0.1.5/hypergo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-08-01 18:13:56.000000 hypergo-0.1.5/hypergo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-01 18:13:56.000000 hypergo-0.1.5/hypergo.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2830 2023-08-01 18:13:44.000000 hypergo-0.1.5/lint.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-01 18:13:44.000000 hypergo-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-08-01 18:13:56.580047 hypergo-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-08-01 18:13:44.000000 hypergo-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:13:56.580047 hypergo-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-08-01 18:13:44.000000 hypergo-0.1.5/tests/test.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-08-01 18:13:44.000000 hypergo-0.1.5/tests/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-08-01 18:13:44.000000 hypergo-0.1.5/tests/test_dynamic_input_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-08-01 18:13:44.000000 hypergo-0.1.5/tests/test_dynamic_routing_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-08-01 18:13:44.000000 hypergo-0.1.5/tests/test_local_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-08-01 18:13:44.000000 hypergo-0.1.5/tests/test_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-08-01 18:13:44.000000 hypergo-0.1.5/tests/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-08-01 18:13:44.000000 hypergo-0.1.5/tests/test_utility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-08-01 18:13:44.000000 hypergo-0.1.5/tests/test_utility_serialization.py
```

### Comparing `hypergo-0.1.4/.github/workflows/python-publish.yml` & `hypergo-0.1.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.4/.gitignore` & `hypergo-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.4/BACKLOG.md` & `hypergo-0.1.5/BACKLOG.md`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.4/RELEASE_NOTES.md` & `hypergo-0.1.5/RELEASE_NOTES.md`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.4/hypergo/azure_service_bus_connection.py` & `hypergo-0.1.5/hypergo/azure_service_bus_connection.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.4/hypergo/config.py` & `hypergo-0.1.5/hypergo/config.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.4/hypergo/executor.py` & `hypergo-0.1.5/hypergo/executor.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.4/hypergo/graph.py` & `hypergo-0.1.5/hypergo/graph.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.4/hypergo/hypergo_cli.py` & `hypergo-0.1.5/hypergo/hypergo_cli.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.4/hypergo/hypergo_click.py` & `hypergo-0.1.5/hypergo/hypergo_click.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.4/hypergo/hypergo_cmd.py` & `hypergo-0.1.5/hypergo/hypergo_cmd.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.4/hypergo/local_storage.py` & `hypergo-0.1.5/hypergo/local_storage.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.4/hypergo/message.py` & `hypergo-0.1.5/hypergo/message.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.4/hypergo/service_bus_connection.py` & `hypergo-0.1.5/hypergo/service_bus_connection.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.4/hypergo/stdio_connection.py` & `hypergo-0.1.5/hypergo/stdio_connection.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.4/hypergo/storage.py` & `hypergo-0.1.5/hypergo/storage.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.4/hypergo/transform.py` & `hypergo-0.1.5/hypergo/transform.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 
     @staticmethod
     def compression(
         key: str,
     ) -> Callable[[Callable[..., Generator[T, None, None]]], Callable[..., Generator[T, None, None]]]:
         def decorator(func: Callable[..., Generator[T, None, None]]) -> Callable[..., Generator[T, None, None]]:
             def wrapped_func(self: Any, data: T) -> Generator[T, None, None]:
-                input_operations = Utility.deep_get(self.config, "input_operations")
-                output_operations = Utility.deep_get(self.config, "output_operations")
+                input_operations = Utility.deep_get(self.config, "input_operations", default_sentinel=[])
+                output_operations = Utility.deep_get(self.config, "output_operations", default_sentinel=[])
 
                 if "compression" in input_operations:
                     data = Utility.uncompress(data, key)
 
                 for result in func(self, data):
                     if "compression" in output_operations:
                         result = Utility.compress(result, key)
@@ -40,16 +40,16 @@
     @staticmethod
     def pass_by_reference(
         func: Callable[..., Generator[T, None, None]]
     ) -> Callable[..., Generator[JsonDict, None, None]]:
         def wrapped_func(self: Any, data: T) -> Generator[JsonDict, None, None]:
             storage: Storage = self.storage.use_sub_path("passbyreference")
             the_data: JsonType = cast(JsonType, data)
-            input_operations: List[str] = Utility.deep_get(self.config, "input_operations")
-            output_operations: List[str] = Utility.deep_get(self.config, "output_operations")
+            input_operations: List[str] = Utility.deep_get(self.config, "input_operations", default_sentinel=[])
+            output_operations: List[str] = Utility.deep_get(self.config, "output_operations", default_sentinel=[])
 
             if "pass_by_reference" in input_operations:
                 storage_key = Utility.deep_get(cast(JsonDict, data), "storagekey")
                 the_data = Utility.objectify(storage.load(storage_key))
 
             for result in func(self, the_data):
                 out_message = cast(JsonDict, result)
```

### Comparing `hypergo-0.1.4/hypergo/utility.py` & `hypergo-0.1.5/hypergo/utility.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,18 +25,18 @@
         return handlers.get(type(value), func)(value)
 
     return wrapper
 
 
 class Utility:
     @staticmethod
-    def deep_get(dic: Union[TypedDictType, Dict[str, Any]], key: str) -> Any:
-        if not pydash.has(dic, key):
-            raise KeyError(f"Spec {key}  not found in the dictionary")
-        return pydash.get(dic, key)
+    def deep_get(dic: Union[TypedDictType, Dict[str, Any]], key: str, default_sentinel: Optional[Any] = object) -> Any:
+        if not pydash.has(dic, key) and default_sentinel == object:
+            raise KeyError(f"Spec \"{key}\" not found in the dictionary {json.dumps(dic)}")
+        return pydash.get(dic, key, default_sentinel)
 
     @staticmethod
     def deep_set(dic: Union[TypedDictType, Dict[str, Any]], key: str, val: Any) -> None:
         glom.assign(dic, key, val, missing=dict)
 
     @staticmethod
     def yaml_read(file_name: str) -> Mapping[str, Any]:
```

### Comparing `hypergo-0.1.4/hypergo/version.py` & `hypergo-0.1.5/hypergo/version.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.4/hypergo.egg-info/SOURCES.txt` & `hypergo-0.1.5/hypergo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.4/lint.sh` & `hypergo-0.1.5/lint.sh`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.4/setup.py` & `hypergo-0.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.4/tests/test.json` & `hypergo-0.1.5/tests/test.json`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.4/tests/test.yaml` & `hypergo-0.1.5/tests/test.yaml`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.4/tests/test_dynamic_input_bindings.py` & `hypergo-0.1.5/tests/test_dynamic_input_bindings.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.4/tests/test_dynamic_routing_key.py` & `hypergo-0.1.5/tests/test_dynamic_routing_key.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.4/tests/test_local_storage.py` & `hypergo-0.1.5/tests/test_local_storage.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.4/tests/test_message.py` & `hypergo-0.1.5/tests/test_message.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.4/tests/test_storage.py` & `hypergo-0.1.5/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.4/tests/test_utility.py` & `hypergo-0.1.5/tests/test_utility.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.4/tests/test_utility_serialization.py` & `hypergo-0.1.5/tests/test_utility_serialization.py`

 * *Files identical despite different names*

