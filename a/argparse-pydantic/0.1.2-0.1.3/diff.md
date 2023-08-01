# Comparing `tmp/argparse_pydantic-0.1.2.tar.gz` & `tmp/argparse_pydantic-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argparse_pydantic-0.1.2.tar", last modified: Mon Jul 31 13:04:07 2023, max compression
+gzip compressed data, was "argparse_pydantic-0.1.3.tar", last modified: Tue Aug  1 11:32:23 2023, max compression
```

## Comparing `argparse_pydantic-0.1.2.tar` & `argparse_pydantic-0.1.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-07-31 13:04:07.225324 argparse_pydantic-0.1.2/
--rw-rw-r--   0 aya       (1000) aya       (1000)    11357 2023-07-28 15:19:19.000000 argparse_pydantic-0.1.2/LICENSE
--rw-rw-r--   0 aya       (1000) aya       (1000)     3230 2023-07-31 13:04:07.225324 argparse_pydantic-0.1.2/PKG-INFO
--rw-rw-r--   0 aya       (1000) aya       (1000)     2523 2023-07-31 12:57:21.000000 argparse_pydantic-0.1.2/README.md
--rw-rw-r--   0 aya       (1000) aya       (1000)      833 2023-07-31 13:04:07.225324 argparse_pydantic-0.1.2/setup.cfg
--rw-rw-r--   0 aya       (1000) aya       (1000)      597 2023-07-28 15:19:19.000000 argparse_pydantic-0.1.2/setup.py
-drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-07-31 13:04:07.221323 argparse_pydantic-0.1.2/src/
-drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-07-31 13:04:07.221323 argparse_pydantic-0.1.2/src/argparse_pydantic/
--rw-rw-r--   0 aya       (1000) aya       (1000)      139 2023-07-28 15:19:19.000000 argparse_pydantic-0.1.2/src/argparse_pydantic/__init__.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     5294 2023-07-31 09:25:37.000000 argparse_pydantic-0.1.2/src/argparse_pydantic/core.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     1284 2023-07-28 15:19:19.000000 argparse_pydantic-0.1.2/src/argparse_pydantic/helpers.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     3240 2023-07-28 15:19:19.000000 argparse_pydantic-0.1.2/src/argparse_pydantic/test_tools.py
--rw-rw-r--   0 aya       (1000) aya       (1000)       22 2023-07-31 12:59:57.000000 argparse_pydantic-0.1.2/src/argparse_pydantic/version.py
-drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-07-31 13:04:07.225324 argparse_pydantic-0.1.2/src/argparse_pydantic.egg-info/
--rw-rw-r--   0 aya       (1000) aya       (1000)     3230 2023-07-31 13:04:07.000000 argparse_pydantic-0.1.2/src/argparse_pydantic.egg-info/PKG-INFO
--rw-rw-r--   0 aya       (1000) aya       (1000)      705 2023-07-31 13:04:07.000000 argparse_pydantic-0.1.2/src/argparse_pydantic.egg-info/SOURCES.txt
--rw-rw-r--   0 aya       (1000) aya       (1000)        1 2023-07-31 13:04:07.000000 argparse_pydantic-0.1.2/src/argparse_pydantic.egg-info/dependency_links.txt
--rw-rw-r--   0 aya       (1000) aya       (1000)       61 2023-07-31 13:04:07.000000 argparse_pydantic-0.1.2/src/argparse_pydantic.egg-info/requires.txt
--rw-rw-r--   0 aya       (1000) aya       (1000)       18 2023-07-31 13:04:07.000000 argparse_pydantic-0.1.2/src/argparse_pydantic.egg-info/top_level.txt
-drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-07-31 13:04:07.225324 argparse_pydantic-0.1.2/tests/
--rw-rw-r--   0 aya       (1000) aya       (1000)     2469 2023-07-28 15:19:19.000000 argparse_pydantic-0.1.2/tests/test_add_argument_action.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     1382 2023-07-31 12:34:17.000000 argparse_pydantic-0.1.2/tests/test_add_argument_base.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     1956 2023-07-28 15:19:19.000000 argparse_pydantic-0.1.2/tests/test_add_argument_flag.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     4752 2023-07-31 12:31:22.000000 argparse_pydantic-0.1.2/tests/test_add_argument_json_schema_extra.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     2311 2023-07-31 11:01:21.000000 argparse_pydantic-0.1.2/tests/test_add_argument_simple.py
--rw-rw-r--   0 aya       (1000) aya       (1000)      980 2023-07-28 15:19:19.000000 argparse_pydantic-0.1.2/tests/test_core_base.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     1199 2023-07-28 15:19:19.000000 argparse_pydantic-0.1.2/tests/test_create_parser.py
--rw-rw-r--   0 aya       (1000) aya       (1000)      521 2023-07-28 15:19:19.000000 argparse_pydantic-0.1.2/tests/test_parse_args.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     3778 2023-07-28 15:19:19.000000 argparse_pydantic-0.1.2/tests/test_test_tools.py
+drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-08-01 11:32:23.144056 argparse_pydantic-0.1.3/
+-rw-rw-r--   0 aya       (1000) aya       (1000)    11357 2023-07-28 15:19:19.000000 argparse_pydantic-0.1.3/LICENSE
+-rw-rw-r--   0 aya       (1000) aya       (1000)     4308 2023-08-01 11:32:23.144056 argparse_pydantic-0.1.3/PKG-INFO
+-rw-rw-r--   0 aya       (1000) aya       (1000)     3601 2023-08-01 11:30:08.000000 argparse_pydantic-0.1.3/README.md
+-rw-rw-r--   0 aya       (1000) aya       (1000)      833 2023-08-01 11:32:23.144056 argparse_pydantic-0.1.3/setup.cfg
+-rw-rw-r--   0 aya       (1000) aya       (1000)      597 2023-07-28 15:19:19.000000 argparse_pydantic-0.1.3/setup.py
+drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-08-01 11:32:23.136056 argparse_pydantic-0.1.3/src/
+drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-08-01 11:32:23.140056 argparse_pydantic-0.1.3/src/argparse_pydantic/
+-rw-rw-r--   0 aya       (1000) aya       (1000)      139 2023-07-28 15:19:19.000000 argparse_pydantic-0.1.3/src/argparse_pydantic/__init__.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     5900 2023-07-31 14:58:01.000000 argparse_pydantic-0.1.3/src/argparse_pydantic/core.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     1284 2023-07-28 15:19:19.000000 argparse_pydantic-0.1.3/src/argparse_pydantic/helpers.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     3240 2023-07-28 15:19:19.000000 argparse_pydantic-0.1.3/src/argparse_pydantic/test_tools.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)       22 2023-08-01 11:30:26.000000 argparse_pydantic-0.1.3/src/argparse_pydantic/version.py
+drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-08-01 11:32:23.140056 argparse_pydantic-0.1.3/src/argparse_pydantic.egg-info/
+-rw-rw-r--   0 aya       (1000) aya       (1000)     4308 2023-08-01 11:32:23.000000 argparse_pydantic-0.1.3/src/argparse_pydantic.egg-info/PKG-INFO
+-rw-rw-r--   0 aya       (1000) aya       (1000)      705 2023-08-01 11:32:23.000000 argparse_pydantic-0.1.3/src/argparse_pydantic.egg-info/SOURCES.txt
+-rw-rw-r--   0 aya       (1000) aya       (1000)        1 2023-08-01 11:32:23.000000 argparse_pydantic-0.1.3/src/argparse_pydantic.egg-info/dependency_links.txt
+-rw-rw-r--   0 aya       (1000) aya       (1000)       61 2023-08-01 11:32:23.000000 argparse_pydantic-0.1.3/src/argparse_pydantic.egg-info/requires.txt
+-rw-rw-r--   0 aya       (1000) aya       (1000)       18 2023-08-01 11:32:23.000000 argparse_pydantic-0.1.3/src/argparse_pydantic.egg-info/top_level.txt
+drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-08-01 11:32:23.144056 argparse_pydantic-0.1.3/tests/
+-rw-rw-r--   0 aya       (1000) aya       (1000)     2469 2023-07-28 15:19:19.000000 argparse_pydantic-0.1.3/tests/test_add_argument_action.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     2170 2023-08-01 08:57:52.000000 argparse_pydantic-0.1.3/tests/test_add_argument_base.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     1956 2023-07-28 15:19:19.000000 argparse_pydantic-0.1.3/tests/test_add_argument_flag.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     4752 2023-07-31 12:31:22.000000 argparse_pydantic-0.1.3/tests/test_add_argument_json_schema_extra.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     2311 2023-07-31 11:01:21.000000 argparse_pydantic-0.1.3/tests/test_add_argument_simple.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)      980 2023-07-28 15:19:19.000000 argparse_pydantic-0.1.3/tests/test_core_base.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     1199 2023-07-28 15:19:19.000000 argparse_pydantic-0.1.3/tests/test_create_parser.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)      521 2023-07-28 15:19:19.000000 argparse_pydantic-0.1.3/tests/test_parse_args.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     3778 2023-07-28 15:19:19.000000 argparse_pydantic-0.1.3/tests/test_test_tools.py
```

### Comparing `argparse_pydantic-0.1.2/LICENSE` & `argparse_pydantic-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `argparse_pydantic-0.1.2/PKG-INFO` & `argparse_pydantic-0.1.3/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-Metadata-Version: 2.1
-Name: argparse_pydantic
-Version: 0.1.2
-Summary: argparse config with pydantic model.
-Home-page: https://github.com/ayasyrev/argparse_pydantic
-Author: Yasyrev Andrei
-Author-email: a.yasyrev@gmail.com
-License: apache2
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
-
 # Argparse Pydantic
 
 Config for argparse with pydantic model.
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/argparse_pydantic)](https://pypi.org/project/argparse_pydantic/)
 ![PyPI](https://img.shields.io/pypi/v/argparse_pydantic?color=blue)  
 [![Tests](https://github.com/ayasyrev/argparse_pydantic/workflows/Tests/badge.svg)](https://github.com/ayasyrev/argparse_pydantic/actions?workflow=Tests)  [![Codecov](https://codecov.io/gh/ayasyrev/argparse_pydantic/branch/main/graph/badge.svg)](https://codecov.io/gh/ayasyrev/argparse_pydantic)  
@@ -43,15 +23,15 @@
 Or install from github repo:
 
 `pip install git+https://github.com/ayasyrev/argparse_pydantic.git`
 
 ## Base use.
 
 We use python argparse to parse arguments from command line.  
-So - just create parser as usual:
+So, just create parser as usual:
 
 
 ```python
 import argparse
 
 parser = argparse.ArgumentParser(prog="MyApp")
 ```
@@ -77,28 +57,27 @@
 ```
 
 So we got parser with arguments from config.
 
 It exactly like parser made classic way:  
 `parser.add_argument("echo")`
 
+Now we can use parser in you script usual way - `parser.parse_args()`
 
-```python
-parser.print_help()
+<!-- termynal -->
+```
+$ python my_app.py -h
+usage: MyApp [-h] echo
+
+positional arguments:
+  echo
+
+options:
+  -h, --help  show this help message and exit
 ```
-<details open> <summary>output</summary>  
-    <pre>usage: MyApp [-h] echo
-    
-    positional arguments:
-      echo
-    
-    options:
-      -h, --help  show this help message and exit
-    </pre>
-</details>
 
 Parse command line as usual.
 
 
 ```python
 args = parser.parse_args(["argument from command line"])
 ```
@@ -131,10 +110,66 @@
 ```
 <details open> <summary>output</summary>  
     <pre>'argument from command line'</pre>
 </details>
 
 
 
+### Optional if undefined.
+
+We can use undefined arguments as positional or optional (but required).
+
+
+```python
+class AppCfg2(BaseModel):
+    arg_int: int
+    arg_float: float = 0.1
+```
+
+
+```python
+parser = argparse.ArgumentParser(prog="MyApp")
+parser = add_args_from_model(parser, AppCfg2, undefined_positional=False)
+```
+
+<!-- termynal -->
+```
+$ python my_app.py -h
+usage: MyApp [-h] --arg_int ARG_INT [--arg_float ARG_FLOAT]
+
+options:
+  -h, --help            show this help message and exit
+  --arg_int ARG_INT
+  --arg_float ARG_FLOAT
+```
+
+### Add types and defaults values.
+
+And we can add type hints to help message from our config.  
+
+
+
+```python
+parser = argparse.ArgumentParser(prog="MyApp")
+parser = add_args_from_model(
+    parser,
+    AppCfg2,
+    undefined_positional=False,
+    help_def_type=True,
+)
+```
+
+<!-- termynal -->
+```
+$ python my_app.py -h
+usage: MyApp [-h] --arg_int ARG_INT [--arg_float ARG_FLOAT]
+
+options:
+  -h, --help            show this help message and exit
+  --arg_int ARG_INT     [int]
+  --arg_float ARG_FLOAT
+                        [float] default: 0.1
+```
+
 ## Examples
 
 You can see examples at `examples` folder - Same examples as at python docs and tutorial for argparse.
```

### Comparing `argparse_pydantic-0.1.2/setup.cfg` & `argparse_pydantic-0.1.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `argparse_pydantic-0.1.2/setup.py` & `argparse_pydantic-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `argparse_pydantic-0.1.2/src/argparse_pydantic/core.py` & `argparse_pydantic-0.1.3/src/argparse_pydantic/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import argparse
+import sys
 from typing import Any, Iterable, Optional, Sequence, Type, Union
 
 from pydantic import BaseModel
 from pydantic.fields import FieldInfo
 from pydantic_core import PydanticUndefined
 from typing_extensions import get_args, get_origin
 
@@ -27,14 +28,24 @@
     "version",
     # not in argparse, for flags
     "flag",
     "positional",
 )
 
 
+if sys.version_info < (3, 10):  # pragma: no cover
+    def is_union(tp: type[Any] | None) -> bool:
+        return get_origin(tp) is Union
+else:
+    from types import UnionType
+
+    def is_union(tp: type[Any] | None) -> bool:
+        return get_origin(tp) is Union or isinstance(tp, UnionType)
+
+
 def argument_kwargs(
     flag: str | None = None,
     action: str | None = None,
     nargs: int | str | None = None,
     const: str | None = None,
     default: Any = None,
     type: ArgType = None,  # pylint: disable=redefined-builtin
@@ -64,15 +75,15 @@
     }
     return {key: val for key, val in kwargs.items() if val is not None}
 
 
 def get_field_type(field_info: FieldInfo) -> Type:
     """get field type, convert to base type."""
     field_type = field_info.annotation
-    if get_origin(field_type) is Union:
+    if is_union(field_type):
         return get_args(field_type)[0]
     return field_type
 
 
 def parse_field_kwargs(json_schema_extra: dict[str, Any]) -> dict[str, Any]:
     """parse json_schema_extra for argparse add_argument args"""
     field_kwargs = {key: val for key, val in json_schema_extra.items() if key in ARG_KEYWORDS and val is not None}
@@ -82,14 +93,15 @@
 
 
 def add_field_arg(
     parser: argparse.ArgumentParser,
     field_name: str,
     field_info: FieldInfo,
     undefined_positional: bool = True,
+    help_def_type: bool = False,
 ) -> None:
     """add argument to parser from field_info"""
     flags = [f"--{field_name}"]
     kwargs = argument_kwargs(
         help=field_info.description,
         required=field_info.is_required(),
         default=field_info.default if field_info.default is not PydanticUndefined else None,
@@ -117,15 +129,21 @@
 
     if "action" in kwargs:
         kwargs.pop("type", None)
         validate_action(kwargs["action"], kwargs.get("default", None))
         if kwargs["action"] not in ("count", "store_const"):
             kwargs.pop("default", None)
 
-    # process help message - ? add additional info like defaults and type
+    if help_def_type:
+        field_type = get_field_type(field_info)
+        if field_info.default is PydanticUndefined:
+            default = ""
+        else:
+            default = f"default: {field_info.default}"
+        kwargs["help"] = kwargs.get("help", "") + f" [{field_type.__name__}] {default}"
     parser.add_argument(*flags, **kwargs)
 
 
 def process_flag(flag) -> Optional[str]:
     """check short flag - if without prefix - add it, if long string, return None"""
     if len(flag) == 1:
         return f"-{flag}"
@@ -142,18 +160,19 @@
             raise ValueError(f"action {action} doesn't match default {default}")
 
 
 def add_args_from_model(
     parser: argparse.ArgumentParser,
     model: BaseModel,
     undefined_positional: bool = True,
+    help_def_type: bool = False,
 ) -> argparse.ArgumentParser:
     """add args from model to parser"""
     for field_name, field_info in model.model_fields.items():
-        add_field_arg(parser, field_name, field_info, undefined_positional)
+        add_field_arg(parser, field_name, field_info, undefined_positional, help_def_type)
     return parser
 
 
 def create_model_obj(model: BaseModel, args: argparse.Namespace) -> BaseModel:
     """create model from parsed args"""
     kwargs = {
         key: val for key, val in args.__dict__.items() if key in model.model_fields
```

### Comparing `argparse_pydantic-0.1.2/src/argparse_pydantic/helpers.py` & `argparse_pydantic-0.1.3/src/argparse_pydantic/helpers.py`

 * *Files identical despite different names*

### Comparing `argparse_pydantic-0.1.2/src/argparse_pydantic/test_tools.py` & `argparse_pydantic-0.1.3/src/argparse_pydantic/test_tools.py`

 * *Files identical despite different names*

### Comparing `argparse_pydantic-0.1.2/src/argparse_pydantic.egg-info/PKG-INFO` & `argparse_pydantic-0.1.3/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: argparse-pydantic
-Version: 0.1.2
+Name: argparse_pydantic
+Version: 0.1.3
 Summary: argparse config with pydantic model.
 Home-page: https://github.com/ayasyrev/argparse_pydantic
 Author: Yasyrev Andrei
 Author-email: a.yasyrev@gmail.com
 License: apache2
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -43,15 +43,15 @@
 Or install from github repo:
 
 `pip install git+https://github.com/ayasyrev/argparse_pydantic.git`
 
 ## Base use.
 
 We use python argparse to parse arguments from command line.  
-So - just create parser as usual:
+So, just create parser as usual:
 
 
 ```python
 import argparse
 
 parser = argparse.ArgumentParser(prog="MyApp")
 ```
@@ -77,28 +77,27 @@
 ```
 
 So we got parser with arguments from config.
 
 It exactly like parser made classic way:  
 `parser.add_argument("echo")`
 
+Now we can use parser in you script usual way - `parser.parse_args()`
 
-```python
-parser.print_help()
+<!-- termynal -->
+```
+$ python my_app.py -h
+usage: MyApp [-h] echo
+
+positional arguments:
+  echo
+
+options:
+  -h, --help  show this help message and exit
 ```
-<details open> <summary>output</summary>  
-    <pre>usage: MyApp [-h] echo
-    
-    positional arguments:
-      echo
-    
-    options:
-      -h, --help  show this help message and exit
-    </pre>
-</details>
 
 Parse command line as usual.
 
 
 ```python
 args = parser.parse_args(["argument from command line"])
 ```
@@ -131,10 +130,66 @@
 ```
 <details open> <summary>output</summary>  
     <pre>'argument from command line'</pre>
 </details>
 
 
 
+### Optional if undefined.
+
+We can use undefined arguments as positional or optional (but required).
+
+
+```python
+class AppCfg2(BaseModel):
+    arg_int: int
+    arg_float: float = 0.1
+```
+
+
+```python
+parser = argparse.ArgumentParser(prog="MyApp")
+parser = add_args_from_model(parser, AppCfg2, undefined_positional=False)
+```
+
+<!-- termynal -->
+```
+$ python my_app.py -h
+usage: MyApp [-h] --arg_int ARG_INT [--arg_float ARG_FLOAT]
+
+options:
+  -h, --help            show this help message and exit
+  --arg_int ARG_INT
+  --arg_float ARG_FLOAT
+```
+
+### Add types and defaults values.
+
+And we can add type hints to help message from our config.  
+
+
+
+```python
+parser = argparse.ArgumentParser(prog="MyApp")
+parser = add_args_from_model(
+    parser,
+    AppCfg2,
+    undefined_positional=False,
+    help_def_type=True,
+)
+```
+
+<!-- termynal -->
+```
+$ python my_app.py -h
+usage: MyApp [-h] --arg_int ARG_INT [--arg_float ARG_FLOAT]
+
+options:
+  -h, --help            show this help message and exit
+  --arg_int ARG_INT     [int]
+  --arg_float ARG_FLOAT
+                        [float] default: 0.1
+```
+
 ## Examples
 
 You can see examples at `examples` folder - Same examples as at python docs and tutorial for argparse.
```

### Comparing `argparse_pydantic-0.1.2/src/argparse_pydantic.egg-info/SOURCES.txt` & `argparse_pydantic-0.1.3/src/argparse_pydantic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `argparse_pydantic-0.1.2/tests/test_add_argument_action.py` & `argparse_pydantic-0.1.3/tests/test_add_argument_action.py`

 * *Files identical despite different names*

### Comparing `argparse_pydantic-0.1.2/tests/test_add_argument_flag.py` & `argparse_pydantic-0.1.3/tests/test_add_argument_flag.py`

 * *Files identical despite different names*

### Comparing `argparse_pydantic-0.1.2/tests/test_add_argument_json_schema_extra.py` & `argparse_pydantic-0.1.3/tests/test_add_argument_json_schema_extra.py`

 * *Files identical despite different names*

### Comparing `argparse_pydantic-0.1.2/tests/test_add_argument_simple.py` & `argparse_pydantic-0.1.3/tests/test_add_argument_simple.py`

 * *Files identical despite different names*

### Comparing `argparse_pydantic-0.1.2/tests/test_core_base.py` & `argparse_pydantic-0.1.3/tests/test_core_base.py`

 * *Files identical despite different names*

### Comparing `argparse_pydantic-0.1.2/tests/test_create_parser.py` & `argparse_pydantic-0.1.3/tests/test_create_parser.py`

 * *Files identical despite different names*

### Comparing `argparse_pydantic-0.1.2/tests/test_parse_args.py` & `argparse_pydantic-0.1.3/tests/test_parse_args.py`

 * *Files identical despite different names*

### Comparing `argparse_pydantic-0.1.2/tests/test_test_tools.py` & `argparse_pydantic-0.1.3/tests/test_test_tools.py`

 * *Files identical despite different names*

