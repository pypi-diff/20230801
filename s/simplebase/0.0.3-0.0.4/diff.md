# Comparing `tmp/simplebase-0.0.3.tar.gz` & `tmp/simplebase-0.0.4.tar.gz`

## Comparing `simplebase-0.0.3.tar` & `simplebase-0.0.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simplebase-0.0.3/src/simplebase/__init__.py
--rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 simplebase-0.0.3/src/simplebase/simplebase.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 simplebase-0.0.3/tests/simplebase test.py
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 simplebase-0.0.3/LICENSE
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 simplebase-0.0.3/README.md
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 simplebase-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 simplebase-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simplebase-0.0.4/src/simplebase/__init__.py
+-rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 simplebase-0.0.4/src/simplebase/simplebase.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 simplebase-0.0.4/tests/simplebase test.py
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 simplebase-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 simplebase-0.0.4/README.md
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 simplebase-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 simplebase-0.0.4/PKG-INFO
```

### Comparing `simplebase-0.0.3/src/simplebase/simplebase.py` & `simplebase-0.0.4/src/simplebase/simplebase.py`

 * *Files identical despite different names*

### Comparing `simplebase-0.0.3/LICENSE` & `simplebase-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `simplebase-0.0.3/README.md` & `simplebase-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `simplebase-0.0.3/pyproject.toml` & `simplebase-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "simplebase"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
    { name="sneaky", email="24535asssci@gmail.com" },
 ]
 description = "A simple package for usage of Firebase for novice Python users"
 readme = "README.md"
 requires-python = ">=3.1"
 dependencies = [
-    "firebase-admin >= 6.20"
+    "firebase-admin >= 6.2.0"
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `simplebase-0.0.3/PKG-INFO` & `simplebase-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: simplebase
-Version: 0.0.3
+Version: 0.0.4
 Summary: A simple package for usage of Firebase for novice Python users
 Author-email: sneaky <24535asssci@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.1
-Requires-Dist: firebase-admin>=6.20
+Requires-Dist: firebase-admin>=6.2.0
 Description-Content-Type: text/markdown
 
 # Simplebase
 A simple Firebase wrapper for Python.
 It uses the firebase_admin package for requests to Firebase, and makes things WAY easier to use.
 
 To use the package, you must have Realtime Database and Storage enabled and a private key, stored in a JSON file.
```

