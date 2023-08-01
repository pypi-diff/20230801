# Comparing `tmp/zq-config-0.1.4.tar.gz` & `tmp/zq-config-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zq-config-0.1.4.tar", last modified: Tue Aug  1 08:17:25 2023, max compression
+gzip compressed data, was "zq-config-0.1.5.tar", last modified: Tue Aug  1 10:31:27 2023, max compression
```

## Comparing `zq-config-0.1.4.tar` & `zq-config-0.1.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 test      (1000) test      (1001)        0 2023-08-01 08:17:25.654032 zq-config-0.1.4/
--rw-r--r--   0 test      (1000) test      (1001)     1081 2023-04-21 06:48:00.000000 zq-config-0.1.4/LICENSE.txt
--rw-r--r--   0 test      (1000) test      (1001)     2992 2023-08-01 08:17:25.647365 zq-config-0.1.4/PKG-INFO
--rw-r--r--   0 test      (1000) test      (1001)      511 2023-04-21 07:12:13.000000 zq-config-0.1.4/README.md
--rw-r--r--   0 test      (1000) test      (1001)     4133 2023-08-01 08:15:51.000000 zq-config-0.1.4/pyproject.toml
--rw-r--r--   0 test      (1000) test      (1001)       38 2023-08-01 08:17:25.654032 zq-config-0.1.4/setup.cfg
-drwxr-xr-x   0 test      (1000) test      (1001)        0 2023-08-01 08:17:25.607364 zq-config-0.1.4/tests/
--rw-r--r--   0 test      (1000) test      (1001)      667 2023-04-21 08:09:21.000000 zq-config-0.1.4/tests/test_simple.py
-drwxr-xr-x   0 test      (1000) test      (1001)        0 2023-08-01 08:17:25.614031 zq-config-0.1.4/zq_config/
--rw-r--r--   0 test      (1000) test      (1001)        0 2023-04-21 09:34:13.000000 zq-config-0.1.4/zq_config/__init__.py
-drwxr-xr-x   0 test      (1000) test      (1001)        0 2023-08-01 08:17:25.647365 zq-config-0.1.4/zq_config/backends/
--rw-r--r--   0 test      (1000) test      (1001)      225 2023-06-02 03:20:30.000000 zq-config-0.1.4/zq_config/backends/__init__.py
--rw-r--r--   0 test      (1000) test      (1001)      200 2023-04-21 09:34:28.000000 zq-config-0.1.4/zq_config/backends/backend_registry.py
--rw-r--r--   0 test      (1000) test      (1001)      484 2023-08-01 08:10:35.000000 zq-config-0.1.4/zq_config/backends/nacos.py
--rw-r--r--   0 test      (1000) test      (1001)     1664 2023-08-01 08:07:36.000000 zq-config-0.1.4/zq_config/zq_configs.py
-drwxr-xr-x   0 test      (1000) test      (1001)        0 2023-08-01 08:17:25.634032 zq-config-0.1.4/zq_config.egg-info/
--rw-r--r--   0 test      (1000) test      (1001)     2992 2023-08-01 08:17:25.000000 zq-config-0.1.4/zq_config.egg-info/PKG-INFO
--rw-r--r--   0 test      (1000) test      (1001)      401 2023-08-01 08:17:25.000000 zq-config-0.1.4/zq_config.egg-info/SOURCES.txt
--rw-r--r--   0 test      (1000) test      (1001)        1 2023-08-01 08:17:25.000000 zq-config-0.1.4/zq_config.egg-info/dependency_links.txt
--rw-r--r--   0 test      (1000) test      (1001)       39 2023-08-01 08:17:25.000000 zq-config-0.1.4/zq_config.egg-info/entry_points.txt
--rw-r--r--   0 test      (1000) test      (1001)       50 2023-08-01 08:17:25.000000 zq-config-0.1.4/zq_config.egg-info/requires.txt
--rw-r--r--   0 test      (1000) test      (1001)       10 2023-08-01 08:17:25.000000 zq-config-0.1.4/zq_config.egg-info/top_level.txt
+drwxr-xr-x   0 test      (1000) test      (1001)        0 2023-08-01 10:31:27.950451 zq-config-0.1.5/
+-rw-r--r--   0 test      (1000) test      (1001)     1081 2023-04-21 06:48:00.000000 zq-config-0.1.5/LICENSE.txt
+-rw-r--r--   0 test      (1000) test      (1001)     2992 2023-08-01 10:31:27.950451 zq-config-0.1.5/PKG-INFO
+-rw-r--r--   0 test      (1000) test      (1001)      511 2023-04-21 07:12:13.000000 zq-config-0.1.5/README.md
+-rw-r--r--   0 test      (1000) test      (1001)     4133 2023-08-01 10:31:09.000000 zq-config-0.1.5/pyproject.toml
+-rw-r--r--   0 test      (1000) test      (1001)       38 2023-08-01 10:31:27.950451 zq-config-0.1.5/setup.cfg
+drwxr-xr-x   0 test      (1000) test      (1001)        0 2023-08-01 10:31:27.947118 zq-config-0.1.5/tests/
+-rw-r--r--   0 test      (1000) test      (1001)      667 2023-04-21 08:09:21.000000 zq-config-0.1.5/tests/test_simple.py
+drwxr-xr-x   0 test      (1000) test      (1001)        0 2023-08-01 10:31:27.947118 zq-config-0.1.5/zq_config/
+-rw-r--r--   0 test      (1000) test      (1001)        0 2023-04-21 09:34:13.000000 zq-config-0.1.5/zq_config/__init__.py
+drwxr-xr-x   0 test      (1000) test      (1001)        0 2023-08-01 10:31:27.950451 zq-config-0.1.5/zq_config/backends/
+-rw-r--r--   0 test      (1000) test      (1001)      225 2023-06-02 03:20:30.000000 zq-config-0.1.5/zq_config/backends/__init__.py
+-rw-r--r--   0 test      (1000) test      (1001)      200 2023-04-21 09:34:28.000000 zq-config-0.1.5/zq_config/backends/backend_registry.py
+-rw-r--r--   0 test      (1000) test      (1001)      484 2023-08-01 10:30:48.000000 zq-config-0.1.5/zq_config/backends/nacos.py
+-rw-r--r--   0 test      (1000) test      (1001)     1664 2023-08-01 08:07:36.000000 zq-config-0.1.5/zq_config/zq_configs.py
+drwxr-xr-x   0 test      (1000) test      (1001)        0 2023-08-01 10:31:27.947118 zq-config-0.1.5/zq_config.egg-info/
+-rw-r--r--   0 test      (1000) test      (1001)     2992 2023-08-01 10:31:27.000000 zq-config-0.1.5/zq_config.egg-info/PKG-INFO
+-rw-r--r--   0 test      (1000) test      (1001)      401 2023-08-01 10:31:27.000000 zq-config-0.1.5/zq_config.egg-info/SOURCES.txt
+-rw-r--r--   0 test      (1000) test      (1001)        1 2023-08-01 10:31:27.000000 zq-config-0.1.5/zq_config.egg-info/dependency_links.txt
+-rw-r--r--   0 test      (1000) test      (1001)       39 2023-08-01 10:31:27.000000 zq-config-0.1.5/zq_config.egg-info/entry_points.txt
+-rw-r--r--   0 test      (1000) test      (1001)       50 2023-08-01 10:31:27.000000 zq-config-0.1.5/zq_config.egg-info/requires.txt
+-rw-r--r--   0 test      (1000) test      (1001)       10 2023-08-01 10:31:27.000000 zq-config-0.1.5/zq_config.egg-info/top_level.txt
```

### Comparing `zq-config-0.1.4/LICENSE.txt` & `zq-config-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zq-config-0.1.4/PKG-INFO` & `zq-config-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zq-config
-Version: 0.1.4
+Version: 0.1.5
 Summary: zq-config is wrapper for config centers such as nacos
 Author-email: Tianyue Ren <rentianyue-jk@360shuke.com>
 Maintainer-email: Tianyue Ren <rentianyue-jk@360shuke.com>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
```

### Comparing `zq-config-0.1.4/pyproject.toml` & `zq-config-0.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "zq-config"
-version = "0.1.4"
+version = "0.1.5"
 description = "zq-config is wrapper for config centers such as nacos"
 readme = "README.md"
 
 # Specify which Python versions you support. In contrast to the
 # 'Programming Language' classifiers above, 'pip install' will check this
 # and refuse to install the project if the version does not match. See
 # https://packaging.python.org/guides/distributing-packages-using-setuptools/#python-requires
```

### Comparing `zq-config-0.1.4/tests/test_simple.py` & `zq-config-0.1.5/tests/test_simple.py`

 * *Files identical despite different names*

### Comparing `zq-config-0.1.4/zq_config/zq_configs.py` & `zq-config-0.1.5/zq_config/zq_configs.py`

 * *Files identical despite different names*

### Comparing `zq-config-0.1.4/zq_config.egg-info/PKG-INFO` & `zq-config-0.1.5/zq_config.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zq-config
-Version: 0.1.4
+Version: 0.1.5
 Summary: zq-config is wrapper for config centers such as nacos
 Author-email: Tianyue Ren <rentianyue-jk@360shuke.com>
 Maintainer-email: Tianyue Ren <rentianyue-jk@360shuke.com>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
```

