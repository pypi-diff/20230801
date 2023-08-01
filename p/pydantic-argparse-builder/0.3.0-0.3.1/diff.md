# Comparing `tmp/pydantic_argparse_builder-0.3.0.tar.gz` & `tmp/pydantic_argparse_builder-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_argparse_builder-0.3.0.tar", max compression
+gzip compressed data, was "pydantic_argparse_builder-0.3.1.tar", max compression
```

## Comparing `pydantic_argparse_builder-0.3.0.tar` & `pydantic_argparse_builder-0.3.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11336 2023-03-07 12:04:41.362499 pydantic_argparse_builder-0.3.0/LICENSE
--rw-r--r--   0        0        0      424 2023-03-21 09:42:16.517986 pydantic_argparse_builder-0.3.0/pydantic_argparse_builder/__init__.py
--rw-r--r--   0        0        0       22 2023-08-01 15:06:03.606570 pydantic_argparse_builder-0.3.0/pydantic_argparse_builder/__version__.py
--rw-r--r--   0        0        0     3126 2023-08-01 15:05:48.751829 pydantic_argparse_builder-0.3.0/pydantic_argparse_builder/cli.py
--rw-r--r--   0        0        0      344 2023-05-14 00:56:39.885312 pydantic_argparse_builder-0.3.0/pydantic_argparse_builder/config.py
--rw-r--r--   0        0        0     8808 2023-08-01 15:05:48.752836 pydantic_argparse_builder-0.3.0/pydantic_argparse_builder/parse.py
--rw-r--r--   0        0        0      537 2023-08-01 15:05:48.752836 pydantic_argparse_builder-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3304 2023-08-01 15:05:48.751829 pydantic_argparse_builder-0.3.0/README.md
--rw-r--r--   0        0        0     3921 1970-01-01 00:00:00.000000 pydantic_argparse_builder-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11336 2023-03-07 12:04:41.362499 pydantic_argparse_builder-0.3.1/LICENSE
+-rw-r--r--   0        0        0      424 2023-03-21 09:42:16.517986 pydantic_argparse_builder-0.3.1/pydantic_argparse_builder/__init__.py
+-rw-r--r--   0        0        0       22 2023-08-01 15:06:03.606570 pydantic_argparse_builder-0.3.1/pydantic_argparse_builder/__version__.py
+-rw-r--r--   0        0        0     3126 2023-08-01 15:05:48.751829 pydantic_argparse_builder-0.3.1/pydantic_argparse_builder/cli.py
+-rw-r--r--   0        0        0      402 2023-08-01 16:19:15.189523 pydantic_argparse_builder-0.3.1/pydantic_argparse_builder/config.py
+-rw-r--r--   0        0        0     8949 2023-08-01 16:30:50.225309 pydantic_argparse_builder-0.3.1/pydantic_argparse_builder/parse.py
+-rw-r--r--   0        0        0      567 2023-08-01 16:31:25.619909 pydantic_argparse_builder-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     3304 2023-08-01 15:05:48.751829 pydantic_argparse_builder-0.3.1/README.md
+-rw-r--r--   0        0        0     3971 1970-01-01 00:00:00.000000 pydantic_argparse_builder-0.3.1/PKG-INFO
```

### Comparing `pydantic_argparse_builder-0.3.0/LICENSE` & `pydantic_argparse_builder-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_argparse_builder-0.3.0/pydantic_argparse_builder/cli.py` & `pydantic_argparse_builder-0.3.1/pydantic_argparse_builder/cli.py`

 * *Files identical despite different names*

### Comparing `pydantic_argparse_builder-0.3.0/pydantic_argparse_builder/parse.py` & `pydantic_argparse_builder-0.3.1/pydantic_argparse_builder/parse.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,19 @@
 from argparse import Action, ArgumentParser
 from copy import deepcopy
 from enum import Enum
-from typing import Any, Dict, List, Type, Union, get_args, get_origin, Literal
+from typing import Any, Dict, List, Type, Union, get_args, get_origin, Literal, Mapping
 
-from pydantic import BaseModel
-from pydantic.fields import (
-    SHAPE_DICT,
-    SHAPE_LIST,
-    SHAPE_MAPPING,
-    SHAPE_SET,
-    SHAPE_TUPLE,
-    ModelField,
-    Undefined,
-)
-from pydantic.typing import is_literal_type, is_union
+from pydantic import BaseModel, ConfigDict
+from pydantic.fields import FieldInfo, PydanticUndefined
 
-from pydantic_argparse_builder.config import _CliConfig
 
-
-def get_model_field(model: Type[BaseModel]) -> Dict[str, ModelField]:
+def get_model_field(model: Type[BaseModel]) -> Dict[str, FieldInfo]:
     """Get field info."""
-    return {field.name: field for field in model.__fields__.values()}
+    return {name: field for name, field in model.model_fields.items()}
 
 
 def get_groupby_field_names(model: Type[BaseModel]) -> Dict[str, str]:
     """Get field names for groups
 
     Parameters
     ----------
@@ -103,201 +92,213 @@
     parse_nested_model: bool
         If True, nested model is also parsed, by default True
     Returns
     -------
     ArgumentParser
         Argument parser object
     """
+    model_config = model.model_config
     groups = get_groupby_field_names(model) if groupby_inherit else {}
     cache_parsers = {}
     exist_truncate_args = deepcopy(exclude_truncated_args)
     for name, field in get_model_field(model).items():
         if name in excludes:
             continue
 
         if (
             parse_nested_model
-            and isinstance(field.type_, type)
-            and issubclass(field.type_, BaseModel)
+            and isinstance(field.annotation, type)
+            and issubclass(field.annotation, BaseModel)
         ):
             build_parser(
                 parser,
-                field.type_,
+                field.annotation,
                 excludes=excludes,
                 groupby_inherit=True,
                 exclude_truncated_args=exclude_truncated_args,
                 parse_nested_model=parse_nested_model,
             )
             continue
 
         kwargs = {}
 
         # Set option of multiple arguments
         kwargs.update(**_parse_shape_args(name, field))
 
         # Set default value
-        if field.field_info.default is not Undefined:
+        if field.default is not PydanticUndefined:
             kwargs["default"] = field.get_default()
 
         # If groupby is enabled, create a new parser for each group
         if name in groups:
             group_name = groups[name]
             if group_name not in cache_parsers:
                 _parser = parser.add_argument_group(group_name)
                 cache_parsers[group_name] = _parser
             else:
                 _parser = cache_parsers[group_name]
         else:
             _parser = parser
 
-        kwargs["help"] = field.field_info.description
+        kwargs["help"] = field.description
         # Set option args
-        if field.type_ is bool:
+        if field.annotation is bool:
             # Special case for boolean
             del kwargs["type"]
             kwargs["dest"] = name
 
-            if field.required:
+            if field.is_required():
                 # Create both enable and disable option
-                _add_both_options(_parser, name, field, kwargs, config=model.Config)
+                _add_both_options(
+                    _parser, name, field, kwargs, config=model.model_config
+                )
             else:
                 # Create either one option.
-                _add_either_option(_parser, name, field, kwargs, config=model.Config)
+                _add_either_option(
+                    _parser, name, field, kwargs, config=model.model_config
+                )
         else:
             # default case for other types
-            args = get_cli_names(name, field, prefix="--")
+            args = get_cli_names(name, field, model_config, prefix="--")
             # Set truncateiated parameter
             if auto_truncate:
                 truncate_arg = f"-{args[0].strip('-')[0]}"
                 if truncate_arg not in exist_truncate_args:
                     args.append(truncate_arg)
                     exist_truncate_args.append(truncate_arg)
 
             _parser.add_argument(
                 *args,
-                required=field.required,
+                required=field.is_required(),
                 **kwargs,
             )
 
     return parser
 
 
-def get_cli_names(name: str, field: ModelField, prefix: str = "") -> List[str]:
+def get_cli_names(
+    name: str, field: FieldInfo, model_config: ConfigDict, prefix: str = ""
+) -> List[str]:
     """Create cli string from field name.
 
     Parameters
     ----------
     name : str
         field name
-    field : ModelField
+    field : FieldInfo
         field object
     prefix : str, optional
         prefix of the default arguments, by default ""
 
     Returns
     -------
     List[str]
         list of cli arguments
     """
-    names = field.field_info.extra.get("cli", None)
+    names = _get_extra(field, model_config, "cli", None)
     if names is None:
         names = []
-        if field.has_alias:
+        if field.alias is not None:
             names.append(prefix + field.alias.replace("_", "-"))
         names.append(prefix + name.replace("_", "-"))
     return names
 
 
-def _parse_shape_args(name: str, field: ModelField) -> dict:
+def _parse_shape_args(name: str, field: FieldInfo) -> dict:
     kwargs = {}
-    kwargs["type"] = field.type_
-    if field.shape in (SHAPE_LIST, SHAPE_SET):
-        if field.required:
+    kwargs["type"] = field.annotation
+    origin = get_origin(field.annotation)
+    field.discriminator
+    if origin is list or origin is set:
+        kwargs["type"] = get_args(field.annotation)[0]
+        if field.is_required():
             kwargs["nargs"] = "+"
         else:
             kwargs["nargs"] = "*"
-    elif field.shape in (SHAPE_DICT, SHAPE_MAPPING):
+    elif origin is dict or origin is Mapping:
         kwargs["action"] = StoreKeywordParam
         kwargs["type"] = str
-        if field.required:
+        if field.is_required():
             kwargs["nargs"] = "+"
         else:
             kwargs["nargs"] = "*"
-    elif field.shape == SHAPE_TUPLE:
-        args = get_args(field.type_)
+    elif origin is tuple:
+        args = get_args(field.annotation)
         kwargs["type"] = args[0]
         kwargs["nargs"] = len(args)
-    elif field.type_ is type and issubclass(field.type_, Enum):
-        kwargs["choices"] = list(field.type_)
-    elif is_literal_type(field.type_):
+    elif origin is type and issubclass(field.annotation, Enum):
+        kwargs["choices"] = list(field.annotation)
+    elif origin is Literal:
         del kwargs["type"]
-        kwargs["choices"] = get_args(field.type_)
-    elif is_union(get_origin(field.type_)):
+        kwargs["choices"] = get_args(field.annotation)
+    elif origin is Union:
         kwargs["type"] = str  # TODO: Support union type
     return kwargs
 
 
 def _add_both_options(
     parser: ArgumentParser,
     name: str,
-    field: ModelField,
+    field: FieldInfo,
     kwargs: Dict[str, Any],
-    config: _CliConfig,
+    config: ConfigDict,
 ):
     mutual = parser.add_mutually_exclusive_group(required=True)
 
     args = get_cli_names(
         name,
         field,
-        prefix=field.field_info.extra.get(
-            "cli_enable_prefix", getattr(config, "cli_enable_prefix", "--enable-")
-        ),
+        config,
+        prefix=_get_extra(field, config, "cli_enable_prefix", "--enable-"),
     )
     kwargs["action"] = "store_true"
     mutual.add_argument(
         *args,
         **kwargs,
     )
     args = get_cli_names(
         name,
         field,
-        prefix=field.field_info.extra.get(
-            "cli_disable_prefix", getattr(config, "cli_disable_prefix", "--disable-")
-        ),
+        config,
+        prefix=_get_extra(field, config, "cli_disable_prefix", "--disable-"),
     )
     kwargs["action"] = "store_false"
     mutual.add_argument(
         *args,
         **kwargs,
     )
 
 
 def _add_either_option(
     parser: ArgumentParser,
     name: str,
-    field: ModelField,
+    field: FieldInfo,
     kwargs: Dict[str, Any],
-    config: _CliConfig,
+    config: ConfigDict,
 ):
     if kwargs["default"]:
         args = get_cli_names(
             name,
             field,
-            prefix=field.field_info.extra.get(
-                "cli_disable_prefix",
-                getattr(config, "cli_disable_prefix", "--disable-"),
-            ),
+            config,
+            prefix=_get_extra(field, config, "cli_disable_prefix", "--disable-"),
         )
         kwargs["action"] = "store_false"
     else:
         args = get_cli_names(
             name,
             field,
-            prefix=field.field_info.extra.get(
-                "cli_enable_prefix", getattr(config, "cli_enable_prefix", "--enable-")
-            ),
+            config,
+            prefix=_get_extra(field, config, "cli_enable_prefix", "--enable-"),
         )
         kwargs["action"] = "store_true"
     parser.add_argument(
         *args,
         **kwargs,
     )
+
+
+def _get_extra(field: FieldInfo, config: ConfigDict, key: str, default: Any = None):
+    if field.json_schema_extra is None:
+        return config.get(key, default)
+    else:
+        return field.json_schema_extra.get(key, default)
```

### Comparing `pydantic_argparse_builder-0.3.0/pyproject.toml` & `pydantic_argparse_builder-0.3.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [tool.poetry]
 name = "pydantic-argparse-builder"
-version = "0.3.0"
+version = "0.3.1"
 description = "Build ArgumentParser from pydantic model."
 authors = ["elda27 <kaz.birdstick@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{ include = "pydantic_argparse_builder" }]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pydantic = "^2.0.0"
+pydantic-settings = "^2.0.2"
 
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.0.0"
 pytest = "^7.2.1"
 pytest-cov = "^4.0.0"
```

### Comparing `pydantic_argparse_builder-0.3.0/README.md` & `pydantic_argparse_builder-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pydantic_argparse_builder-0.3.0/PKG-INFO` & `pydantic_argparse_builder-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: pydantic-argparse-builder
-Version: 0.3.0
+Version: 0.3.1
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
 Requires-Dist: pydantic (>=2.0.0,<3.0.0)
+Requires-Dist: pydantic-settings (>=2.0.2,<3.0.0)
 Description-Content-Type: text/markdown
 
 # pydantic-argparse-builder
 [![Python](https://img.shields.io/pypi/pyversions/pydantic-argparse-builder.svg)](https://pypi.org/project/pydantic-argparse-builder/)
 [![PyPI version](https://badge.fury.io/py/pydantic-argparse-builder.svg)](https://badge.fury.io/py/pydantic-argparse-builder)
 [![codecov](https://codecov.io/gh/elda27/pydantic_argparse_builder/branch/main/graph/badge.svg?token=GLqGNtE7Df)](https://codecov.io/gh/elda27/pydantic_argparse_builder)
 [![Downloads](https://static.pepy.tech/badge/pydantic-argparse-builder)](https://pepy.tech/project/pydantic-argparse-builder)
```

