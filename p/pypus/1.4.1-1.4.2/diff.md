# Comparing `tmp/pypus-1.4.1.tar.gz` & `tmp/pypus-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypus-1.4.1.tar", max compression
+gzip compressed data, was "pypus-1.4.2.tar", max compression
```

## Comparing `pypus-1.4.1.tar` & `pypus-1.4.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1073 2021-05-28 19:35:21.744187 pypus-1.4.1/LICENSE
--rw-r--r--   0        0        0      114 2021-05-28 19:36:19.806135 pypus-1.4.1/README.md
--rw-r--r--   0        0        0      587 2023-07-31 21:48:29.015431 pypus-1.4.1/pyproject.toml
--rw-r--r--   0        0        0      937 2023-07-31 18:46:58.056574 pypus-1.4.1/src/pypus/Octo.py
--rw-r--r--   0        0        0        0 2021-05-11 19:37:09.641525 pypus-1.4.1/src/pypus/__init__.py
--rw-r--r--   0        0        0    33139 2023-07-31 21:36:32.576802 pypus-1.4.1/src/pypus/cli.py
--rw-r--r--   0        0        0      601 2023-07-31 21:09:19.484807 pypus-1.4.1/src/pypus/shelf.py
--rw-r--r--   0        0        0      756 1970-01-01 00:00:00.000000 pypus-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2021-05-28 19:35:21.744187 pypus-1.4.2/LICENSE
+-rw-r--r--   0        0        0      114 2021-05-28 19:36:19.806135 pypus-1.4.2/README.md
+-rw-r--r--   0        0        0      587 2023-08-01 15:04:54.031858 pypus-1.4.2/pyproject.toml
+-rw-r--r--   0        0        0      937 2023-07-31 18:46:58.056574 pypus-1.4.2/src/pypus/Octo.py
+-rw-r--r--   0        0        0        0 2021-05-11 19:37:09.641525 pypus-1.4.2/src/pypus/__init__.py
+-rw-r--r--   0        0        0    33028 2023-08-01 15:04:32.235922 pypus-1.4.2/src/pypus/cli.py
+-rw-r--r--   0        0        0      601 2023-07-31 21:09:19.484807 pypus-1.4.2/src/pypus/shelf.py
+-rw-r--r--   0        0        0      756 1970-01-01 00:00:00.000000 pypus-1.4.2/PKG-INFO
```

### Comparing `pypus-1.4.1/LICENSE` & `pypus-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pypus-1.4.1/pyproject.toml` & `pypus-1.4.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pypus"
-version = "1.4.1"
+version = "1.4.2"
 description = "Octopus cli toolkit"
 authors = ["Michael MacKenna <mmackenna@unitedfiregroup.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `pypus-1.4.1/src/pypus/Octo.py` & `pypus-1.4.2/src/pypus/Octo.py`

 * *Files identical despite different names*

### Comparing `pypus-1.4.1/src/pypus/cli.py` & `pypus-1.4.2/src/pypus/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -703,19 +703,17 @@
             print(e)
 
     for var in contents['Variables']:
         obj = Octo.OctoVar(var['Name'], var['Value'], var['Scope'])
         scopes = obj.getScope()
         if 'Environment' in scopes:
             env_list = scopes['Environment']
-            for env in env_list:
+            for index, env in enumerate(env_list):
                 if env in map_values['env_map']:
-                    env_list.remove(env)
-                    env_list.append(map_values['env_map'][env])
-                    print(f"Replaced item {env} with item {map_values['env_map'][env]}")
+                    env_list[index] = map_values['env_map'][env]
             obj.setScopeEnvironment(env_list)
         object_list.append(obj)
     for obj in object_list:
         vdict = obj.getVarAsDict()
         var_dicts.append(vdict)
     shelf.shelf_add_item(new_shelf, 'Variables', var_dicts)
```

### Comparing `pypus-1.4.1/src/pypus/shelf.py` & `pypus-1.4.2/src/pypus/shelf.py`

 * *Files identical despite different names*

### Comparing `pypus-1.4.1/PKG-INFO` & `pypus-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypus
-Version: 1.4.1
+Version: 1.4.2
 Summary: Octopus cli toolkit
 License: MIT
 Author: Michael MacKenna
 Author-email: mmackenna@unitedfiregroup.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

