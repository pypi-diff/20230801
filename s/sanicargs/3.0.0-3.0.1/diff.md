# Comparing `tmp/sanicargs-3.0.0.tar.gz` & `tmp/sanicargs-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sanicargs-3.0.0.tar", max compression
+gzip compressed data, was "sanicargs-3.0.1.tar", max compression
```

## Comparing `sanicargs-3.0.0.tar` & `sanicargs-3.0.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1049 2023-08-01 12:50:39.785228 sanicargs-3.0.0/LICENSE
--rw-r--r--   0        0        0     2922 2023-08-01 14:45:23.859602 sanicargs-3.0.0/README.md
--rw-r--r--   0        0        0     1008 2023-08-01 14:45:23.865739 sanicargs-3.0.0/pyproject.toml
--rw-r--r--   0        0        0     3594 2023-08-01 14:45:23.868646 sanicargs-3.0.0/sanicargs/__init__.py
--rw-r--r--   0        0        0       24 2023-08-01 12:50:39.787169 sanicargs-3.0.0/sanicargs/fields.py
--rw-r--r--   0        0        0     3837 1970-01-01 00:00:00.000000 sanicargs-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1049 2023-08-01 12:50:39.785228 sanicargs-3.0.1/LICENSE
+-rw-r--r--   0        0        0     2962 2023-08-01 14:49:21.527517 sanicargs-3.0.1/README.md
+-rw-r--r--   0        0        0     1008 2023-08-01 14:50:16.392733 sanicargs-3.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3594 2023-08-01 14:45:23.868646 sanicargs-3.0.1/sanicargs/__init__.py
+-rw-r--r--   0        0        0       24 2023-08-01 12:50:39.787169 sanicargs-3.0.1/sanicargs/fields.py
+-rw-r--r--   0        0        0     3877 1970-01-01 00:00:00.000000 sanicargs-3.0.1/PKG-INFO
```

### Comparing `sanicargs-3.0.0/LICENSE` & `sanicargs-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sanicargs-3.0.0/README.md` & `sanicargs-3.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![Build Status](https://travis-ci.org/trustpilot/python-sanicargs.svg?branch=master)](https://travis-ci.org/trustpilot/python-sanicargs) [![Latest Version](https://img.shields.io/pypi/v/sanicargs.svg)](https://pypi.python.org/pypi/sanicargs) [![Python Support](https://img.shields.io/pypi/pyversions/sanicargs.svg)](https://pypi.python.org/pypi/sanicargs)
+[![Build Status](https://github.com/trustpilot/python-sanicargs/actions/workflows/tox.yaml/badge.svg)](https://github.com/trustpilot/python-sanicargs/actions/workflows/tox.yaml) [![Latest Version](https://img.shields.io/pypi/v/sanicargs.svg)](https://pypi.python.org/pypi/sanicargs) [![Python Support](https://img.shields.io/pypi/pyversions/sanicargs.svg)](https://pypi.python.org/pypi/sanicargs)
 
 # Sanicargs
 Parses query parameters and json body parameters for [Sanic](https://github.com/channelcat/sanic) using type annotations.
 
 ## Survey
 Please fill out [this survey](https://docs.google.com/forms/d/e/1FAIpQLSdNLvB7NEJQhUyVdaZpBAgS0f1k9OywZp8xDqhaNY0rl-unZA/viewform?usp=sf_link) if you are using Sanicargs, we are gathering feedback :-)
```

### Comparing `sanicargs-3.0.0/pyproject.toml` & `sanicargs-3.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sanicargs"
-version = "3.0.0"
+version = "3.0.1"
 description = "Parses query args or body parameters in sanic using type annotations"
 readme = "README.md"
 keywords = ["sanicargs", "sanic", "query", "args", "type annotations"]
 authors = [
     "John Sutherland <johns@trustpilot.com>",
 ]
 repository = "https://github.com/trustpilot/python-sanicargs"
```

### Comparing `sanicargs-3.0.0/sanicargs/__init__.py` & `sanicargs-3.0.1/sanicargs/__init__.py`

 * *Files identical despite different names*

### Comparing `sanicargs-3.0.0/PKG-INFO` & `sanicargs-3.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sanicargs
-Version: 3.0.0
+Version: 3.0.1
 Summary: Parses query args or body parameters in sanic using type annotations
 Home-page: https://github.com/trustpilot/python-sanicargs
 Keywords: sanicargs,sanic,query,args,type annotations
 Author: John Sutherland
 Author-email: johns@trustpilot.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ciso8601 (>=2.3.0,<3.0.0)
 Requires-Dist: sanic (>=23.6.0,<24.0.0)
 Project-URL: Repository, https://github.com/trustpilot/python-sanicargs
 Description-Content-Type: text/markdown
 
-[![Build Status](https://travis-ci.org/trustpilot/python-sanicargs.svg?branch=master)](https://travis-ci.org/trustpilot/python-sanicargs) [![Latest Version](https://img.shields.io/pypi/v/sanicargs.svg)](https://pypi.python.org/pypi/sanicargs) [![Python Support](https://img.shields.io/pypi/pyversions/sanicargs.svg)](https://pypi.python.org/pypi/sanicargs)
+[![Build Status](https://github.com/trustpilot/python-sanicargs/actions/workflows/tox.yaml/badge.svg)](https://github.com/trustpilot/python-sanicargs/actions/workflows/tox.yaml) [![Latest Version](https://img.shields.io/pypi/v/sanicargs.svg)](https://pypi.python.org/pypi/sanicargs) [![Python Support](https://img.shields.io/pypi/pyversions/sanicargs.svg)](https://pypi.python.org/pypi/sanicargs)
 
 # Sanicargs
 Parses query parameters and json body parameters for [Sanic](https://github.com/channelcat/sanic) using type annotations.
 
 ## Survey
 Please fill out [this survey](https://docs.google.com/forms/d/e/1FAIpQLSdNLvB7NEJQhUyVdaZpBAgS0f1k9OywZp8xDqhaNY0rl-unZA/viewform?usp=sf_link) if you are using Sanicargs, we are gathering feedback :-)
```

