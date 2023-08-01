# Comparing `tmp/zq-config-0.1.3.tar.gz` & `tmp/zq-config-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zq-config-0.1.3.tar", last modified: Fri Jun  2 03:42:18 2023, max compression
+gzip compressed data, was "zq-config-0.1.4.tar", last modified: Tue Aug  1 08:17:25 2023, max compression
```

## Comparing `zq-config-0.1.3.tar` & `zq-config-0.1.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 test      (1000) test      (1001)        0 2023-06-02 03:42:18.210183 zq-config-0.1.3/
--rw-r--r--   0 test      (1000) test      (1001)     1081 2023-04-21 06:48:00.000000 zq-config-0.1.3/LICENSE.txt
--rw-r--r--   0 test      (1000) test      (1001)     2992 2023-06-02 03:42:18.210183 zq-config-0.1.3/PKG-INFO
--rw-r--r--   0 test      (1000) test      (1001)      511 2023-04-21 07:12:13.000000 zq-config-0.1.3/README.md
--rw-r--r--   0 test      (1000) test      (1001)     4132 2023-06-02 03:20:46.000000 zq-config-0.1.3/pyproject.toml
--rw-r--r--   0 test      (1000) test      (1001)       38 2023-06-02 03:42:18.210183 zq-config-0.1.3/setup.cfg
-drwxr-xr-x   0 test      (1000) test      (1001)        0 2023-06-02 03:42:18.200183 zq-config-0.1.3/tests/
--rw-r--r--   0 test      (1000) test      (1001)      667 2023-04-21 08:09:21.000000 zq-config-0.1.3/tests/test_simple.py
-drwxr-xr-x   0 test      (1000) test      (1001)        0 2023-06-02 03:42:18.200183 zq-config-0.1.3/zq_config/
--rw-r--r--   0 test      (1000) test      (1001)        0 2023-04-21 09:34:13.000000 zq-config-0.1.3/zq_config/__init__.py
-drwxr-xr-x   0 test      (1000) test      (1001)        0 2023-06-02 03:42:18.206850 zq-config-0.1.3/zq_config/backends/
--rw-r--r--   0 test      (1000) test      (1001)      225 2023-06-02 03:20:30.000000 zq-config-0.1.3/zq_config/backends/__init__.py
--rw-r--r--   0 test      (1000) test      (1001)      200 2023-04-21 09:34:28.000000 zq-config-0.1.3/zq_config/backends/backend_registry.py
--rw-r--r--   0 test      (1000) test      (1001)      384 2023-06-02 01:42:23.000000 zq-config-0.1.3/zq_config/backends/nacos.py
--rw-r--r--   0 test      (1000) test      (1001)     1773 2023-06-02 03:02:32.000000 zq-config-0.1.3/zq_config/zq_configs.py
-drwxr-xr-x   0 test      (1000) test      (1001)        0 2023-06-02 03:42:18.206850 zq-config-0.1.3/zq_config.egg-info/
--rw-r--r--   0 test      (1000) test      (1001)     2992 2023-06-02 03:42:18.000000 zq-config-0.1.3/zq_config.egg-info/PKG-INFO
--rw-r--r--   0 test      (1000) test      (1001)      401 2023-06-02 03:42:18.000000 zq-config-0.1.3/zq_config.egg-info/SOURCES.txt
--rw-r--r--   0 test      (1000) test      (1001)        1 2023-06-02 03:42:18.000000 zq-config-0.1.3/zq_config.egg-info/dependency_links.txt
--rw-r--r--   0 test      (1000) test      (1001)       39 2023-06-02 03:42:18.000000 zq-config-0.1.3/zq_config.egg-info/entry_points.txt
--rw-r--r--   0 test      (1000) test      (1001)       49 2023-06-02 03:42:18.000000 zq-config-0.1.3/zq_config.egg-info/requires.txt
--rw-r--r--   0 test      (1000) test      (1001)       10 2023-06-02 03:42:18.000000 zq-config-0.1.3/zq_config.egg-info/top_level.txt
+drwxr-xr-x   0 test      (1000) test      (1001)        0 2023-08-01 08:17:25.654032 zq-config-0.1.4/
+-rw-r--r--   0 test      (1000) test      (1001)     1081 2023-04-21 06:48:00.000000 zq-config-0.1.4/LICENSE.txt
+-rw-r--r--   0 test      (1000) test      (1001)     2992 2023-08-01 08:17:25.647365 zq-config-0.1.4/PKG-INFO
+-rw-r--r--   0 test      (1000) test      (1001)      511 2023-04-21 07:12:13.000000 zq-config-0.1.4/README.md
+-rw-r--r--   0 test      (1000) test      (1001)     4133 2023-08-01 08:15:51.000000 zq-config-0.1.4/pyproject.toml
+-rw-r--r--   0 test      (1000) test      (1001)       38 2023-08-01 08:17:25.654032 zq-config-0.1.4/setup.cfg
+drwxr-xr-x   0 test      (1000) test      (1001)        0 2023-08-01 08:17:25.607364 zq-config-0.1.4/tests/
+-rw-r--r--   0 test      (1000) test      (1001)      667 2023-04-21 08:09:21.000000 zq-config-0.1.4/tests/test_simple.py
+drwxr-xr-x   0 test      (1000) test      (1001)        0 2023-08-01 08:17:25.614031 zq-config-0.1.4/zq_config/
+-rw-r--r--   0 test      (1000) test      (1001)        0 2023-04-21 09:34:13.000000 zq-config-0.1.4/zq_config/__init__.py
+drwxr-xr-x   0 test      (1000) test      (1001)        0 2023-08-01 08:17:25.647365 zq-config-0.1.4/zq_config/backends/
+-rw-r--r--   0 test      (1000) test      (1001)      225 2023-06-02 03:20:30.000000 zq-config-0.1.4/zq_config/backends/__init__.py
+-rw-r--r--   0 test      (1000) test      (1001)      200 2023-04-21 09:34:28.000000 zq-config-0.1.4/zq_config/backends/backend_registry.py
+-rw-r--r--   0 test      (1000) test      (1001)      484 2023-08-01 08:10:35.000000 zq-config-0.1.4/zq_config/backends/nacos.py
+-rw-r--r--   0 test      (1000) test      (1001)     1664 2023-08-01 08:07:36.000000 zq-config-0.1.4/zq_config/zq_configs.py
+drwxr-xr-x   0 test      (1000) test      (1001)        0 2023-08-01 08:17:25.634032 zq-config-0.1.4/zq_config.egg-info/
+-rw-r--r--   0 test      (1000) test      (1001)     2992 2023-08-01 08:17:25.000000 zq-config-0.1.4/zq_config.egg-info/PKG-INFO
+-rw-r--r--   0 test      (1000) test      (1001)      401 2023-08-01 08:17:25.000000 zq-config-0.1.4/zq_config.egg-info/SOURCES.txt
+-rw-r--r--   0 test      (1000) test      (1001)        1 2023-08-01 08:17:25.000000 zq-config-0.1.4/zq_config.egg-info/dependency_links.txt
+-rw-r--r--   0 test      (1000) test      (1001)       39 2023-08-01 08:17:25.000000 zq-config-0.1.4/zq_config.egg-info/entry_points.txt
+-rw-r--r--   0 test      (1000) test      (1001)       50 2023-08-01 08:17:25.000000 zq-config-0.1.4/zq_config.egg-info/requires.txt
+-rw-r--r--   0 test      (1000) test      (1001)       10 2023-08-01 08:17:25.000000 zq-config-0.1.4/zq_config.egg-info/top_level.txt
```

### Comparing `zq-config-0.1.3/LICENSE.txt` & `zq-config-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zq-config-0.1.3/PKG-INFO` & `zq-config-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zq-config
-Version: 0.1.3
+Version: 0.1.4
 Summary: zq-config is wrapper for config centers such as nacos
 Author-email: Tianyue Ren <rentianyue-jk@360shuke.com>
 Maintainer-email: Tianyue Ren <rentianyue-jk@360shuke.com>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
```

### Comparing `zq-config-0.1.3/pyproject.toml` & `zq-config-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "zq-config"
-version = "0.1.3"
+version = "0.1.4"
 description = "zq-config is wrapper for config centers such as nacos"
 readme = "README.md"
 
 # Specify which Python versions you support. In contrast to the
 # 'Programming Language' classifiers above, 'pip install' will check this
 # and refuse to install the project if the version does not match. See
 # https://packaging.python.org/guides/distributing-packages-using-setuptools/#python-requires
@@ -55,15 +55,15 @@
 # Any package you put here will be installed by pip when your project is
 # installed, so they must be valid existing projects.
 #
 # For an analysis of this field vs pip's requirements files see:
 # https://packaging.python.org/discussions/install-requires-vs-requirements/
 dependencies = [ # Optional
   # "peppercorn",
-  "ttl-cache"
+  "cachetools"
 ]
 
 # List additional groups of dependencies here (e.g. development
 # dependencies). Users will be able to install these using the "extras"
 # syntax, for example:
 #
 #   $ pip install sampleproject[dev]
```

### Comparing `zq-config-0.1.3/tests/test_simple.py` & `zq-config-0.1.4/tests/test_simple.py`

 * *Files identical despite different names*

### Comparing `zq-config-0.1.3/zq_config/zq_configs.py` & `zq-config-0.1.4/zq_config/zq_configs.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from typing import cast
 from importlib import import_module
 from contextlib import suppress
 from zq_config.backends import Backend
 
 from zq_config.backends.backend_registry import BACKENDS_TYPES
 
 def _try_import(module):
@@ -14,47 +13,42 @@
 
 class ZQ_Config:
     _backend: Backend = None
     _init: bool = False
     _json = None
     _toml = None
 
-    @classmethod
     def __init__(cls, backend_type, **kwargs) -> None:
         if cls._init:
             return
         if backend_type not in BACKENDS_TYPES:
             raise Exception("Not found backend {}".format(backend_type))
 
         cls._backend = BACKENDS_TYPES[backend_type](**kwargs)
 
         # try import parsers
         cls._json = _try_import("json")
         cls._toml = _try_import("toml")
 
         cls._init = True
 
-    @classmethod
     def get_raw(cls, data_id, data_group=None):
         return cls._backend.get(data_id, data_group)
 
-    @classmethod
     def get_json(cls, data_id, data_group=None):
         data = cls._backend.get(data_id, data_group)
         if cls._json == None:
             raise Exception("json module is not install")
         return cls._json.loads(data)
 
-    @classmethod
     def get_toml(cls, data_id, data_group=None):
         data = cls._backend.get(data_id, data_group)
         if cls._toml == None:
             raise Exception("toml module is not install")
         return cls._toml.loads(data)
 
-    @classmethod
     def get(cls, data_id, data_group=None, format="json"):
         if format == "json":
             return cls.get_json(data_id, data_group)
         if format == "toml":
             return cls.get_toml(data_id, data_group)
         raise Exception("{} format is not support".format(format))
```

### Comparing `zq-config-0.1.3/zq_config.egg-info/PKG-INFO` & `zq-config-0.1.4/zq_config.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zq-config
-Version: 0.1.3
+Version: 0.1.4
 Summary: zq-config is wrapper for config centers such as nacos
 Author-email: Tianyue Ren <rentianyue-jk@360shuke.com>
 Maintainer-email: Tianyue Ren <rentianyue-jk@360shuke.com>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
```

