# Comparing `tmp/ai_functions-0.4.2.tar.gz` & `tmp/ai_functions-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_functions-0.4.2.tar", max compression
+gzip compressed data, was "ai_functions-0.4.3.tar", max compression
```

## Comparing `ai_functions-0.4.2.tar` & `ai_functions-0.4.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       94 2023-07-22 07:26:46.226935 ai_functions-0.4.2/ai_functions/__init__.py
--rw-r--r--   0        0        0     6733 2023-08-01 02:43:50.694045 ai_functions-0.4.2/ai_functions/functions.py
--rw-r--r--   0        0        0      614 2023-08-01 02:44:05.183253 ai_functions-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     2190 2023-07-25 20:02:47.045696 ai_functions-0.4.2/README.md
--rw-r--r--   0        0        0     2676 1970-01-01 00:00:00.000000 ai_functions-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0       94 2023-07-22 07:26:46.226935 ai_functions-0.4.3/ai_functions/__init__.py
+-rw-r--r--   0        0        0     6890 2023-08-01 17:40:15.381602 ai_functions-0.4.3/ai_functions/functions.py
+-rw-r--r--   0        0        0      614 2023-08-01 19:27:56.264766 ai_functions-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     2190 2023-07-25 20:02:47.045696 ai_functions-0.4.3/README.md
+-rw-r--r--   0        0        0     2676 1970-01-01 00:00:00.000000 ai_functions-0.4.3/PKG-INFO
```

### Comparing `ai_functions-0.4.2/ai_functions/functions.py` & `ai_functions-0.4.3/ai_functions/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import asyncio
 import inspect
 import json
+import typing
 from typing import get_origin, Annotated, get_args, Callable, Iterable, Union
 import logging
 
 log = logging.getLogger(__name__)
 
 JSON_TYPE_MAP = {
     str: "string",
     int: "number",
     bool: "boolean",
     float: "number",
-    list: "array"
+    list: "array",
+    dict: "object"
 }
 
 
 def convert_response(ret):
     # convert content to be a string, for sure
     try:
         content = ret if isinstance(ret, str) else json.dumps(ret)
@@ -99,16 +101,21 @@
         if get_origin(param.annotation) is not Annotated:
             continue
         base_type = get_args(param.annotation)[0]
         param_description = param.annotation.__metadata__[0]
         if param_description is None:
             continue
         if param.default == inspect.Parameter.empty:
-            required.append(param_name) 
+            required.append(param_name)
+
+        type_args = typing.get_args(base_type)
+        if type_args:
+            base_type = typing.get_origin(base_type)
         param_type = JSON_TYPE_MAP[base_type]
+
         annotated_args[param_name] = {"type": param_type, "description": param_description}
     return annotated_args, required
 
 
 def get_openai_dict(funcs: Iterable[Callable] = None):
     ret = []
     for func in funcs:
```

### Comparing `ai_functions-0.4.2/pyproject.toml` & `ai_functions-0.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ai-functions"
-version = "0.4.2"
+version = "0.4.3"
 description = "manage openai functions and execution"
 authors = ["erik aronesty <erik@q32.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "ai_functions"}]
 
 [tool.poetry.dependencies]
```

### Comparing `ai_functions-0.4.2/README.md` & `ai_functions-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `ai_functions-0.4.2/PKG-INFO` & `ai_functions-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-functions
-Version: 0.4.2
+Version: 0.4.3
 Summary: manage openai functions and execution
 License: MIT
 Author: erik aronesty
 Author-email: erik@q32.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

