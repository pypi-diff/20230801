# Comparing `tmp/py3seed-0.2.8.tar.gz` & `tmp/py3seed-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3seed-0.2.8.tar", last modified: Tue Aug  1 07:45:35 2023, max compression
+gzip compressed data, was "py3seed-0.2.9.tar", last modified: Tue Aug  1 08:50:26 2023, max compression
```

## Comparing `py3seed-0.2.8.tar` & `py3seed-0.2.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-01 07:45:35.005659 py3seed-0.2.8/
--rw-r--r--   0 weiminfeng   (501) staff       (20)     1072 2021-08-08 16:29:42.000000 py3seed-0.2.8/LICENSE
--rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-08-01 07:45:35.005887 py3seed-0.2.8/PKG-INFO
--rw-r--r--   0 weiminfeng   (501) staff       (20)      288 2021-08-11 03:57:41.000000 py3seed-0.2.8/README.md
--rw-r--r--   0 weiminfeng   (501) staff       (20)      104 2021-09-18 08:01:25.000000 py3seed-0.2.8/pyproject.toml
--rw-r--r--   0 weiminfeng   (501) staff       (20)      911 2023-08-01 07:45:35.007070 py3seed-0.2.8/setup.cfg
--rw-r--r--   0 weiminfeng   (501) staff       (20)      214 2023-07-06 08:35:28.000000 py3seed-0.2.8/setup.py
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-01 07:45:34.978241 py3seed-0.2.8/src/
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-01 07:45:34.995212 py3seed-0.2.8/src/py3seed/
--rw-r--r--   0 weiminfeng   (501) staff       (20)      743 2023-07-10 07:31:29.000000 py3seed-0.2.8/src/py3seed/__init__.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     1624 2023-07-10 03:47:01.000000 py3seed-0.2.8/src/py3seed/__main__.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)      992 2021-09-02 08:44:38.000000 py3seed-0.2.8/src/py3seed/admin.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     7571 2023-07-21 09:02:47.000000 py3seed-0.2.8/src/py3seed/cachesupport.py
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-01 07:45:34.999745 py3seed-0.2.8/src/py3seed/commands/
--rw-r--r--   0 weiminfeng   (501) staff       (20)      151 2021-09-01 02:10:05.000000 py3seed-0.2.8/src/py3seed/commands/__init__.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    23359 2023-08-01 07:38:02.000000 py3seed-0.2.8/src/py3seed/commands/gen.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)      732 2023-06-27 01:48:25.000000 py3seed-0.2.8/src/py3seed/error.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    11554 2023-07-10 03:49:24.000000 py3seed-0.2.8/src/py3seed/inflection.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     1166 2022-05-06 11:35:05.000000 py3seed-0.2.8/src/py3seed/log.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    17725 2023-07-11 02:10:39.000000 py3seed-0.2.8/src/py3seed/merge3.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    57700 2023-07-31 04:55:20.000000 py3seed-0.2.8/src/py3seed/model.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    14489 2023-07-10 03:55:58.000000 py3seed-0.2.8/src/py3seed/mongosupport.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    14651 2023-07-27 13:10:29.000000 py3seed-0.2.8/src/py3seed/utils.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     7471 2023-07-10 03:54:22.000000 py3seed-0.2.8/src/py3seed/websupport.py
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-01 07:45:34.997927 py3seed-0.2.8/src/py3seed.egg-info/
--rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-08-01 07:45:34.000000 py3seed-0.2.8/src/py3seed.egg-info/PKG-INFO
--rw-r--r--   0 weiminfeng   (501) staff       (20)      718 2023-08-01 07:45:34.000000 py3seed-0.2.8/src/py3seed.egg-info/SOURCES.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)        1 2023-08-01 07:45:34.000000 py3seed-0.2.8/src/py3seed.egg-info/dependency_links.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)      111 2023-08-01 07:45:34.000000 py3seed-0.2.8/src/py3seed.egg-info/entry_points.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)       48 2023-08-01 07:45:34.000000 py3seed-0.2.8/src/py3seed.egg-info/requires.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)        8 2023-08-01 07:45:34.000000 py3seed-0.2.8/src/py3seed.egg-info/top_level.txt
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-01 07:45:35.005052 py3seed-0.2.8/tests/
--rw-r--r--   0 weiminfeng   (501) staff       (20)     4032 2023-07-21 09:03:11.000000 py3seed-0.2.8/tests/test_cachesupport.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     6832 2023-07-31 12:50:18.000000 py3seed-0.2.8/tests/test_gen.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    14977 2023-07-10 03:39:53.000000 py3seed-0.2.8/tests/test_merge3.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     5116 2023-07-05 06:36:00.000000 py3seed-0.2.8/tests/test_model.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     2083 2023-07-05 06:36:25.000000 py3seed-0.2.8/tests/test_mongosupport.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-01 08:50:26.741783 py3seed-0.2.9/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     1072 2021-08-08 16:29:42.000000 py3seed-0.2.9/LICENSE
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-08-01 08:50:26.741918 py3seed-0.2.9/PKG-INFO
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      288 2021-08-11 03:57:41.000000 py3seed-0.2.9/README.md
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      104 2021-09-18 08:01:25.000000 py3seed-0.2.9/pyproject.toml
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      911 2023-08-01 08:50:26.742534 py3seed-0.2.9/setup.cfg
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      214 2023-07-06 08:35:28.000000 py3seed-0.2.9/setup.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-01 08:50:26.715424 py3seed-0.2.9/src/
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-01 08:50:26.730803 py3seed-0.2.9/src/py3seed/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      743 2023-07-10 07:31:29.000000 py3seed-0.2.9/src/py3seed/__init__.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     1624 2023-07-10 03:47:01.000000 py3seed-0.2.9/src/py3seed/__main__.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      992 2021-09-02 08:44:38.000000 py3seed-0.2.9/src/py3seed/admin.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     7571 2023-07-21 09:02:47.000000 py3seed-0.2.9/src/py3seed/cachesupport.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-01 08:50:26.734623 py3seed-0.2.9/src/py3seed/commands/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      151 2021-09-01 02:10:05.000000 py3seed-0.2.9/src/py3seed/commands/__init__.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    22949 2023-08-01 08:49:28.000000 py3seed-0.2.9/src/py3seed/commands/gen.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      732 2023-06-27 01:48:25.000000 py3seed-0.2.9/src/py3seed/error.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    11554 2023-07-10 03:49:24.000000 py3seed-0.2.9/src/py3seed/inflection.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     1166 2022-05-06 11:35:05.000000 py3seed-0.2.9/src/py3seed/log.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    17725 2023-07-11 02:10:39.000000 py3seed-0.2.9/src/py3seed/merge3.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    57700 2023-07-31 04:55:20.000000 py3seed-0.2.9/src/py3seed/model.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    14489 2023-07-10 03:55:58.000000 py3seed-0.2.9/src/py3seed/mongosupport.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    14651 2023-07-27 13:10:29.000000 py3seed-0.2.9/src/py3seed/utils.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     7471 2023-07-10 03:54:22.000000 py3seed-0.2.9/src/py3seed/websupport.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-01 08:50:26.733484 py3seed-0.2.9/src/py3seed.egg-info/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-08-01 08:50:26.000000 py3seed-0.2.9/src/py3seed.egg-info/PKG-INFO
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      718 2023-08-01 08:50:26.000000 py3seed-0.2.9/src/py3seed.egg-info/SOURCES.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)        1 2023-08-01 08:50:26.000000 py3seed-0.2.9/src/py3seed.egg-info/dependency_links.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      111 2023-08-01 08:50:26.000000 py3seed-0.2.9/src/py3seed.egg-info/entry_points.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)       48 2023-08-01 08:50:26.000000 py3seed-0.2.9/src/py3seed.egg-info/requires.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)        8 2023-08-01 08:50:26.000000 py3seed-0.2.9/src/py3seed.egg-info/top_level.txt
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-01 08:50:26.741102 py3seed-0.2.9/tests/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     4032 2023-07-21 09:03:11.000000 py3seed-0.2.9/tests/test_cachesupport.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     6832 2023-07-31 12:50:18.000000 py3seed-0.2.9/tests/test_gen.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    14977 2023-07-10 03:39:53.000000 py3seed-0.2.9/tests/test_merge3.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     5116 2023-07-05 06:36:00.000000 py3seed-0.2.9/tests/test_model.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     2083 2023-07-05 06:36:25.000000 py3seed-0.2.9/tests/test_mongosupport.py
```

### Comparing `py3seed-0.2.8/LICENSE` & `py3seed-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.8/PKG-INFO` & `py3seed-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3seed
-Version: 0.2.8
+Version: 0.2.9
 Summary: A package that bootstraps your project by simple data models definition and auto api and user interface generation
 Home-page: https://github.com/okosioc/pyseed
 Author: Samuel Feng
 Author-email: okosioc@gmail.com
 Project-URL: Bug Tracker, https://github.com/okosioc/pyseed/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py3seed-0.2.8/setup.cfg` & `py3seed-0.2.9/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = py3seed
-version = 0.2.8
+version = 0.2.9
 author = Samuel Feng
 author_email = okosioc@gmail.com
 description = A package that bootstraps your project by simple data models definition and auto api and user interface generation
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/okosioc/pyseed
 project_urls =
```

### Comparing `py3seed-0.2.8/src/py3seed/__init__.py` & `py3seed-0.2.9/src/py3seed/__init__.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.8/src/py3seed/__main__.py` & `py3seed-0.2.9/src/py3seed/__main__.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.8/src/py3seed/admin.py` & `py3seed-0.2.9/src/py3seed/admin.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.8/src/py3seed/cachesupport.py` & `py3seed-0.2.9/src/py3seed/cachesupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.8/src/py3seed/commands/gen.py` & `py3seed-0.2.9/src/py3seed/commands/gen.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,50 +53,25 @@
         return url_encode(args)
 
     def new_model(class_name):
         """ New a model by class name. """
         klass = globals()[class_name]
         return klass()
 
-    def match_field(fields_, matcher):
-        """ Get the first matching field from columns.
-        e.g,
-        - match_field(columns, 'name|title|\\w+_name')
-        """
-        matcher = re.compile(matcher if matcher.startswith('(') else f'({matcher})')
-        if isinstance(fields_, dict):
-            fields_ = fields_.keys()
-        #
-        for f in fields_:
-            if matcher.match(f):
-                return f
-        # If no matching, return nothing
-        return None
-
-    def parse_layout_fields(layout):
-        """ Get layout fields.
-
-        each column in layout can be blank('')/hyphen(-)/group(integer&float)/field(string) suffixed with query and format-span string
-        this function will return a list of field names.
-        """
-        return list(get_layout_fields(layout))
-
     def exists(path):
         """ Check if path exists. """
         # Only support FileSystemLoader which has a searchpath
         if not isinstance(env.loader, FileSystemLoader):
             return False
         #
         fp = os.path.join(env.loader.searchpath[0], path)
         return os.path.exists(fp)
 
     env.globals['update_query'] = update_query
     env.globals['new_model'] = new_model
-    env.globals['match_field'] = match_field
-    env.globals['parse_layout_fields'] = parse_layout_fields
     env.globals['exists'] = exists
 
     def split(value, separator):
         """ Split a string. """
         return value.split(separator)
 
     def items(value):
@@ -130,18 +105,33 @@
         #
         return s
 
     def last_name(path):
         """ Get last name from path, e.g, user.name -> name, user -> user. """
         return path.split('.')[-1]
 
+    def match(values, matcher):
+        """ Get the first matching field from values.
+        e.g,
+        - values|match('name|title|\\w+_name')
+        """
+        matcher = re.compile(matcher if matcher.startswith('(') else f'({matcher})')
+        if isinstance(values, dict):
+            values = values.keys()
+        #
+        for v in values:
+            if matcher.match(v):
+                return v
+        # If no matching, return nothing
+        return None
+
     def fields(layout_or_schema, matcher=None):
         """ Get the matched fields from layout or schema. """
         if isinstance(layout_or_schema, list):  # layout is [[{}, ...], ...]
-            _fields = parse_layout_fields(layout_or_schema)
+            _fields = list(get_layout_fields(layout_or_schema))
         elif isinstance(layout_or_schema, dict):  # schema is dict {type: 'object', properties: {name, type, ... }}
             _fields = list(layout_or_schema['properties'].keys())
         else:
             raise ValueError(f'Unsupported type to calculate fields: {type(layout_or_schema)}')
         #
         if matcher:
             # NOTE: in jinja2, you need to escape regex str, e.g, \w -> \\w
@@ -160,14 +150,15 @@
     env.filters['items'] = items
     env.filters['keys'] = keys
     env.filters['quote'] = quote
     env.filters['basename'] = basename
     env.filters['urlquote'] = urlquote
     env.filters['right'] = right
     env.filters['last_name'] = last_name
+    env.filters['match'] = match
     env.filters['fields'] = fields
     env.filters['field'] = field
     #
     return env
 
 
 def _gen(ds: str = None):
```

### Comparing `py3seed-0.2.8/src/py3seed/error.py` & `py3seed-0.2.9/src/py3seed/error.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.8/src/py3seed/inflection.py` & `py3seed-0.2.9/src/py3seed/inflection.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.8/src/py3seed/log.py` & `py3seed-0.2.9/src/py3seed/log.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.8/src/py3seed/merge3.py` & `py3seed-0.2.9/src/py3seed/merge3.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.8/src/py3seed/model.py` & `py3seed-0.2.9/src/py3seed/model.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.8/src/py3seed/mongosupport.py` & `py3seed-0.2.9/src/py3seed/mongosupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.8/src/py3seed/utils.py` & `py3seed-0.2.9/src/py3seed/utils.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.8/src/py3seed/websupport.py` & `py3seed-0.2.9/src/py3seed/websupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.8/src/py3seed.egg-info/PKG-INFO` & `py3seed-0.2.9/src/py3seed.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3seed
-Version: 0.2.8
+Version: 0.2.9
 Summary: A package that bootstraps your project by simple data models definition and auto api and user interface generation
 Home-page: https://github.com/okosioc/pyseed
 Author: Samuel Feng
 Author-email: okosioc@gmail.com
 Project-URL: Bug Tracker, https://github.com/okosioc/pyseed/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py3seed-0.2.8/src/py3seed.egg-info/SOURCES.txt` & `py3seed-0.2.9/src/py3seed.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.8/tests/test_cachesupport.py` & `py3seed-0.2.9/tests/test_cachesupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.8/tests/test_gen.py` & `py3seed-0.2.9/tests/test_gen.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.8/tests/test_merge3.py` & `py3seed-0.2.9/tests/test_merge3.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.8/tests/test_model.py` & `py3seed-0.2.9/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.8/tests/test_mongosupport.py` & `py3seed-0.2.9/tests/test_mongosupport.py`

 * *Files identical despite different names*

