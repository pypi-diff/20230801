# Comparing `tmp/awspstore-1.3.0.tar.gz` & `tmp/awspstore-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awspstore-1.3.0.tar", last modified: Mon Nov  7 13:48:54 2022, max compression
+gzip compressed data, was "awspstore-1.4.0.tar", last modified: Tue Aug  1 10:34:39 2023, max compression
```

## Comparing `awspstore-1.3.0.tar` & `awspstore-1.4.0.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 13:48:54.485707 awspstore-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1062 2022-11-07 13:48:41.000000 awspstore-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2493 2022-11-07 13:48:54.485707 awspstore-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2037 2022-11-07 13:48:41.000000 awspstore-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 13:48:54.481707 awspstore-1.3.0/awspstore/
--rw-r--r--   0 runner    (1001) docker     (121)     3053 2022-11-07 13:48:41.000000 awspstore-1.3.0/awspstore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 13:48:54.481707 awspstore-1.3.0/awspstore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2493 2022-11-07 13:48:54.000000 awspstore-1.3.0/awspstore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      212 2022-11-07 13:48:54.000000 awspstore-1.3.0/awspstore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-07 13:48:54.000000 awspstore-1.3.0/awspstore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-11-07 13:48:54.000000 awspstore-1.3.0/awspstore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-11-07 13:48:54.000000 awspstore-1.3.0/awspstore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-07 13:48:54.485707 awspstore-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      755 2022-11-07 13:48:41.000000 awspstore-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:34:39.576294 awspstore-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-08-01 10:34:12.000000 awspstore-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-08-01 10:34:39.576294 awspstore-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-08-01 10:34:12.000000 awspstore-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:34:39.572294 awspstore-1.4.0/awspstore/
+-rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-08-01 10:34:12.000000 awspstore-1.4.0/awspstore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:34:39.572294 awspstore-1.4.0/awspstore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-08-01 10:34:39.000000 awspstore-1.4.0/awspstore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-08-01 10:34:39.000000 awspstore-1.4.0/awspstore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 10:34:39.000000 awspstore-1.4.0/awspstore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-01 10:34:39.000000 awspstore-1.4.0/awspstore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-01 10:34:39.000000 awspstore-1.4.0/awspstore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 10:34:39.576294 awspstore-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-08-01 10:34:12.000000 awspstore-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:34:39.572294 awspstore-1.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-08-01 10:34:12.000000 awspstore-1.4.0/tests/test_utils.py
```

### Comparing `awspstore-1.3.0/LICENSE` & `awspstore-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `awspstore-1.3.0/PKG-INFO` & `awspstore-1.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awspstore
-Version: 1.3.0
+Version: 1.4.0
 Summary: Vault for your software project using AWS Parameter Store
 Home-page: https://github.com/eldad1221/aws-vault
 Author: Eldad Bishari
 Author-email: eldad@1221tlv.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `awspstore-1.3.0/README.md` & `awspstore-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `awspstore-1.3.0/awspstore/__init__.py` & `awspstore-1.4.0/awspstore/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -62,14 +62,32 @@
 
         if dump_parameters:
             log_parameter(k=p_name, v=value)
 
     return result
 
 
+def get_parameters_by_path(path: str, env_vars: list, update_environ: bool = False, dump_parameters: bool = False):
+    params = {}
+    chunk_size = 10
+    for i in range(0, len(env_vars), chunk_size):
+        x = i
+        vars_to_load = env_vars[x:x + chunk_size]
+        params.update(
+            get_parameters_value(
+                path=f'/{path}',
+                parameters=[f'/{path}/{p_name}' for p_name in vars_to_load],
+                update_environ=update_environ,
+                dump_parameters=dump_parameters
+            )
+        )
+    Log.debug(f'Path {path}, loaded {len(params)} variables.')
+    return params
+
+
 def dump(d: dict):
     for k, v in sorted(d.items()):
         log_parameter(k=k, v=v)
 
 
 def log_parameter(k: str, v: str):
     if is_secret(k):
```

### Comparing `awspstore-1.3.0/awspstore.egg-info/PKG-INFO` & `awspstore-1.4.0/awspstore.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awspstore
-Version: 1.3.0
+Version: 1.4.0
 Summary: Vault for your software project using AWS Parameter Store
 Home-page: https://github.com/eldad1221/aws-vault
 Author: Eldad Bishari
 Author-email: eldad@1221tlv.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `awspstore-1.3.0/setup.py` & `awspstore-1.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="awspstore",
-    version="1.3.0",
+    version="1.4.0",
     author="Eldad Bishari",
     author_email="eldad@1221tlv.org",
     description="Vault for your software project using AWS Parameter Store",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/eldad1221/aws-vault",
     packages=setuptools.find_packages(),
```

