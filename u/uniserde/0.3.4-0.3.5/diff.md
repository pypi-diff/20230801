# Comparing `tmp/uniserde-0.3.4.tar.gz` & `tmp/uniserde-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uniserde-0.3.4.tar", max compression
+gzip compressed data, was "uniserde-0.3.5.tar", max compression
```

## Comparing `uniserde-0.3.4.tar` & `uniserde-0.3.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1059 2023-07-21 17:40:19.302257 uniserde-0.3.4/LICENSE
--rw-r--r--   0        0        0     8358 2023-07-30 06:09:10.148042 uniserde-0.3.4/README.md
--rw-r--r--   0        0        0      695 2023-07-30 06:24:17.458574 uniserde-0.3.4/pyproject.toml
--rw-r--r--   0        0        0      328 2023-07-04 19:27:50.392268 uniserde-0.3.4/uniserde/__init__.py
--rw-r--r--   0        0        0     2098 2023-07-28 13:46:04.514003 uniserde-0.3.4/uniserde/bson_deserialize.py
--rw-r--r--   0        0        0     9416 2023-07-30 06:21:16.785122 uniserde-0.3.4/uniserde/caching_serdeserializer.py
--rw-r--r--   0        0        0     1210 2023-07-04 19:24:43.375352 uniserde-0.3.4/uniserde/case_convert.py
--rw-r--r--   0        0        0     4051 2023-07-28 13:42:15.590760 uniserde-0.3.4/uniserde/common.py
--rw-r--r--   0        0        0     6022 2023-07-30 06:12:14.778353 uniserde-0.3.4/uniserde/json_deserialize.py
--rw-r--r--   0        0        0      600 2023-07-22 10:52:35.786683 uniserde-0.3.4/uniserde/lazy_wrapped.py
--rw-r--r--   0        0        0     1974 2023-07-04 19:24:43.382018 uniserde-0.3.4/uniserde/objectid_proxy.py
--rw-r--r--   0        0        0     9065 2023-07-30 06:23:39.365214 uniserde-0.3.4/uniserde/schema_mongodb.py
--rw-r--r--   0        0        0     2150 2023-07-29 22:24:28.305621 uniserde-0.3.4/uniserde/serde_bson.py
--rw-r--r--   0        0        0     2670 2023-07-28 13:42:15.594093 uniserde-0.3.4/uniserde/serde_class.py
--rw-r--r--   0        0        0     5688 2023-07-30 06:23:39.368547 uniserde-0.3.4/uniserde/serde_json.py
--rw-r--r--   0        0        0      487 2023-07-04 19:24:43.382018 uniserde-0.3.4/uniserde/typedefs.py
--rw-r--r--   0        0        0     9124 1970-01-01 00:00:00.000000 uniserde-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1059 2023-07-21 17:40:19.302257 uniserde-0.3.5/LICENSE
+-rw-r--r--   0        0        0     9367 2023-08-01 18:09:12.887737 uniserde-0.3.5/README.md
+-rw-r--r--   0        0        0      695 2023-08-01 18:24:18.918462 uniserde-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0      336 2023-07-31 06:46:10.489205 uniserde-0.3.5/uniserde/__init__.py
+-rw-r--r--   0        0        0     2439 2023-07-31 08:58:33.668781 uniserde-0.3.5/uniserde/bson_deserialize.py
+-rw-r--r--   0        0        0     2162 2023-07-31 06:37:08.888725 uniserde-0.3.5/uniserde/bson_serialize.py
+-rw-r--r--   0        0        0    10609 2023-08-01 17:53:13.096894 uniserde-0.3.5/uniserde/caching_serdeserializer.py
+-rw-r--r--   0        0        0     1210 2023-07-04 19:24:43.375352 uniserde-0.3.5/uniserde/case_convert.py
+-rw-r--r--   0        0        0     4051 2023-07-28 13:42:15.590760 uniserde-0.3.5/uniserde/common.py
+-rw-r--r--   0        0        0     6921 2023-07-31 08:16:58.436825 uniserde-0.3.5/uniserde/json_deserialize.py
+-rw-r--r--   0        0        0     5688 2023-07-30 06:23:39.368547 uniserde-0.3.5/uniserde/json_serialize.py
+-rw-r--r--   0        0        0     3840 2023-08-01 18:06:03.527719 uniserde-0.3.5/uniserde/lazy_wrapper.py
+-rw-r--r--   0        0        0     2102 2023-07-31 06:36:20.252018 uniserde-0.3.5/uniserde/objectid_proxy.py
+-rw-r--r--   0        0        0     9182 2023-07-31 08:05:30.396114 uniserde-0.3.5/uniserde/schema_mongodb.py
+-rw-r--r--   0        0        0     2980 2023-07-31 08:06:04.899486 uniserde-0.3.5/uniserde/serde_class.py
+-rw-r--r--   0        0        0      487 2023-07-04 19:24:43.382018 uniserde-0.3.5/uniserde/typedefs.py
+-rw-r--r--   0        0        0    10133 1970-01-01 00:00:00.000000 uniserde-0.3.5/PKG-INFO
```

### Comparing `uniserde-0.3.4/LICENSE` & `uniserde-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `uniserde-0.3.4/README.md` & `uniserde-0.3.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Convention based, effortless serialization and deserialization
 
 `uniserde` can convert Python classes to/from JSON and BSON without any input
 from your side. Simply define the classes, and the library does the rest.
 
-Simply define your types as classes with type annotations, and call one of the
+Define your types as classes with type annotations, and call one of `uniserde`'s
 serialization/deserialization functions:
 
 ```py
 from uniserde import Serde
 from datetime import datetime, timezone
 from dataclasses import dataclass
 from .objectid_proxy import ObjectId
@@ -40,26 +40,25 @@
 ```
 
 You can easily convert this to a string using Python's built-in `json` module if
 that's what you need.
 
 ## API
 
-The API is intentionally simple. Functions/Classes you might be interested in
-are:
+The API is extremely simple. Functions/Classes you might be interested in are:
 
 - `as_json`, `as_bson`
 
   Given a class with type annotations, these create a JSON/BSON like dictionary.
   You can feed those into functions like `json.dump`, or use them as is.
 
 - `from_json`, `from_bson`
 
-  Given a JSON/BSON like dictionary, these will instantiate the corresponding
-  Python class. Raise `SerdeError` if the values are invalid.
+  Given a JSON/BSON like dictionary and Python type, these will instantiate the
+  corresponding Python class. Raise `SerdeError` if the values are invalid.
 
 - `Serde` is a helper class you can optionally apply to your models. It adds the
   convenience functions `as_json`, `as_bson`, `from_json`, and `from_bson`
   directly to the models.
 
 - Sometimes a class simply acts as a type-safe base, but you really just want to
   serialize the children of that class. In that case you can decorate the class
@@ -69,65 +68,85 @@
 - `as_mongodb_schema` automatically creates JSON schemas compatible with MongoDB
   from models
 
 - Custom serialization / deserialization can be achieved by inheriting from the
   `Serde` class and overriding the `as_json`, `as_bson`, `from_json`,
   `from_bson` and/or `as_mongodb_schema` methods.
 
+## Lazy Deserialization
+
+Normally, serialization happens all at once: You tell `uniserde` to create a
+class instance from a JSON, `uniserde` processes all of the fields and returns
+the finished class.
+
+This works great, but can be wasteful if you are working with large documents
+and only need to access few fields. To help with this, you can pass `lazy=True`
+when deserializing any object. `uniserde` will then hold off deserializing
+fields until they are accessed for the first time, saving precious processing
+time.
+
+**A word of caution:** Data is validated as it is deserialized. Since lazy
+deserialization defers work until the data is accessed, this means any data you
+don't access also won't be validated. Thus, lazy serialization can be a very
+powerful tool for speeding up interactions with large objects, but you should
+only use when you are absolutely certain the data is correct. (For example
+because you have just fetched the object from your own, trusted, database.)
+
 ## Types & Conventions
 
 The library tries to stick to the naming conventions used by the target formats:
 
-- names in JSON are written in lowerCamelCase, as is commonly done in
-  JavaScript
+- names in JSON are written in _lowerCamelCase_, as is convention in JavaScript
 - BSON uses the same conventions as JSON
-- Python class names are expected to be written in UpperCamelCase
-- Python enum values must be in ALL_UPPER_CASE
+- Python class names must be in _UpperCamelCase_
+- Python fields must be in _all_lower_case_
+- Python enum values must be in _ALL_UPPER_CASE_
 
 ### JSON
 
-| Python           | JSON              | Notes                                                                                                                 |
-| ---------------- | ----------------- | --------------------------------------------------------------------------------------------------------------------  |
-| `bool`           | `bool`            |                                                                                                                       |
-| `int`            | `float`           |                                                                                                                       |
-| `float`          | `float`           |                                                                                                                       |
-| `str`            | `str`             |                                                                                                                       |
-| `Tuple`          | `list`            |                                                                                                                       |
-| `List`           | `list`            |                                                                                                                       |
-| `Set`            | `list`            |                                                                                                                       |
-| `Optional`       | value or `None`   |                                                                                                                       |
-| `Any`            | as-is             |                                                                                                                       |
-| `Literal[str]`   | `str`             |                                                                                                                       |
-| `enum.Enum`      | `str`             | Enum values are mapped to their name (NOT value!)                                                                     |
-| `enum.Flag`      | `List[str]`       | Each flag is encoded the same way a single `Enum` would.                                                              |
-| custom class     | `dict`            | Each attribute is stored as key, in lowerCamelCase. If marked with `as_child`, an additional `type` field is added.   |
-| `bytes`          | `str`             | base64 encoded                                                                                                        |
-| `datetime`       | `str`             | as ISO 8601 - with timezone. Naïve datetimes are intentionally not supported. Do yourself a favor and don't use them. |
-| `timedelta`      | `float`           | duration, in seconds                                                                                                  |
-| `Dict[str, ...]` | `dict`            |                                                                                                                       |
-| `bson.ObjectId`  | `str`             |                                                                                                                       |
+| Python               | JSON              | Notes                                                                                                                 |
+| -------------------- | ----------------- | --------------------------------------------------------------------------------------------------------------------- |
+| `bool`               | `bool`            |                                                                                                                       |
+| `int`                | `float`           |                                                                                                                       |
+| `float`              | `float`           |                                                                                                                       |
+| `str`                | `str`             |                                                                                                                       |
+| `Tuple`              | `list`            |                                                                                                                       |
+| `List`               | `list`            |                                                                                                                       |
+| `Set`                | `list`            |                                                                                                                       |
+| `Optional`           | value or `None`   |                                                                                                                       |
+| `Any`                | as-is             |                                                                                                                       |
+| `Literal[str]`       | `str`             |                                                                                                                       |
+| `enum.Enum`          | `str`             | Enum values are mapped to their _name_ (**NOT value!**)                                                               |
+| `enum.Flag`          | `List[str]`       | Each flag is encoded the same way a regular `enum.Enum` value would.                                                  |
+| custom class         | `dict`            | Each attribute is stored as key, in _lowerCamelCase_. If marked with `as_child`, an additional `type` field is added. |
+| `bytes`              | `str`             | base64 encoded                                                                                                        |
+| `datttime.datetime`  | `str`             | as ISO 8601 - with timezone. Naïve datetimes are intentionally not supported. Do yourself a favor and don't use them. |
+| `datetime.timedelta` | `float`           | duration, in seconds                                                                                                  |
+| `Dict[str, ...]`     | `dict`            |                                                                                                                       |
+| `bson.ObjectId`      | `str`             |                                                                                                                       |
 
 ### BSON
 
 BSON uses the same conventions as JSON, with just a few changes
 
-| Python          | BSON            | Notes                                                                                                                                                 |
-| --------------- | --------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------- |
-| custom class    | `dict`          | Same as JSON, but any fields named `id` are renamed to `_id` to match MongoDB. (Exception: if an `_id` field is already present, `id` is not renamed) |
-| `bytes`         | `bytes`         |                                                                                                                                                       |
-| `datetime`      | `datetime`      | Serialization requires a timezone be set. Deserialization imputes UTC, to match MongoDB convention.                                                   |
-| `bson.ObjectId` | `bson.ObjectId` |                                                                                                                                                       |
+| Python              | BSON                | Notes                                                                                    |
+| ------------------- | ------------------- | ---------------------------------------------------------------------------------------- |
+| custom class        | `dict`              | Same as JSON, but any fields named `id` are renamed to `_id` to match MongoDB.           |
+| `bytes`             | `bytes`             |                                                                                          |
+| `datetime.datetime` | `datetime.datetime` | Serialization requires a timezone be set. Deserialization imputes UTC, to match MongoDB. |
+| `bson.ObjectId`     | `bson.ObjectId`     |                                                                                          |
 
-## Schema Generation
+## MongoDB Schema Generation
 
 If you are working with MongoDB you will come to appreciate the automatic schema
 generation. Calling `uniserde.as_mongodb_schema` on any supported class will return
 a MongoDB compatible JSON schema without hassle.
 
-For example `uniserde.as_mongodb_schema(Person)` with the `Person` class from above:
+For example, here's the result of `uniserde.as_mongodb_schema(Person)` with the
+`Person` class above:
 
 ```py
 {
     'type': 'object',
     'properties': {
         '_id': {
             'bsonType': 'objectId'
@@ -147,20 +166,23 @@
     ]
 }
 ```
 
 ## TODO
 
 - Support for `Union` is currently very limited. Really only `Optional` is
-  supported (which maps to `Union`)
+  supported (which Python internally maps to `Union`)
 - `Literal` currently only supports strings
-- Make support for BSON optional, so the library doesn't depend on MongoDB
 - Extend `as_child`, to allow marking some classes as abstract. i.e. their
   parents/children can be serialized, but not those classes themselves
 - Being able to specify additional limitations to fields would be nice:
   - must match regex
   - minimum / maximum
   - custom validation functions
-- more Unit tests
+- more Unit tests (custom de-serializers!?)
 - Add more examples to the README
   - show custom serializers/deserializers
   - recommended usage
+- regression tracking
+- calling `uniserde.serialize` on nonclasses causes problems, because the
+  serialization `as_type` is guessed incorrectly. e.g. `[1, 2, 3]` will be
+  incorrectly serialized as `list` rather than `List[int]`.
```

### Comparing `uniserde-0.3.4/pyproject.toml` & `uniserde-0.3.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "uniserde"
-version = "0.3.4"
+version = "0.3.5"
 description = "Convention based, effortless serialization and deserialization"
 authors = ["Jakob Pinterits <jakob.pinterits@gmail.com>"]
 license = "MIT"
 repository = "https://gitlab.com/Vivern/uniserde"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `uniserde-0.3.4/uniserde/bson_deserialize.py` & `uniserde-0.3.5/uniserde/bson_deserialize.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 from datetime import datetime, timezone
 from typing import *  # type: ignore
 
-from uniserde.objectid_proxy import ObjectId
-
 from . import caching_serdeserializer, case_convert, json_deserialize
 from .common import SerdeError
+from .objectid_proxy import ObjectId
 from .typedefs import Bsonable
 
 __all__ = [
     "from_bson",
 ]
 
 
 T = TypeVar("T")
 
 
 class BsonDeserializer(caching_serdeserializer.CachingSerDeserializer[Bsonable, Any]):
-    def _get_class_fields_and_handlers(
-        self, value_type: Type
-    ) -> Iterable[Tuple[str, str, Callable[[Bsonable, Type], Any]]]:
+    def _get_class_fields(self, value_type: Type) -> Iterable[Tuple[str, str, Type]]:
         for field_name_py, field_type in get_type_hints(value_type).items():
             if field_name_py == "id":
                 field_name_doc = "_id"
             else:
                 field_name_doc = case_convert.all_lower_to_camel_case(field_name_py)
 
             yield (
@@ -52,24 +49,39 @@
         float,
         bytes,
         str,
         ObjectId,
     }  # type: ignore
 
     _handler_cache = json_deserialize.JsonDeserializer._handler_cache.copy()  # type: ignore
-    _handler_cache[datetime] = _deserialize_datetime_from_datetime  # type: ignore
+    _handler_cache.update(
+        {
+            (True, datetime): _deserialize_datetime_from_datetime,
+            (False, datetime): _deserialize_datetime_from_datetime,
+        }  # type: ignore
+    )
+
     _override_method_name = "from_bson"
 
 
 def from_bson(
-    value: Any,
+    document: Any,
     as_type: Type[T],
     *,
     custom_deserializers: Dict[Type, Callable[[Bsonable], Any]] = {},
+    lazy: bool = False,
 ) -> T:
+    """
+    Deserialize an entire data class from BSON, by applying the field
+    deserializer to each field. Field names are converted from camel case.
+
+    Warning: The document may be modified in-place by this function!
+    """
+
     deserializer = BsonDeserializer(
         custom_deserializers={
             t: lambda v, _: cb(v) for t, cb in custom_deserializers.items()
-        }
+        },
+        lazy=lazy,
     )
 
-    return deserializer.process(value, as_type)
+    return deserializer.process(document, as_type)
```

### Comparing `uniserde-0.3.4/uniserde/caching_serdeserializer.py` & `uniserde-0.3.5/uniserde/caching_serdeserializer.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,69 +1,79 @@
 import enum
 import inspect
 from abc import ABC, abstractmethod
 from typing import *  # type: ignore
 
-import uniserde
-
-from . import case_convert, common, serde_class
+from . import case_convert, common, lazy_wrapper, serde_class
 from .common import SerdeError
 
 IN = TypeVar("IN")
 OUT = TypeVar("OUT")
 
 Handler: TypeAlias = Callable[["CachingSerDeserializer[IN, OUT]", IN, Type[OUT]], OUT]
 
 
 class CachingSerDeserializer(ABC, Generic[IN, OUT]):
+    """
+    Serializes/Deserializes objects, while caching any type-specific handlers it
+    creates. This provides massive speedups over constantly trying to figure out
+    what to do. (~3x compared to the old approach.)
+
+    Despite the name, currently only handles deserialization.
+    """
+
     # Types which are passed through without any processing. Must be defined by
     # subclasses.
     _passthrough_types: Set[Type[IN]]
 
-    # Maps types to handlers. This acts as cache for previously seen types. Must
-    # be defined by subclasses. (An empty dict is fine.)
-    _handler_cache: Dict[Type[IN], Handler]
+    # Maps (lazy, type) to handlers. This acts as cache for previously seen
+    # types.
+    #
+    # Must be defined by subclasses. (An empty dict is fine.)
+    _handler_cache: Dict[Tuple[bool, Type[IN]], Handler]
 
     # If a method of this name is present in a class (and it isn't the one
     # inherited from `Serde`) this will be used for handling that class, rather
     # than the default behavior.
     _override_method_name: str
 
     def __init_subclass__(cls) -> None:
         # Add handlers for all of the class's passthrough types
         def make_handler_from_passthrough_type(
             passthrough_type: Type,
         ) -> Handler:
             def result(self, value: IN, as_type: Type[OUT]) -> OUT:
-                if not isinstance(value, as_type) and not (
-                    isinstance(value, int) and as_type is float
+                if not isinstance(value, passthrough_type) and not (
+                    isinstance(value, int) and passthrough_type is float
                 ):
-                    raise SerdeError(f"Expected `{as_type}`, got `{value}`")
+                    raise SerdeError(f"Expected `{passthrough_type}`, got `{value}`")
 
                 return value  # type: ignore
 
             return result
 
         for typ in cls._passthrough_types:
-            cls._handler_cache[typ] = make_handler_from_passthrough_type(typ)
+            handler = make_handler_from_passthrough_type(typ)
+            cls._handler_cache[(True, typ)] = handler
+            cls._handler_cache[(False, typ)] = handler
 
     def __init__(
         self,
         *,
-        custom_deserializers: Dict[Type, Callable[[IN, Type[OUT]], OUT]] = {},
+        custom_deserializers: Dict[Type, Callable[[IN, Type[OUT]], OUT]],
+        lazy: bool,
     ):
         self._custom_deserializers = custom_deserializers
+        self._lazy = lazy
 
     @abstractmethod
-    def _get_class_fields_and_handlers(
-        self, value_type: Type
-    ) -> Iterable[Tuple[str, str, Callable[[IN, Type], Any]]]:
+    def _get_class_fields(self, value_type: Type) -> Iterable[Tuple[str, str, Type]]:
         """
-        Return a list of (python_name, json_name, handler) tuples for each
-        field in the class.
+        Return a tuple (python_name, json_name, type) for each field in the
+        class.
         """
         raise NotImplementedError()
 
     def process(self, value: IN, as_type: Type[OUT]) -> OUT:
         # Special case: rapidly handle simple passthrough types to increase
         # performance
         if as_type in self._passthrough_types:
@@ -79,36 +89,36 @@
         return handler(self, value, as_type)
 
     def _get_handler(
         self,
         value_type: Type,
     ) -> Handler:
         # Prepare the key for the cache lookup
-        key = get_origin(value_type)
-        if key is None:
-            key = value_type
+        type_key = get_origin(value_type)
+        if type_key is None:
+            type_key = value_type
 
         # Custom handlers take precedence
         try:
-            custom_handler = self._custom_deserializers[key]
+            custom_handler = self._custom_deserializers[type_key]
         except KeyError:
             pass
         else:
             return lambda self, value, as_type: custom_handler(value, as_type)
 
         # Use a cached handler if possible
         try:
-            return self._handler_cache[key]
+            return self._handler_cache[(self._lazy, type_key)]
         except KeyError:
             pass
 
         # Otherwise create the appropriate handler and cache it for next time
         assert inspect.isclass(value_type), value_type
         handler = self._create_class_handler(value_type)
-        self._handler_cache[key] = handler
+        self._handler_cache[(self._lazy, type_key)] = handler
 
         return handler
 
     def _create_class_handler(
         self,
         value_type: Type,
     ) -> Handler:
@@ -203,36 +213,57 @@
                     raise SerdeError(
                         f"Encountered invalid type tag `{type_tag}`"
                     ) from None
 
                 # Delegate to that class's handler
                 return child_class_handler(self, value, child_class)
 
+            # TODO: The generated handler works for all subclasses, but will
+            #       only be cached for the one class that has just been
+            #       requested. Consider explicitly caching it for all classes.
+
             return handle_as_child
 
         # Case: Regular old class
         return self._create_fieldwise_class_handler(value_type)
 
     def _create_fieldwise_class_handler(self, value_type: Type) -> Handler:
+        # Lazy?
+        if self._lazy and lazy_wrapper.can_create_lazy_instance(value_type):
+
+            def _handler(self, value, _type):
+                return lazy_wrapper.create_lazy_instance(
+                    value,
+                    self,
+                    value_type,
+                )
+
+            return _handler
+
+        # Eager
         handler = FieldwiseClassHandler()
 
-        for py_name, doc_name, field_type in self._get_class_fields_and_handlers(
-            value_type
-        ):
+        for py_name, doc_name, field_type in self._get_class_fields(value_type):
             handler.add_field(
                 py_name,
                 doc_name,
                 field_type,
                 self._get_handler(field_type),
             )
 
         return handler
 
 
 class FieldwiseClassHandler:
+    """
+    Deserializes a class, field by field. The fields and their handlers are
+    already passed in the constructor to avoid having to recompute them for each
+    instance.
+    """
+
     fields: List[Tuple[str, str, Type, Handler]]
 
     def __init__(self):
         self.fields = []
 
     def add_field(
         self,
@@ -247,27 +278,27 @@
         self,
         calling_ser_deserializer: CachingSerDeserializer,
         raw: Any,
         value_type: Type,
     ) -> Any:
         # Make sure the raw value is a dict
         if not isinstance(raw, dict):
-            raise uniserde.SerdeError(f"Expected object, got `{raw!r}`")
+            raise SerdeError(f"Expected object, got `{raw!r}`")
 
         # Create an instance of the class
         result = object.__new__(value_type)
         result_dict = vars(result)
 
         # Handle all fields
         for py_name, doc_name, field_type, handler in self.fields:
             # Get the raw value
             try:
                 raw_value = raw.pop(doc_name)
             except KeyError:
-                raise uniserde.SerdeError(f"Missing field `{doc_name!r}`") from None
+                raise SerdeError(f"Missing field `{doc_name!r}`") from None
 
             # Process it
             processed_value = handler(calling_ser_deserializer, raw_value, field_type)
 
             # Store it
             result_dict[py_name] = processed_value
```

### Comparing `uniserde-0.3.4/uniserde/case_convert.py` & `uniserde-0.3.5/uniserde/case_convert.py`

 * *Files identical despite different names*

### Comparing `uniserde-0.3.4/uniserde/common.py` & `uniserde-0.3.5/uniserde/common.py`

 * *Files identical despite different names*

### Comparing `uniserde-0.3.4/uniserde/json_deserialize.py` & `uniserde-0.3.5/uniserde/json_deserialize.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,30 +2,28 @@
 from datetime import datetime, timedelta
 from typing import *  # type: ignore
 
 import dateutil.parser
 
 from . import caching_serdeserializer, case_convert
 from .common import SerdeError
+from .json_serialize import Jsonable
 from .objectid_proxy import ObjectId
-from .serde_json import Jsonable
 from .typedefs import Jsonable
 
 __all__ = [
     "from_json",
 ]
 
 
 T = TypeVar("T")
 
 
 class JsonDeserializer(caching_serdeserializer.CachingSerDeserializer[Jsonable, Any]):
-    def _get_class_fields_and_handlers(
-        self, value_type: Type
-    ) -> Iterable[Tuple[str, str, Callable[[Jsonable, Type], Any]]]:
+    def _get_class_fields(self, value_type: Type) -> Iterable[Tuple[str, str, Type]]:
         for field_name_py, field_type in get_type_hints(value_type).items():
             yield (
                 field_name_py,
                 case_convert.all_lower_to_camel_case(field_name_py),
                 field_type,
             )
 
@@ -180,36 +178,56 @@
         bool,
         int,
         float,
         str,
     }  # type: ignore
 
     _handler_cache = {
-        bytes: _deserialize_bytes_from_str,
-        datetime: _deserialize_datetime_from_str,
-        timedelta: _deserialize_timedelta_from_float,
-        tuple: _deserialize_tuple_from_list,
-        list: _deserialize_list_from_list,
-        set: _deserialize_set_from_list,
-        dict: _deserialize_dict_from_dict,
-        Union: _deserialize_optional,
-        Any: _deserialize_any,
-        ObjectId: _deserialize_object_id_from_str,
-        Literal: _deserialize_literal_as_is,
+        (True, bytes): _deserialize_bytes_from_str,
+        (False, bytes): _deserialize_bytes_from_str,
+        (True, datetime): _deserialize_datetime_from_str,
+        (False, datetime): _deserialize_datetime_from_str,
+        (True, timedelta): _deserialize_timedelta_from_float,
+        (False, timedelta): _deserialize_timedelta_from_float,
+        (True, tuple): _deserialize_tuple_from_list,
+        (False, tuple): _deserialize_tuple_from_list,
+        (True, list): _deserialize_list_from_list,
+        (False, list): _deserialize_list_from_list,
+        (True, set): _deserialize_set_from_list,
+        (False, set): _deserialize_set_from_list,
+        (True, dict): _deserialize_dict_from_dict,
+        (False, dict): _deserialize_dict_from_dict,
+        (True, Union): _deserialize_optional,
+        (False, Union): _deserialize_optional,
+        (True, Any): _deserialize_any,
+        (False, Any): _deserialize_any,
+        (True, ObjectId): _deserialize_object_id_from_str,
+        (False, ObjectId): _deserialize_object_id_from_str,
+        (True, Literal): _deserialize_literal_as_is,
+        (False, Literal): _deserialize_literal_as_is,
     }  # type: ignore
 
     _override_method_name = "from_json"
 
 
 def from_json(
-    value: Any,
+    document: Any,
     as_type: Type[T],
     *,
     custom_deserializers: Dict[Type, Callable[[Jsonable], Any]] = {},
+    lazy: bool = False,
 ) -> T:
+    """
+    Deserialize an entire class from JSON, by applying the field deserializer to
+    each field. Field names are converted from camel case.
+
+    Warning: The document may be modified in-place by this function!
+    """
+
     deserializer = JsonDeserializer(
         custom_deserializers={
             t: lambda v, _: cb(v) for t, cb in custom_deserializers.items()
-        }
+        },
+        lazy=lazy,
     )
 
-    return deserializer.process(value, as_type)
+    return deserializer.process(document, as_type)
```

### Comparing `uniserde-0.3.4/uniserde/objectid_proxy.py` & `uniserde-0.3.5/uniserde/objectid_proxy.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 """
-This module provides the `ObjectId` class. If the `bson` module is installed, it
+This module provides the `ObjectId` class. If the `bson` module is available, it
 is imported from there. Otherwise it falls back to a class with an identical,
 albeit incomplete, interface.
+
+uniserde expects the `bson` package provided by `pymongo`, NOT the one called
+`bson` on pypi. However, both seem to work fine.
 """
 
 import binascii
 import os
 import struct
 import time
 from typing import *  # type: ignore
```

### Comparing `uniserde-0.3.4/uniserde/schema_mongodb.py` & `uniserde-0.3.5/uniserde/schema_mongodb.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,20 +56,32 @@
 
     def _make_schema_datetime_to_datetime(self, value_type: Type) -> Jsonable:
         return {"bsonType": "date"}
 
     def _make_schema_timedelta_to_float(self, value_type: Type) -> Jsonable:
         return {"bsonType": ["int", "long", "double"]}
 
+    def _make_schema_tuple_to_list(self, value_type: Type) -> Jsonable:
+        return {
+            "type": "array",
+            "items": [self.process(subtype) for subtype in get_args(value_type)],
+        }
+
     def _make_schema_list_to_list(self, value_type: Type) -> Jsonable:
         return {
             "type": "array",
             "items": self.process(get_args(value_type)[0]),
         }
 
+    def _make_schema_set_to_list(self, value_type: Type) -> Jsonable:
+        return {
+            "type": "array",
+            "items": self.process(get_args(value_type)[0]),
+        }
+
     def _make_schema_dict_to_dict(self, value_type: Type) -> Jsonable:
         subtypes = get_args(value_type)
         assert subtypes[0] is str, value_type
 
         return {
             "type": "object",
             "items": self.process(subtypes[1]),
@@ -143,26 +155,14 @@
             return sub_schemas[0]
 
         return {"anyOf": sub_schemas}
 
     def _make_schema_any(self, value_type: Type) -> Jsonable:
         return {}
 
-    def _make_schema_tuple_to_list(self, value_type: Type) -> Jsonable:
-        return {
-            "type": "array",
-            "items": [self.process(subtype) for subtype in get_args(value_type)],
-        }
-
-    def _make_schema_set_to_list(self, value_type: Type) -> Jsonable:
-        return {
-            "type": "array",
-            "items": self.process(get_args(value_type)[0]),
-        }
-
     def _create_class_schema_ignore_serialize_as_child(
         self, value_type: Type
     ) -> Jsonable:
         doc_field_names = []
         doc_properties = {}
         result = {
             "type": "object",
@@ -272,9 +272,14 @@
 
 
 def as_mongodb_schema(
     value_type: Type,
     *,
     custom_handlers: Dict[Type, Callable[[Type], Jsonable]] = {},
 ) -> Any:
+    """
+    Return a MongoDB schema for this class. The schema matches values resulting
+    from `as_bson`.
+    """
+
     builder = MongoDbSchemaBuilder(custom_handlers)
     return builder.process(value_type)
```

### Comparing `uniserde-0.3.4/uniserde/serde_bson.py` & `uniserde-0.3.5/uniserde/bson_serialize.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from datetime import datetime
 from typing import *  # type: ignore
 
-from . import serde_class, serde_json
+from . import json_serialize, serde_class
 from .common import *
 from .objectid_proxy import ObjectId
 from .typedefs import Bsonable
 
 __all__ = [
     "as_bson",
 ]
@@ -43,15 +43,15 @@
 
 
 def serialize_class(
     value: Any,
     value_type: Type,
     recur: Recur,
 ) -> Dict[str, Any]:
-    result = serde_json.serialize_class(value, value_type, recur)
+    result = json_serialize.serialize_class(value, value_type, recur)
 
     # Case: The class has a custom serialization method
     try:
         override_method = getattr(value, "as_bson")
     except AttributeError:
         pass
     else:
@@ -64,15 +64,15 @@
             result["_id"] = result.pop("id")
         except KeyError:
             pass
 
     return result
 
 
-BSON_SERIALIZERS: Dict[Type, Serializer] = serde_json.JSON_SERIALIZERS.copy()
+BSON_SERIALIZERS: Dict[Type, Serializer] = json_serialize.JSON_SERIALIZERS.copy()
 BSON_SERIALIZERS.update(
     {
         bytes: serialize_bytes_to_bytes,
         datetime: serialize_datetime_to_datetime,
         ObjectId: serialize_object_id_to_object_id,
     }
 )
```

### Comparing `uniserde-0.3.4/uniserde/serde_class.py` & `uniserde-0.3.5/uniserde/serde_class.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,46 +42,59 @@
             custom_serializers=custom_serializers,
         )  # type: ignore
 
     @classmethod
     def from_bson(
         cls: Type[T],
         document: Dict[str, Any],
+        *,
         custom_deserializers: Dict[Type, Callable[[Any], Any]] = {},
+        lazy: bool = False,
     ) -> T:
         """
         Deserialize an entire data class from BSON, by applying the field
-        deserializer to each field. Field names are converted to camel case. The
-        value may be modified by this function!
+        deserializer to each field. Field names are converted from camel case.
+
+        Warning: The document may be modified in-place by this function!
         """
         return uniserde.from_bson(
             document,
             as_type=cls,
             custom_deserializers=custom_deserializers,
+            lazy=lazy,
         )
 
     @classmethod
     def from_json(
         cls: Type[T],
         document: Dict[str, Any],
+        *,
         custom_deserializers: Dict[Type, Callable[[Any], Any]] = {},
+        lazy: bool = False,
     ) -> T:
         """
-        Deserialize an entire data class from JSON, by applying the field
-        deserializer to each field. Field names are converted to camel case. The
-        value may be modified by this function!
+        Deserialize an entire class from JSON, by applying the field
+        deserializer to each field. Field names are converted from camel case.
+
+        Warning: The document may be modified in-place by this function!
         """
         return uniserde.from_json(
             document,
             as_type=cls,
             custom_deserializers=custom_deserializers,
+            lazy=lazy,
         )
 
     @classmethod
     def as_mongodb_schema(
         cls,
+        *,
         custom_handlers: Dict[Type, Callable[[Any], Any]] = {},
     ) -> Any:
+        """
+        Return a MongoDB schema for this class. The schema matches values
+        resulting from `as_bson`.
+        """
         return uniserde.as_mongodb_schema(
             cls,
             custom_handlers=custom_handlers,
         )
```

### Comparing `uniserde-0.3.4/uniserde/serde_json.py` & `uniserde-0.3.5/uniserde/json_serialize.py`

 * *Files identical despite different names*

### Comparing `uniserde-0.3.4/PKG-INFO` & `uniserde-0.3.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uniserde
-Version: 0.3.4
+Version: 0.3.5
 Summary: Convention based, effortless serialization and deserialization
 Home-page: https://gitlab.com/Vivern/uniserde
 License: MIT
 Author: Jakob Pinterits
 Author-email: jakob.pinterits@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -19,15 +19,15 @@
 Description-Content-Type: text/markdown
 
 # Convention based, effortless serialization and deserialization
 
 `uniserde` can convert Python classes to/from JSON and BSON without any input
 from your side. Simply define the classes, and the library does the rest.
 
-Simply define your types as classes with type annotations, and call one of the
+Define your types as classes with type annotations, and call one of `uniserde`'s
 serialization/deserialization functions:
 
 ```py
 from uniserde import Serde
 from datetime import datetime, timezone
 from dataclasses import dataclass
 from .objectid_proxy import ObjectId
@@ -60,26 +60,25 @@
 ```
 
 You can easily convert this to a string using Python's built-in `json` module if
 that's what you need.
 
 ## API
 
-The API is intentionally simple. Functions/Classes you might be interested in
-are:
+The API is extremely simple. Functions/Classes you might be interested in are:
 
 - `as_json`, `as_bson`
 
   Given a class with type annotations, these create a JSON/BSON like dictionary.
   You can feed those into functions like `json.dump`, or use them as is.
 
 - `from_json`, `from_bson`
 
-  Given a JSON/BSON like dictionary, these will instantiate the corresponding
-  Python class. Raise `SerdeError` if the values are invalid.
+  Given a JSON/BSON like dictionary and Python type, these will instantiate the
+  corresponding Python class. Raise `SerdeError` if the values are invalid.
 
 - `Serde` is a helper class you can optionally apply to your models. It adds the
   convenience functions `as_json`, `as_bson`, `from_json`, and `from_bson`
   directly to the models.
 
 - Sometimes a class simply acts as a type-safe base, but you really just want to
   serialize the children of that class. In that case you can decorate the class
@@ -89,65 +88,85 @@
 - `as_mongodb_schema` automatically creates JSON schemas compatible with MongoDB
   from models
 
 - Custom serialization / deserialization can be achieved by inheriting from the
   `Serde` class and overriding the `as_json`, `as_bson`, `from_json`,
   `from_bson` and/or `as_mongodb_schema` methods.
 
+## Lazy Deserialization
+
+Normally, serialization happens all at once: You tell `uniserde` to create a
+class instance from a JSON, `uniserde` processes all of the fields and returns
+the finished class.
+
+This works great, but can be wasteful if you are working with large documents
+and only need to access few fields. To help with this, you can pass `lazy=True`
+when deserializing any object. `uniserde` will then hold off deserializing
+fields until they are accessed for the first time, saving precious processing
+time.
+
+**A word of caution:** Data is validated as it is deserialized. Since lazy
+deserialization defers work until the data is accessed, this means any data you
+don't access also won't be validated. Thus, lazy serialization can be a very
+powerful tool for speeding up interactions with large objects, but you should
+only use when you are absolutely certain the data is correct. (For example
+because you have just fetched the object from your own, trusted, database.)
+
 ## Types & Conventions
 
 The library tries to stick to the naming conventions used by the target formats:
 
-- names in JSON are written in lowerCamelCase, as is commonly done in
-  JavaScript
+- names in JSON are written in _lowerCamelCase_, as is convention in JavaScript
 - BSON uses the same conventions as JSON
-- Python class names are expected to be written in UpperCamelCase
-- Python enum values must be in ALL_UPPER_CASE
+- Python class names must be in _UpperCamelCase_
+- Python fields must be in _all_lower_case_
+- Python enum values must be in _ALL_UPPER_CASE_
 
 ### JSON
 
-| Python           | JSON              | Notes                                                                                                                 |
-| ---------------- | ----------------- | --------------------------------------------------------------------------------------------------------------------  |
-| `bool`           | `bool`            |                                                                                                                       |
-| `int`            | `float`           |                                                                                                                       |
-| `float`          | `float`           |                                                                                                                       |
-| `str`            | `str`             |                                                                                                                       |
-| `Tuple`          | `list`            |                                                                                                                       |
-| `List`           | `list`            |                                                                                                                       |
-| `Set`            | `list`            |                                                                                                                       |
-| `Optional`       | value or `None`   |                                                                                                                       |
-| `Any`            | as-is             |                                                                                                                       |
-| `Literal[str]`   | `str`             |                                                                                                                       |
-| `enum.Enum`      | `str`             | Enum values are mapped to their name (NOT value!)                                                                     |
-| `enum.Flag`      | `List[str]`       | Each flag is encoded the same way a single `Enum` would.                                                              |
-| custom class     | `dict`            | Each attribute is stored as key, in lowerCamelCase. If marked with `as_child`, an additional `type` field is added.   |
-| `bytes`          | `str`             | base64 encoded                                                                                                        |
-| `datetime`       | `str`             | as ISO 8601 - with timezone. Naïve datetimes are intentionally not supported. Do yourself a favor and don't use them. |
-| `timedelta`      | `float`           | duration, in seconds                                                                                                  |
-| `Dict[str, ...]` | `dict`            |                                                                                                                       |
-| `bson.ObjectId`  | `str`             |                                                                                                                       |
+| Python               | JSON              | Notes                                                                                                                 |
+| -------------------- | ----------------- | --------------------------------------------------------------------------------------------------------------------- |
+| `bool`               | `bool`            |                                                                                                                       |
+| `int`                | `float`           |                                                                                                                       |
+| `float`              | `float`           |                                                                                                                       |
+| `str`                | `str`             |                                                                                                                       |
+| `Tuple`              | `list`            |                                                                                                                       |
+| `List`               | `list`            |                                                                                                                       |
+| `Set`                | `list`            |                                                                                                                       |
+| `Optional`           | value or `None`   |                                                                                                                       |
+| `Any`                | as-is             |                                                                                                                       |
+| `Literal[str]`       | `str`             |                                                                                                                       |
+| `enum.Enum`          | `str`             | Enum values are mapped to their _name_ (**NOT value!**)                                                               |
+| `enum.Flag`          | `List[str]`       | Each flag is encoded the same way a regular `enum.Enum` value would.                                                  |
+| custom class         | `dict`            | Each attribute is stored as key, in _lowerCamelCase_. If marked with `as_child`, an additional `type` field is added. |
+| `bytes`              | `str`             | base64 encoded                                                                                                        |
+| `datttime.datetime`  | `str`             | as ISO 8601 - with timezone. Naïve datetimes are intentionally not supported. Do yourself a favor and don't use them. |
+| `datetime.timedelta` | `float`           | duration, in seconds                                                                                                  |
+| `Dict[str, ...]`     | `dict`            |                                                                                                                       |
+| `bson.ObjectId`      | `str`             |                                                                                                                       |
 
 ### BSON
 
 BSON uses the same conventions as JSON, with just a few changes
 
-| Python          | BSON            | Notes                                                                                                                                                 |
-| --------------- | --------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------- |
-| custom class    | `dict`          | Same as JSON, but any fields named `id` are renamed to `_id` to match MongoDB. (Exception: if an `_id` field is already present, `id` is not renamed) |
-| `bytes`         | `bytes`         |                                                                                                                                                       |
-| `datetime`      | `datetime`      | Serialization requires a timezone be set. Deserialization imputes UTC, to match MongoDB convention.                                                   |
-| `bson.ObjectId` | `bson.ObjectId` |                                                                                                                                                       |
+| Python              | BSON                | Notes                                                                                    |
+| ------------------- | ------------------- | ---------------------------------------------------------------------------------------- |
+| custom class        | `dict`              | Same as JSON, but any fields named `id` are renamed to `_id` to match MongoDB.           |
+| `bytes`             | `bytes`             |                                                                                          |
+| `datetime.datetime` | `datetime.datetime` | Serialization requires a timezone be set. Deserialization imputes UTC, to match MongoDB. |
+| `bson.ObjectId`     | `bson.ObjectId`     |                                                                                          |
 
-## Schema Generation
+## MongoDB Schema Generation
 
 If you are working with MongoDB you will come to appreciate the automatic schema
 generation. Calling `uniserde.as_mongodb_schema` on any supported class will return
 a MongoDB compatible JSON schema without hassle.
 
-For example `uniserde.as_mongodb_schema(Person)` with the `Person` class from above:
+For example, here's the result of `uniserde.as_mongodb_schema(Person)` with the
+`Person` class above:
 
 ```py
 {
     'type': 'object',
     'properties': {
         '_id': {
             'bsonType': 'objectId'
@@ -167,21 +186,24 @@
     ]
 }
 ```
 
 ## TODO
 
 - Support for `Union` is currently very limited. Really only `Optional` is
-  supported (which maps to `Union`)
+  supported (which Python internally maps to `Union`)
 - `Literal` currently only supports strings
-- Make support for BSON optional, so the library doesn't depend on MongoDB
 - Extend `as_child`, to allow marking some classes as abstract. i.e. their
   parents/children can be serialized, but not those classes themselves
 - Being able to specify additional limitations to fields would be nice:
   - must match regex
   - minimum / maximum
   - custom validation functions
-- more Unit tests
+- more Unit tests (custom de-serializers!?)
 - Add more examples to the README
   - show custom serializers/deserializers
   - recommended usage
+- regression tracking
+- calling `uniserde.serialize` on nonclasses causes problems, because the
+  serialization `as_type` is guessed incorrectly. e.g. `[1, 2, 3]` will be
+  incorrectly serialized as `list` rather than `List[int]`.
```

