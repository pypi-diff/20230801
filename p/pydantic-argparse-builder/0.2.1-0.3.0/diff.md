# Comparing `tmp/pydantic_argparse_builder-0.2.1.tar.gz` & `tmp/pydantic_argparse_builder-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_argparse_builder-0.2.1.tar", max compression
+gzip compressed data, was "pydantic_argparse_builder-0.3.0.tar", max compression
```

## Comparing `pydantic_argparse_builder-0.2.1.tar` & `pydantic_argparse_builder-0.3.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11336 2023-03-07 12:04:41.362499 pydantic_argparse_builder-0.2.1/LICENSE
--rw-r--r--   0        0        0      424 2023-03-21 09:00:19.334484 pydantic_argparse_builder-0.2.1/pydantic_argparse_builder/__init__.py
--rw-r--r--   0        0        0       22 2023-03-21 05:18:10.814486 pydantic_argparse_builder-0.2.1/pydantic_argparse_builder/__version__.py
--rw-r--r--   0        0        0     3106 2023-03-21 05:16:47.430587 pydantic_argparse_builder-0.2.1/pydantic_argparse_builder/cli.py
--rw-r--r--   0        0        0      344 2023-03-21 06:05:14.774253 pydantic_argparse_builder-0.2.1/pydantic_argparse_builder/config.py
--rw-r--r--   0        0        0     8173 2023-03-21 09:13:02.322773 pydantic_argparse_builder-0.2.1/pydantic_argparse_builder/parse.py
--rw-r--r--   0        0        0      536 2023-03-21 05:17:52.722346 pydantic_argparse_builder-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2836 2023-03-07 12:04:41.363493 pydantic_argparse_builder-0.2.1/README.md
--rw-r--r--   0        0        0     3454 1970-01-01 00:00:00.000000 pydantic_argparse_builder-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    11336 2023-03-07 12:04:41.362499 pydantic_argparse_builder-0.3.0/LICENSE
+-rw-r--r--   0        0        0      424 2023-03-21 09:42:16.517986 pydantic_argparse_builder-0.3.0/pydantic_argparse_builder/__init__.py
+-rw-r--r--   0        0        0       22 2023-08-01 15:06:03.606570 pydantic_argparse_builder-0.3.0/pydantic_argparse_builder/__version__.py
+-rw-r--r--   0        0        0     3126 2023-08-01 15:05:48.751829 pydantic_argparse_builder-0.3.0/pydantic_argparse_builder/cli.py
+-rw-r--r--   0        0        0      344 2023-05-14 00:56:39.885312 pydantic_argparse_builder-0.3.0/pydantic_argparse_builder/config.py
+-rw-r--r--   0        0        0     8808 2023-08-01 15:05:48.752836 pydantic_argparse_builder-0.3.0/pydantic_argparse_builder/parse.py
+-rw-r--r--   0        0        0      537 2023-08-01 15:05:48.752836 pydantic_argparse_builder-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3304 2023-08-01 15:05:48.751829 pydantic_argparse_builder-0.3.0/README.md
+-rw-r--r--   0        0        0     3921 1970-01-01 00:00:00.000000 pydantic_argparse_builder-0.3.0/PKG-INFO
```

### Comparing `pydantic_argparse_builder-0.2.1/LICENSE` & `pydantic_argparse_builder-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_argparse_builder-0.2.1/pydantic_argparse_builder/cli.py` & `pydantic_argparse_builder-0.3.0/pydantic_argparse_builder/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import inspect
 from argparse import ArgumentParser
 from contextlib import contextmanager
 from functools import wraps
-from typing import Any, Callable, Dict, Tuple, Type
+from typing import Any, Callable, Dict, Tuple, Type, Union
 
 from pydantic import BaseModel
 from typing_extensions import ContextManager
 
 from pydantic_argparse_builder.parse import build_parser
 
-_registry: Dict[str, Tuple[Callable[[BaseModel], None]]] = {}
+_registry: Dict[Union[str, None], Tuple[Callable[[BaseModel], None]]] = {}
 
 
 def get_command_model(func: Callable[[BaseModel], None]) -> Type[BaseModel]:
     """Get model from command function
 
     Parameters
     ----------
```

### Comparing `pydantic_argparse_builder-0.2.1/pydantic_argparse_builder/parse.py` & `pydantic_argparse_builder-0.3.0/pydantic_argparse_builder/parse.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from argparse import Action, ArgumentParser
 from copy import deepcopy
 from enum import Enum
-from typing import Any, Dict, List, Type, Union, get_args, get_origin
+from typing import Any, Dict, List, Type, Union, get_args, get_origin, Literal
 
 from pydantic import BaseModel
 from pydantic.fields import (
     SHAPE_DICT,
     SHAPE_LIST,
     SHAPE_MAPPING,
     SHAPE_SET,
@@ -55,15 +55,15 @@
     def __call__(
         self,
         parser: ArgumentParser,
         namespace: Any,
         values: Union[str, List[str]],
         option_strings=None,
     ):
-        param_dict = getattr(namespace, self.dest, [])
+        param_dict = getattr(namespace, self.dest)
         if param_dict is None:
             param_dict = {}
         if not isinstance(values, list):
             values = [values]
 
         for value in values:
             parts = value.split("=")
@@ -78,14 +78,15 @@
 def build_parser(
     parser: ArgumentParser,
     model: Type[BaseModel],
     excludes: List[str] = [],
     auto_truncate: bool = True,
     groupby_inherit: bool = True,
     exclude_truncated_args: List[str] = ["-h"],
+    parse_nested_model: bool = True,
 ) -> ArgumentParser:
     """Create argument parser from pydantic model.
 
     Parameters
     ----------
     parser : ArgumentParser
         Argument parser object
@@ -95,27 +96,43 @@
         Exclude field, by default []
     auto_truncate : bool, optional
         Enable truncated parameter such as `-h`, by default True
     groupby_inherit: bool, optional
         If True, inherited basemodels are grouped by class name, by default True
     exclude_truncated_args: List[str], optional
         Exclude truncated arguments, by default ["-h"]
-
+    parse_nested_model: bool
+        If True, nested model is also parsed, by default True
     Returns
     -------
     ArgumentParser
         Argument parser object
     """
     groups = get_groupby_field_names(model) if groupby_inherit else {}
     cache_parsers = {}
     exist_truncate_args = deepcopy(exclude_truncated_args)
     for name, field in get_model_field(model).items():
         if name in excludes:
             continue
 
+        if (
+            parse_nested_model
+            and isinstance(field.type_, type)
+            and issubclass(field.type_, BaseModel)
+        ):
+            build_parser(
+                parser,
+                field.type_,
+                excludes=excludes,
+                groupby_inherit=True,
+                exclude_truncated_args=exclude_truncated_args,
+                parse_nested_model=parse_nested_model,
+            )
+            continue
+
         kwargs = {}
 
         # Set option of multiple arguments
         kwargs.update(**_parse_shape_args(name, field))
 
         # Set default value
         if field.field_info.default is not Undefined:
@@ -143,18 +160,18 @@
                 # Create both enable and disable option
                 _add_both_options(_parser, name, field, kwargs, config=model.Config)
             else:
                 # Create either one option.
                 _add_either_option(_parser, name, field, kwargs, config=model.Config)
         else:
             # default case for other types
-            args = [f"--{name.replace('_', '-')}"]
+            args = get_cli_names(name, field, prefix="--")
             # Set truncateiated parameter
             if auto_truncate:
-                truncate_arg = f"-{name[0]}"
+                truncate_arg = f"-{args[0].strip('-')[0]}"
                 if truncate_arg not in exist_truncate_args:
                     args.append(truncate_arg)
                     exist_truncate_args.append(truncate_arg)
 
             _parser.add_argument(
                 *args,
                 required=field.required,
@@ -179,17 +196,18 @@
     Returns
     -------
     List[str]
         list of cli arguments
     """
     names = field.field_info.extra.get("cli", None)
     if names is None:
-        names = [prefix + name.replace("_", "-")]
+        names = []
         if field.has_alias:
             names.append(prefix + field.alias.replace("_", "-"))
+        names.append(prefix + name.replace("_", "-"))
     return names
 
 
 def _parse_shape_args(name: str, field: ModelField) -> dict:
     kwargs = {}
     kwargs["type"] = field.type_
     if field.shape in (SHAPE_LIST, SHAPE_SET):
```

### Comparing `pydantic_argparse_builder-0.2.1/pyproject.toml` & `pydantic_argparse_builder-0.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "pydantic-argparse-builder"
-version = "0.2.1"
+version = "0.3.0"
 description = "Build ArgumentParser from pydantic model."
 authors = ["elda27 <kaz.birdstick@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
-packages = [{include = "pydantic_argparse_builder"}]
+packages = [{ include = "pydantic_argparse_builder" }]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-pydantic = "^1.10.5"
+pydantic = "^2.0.0"
 
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.0.0"
 pytest = "^7.2.1"
 pytest-cov = "^4.0.0"
```

### Comparing `pydantic_argparse_builder-0.2.1/PKG-INFO` & `pydantic_argparse_builder-0.3.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: pydantic-argparse-builder
-Version: 0.2.1
+Version: 0.3.0
 Summary: Build ArgumentParser from pydantic model.
 License: Apache-2.0
 Author: elda27
 Author-email: kaz.birdstick@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pydantic (>=1.10.5,<2.0.0)
+Requires-Dist: pydantic (>=2.0.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # pydantic-argparse-builder
 [![Python](https://img.shields.io/pypi/pyversions/pydantic-argparse-builder.svg)](https://pypi.org/project/pydantic-argparse-builder/)
 [![PyPI version](https://badge.fury.io/py/pydantic-argparse-builder.svg)](https://badge.fury.io/py/pydantic-argparse-builder)
 [![codecov](https://codecov.io/gh/elda27/pydantic_argparse_builder/branch/main/graph/badge.svg?token=GLqGNtE7Df)](https://codecov.io/gh/elda27/pydantic_argparse_builder)
 [![Downloads](https://static.pepy.tech/badge/pydantic-argparse-builder)](https://pepy.tech/project/pydantic-argparse-builder)
@@ -90,12 +90,27 @@
 positional arguments:
   {alpha,beta}
 
 optional arguments:
   -h, --help    show this help message and exit
 ```
 
+## Additional config
+Behaviour of pydantic can be controlled via the `Config` class or extra arguments of `Field`.
+`Config` is affected all fields.
+Extra arguments of `Field` is affected specific field. 
+
+
+<dl>
+  <dt><code>cli_disable_prefix</code></dt>
+  <dd>Prefix of argument of boolean type for `store_false`. Default to <code>--disable-</code></dd>
+
+  <dt><code>cli_enable_prefix</code></dt>
+  <dd>Prefix of argument of boolean type for `store_true`. Default to <code>--enable-</code></dd>
+
+</dl>
+
+
 ## Future works
 
-- [ ]: High level api such as click
 - [ ]: Options completion for bash
```

