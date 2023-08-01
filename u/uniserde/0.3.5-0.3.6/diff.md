# Comparing `tmp/uniserde-0.3.5.tar.gz` & `tmp/uniserde-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uniserde-0.3.5.tar", max compression
+gzip compressed data, was "uniserde-0.3.6.tar", max compression
```

## Comparing `uniserde-0.3.5.tar` & `uniserde-0.3.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1059 2023-07-21 17:40:19.302257 uniserde-0.3.5/LICENSE
--rw-r--r--   0        0        0     9367 2023-08-01 18:09:12.887737 uniserde-0.3.5/README.md
--rw-r--r--   0        0        0      695 2023-08-01 18:24:18.918462 uniserde-0.3.5/pyproject.toml
--rw-r--r--   0        0        0      336 2023-07-31 06:46:10.489205 uniserde-0.3.5/uniserde/__init__.py
--rw-r--r--   0        0        0     2439 2023-07-31 08:58:33.668781 uniserde-0.3.5/uniserde/bson_deserialize.py
--rw-r--r--   0        0        0     2162 2023-07-31 06:37:08.888725 uniserde-0.3.5/uniserde/bson_serialize.py
--rw-r--r--   0        0        0    10609 2023-08-01 17:53:13.096894 uniserde-0.3.5/uniserde/caching_serdeserializer.py
--rw-r--r--   0        0        0     1210 2023-07-04 19:24:43.375352 uniserde-0.3.5/uniserde/case_convert.py
--rw-r--r--   0        0        0     4051 2023-07-28 13:42:15.590760 uniserde-0.3.5/uniserde/common.py
--rw-r--r--   0        0        0     6921 2023-07-31 08:16:58.436825 uniserde-0.3.5/uniserde/json_deserialize.py
--rw-r--r--   0        0        0     5688 2023-07-30 06:23:39.368547 uniserde-0.3.5/uniserde/json_serialize.py
--rw-r--r--   0        0        0     3840 2023-08-01 18:06:03.527719 uniserde-0.3.5/uniserde/lazy_wrapper.py
--rw-r--r--   0        0        0     2102 2023-07-31 06:36:20.252018 uniserde-0.3.5/uniserde/objectid_proxy.py
--rw-r--r--   0        0        0     9182 2023-07-31 08:05:30.396114 uniserde-0.3.5/uniserde/schema_mongodb.py
--rw-r--r--   0        0        0     2980 2023-07-31 08:06:04.899486 uniserde-0.3.5/uniserde/serde_class.py
--rw-r--r--   0        0        0      487 2023-07-04 19:24:43.382018 uniserde-0.3.5/uniserde/typedefs.py
--rw-r--r--   0        0        0    10133 1970-01-01 00:00:00.000000 uniserde-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1059 2023-07-21 17:40:19.302257 uniserde-0.3.6/LICENSE
+-rw-r--r--   0        0        0     9367 2023-08-01 18:09:12.887737 uniserde-0.3.6/README.md
+-rw-r--r--   0        0        0      695 2023-08-01 20:40:19.970990 uniserde-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0      336 2023-07-31 06:46:10.489205 uniserde-0.3.6/uniserde/__init__.py
+-rw-r--r--   0        0        0     2439 2023-07-31 08:58:33.668781 uniserde-0.3.6/uniserde/bson_deserialize.py
+-rw-r--r--   0        0        0     2162 2023-07-31 06:37:08.888725 uniserde-0.3.6/uniserde/bson_serialize.py
+-rw-r--r--   0        0        0    10609 2023-08-01 17:53:13.096894 uniserde-0.3.6/uniserde/caching_serdeserializer.py
+-rw-r--r--   0        0        0     1210 2023-07-04 19:24:43.375352 uniserde-0.3.6/uniserde/case_convert.py
+-rw-r--r--   0        0        0     4051 2023-07-28 13:42:15.590760 uniserde-0.3.6/uniserde/common.py
+-rw-r--r--   0        0        0     6921 2023-07-31 08:16:58.436825 uniserde-0.3.6/uniserde/json_deserialize.py
+-rw-r--r--   0        0        0     5688 2023-07-30 06:23:39.368547 uniserde-0.3.6/uniserde/json_serialize.py
+-rw-r--r--   0        0        0     4115 2023-08-01 20:38:30.124059 uniserde-0.3.6/uniserde/lazy_wrapper.py
+-rw-r--r--   0        0        0     2102 2023-07-31 06:36:20.252018 uniserde-0.3.6/uniserde/objectid_proxy.py
+-rw-r--r--   0        0        0     9182 2023-07-31 08:05:30.396114 uniserde-0.3.6/uniserde/schema_mongodb.py
+-rw-r--r--   0        0        0     2980 2023-07-31 08:06:04.899486 uniserde-0.3.6/uniserde/serde_class.py
+-rw-r--r--   0        0        0      487 2023-07-04 19:24:43.382018 uniserde-0.3.6/uniserde/typedefs.py
+-rw-r--r--   0        0        0    10133 1970-01-01 00:00:00.000000 uniserde-0.3.6/PKG-INFO
```

### Comparing `uniserde-0.3.5/LICENSE` & `uniserde-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `uniserde-0.3.5/README.md` & `uniserde-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `uniserde-0.3.5/pyproject.toml` & `uniserde-0.3.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "uniserde"
-version = "0.3.5"
+version = "0.3.6"
 description = "Convention based, effortless serialization and deserialization"
 authors = ["Jakob Pinterits <jakob.pinterits@gmail.com>"]
 license = "MIT"
 repository = "https://gitlab.com/Vivern/uniserde"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `uniserde-0.3.5/uniserde/bson_deserialize.py` & `uniserde-0.3.6/uniserde/bson_deserialize.py`

 * *Files identical despite different names*

### Comparing `uniserde-0.3.5/uniserde/bson_serialize.py` & `uniserde-0.3.6/uniserde/bson_serialize.py`

 * *Files identical despite different names*

### Comparing `uniserde-0.3.5/uniserde/caching_serdeserializer.py` & `uniserde-0.3.6/uniserde/caching_serdeserializer.py`

 * *Files identical despite different names*

### Comparing `uniserde-0.3.5/uniserde/case_convert.py` & `uniserde-0.3.6/uniserde/case_convert.py`

 * *Files identical despite different names*

### Comparing `uniserde-0.3.5/uniserde/common.py` & `uniserde-0.3.6/uniserde/common.py`

 * *Files identical despite different names*

### Comparing `uniserde-0.3.5/uniserde/json_deserialize.py` & `uniserde-0.3.6/uniserde/json_deserialize.py`

 * *Files identical despite different names*

### Comparing `uniserde-0.3.5/uniserde/json_serialize.py` & `uniserde-0.3.6/uniserde/json_serialize.py`

 * *Files identical despite different names*

### Comparing `uniserde-0.3.5/uniserde/lazy_wrapper.py` & `uniserde-0.3.6/uniserde/lazy_wrapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,17 +31,25 @@
 
 _FIELD_MAP_CACHE: Dict[
     Tuple[Type, Type[caching_serdeserializer.CachingSerDeserializer]], Type
 ] = {}
 
 
 def _lazy_getattr(self, name: str) -> Any:
-    # See if there is a field definition for this field
+    # Fetch the field definitions. This will fail if this particular instance
+    # isn't lazy
     try:
-        field_doc_name, field_type = self._uniserde_field_definitions_[name]
+        field_definitions = vars(self)["_uniserde_field_definitions_"]
+    except KeyError:
+        raise AttributeError(name) from None
+
+    # See if there is a field definition for this field. This will fail if the
+    # field doesn't exist
+    try:
+        field_doc_name, field_type = field_definitions[name]
     except KeyError:
         raise AttributeError(name) from None
 
     # Get the field value
     try:
         field_raw_value = self._uniserde_remaining_fields_.pop(field_doc_name)
     except KeyError:
```

### Comparing `uniserde-0.3.5/uniserde/objectid_proxy.py` & `uniserde-0.3.6/uniserde/objectid_proxy.py`

 * *Files identical despite different names*

### Comparing `uniserde-0.3.5/uniserde/schema_mongodb.py` & `uniserde-0.3.6/uniserde/schema_mongodb.py`

 * *Files identical despite different names*

### Comparing `uniserde-0.3.5/uniserde/serde_class.py` & `uniserde-0.3.6/uniserde/serde_class.py`

 * *Files identical despite different names*

### Comparing `uniserde-0.3.5/PKG-INFO` & `uniserde-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uniserde
-Version: 0.3.5
+Version: 0.3.6
 Summary: Convention based, effortless serialization and deserialization
 Home-page: https://gitlab.com/Vivern/uniserde
 License: MIT
 Author: Jakob Pinterits
 Author-email: jakob.pinterits@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

