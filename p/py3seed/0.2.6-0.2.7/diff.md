# Comparing `tmp/py3seed-0.2.6.tar.gz` & `tmp/py3seed-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3seed-0.2.6.tar", last modified: Mon Jul 31 12:57:18 2023, max compression
+gzip compressed data, was "py3seed-0.2.7.tar", last modified: Tue Aug  1 01:46:58 2023, max compression
```

## Comparing `py3seed-0.2.6.tar` & `py3seed-0.2.7.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-31 12:57:18.452658 py3seed-0.2.6/
--rw-r--r--   0 weiminfeng   (501) staff       (20)     1072 2021-08-08 16:29:42.000000 py3seed-0.2.6/LICENSE
--rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-07-31 12:57:18.452846 py3seed-0.2.6/PKG-INFO
--rw-r--r--   0 weiminfeng   (501) staff       (20)      288 2021-08-11 03:57:41.000000 py3seed-0.2.6/README.md
--rw-r--r--   0 weiminfeng   (501) staff       (20)      104 2021-09-18 08:01:25.000000 py3seed-0.2.6/pyproject.toml
--rw-r--r--   0 weiminfeng   (501) staff       (20)      911 2023-07-31 12:57:18.453701 py3seed-0.2.6/setup.cfg
--rw-r--r--   0 weiminfeng   (501) staff       (20)      214 2023-07-06 08:35:28.000000 py3seed-0.2.6/setup.py
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-31 12:57:18.414588 py3seed-0.2.6/src/
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-31 12:57:18.441412 py3seed-0.2.6/src/py3seed/
--rw-r--r--   0 weiminfeng   (501) staff       (20)      743 2023-07-10 07:31:29.000000 py3seed-0.2.6/src/py3seed/__init__.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     1624 2023-07-10 03:47:01.000000 py3seed-0.2.6/src/py3seed/__main__.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)      992 2021-09-02 08:44:38.000000 py3seed-0.2.6/src/py3seed/admin.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     7571 2023-07-21 09:02:47.000000 py3seed-0.2.6/src/py3seed/cachesupport.py
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-31 12:57:18.445358 py3seed-0.2.6/src/py3seed/commands/
--rw-r--r--   0 weiminfeng   (501) staff       (20)      151 2021-09-01 02:10:05.000000 py3seed-0.2.6/src/py3seed/commands/__init__.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    23008 2023-07-31 12:55:44.000000 py3seed-0.2.6/src/py3seed/commands/gen.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)      732 2023-06-27 01:48:25.000000 py3seed-0.2.6/src/py3seed/error.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    11554 2023-07-10 03:49:24.000000 py3seed-0.2.6/src/py3seed/inflection.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     1166 2022-05-06 11:35:05.000000 py3seed-0.2.6/src/py3seed/log.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    17725 2023-07-11 02:10:39.000000 py3seed-0.2.6/src/py3seed/merge3.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    57700 2023-07-31 04:55:20.000000 py3seed-0.2.6/src/py3seed/model.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    14489 2023-07-10 03:55:58.000000 py3seed-0.2.6/src/py3seed/mongosupport.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    14651 2023-07-27 13:10:29.000000 py3seed-0.2.6/src/py3seed/utils.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     7471 2023-07-10 03:54:22.000000 py3seed-0.2.6/src/py3seed/websupport.py
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-31 12:57:18.444293 py3seed-0.2.6/src/py3seed.egg-info/
--rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-07-31 12:57:18.000000 py3seed-0.2.6/src/py3seed.egg-info/PKG-INFO
--rw-r--r--   0 weiminfeng   (501) staff       (20)      718 2023-07-31 12:57:18.000000 py3seed-0.2.6/src/py3seed.egg-info/SOURCES.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)        1 2023-07-31 12:57:18.000000 py3seed-0.2.6/src/py3seed.egg-info/dependency_links.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)      111 2023-07-31 12:57:18.000000 py3seed-0.2.6/src/py3seed.egg-info/entry_points.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)       48 2023-07-31 12:57:18.000000 py3seed-0.2.6/src/py3seed.egg-info/requires.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)        8 2023-07-31 12:57:18.000000 py3seed-0.2.6/src/py3seed.egg-info/top_level.txt
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-31 12:57:18.452021 py3seed-0.2.6/tests/
--rw-r--r--   0 weiminfeng   (501) staff       (20)     4032 2023-07-21 09:03:11.000000 py3seed-0.2.6/tests/test_cachesupport.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     6832 2023-07-31 12:50:18.000000 py3seed-0.2.6/tests/test_gen.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    14977 2023-07-10 03:39:53.000000 py3seed-0.2.6/tests/test_merge3.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     5116 2023-07-05 06:36:00.000000 py3seed-0.2.6/tests/test_model.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     2083 2023-07-05 06:36:25.000000 py3seed-0.2.6/tests/test_mongosupport.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-01 01:46:58.603205 py3seed-0.2.7/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     1072 2021-08-08 16:29:42.000000 py3seed-0.2.7/LICENSE
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-08-01 01:46:58.603351 py3seed-0.2.7/PKG-INFO
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      288 2021-08-11 03:57:41.000000 py3seed-0.2.7/README.md
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      104 2021-09-18 08:01:25.000000 py3seed-0.2.7/pyproject.toml
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      911 2023-08-01 01:46:58.604035 py3seed-0.2.7/setup.cfg
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      214 2023-07-06 08:35:28.000000 py3seed-0.2.7/setup.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-01 01:46:58.575978 py3seed-0.2.7/src/
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-01 01:46:58.592090 py3seed-0.2.7/src/py3seed/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      743 2023-07-10 07:31:29.000000 py3seed-0.2.7/src/py3seed/__init__.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     1624 2023-07-10 03:47:01.000000 py3seed-0.2.7/src/py3seed/__main__.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      992 2021-09-02 08:44:38.000000 py3seed-0.2.7/src/py3seed/admin.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     7571 2023-07-21 09:02:47.000000 py3seed-0.2.7/src/py3seed/cachesupport.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-01 01:46:58.596161 py3seed-0.2.7/src/py3seed/commands/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      151 2021-09-01 02:10:05.000000 py3seed-0.2.7/src/py3seed/commands/__init__.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    23320 2023-08-01 01:42:44.000000 py3seed-0.2.7/src/py3seed/commands/gen.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      732 2023-06-27 01:48:25.000000 py3seed-0.2.7/src/py3seed/error.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    11554 2023-07-10 03:49:24.000000 py3seed-0.2.7/src/py3seed/inflection.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     1166 2022-05-06 11:35:05.000000 py3seed-0.2.7/src/py3seed/log.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    17725 2023-07-11 02:10:39.000000 py3seed-0.2.7/src/py3seed/merge3.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    57700 2023-07-31 04:55:20.000000 py3seed-0.2.7/src/py3seed/model.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    14489 2023-07-10 03:55:58.000000 py3seed-0.2.7/src/py3seed/mongosupport.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    14651 2023-07-27 13:10:29.000000 py3seed-0.2.7/src/py3seed/utils.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     7471 2023-07-10 03:54:22.000000 py3seed-0.2.7/src/py3seed/websupport.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-01 01:46:58.594298 py3seed-0.2.7/src/py3seed.egg-info/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-08-01 01:46:58.000000 py3seed-0.2.7/src/py3seed.egg-info/PKG-INFO
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      718 2023-08-01 01:46:58.000000 py3seed-0.2.7/src/py3seed.egg-info/SOURCES.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)        1 2023-08-01 01:46:58.000000 py3seed-0.2.7/src/py3seed.egg-info/dependency_links.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      111 2023-08-01 01:46:58.000000 py3seed-0.2.7/src/py3seed.egg-info/entry_points.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)       48 2023-08-01 01:46:58.000000 py3seed-0.2.7/src/py3seed.egg-info/requires.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)        8 2023-08-01 01:46:58.000000 py3seed-0.2.7/src/py3seed.egg-info/top_level.txt
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-01 01:46:58.602681 py3seed-0.2.7/tests/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     4032 2023-07-21 09:03:11.000000 py3seed-0.2.7/tests/test_cachesupport.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     6832 2023-07-31 12:50:18.000000 py3seed-0.2.7/tests/test_gen.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    14977 2023-07-10 03:39:53.000000 py3seed-0.2.7/tests/test_merge3.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     5116 2023-07-05 06:36:00.000000 py3seed-0.2.7/tests/test_model.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     2083 2023-07-05 06:36:25.000000 py3seed-0.2.7/tests/test_mongosupport.py
```

### Comparing `py3seed-0.2.6/LICENSE` & `py3seed-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.6/PKG-INFO` & `py3seed-0.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3seed
-Version: 0.2.6
+Version: 0.2.7
 Summary: A package that bootstraps your project by simple data models definition and auto api and user interface generation
 Home-page: https://github.com/okosioc/pyseed
 Author: Samuel Feng
 Author-email: okosioc@gmail.com
 Project-URL: Bug Tracker, https://github.com/okosioc/pyseed/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py3seed-0.2.6/setup.cfg` & `py3seed-0.2.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = py3seed
-version = 0.2.6
+version = 0.2.7
 author = Samuel Feng
 author_email = okosioc@gmail.com
 description = A package that bootstraps your project by simple data models definition and auto api and user interface generation
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/okosioc/pyseed
 project_urls =
```

### Comparing `py3seed-0.2.6/src/py3seed/__init__.py` & `py3seed-0.2.7/src/py3seed/__init__.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.6/src/py3seed/__main__.py` & `py3seed-0.2.7/src/py3seed/__main__.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.6/src/py3seed/admin.py` & `py3seed-0.2.7/src/py3seed/admin.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.6/src/py3seed/cachesupport.py` & `py3seed-0.2.7/src/py3seed/cachesupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.6/src/py3seed/commands/gen.py` & `py3seed-0.2.7/src/py3seed/commands/gen.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,34 +206,38 @@
             model_setting = {
                 'schema': schema,  # dict
                 **generate_names(model_name)
             }
             #
             views = []
             for k, v in model_class.__views__.items():
+                # k has format domains://name, domains are sperated by |, e.g, www|miniapp://index
+                if '//' not in k:
+                    logger.error(f'View name {k} for model {model_name} is not valid, should be domains://name')
+                    return False
+                domains, name = k.split('://')
+                domains = [d.strip() for d in domains.split('|')]
                 # Filter views if include_domains has value
-                domains = v['domains']
                 if include_domains:
                     domains = [d for d in domains if d in include_domains]
                 #
                 if not domains:
                     continue
                 else:
                     domain_names.update(domains)
                 # Parse view name
                 # e.g,
                 # - index -> blueprint = public, name = index
                 # - admin/dashboard -> blueprint = admin, name = dashboard
-                if '/' in k:
-                    blueprint, name = k.split('/')
+                if '/' in name:
+                    blueprint, name = name.split('/')
                 else:
                     blueprint = 'public'
-                    name = k
                 #
-                layout = v['layout'].strip()
+                layout = v
                 logger.info(f'- {blueprint}/{name}: {layout}')
                 # Validate to make sure view name is unique
                 if name in view_names:
                     logger.error(f'View name {v["name"]} is not unique')
                     return False
                 #
                 view_names.add(name)
```

### Comparing `py3seed-0.2.6/src/py3seed/error.py` & `py3seed-0.2.7/src/py3seed/error.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.6/src/py3seed/inflection.py` & `py3seed-0.2.7/src/py3seed/inflection.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.6/src/py3seed/log.py` & `py3seed-0.2.7/src/py3seed/log.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.6/src/py3seed/merge3.py` & `py3seed-0.2.7/src/py3seed/merge3.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.6/src/py3seed/model.py` & `py3seed-0.2.7/src/py3seed/model.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.6/src/py3seed/mongosupport.py` & `py3seed-0.2.7/src/py3seed/mongosupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.6/src/py3seed/utils.py` & `py3seed-0.2.7/src/py3seed/utils.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.6/src/py3seed/websupport.py` & `py3seed-0.2.7/src/py3seed/websupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.6/src/py3seed.egg-info/PKG-INFO` & `py3seed-0.2.7/src/py3seed.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3seed
-Version: 0.2.6
+Version: 0.2.7
 Summary: A package that bootstraps your project by simple data models definition and auto api and user interface generation
 Home-page: https://github.com/okosioc/pyseed
 Author: Samuel Feng
 Author-email: okosioc@gmail.com
 Project-URL: Bug Tracker, https://github.com/okosioc/pyseed/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py3seed-0.2.6/src/py3seed.egg-info/SOURCES.txt` & `py3seed-0.2.7/src/py3seed.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.6/tests/test_cachesupport.py` & `py3seed-0.2.7/tests/test_cachesupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.6/tests/test_gen.py` & `py3seed-0.2.7/tests/test_gen.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.6/tests/test_merge3.py` & `py3seed-0.2.7/tests/test_merge3.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.6/tests/test_model.py` & `py3seed-0.2.7/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.6/tests/test_mongosupport.py` & `py3seed-0.2.7/tests/test_mongosupport.py`

 * *Files identical despite different names*

