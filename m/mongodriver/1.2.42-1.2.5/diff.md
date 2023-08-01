# Comparing `tmp/mongodriver-1.2.42.tar.gz` & `tmp/mongodriver-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongodriver-1.2.42.tar", last modified: Tue Aug  1 11:36:50 2023, max compression
+gzip compressed data, was "mongodriver-1.2.5.tar", last modified: Tue Aug  1 11:43:25 2023, max compression
```

## Comparing `mongodriver-1.2.42.tar` & `mongodriver-1.2.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 jstrouse   (501) staff       (20)        0 2023-08-01 11:36:50.852436 mongodriver-1.2.42/
--rw-r--r--   0 jstrouse   (501) staff       (20)     1061 2022-08-27 03:52:41.000000 mongodriver-1.2.42/LICENSE
--rw-r--r--   0 jstrouse   (501) staff       (20)     3324 2023-08-01 11:36:50.852236 mongodriver-1.2.42/PKG-INFO
--rw-r--r--   0 jstrouse   (501) staff       (20)     2844 2023-07-20 15:38:01.000000 mongodriver-1.2.42/README.md
--rw-r--r--   0 jstrouse   (501) staff       (20)       80 2023-07-20 15:31:35.000000 mongodriver-1.2.42/pyproject.toml
--rw-r--r--   0 jstrouse   (501) staff       (20)       38 2023-08-01 11:36:50.852505 mongodriver-1.2.42/setup.cfg
--rw-r--r--   0 jstrouse   (501) staff       (20)      892 2023-08-01 11:36:41.000000 mongodriver-1.2.42/setup.py
-drwxr-xr-x   0 jstrouse   (501) staff       (20)        0 2023-08-01 11:36:50.849137 mongodriver-1.2.42/src/
-drwxr-xr-x   0 jstrouse   (501) staff       (20)        0 2023-08-01 11:36:50.850732 mongodriver-1.2.42/src/mongodriver/
--rw-r--r--   0 jstrouse   (501) staff       (20)        0 2023-08-01 11:20:05.000000 mongodriver-1.2.42/src/mongodriver/__init__.py
--rw-r--r--   0 jstrouse   (501) staff       (20)     7966 2023-08-01 11:21:58.000000 mongodriver-1.2.42/src/mongodriver/mongodriver.py
-drwxr-xr-x   0 jstrouse   (501) staff       (20)        0 2023-08-01 11:36:50.851934 mongodriver-1.2.42/src/mongodriver.egg-info/
--rw-r--r--   0 jstrouse   (501) staff       (20)     3324 2023-08-01 11:36:50.000000 mongodriver-1.2.42/src/mongodriver.egg-info/PKG-INFO
--rw-r--r--   0 jstrouse   (501) staff       (20)      294 2023-08-01 11:36:50.000000 mongodriver-1.2.42/src/mongodriver.egg-info/SOURCES.txt
--rw-r--r--   0 jstrouse   (501) staff       (20)        1 2023-08-01 11:36:50.000000 mongodriver-1.2.42/src/mongodriver.egg-info/dependency_links.txt
--rw-r--r--   0 jstrouse   (501) staff       (20)       29 2023-08-01 11:36:50.000000 mongodriver-1.2.42/src/mongodriver.egg-info/requires.txt
--rw-r--r--   0 jstrouse   (501) staff       (20)       12 2023-08-01 11:36:50.000000 mongodriver-1.2.42/src/mongodriver.egg-info/top_level.txt
+drwxr-xr-x   0 jstrouse   (501) staff       (20)        0 2023-08-01 11:43:25.429173 mongodriver-1.2.5/
+-rw-r--r--   0 jstrouse   (501) staff       (20)     1061 2022-08-27 03:52:41.000000 mongodriver-1.2.5/LICENSE
+-rw-r--r--   0 jstrouse   (501) staff       (20)     3323 2023-08-01 11:43:25.428990 mongodriver-1.2.5/PKG-INFO
+-rw-r--r--   0 jstrouse   (501) staff       (20)     2844 2023-07-20 15:38:01.000000 mongodriver-1.2.5/README.md
+-rw-r--r--   0 jstrouse   (501) staff       (20)       80 2023-07-20 15:31:35.000000 mongodriver-1.2.5/pyproject.toml
+-rw-r--r--   0 jstrouse   (501) staff       (20)       38 2023-08-01 11:43:25.429250 mongodriver-1.2.5/setup.cfg
+-rw-r--r--   0 jstrouse   (501) staff       (20)      891 2023-08-01 11:40:38.000000 mongodriver-1.2.5/setup.py
+drwxr-xr-x   0 jstrouse   (501) staff       (20)        0 2023-08-01 11:43:25.425322 mongodriver-1.2.5/src/
+drwxr-xr-x   0 jstrouse   (501) staff       (20)        0 2023-08-01 11:43:25.427186 mongodriver-1.2.5/src/mongodriver/
+-rw-r--r--   0 jstrouse   (501) staff       (20)       22 2023-08-01 11:40:38.000000 mongodriver-1.2.5/src/mongodriver/__init__.py
+-rw-r--r--   0 jstrouse   (501) staff       (20)     7955 2023-08-01 11:40:38.000000 mongodriver-1.2.5/src/mongodriver/mongodriver.py
+drwxr-xr-x   0 jstrouse   (501) staff       (20)        0 2023-08-01 11:43:25.428660 mongodriver-1.2.5/src/mongodriver.egg-info/
+-rw-r--r--   0 jstrouse   (501) staff       (20)     3323 2023-08-01 11:43:25.000000 mongodriver-1.2.5/src/mongodriver.egg-info/PKG-INFO
+-rw-r--r--   0 jstrouse   (501) staff       (20)      294 2023-08-01 11:43:25.000000 mongodriver-1.2.5/src/mongodriver.egg-info/SOURCES.txt
+-rw-r--r--   0 jstrouse   (501) staff       (20)        1 2023-08-01 11:43:25.000000 mongodriver-1.2.5/src/mongodriver.egg-info/dependency_links.txt
+-rw-r--r--   0 jstrouse   (501) staff       (20)       29 2023-08-01 11:43:25.000000 mongodriver-1.2.5/src/mongodriver.egg-info/requires.txt
+-rw-r--r--   0 jstrouse   (501) staff       (20)       12 2023-08-01 11:43:25.000000 mongodriver-1.2.5/src/mongodriver.egg-info/top_level.txt
```

### Comparing `mongodriver-1.2.42/LICENSE` & `mongodriver-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mongodriver-1.2.42/PKG-INFO` & `mongodriver-1.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongodriver
-Version: 1.2.42
+Version: 1.2.5
 Summary: Object-oriented interactions with MongoDB
 Home-page: https://github.com/jakestrouse00/mongodriver
 Author: Jake Strouse
 Author-email: jstrouse@meh.llc
 License: MIT
 Keywords: mongodb
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mongodriver-1.2.42/README.md` & `mongodriver-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `mongodriver-1.2.42/setup.py` & `mongodriver-1.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Get the long description from the README file
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='mongodriver',
-    version='1.2.42',
+    version='1.2.5',
     license='MIT',
     author="Jake Strouse",
     author_email='jstrouse@meh.llc',
     packages=find_packages('src'),
     url='https://github.com/jakestrouse00/mongodriver',
     package_dir={'': 'src'},
     keywords='mongodb',
```

### Comparing `mongodriver-1.2.42/src/mongodriver/mongodriver.py` & `mongodriver-1.2.5/src/mongodriver/mongodriver.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import pymongo
 from typing import Any, List, Union, Dict
 from dataclasses import dataclass, field
 from bson import ObjectId
 
-__version__ = "1.2.41"
 
 @dataclass
 class Document:
     _id: str = field(repr=True)
     variables: dict
     client: pymongo.collection.Collection = field(repr=False)
     _initialized: bool = field(repr=False, default=False)
@@ -113,15 +112,15 @@
     def create(self, data: dict) -> Document:
         """CREATE A DOCUMENT FROM A DICT AND RETURN THE Document OBJECT"""
         document = self.client.insert_one(data)
         python_document = Document(document.inserted_id, data, self.client)
         return python_document
 
     def update(
-        self, data: dict | Document, new_values: dict, sort: dict = None
+            self, data: dict | Document, new_values: dict, sort: dict = None
     ) -> Document:
         if "_id" in new_values.keys():
             new_values.pop("_id")
         if isinstance(data, Document):
             if sort is not None:
                 sort = sort.items()
             self.client.find_one_and_update(
@@ -164,28 +163,28 @@
             python_document = Document(str(doc_id), document, self.client)
             loaded_documents.append(python_document)
         return loaded_documents
 
     def find(self, search_terms: dict) -> List[Document]:
         """FIND A DOCUMENT AND RETURN IT AS A Document CLASS"""
         if "_id" in search_terms.keys() and not isinstance(
-            search_terms["_id"], ObjectId
+                search_terms["_id"], ObjectId
         ):
             search_terms["_id"] = ObjectId(search_terms["_id"])
         processed_documents = []
         documents = self.client.find(search_terms)
         for document in documents:
             doc_id = str(document["_id"])
             python_document = Document(doc_id, document, self.client)
             processed_documents.append(python_document)
         return processed_documents
 
     def find_one(self, search_terms: dict) -> Document | None:
         if "_id" in search_terms.keys() and not isinstance(
-            search_terms["_id"], ObjectId
+                search_terms["_id"], ObjectId
         ):
             search_terms["_id"] = ObjectId(search_terms["_id"])
         document = self.client.find_one(search_terms)
         if document is None:
             return None
         doc_id = str(document["_id"])
         python_document = Document(doc_id, document, self.client)
```

### Comparing `mongodriver-1.2.42/src/mongodriver.egg-info/PKG-INFO` & `mongodriver-1.2.5/src/mongodriver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongodriver
-Version: 1.2.42
+Version: 1.2.5
 Summary: Object-oriented interactions with MongoDB
 Home-page: https://github.com/jakestrouse00/mongodriver
 Author: Jake Strouse
 Author-email: jstrouse@meh.llc
 License: MIT
 Keywords: mongodb
 Classifier: Programming Language :: Python :: 3
```

