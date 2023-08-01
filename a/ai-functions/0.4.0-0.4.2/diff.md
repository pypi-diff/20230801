# Comparing `tmp/ai_functions-0.4.0.tar.gz` & `tmp/ai_functions-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_functions-0.4.0.tar", max compression
+gzip compressed data, was "ai_functions-0.4.2.tar", max compression
```

## Comparing `ai_functions-0.4.0.tar` & `ai_functions-0.4.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       94 2023-07-22 07:26:46.226935 ai_functions-0.4.0/ai_functions/__init__.py
--rw-r--r--   0        0        0     6604 2023-07-22 20:26:41.473071 ai_functions-0.4.0/ai_functions/functions.py
--rw-r--r--   0        0        0      614 2023-07-22 20:27:56.171838 ai_functions-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1520 2023-07-21 17:19:00.362094 ai_functions-0.4.0/README.md
--rw-r--r--   0        0        0     2006 1970-01-01 00:00:00.000000 ai_functions-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0       94 2023-07-22 07:26:46.226935 ai_functions-0.4.2/ai_functions/__init__.py
+-rw-r--r--   0        0        0     6733 2023-08-01 02:43:50.694045 ai_functions-0.4.2/ai_functions/functions.py
+-rw-r--r--   0        0        0      614 2023-08-01 02:44:05.183253 ai_functions-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     2190 2023-07-25 20:02:47.045696 ai_functions-0.4.2/README.md
+-rw-r--r--   0        0        0     2676 1970-01-01 00:00:00.000000 ai_functions-0.4.2/PKG-INFO
```

### Comparing `ai_functions-0.4.0/ai_functions/functions.py` & `ai_functions-0.4.2/ai_functions/functions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import asyncio
 import inspect
 import json
-from typing import get_origin, Any, Annotated, get_args, Callable, Iterable, Union
+from typing import get_origin, Annotated, get_args, Callable, Iterable, Union
 import logging
 
 log = logging.getLogger(__name__)
 
 JSON_TYPE_MAP = {
     str: "string",
     int: "number",
@@ -27,14 +27,17 @@
 class AIFunctions:
     def __init__(self, funcs=[], *, loop=None, convert_output=convert_response):
         self.map = dict({f.__name__: f for f in funcs})
         self.loop = loop
         self.validate()
         self.convert_output = convert_output
 
+    def clone(self):
+        return AIFunctions(self.map.values(), loop=self.loop, convert_output=self.convert_output)
+
     def validate(self):
         """Check that all functions have appropriate annotations."""
         get_openai_dict(self.map.values())
 
     def openai_dict(self, funcs: Iterable[Union[str, Callable]] = []):
         """Make an openai compatible function dict"""
         if funcs:
@@ -124,15 +127,15 @@
                 type="object",
                 properties=dict(
                     **args
                 ),
             )
         )
         if required:
-            d["required"] = required
+            d["parameters"]["required"] = required
         ret.append(d)
 
     return ret
 
 
 def execute_function(funcs: Iterable[Callable], name: str, arguments: Union[str, dict], *, loop=None,
                      convert_output=convert_response, **kws):
```

### Comparing `ai_functions-0.4.0/pyproject.toml` & `ai_functions-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ai-functions"
-version = "0.4.0"
+version = "0.4.2"
 description = "manage openai functions and execution"
 authors = ["erik aronesty <erik@q32.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "ai_functions"}]
 
 [tool.poetry.dependencies]
```

### Comparing `ai_functions-0.4.0/PKG-INFO` & `ai_functions-0.4.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,19 @@
-Metadata-Version: 2.1
-Name: ai-functions
-Version: 0.4.0
-Summary: manage openai functions and execution
-License: MIT
-Author: erik aronesty
-Author-email: erik@q32.com
-Requires-Python: >=3.9,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-
 # Python AI Functions
 
 
 Simple library that can convert from python functions to a JSON schema description of those functions, suitable for use with AI libraries.
 
 
+## Installation
+
+`pip install ai-functions`
+
+## Usage
+
 For example:
 
 ```
 from ai_functions import get_openai_functions, execute_function
 
 
 def search_web(query: Annotated[str, "google formatted keywords to search for"]):
@@ -54,19 +45,32 @@
 
 functions = container.openai_dict()
 subset_functions = container.openai_dict(["search_web"])
 container.execute("search_web", {"query":"top web hosting sites"})
 container.opeanai_execute({"name": "search_web", "arguments": "{\"query\":\"top web hosting sites\"}")
 
 ```
+## What stuff does this handle?
+
+ - Converts your annotated schema into an appropriate prompt 
+ - Handles converting arguments to JSON if they are specified as a string.
+ - Auto-casts arguments to the right types, if they aren't right.
+ - Raises errors that AI engines understand if returned as a function response, instead of errors with poor descriptions.
+
+## Async execute
+ - If a loop is provided to the AIFunctions constructor, or to any execute calls, it will be used to schedule a coroutine.
+ - Async versions of execute are available, prefix all calls with `async_`
+
 
+### Some fine print
 
-It handles converting arguments to JSON if they are specified as a string.
+If you want to have a paramter that is still seen as "valid", but isn't part of the schema, you can 
+annotate it with None as the description.  But this is really an "enforcement" thing, and might not
+belong in this library.
 
-It auto-casts arguments to the right types, if they aren't right.
+Dealing with context is a beast in chat apps, so more work here might be helpful.
 
-It returns errors that AI engines understands, instead of errors with poor descriptions.
+For example, I use meta-functions that unlock others, to prevent context-bloat.  
 
-If a loop is provided to the AIFunctions constructor, or to any execute calls, it will be used to schedule a coroutine.
+Might put that in another lib soon, or put it here.
 
-Async versions of execute are available, prefix all calls with `async_`
```

