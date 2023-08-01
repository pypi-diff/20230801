# Comparing `tmp/mongoy-0.1.3.tar.gz` & `tmp/mongoy-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongoy-0.1.3.tar", last modified: Tue Jul 25 16:44:54 2023, max compression
+gzip compressed data, was "mongoy-0.1.4.tar", last modified: Tue Aug  1 09:36:04 2023, max compression
```

## Comparing `mongoy-0.1.3.tar` & `mongoy-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 16:44:54.285753 mongoy-0.1.3/
--rw-rw-rw-   0        0        0     1067 2023-07-25 16:42:49.000000 mongoy-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     2052 2023-07-25 16:44:54.285753 mongoy-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1701 2023-07-25 16:42:49.000000 mongoy-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 16:44:54.261745 mongoy-0.1.3/mongoy/
--rw-rw-rw-   0        0        0        0 2023-07-25 16:43:10.000000 mongoy-0.1.3/mongoy/__init__.py
--rw-rw-rw-   0        0        0     4084 2023-07-25 16:42:49.000000 mongoy-0.1.3/mongoy/mongo.py
-drwxrwxrwx   0        0        0        0 2023-07-25 16:44:54.277749 mongoy-0.1.3/mongoy.egg-info/
--rw-rw-rw-   0        0        0     2052 2023-07-25 16:44:53.000000 mongoy-0.1.3/mongoy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2023-07-25 16:44:54.000000 mongoy-0.1.3/mongoy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 16:44:53.000000 mongoy-0.1.3/mongoy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-25 16:44:53.000000 mongoy-0.1.3/mongoy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-25 16:44:53.000000 mongoy-0.1.3/mongoy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-25 16:44:54.285753 mongoy-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1212 2023-07-25 16:44:48.000000 mongoy-0.1.3/setup.py
+drwxr-xr-x   0 jarmanrandhawa   (501) staff       (20)        0 2023-08-01 09:36:04.758758 mongoy-0.1.4/
+-rw-r--r--   0 jarmanrandhawa   (501) staff       (20)     1061 2023-07-18 15:58:12.000000 mongoy-0.1.4/LICENSE
+-rw-r--r--   0 jarmanrandhawa   (501) staff       (20)     1939 2023-08-01 09:36:04.758633 mongoy-0.1.4/PKG-INFO
+-rw-r--r--   0 jarmanrandhawa   (501) staff       (20)     1601 2023-07-19 08:24:07.000000 mongoy-0.1.4/README.md
+drwxr-xr-x   0 jarmanrandhawa   (501) staff       (20)        0 2023-08-01 09:36:04.757276 mongoy-0.1.4/mongoy/
+drwxr-xr-x   0 jarmanrandhawa   (501) staff       (20)        0 2023-08-01 09:36:04.758461 mongoy-0.1.4/mongoy/mongoy.egg-info/
+-rw-r--r--   0 jarmanrandhawa   (501) staff       (20)     1939 2023-08-01 09:36:04.000000 mongoy-0.1.4/mongoy/mongoy.egg-info/PKG-INFO
+-rw-r--r--   0 jarmanrandhawa   (501) staff       (20)      210 2023-08-01 09:36:04.000000 mongoy-0.1.4/mongoy/mongoy.egg-info/SOURCES.txt
+-rw-r--r--   0 jarmanrandhawa   (501) staff       (20)        1 2023-08-01 09:36:04.000000 mongoy-0.1.4/mongoy/mongoy.egg-info/dependency_links.txt
+-rw-r--r--   0 jarmanrandhawa   (501) staff       (20)       16 2023-08-01 09:36:04.000000 mongoy-0.1.4/mongoy/mongoy.egg-info/requires.txt
+-rw-r--r--   0 jarmanrandhawa   (501) staff       (20)        7 2023-08-01 09:36:04.000000 mongoy-0.1.4/mongoy/mongoy.egg-info/top_level.txt
+-rw-r--r--   0 jarmanrandhawa   (501) staff       (20)       38 2023-08-01 09:36:04.758793 mongoy-0.1.4/setup.cfg
+-rw-r--r--   0 jarmanrandhawa   (501) staff       (20)     1199 2023-08-01 09:36:00.000000 mongoy-0.1.4/setup.py
```

### Comparing `mongoy-0.1.3/LICENSE` & `mongoy-0.1.4/LICENSE`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright 2023 Pavittar Singh
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
+Copyright 2023 Pavittar Singh
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `mongoy-0.1.3/PKG-INFO` & `mongoy-0.1.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,113 +1,113 @@
-Metadata-Version: 2.1
-Name: mongoy
-Version: 0.1.3
-Summary: wrapper utility for mongodb
-Author: pavittarx
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-A wrapper library on top of pymongo.
-
-```shell
-  pip install mongoy
-```
-
-## Connecting to Database
-
-```python
-   from mongoy.mongo import Mongo
-
-   connection = 'mongodb://127.0.0.1:27017'
-   db_name = 'mydb''
-
-   mgy = Mongo(connection, db_name)
-```
-
-
-### Get `pymongo` db instance
-```python
-  # get pymongo db instance
-  db = mgy.get_db()
-```
-
-### Register a collection for operations
-
-```python
-   # Register a collection for CRUD data ops
-
-   mgy.register_collection('users')
-```
-
-```python
-  # Add a document
-  doc = {
-    'name': 'test',
-    'age': 10,
-  }
-
-  result = mgy.users.insert(doc)
-
-
-  # Add multiple documents
-  docs = [{
-    'name': 'testuser',
-    'age': 21
-  }, {
-    'name': 'testy',
-    'age': 22
-  }, {
-    'name': 'uwoo',
-    'age': 27
-  }]
-
-  result = mgy.users.insert(docs)
-```
-
-```python
-  # Find Documents
-
-  result = mgy.users.find()
-
-  age_22_users = mgy.users.find({
-    'age': 22
-  })
-
-  others = mgy.users.find({
-    'age': {'$ne': 22}
-  })
-
-  mgy.users.find({
-    '_id': result[0]['_id']
-  })
-```
-
-```python
-  from bson.objectid import ObjectId
-  id = ObjectId('some-mongo-id')
-
-  # Update single document 
-  mgy.users.find_one_and_update({'_id': id}, {'$set': {'age': 30}})
-
-  # Update all matching documents
-  mgy.users.find_all_and_update({'age': {'$lt': 25}}, {'$set': {'age': 30}})
-
-  # Insert if not exists 
-  mgy.users.find_one_and_update({'_id': id}, {'$set': {'age': 30}}, upsert=True)
-```
-
-```python
-  # Delete Single Documents
-  mgy.users.delete({
-    'age': 22
-  })
-
-   # Delete all matching Documents
-  mgy.users.delete({
-    'age': 22
-  }, all=True)
-
-```
+Metadata-Version: 2.1
+Name: mongoy
+Version: 0.1.4
+Summary: wrapper utility for mongodb
+Author: pavittarx
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+A wrapper library on top of pymongo.
+
+```shell
+  pip install mongoy
+```
+
+## Connecting to Database
+
+```python
+   from mongoy.mongo import Mongo
+
+   connection = 'mongodb://127.0.0.1:27017'
+   db_name = 'mydb''
+
+   mgy = Mongo(connection, db_name)
+```
+
+
+### Get `pymongo` db instance
+```python
+  # get pymongo db instance
+  db = mgy.get_db()
+```
+
+### Register a collection for operations
+
+```python
+   # Register a collection for CRUD data ops
+
+   mgy.register_collection('users')
+```
+
+```python
+  # Add a document
+  doc = {
+    'name': 'test',
+    'age': 10,
+  }
+
+  result = mgy.users.insert(doc)
+
+
+  # Add multiple documents
+  docs = [{
+    'name': 'testuser',
+    'age': 21
+  }, {
+    'name': 'testy',
+    'age': 22
+  }, {
+    'name': 'uwoo',
+    'age': 27
+  }]
+
+  result = mgy.users.insert(docs)
+```
+
+```python
+  # Find Documents
+
+  result = mgy.users.find()
+
+  age_22_users = mgy.users.find({
+    'age': 22
+  })
+
+  others = mgy.users.find({
+    'age': {'$ne': 22}
+  })
+
+  mgy.users.find({
+    '_id': result[0]['_id']
+  })
+```
+
+```python
+  from bson.objectid import ObjectId
+  id = ObjectId('some-mongo-id')
+
+  # Update single document 
+  mgy.users.find_one_and_update({'_id': id}, {'$set': {'age': 30}})
+
+  # Update all matching documents
+  mgy.users.find_all_and_update({'age': {'$lt': 25}}, {'$set': {'age': 30}})
+
+  # Insert if not exists 
+  mgy.users.find_one_and_update({'_id': id}, {'$set': {'age': 30}}, upsert=True)
+```
+
+```python
+  # Delete Single Documents
+  mgy.users.delete({
+    'age': 22
+  })
+
+   # Delete all matching Documents
+  mgy.users.delete({
+    'age': 22
+  }, all=True)
+
+```
```

### Comparing `mongoy-0.1.3/README.md` & `mongoy-0.1.4/README.md`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,101 +1,101 @@
-A wrapper library on top of pymongo.
-
-```shell
-  pip install mongoy
-```
-
-## Connecting to Database
-
-```python
-   from mongoy.mongo import Mongo
-
-   connection = 'mongodb://127.0.0.1:27017'
-   db_name = 'mydb''
-
-   mgy = Mongo(connection, db_name)
-```
-
-
-### Get `pymongo` db instance
-```python
-  # get pymongo db instance
-  db = mgy.get_db()
-```
-
-### Register a collection for operations
-
-```python
-   # Register a collection for CRUD data ops
-
-   mgy.register_collection('users')
-```
-
-```python
-  # Add a document
-  doc = {
-    'name': 'test',
-    'age': 10,
-  }
-
-  result = mgy.users.insert(doc)
-
-
-  # Add multiple documents
-  docs = [{
-    'name': 'testuser',
-    'age': 21
-  }, {
-    'name': 'testy',
-    'age': 22
-  }, {
-    'name': 'uwoo',
-    'age': 27
-  }]
-
-  result = mgy.users.insert(docs)
-```
-
-```python
-  # Find Documents
-
-  result = mgy.users.find()
-
-  age_22_users = mgy.users.find({
-    'age': 22
-  })
-
-  others = mgy.users.find({
-    'age': {'$ne': 22}
-  })
-
-  mgy.users.find({
-    '_id': result[0]['_id']
-  })
-```
-
-```python
-  from bson.objectid import ObjectId
-  id = ObjectId('some-mongo-id')
-
-  # Update single document 
-  mgy.users.find_one_and_update({'_id': id}, {'$set': {'age': 30}})
-
-  # Update all matching documents
-  mgy.users.find_all_and_update({'age': {'$lt': 25}}, {'$set': {'age': 30}})
-
-  # Insert if not exists 
-  mgy.users.find_one_and_update({'_id': id}, {'$set': {'age': 30}}, upsert=True)
-```
-
-```python
-  # Delete Single Documents
-  mgy.users.delete({
-    'age': 22
-  })
-
-   # Delete all matching Documents
-  mgy.users.delete({
-    'age': 22
-  }, all=True)
-
+A wrapper library on top of pymongo.
+
+```shell
+  pip install mongoy
+```
+
+## Connecting to Database
+
+```python
+   from mongoy.mongo import Mongo
+
+   connection = 'mongodb://127.0.0.1:27017'
+   db_name = 'mydb''
+
+   mgy = Mongo(connection, db_name)
+```
+
+
+### Get `pymongo` db instance
+```python
+  # get pymongo db instance
+  db = mgy.get_db()
+```
+
+### Register a collection for operations
+
+```python
+   # Register a collection for CRUD data ops
+
+   mgy.register_collection('users')
+```
+
+```python
+  # Add a document
+  doc = {
+    'name': 'test',
+    'age': 10,
+  }
+
+  result = mgy.users.insert(doc)
+
+
+  # Add multiple documents
+  docs = [{
+    'name': 'testuser',
+    'age': 21
+  }, {
+    'name': 'testy',
+    'age': 22
+  }, {
+    'name': 'uwoo',
+    'age': 27
+  }]
+
+  result = mgy.users.insert(docs)
+```
+
+```python
+  # Find Documents
+
+  result = mgy.users.find()
+
+  age_22_users = mgy.users.find({
+    'age': 22
+  })
+
+  others = mgy.users.find({
+    'age': {'$ne': 22}
+  })
+
+  mgy.users.find({
+    '_id': result[0]['_id']
+  })
+```
+
+```python
+  from bson.objectid import ObjectId
+  id = ObjectId('some-mongo-id')
+
+  # Update single document 
+  mgy.users.find_one_and_update({'_id': id}, {'$set': {'age': 30}})
+
+  # Update all matching documents
+  mgy.users.find_all_and_update({'age': {'$lt': 25}}, {'$set': {'age': 30}})
+
+  # Insert if not exists 
+  mgy.users.find_one_and_update({'_id': id}, {'$set': {'age': 30}}, upsert=True)
+```
+
+```python
+  # Delete Single Documents
+  mgy.users.delete({
+    'age': 22
+  })
+
+   # Delete all matching Documents
+  mgy.users.delete({
+    'age': 22
+  }, all=True)
+
 ```
```

### Comparing `mongoy-0.1.3/mongoy.egg-info/PKG-INFO` & `mongoy-0.1.4/mongoy/mongoy.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,113 +1,113 @@
-Metadata-Version: 2.1
-Name: mongoy
-Version: 0.1.3
-Summary: wrapper utility for mongodb
-Author: pavittarx
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-A wrapper library on top of pymongo.
-
-```shell
-  pip install mongoy
-```
-
-## Connecting to Database
-
-```python
-   from mongoy.mongo import Mongo
-
-   connection = 'mongodb://127.0.0.1:27017'
-   db_name = 'mydb''
-
-   mgy = Mongo(connection, db_name)
-```
-
-
-### Get `pymongo` db instance
-```python
-  # get pymongo db instance
-  db = mgy.get_db()
-```
-
-### Register a collection for operations
-
-```python
-   # Register a collection for CRUD data ops
-
-   mgy.register_collection('users')
-```
-
-```python
-  # Add a document
-  doc = {
-    'name': 'test',
-    'age': 10,
-  }
-
-  result = mgy.users.insert(doc)
-
-
-  # Add multiple documents
-  docs = [{
-    'name': 'testuser',
-    'age': 21
-  }, {
-    'name': 'testy',
-    'age': 22
-  }, {
-    'name': 'uwoo',
-    'age': 27
-  }]
-
-  result = mgy.users.insert(docs)
-```
-
-```python
-  # Find Documents
-
-  result = mgy.users.find()
-
-  age_22_users = mgy.users.find({
-    'age': 22
-  })
-
-  others = mgy.users.find({
-    'age': {'$ne': 22}
-  })
-
-  mgy.users.find({
-    '_id': result[0]['_id']
-  })
-```
-
-```python
-  from bson.objectid import ObjectId
-  id = ObjectId('some-mongo-id')
-
-  # Update single document 
-  mgy.users.find_one_and_update({'_id': id}, {'$set': {'age': 30}})
-
-  # Update all matching documents
-  mgy.users.find_all_and_update({'age': {'$lt': 25}}, {'$set': {'age': 30}})
-
-  # Insert if not exists 
-  mgy.users.find_one_and_update({'_id': id}, {'$set': {'age': 30}}, upsert=True)
-```
-
-```python
-  # Delete Single Documents
-  mgy.users.delete({
-    'age': 22
-  })
-
-   # Delete all matching Documents
-  mgy.users.delete({
-    'age': 22
-  }, all=True)
-
-```
+Metadata-Version: 2.1
+Name: mongoy
+Version: 0.1.4
+Summary: wrapper utility for mongodb
+Author: pavittarx
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+A wrapper library on top of pymongo.
+
+```shell
+  pip install mongoy
+```
+
+## Connecting to Database
+
+```python
+   from mongoy.mongo import Mongo
+
+   connection = 'mongodb://127.0.0.1:27017'
+   db_name = 'mydb''
+
+   mgy = Mongo(connection, db_name)
+```
+
+
+### Get `pymongo` db instance
+```python
+  # get pymongo db instance
+  db = mgy.get_db()
+```
+
+### Register a collection for operations
+
+```python
+   # Register a collection for CRUD data ops
+
+   mgy.register_collection('users')
+```
+
+```python
+  # Add a document
+  doc = {
+    'name': 'test',
+    'age': 10,
+  }
+
+  result = mgy.users.insert(doc)
+
+
+  # Add multiple documents
+  docs = [{
+    'name': 'testuser',
+    'age': 21
+  }, {
+    'name': 'testy',
+    'age': 22
+  }, {
+    'name': 'uwoo',
+    'age': 27
+  }]
+
+  result = mgy.users.insert(docs)
+```
+
+```python
+  # Find Documents
+
+  result = mgy.users.find()
+
+  age_22_users = mgy.users.find({
+    'age': 22
+  })
+
+  others = mgy.users.find({
+    'age': {'$ne': 22}
+  })
+
+  mgy.users.find({
+    '_id': result[0]['_id']
+  })
+```
+
+```python
+  from bson.objectid import ObjectId
+  id = ObjectId('some-mongo-id')
+
+  # Update single document 
+  mgy.users.find_one_and_update({'_id': id}, {'$set': {'age': 30}})
+
+  # Update all matching documents
+  mgy.users.find_all_and_update({'age': {'$lt': 25}}, {'$set': {'age': 30}})
+
+  # Insert if not exists 
+  mgy.users.find_one_and_update({'_id': id}, {'$set': {'age': 30}}, upsert=True)
+```
+
+```python
+  # Delete Single Documents
+  mgy.users.delete({
+    'age': 22
+  })
+
+   # Delete all matching Documents
+  mgy.users.delete({
+    'age': 22
+  }, all=True)
+
+```
```

### Comparing `mongoy-0.1.3/setup.py` & `mongoy-0.1.4/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-import setuptools
-
-with open("README.md", "r") as fh:
-    long_description = fh.read()
-
-setuptools.setup(
-    name="mongoy",                     # This is the name of the package
-    version="0.1.3",                        # The initial release version
-    author="pavittarx",                     # Full name of the author
-    description="wrapper utility for mongodb",
-    long_description=long_description,      # Long description read from the the readme file
-    long_description_content_type="text/markdown",
-    packages=setuptools.find_packages(),    # List of all python modules to be installed
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-    ],                                      # Information to filter the project on PyPi website
-    python_requires='>=3.6',                # Minimum version requirement of the package
-    py_modules=["mongoy"],             # Name of the python package
-    # package_dir={'':'mongoy'},     # Directory of the source code of the package
-    install_requires=["pymongo"]                     # Install other dependencies if any
+import setuptools
+
+with open("README.md", "r") as fh:
+    long_description = fh.read()
+
+setuptools.setup(
+    name="mongoy",                     # This is the name of the package
+    version="0.1.4",                        # The initial release version
+    author="pavittarx",                     # Full name of the author
+    description="wrapper utility for mongodb",
+    long_description=long_description,      # Long description read from the the readme file
+    long_description_content_type="text/markdown",
+    packages=setuptools.find_packages(),    # List of all python modules to be installed
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+    ],                                      # Information to filter the project on PyPi website
+    python_requires='>=3.6',                # Minimum version requirement of the package
+    py_modules=["mongoy"],             # Name of the python package
+    package_dir={'':'mongoy'},     # Directory of the source code of the package
+    install_requires=["pymongo", "certifi"]                     # Install other dependencies if any
 )
```

