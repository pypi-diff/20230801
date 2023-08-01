# Comparing `tmp/nligraphspacy-1.1.6.tar.gz` & `tmp/nligraphspacy-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nligraphspacy-1.1.6.tar", last modified: Sat Jun 24 15:11:47 2023, max compression
+gzip compressed data, was "nligraphspacy-1.1.7.tar", last modified: Tue Aug  1 02:52:57 2023, max compression
```

## Comparing `nligraphspacy-1.1.6.tar` & `nligraphspacy-1.1.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:11:47.870214 nligraphspacy-1.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-24 15:11:35.000000 nligraphspacy-1.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-06-24 15:11:47.870214 nligraphspacy-1.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-24 15:11:35.000000 nligraphspacy-1.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:11:47.870214 nligraphspacy-1.1.6/nligraphspacy/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-24 15:11:35.000000 nligraphspacy-1.1.6/nligraphspacy/NLIGRAPH.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 15:11:35.000000 nligraphspacy-1.1.6/nligraphspacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:11:47.870214 nligraphspacy-1.1.6/nligraphspacy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-06-24 15:11:47.000000 nligraphspacy-1.1.6/nligraphspacy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-24 15:11:47.000000 nligraphspacy-1.1.6/nligraphspacy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 15:11:47.000000 nligraphspacy-1.1.6/nligraphspacy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 15:11:47.000000 nligraphspacy-1.1.6/nligraphspacy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-24 15:11:47.000000 nligraphspacy-1.1.6/nligraphspacy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-24 15:11:47.000000 nligraphspacy-1.1.6/nligraphspacy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 15:11:47.870214 nligraphspacy-1.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-24 15:11:35.000000 nligraphspacy-1.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:52:57.842520 nligraphspacy-1.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-01 02:52:42.000000 nligraphspacy-1.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-08-01 02:52:57.838519 nligraphspacy-1.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-08-01 02:52:42.000000 nligraphspacy-1.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:52:57.838519 nligraphspacy-1.1.7/nligraphspacy/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-08-01 02:52:42.000000 nligraphspacy-1.1.7/nligraphspacy/NLIGRAPH.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 02:52:42.000000 nligraphspacy-1.1.7/nligraphspacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:52:57.838519 nligraphspacy-1.1.7/nligraphspacy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-08-01 02:52:57.000000 nligraphspacy-1.1.7/nligraphspacy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-01 02:52:57.000000 nligraphspacy-1.1.7/nligraphspacy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 02:52:57.000000 nligraphspacy-1.1.7/nligraphspacy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 02:52:57.000000 nligraphspacy-1.1.7/nligraphspacy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-01 02:52:57.000000 nligraphspacy-1.1.7/nligraphspacy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-01 02:52:57.000000 nligraphspacy-1.1.7/nligraphspacy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 02:52:57.842520 nligraphspacy-1.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-08-01 02:52:42.000000 nligraphspacy-1.1.7/setup.py
```

### Comparing `nligraphspacy-1.1.6/LICENSE` & `nligraphspacy-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nligraphspacy-1.1.6/PKG-INFO` & `nligraphspacy-1.1.7/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nligraphspacy
-Version: 1.1.6
+Version: 1.1.7
 Summary: Knowledge graph using Spacy NLP
 Home-page: https://github.com/Vishnunkumar/nligraphspacy/
 Author: Vishnu Nandakumar
 Author-email: nkumarvishnu25@gmail.com
 License: MIT license
 Keywords: spacy nli keywords entities
 Classifier: Development Status :: 3 - Alpha
@@ -30,8 +30,17 @@
 ## Implementation
 
 ```python
 from nligraphspacy import NLIGRAPH
 nligraph = NLIGRAPH.RelationEntityExtract("She worked in the city of London")
 nligraph.process_text()
 # ('She', 'worked', 'London')
+
+nligraph.get_seperate_entities()
+# [{'text': 'A', 'label': ''},
+# {'text': 'DAG', 'label': 'SOURCE-NODE'},
+# {'text': 'is', 'label': ''},
+# {'text': 'used', 'label': 'EDGE'},
+# {'text': 'for', 'label': ''},
+# {'text': 'organizing', 'label': ''},
+# {'text': 'tasks', 'label': 'TARGET-NODE'}]
 ```
```

### Comparing `nligraphspacy-1.1.6/nligraphspacy/NLIGRAPH.py` & `nligraphspacy-1.1.7/nligraphspacy/NLIGRAPH.py`

 * *Files identical despite different names*

### Comparing `nligraphspacy-1.1.6/nligraphspacy.egg-info/PKG-INFO` & `nligraphspacy-1.1.7/nligraphspacy.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nligraphspacy
-Version: 1.1.6
+Version: 1.1.7
 Summary: Knowledge graph using Spacy NLP
 Home-page: https://github.com/Vishnunkumar/nligraphspacy/
 Author: Vishnu Nandakumar
 Author-email: nkumarvishnu25@gmail.com
 License: MIT license
 Keywords: spacy nli keywords entities
 Classifier: Development Status :: 3 - Alpha
@@ -30,8 +30,17 @@
 ## Implementation
 
 ```python
 from nligraphspacy import NLIGRAPH
 nligraph = NLIGRAPH.RelationEntityExtract("She worked in the city of London")
 nligraph.process_text()
 # ('She', 'worked', 'London')
+
+nligraph.get_seperate_entities()
+# [{'text': 'A', 'label': ''},
+# {'text': 'DAG', 'label': 'SOURCE-NODE'},
+# {'text': 'is', 'label': ''},
+# {'text': 'used', 'label': 'EDGE'},
+# {'text': 'for', 'label': ''},
+# {'text': 'organizing', 'label': ''},
+# {'text': 'tasks', 'label': 'TARGET-NODE'}]
 ```
```

### Comparing `nligraphspacy-1.1.6/setup.py` & `nligraphspacy-1.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,25 +6,25 @@
 requirements = [
     'spacy',
     'en-nligraphspacy'
 ]
 
 setuptools.setup(
     name="nligraphspacy",
-    version="1.1.6",
+    version="1.1.7",
     author="Vishnu Nandakumar",
     author_email="nkumarvishnu25@gmail.com",
     description="Knowledge graph using Spacy NLP",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url = 'https://github.com/Vishnunkumar/nligraphspacy/',
     packages=[
         'nligraphspacy',
     ],
-    package_dir={'nligraphspacy': 'nligraphspacy/'},
+    package_dir={'nligraphspacy': 'nligraphspacy'},
     package_data={
         'nligraphspacy': ['nligraphspacy/*']
     },
     install_requires=requirements,
     license="MIT license",
     zip_safe=False,
     keywords='spacy nli keywords entities',
```

