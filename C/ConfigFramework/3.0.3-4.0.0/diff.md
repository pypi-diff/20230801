# Comparing `tmp/ConfigFramework-3.0.3.tar.gz` & `tmp/ConfigFramework-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ConfigFramework-3.0.3.tar", last modified: Fri Mar 17 12:59:49 2023, max compression
+gzip compressed data, was "ConfigFramework-4.0.0.tar", last modified: Tue Aug  1 19:26:14 2023, max compression
```

## Comparing `ConfigFramework-3.0.3.tar` & `ConfigFramework-4.0.0.tar`

### file list

```diff
@@ -1,36 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 12:59:49.678861 ConfigFramework-3.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 12:59:49.674861 ConfigFramework-3.0.3/ConfigFramework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-03-17 12:59:49.000000 ConfigFramework-3.0.3/ConfigFramework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-03-17 12:59:49.000000 ConfigFramework-3.0.3/ConfigFramework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 12:59:49.000000 ConfigFramework-3.0.3/ConfigFramework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-17 12:59:49.000000 ConfigFramework-3.0.3/ConfigFramework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-17 12:59:49.000000 ConfigFramework-3.0.3/ConfigFramework.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-03-17 12:59:34.000000 ConfigFramework-3.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-03-17 12:59:49.678861 ConfigFramework-3.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5852 2023-03-17 12:59:34.000000 ConfigFramework-3.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 12:59:49.674861 ConfigFramework-3.0.3/config_framework/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-03-17 12:59:34.000000 ConfigFramework-3.0.3/config_framework/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 12:59:49.674861 ConfigFramework-3.0.3/config_framework/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-03-17 12:59:34.000000 ConfigFramework-3.0.3/config_framework/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-03-17 12:59:34.000000 ConfigFramework-3.0.3/config_framework/loaders/composite.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-03-17 12:59:34.000000 ConfigFramework-3.0.3/config_framework/loaders/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-03-17 12:59:34.000000 ConfigFramework-3.0.3/config_framework/loaders/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-03-17 12:59:34.000000 ConfigFramework-3.0.3/config_framework/loaders/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-03-17 12:59:34.000000 ConfigFramework-3.0.3/config_framework/loaders/json_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-03-17 12:59:34.000000 ConfigFramework-3.0.3/config_framework/loaders/yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 12:59:34.000000 ConfigFramework-3.0.3/config_framework/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 12:59:49.678861 ConfigFramework-3.0.3/config_framework/types/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-03-17 12:59:34.000000 ConfigFramework-3.0.3/config_framework/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 12:59:49.678861 ConfigFramework-3.0.3/config_framework/types/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-17 12:59:34.000000 ConfigFramework-3.0.3/config_framework/types/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-03-17 12:59:34.000000 ConfigFramework-3.0.3/config_framework/types/abstract/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-03-17 12:59:34.000000 ConfigFramework-3.0.3/config_framework/types/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-03-17 12:59:34.000000 ConfigFramework-3.0.3/config_framework/types/custom_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9363 2023-03-17 12:59:34.000000 ConfigFramework-3.0.3/config_framework/types/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-03-17 12:59:34.000000 ConfigFramework-3.0.3/config_framework/types/variable_key.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 12:59:49.678861 ConfigFramework-3.0.3/config_framework/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-03-17 12:59:34.000000 ConfigFramework-3.0.3/config_framework/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-03-17 12:59:34.000000 ConfigFramework-3.0.3/config_framework/utils/loader_specific_deserializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-03-17 12:59:34.000000 ConfigFramework-3.0.3/config_framework/utils/loader_specific_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-17 12:59:49.678861 ConfigFramework-3.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-03-17 12:59:34.000000 ConfigFramework-3.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:26:14.518429 ConfigFramework-4.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:26:14.514429 ConfigFramework-4.0.0/ConfigFramework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-08-01 19:26:14.000000 ConfigFramework-4.0.0/ConfigFramework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-08-01 19:26:14.000000 ConfigFramework-4.0.0/ConfigFramework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 19:26:14.000000 ConfigFramework-4.0.0/ConfigFramework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-08-01 19:26:14.000000 ConfigFramework-4.0.0/ConfigFramework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-01 19:26:14.000000 ConfigFramework-4.0.0/ConfigFramework.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-08-01 19:25:57.000000 ConfigFramework-4.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-08-01 19:26:14.518429 ConfigFramework-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-08-01 19:25:57.000000 ConfigFramework-4.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:26:14.514429 ConfigFramework-4.0.0/config_framework/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-08-01 19:25:57.000000 ConfigFramework-4.0.0/config_framework/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:26:14.514429 ConfigFramework-4.0.0/config_framework/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-08-01 19:25:57.000000 ConfigFramework-4.0.0/config_framework/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-08-01 19:25:57.000000 ConfigFramework-4.0.0/config_framework/loaders/composite.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-08-01 19:25:57.000000 ConfigFramework-4.0.0/config_framework/loaders/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-08-01 19:25:57.000000 ConfigFramework-4.0.0/config_framework/loaders/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-08-01 19:25:57.000000 ConfigFramework-4.0.0/config_framework/loaders/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-08-01 19:25:57.000000 ConfigFramework-4.0.0/config_framework/loaders/json_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-08-01 19:25:57.000000 ConfigFramework-4.0.0/config_framework/loaders/toml_full_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-08-01 19:25:57.000000 ConfigFramework-4.0.0/config_framework/loaders/toml_read_only.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-08-01 19:25:57.000000 ConfigFramework-4.0.0/config_framework/loaders/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 19:25:57.000000 ConfigFramework-4.0.0/config_framework/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:26:14.514429 ConfigFramework-4.0.0/config_framework/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-08-01 19:25:57.000000 ConfigFramework-4.0.0/config_framework/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:26:14.518429 ConfigFramework-4.0.0/config_framework/types/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-01 19:25:57.000000 ConfigFramework-4.0.0/config_framework/types/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-08-01 19:25:57.000000 ConfigFramework-4.0.0/config_framework/types/abstract/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-08-01 19:25:57.000000 ConfigFramework-4.0.0/config_framework/types/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-08-01 19:25:57.000000 ConfigFramework-4.0.0/config_framework/types/custom_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9621 2023-08-01 19:25:57.000000 ConfigFramework-4.0.0/config_framework/types/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-08-01 19:25:57.000000 ConfigFramework-4.0.0/config_framework/types/variable_key.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:26:14.518429 ConfigFramework-4.0.0/config_framework/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-08-01 19:25:57.000000 ConfigFramework-4.0.0/config_framework/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-08-01 19:25:57.000000 ConfigFramework-4.0.0/config_framework/utils/loader_specific_deserializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-08-01 19:25:57.000000 ConfigFramework-4.0.0/config_framework/utils/loader_specific_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-08-01 19:25:57.000000 ConfigFramework-4.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 19:26:14.518429 ConfigFramework-4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-08-01 19:25:57.000000 ConfigFramework-4.0.0/setup.py
```

### Comparing `ConfigFramework-3.0.3/ConfigFramework.egg-info/PKG-INFO` & `ConfigFramework-4.0.0/ConfigFramework.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 Metadata-Version: 2.1
 Name: ConfigFramework
-Version: 3.0.3
+Version: 4.0.0
 Summary: A small framework to build your flexible project configurations
 Home-page: https://github.com/Rud356/ConfigFramework
 Author: Rud356
-Author-email: rud356github@gmail.com
-License: GPLv3
+Author-email: Rud356 <rud356github@gmail.com>
+License: MIT License
+Keywords: config,configuration,config managment,configuration managment
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: toml
 Provides-Extra: mypy
 Provides-Extra: dev
 License-File: LICENSE
 
-# ConfigFramework 3.0
+# ConfigFramework 4.0
 ![PyPI version](https://img.shields.io/pypi/v/ConfigFramework)
 ![Python version](https://img.shields.io/pypi/pyversions/ConfigFramework)
 ![PyPi downloads/m](https://img.shields.io/pypi/dm/ConfigFramework)
 ![Issues](https://img.shields.io/github/issues/Rud356/ConfigFramework)
 [![Python package](https://github.com/Rud356/ConfigFramework/actions/workflows/python-tests.yml/badge.svg)](https://github.com/Rud356/ConfigFramework/actions/workflows/python-tests.yml)
 
 A small and simple framework to build your configs. 
@@ -38,14 +41,17 @@
 
 Install with command:
 `pip install ConfigFramework`
 
 To install with mypy you must use command:
 `pip install ConfigFramework[mypy]`
 
+If you have python below 3.11 or need toml format with ability to write it back:
+`pip install ConfigFramework[toml]`
+
 To install with mypy and dev dependencies building requirements you must use command:
 `pip install ConfigFramework[mypy,dev]`
 
 ## Documentation
 [ConfigFrameworks stable branch documentation](https://configframework.readthedocs.io)
 
 ### How to build docs for local usage
@@ -54,64 +60,32 @@
 3. Execute `make html`
 4. Open build/html folder and then open index.html in your browser
 
 ## Example of usage
 
 Here's basic example:
 ```python3
-from typing import Tuple
-from config_framework import BaseConfig, VariableKey, Variable, types
+from config_framework import BaseConfig, VariableKey, Variable
 from config_framework.loaders import Dict
 
 loader = Dict.load(
     data=dict(
         user_id=1,
-        nested_val=dict(pi=3.14),
-        python="3.6.7"
+        nested_val=dict(pi=3.14)
     )
 )
 
 
 class ConfigSample(BaseConfig):
-    user_id: Variable[int] = Variable(loader, VariableKey("user_id"))
-    pi_value = Variable(loader, VariableKey("nested_val") / "pi")
+    user_id: Variable[int] = Variable(VariableKey("user_id"))
+    pi_value = Variable(VariableKey("nested_val") / "pi")
     # Defaults only applied when key isn't found.
-    # Also default values will be validated after initializing
-    # and after you register new validator.
-    some_value = Variable(loader, "not_found_value", default="Hello world")
-    python: Variable[Tuple[int, int, int]] = Variable(
-          loader, "python"
-      )
-
-    @staticmethod
-    @python.register_deserializer
-    def deserialize_version(
-        var: Variable, value: str
-    ) -> Tuple[int, int, int]:
-        version = tuple(map(int, value.split(".")))
-        if len(version) != 3:
-            raise types.custom_exceptions.InvalidValueError(
-                "Version must contain 3 parts"
-            )
+    # Also default values will be validated after initializing, and after you register new validator.
+    some_value = Variable("not_found_value", default="Hello world")
 
-        return version  # noqa: there's a check on being must be exactly 3 parts
-
-    @staticmethod
-    @python.register_serializer
-    def serialize_version(
-        var: Variable, value: Tuple[int, int, int]
-    ) -> str:
-        if len(value) != 3:
-            raise types.custom_exceptions.InvalidValueError(
-                "Version must contain 3 parts"
-            )
-
-        version = ".".join(map(str, value))
-        return version
-    
     @staticmethod
     @user_id.register_validator
     def validate_user_id(var, value):
         # Functions can return bool values or raise
         # config_framework.types.custom_exceptions.InvalidValueError
         # for more detailed description.
         return value == 1
@@ -119,15 +93,15 @@
     def __post_init__(self) -> None:
         print("Post init here!")
         print("Values aren't locked yet")
 
         self.new_value = 122
 
 
-config = ConfigSample()
+config = ConfigSample(loader)
 print("User id:", config.user_id)
 print("Pi value:", config.pi_value)
 print("Some value:", config.some_value)
 print("Post inited value:", config.new_value)
 
 # Configs by default aren't modifiable since frozen=True
 # If you need changing variables for modifying config - you must
@@ -137,46 +111,45 @@
 ```
 
 See examples with explanation [here](https://github.com/Rud356/ConfigFramework/blob/master/examples/)
 
 ## Supported formats
 Config formats:
 - Yaml
+- Toml (read only with default lib included with python 3.11, and read-write with toml external lib)
 - Json (strings or files)
 - Environment variables
 - Pythons dictionaries
 - Composite loading from multiple simple loaders
 
 ## Features
 - Loading configs from multiple sources
 - Creating custom loaders and variables types
-- Nested configs
 - Flexible configs definition
 - Config values validations
 - Casting variables values to specific types using functions
 - Casting to acceptable variable type before dumping variable to loader
 - Variables serialization/deserialization depending on from which loader it was fetched
 - Default values for per loader or per variable
 - Translating one config loaders data to other (with or without including default values for each one)
 - Composite loaders that allow you to define where to look up values using only one loader, that handles
   combining others
-- Simpler access to variables values (new in 3.0)
+- Simple access to variables values
+- Single entry point for initialization of config with loader
 
-## About 3.0
-This version of config framework breaks many things and has other structure, 
-so you will have to manually migrate to this one. I think it was necessary
-to improve many things, and I hope it will make your life easier.
+## About 4.0
+This version of ConfigFramework is not backwards compatible and requires a bit of work to make migration.
+It was needed to get rid of annoying initialization with one config loader per variable listing, which
+also made it really hard to replace config sources and made it more uncertain where is the source of data for variable.
 
 ### What is different?
-- Now module will be called config_framework when you import it into project
-- Structure of whole project is different comparing to 2.0
-- Usage of VariableKey to create key that will tell how to access nested values
-without worrying about what symbols to use, but requiring to explicitly write
-VariableKey whenever you want to go from this root key
-- Improved usability by using descriptors and making more logical arguments order
-- By default, config will not allow you
-assigning any values after `__post_init__` was called
+- Configs must get only one loader as input when initializing them, and all variables don't have argument for specifying
+loader.
+- Added toml support for python above 3.11 and with external library that adds ability to read and write data.
+- Changes in internals regarding variables initialization to support assigning data from provided loader dynamically on
+initialization of whole config.
+- Added pyproject.toml for more modern package management.
 
 ### Known issues
 - Typehint for `Variable[any_type]` doesn't work properly and give
 only hints for Variable methods, while must give hints for any_type, when
 called from instance of any subclass of BaseConfig
```

### Comparing `ConfigFramework-3.0.3/ConfigFramework.egg-info/SOURCES.txt` & `ConfigFramework-4.0.0/ConfigFramework.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 LICENSE
 README.md
+pyproject.toml
 setup.py
 ConfigFramework.egg-info/PKG-INFO
 ConfigFramework.egg-info/SOURCES.txt
 ConfigFramework.egg-info/dependency_links.txt
 ConfigFramework.egg-info/requires.txt
 ConfigFramework.egg-info/top_level.txt
 config_framework/__init__.py
 config_framework/py.typed
 config_framework/loaders/__init__.py
 config_framework/loaders/composite.py
 config_framework/loaders/dict.py
 config_framework/loaders/env.py
 config_framework/loaders/json.py
 config_framework/loaders/json_string.py
+config_framework/loaders/toml_full_features.py
+config_framework/loaders/toml_read_only.py
 config_framework/loaders/yaml.py
 config_framework/types/__init__.py
 config_framework/types/config.py
 config_framework/types/custom_exceptions.py
 config_framework/types/variable.py
 config_framework/types/variable_key.py
 config_framework/types/abstract/__init__.py
```

### Comparing `ConfigFramework-3.0.3/LICENSE` & `ConfigFramework-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ConfigFramework-3.0.3/PKG-INFO` & `ConfigFramework-4.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 Metadata-Version: 2.1
 Name: ConfigFramework
-Version: 3.0.3
+Version: 4.0.0
 Summary: A small framework to build your flexible project configurations
 Home-page: https://github.com/Rud356/ConfigFramework
 Author: Rud356
-Author-email: rud356github@gmail.com
-License: GPLv3
+Author-email: Rud356 <rud356github@gmail.com>
+License: MIT License
+Keywords: config,configuration,config managment,configuration managment
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: toml
 Provides-Extra: mypy
 Provides-Extra: dev
 License-File: LICENSE
 
-# ConfigFramework 3.0
+# ConfigFramework 4.0
 ![PyPI version](https://img.shields.io/pypi/v/ConfigFramework)
 ![Python version](https://img.shields.io/pypi/pyversions/ConfigFramework)
 ![PyPi downloads/m](https://img.shields.io/pypi/dm/ConfigFramework)
 ![Issues](https://img.shields.io/github/issues/Rud356/ConfigFramework)
 [![Python package](https://github.com/Rud356/ConfigFramework/actions/workflows/python-tests.yml/badge.svg)](https://github.com/Rud356/ConfigFramework/actions/workflows/python-tests.yml)
 
 A small and simple framework to build your configs. 
@@ -38,14 +41,17 @@
 
 Install with command:
 `pip install ConfigFramework`
 
 To install with mypy you must use command:
 `pip install ConfigFramework[mypy]`
 
+If you have python below 3.11 or need toml format with ability to write it back:
+`pip install ConfigFramework[toml]`
+
 To install with mypy and dev dependencies building requirements you must use command:
 `pip install ConfigFramework[mypy,dev]`
 
 ## Documentation
 [ConfigFrameworks stable branch documentation](https://configframework.readthedocs.io)
 
 ### How to build docs for local usage
@@ -54,64 +60,32 @@
 3. Execute `make html`
 4. Open build/html folder and then open index.html in your browser
 
 ## Example of usage
 
 Here's basic example:
 ```python3
-from typing import Tuple
-from config_framework import BaseConfig, VariableKey, Variable, types
+from config_framework import BaseConfig, VariableKey, Variable
 from config_framework.loaders import Dict
 
 loader = Dict.load(
     data=dict(
         user_id=1,
-        nested_val=dict(pi=3.14),
-        python="3.6.7"
+        nested_val=dict(pi=3.14)
     )
 )
 
 
 class ConfigSample(BaseConfig):
-    user_id: Variable[int] = Variable(loader, VariableKey("user_id"))
-    pi_value = Variable(loader, VariableKey("nested_val") / "pi")
+    user_id: Variable[int] = Variable(VariableKey("user_id"))
+    pi_value = Variable(VariableKey("nested_val") / "pi")
     # Defaults only applied when key isn't found.
-    # Also default values will be validated after initializing
-    # and after you register new validator.
-    some_value = Variable(loader, "not_found_value", default="Hello world")
-    python: Variable[Tuple[int, int, int]] = Variable(
-          loader, "python"
-      )
-
-    @staticmethod
-    @python.register_deserializer
-    def deserialize_version(
-        var: Variable, value: str
-    ) -> Tuple[int, int, int]:
-        version = tuple(map(int, value.split(".")))
-        if len(version) != 3:
-            raise types.custom_exceptions.InvalidValueError(
-                "Version must contain 3 parts"
-            )
+    # Also default values will be validated after initializing, and after you register new validator.
+    some_value = Variable("not_found_value", default="Hello world")
 
-        return version  # noqa: there's a check on being must be exactly 3 parts
-
-    @staticmethod
-    @python.register_serializer
-    def serialize_version(
-        var: Variable, value: Tuple[int, int, int]
-    ) -> str:
-        if len(value) != 3:
-            raise types.custom_exceptions.InvalidValueError(
-                "Version must contain 3 parts"
-            )
-
-        version = ".".join(map(str, value))
-        return version
-    
     @staticmethod
     @user_id.register_validator
     def validate_user_id(var, value):
         # Functions can return bool values or raise
         # config_framework.types.custom_exceptions.InvalidValueError
         # for more detailed description.
         return value == 1
@@ -119,15 +93,15 @@
     def __post_init__(self) -> None:
         print("Post init here!")
         print("Values aren't locked yet")
 
         self.new_value = 122
 
 
-config = ConfigSample()
+config = ConfigSample(loader)
 print("User id:", config.user_id)
 print("Pi value:", config.pi_value)
 print("Some value:", config.some_value)
 print("Post inited value:", config.new_value)
 
 # Configs by default aren't modifiable since frozen=True
 # If you need changing variables for modifying config - you must
@@ -137,46 +111,45 @@
 ```
 
 See examples with explanation [here](https://github.com/Rud356/ConfigFramework/blob/master/examples/)
 
 ## Supported formats
 Config formats:
 - Yaml
+- Toml (read only with default lib included with python 3.11, and read-write with toml external lib)
 - Json (strings or files)
 - Environment variables
 - Pythons dictionaries
 - Composite loading from multiple simple loaders
 
 ## Features
 - Loading configs from multiple sources
 - Creating custom loaders and variables types
-- Nested configs
 - Flexible configs definition
 - Config values validations
 - Casting variables values to specific types using functions
 - Casting to acceptable variable type before dumping variable to loader
 - Variables serialization/deserialization depending on from which loader it was fetched
 - Default values for per loader or per variable
 - Translating one config loaders data to other (with or without including default values for each one)
 - Composite loaders that allow you to define where to look up values using only one loader, that handles
   combining others
-- Simpler access to variables values (new in 3.0)
+- Simple access to variables values
+- Single entry point for initialization of config with loader
 
-## About 3.0
-This version of config framework breaks many things and has other structure, 
-so you will have to manually migrate to this one. I think it was necessary
-to improve many things, and I hope it will make your life easier.
+## About 4.0
+This version of ConfigFramework is not backwards compatible and requires a bit of work to make migration.
+It was needed to get rid of annoying initialization with one config loader per variable listing, which
+also made it really hard to replace config sources and made it more uncertain where is the source of data for variable.
 
 ### What is different?
-- Now module will be called config_framework when you import it into project
-- Structure of whole project is different comparing to 2.0
-- Usage of VariableKey to create key that will tell how to access nested values
-without worrying about what symbols to use, but requiring to explicitly write
-VariableKey whenever you want to go from this root key
-- Improved usability by using descriptors and making more logical arguments order
-- By default, config will not allow you
-assigning any values after `__post_init__` was called
+- Configs must get only one loader as input when initializing them, and all variables don't have argument for specifying
+loader.
+- Added toml support for python above 3.11 and with external library that adds ability to read and write data.
+- Changes in internals regarding variables initialization to support assigning data from provided loader dynamically on
+initialization of whole config.
+- Added pyproject.toml for more modern package management.
 
 ### Known issues
 - Typehint for `Variable[any_type]` doesn't work properly and give
 only hints for Variable methods, while must give hints for any_type, when
 called from instance of any subclass of BaseConfig
```

### Comparing `ConfigFramework-3.0.3/README.md` & `ConfigFramework-4.0.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# ConfigFramework 3.0
+# ConfigFramework 4.0
 ![PyPI version](https://img.shields.io/pypi/v/ConfigFramework)
 ![Python version](https://img.shields.io/pypi/pyversions/ConfigFramework)
 ![PyPi downloads/m](https://img.shields.io/pypi/dm/ConfigFramework)
 ![Issues](https://img.shields.io/github/issues/Rud356/ConfigFramework)
 [![Python package](https://github.com/Rud356/ConfigFramework/actions/workflows/python-tests.yml/badge.svg)](https://github.com/Rud356/ConfigFramework/actions/workflows/python-tests.yml)
 
 A small and simple framework to build your configs. 
@@ -15,14 +15,17 @@
 
 Install with command:
 `pip install ConfigFramework`
 
 To install with mypy you must use command:
 `pip install ConfigFramework[mypy]`
 
+If you have python below 3.11 or need toml format with ability to write it back:
+`pip install ConfigFramework[toml]`
+
 To install with mypy and dev dependencies building requirements you must use command:
 `pip install ConfigFramework[mypy,dev]`
 
 ## Documentation
 [ConfigFrameworks stable branch documentation](https://configframework.readthedocs.io)
 
 ### How to build docs for local usage
@@ -31,64 +34,32 @@
 3. Execute `make html`
 4. Open build/html folder and then open index.html in your browser
 
 ## Example of usage
 
 Here's basic example:
 ```python3
-from typing import Tuple
-from config_framework import BaseConfig, VariableKey, Variable, types
+from config_framework import BaseConfig, VariableKey, Variable
 from config_framework.loaders import Dict
 
 loader = Dict.load(
     data=dict(
         user_id=1,
-        nested_val=dict(pi=3.14),
-        python="3.6.7"
+        nested_val=dict(pi=3.14)
     )
 )
 
 
 class ConfigSample(BaseConfig):
-    user_id: Variable[int] = Variable(loader, VariableKey("user_id"))
-    pi_value = Variable(loader, VariableKey("nested_val") / "pi")
+    user_id: Variable[int] = Variable(VariableKey("user_id"))
+    pi_value = Variable(VariableKey("nested_val") / "pi")
     # Defaults only applied when key isn't found.
-    # Also default values will be validated after initializing
-    # and after you register new validator.
-    some_value = Variable(loader, "not_found_value", default="Hello world")
-    python: Variable[Tuple[int, int, int]] = Variable(
-          loader, "python"
-      )
-
-    @staticmethod
-    @python.register_deserializer
-    def deserialize_version(
-        var: Variable, value: str
-    ) -> Tuple[int, int, int]:
-        version = tuple(map(int, value.split(".")))
-        if len(version) != 3:
-            raise types.custom_exceptions.InvalidValueError(
-                "Version must contain 3 parts"
-            )
+    # Also default values will be validated after initializing, and after you register new validator.
+    some_value = Variable("not_found_value", default="Hello world")
 
-        return version  # noqa: there's a check on being must be exactly 3 parts
-
-    @staticmethod
-    @python.register_serializer
-    def serialize_version(
-        var: Variable, value: Tuple[int, int, int]
-    ) -> str:
-        if len(value) != 3:
-            raise types.custom_exceptions.InvalidValueError(
-                "Version must contain 3 parts"
-            )
-
-        version = ".".join(map(str, value))
-        return version
-    
     @staticmethod
     @user_id.register_validator
     def validate_user_id(var, value):
         # Functions can return bool values or raise
         # config_framework.types.custom_exceptions.InvalidValueError
         # for more detailed description.
         return value == 1
@@ -96,15 +67,15 @@
     def __post_init__(self) -> None:
         print("Post init here!")
         print("Values aren't locked yet")
 
         self.new_value = 122
 
 
-config = ConfigSample()
+config = ConfigSample(loader)
 print("User id:", config.user_id)
 print("Pi value:", config.pi_value)
 print("Some value:", config.some_value)
 print("Post inited value:", config.new_value)
 
 # Configs by default aren't modifiable since frozen=True
 # If you need changing variables for modifying config - you must
@@ -114,46 +85,45 @@
 ```
 
 See examples with explanation [here](https://github.com/Rud356/ConfigFramework/blob/master/examples/)
 
 ## Supported formats
 Config formats:
 - Yaml
+- Toml (read only with default lib included with python 3.11, and read-write with toml external lib)
 - Json (strings or files)
 - Environment variables
 - Pythons dictionaries
 - Composite loading from multiple simple loaders
 
 ## Features
 - Loading configs from multiple sources
 - Creating custom loaders and variables types
-- Nested configs
 - Flexible configs definition
 - Config values validations
 - Casting variables values to specific types using functions
 - Casting to acceptable variable type before dumping variable to loader
 - Variables serialization/deserialization depending on from which loader it was fetched
 - Default values for per loader or per variable
 - Translating one config loaders data to other (with or without including default values for each one)
 - Composite loaders that allow you to define where to look up values using only one loader, that handles
   combining others
-- Simpler access to variables values (new in 3.0)
+- Simple access to variables values
+- Single entry point for initialization of config with loader
 
-## About 3.0
-This version of config framework breaks many things and has other structure, 
-so you will have to manually migrate to this one. I think it was necessary
-to improve many things, and I hope it will make your life easier.
+## About 4.0
+This version of ConfigFramework is not backwards compatible and requires a bit of work to make migration.
+It was needed to get rid of annoying initialization with one config loader per variable listing, which
+also made it really hard to replace config sources and made it more uncertain where is the source of data for variable.
 
 ### What is different?
-- Now module will be called config_framework when you import it into project
-- Structure of whole project is different comparing to 2.0
-- Usage of VariableKey to create key that will tell how to access nested values
-without worrying about what symbols to use, but requiring to explicitly write
-VariableKey whenever you want to go from this root key
-- Improved usability by using descriptors and making more logical arguments order
-- By default, config will not allow you
-assigning any values after `__post_init__` was called
+- Configs must get only one loader as input when initializing them, and all variables don't have argument for specifying
+loader.
+- Added toml support for python above 3.11 and with external library that adds ability to read and write data.
+- Changes in internals regarding variables initialization to support assigning data from provided loader dynamically on
+initialization of whole config.
+- Added pyproject.toml for more modern package management.
 
 ### Known issues
 - Typehint for `Variable[any_type]` doesn't work properly and give
 only hints for Variable methods, while must give hints for any_type, when
 called from instance of any subclass of BaseConfig
```

### Comparing `ConfigFramework-3.0.3/config_framework/loaders/composite.py` & `ConfigFramework-4.0.0/config_framework/loaders/composite.py`

 * *Files identical despite different names*

### Comparing `ConfigFramework-3.0.3/config_framework/loaders/dict.py` & `ConfigFramework-4.0.0/config_framework/loaders/dict.py`

 * *Files identical despite different names*

### Comparing `ConfigFramework-3.0.3/config_framework/loaders/env.py` & `ConfigFramework-4.0.0/config_framework/loaders/env.py`

 * *Files identical despite different names*

### Comparing `ConfigFramework-3.0.3/config_framework/loaders/json.py` & `ConfigFramework-4.0.0/config_framework/loaders/json.py`

 * *Files identical despite different names*

### Comparing `ConfigFramework-3.0.3/config_framework/loaders/json_string.py` & `ConfigFramework-4.0.0/config_framework/loaders/json_string.py`

 * *Files identical despite different names*

### Comparing `ConfigFramework-3.0.3/config_framework/loaders/yaml.py` & `ConfigFramework-4.0.0/config_framework/loaders/yaml.py`

 * *Files identical despite different names*

### Comparing `ConfigFramework-3.0.3/config_framework/types/abstract/loader.py` & `ConfigFramework-4.0.0/config_framework/types/abstract/loader.py`

 * *Files identical despite different names*

### Comparing `ConfigFramework-3.0.3/config_framework/types/config.py` & `ConfigFramework-4.0.0/config_framework/types/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 from __future__ import annotations
 
-from typing import Set
+from typing import Set, ClassVar
 
 from .abstract.loader import AbstractLoader
 from .variable import Variable
 
 
 class BaseConfig:
     frozen: bool
-    _variables: Set[Variable]
-    _loaders: Set[AbstractLoader]
+    _loader: AbstractLoader
+    _variables: ClassVar[Set[Variable]]
 
-    def __init__(self, frozen: bool = True):
+    def __init__(self, loader: AbstractLoader, frozen: bool = True):
         """
         Initializes config class.
 
+        :param loader: loader that will be used to set values to variables of config object.
         :param frozen: prevents user from assigning any values directly
             to class instance. Object will be not modifiable after
             __post_init__ is called.
         :return: nothing.
         """
         self.frozen = False
+
+        for variable in self._variables:
+            variable._set_value_from_loader(loader)
+
+        self._loader = loader
         self.__post_init__()
         self.frozen: bool = frozen
 
     def __post_init__(self) -> None:
         """
         Function with custom user actions for any purpose.
 
@@ -35,21 +41,19 @@
     def __init_subclass__(cls, **kwargs) -> None:
         """
         Function that collects all variables and loaders from inherited config.
 
         :kwargs: subclasses kwargs.
         :return: nothing.
         """
-        cls._loaders = set()
         cls._variables = set()
 
         for key, value in cls.__dict__.items():
             if isinstance(value, Variable):
                 cls._variables.add(value)
-                cls._loaders.add(value.source)
 
     def __setattr__(self, key, value):
         """
         Assigns value to class under specific key.
 
         :param key: attribute key.
         :param value: attribute value.
@@ -72,12 +76,11 @@
         """
         Saves updated variables values to some storage using
             AbstractLoader.dump method.
 
         :param include_defaults: if dump of config must include default values.
         :return: nothing.
         """
-        for loader in self._loaders:
-            loader.dump(include_defaults)
+        self._loader.dump(include_defaults)
 
     def __repr__(self):
         return self.__class__.__name__
```

### Comparing `ConfigFramework-3.0.3/config_framework/types/variable.py` & `ConfigFramework-4.0.0/config_framework/types/variable.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,41 +15,31 @@
 Var = TypeVar("Var")
 CustomSerializer = Callable[["Variable", Var], Any]
 CustomDeserializer = Callable[["Variable", Any], Var]
 CustomValidator = Callable[["Variable", Var], bool]
 
 
 class Variable(Generic[Var]):
+    source: Optional[AbstractLoader]
     _value: Var
 
     def __init__(
-        self, source: AbstractLoader,
+        self,
         key: Union[VariableKey, str],
         default: Optional[Var] = None
     ):
-        self.default: Optional[Var] = default
-
-        if self.default is not None:
-            self.validate_value(self.default)
-
-        self.source: AbstractLoader = source
+        self.default = default
+        if default is not None:
+            self.validate_value(default)
+            self.default = default
 
         if isinstance(key, str):
             key = VariableKey(key)
 
         self.key: VariableKey = key
-        self.default = default
-
-        if not default:
-            self._value = self.deserialize(self.source[key])
-
-        else:
-            self._value = self.deserialize(self.source.get(key, default))
-
-        self._value = self.deserialize(self._value)
 
     @overload
     def __get__(
         self, instance: None, cls: Any
     ) -> Variable[Var]:
         ...
 
@@ -67,41 +57,66 @@
         Gives you a value or Variable with your value depending on condition.
 
         :param instance: if it is None then you will receive Variable instance.
             If it's not - you will get just a value inside of Variable.
         :param cls: class from which variable was called.
         returns: Variable._value or Variable instance, depending on conditions,
             explained previously.
+        :raises ValueError: if there are no defaults or
         """
         if instance:
-            return self._value
+            try:
+                return self._value
+
+            except AttributeError:
+                if self.default is not None:
+                    return self.default
+
+                raise ValueError(f"No variable value set for variable with key {self.key}")
 
         else:
             return self
 
     def __set__(self, obj: Optional[object], value: Var) -> None:
         """
         Sets a new value to your variable.
 
+        :param obj: object from which method was called.
+        :param value: which value will be assigned to _value field.
         :raises config_framework.types.custom_exceptions.ValueValidationError:
             adds explanation on where is invalid value in your config and
             from which loader value is from. This contains also a traceback
             to your config_framework.types.custom_exceptions.InvalidValueError.
         """
         self.validate_value(value)
         self._value = value
 
-        self.source[self.key] = self.serialize()
+    def _set_value_from_loader(self, loader: AbstractLoader) -> None:
+        """
+        Helps to set value to Variable object with validation to allow initialization of it
+        during creating Config object, so users can choose desired loaders on startup.
+
+        :param loader:
+        :return:
+        """
+        self.source = loader
+        if not self.default:
+            value = self.deserialize(loader[self.key])
+
+        else:
+            value = self.deserialize(loader.get(self.key, self.default))
+
+        self.__set__(self, value)
 
     def serialize(
         self: Variable
     ) -> Any:  # noqa:
         # Might be used by other functions.
         """
-        Casts variables value to specific loaders type so it can be saved.
+        Casts variables value to specific loaders type, so it can be saved.
 
         :returns: anything.
         """
         return self.custom_serializer(self, self._value)
 
     def deserialize(
         self,
@@ -123,17 +138,17 @@
         self.validate_value(casted_value)
         return casted_value
 
     def validate_value(self, value: Var) -> bool:
         """
         Checks if certain value is correct via users code.
 
-        :param value: value of correct python type (after being casted from
+        :param value: value of correct python type (after being cast from
             raw loader value) that will be validated.
-        :returns: bool value representing if its correct or not.
+        :returns: bool value representing if It's correct or not.
 
         :raises config_framework.types.custom_exceptions.ValueValidationError:
             adds explanation on where is invalid value in your config and
             from which loader value is from. This contains also a traceback
             to your config_framework.types.custom_exceptions.InvalidValueError.
         """
         try:
@@ -141,15 +156,15 @@
             if not is_valid:
                 raise custom_exceptions.ValueValidationError()
 
             return is_valid
 
         except custom_exceptions.ValueValidationError as user_error:
             raise custom_exceptions.InvalidValueError(
-                f"{self.key} got invalid value from source {self.source}"
+                f"{self.key} got invalid value"
             ) from user_error
 
     def _validate_default_value(self) -> None:
         try:
             if self.default is None:
                 return None
 
@@ -219,51 +234,39 @@
         and instantly validates current value.
 
         :param f: some method that signature matches to CustomValidator.
         :return: function itself.
         """
         setattr(self, "custom_validator", f)
         # Validating already existing value with new validator
-        self.validate_value(self._value)
+        if self.default is not None:
+            self.validate_value(self.default)
+
+        if hasattr(self, "_value"):
+            self.validate_value(self._value)
         return f
 
     def register_serializer(
         self, f: CustomSerializer
     ) -> CustomSerializer:
         """
         Registers passed function as custom_serializer to be used later
         and instantly uses it to trigger possible errors.
 
         :param f: some method that signature matches to CustomSerializer.
         :return: function itself.
         """
         setattr(self, "custom_serializer", f)
-        # Testing if serializer works fine
-        self.serialize()
         return f
 
     def register_deserializer(
         self, f: CustomDeserializer
     ) -> CustomDeserializer:
         """
         Registers passed function as custom_deserializer to be used later
         and instantly uses it to trigger possible errors on value from.
 
         :param f: some method that signature matches to CustomDeserializer.
         :return: function itself.
         """
         setattr(self, "custom_deserializer", f)
-        # Testing if deserializer works fine after being set
-        # and applying it to value from source.
-
-        if not self.default:
-            self._value = self.deserialize(
-                self.source[self.key]
-            )
-
-        else:
-            self._value = self.deserialize(
-                self.source.get(self.key, self.default)
-            )
-
-        self.validate_value(self._value)
         return f
```

### Comparing `ConfigFramework-3.0.3/config_framework/types/variable_key.py` & `ConfigFramework-4.0.0/config_framework/types/variable_key.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import Iterable, Union, Optional, Iterator, List
+from typing import Iterable, Union, Iterator, List
 
 
 class VariableKey(Iterable):
     """
     Class that helps us organize how keys for config variables
     to look for inside of some complicated nested structures.
     """
```

### Comparing `ConfigFramework-3.0.3/config_framework/utils/loader_specific_deserializer.py` & `ConfigFramework-4.0.0/config_framework/utils/loader_specific_deserializer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import Dict, Union, Any, Type
+from typing import Dict, Union, Any, Type, Optional
 
 from config_framework.loaders.composite import Composite
 from config_framework.types import Variable
 from config_framework.types.abstract import AbstractLoader
 from config_framework.types.variable import Var, CustomDeserializer
 
 
@@ -38,15 +38,17 @@
         :param from_value: raw value from loader.
         :returns: validated and caster to python type value.
         :raises config_framework.types.custom_exceptions.ValueValidationError:
             adds explanation on where is invalid value in your config and
             from which loader value is from. This contains also a traceback
             to your config_framework.types.custom_exceptions.InvalidValueError.
         """
-        cast_from_loader = variable.source
+        assert hasattr(variable, "source"), f"No source loader specified for variable {variable.key}"
+        cast_from_loader: Optional[AbstractLoader] = variable.source
+        assert cast_from_loader is not None, f"Variable {variable.key} has loader set to None"
 
         if isinstance(cast_from_loader, Composite):
             cast_from_loader = self.fetch_original_source(
                 variable, cast_from_loader
             )
 
         try:
@@ -64,16 +66,15 @@
             raise KeyError(
                 f"Deserializer for {cast_from_loader} isn't specified"
                 " and not found any default one."
             )
 
         deserialized_variable: Var = deserializer(
             variable,
-            variable._value  # noqa: we need to get this value from variable
-            # to deserialize
+            from_value
         )
         variable.validate_value(deserialized_variable)
         return deserialized_variable
 
     @staticmethod
     def fetch_original_source(
         variable: Variable, composite_loader: Composite
```

### Comparing `ConfigFramework-3.0.3/config_framework/utils/loader_specific_serializer.py` & `ConfigFramework-4.0.0/config_framework/utils/loader_specific_serializer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import Dict, Union, Any, Type
+from typing import Dict, Union, Any, Type, Optional
 
 from config_framework.loaders.composite import Composite
 from config_framework.types import Variable
 from config_framework.types.abstract import AbstractLoader
 from config_framework.types.variable import Var, CustomSerializer
 
 
@@ -35,15 +35,18 @@
         """
         Casts value to specific loaders type so it can be saved.
 
         :param value: python value that needs
             to be transformed to loaders type.
         :returns: anything.
         """
-        cast_for_loader = variable.source
+        assert hasattr(variable, "source"), f"No source loader specified for variable {variable.key}"
+        cast_for_loader: Optional[AbstractLoader] = variable.source
+        assert cast_for_loader is not None, f"Variable {variable.key} has loader set to None"
+
         if isinstance(cast_for_loader, Composite):
             cast_for_loader = self.fetch_original_source(
                 variable,  # noqa: we need this value from internals
                 cast_for_loader
             )
 
         try:
```

### Comparing `ConfigFramework-3.0.3/setup.py` & `ConfigFramework-4.0.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,29 +14,31 @@
     name="ConfigFramework",
     version=config_framework.__version__,
     author="Rud356",
     author_email="rud356github@gmail.com",
     description="A small framework to build your flexible project configurations",
     long_description=text,
     long_description_content_type="text/markdown",
-    license="GPLv3",
+    license="MIT",
     url="https://github.com/Rud356/ConfigFramework",
     packages=setuptools.find_packages(exclude=["tests", "examples"]),
     package_data={"config_framework": ["py.typed"]},
     install_requires=requirements,
     extras_require={
-        'mypy': ["mypy", "types-PyYAML"],
+        "toml": ["toml"],
+        'mypy': ["mypy", "types-PyYAML", "types-toml"],
         'dev': dev_requirements
     },
     classifiers=[
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Intended Audience :: Developers",
         "Natural Language :: English",
     ],
     python_requires=">=3.7"
 )
```

