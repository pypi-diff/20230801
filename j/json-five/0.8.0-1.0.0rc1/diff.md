# Comparing `tmp/json-five-0.8.0.tar.gz` & `tmp/json-five-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json-five-0.8.0.tar", last modified: Mon Dec  5 18:50:23 2022, max compression
+gzip compressed data, was "json-five-1.0.0rc1.tar", last modified: Tue Aug  1 04:50:10 2023, max compression
```

## Comparing `json-five-0.8.0.tar` & `json-five-1.0.0rc1.tar`

### file list

```diff
@@ -1,21 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-05 18:50:23.440644 json-five-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2022-12-05 18:50:19.000000 json-five-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       34 2022-12-05 18:50:19.000000 json-five-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     2380 2022-12-05 18:50:23.440644 json-five-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1760 2022-12-05 18:50:19.000000 json-five-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-05 18:50:23.436643 json-five-0.8.0/json5/
--rw-r--r--   0 runner    (1001) docker     (122)      100 2022-12-05 18:50:19.000000 json-five-0.8.0/json5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10063 2022-12-05 18:50:19.000000 json-five-0.8.0/json5/dumper.py
--rw-r--r--   0 runner    (1001) docker     (122)     4788 2022-12-05 18:50:19.000000 json-five-0.8.0/json5/loader.py
--rw-r--r--   0 runner    (1001) docker     (122)     5484 2022-12-05 18:50:19.000000 json-five-0.8.0/json5/model.py
--rw-r--r--   0 runner    (1001) docker     (122)    15488 2022-12-05 18:50:19.000000 json-five-0.8.0/json5/parser.py
--rw-r--r--   0 runner    (1001) docker     (122)     2964 2022-12-05 18:50:19.000000 json-five-0.8.0/json5/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (122)     1058 2022-12-05 18:50:19.000000 json-five-0.8.0/json5/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-05 18:50:23.440644 json-five-0.8.0/json_five.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2380 2022-12-05 18:50:23.000000 json-five-0.8.0/json_five.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      327 2022-12-05 18:50:23.000000 json-five-0.8.0/json_five.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-05 18:50:23.000000 json-five-0.8.0/json_five.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2022-12-05 18:50:23.000000 json-five-0.8.0/json_five.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2022-12-05 18:50:23.000000 json-five-0.8.0/json_five.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       74 2022-12-05 18:50:23.440644 json-five-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      886 2022-12-05 18:50:19.000000 json-five-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:50:10.111713 json-five-1.0.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-01 04:49:59.000000 json-five-1.0.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-01 04:49:59.000000 json-five-1.0.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-08-01 04:50:10.111713 json-five-1.0.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-08-01 04:49:59.000000 json-five-1.0.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:50:10.111713 json-five-1.0.0rc1/json5/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-08-01 04:49:59.000000 json-five-1.0.0rc1/json5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11263 2023-08-01 04:49:59.000000 json-five-1.0.0rc1/json5/dumper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9195 2023-08-01 04:49:59.000000 json-five-1.0.0rc1/json5/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7768 2023-08-01 04:49:59.000000 json-five-1.0.0rc1/json5/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21269 2023-08-01 04:49:59.000000 json-five-1.0.0rc1/json5/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 04:49:59.000000 json-five-1.0.0rc1/json5/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-08-01 04:49:59.000000 json-five-1.0.0rc1/json5/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-08-01 04:49:59.000000 json-five-1.0.0rc1/json5/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:50:10.111713 json-five-1.0.0rc1/json_five.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-08-01 04:50:10.000000 json-five-1.0.0rc1/json_five.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-08-01 04:50:10.000000 json-five-1.0.0rc1/json_five.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 04:50:10.000000 json-five-1.0.0rc1/json_five.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-01 04:50:10.000000 json-five-1.0.0rc1/json_five.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-01 04:50:10.000000 json-five-1.0.0rc1/json_five.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-08-01 04:50:10.111713 json-five-1.0.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 04:49:59.000000 json-five-1.0.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:50:10.111713 json-five-1.0.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7360 2023-08-01 04:49:59.000000 json-five-1.0.0rc1/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-08-01 04:49:59.000000 json-five-1.0.0rc1/tests/test_json5_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8082 2023-08-01 04:49:59.000000 json-five-1.0.0rc1/tests/test_json5_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-08-01 04:49:59.000000 json-five-1.0.0rc1/tests/test_json5_official_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-08-01 04:49:59.000000 json-five-1.0.0rc1/tests/test_json_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-08-01 04:49:59.000000 json-five-1.0.0rc1/tests/test_loads_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-08-01 04:49:59.000000 json-five-1.0.0rc1/tests/test_model_loader_dumper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-08-01 04:49:59.000000 json-five-1.0.0rc1/tests/test_modelizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-08-01 04:49:59.000000 json-five-1.0.0rc1/tests/test_regressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-08-01 04:49:59.000000 json-five-1.0.0rc1/tests/test_roundtrip.py
```

### Comparing `json-five-0.8.0/LICENSE` & `json-five-1.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `json-five-0.8.0/PKG-INFO` & `json-five-1.0.0rc1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: json-five
-Version: 0.8.0
+Version: 1.0.0rc1
 Summary: A JSON5 parser that, among other features, supports round-trip preservation of comments
 Home-page: https://github.com/spyoungtech/json-five
 Author: Spencer Phillip Young
 Author-email: spencer.young@spyoung.com
 License: Apache
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # json-five
 
 JSON5 for Python
```

### Comparing `json-five-0.8.0/README.md` & `json-five-1.0.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `json-five-0.8.0/json5/dumper.py` & `json-five-1.0.0rc1/json5/dumper.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,61 +1,76 @@
+from __future__ import annotations
+
+import io
+import json
+import math
+import typing
+from abc import abstractmethod
+from typing import Any
+
 from .loader import JsonIdentifier
 from .utils import singledispatchmethod
 from json5.model import *
-from collections import UserDict
-import json
-import io
 
-class Environment(UserDict):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.outfile = io.StringIO()
-        self.indent_level = 0
-        self.indent = 0
 
+class Environment:
+    def __init__(self) -> None:
+        self.outfile: typing.TextIO = io.StringIO()
+        self.indent_level: int = 0
+        self.indent: int = 0
 
-    def write(self, s, indent=None):
+    def write(self, s: str, indent: int | None = None) -> None:
         if indent is None:
             indent = self.indent_level
         whitespace = ' ' * self.indent * indent
         s = f'{whitespace}{s}'
         self.outfile.write(s)
 
 
-def dump(obj, f, **kwargs):
+def dump(obj: Any, f: typing.TextIO, **kwargs: Any) -> int:
     text = dumps(obj, **kwargs)
     return f.write(text)
 
 
-def dumps(obj, dumper=None, indent=0):
+def dumps(obj: Any, dumper: BaseDumper | None = None, indent: int = 0) -> str:
     env = Environment()
     env.indent = indent
     if dumper is None:
         dumper = DefaultDumper(env=env)
-    model = dumper.dump(obj)
+    dumper.dump(obj)
     dumper.env.outfile.seek(0)
-    return dumper.env.outfile.read()
+    ret: str = dumper.env.outfile.read()
+    return ret
 
-class DefaultDumper:
-    """
-    Dump Python objects to a JSON string
-    """
-    def __init__(self, env=None):
+
+class BaseDumper:
+    def __init__(self, env: Environment | None = None):
         if env is None:
             env = Environment()
         self.env = env
 
     @singledispatchmethod
-    def dump(self, obj):
+    @abstractmethod
+    def dump(self, obj: Any) -> Any:
+        return NotImplemented
+
+
+class DefaultDumper(BaseDumper):
+    """
+    Dump Python objects to a JSON string
+    """
+
+    @singledispatchmethod
+    def dump(self, obj: Any) -> Any:
         raise NotImplementedError(f"Cannot dump node {repr(obj)}")
 
     to_json = dump.register
 
     @to_json(dict)
-    def dict_to_json(self, d):
+    def dict_to_json(self, d: dict[Any, Any]) -> Any:
         self.env.write('{', indent=0)
         if self.env.indent:
             self.env.write('\n')
             self.env.indent_level += 1
         for index, (key, value) in enumerate(d.items(), start=1):
             if self.env.indent:
                 self.env.write('')
@@ -73,119 +88,118 @@
         if self.env.indent:
             self.env.indent_level -= 1
             self.env.write('\n')
             self.env.write('}')
         else:
             self.env.write('}', indent=0)
 
-
     @to_json(int)
-    def int_to_json(self, i):
+    def int_to_json(self, i: int) -> Any:
         self.env.write(str(i), indent=0)
 
     @to_json(JsonIdentifier)
-    def identifier_to_json(self, s):
+    def identifier_to_json(self, s: JsonIdentifier) -> Any:
         self.env.write(s, indent=0)
 
     @to_json(str)
-    def str_to_json(self, s):
+    def str_to_json(self, s: str) -> Any:
         self.env.write(json.dumps(s), indent=0)
 
-
     @to_json(list)
-    def list_to_json(self, l):
+    def list_to_json(self, the_list: list[Any]) -> Any:
         self.env.write('[', indent=0)
         if self.env.indent:
             self.env.indent_level += 1
             self.env.write('\n', indent=0)
-        list_length = len(l)
-        for index, item in enumerate(l, start=1):
+        list_length = len(the_list)
+        for index, item in enumerate(the_list, start=1):
             if self.env.indent:
                 self.env.write('')
             self.dump(item)
             if index != list_length:
                 if self.env.indent:
                     self.env.write(',', indent=0)
                 else:
                     self.env.write(', ', indent=0)
             if self.env.indent:
                 self.env.write('\n', indent=0)
         if self.env.indent:
             self.env.indent_level -= 1
         self.env.write(']')
 
-
     @to_json(float)
-    def float_to_json(self, f):
+    def float_to_json(self, f: float) -> Any:
         if f == math.inf:
             self.env.write('Infinity', indent=0)
         elif f == -math.inf:
             self.env.write('-Infinity', indent=0)
         elif f is math.nan:
             self.env.write('NaN', indent=0)
         else:
             self.env.write(str(f), indent=0)
 
     @to_json(bool)
-    def bool_to_json(self, b):
+    def bool_to_json(self, b: bool) -> Any:
         self.env.write(str(b).lower(), indent=0)
 
     @to_json(type(None))
-    def none_to_json(self, _):
+    def none_to_json(self, _: Any) -> Any:
         self.env.write('null', indent=0)
 
+
 class ModelDumper:
     """
     Dump a model to a JSON string
     """
-    def __init__(self, env=None):
+
+    def __init__(self, env: Environment | None = None):
         #  any provided environment is ignored
         self.env = Environment()
 
-    def process_wsc_before(self, node):
+    def process_wsc_before(self, node: Node) -> None:
         for wsc in node.wsc_before:
             if isinstance(wsc, Comment):
                 self.dump(wsc)
             elif isinstance(wsc, str):
                 self.env.write(wsc)
             else:
                 raise ValueError(f"Did not expect {type(node)}")
 
-    def process_wsc_after(self, node):
+    def process_wsc_after(self, node: Node) -> None:
         for wsc in node.wsc_after:
             if isinstance(wsc, Comment):
                 self.dump(wsc)
             elif isinstance(wsc, str):
                 self.env.write(wsc)
             else:
                 raise ValueError(f"Did not expect {type(wsc)}")
 
-    def process_leading_wsc(self, node):
+    def process_leading_wsc(self, node: JSONObject | JSONArray) -> None:
         for wsc in node.leading_wsc:
             if isinstance(wsc, Comment):
                 self.dump(wsc)
             elif isinstance(wsc, str):
                 self.env.write(wsc)
             else:
                 raise ValueError(f"Did not expect {type(wsc)}")
 
     @singledispatchmethod
-    def dump(self, node):
+    def dump(self, node: Node) -> Any:
         raise NotImplementedError('foo')
 
     to_json = dump.register
 
     @to_json(JSONText)
-    def json_model_to_json(self, node):
+    def json_model_to_json(self, node: JSONText) -> Any:
         self.process_wsc_before(node)
         self.dump(node.value)
         self.process_wsc_after(node)
 
     @to_json(JSONObject)
-    def json_object_to_json(self, node):
+    def json_object_to_json(self, node: JSONObject) -> Any:
         self.process_wsc_before(node)
         self.env.write('{')
         if node.leading_wsc:
             self.process_leading_wsc(node)
         num_pairs = len(node.key_value_pairs)
         for index, kvp in enumerate(node.key_value_pairs, start=1):
             self.dump(kvp.key)
@@ -195,162 +209,163 @@
                 self.env.write(',')
         if node.trailing_comma:
             self.dump(node.trailing_comma)
         self.env.write('}')
         self.process_wsc_after(node)
 
     @to_json(JSONArray)
-    def json_array_to_json(self, node):
+    def json_array_to_json(self, node: JSONArray) -> Any:
         self.process_wsc_before(node)
         self.env.write('[')
         if node.leading_wsc:
             self.process_leading_wsc(node)
         for index, value in enumerate(node.values, start=1):
             self.dump(value)
             if index != len(node.values):
                 self.env.write(',')
         if node.trailing_comma:
             self.dump(node.trailing_comma)
         self.env.write(']')
         self.process_wsc_after(node)
 
     @to_json(Identifier)
-    def identifier_to_json(self, node):
+    def identifier_to_json(self, node: Identifier) -> Any:
         self.process_wsc_before(node)
         self.env.write(node.raw_value)
         self.process_wsc_after(node)
 
     @to_json(Integer)
-    def integer_to_json(self, node):
+    def integer_to_json(self, node: Integer) -> Any:
         self.process_wsc_before(node)
         self.env.write(node.raw_value)
         self.process_wsc_after(node)
 
     @to_json(Float)
-    def float_to_json(self, node):
+    def float_to_json(self, node: Float) -> Any:
         self.process_wsc_before(node)
         self.env.write(node.raw_value)
         self.process_wsc_after(node)
 
     @to_json(UnaryOp)
-    def unary_to_json(self, node):
+    def unary_to_json(self, node: UnaryOp) -> Any:
         self.process_wsc_before(node)
         self.env.write(node.op)
         self.dump(node.value)
         self.process_wsc_after(node)
 
     @to_json(String)
-    def string_to_json(self, node):
+    def string_to_json(self, node: SingleQuotedString | DoubleQuotedString) -> Any:
         self.process_wsc_before(node)
         self.env.write(node.raw_value)  # The original value, including any escape sequences or line continuations
         self.process_wsc_after(node)
 
     @to_json(NullLiteral)
-    def null_to_json(self, node):
+    def null_to_json(self, node: NullLiteral) -> Any:
         self.process_wsc_before(node)
         self.env.write('null')
         self.process_wsc_after(node)
 
     @to_json(BooleanLiteral)
-    def boolean_to_json(self, node):
+    def boolean_to_json(self, node: BooleanLiteral) -> Any:
         self.process_wsc_before(node)
         if node.value:
             self.env.write('true')
         else:
             self.env.write('false')
         self.process_wsc_after(node)
 
     @to_json(LineComment)
-    def line_comment_to_json(self, node):
+    def line_comment_to_json(self, node: LineComment) -> Any:
         self.process_wsc_before(node)
         self.env.write(node.value)
         self.process_wsc_after(node)
 
     @to_json(BlockComment)
-    def block_comment_to_json(self, node):
+    def block_comment_to_json(self, node: BlockComment) -> Any:
         self.process_wsc_before(node)
         self.env.write(node.value)
         self.process_wsc_after(node)
 
     @to_json(TrailingComma)
-    def trailing_comma_to_json(self, node):
+    def trailing_comma_to_json(self, node: TrailingComma) -> Any:
         self.process_wsc_before(node)
         self.env.write(',')
         self.process_wsc_after(node)
 
     @to_json(Infinity)
-    def infinity_to_json(self, node):
+    def infinity_to_json(self, node: Infinity) -> Any:
         self.process_wsc_before(node)
 
         self.env.write('Infinity')
         self.process_wsc_after(node)
 
     @to_json(NaN)
-    def nan_to_json(self, node):
+    def nan_to_json(self, node: NaN) -> Any:
         self.process_wsc_before(node)
         self.env.write('NaN')
         self.process_wsc_after(node)
 
+
 class Modelizer:
     """
     Turn Python objects into a model
     """
+
     @singledispatchmethod
-    def modelize(self, obj):
+    def modelize(self, obj: Any) -> Node:
         raise NotImplementedError(f"Cannot modelize object of type {type(obj)}")
 
     to_model = modelize.register
 
     @to_model(str)
-    def str_to_model(self, s):
+    def str_to_model(self, s: str) -> SingleQuotedString | DoubleQuotedString:
         if repr(s).startswith("'"):
             return SingleQuotedString(s, raw_value=repr(s))
         else:
             return DoubleQuotedString(s, raw_value=repr(s))
 
     @to_model(dict)
-    def dict_to_model(self, d):
-        kvps = []
+    def dict_to_model(self, d: dict[Any, Any]) -> JSONObject:
+        kvps: list[KeyValuePair] = []
         for key, value in d.items():
-            kvp = KeyValuePair(key=self.modelize(key), value=self.modelize(value))
+            kvp = KeyValuePair(key=self.modelize(key), value=self.modelize(value))  # type: ignore[arg-type]
             kvps.append(kvp)
         return JSONObject(*kvps)
 
     @to_model(list)
-    def list_to_model(self, lst):
-        list_values = []
+    def list_to_model(self, lst: list[Any]) -> JSONArray:
+        list_values: list[Value] = []
         for v in lst:
-            list_values.append(self.modelize(v))
+            list_values.append(self.modelize(v))  # type: ignore[arg-type]
         return JSONArray(*list_values)
 
     @to_model(int)
-    def int_to_model(self, i):
+    def int_to_model(self, i: int) -> Integer:
         return Integer(str(i))
 
-
     @to_model(float)
-    def float_to_model(self, f):
+    def float_to_model(self, f: float) -> Infinity | NaN | Float | UnaryOp:
         if f == math.inf:
             return Infinity()
         elif f == -math.inf:
             return UnaryOp('-', Infinity())
         elif f is math.nan:
             return NaN()
         else:
             return Float(str(f))
 
     @to_model(bool)
-    def bool_to_model(self, b):
+    def bool_to_model(self, b: bool) -> BooleanLiteral:
         return BooleanLiteral(b)
 
     @to_model(type(None))
-    def none_to_model(self, _):
+    def none_to_model(self, _: Any) -> NullLiteral:
         return NullLiteral()
 
 
-def modelize(obj):
+def modelize(obj: Any) -> Node:
     """
 
     :param obj: a python object
     :return: a model representing the python object
     """
     return Modelizer().modelize(obj)
```

### Comparing `json-five-0.8.0/json5/tokenizer.py` & `json-five-1.0.0rc1/json5/tokenizer.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,102 +1,127 @@
+from __future__ import annotations
+
+import logging
+import typing
+from typing import Generator
+from typing import NoReturn
+
 import regex as re
-import sys
-from sly import Lexer
-from sly.lex import Token
+from sly import Lexer  # type: ignore
+from sly.lex import Token  # type: ignore
+
 from json5.utils import JSON5DecodeError
-import logging
 
 logger = logging.getLogger(__name__)
 # logger.addHandler(logging.StreamHandler(stream=sys.stderr))
 # logger.setLevel(level=logging.DEBUG)
-class JSON5Token(Token):
+
+
+class JSON5Token(Token):  # type: ignore[misc]
     '''
     Representation of a single token.
     '''
-    def __init__(self, tok, doc):
+
+    def __init__(self, tok: Token, doc: str):
         self.type = tok.type
         self.value = tok.value
         self.lineno = tok.lineno
         self.index = tok.index
         self.doc = doc
         self.end = getattr(tok, 'end', None)
+
     __slots__ = ('type', 'value', 'lineno', 'index', 'doc', 'end')
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f'JSON5Token(type={self.type!r}, value={self.value!r}, lineno={self.lineno}, index={self.index}, end={self.end})'
 
 
-class JSONLexer(Lexer):
+T_CallArg = typing.TypeVar('T_CallArg')
+_: typing.Callable[[str], typing.Callable[[T_CallArg], T_CallArg]]
+
+
+class JSONLexer(Lexer):  # type: ignore[misc]
     regex_module = re
     reflags = re.DOTALL
-    tokens = {LBRACE, RBRACE,
-              LBRACKET, RBRACKET,
-              DOUBLE_QUOTE_STRING, SINGLE_QUOTE_STRING,
-              UNTERMINATED_DOUBLE_QUOTE_STRING,
-              UNTERMINATED_SINGLE_QUOTE_STRING,
-              NAME,
-              COMMA,
-              BLOCK_COMMENT,
-              LINE_COMMENT,
-              WHITESPACE,
-              TRUE, FALSE, NULL,
-              COLON,
-
-              # Numbers
-              PLUS, MINUS,
-              FLOAT, INTEGER,
-              INFINITY, NAN, EXPONENT,
-              HEXADECIMAL,
-              OCTAL  # Not allowed, but we capture as a token to raise error later
-              }
+    tokens = {
+        LBRACE,
+        RBRACE,
+        LBRACKET,
+        RBRACKET,
+        DOUBLE_QUOTE_STRING,
+        SINGLE_QUOTE_STRING,
+        UNTERMINATED_DOUBLE_QUOTE_STRING,
+        UNTERMINATED_SINGLE_QUOTE_STRING,
+        NAME,
+        COMMA,
+        BLOCK_COMMENT,
+        LINE_COMMENT,
+        WHITESPACE,
+        TRUE,
+        FALSE,
+        NULL,
+        COLON,
+        # Numbers
+        PLUS,
+        MINUS,
+        FLOAT,
+        INTEGER,
+        INFINITY,
+        NAN,
+        EXPONENT,
+        HEXADECIMAL,
+        OCTAL,  # Not allowed, but we capture as a token to raise error later
+    }
 
-    def tokenize(self, text, *args, **kwargs):
-        for tok in super().tokenize(text, *args, **kwargs):
+    def tokenize(self, text: str, lineno: int = 1, index: int = 0) -> Generator[JSON5Token, None, None]:
+        for tok in super().tokenize(text, lineno, index):
             tok = JSON5Token(tok, text)
             yield tok
 
     LBRACE = r'{'
     RBRACE = r'}'
     LBRACKET = r'\['
     RBRACKET = r'\]'
     COLON = r"\:"
     COMMA = r"\,"
 
     DOUBLE_QUOTE_STRING = r'"(?:[^"\\]|\\.)*"'
     SINGLE_QUOTE_STRING = r"'(?:[^'\\]|\\.)*'"
 
     LINE_COMMENT = r"//[^\n]*"
+
     @_(r'/\*((.|\n))*?\*/')
-    def BLOCK_COMMENT(self, tok):
+    def BLOCK_COMMENT(self, tok: JSON5Token) -> JSON5Token:
         self.lineno += tok.value.count('\n')
         return tok
 
     @_("[\u0009\u000A\u000B\u000C\u000D\u0020\u00A0\u2028\u2029\ufeff]+")
-    def WHITESPACE(self, tok):
+    def WHITESPACE(self, tok: JSON5Token) -> JSON5Token:
         self.lineno += tok.value.count('\n')
         return tok
 
     MINUS = r'\-'
     PLUS = r'\+'
     EXPONENT = r"(e|E)(\-|\+)?\d+"
     HEXADECIMAL = r'0(x|X)[0-9a-fA-F]+'
     OCTAL = r'(0\d+|0o\d+)'
-    FLOAT = r'(\d+\.\d*)|(\d*\.\d+)'      # 23.45
+    FLOAT = r'(\d+\.\d*)|(\d*\.\d+)'  # 23.45
     INTEGER = r'\d+'
     NAME = r'[\w_\$\\]([\w_\d\$\\\p{Pc}\p{Mn}\p{Mc}\u200C\u200D])*'
 
-    NAME['true'] = TRUE
-    NAME['false'] = FALSE
-    NAME['null'] = NULL
-    NAME['Infinity'] = INFINITY
-    NAME['NaN'] = NAN
+    NAME['true'] = TRUE  # type: ignore[index]
+    NAME['false'] = FALSE  # type: ignore[index]
+    NAME['null'] = NULL  # type: ignore[index]
+    NAME['Infinity'] = INFINITY  # type: ignore[index]
+    NAME['NaN'] = NAN  # type: ignore[index]
 
     UNTERMINATED_DOUBLE_QUOTE_STRING = r'"(?:[^"\\]|\\.)*'
     UNTERMINATED_SINGLE_QUOTE_STRING = r"'(?:[^'\\]|\\.)*"
 
-    def error(self, t):
+    def error(self, t: JSON5Token) -> NoReturn:
         raise JSON5DecodeError(f'Illegal character {t.value[0]!r} at index {self.index}', None)
 
-def tokenize(text):
+
+def tokenize(text: str) -> Generator[JSON5Token, None, None]:
     lexer = JSONLexer()
     tokens = lexer.tokenize(text)
     return tokens
```

### Comparing `json-five-0.8.0/json_five.egg-info/PKG-INFO` & `json-five-1.0.0rc1/json_five.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: json-five
-Version: 0.8.0
+Version: 1.0.0rc1
 Summary: A JSON5 parser that, among other features, supports round-trip preservation of comments
 Home-page: https://github.com/spyoungtech/json-five
 Author: Spencer Phillip Young
 Author-email: spencer.young@spyoung.com
 License: Apache
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # json-five
 
 JSON5 for Python
```

