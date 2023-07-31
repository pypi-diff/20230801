# Comparing `tmp/retakesearch-0.1.19.tar.gz` & `tmp/retakesearch-0.1.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retakesearch-0.1.19.tar", max compression
+gzip compressed data, was "retakesearch-0.1.20.tar", max compression
```

## Comparing `retakesearch-0.1.19.tar` & `retakesearch-0.1.20.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2023-07-31 22:32:28.353806 retakesearch-0.1.19/README.md
--rw-r--r--   0        0        0      429 2023-07-31 22:32:50.934021 retakesearch-0.1.19/pyproject.toml
--rw-r--r--   0        0        0      174 2023-07-31 22:32:28.353806 retakesearch-0.1.19/retakesearch/__init__.py
--rw-r--r--   0        0        0     1818 2023-07-31 22:32:28.353806 retakesearch-0.1.19/retakesearch/client.py
--rw-r--r--   0        0        0     3796 2023-07-31 22:32:28.353806 retakesearch-0.1.19/retakesearch/index.py
--rw-r--r--   0        0        0      159 2023-07-31 22:32:28.353806 retakesearch-0.1.19/retakesearch/search.py
--rw-r--r--   0        0        0      699 1970-01-01 00:00:00.000000 retakesearch-0.1.19/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-31 23:41:14.051745 retakesearch-0.1.20/README.md
+-rw-r--r--   0        0        0      429 2023-07-31 23:41:31.127879 retakesearch-0.1.20/pyproject.toml
+-rw-r--r--   0        0        0      174 2023-07-31 23:41:14.051745 retakesearch-0.1.20/retakesearch/__init__.py
+-rw-r--r--   0        0        0     1818 2023-07-31 23:41:14.051745 retakesearch-0.1.20/retakesearch/client.py
+-rw-r--r--   0        0        0     3796 2023-07-31 23:41:14.051745 retakesearch-0.1.20/retakesearch/index.py
+-rw-r--r--   0        0        0      159 2023-07-31 23:41:14.051745 retakesearch-0.1.20/retakesearch/search.py
+-rw-r--r--   0        0        0      699 1970-01-01 00:00:00.000000 retakesearch-0.1.20/PKG-INFO
```

### Comparing `retakesearch-0.1.19/retakesearch/client.py` & `retakesearch-0.1.20/retakesearch/client.py`

 * *Files identical despite different names*

### Comparing `retakesearch-0.1.19/retakesearch/index.py` & `retakesearch-0.1.20/retakesearch/index.py`

 * *Files identical despite different names*

### Comparing `retakesearch-0.1.19/PKG-INFO` & `retakesearch-0.1.20/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: retakesearch
-Version: 0.1.19
+Version: 0.1.20
 Summary: Python client for Retake: universal search infra for developers
 Author: Ming Ying
 Author-email: ming.ying.nyc@gmail.com
 Requires-Python: >=3.6,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: certifi (>=2023.7.22,<2024.0.0)
-Requires-Dist: retakesearch-py (>=2.2.1,<3.0.0)
+Requires-Dist: retakesearch-py (>=2.2.2,<3.0.0)
 Description-Content-Type: text/markdown
```

