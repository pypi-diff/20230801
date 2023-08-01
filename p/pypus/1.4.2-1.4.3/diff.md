# Comparing `tmp/pypus-1.4.2.tar.gz` & `tmp/pypus-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypus-1.4.2.tar", max compression
+gzip compressed data, was "pypus-1.4.3.tar", max compression
```

## Comparing `pypus-1.4.2.tar` & `pypus-1.4.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1073 2021-05-28 19:35:21.744187 pypus-1.4.2/LICENSE
--rw-r--r--   0        0        0      114 2021-05-28 19:36:19.806135 pypus-1.4.2/README.md
--rw-r--r--   0        0        0      587 2023-08-01 15:04:54.031858 pypus-1.4.2/pyproject.toml
--rw-r--r--   0        0        0      937 2023-07-31 18:46:58.056574 pypus-1.4.2/src/pypus/Octo.py
--rw-r--r--   0        0        0        0 2021-05-11 19:37:09.641525 pypus-1.4.2/src/pypus/__init__.py
--rw-r--r--   0        0        0    33028 2023-08-01 15:04:32.235922 pypus-1.4.2/src/pypus/cli.py
--rw-r--r--   0        0        0      601 2023-07-31 21:09:19.484807 pypus-1.4.2/src/pypus/shelf.py
--rw-r--r--   0        0        0      756 1970-01-01 00:00:00.000000 pypus-1.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2021-05-28 19:35:21.744187 pypus-1.4.3/LICENSE
+-rw-r--r--   0        0        0      104 2023-08-01 16:02:31.723883 pypus-1.4.3/README.md
+-rw-r--r--   0        0        0      629 2023-08-01 16:14:46.780146 pypus-1.4.3/pyproject.toml
+-rw-r--r--   0        0        0      937 2023-07-31 18:46:58.056574 pypus-1.4.3/src/pypus/Octo.py
+-rw-r--r--   0        0        0        0 2021-05-11 19:37:09.641525 pypus-1.4.3/src/pypus/__init__.py
+-rw-r--r--   0        0        0    33323 2023-08-01 16:13:54.300487 pypus-1.4.3/src/pypus/cli.py
+-rw-r--r--   0        0        0      601 2023-07-31 21:09:19.484807 pypus-1.4.3/src/pypus/shelf.py
+-rw-r--r--   0        0        0      746 1970-01-01 00:00:00.000000 pypus-1.4.3/PKG-INFO
```

### Comparing `pypus-1.4.2/LICENSE` & `pypus-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pypus-1.4.2/pyproject.toml` & `pypus-1.4.3/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pypus"
-version = "1.4.2"
+version = "1.4.3"
 description = "Octopus cli toolkit"
 authors = ["Michael MacKenna <mmackenna@unitedfiregroup.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
@@ -19,11 +19,13 @@
 pylint = "^2.8.2"
 
 [tool.poetry.scripts]
 pypus = 'pypus.cli:main'
 
 [tool.poetry.group.dev.dependencies]
 ipython = "^8.14.0"
+mkdocs = "^1.5.1"
+mkdocs-click = "^0.8.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pypus-1.4.2/src/pypus/Octo.py` & `pypus-1.4.3/src/pypus/Octo.py`

 * *Files identical despite different names*

### Comparing `pypus-1.4.2/src/pypus/cli.py` & `pypus-1.4.3/src/pypus/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -650,31 +650,39 @@
             else:
                 cprint('No publishing needed', 'green')
 
 
 @main.command('read-yaml', short_help='Read a yaml file')
 @click.argument('yaml-file', type=click.Path(exists=True))
 def import_yaml(yaml_file):
+    """ Reads a yaml file """
     with open(yaml_file, "r") as stream:
         try:
             print(yaml.safe_load(stream))
         except yaml.YAMLError as exc:
             print(exc)
 
 
 @main.command("list-shelf-data", short_help="Print data in a shelf")
 @click.argument("shelf_name")
 def list_shelf_data(shelf_name):
+    """ Lists out contents for a Python shelf
+    do not provide the file extension for the shelf
+    you are referencing. The path should be included
+    """
     contents = shelf.shelf_list_contents(shelf_name)
 
 
 @main.command("get-shelf-key", short_help="Print data for a key in a shelf")
 @click.argument("shelf_name")
 @click.argument("key_name")
 def get_shelf_key(shelf_name, key_name):
+    """ Assuming your shelf is a list of key value pairs,
+    get the value for a particular key.
+    """
     contents = shelf.get_shelf_item(shelf_name, key_name)
     for var in contents['Variables']:
         print(f"{var['Name']} {var['Value']} {var['Scope']}")
 
 
 @main.command('transpose-from-shelf', short_help='Transpose varaibles from shelf')
 @click.argument('shelf-name')
```

### Comparing `pypus-1.4.2/src/pypus/shelf.py` & `pypus-1.4.3/src/pypus/shelf.py`

 * *Files identical despite different names*

### Comparing `pypus-1.4.2/PKG-INFO` & `pypus-1.4.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypus
-Version: 1.4.2
+Version: 1.4.3
 Summary: Octopus cli toolkit
 License: MIT
 Author: Michael MacKenna
 Author-email: mmackenna@unitedfiregroup.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -15,15 +15,15 @@
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: requests (>=2.25.1,<3.0.0)
 Requires-Dist: termcolor (>=1.1.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Pypus
 
-Pypus is a cli tool for publishing Octopus Deploy Runbooks.
+Pypus is a cli tool for Octopus Deploy API tasks.
 
 ## Install
 
 ```bash
 $ pip install pypus
 ```
```

