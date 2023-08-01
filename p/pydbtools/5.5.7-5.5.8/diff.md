# Comparing `tmp/pydbtools-5.5.7.tar.gz` & `tmp/pydbtools-5.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydbtools-5.5.7.tar", max compression
+gzip compressed data, was "pydbtools-5.5.8.tar", max compression
```

## Comparing `pydbtools-5.5.7.tar` & `pydbtools-5.5.8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       48 2023-07-25 14:30:31.049731 pydbtools-5.5.7/docs/README.md
--rw-r--r--   0        0        0      855 2023-07-25 14:30:31.053731 pydbtools-5.5.7/pydbtools/__init__.py
--rw-r--r--   0        0        0     1130 2023-07-25 14:30:31.053731 pydbtools-5.5.7/pydbtools/_sql_render.py
--rw-r--r--   0        0        0    23104 2023-07-25 14:30:31.053731 pydbtools-5.5.7/pydbtools/_wrangler.py
--rw-r--r--   0        0        0     6391 2023-07-25 14:30:31.053731 pydbtools-5.5.7/pydbtools/utils.py
--rw-r--r--   0        0        0      857 2023-07-25 14:30:31.053731 pydbtools-5.5.7/pyproject.toml
--rw-r--r--   0        0        0      941 1970-01-01 00:00:00.000000 pydbtools-5.5.7/PKG-INFO
+-rw-r--r--   0        0        0       48 2023-08-01 10:40:48.026857 pydbtools-5.5.8/docs/README.md
+-rw-r--r--   0        0        0      855 2023-08-01 10:40:48.030857 pydbtools-5.5.8/pydbtools/__init__.py
+-rw-r--r--   0        0        0     1130 2023-08-01 10:40:48.030857 pydbtools-5.5.8/pydbtools/_sql_render.py
+-rw-r--r--   0        0        0    23104 2023-08-01 10:40:48.034857 pydbtools-5.5.8/pydbtools/_wrangler.py
+-rw-r--r--   0        0        0     6391 2023-08-01 10:40:48.034857 pydbtools-5.5.8/pydbtools/utils.py
+-rw-r--r--   0        0        0      857 2023-08-01 10:40:48.034857 pydbtools-5.5.8/pyproject.toml
+-rw-r--r--   0        0        0      941 1970-01-01 00:00:00.000000 pydbtools-5.5.8/PKG-INFO
```

### Comparing `pydbtools-5.5.7/pydbtools/__init__.py` & `pydbtools-5.5.8/pydbtools/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,8 +29,8 @@
     create_table,
 )
 
 from ._sql_render import get_sql_from_file, render_sql_template  # noqa: F401
 
 from .utils import s3_path_join  # noqa: F401
 
-__version__ = "5.5.7"
+__version__ = "5.5.8"
```

### Comparing `pydbtools-5.5.7/pydbtools/_sql_render.py` & `pydbtools-5.5.8/pydbtools/_sql_render.py`

 * *Files identical despite different names*

### Comparing `pydbtools-5.5.7/pydbtools/_wrangler.py` & `pydbtools-5.5.8/pydbtools/_wrangler.py`

 * *Files identical despite different names*

### Comparing `pydbtools-5.5.7/pydbtools/utils.py` & `pydbtools-5.5.8/pydbtools/utils.py`

 * *Files identical despite different names*

### Comparing `pydbtools-5.5.7/pyproject.toml` & `pydbtools-5.5.8/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "pydbtools"
-version = "5.5.7"
+version = "5.5.8"
 description = "A python package to query data via amazon athena and bring it into a pandas df using aws-wrangler."
 license = "MIT"
 authors = ["Karik Isichei <karik.isichei@digital.justice.gov.uk>"]
 readme = "docs/README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
```

### Comparing `pydbtools-5.5.7/PKG-INFO` & `pydbtools-5.5.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydbtools
-Version: 5.5.7
+Version: 5.5.8
 Summary: A python package to query data via amazon athena and bring it into a pandas df using aws-wrangler.
 License: MIT
 Author: Karik Isichei
 Author-email: karik.isichei@digital.justice.gov.uk
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

