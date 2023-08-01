# Comparing `tmp/pypeline-python-0.1.1.tar.gz` & `tmp/pypeline-python-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypeline-python-0.1.1.tar", last modified: Wed Jun 28 15:29:04 2023, max compression
+gzip compressed data, was "pypeline-python-0.1.2.tar", last modified: Tue Aug  1 16:49:22 2023, max compression
```

## Comparing `pypeline-python-0.1.1.tar` & `pypeline-python-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:04.332300 pypeline-python-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-28 15:28:53.000000 pypeline-python-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-28 15:29:04.332300 pypeline-python-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-06-28 15:28:53.000000 pypeline-python-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:04.328300 pypeline-python-0.1.1/pypeline_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-28 15:29:04.000000 pypeline-python-0.1.1/pypeline_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-28 15:29:04.000000 pypeline-python-0.1.1/pypeline_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 15:29:04.000000 pypeline-python-0.1.1/pypeline_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-28 15:29:04.000000 pypeline-python-0.1.1/pypeline_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-28 15:29:04.000000 pypeline-python-0.1.1/pypeline_python.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:04.332300 pypeline-python-0.1.1/pypipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-28 15:28:53.000000 pypeline-python-0.1.1/pypipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-28 15:28:53.000000 pypeline-python-0.1.1/pypipeline/action.py
--rw-r--r--   0 runner    (1001) docker     (123)    11083 2023-06-28 15:28:53.000000 pypeline-python-0.1.1/pypipeline/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-28 15:28:53.000000 pypeline-python-0.1.1/pypipeline/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-06-28 15:28:53.000000 pypeline-python-0.1.1/pypipeline/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-28 15:28:53.000000 pypeline-python-0.1.1/pypipeline/item.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-28 15:28:53.000000 pypeline-python-0.1.1/pypipeline/items_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-06-28 15:28:53.000000 pypeline-python-0.1.1/pypipeline/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-28 15:28:53.000000 pypeline-python-0.1.1/pypipeline/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-06-28 15:28:53.000000 pypeline-python-0.1.1/pypipeline/util.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 15:29:04.332300 pypeline-python-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-28 15:28:53.000000 pypeline-python-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:49:22.378436 pypeline-python-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-01 16:49:13.000000 pypeline-python-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-08-01 16:49:22.378436 pypeline-python-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-08-01 16:49:13.000000 pypeline-python-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:49:22.378436 pypeline-python-0.1.2/pypeline_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-08-01 16:49:22.000000 pypeline-python-0.1.2/pypeline_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-08-01 16:49:22.000000 pypeline-python-0.1.2/pypeline_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 16:49:22.000000 pypeline-python-0.1.2/pypeline_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-01 16:49:22.000000 pypeline-python-0.1.2/pypeline_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-01 16:49:22.000000 pypeline-python-0.1.2/pypeline_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:49:22.378436 pypeline-python-0.1.2/pypipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-08-01 16:49:13.000000 pypeline-python-0.1.2/pypipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-08-01 16:49:13.000000 pypeline-python-0.1.2/pypipeline/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14325 2023-08-01 16:49:13.000000 pypeline-python-0.1.2/pypipeline/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-08-01 16:49:13.000000 pypeline-python-0.1.2/pypipeline/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-08-01 16:49:13.000000 pypeline-python-0.1.2/pypipeline/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-08-01 16:49:13.000000 pypeline-python-0.1.2/pypipeline/item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-08-01 16:49:13.000000 pypeline-python-0.1.2/pypipeline/items_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-08-01 16:49:13.000000 pypeline-python-0.1.2/pypipeline/modifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-08-01 16:49:13.000000 pypeline-python-0.1.2/pypipeline/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-08-01 16:49:13.000000 pypeline-python-0.1.2/pypipeline/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 16:49:22.378436 pypeline-python-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-08-01 16:49:13.000000 pypeline-python-0.1.2/setup.py
```

### Comparing `pypeline-python-0.1.1/LICENSE` & `pypeline-python-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pypeline-python-0.1.1/PKG-INFO` & `pypeline-python-0.1.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypeline-python
-Version: 0.1.1
+Version: 0.1.2
 Summary: PyPipeline is a simple Python framework for building data processing pipelines.
 Home-page: https://github.com/zigai/py-pipeline
 Author: Žiga Ivanšek
 Author-email: ziga.ivansek@gmail.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
@@ -12,25 +12,25 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyPipeline
-[![PyPI version](https://badge.fury.io/py/py-pipeline.svg)](https://badge.fury.io/py/py-pipeline)
+[![PyPI version](https://badge.fury.io/py/pypeline-python.svg)](https://badge.fury.io/py/pypeline-python)
 ![Supported versions](https://img.shields.io/badge/python-3.10+-blue.svg)
-[![Downloads](https://static.pepy.tech/badge/py-pipeline)](https://pepy.tech/project/py-pipeline)
+[![Downloads](https://static.pepy.tech/badge/pypeline-python)](https://pepy.tech/project/pypeline-python)
 [![license](https://img.shields.io/github/license/zigai/py-pipeline.svg)](https://github.com/zigai/py-pipeline/blob/main/LICENSE)
 
 ```PyPipeline``` is a simple Python framework for building data processing pipelines.
 
 # Installation
 #### From PyPi
 ```
-pip install py-pipeline
+pip install pypeline-python
 ```
 #### From source
 ```
 pip install git+https://github.com/zigai/py-pipeline.git
 ```
 # License
 [MIT License](https://github.com/zigai/py-pipeline/blob/master/LICENSE)
```

### Comparing `pypeline-python-0.1.1/README.md` & `pypeline-python-0.1.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # PyPipeline
-[![PyPI version](https://badge.fury.io/py/py-pipeline.svg)](https://badge.fury.io/py/py-pipeline)
+[![PyPI version](https://badge.fury.io/py/pypeline-python.svg)](https://badge.fury.io/py/pypeline-python)
 ![Supported versions](https://img.shields.io/badge/python-3.10+-blue.svg)
-[![Downloads](https://static.pepy.tech/badge/py-pipeline)](https://pepy.tech/project/py-pipeline)
+[![Downloads](https://static.pepy.tech/badge/pypeline-python)](https://pepy.tech/project/pypeline-python)
 [![license](https://img.shields.io/github/license/zigai/py-pipeline.svg)](https://github.com/zigai/py-pipeline/blob/main/LICENSE)
 
 ```PyPipeline``` is a simple Python framework for building data processing pipelines.
 
 # Installation
 #### From PyPi
 ```
-pip install py-pipeline
+pip install pypeline-python
 ```
 #### From source
 ```
 pip install git+https://github.com/zigai/py-pipeline.git
 ```
 # License
 [MIT License](https://github.com/zigai/py-pipeline/blob/master/LICENSE)
```

### Comparing `pypeline-python-0.1.1/pypeline_python.egg-info/PKG-INFO` & `pypeline-python-0.1.2/pypeline_python.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypeline-python
-Version: 0.1.1
+Version: 0.1.2
 Summary: PyPipeline is a simple Python framework for building data processing pipelines.
 Home-page: https://github.com/zigai/py-pipeline
 Author: Žiga Ivanšek
 Author-email: ziga.ivansek@gmail.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
@@ -12,25 +12,25 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyPipeline
-[![PyPI version](https://badge.fury.io/py/py-pipeline.svg)](https://badge.fury.io/py/py-pipeline)
+[![PyPI version](https://badge.fury.io/py/pypeline-python.svg)](https://badge.fury.io/py/pypeline-python)
 ![Supported versions](https://img.shields.io/badge/python-3.10+-blue.svg)
-[![Downloads](https://static.pepy.tech/badge/py-pipeline)](https://pepy.tech/project/py-pipeline)
+[![Downloads](https://static.pepy.tech/badge/pypeline-python)](https://pepy.tech/project/pypeline-python)
 [![license](https://img.shields.io/github/license/zigai/py-pipeline.svg)](https://github.com/zigai/py-pipeline/blob/main/LICENSE)
 
 ```PyPipeline``` is a simple Python framework for building data processing pipelines.
 
 # Installation
 #### From PyPi
 ```
-pip install py-pipeline
+pip install pypeline-python
 ```
 #### From source
 ```
 pip install git+https://github.com/zigai/py-pipeline.git
 ```
 # License
 [MIT License](https://github.com/zigai/py-pipeline/blob/master/LICENSE)
```

### Comparing `pypeline-python-0.1.1/pypipeline/action.py` & `pypeline-python-0.1.2/pypipeline/action.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,52 +1,124 @@
 import inspect
+from typing import Any, Dict, Type
+
+from objinspect import Class
+from stdl.str_u import kebab_case
 
 from pypipeline.item import Item
 
 
 class Action:
     priority: int = 1
     abbrev: str | None = None
     type: str | None = None
+    dict_exclude: list[str] = []
+    allow_autoparse: bool = True
 
     def __init__(self) -> None:
         self.validate()
 
+    @classmethod
+    @property
+    def name(cls):
+        return kebab_case(cls.__name__)
+
+    def dict(self) -> dict[str, Any]:
+        return {
+            "name": self.name,
+            "type": self.type,
+            "args": self.get_args(),
+        }
+
+    def get_args(self) -> Dict[str, Any]:
+        cls = Class(self.__class__)
+        init_args = cls.init_args
+        args = {}
+        if not init_args:
+            return {}
+
+        for i in init_args:
+            if i.name in self.dict_exclude:
+                continue
+            args[i.name] = getattr(self, i.name)
+        return args
+
     def __repr__(self):
         vars_str = ", ".join([f"{i}={j}" for i, j in vars(self).items()])
         return f"{self.__class__.__name__}({vars_str})"
 
     def __lt__(self, other):
         if isinstance(other, Action):
             return self.priority < other.priority
+        raise NotImplementedError
+
+    def validate(self) -> None:
+        """
+        Should raise an Error if the action is invalid.
+        """
+        return
+
+    def process(self, item: Item) -> Item | bool:
+        raise NotImplementedError
+
+    def eval(self, item: Item) -> Item:
+        raise NotImplementedError
+
+    @classmethod
+    def parse(cls, val: str | None = None) -> "Action":
         return NotImplemented
 
     @classmethod
     def is_parsable(cls):
         try:
             if cls.parse() is NotImplemented:
                 return False
             return True
         except NotImplementedError:
             return False
         except TypeError:
             return True
 
     @classmethod
-    def get_docstr(cls) -> str:
+    def get_docstring(cls) -> str:
         return inspect.getdoc(cls) or ""
 
-    def process(self, item: Item) -> Item | bool:
-        return NotImplemented
+
+class Modifier(Action):
+    type = "modifier"
+
+    def process(self, item: Item) -> Item:
+        raise NotImplementedError
 
     def eval(self, item: Item) -> Item:
-        return NotImplemented
+        return self.process(item)
 
-    @classmethod
-    def parse(cls, val: str | None = None) -> "Action":
-        return NotImplemented
 
-    def validate(self) -> None:
-        return
+class Filter(Action):
+    type = "filter"
+    dict_exclude: list[str] = ["invert"]
+
+    def __init__(self, invert=False) -> None:
+        self.invert = invert
+        super().__init__()
+
+    def eval(self, item: Item) -> Item:
+        res = self.process(item)
+        if self.invert:
+            res = not res
+        item.discarded = not res
+        return item
+
+
+def get_actions_dict(actions: list[Type[Action]]) -> dict[str, Type[Action]]:
+    return {i.name: i for i in actions}
+
+
+def parse_action(data: dict, actions: dict[str, Type[Action]]) -> Action:
+    name = data["name"]
+    if name not in actions:
+        raise ValueError(f"Unknown action: '{name}'")
+    cls = actions[name]
+    return cls(**data["args"])
 
 
-__all__ = ["Action"]
+__all__ = ["Action", "Modifier", "Filter", "parse_action"]
```

### Comparing `pypeline-python-0.1.1/pypipeline/cli.py` & `pypeline-python-0.1.2/pypipeline/cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import inspect
 import sys
 from functools import cached_property
 from multiprocessing import cpu_count
-from typing import Literal
+from typing import Literal, Type
 
 import docstring_parser
+from objinspect import Class, Method
 from stdl.fs import read_stdin
 from stdl.str_u import colored, kebab_case
+from strto import get_parser
 
-from pypipeline.action import Action
+from pypipeline.action import Action, get_actions_dict
 from pypipeline.constants import (
     CLI_HELP_INDENT,
     CLI_MAX_LJUST,
     CLI_MIN_LJUST,
     FILTER_INVERT_SUFFIX,
     FLAG_PREFIX_LONG,
     FLAG_PREFIX_SHORT,
@@ -20,14 +22,98 @@
     ExitCodes,
 )
 from pypipeline.item import Item
 from pypipeline.items_container import ItemsContainer
 from pypipeline.pipeline import Pipeline
 from pypipeline.util import fill_missing_abbreviations, get_executable_name, get_taken_abbreviations
 
+TYPE_PARSER = get_parser()
+
+
+def flag_remove_prefix(flag: str) -> str:
+    if flag.startswith(FLAG_PREFIX_LONG):
+        return flag[len(FLAG_PREFIX_LONG) :]
+    if flag.startswith(FLAG_PREFIX_SHORT):
+        return flag[len(FLAG_PREFIX_SHORT) :]
+    return flag
+
+
+class ActionAutoParser:
+    def __init__(self, action: Type[Action]) -> None:
+        self.action = action
+        self.has_custom_parse_fn = action.is_parsable()
+        self.obj_action = Class(action)
+
+        if self.has_custom_parse_fn:
+            self.init_obj_container = Method(self.action.parse, self.action)
+            self.init_args = self.init_obj_container.params
+            self.init_fn = self.action.parse
+        else:
+            self.init_args = self.obj_action.init_args
+            self.init_obj_container = self.obj_action.init_method
+            self.init_fn = self.action
+
+        self.arg_index = 0
+        self.args = {}
+        self.positionals, self.optionals = self.get_expected_num_of_args()
+
+    def positionals_done(self) -> bool:
+        return self.arg_index >= self.positionals
+
+    def get_expected_num_of_args(self) -> tuple[int, int]:
+        if self.init_args is None or len(self.init_args) == 0:
+            return 0, 0
+
+        positionals, optionals = 0, 0
+        for arg in self.init_args:
+            if arg.name == "invert":
+                continue
+            if arg.is_optional:
+                optionals += 1
+            else:
+                positionals += 1
+        return positionals, optionals
+
+    def parse(self, value):
+        if self.init_args is None or len(self.init_args) == 0:
+            raise ValueError(f"Action '{self.obj_action.name}' does not take any arguments.")
+
+        if not self.positionals_done():
+            param = self.init_args[self.arg_index]
+            self.args[param.name] = TYPE_PARSER.parse(value, param.type)
+            self.arg_index += 1
+            return
+
+        if "=" in value:
+            param_name, param_value = value.split("=")
+            if param_name not in self.obj_action._methods:
+                raise ValueError(
+                    f"Action '{self.obj_action.name}' does not have an argument '{param_name}'."
+                )
+            param_obj = self.init_obj_container.get_param(param_name)  # type: ignore
+            self.args[param_name] = TYPE_PARSER.parse(param_value, param_obj.type)
+            return
+
+        param = self.init_args[self.arg_index]
+        self.args[param.name] = TYPE_PARSER.parse(value, param.type)
+        self.arg_index += 1
+
+    def parsed_max(self) -> bool:
+        return self.arg_index >= self.positionals + self.optionals
+
+    def get_action(self, inverted=False):
+        try:
+            del self.args["invert"]
+        except:
+            pass
+        instance = self.init_fn(**self.args)
+        if instance.type == "filter":
+            instance.invert = inverted  # type: ignore
+        return instance
+
 
 class ActionContainer:
     def __init__(self, action: Action) -> None:
         self.cls = action
 
     def __repr__(self) -> str:
         return f"ActionContainer(for:'{self.name}', CLI flags:'{self.cli_help_flag}')"  # type: ignore
@@ -44,15 +130,15 @@
 
     @cached_property
     def flag_long(self):
         return FLAG_PREFIX_LONG + kebab_case(self.name)
 
     @cached_property
     def description(self) -> str:
-        doc = self.cls.get_docstr()
+        doc = self.cls.get_docstring()
         if doc is None:
             return ""
         doc = docstring_parser.parse(doc)
         if doc.short_description:
             return doc.short_description
         if doc.long_description:
             return doc.long_description
@@ -97,21 +183,21 @@
 
     @cached_property
     def ljust(self) -> int:
         ljust = max(*[len(i.cli_help_flag) for i in self.actions], CLI_MIN_LJUST)
         ljust = min(ljust, CLI_MAX_LJUST)
         return ljust
 
-    def get_actions_help_section(self) -> str:
-        help_filters, help_transformers = ["\nfilters:"], ["\ntransformers:"]
+    def cli_help_section(self) -> str:
+        help_filters, help_transformers = ["\nfilters:"], ["\nmodifiers:"]
         for i in self.actions:
             h = f"{i.cli_help_flag.ljust(self.ljust)}   {i.description}"
             if i.cls.type == "filter":
                 help_filters.append(h)
-            elif i.cls.type == "transformer":
+            elif i.cls.type == "modifier":
                 help_transformers.append(h)
             else:
                 raise ValueError(i.cls.type)
 
         return "\n".join([*help_filters, *help_transformers])
 
     def get(self, name: str):
@@ -140,75 +226,72 @@
         self.executable = get_executable_name()
         self.t = cpu_count() - 1
         self.verbose = False
         self.help = None
         self.items = []
 
         self.manager = CommandLineActionsManager(actions)
-        self.help = self._get_help_str()
+        self.help = self.help_string
 
         if run:
             self.run()
 
     def log_error(self, message: str):
         print(f"{self.err_label} {message}", file=sys.stderr)
 
     def log_info(self, message: str):
         if not self.verbose:
             return
         print(f"[{self.name}] {message}")
 
-    def _remove_prefix(self, flag: str) -> str:
-        if flag.startswith(FLAG_PREFIX_LONG):
-            return flag[len(FLAG_PREFIX_LONG) :]
-        if flag.startswith(FLAG_PREFIX_SHORT):
-            return flag[len(FLAG_PREFIX_SHORT) :]
-        return flag
-
-    def _get_usage_section(self) -> str:
+    def help_usage(self) -> str:
         return f"usage: {self.executable} [--help] [-v] [--mode] MODE [-t] T [actions] [items]"
 
-    def _get_usage_notes_section(self) -> list[str]:
-        return [
+    def help_usage_notes(self) -> str:
+        notes = [
             f"\n\nnotes:",
             "  filters can be inverted by adding a '!' after the flag",
             f"  you can get help for a specific action by running '{self.executable} <action> --help'\n",
         ]
+        return "\n".join(notes)
 
-    def _get_options_help_section(self, ljust: int) -> list[str]:
-        return [
+    def help_arg_options(self, ljust: int) -> str:
+        options = [
             "\noptions:",
             f"  --help".ljust(ljust) + "   show this help message and exit",
             f"  --mode".ljust(ljust) + f"   display kept/discarded items (default: '{self.mode}')",
             f"  -t".ljust(ljust) + f"   number of threads to use (default: {self.t})",
             f"  -v, -verbose".ljust(ljust)
             + "   verbose mode (extra log messages and progress bars)",
         ]
+        return "\n".join(options)
 
-    def _get_help_str(self):
+    @property
+    def help_string(self):
         return (
-            self._get_usage_section()
+            self.help_usage()
             + self.description
             + "\n"
-            + "\n".join(self._get_options_help_section(self.manager.ljust))
+            + self.help_arg_options(self.manager.ljust)
             + "\n"
-            + self.manager.get_actions_help_section()
-            + "\n".join(self._get_usage_notes_section())
+            + self.manager.cli_help_section()
+            + self.help_usage_notes()
         )
 
     def parse_args(self) -> list[Action]:
         args = sys.argv[1:]
+        last_index = len(args) - 1
         if not args:
             self.log_error(f"no arguments provided. run '{self.executable} --help' for help")
             sys.exit(ExitCodes.INPUT_ERROR)
 
         actions = []
         i = 0
         while i < len(args):
-            arg = self._remove_prefix(args[i])
+            arg = flag_remove_prefix(args[i])
             if arg in RESERVED_FLAGS:
                 match arg:
                     case "help":
                         print(self.help)
                         sys.exit(ExitCodes.SUCCESS)
                     case "t":
                         self.t = int(args[i + 1])
@@ -226,25 +309,38 @@
                         self.verbose = True
                         i += 1
                     case _:
                         self.log_error(f"unknown argument: {args[i]}")
                         sys.exit(ExitCodes.PARSING_ERROR)
                 continue
             if action := self.manager.get(args[i]):
-                inverted = arg.endswith(FILTER_INVERT_SUFFIX)
-                action_cls = action.cls
-                action_args = args[i + 1]
-                if action_args == "--help":
+                next_arg = args[i + 1]
+                if next_arg == "--help":
                     print(action.get_help_long())
                     sys.exit(ExitCodes.SUCCESS)
-                action_obj = action_cls.parse(
-                    action_args, **{"invert": inverted} if inverted else {}
-                )
-                actions.append(action_obj)
-                i += 2
+
+                action_args = []
+                while True:
+                    next_index = i + 1
+                    if next_index > last_index:  # no more args
+                        break
+
+                    next_arg = args[next_index]
+                    if self.manager.get(next_arg):  # next arg is an action
+                        break
+
+                    action_args.append(next_arg)
+                    i += 1
+                inverted = arg.endswith(FILTER_INVERT_SUFFIX)
+                parser = ActionAutoParser(action.cls)  # type: ignore
+                for argumfdafd in action_args:
+                    parser.parse(argumfdafd)
+                obj = parser.get_action(inverted=inverted)
+                actions.append(obj)
+                i += 1
                 continue
             if not arg.startswith(FLAG_PREFIX_LONG) and not arg.startswith(FLAG_PREFIX_SHORT):
                 self.items.append(arg)
                 i += 1
             else:
                 self.log_error(f"unknown argument: {args[i]}")
                 sys.exit(ExitCodes.PARSING_ERROR)
@@ -281,30 +377,30 @@
     def run(self):
         try:
             actions = self.parse_args()
         except Exception as e:
             self.log_error(f"error while parsing arguments: {e}")
             sys.exit(ExitCodes.PARSING_ERROR)
 
-        if self.read_from_stdin:
-            self.items.extend(read_stdin())
+        # if self.read_from_stdin:
+        #    self.items.extend(read_stdin())
 
         if actions is None:
             self.log_error(
                 f"no actions provided. run '{self.executable} --help' to see available actions"
             )
             sys.exit(ExitCodes.INPUT_ERROR)
 
         try:
             items = self.collect_items(self.items)
         except Exception as e:
             self.log_error(f"error while collecting items: {e}")
             sys.exit(ExitCodes.INPUT_ERROR)
 
-        if not items:
+        if not items or len(items) == 0:
             self.log_info("no items to process found")
             sys.exit(ExitCodes.INPUT_ERROR)
 
         try:
             processed_items = self._process_items(items, actions)
         except Exception as e:
             self.log_error(f"error while processing items: {e}")
```

### Comparing `pypeline-python-0.1.1/pypipeline/filter.py` & `pypeline-python-0.1.2/pypipeline/filter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,17 @@
 import re
 from fnmatch import fnmatch
+from typing import Literal
 
-from pypipeline.action import Action
+from pypipeline.action import Action, Filter
 from pypipeline.constants import INT_MAX, INT_MIN, SEP
 from pypipeline.item import Item
 from pypipeline.util import get_pattern_type
 
 
-class Filter(Action):
-    type = "filter"
-
-    def __init__(self, invert=False) -> None:
-        self.invert = invert
-        super().__init__()
-
-    def process(self, item: Item) -> bool:
-        return NotImplemented
-
-    def eval(self, item: Item) -> Item:
-        res = self.process(item)
-        if self.invert:
-            res = not res
-        item.discarded = not res
-        return item
-
-
 class IntFilter(Filter):
     t = int
 
     def __init__(self, low=INT_MIN, high=INT_MAX, invert=False) -> None:
         self.low = low
         self.high = high
         super().__init__(invert)
@@ -91,24 +74,32 @@
     def parse(cls, val: str):
         return cls(val)
 
 
 class TextPatternFilter(Filter):
     """A filter that can be either a glob or regex pattern."""
 
-    def __init__(self, pattern: str, invert=False, pattern_type=None) -> None:
-        if pattern_type is None:
-            pattern_type = get_pattern_type(pattern)
-        if pattern_type is None:
+    dict_exclude = ["t", "invert"]
+
+    def __init__(
+        self,
+        pattern: str,
+        invert=False,
+        t: Literal["regex", "glob", None] = None,
+    ) -> None:
+        if t is None:
+            t = get_pattern_type(pattern)
+        if t is None:
             raise ValueError(f"'{pattern}' is not a valid glob or regex pattern.")
-        if pattern_type == "regex":
+        if t == "regex":
             self.inner = RegexFilter(pattern, invert)
-        elif pattern_type == "glob":
+        elif t == "glob":
             self.inner = GlobFilter(pattern, invert)
-        self.pattern_type = pattern_type
+        self.t = t
+        self.pattern = pattern
         super().__init__(invert)
 
     def process(self, text: str) -> bool:
         return self.inner.process(text)
 
     @classmethod
     def parse(cls, val: str):
```

### Comparing `pypeline-python-0.1.1/pypipeline/items_container.py` & `pypeline-python-0.1.2/pypipeline/items_container.py`

 * *Files identical despite different names*

### Comparing `pypeline-python-0.1.1/pypipeline/pipeline.py` & `pypeline-python-0.1.2/pypipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `pypeline-python-0.1.1/pypipeline/util.py` & `pypeline-python-0.1.2/pypipeline/util.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 import re
 import sys
+from typing import Literal
 
+from stdl import fs
 from stdl.str_u import snake_case
 
 from pypipeline.action import Action
 
 
-def get_pattern_type(pattern: str):
+def get_pattern_type(pattern: str) -> Literal["glob", "regex", None]:
     """Returns whether the pattern is a glob or regex pattern."""
     if "*" in pattern or "?" in pattern:
         return "glob"
     elif re.match(r"^.*(\[.*\]|\\.|\\\|[\w])+.*$", pattern):
         return "regex"
     else:
         return None
 
 
 def get_abbreviation(name: str, taken: list[str]) -> str | None:
     """
     Tries to return a short name for a command.
     Returns None if it cannot find a short name.
+
+    Args:
+        name (str): The name of the command.
+        taken (list[str]): A list of taken abbreviations.
+
     Example:
         >>> get_command_short_name("hello_world", [])
         >>> "h"
         >>> get_command_short_name("hello_world", ["h"])
         >>> "hw"
         >>> get_command_short_name("hello_world", ["hw", "h"])
         >>> "he"
@@ -50,27 +57,33 @@
             return short_name
         return None
     except IndexError:
         return None
 
 
 def get_taken_abbreviations(actions: list[Action]) -> list[str]:
+    """
+    Returns a list of taken abbreviations for a list of actions.
+    """
     taken = []
     for i in actions:
         if i.abbrev is None:
             continue
         if i.abbrev in taken:
             raise ValueError(i.abbrev)
         taken.append(i.abbrev)
     return taken
 
 
-def fill_missing_abbreviations(actions: list[Action], taken: list[str]):
+def fill_missing_abbreviations(actions: list[Action], taken: list[str]) -> None:
+    """
+    Fills in missing abbreviations for a list of actions.
+    """
     for i in actions:
         if i.abbrev is None:
             i.abbrev = get_abbreviation(snake_case(i.__class__.__name__), taken=taken)
 
 
 def get_executable_name(*, full=False) -> str:
     if full:
         return sys.argv[0]
-    return sys.argv[0].split("/")[-1]
+    return sys.argv[0].split(fs.SEP)[-1]
```

### Comparing `pypeline-python-0.1.1/setup.py` & `pypeline-python-0.1.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 HERE = pathlib.Path(__file__).parent
 README = (HERE / "README.md").read_text()
 REQUIREMENTS = (HERE / "requirements.txt").read_text()
 
 setup(
     name="pypeline-python",
-    version="0.1.1",
+    version="0.1.2",
     description="PyPipeline is a simple Python framework for building data processing pipelines.",
     long_description=README,
     long_description_content_type="text/markdown",
     author="Žiga Ivanšek",
     author_email="ziga.ivansek@gmail.com",
     url="https://github.com/zigai/py-pipeline",
     license="MIT",
```

