# Comparing `tmp/seppmail_converter-1.1.0.tar.gz` & `tmp/seppmail_converter-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seppmail_converter-1.1.0.tar", max compression
+gzip compressed data, was "seppmail_converter-1.2.0.tar", max compression
```

## Comparing `seppmail_converter-1.1.0.tar` & `seppmail_converter-1.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    34523 2023-07-31 23:30:35.224490 seppmail_converter-1.1.0/LICENSE.md
--rw-r--r--   0        0        0     1322 2023-07-31 23:30:35.224490 seppmail_converter-1.1.0/README.md
--rw-r--r--   0        0        0      911 2023-07-31 23:31:11.733790 seppmail_converter-1.1.0/pyproject.toml
--rw-r--r--   0        0        0       22 2023-07-31 23:31:11.829793 seppmail_converter-1.1.0/seppmail_converter/__init__.py
--rw-r--r--   0        0        0      133 2023-07-31 23:30:35.224490 seppmail_converter-1.1.0/seppmail_converter/exceptions.py
--rw-r--r--   0        0        0     5394 2023-07-31 23:30:35.224490 seppmail_converter-1.1.0/seppmail_converter/main.py
--rw-r--r--   0        0        0     2155 1970-01-01 00:00:00.000000 seppmail_converter-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-07-31 23:38:46.006803 seppmail_converter-1.2.0/LICENSE.md
+-rw-r--r--   0        0        0     1322 2023-07-31 23:38:46.006803 seppmail_converter-1.2.0/README.md
+-rw-r--r--   0        0        0      928 2023-07-31 23:39:31.458599 seppmail_converter-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-07-31 23:39:31.578608 seppmail_converter-1.2.0/seppmail_converter/__init__.py
+-rw-r--r--   0        0        0      133 2023-07-31 23:38:46.006803 seppmail_converter-1.2.0/seppmail_converter/exceptions.py
+-rw-r--r--   0        0        0     5394 2023-07-31 23:38:46.006803 seppmail_converter-1.2.0/seppmail_converter/main.py
+-rw-r--r--   0        0        0     2155 1970-01-01 00:00:00.000000 seppmail_converter-1.2.0/PKG-INFO
```

### Comparing `seppmail_converter-1.1.0/LICENSE.md` & `seppmail_converter-1.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `seppmail_converter-1.1.0/README.md` & `seppmail_converter-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `seppmail_converter-1.1.0/pyproject.toml` & `seppmail_converter-1.2.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "seppmail-converter"
-version = "1.1.0"
+version = "1.2.0"
 description = "Decode SEPPMail emails into EML files"
 license = "AGPL-3.0-or-later"
 authors = ["Daniel Malik <daniel.malik@mhsp.solutions>"]
 readme = "README.md"
 classifiers = ["Environment :: Console"]
 repository = "https://github.com/mhsp/seppmail-converter"
 
@@ -16,22 +16,22 @@
 lxml = "^4.9.3"
 
 [tool.poetry.scripts]
 seppmail-converter = 'seppmail_converter.main:entry'
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^8.0.4"
+black = "^23.7.0"
 
 [tool.semantic_release]
 version.variable = [
     "seppmail_converter/__init__.py:__version__",
     "pyproject.toml:version",
 ]
 branch = "master"
 upload_to_pypi = true
 upload_to_release = true
 build_command = "poetry build"
 
-
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `seppmail_converter-1.1.0/seppmail_converter/main.py` & `seppmail_converter-1.2.0/seppmail_converter/main.py`

 * *Files identical despite different names*

### Comparing `seppmail_converter-1.1.0/PKG-INFO` & `seppmail_converter-1.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seppmail-converter
-Version: 1.1.0
+Version: 1.2.0
 Summary: Decode SEPPMail emails into EML files
 Home-page: https://github.com/mhsp/seppmail-converter
 License: AGPL-3.0-or-later
 Author: Daniel Malik
 Author-email: daniel.malik@mhsp.solutions
 Requires-Python: >=3.10,<4.0
 Classifier: Environment :: Console
```

