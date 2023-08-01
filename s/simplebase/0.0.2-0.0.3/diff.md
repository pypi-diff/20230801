# Comparing `tmp/simplebase-0.0.2.tar.gz` & `tmp/simplebase-0.0.3.tar.gz`

## Comparing `simplebase-0.0.2.tar` & `simplebase-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simplebase-0.0.2/src/simplebase/__init__.py
--rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 simplebase-0.0.2/src/simplebase/simplebase.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 simplebase-0.0.2/tests/simplebase test.py
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 simplebase-0.0.2/LICENSE
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 simplebase-0.0.2/README.md
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 simplebase-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 simplebase-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simplebase-0.0.3/src/simplebase/__init__.py
+-rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 simplebase-0.0.3/src/simplebase/simplebase.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 simplebase-0.0.3/tests/simplebase test.py
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 simplebase-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 simplebase-0.0.3/README.md
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 simplebase-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 simplebase-0.0.3/PKG-INFO
```

### Comparing `simplebase-0.0.2/LICENSE` & `simplebase-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `simplebase-0.0.2/pyproject.toml` & `simplebase-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "simplebase"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
    { name="sneaky", email="24535asssci@gmail.com" },
 ]
 description = "A simple package for usage of Firebase for novice Python users"
 readme = "README.md"
 requires-python = ">=3.1"
 dependencies = [
```

