# Comparing `tmp/altvmasterlist-2.5.0.tar.gz` & `tmp/altvmasterlist-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "altvmasterlist-2.5.0.tar", max compression
+gzip compressed data, was "altvmasterlist-2.5.1.tar", max compression
```

## Comparing `altvmasterlist-2.5.0.tar` & `altvmasterlist-2.5.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    16725 2023-05-26 12:19:41.827143 altvmasterlist-2.5.0/LICENSE
--rw-r--r--   0        0        0      425 2023-05-26 12:19:41.827143 altvmasterlist-2.5.0/README.md
--rw-r--r--   0        0        0     1073 2023-05-26 12:19:41.831143 altvmasterlist-2.5.0/pyproject.toml
--rw-r--r--   0        0        0      402 2023-05-26 12:19:41.831143 altvmasterlist-2.5.0/src/altvmasterlist/__init__.py
--rw-r--r--   0        0        0     6960 2023-05-26 12:19:41.831143 altvmasterlist-2.5.0/src/altvmasterlist/altstats.py
--rw-r--r--   0        0        0     9658 2023-05-26 12:19:41.831143 altvmasterlist-2.5.0/src/altvmasterlist/masterlist.py
--rw-r--r--   0        0        0    11294 2023-05-26 12:19:41.831143 altvmasterlist-2.5.0/src/altvmasterlist/shared.py
--rw-r--r--   0        0        0     1367 1970-01-01 00:00:00.000000 altvmasterlist-2.5.0/PKG-INFO
+-rw-r--r--   0        0        0    16725 2023-08-01 08:30:18.983054 altvmasterlist-2.5.1/LICENSE
+-rw-r--r--   0        0        0      425 2023-08-01 08:30:18.983054 altvmasterlist-2.5.1/README.md
+-rw-r--r--   0        0        0     1073 2023-08-01 08:30:18.987055 altvmasterlist-2.5.1/pyproject.toml
+-rw-r--r--   0        0        0      402 2023-08-01 08:30:18.987055 altvmasterlist-2.5.1/src/altvmasterlist/__init__.py
+-rw-r--r--   0        0        0     6960 2023-08-01 08:30:18.987055 altvmasterlist-2.5.1/src/altvmasterlist/altstats.py
+-rw-r--r--   0        0        0     9658 2023-08-01 08:30:18.987055 altvmasterlist-2.5.1/src/altvmasterlist/masterlist.py
+-rw-r--r--   0        0        0    11294 2023-08-01 08:30:18.987055 altvmasterlist-2.5.1/src/altvmasterlist/shared.py
+-rw-r--r--   0        0        0     1367 1970-01-01 00:00:00.000000 altvmasterlist-2.5.1/PKG-INFO
```

### Comparing `altvmasterlist-2.5.0/LICENSE` & `altvmasterlist-2.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `altvmasterlist-2.5.0/pyproject.toml` & `altvmasterlist-2.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "altvmasterlist"
-version = "2.5.0"
+version = "2.5.1"
 description = "A package to use the alt:V Masterlist api."
 authors = ["Nickwasused <contact.nickwasused.fa6c8@simplelogin.co>"]
 license = "MPL-2.0"
 readme = "README.md"
 repository = "https://github.com/Nickwasused/altv-python-masterlist"
 documentation = "https://nickwasused.github.io/altv-python-masterlist/"
 classifiers = [
```

### Comparing `altvmasterlist-2.5.0/src/altvmasterlist/altstats.py` & `altvmasterlist-2.5.1/src/altvmasterlist/altstats.py`

 * *Files identical despite different names*

### Comparing `altvmasterlist-2.5.0/src/altvmasterlist/masterlist.py` & `altvmasterlist-2.5.1/src/altvmasterlist/masterlist.py`

 * *Files identical despite different names*

### Comparing `altvmasterlist-2.5.0/src/altvmasterlist/shared.py` & `altvmasterlist-2.5.1/src/altvmasterlist/shared.py`

 * *Files identical despite different names*

### Comparing `altvmasterlist-2.5.0/PKG-INFO` & `altvmasterlist-2.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: altvmasterlist
-Version: 2.5.0
+Version: 2.5.1
 Summary: A package to use the alt:V Masterlist api.
 Home-page: https://github.com/Nickwasused/altv-python-masterlist
 License: MPL-2.0
 Author: Nickwasused
 Author-email: contact.nickwasused.fa6c8@simplelogin.co
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved
```

