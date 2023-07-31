# Comparing `tmp/akamai_purge_cache-1.0.0.tar.gz` & `tmp/akamai_purge_cache-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "akamai_purge_cache-1.0.0.tar", max compression
+gzip compressed data, was "akamai_purge_cache-1.2.0.tar", max compression
```

## Comparing `akamai_purge_cache-1.0.0.tar` & `akamai_purge_cache-1.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rwxr-xr-x   0        0        0     1085 2023-07-26 00:30:10.895312 akamai_purge_cache-1.0.0/README.md
--rwxr-xr-x   0        0        0        0 2023-07-25 14:00:09.217851 akamai_purge_cache-1.0.0/akamai_purge_cache/__init__.py
--rwxr-xr-x   0        0        0      852 2023-07-25 19:52:16.805321 akamai_purge_cache-1.0.0/akamai_purge_cache/purge.py
--rwxr-xr-x   0        0        0      711 2023-07-28 22:16:59.487049 akamai_purge_cache-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1814 1970-01-01 00:00:00.000000 akamai_purge_cache-1.0.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1085 2023-07-31 20:55:46.323684 akamai_purge_cache-1.2.0/README.md
+-rwxr-xr-x   0        0        0        0 2023-07-25 14:04:26.225250 akamai_purge_cache-1.2.0/akamai_purge_cache/__init__.py
+-rwxr-xr-x   0        0        0     1662 2023-07-31 20:55:46.324787 akamai_purge_cache-1.2.0/akamai_purge_cache/purge.py
+-rwxr-xr-x   0        0        0      711 2023-07-31 22:45:27.544217 akamai_purge_cache-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1814 1970-01-01 00:00:00.000000 akamai_purge_cache-1.2.0/PKG-INFO
```

### Comparing `akamai_purge_cache-1.0.0/README.md` & `akamai_purge_cache-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `akamai_purge_cache-1.0.0/pyproject.toml` & `akamai_purge_cache-1.2.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry] 
 name = "akamai_purge_cache"
-version = "1.0.0" 
+version = "1.2.0" 
 description = "Marriott CDN Team Fastpurge POC script" 
 authors = ["Alan Janis <alan.janis@marriott.com>", "Raahi Chada <raahi.chada@marriott.com"]
 readme = "README.md"
 packages = [{include = "akamai_purge_cache"}]
 
 [tool.poetry.dependencies]
 python = ">=3.10"
```

### Comparing `akamai_purge_cache-1.0.0/PKG-INFO` & `akamai_purge_cache-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akamai-purge-cache
-Version: 1.0.0
+Version: 1.2.0
 Summary: Marriott CDN Team Fastpurge POC script
 Author: Alan Janis
 Author-email: alan.janis@marriott.com
 Requires-Python: >=3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

