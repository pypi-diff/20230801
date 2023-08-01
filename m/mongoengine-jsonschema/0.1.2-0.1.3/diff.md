# Comparing `tmp/mongoengine-jsonschema-0.1.2.tar.gz` & `tmp/mongoengine-jsonschema-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongoengine-jsonschema-0.1.2.tar", last modified: Tue Jul 18 18:15:09 2023, max compression
+gzip compressed data, was "mongoengine-jsonschema-0.1.3.tar", last modified: Tue Aug  1 11:00:57 2023, max compression
```

## Comparing `mongoengine-jsonschema-0.1.2.tar` & `mongoengine-jsonschema-0.1.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 yossi     (1000) yossi     (1000)        0 2023-07-18 18:15:09.413392 mongoengine-jsonschema-0.1.2/
--rw-rw-r--   0 yossi     (1000) yossi     (1000)     1069 2023-07-18 18:14:09.000000 mongoengine-jsonschema-0.1.2/LICENSE
--rw-rw-r--   0 yossi     (1000) yossi     (1000)       42 2023-07-18 18:14:09.000000 mongoengine-jsonschema-0.1.2/MANIFEST.in
--rw-rw-r--   0 yossi     (1000) yossi     (1000)     5545 2023-07-18 18:15:09.413392 mongoengine-jsonschema-0.1.2/PKG-INFO
--rw-rw-r--   0 yossi     (1000) yossi     (1000)     4548 2023-07-18 18:14:09.000000 mongoengine-jsonschema-0.1.2/README.md
--rw-rw-r--   0 yossi     (1000) yossi     (1000)        6 2023-07-18 18:14:09.000000 mongoengine-jsonschema-0.1.2/VERSION
--rw-rw-r--   0 yossi     (1000) yossi     (1000)      108 2023-07-18 18:14:09.000000 mongoengine-jsonschema-0.1.2/pyproject.toml
--rw-rw-r--   0 yossi     (1000) yossi     (1000)       47 2023-07-18 18:14:09.000000 mongoengine-jsonschema-0.1.2/requirements.txt
--rw-rw-r--   0 yossi     (1000) yossi     (1000)       38 2023-07-18 18:15:09.413392 mongoengine-jsonschema-0.1.2/setup.cfg
--rw-rw-r--   0 yossi     (1000) yossi     (1000)     2251 2023-07-18 18:14:09.000000 mongoengine-jsonschema-0.1.2/setup.py
-drwxrwxr-x   0 yossi     (1000) yossi     (1000)        0 2023-07-18 18:15:09.413392 mongoengine-jsonschema-0.1.2/src/
-drwxrwxr-x   0 yossi     (1000) yossi     (1000)        0 2023-07-18 18:15:09.413392 mongoengine-jsonschema-0.1.2/src/mongoengine_jsonschema/
--rw-rw-r--   0 yossi     (1000) yossi     (1000)       35 2023-07-18 18:14:09.000000 mongoengine-jsonschema-0.1.2/src/mongoengine_jsonschema/__init__.py
--rw-rw-r--   0 yossi     (1000) yossi     (1000)    13133 2023-07-18 18:14:09.000000 mongoengine-jsonschema-0.1.2/src/mongoengine_jsonschema/mixin.py
-drwxrwxr-x   0 yossi     (1000) yossi     (1000)        0 2023-07-18 18:15:09.413392 mongoengine-jsonschema-0.1.2/src/mongoengine_jsonschema.egg-info/
--rw-rw-r--   0 yossi     (1000) yossi     (1000)     5545 2023-07-18 18:15:09.000000 mongoengine-jsonschema-0.1.2/src/mongoengine_jsonschema.egg-info/PKG-INFO
--rw-rw-r--   0 yossi     (1000) yossi     (1000)      477 2023-07-18 18:15:09.000000 mongoengine-jsonschema-0.1.2/src/mongoengine_jsonschema.egg-info/SOURCES.txt
--rw-rw-r--   0 yossi     (1000) yossi     (1000)        1 2023-07-18 18:15:09.000000 mongoengine-jsonschema-0.1.2/src/mongoengine_jsonschema.egg-info/dependency_links.txt
--rw-rw-r--   0 yossi     (1000) yossi     (1000)        1 2023-07-18 18:14:58.000000 mongoengine-jsonschema-0.1.2/src/mongoengine_jsonschema.egg-info/not-zip-safe
--rw-rw-r--   0 yossi     (1000) yossi     (1000)       48 2023-07-18 18:15:09.000000 mongoengine-jsonschema-0.1.2/src/mongoengine_jsonschema.egg-info/requires.txt
--rw-rw-r--   0 yossi     (1000) yossi     (1000)       23 2023-07-18 18:15:09.000000 mongoengine-jsonschema-0.1.2/src/mongoengine_jsonschema.egg-info/top_level.txt
-drwxrwxr-x   0 yossi     (1000) yossi     (1000)        0 2023-07-18 18:15:09.413392 mongoengine-jsonschema-0.1.2/tests/
--rw-rw-r--   0 yossi     (1000) yossi     (1000)    31999 2023-07-18 18:14:09.000000 mongoengine-jsonschema-0.1.2/tests/test_json_schema.py
+drwxrwxr-x   0 yossi     (1000) yossi     (1000)        0 2023-08-01 11:00:57.746960 mongoengine-jsonschema-0.1.3/
+-rw-rw-r--   0 yossi     (1000) yossi     (1000)     1069 2023-07-18 18:14:09.000000 mongoengine-jsonschema-0.1.3/LICENSE
+-rw-rw-r--   0 yossi     (1000) yossi     (1000)       42 2023-07-18 18:14:09.000000 mongoengine-jsonschema-0.1.3/MANIFEST.in
+-rw-rw-r--   0 yossi     (1000) yossi     (1000)     5544 2023-08-01 11:00:57.746960 mongoengine-jsonschema-0.1.3/PKG-INFO
+-rw-rw-r--   0 yossi     (1000) yossi     (1000)     4548 2023-07-18 18:14:09.000000 mongoengine-jsonschema-0.1.3/README.md
+-rw-rw-r--   0 yossi     (1000) yossi     (1000)        5 2023-08-01 11:00:38.000000 mongoengine-jsonschema-0.1.3/VERSION
+-rw-rw-r--   0 yossi     (1000) yossi     (1000)      108 2023-07-18 18:14:09.000000 mongoengine-jsonschema-0.1.3/pyproject.toml
+-rw-rw-r--   0 yossi     (1000) yossi     (1000)       47 2023-07-18 18:14:09.000000 mongoengine-jsonschema-0.1.3/requirements.txt
+-rw-rw-r--   0 yossi     (1000) yossi     (1000)       38 2023-08-01 11:00:57.746960 mongoengine-jsonschema-0.1.3/setup.cfg
+-rw-rw-r--   0 yossi     (1000) yossi     (1000)     2265 2023-08-01 11:00:38.000000 mongoengine-jsonschema-0.1.3/setup.py
+drwxrwxr-x   0 yossi     (1000) yossi     (1000)        0 2023-08-01 11:00:57.742960 mongoengine-jsonschema-0.1.3/src/
+drwxrwxr-x   0 yossi     (1000) yossi     (1000)        0 2023-08-01 11:00:57.746960 mongoengine-jsonschema-0.1.3/src/mongoengine_jsonschema/
+-rw-rw-r--   0 yossi     (1000) yossi     (1000)       35 2023-07-18 18:14:09.000000 mongoengine-jsonschema-0.1.3/src/mongoengine_jsonschema/__init__.py
+-rw-rw-r--   0 yossi     (1000) yossi     (1000)    13133 2023-07-18 18:14:09.000000 mongoengine-jsonschema-0.1.3/src/mongoengine_jsonschema/mixin.py
+drwxrwxr-x   0 yossi     (1000) yossi     (1000)        0 2023-08-01 11:00:57.746960 mongoengine-jsonschema-0.1.3/src/mongoengine_jsonschema.egg-info/
+-rw-rw-r--   0 yossi     (1000) yossi     (1000)     5544 2023-08-01 11:00:57.000000 mongoengine-jsonschema-0.1.3/src/mongoengine_jsonschema.egg-info/PKG-INFO
+-rw-rw-r--   0 yossi     (1000) yossi     (1000)      477 2023-08-01 11:00:57.000000 mongoengine-jsonschema-0.1.3/src/mongoengine_jsonschema.egg-info/SOURCES.txt
+-rw-rw-r--   0 yossi     (1000) yossi     (1000)        1 2023-08-01 11:00:57.000000 mongoengine-jsonschema-0.1.3/src/mongoengine_jsonschema.egg-info/dependency_links.txt
+-rw-rw-r--   0 yossi     (1000) yossi     (1000)        1 2023-08-01 11:00:47.000000 mongoengine-jsonschema-0.1.3/src/mongoengine_jsonschema.egg-info/not-zip-safe
+-rw-rw-r--   0 yossi     (1000) yossi     (1000)       48 2023-08-01 11:00:57.000000 mongoengine-jsonschema-0.1.3/src/mongoengine_jsonschema.egg-info/requires.txt
+-rw-rw-r--   0 yossi     (1000) yossi     (1000)       23 2023-08-01 11:00:57.000000 mongoengine-jsonschema-0.1.3/src/mongoengine_jsonschema.egg-info/top_level.txt
+drwxrwxr-x   0 yossi     (1000) yossi     (1000)        0 2023-08-01 11:00:57.746960 mongoengine-jsonschema-0.1.3/tests/
+-rw-rw-r--   0 yossi     (1000) yossi     (1000)    31999 2023-07-18 18:14:09.000000 mongoengine-jsonschema-0.1.3/tests/test_json_schema.py
```

### Comparing `mongoengine-jsonschema-0.1.2/LICENSE` & `mongoengine-jsonschema-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mongoengine-jsonschema-0.1.2/PKG-INFO` & `mongoengine-jsonschema-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongoengine-jsonschema
-Version: 0.1.2
+Version: 0.1.3
 Summary: MongoEngine JSON Schema Generator
 Home-page: https://github.com/symphonicityy/mongoengine-jsonschema
 Author: Yusuf Eroglu
 Author-email: myusuferoglu@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/symphonicityy/mongoengine-jsonschema/blob/main/README.md
 Project-URL: Code, https://github.com/symphonicityy/mongoengine-jsonschema
@@ -15,15 +15,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: File Formats :: JSON
 Classifier: Topic :: File Formats :: JSON :: JSON Schema
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Database
-Requires-Python: >=3.10
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # JSON Schema Generator for MongoEngine Documents
 
 ## 📖 About the project
```

### Comparing `mongoengine-jsonschema-0.1.2/README.md` & `mongoengine-jsonschema-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `mongoengine-jsonschema-0.1.2/setup.py` & `mongoengine-jsonschema-0.1.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 NAME = 'mongoengine-jsonschema'
 
 with open('VERSION', 'r') as f:
     VERSION = f.readline().strip('\n')
 
 this_directory = Path(__file__).parent
-DESCRIPTION = (this_directory / "README.md").read_text()
+DESCRIPTION = (this_directory / "README.md").read_text(encoding='utf8')
 
 meta = {
     'version': VERSION,
     'doc': 'MongoEngine JSON Schema Generator',
     'author': 'Yusuf Eroglu',
     'contact': 'myusuferoglu@gmail.com',
     'homepage': "https://github.com/symphonicityy/mongoengine-jsonschema"
@@ -54,15 +54,15 @@
     author_email=meta['contact'],
     url=meta['homepage'],
     license='MIT',
     platforms=['any'],
     install_requires=install_requires(),
     package_dir={'': 'src'},
     packages=setuptools.find_packages('src'),
-    python_requires=">=3.10",
+    python_requires=">=3.8",
     include_package_data=True,
     zip_safe=False,
     project_urls={
         "Documentation": "https://github.com/symphonicityy/mongoengine-jsonschema/blob/main/README.md",
         "Code": "https://github.com/symphonicityy/mongoengine-jsonschema",
     },
     classifiers=[
```

### Comparing `mongoengine-jsonschema-0.1.2/src/mongoengine_jsonschema/mixin.py` & `mongoengine-jsonschema-0.1.3/src/mongoengine_jsonschema/mixin.py`

 * *Files identical despite different names*

### Comparing `mongoengine-jsonschema-0.1.2/src/mongoengine_jsonschema.egg-info/PKG-INFO` & `mongoengine-jsonschema-0.1.3/src/mongoengine_jsonschema.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongoengine-jsonschema
-Version: 0.1.2
+Version: 0.1.3
 Summary: MongoEngine JSON Schema Generator
 Home-page: https://github.com/symphonicityy/mongoengine-jsonschema
 Author: Yusuf Eroglu
 Author-email: myusuferoglu@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/symphonicityy/mongoengine-jsonschema/blob/main/README.md
 Project-URL: Code, https://github.com/symphonicityy/mongoengine-jsonschema
@@ -15,15 +15,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: File Formats :: JSON
 Classifier: Topic :: File Formats :: JSON :: JSON Schema
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Database
-Requires-Python: >=3.10
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # JSON Schema Generator for MongoEngine Documents
 
 ## 📖 About the project
```

### Comparing `mongoengine-jsonschema-0.1.2/tests/test_json_schema.py` & `mongoengine-jsonschema-0.1.3/tests/test_json_schema.py`

 * *Files identical despite different names*

