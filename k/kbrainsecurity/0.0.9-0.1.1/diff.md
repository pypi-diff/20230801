# Comparing `tmp/kbrainsecurity-0.0.9.tar.gz` & `tmp/kbrainsecurity-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kbrainsecurity-0.0.9.tar", max compression
+gzip compressed data, was "kbrainsecurity-0.1.1.tar", max compression
```

## Comparing `kbrainsecurity-0.0.9.tar` & `kbrainsecurity-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    34353 2023-06-24 14:13:14.234140 kbrainsecurity-0.0.9/LICENSE.md
--rw-r--r--   0        0        0      982 2023-06-24 14:13:14.234140 kbrainsecurity-0.0.9/README.md
--rw-r--r--   0        0        0      640 2023-06-24 14:14:05.559002 kbrainsecurity-0.0.9/pyproject.toml
--rw-r--r--   0        0        0     1358 2023-06-24 14:13:14.234140 kbrainsecurity-0.0.9/src/authentication/azure_authentication.py
--rw-r--r--   0        0        0     1336 2023-06-24 14:13:14.234140 kbrainsecurity-0.0.9/src/authentication/bearer.py
--rw-r--r--   0        0        0     1556 1970-01-01 00:00:00.000000 kbrainsecurity-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0    34353 2023-08-01 03:25:52.729279 kbrainsecurity-0.1.1/LICENSE.md
+-rw-r--r--   0        0        0      982 2023-08-01 03:25:52.729279 kbrainsecurity-0.1.1/README.md
+-rw-r--r--   0        0        0      655 2023-08-01 03:26:38.677915 kbrainsecurity-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1318 2023-08-01 03:25:52.733279 kbrainsecurity-0.1.1/src/kbrainsecurity/azure_authentication.py
+-rw-r--r--   0        0        0     1336 2023-08-01 03:25:52.733279 kbrainsecurity-0.1.1/src/kbrainsecurity/bearer.py
+-rw-r--r--   0        0        0     1556 1970-01-01 00:00:00.000000 kbrainsecurity-0.1.1/PKG-INFO
```

### Comparing `kbrainsecurity-0.0.9/LICENSE.md` & `kbrainsecurity-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `kbrainsecurity-0.0.9/README.md` & `kbrainsecurity-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `kbrainsecurity-0.0.9/pyproject.toml` & `kbrainsecurity-0.1.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [tool.poetry]
 name = "kbrainsecurity"
-version = "0.0.9"
+version = "0.1.1"
 description = "Security and authentication functions for use in KBRAIN"
 authors = ["Daniel E. Fredriksen <daniel.fredriksen@us.kbr.com>"]
 license = "AGPLv3"
 readme = "README.md"
-packages = [{include = "authentication", from="src"}]
+packages = [{include = "kbrainsecurity", from="src"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 python-jose = "^3.3.0"
 azure-functions = "^1.15.0"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
 pre-commit = "^3.3.3"
 pytest-cov = "^4.1.0"
 
 [tool.pytest.ini.options]
-pythonpath = ["src"]
+pythonpath = ["src/kbrainsecurity"]
 testpaths = ["tests"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `kbrainsecurity-0.0.9/src/authentication/bearer.py` & `kbrainsecurity-0.1.1/src/kbrainsecurity/bearer.py`

 * *Files identical despite different names*

### Comparing `kbrainsecurity-0.0.9/PKG-INFO` & `kbrainsecurity-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kbrainsecurity
-Version: 0.0.9
+Version: 0.1.1
 Summary: Security and authentication functions for use in KBRAIN
 License: AGPLv3
 Author: Daniel E. Fredriksen
 Author-email: daniel.fredriksen@us.kbr.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

