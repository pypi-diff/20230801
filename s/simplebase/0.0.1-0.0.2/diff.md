# Comparing `tmp/simplebase-0.0.1.tar.gz` & `tmp/simplebase-0.0.2.tar.gz`

## Comparing `simplebase-0.0.1.tar` & `simplebase-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simplebase-0.0.1/src/simplebase/__init__.py
--rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 simplebase-0.0.1/src/simplebase/simplebase.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 simplebase-0.0.1/tests/simplebase test.py
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 simplebase-0.0.1/LICENSE
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 simplebase-0.0.1/README.md
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 simplebase-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 simplebase-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simplebase-0.0.2/src/simplebase/__init__.py
+-rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 simplebase-0.0.2/src/simplebase/simplebase.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 simplebase-0.0.2/tests/simplebase test.py
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 simplebase-0.0.2/LICENSE
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 simplebase-0.0.2/README.md
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 simplebase-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 simplebase-0.0.2/PKG-INFO
```

### Comparing `simplebase-0.0.1/src/simplebase/simplebase.py` & `simplebase-0.0.2/src/simplebase/simplebase.py`

 * *Files identical despite different names*

### Comparing `simplebase-0.0.1/LICENSE` & `simplebase-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `simplebase-0.0.1/PKG-INFO` & `simplebase-0.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 Metadata-Version: 2.1
 Name: simplebase
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simple package for usage of Firebase for novice Python users
 Author-email: sneaky <24535asssci@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.1
+Requires-Dist: firebase-admin>=6.20
 Description-Content-Type: text/markdown
 
-Simplebase
+# Simplebase
 A simple Firebase wrapper for Python.
 It uses the firebase_admin package for requests to Firebase, and makes things WAY easier to use.
 
 To use the package, you must have Realtime Database and Storage enabled and a private key, stored in a JSON file.
 
 You can connect to Firebase like this:
-'connect("dbkey.json", "https://xxxxxxx-default-rtdb.firebaseio.com", "xxxxxxx.appspot.com")
+> connect("dbkey.json", "https://xxxxxxx-default-rtdb.firebaseio.com", "xxxxxxx.appspot.com")
 
 Go to a path:
-'refdb("/test/")'
+> refdb("/test/")
 
 Get from the path:
-'get()'
+> get()
 
 Add to / create a nested path with a value:
-'addToNest("/test/", "key", "value")'
+> addToNest("/test/", "key", "value")
 
 Add to a path with a value:
-'add("key", "value")'
+> add("key", "value")
 
 Delete a nested path:
-'deleteNest("/test/")'
+> deleteNest("/test/")
```

