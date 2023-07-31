# Comparing `tmp/seppmail_converter-1.0.3.tar.gz` & `tmp/seppmail_converter-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seppmail_converter-1.0.3.tar", max compression
+gzip compressed data, was "seppmail_converter-1.1.0.tar", max compression
```

## Comparing `seppmail_converter-1.0.3.tar` & `seppmail_converter-1.1.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    34523 2023-07-28 11:46:34.408306 seppmail_converter-1.0.3/LICENSE.md
--rw-r--r--   0        0        0     1061 2023-07-28 11:46:34.408306 seppmail_converter-1.0.3/README.md
--rw-r--r--   0        0        0      911 2023-07-28 11:47:10.143686 seppmail_converter-1.0.3/pyproject.toml
--rw-r--r--   0        0        0       22 2023-07-28 11:47:10.247696 seppmail_converter-1.0.3/seppmail_converter/__init__.py
--rw-r--r--   0        0        0      133 2023-07-28 11:46:34.408306 seppmail_converter-1.0.3/seppmail_converter/exceptions.py
--rw-r--r--   0        0        0     5394 2023-07-28 11:46:34.408306 seppmail_converter-1.0.3/seppmail_converter/main.py
--rw-r--r--   0        0        0     1894 1970-01-01 00:00:00.000000 seppmail_converter-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-07-31 23:30:35.224490 seppmail_converter-1.1.0/LICENSE.md
+-rw-r--r--   0        0        0     1322 2023-07-31 23:30:35.224490 seppmail_converter-1.1.0/README.md
+-rw-r--r--   0        0        0      911 2023-07-31 23:31:11.733790 seppmail_converter-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-07-31 23:31:11.829793 seppmail_converter-1.1.0/seppmail_converter/__init__.py
+-rw-r--r--   0        0        0      133 2023-07-31 23:30:35.224490 seppmail_converter-1.1.0/seppmail_converter/exceptions.py
+-rw-r--r--   0        0        0     5394 2023-07-31 23:30:35.224490 seppmail_converter-1.1.0/seppmail_converter/main.py
+-rw-r--r--   0        0        0     2155 1970-01-01 00:00:00.000000 seppmail_converter-1.1.0/PKG-INFO
```

### Comparing `seppmail_converter-1.0.3/LICENSE.md` & `seppmail_converter-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `seppmail_converter-1.0.3/README.md` & `seppmail_converter-1.1.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 # SEPPMail Converter
+![PyPI](https://img.shields.io/pypi/v/seppmail-converter)
+![GitHub Workflow Status (with event)](https://img.shields.io/github/actions/workflow/status/mhsp/seppmail-converter/release.yml)
+![GitHub](https://img.shields.io/github/license/mhsp/seppmail-converter)
 
 This python tool allows you to convert [SEPPMail](https://www.seppmail.com/) encrypted email files (`html`) to `.eml` files.
 
 ## Usage
 
 ```
 Usage: seppmail-converter [OPTIONS] INPUT_FILE
```

### Comparing `seppmail_converter-1.0.3/pyproject.toml` & `seppmail_converter-1.1.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "seppmail-converter"
-version = "1.0.3"
+version = "1.1.0"
 description = "Decode SEPPMail emails into EML files"
 license = "AGPL-3.0-or-later"
 authors = ["Daniel Malik <daniel.malik@mhsp.solutions>"]
 readme = "README.md"
 classifiers = ["Environment :: Console"]
 repository = "https://github.com/mhsp/seppmail-converter"
```

### Comparing `seppmail_converter-1.0.3/seppmail_converter/main.py` & `seppmail_converter-1.1.0/seppmail_converter/main.py`

 * *Files identical despite different names*

### Comparing `seppmail_converter-1.0.3/PKG-INFO` & `seppmail_converter-1.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seppmail-converter
-Version: 1.0.3
+Version: 1.1.0
 Summary: Decode SEPPMail emails into EML files
 Home-page: https://github.com/mhsp/seppmail-converter
 License: AGPL-3.0-or-later
 Author: Daniel Malik
 Author-email: daniel.malik@mhsp.solutions
 Requires-Python: >=3.10,<4.0
 Classifier: Environment :: Console
@@ -16,14 +16,17 @@
 Requires-Dist: click (>=8.1.6,<9.0.0)
 Requires-Dist: lxml (>=4.9.3,<5.0.0)
 Requires-Dist: requests (>=2.31,<3.0)
 Project-URL: Repository, https://github.com/mhsp/seppmail-converter
 Description-Content-Type: text/markdown
 
 # SEPPMail Converter
+![PyPI](https://img.shields.io/pypi/v/seppmail-converter)
+![GitHub Workflow Status (with event)](https://img.shields.io/github/actions/workflow/status/mhsp/seppmail-converter/release.yml)
+![GitHub](https://img.shields.io/github/license/mhsp/seppmail-converter)
 
 This python tool allows you to convert [SEPPMail](https://www.seppmail.com/) encrypted email files (`html`) to `.eml` files.
 
 ## Usage
 
 ```
 Usage: seppmail-converter [OPTIONS] INPUT_FILE
```

