# Comparing `tmp/nemusicapi-0.0.1.tar.gz` & `tmp/nemusicapi-0.0.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nemusicapi-0.0.1.tar", max compression
+gzip compressed data, was "nemusicapi-0.0.2a1.tar", max compression
```

## Comparing `nemusicapi-0.0.1.tar` & `nemusicapi-0.0.2a1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    11558 2023-08-01 07:21:02.527622 nemusicapi-0.0.1/LICENSE
--rw-r--r--   0        0        0     3351 2023-08-01 07:33:42.704150 nemusicapi-0.0.1/NEmusicApi/api.py
--rw-r--r--   0        0        0      350 2023-08-01 09:07:26.281821 nemusicapi-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       40 2023-08-01 07:21:02.528622 nemusicapi-0.0.1/README.md
--rw-r--r--   0        0        0      569 1970-01-01 00:00:00.000000 nemusicapi-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11558 2023-08-01 07:21:02.527622 nemusicapi-0.0.2a1/LICENSE
+-rw-r--r--   0        0        0     3351 2023-08-01 07:33:42.704150 nemusicapi-0.0.2a1/NEmusicApi/api.py
+-rw-r--r--   0        0        0      466 2023-08-01 09:17:47.191205 nemusicapi-0.0.2a1/pyproject.toml
+-rw-r--r--   0        0        0       40 2023-08-01 07:21:02.528622 nemusicapi-0.0.2a1/README.md
+-rw-r--r--   0        0        0      705 1970-01-01 00:00:00.000000 nemusicapi-0.0.2a1/PKG-INFO
```

### Comparing `nemusicapi-0.0.1/LICENSE` & `nemusicapi-0.0.2a1/LICENSE`

 * *Files identical despite different names*

### Comparing `nemusicapi-0.0.1/NEmusicApi/api.py` & `nemusicapi-0.0.2a1/NEmusicApi/api.py`

 * *Files identical despite different names*

### Comparing `nemusicapi-0.0.1/PKG-INFO` & `nemusicapi-0.0.2a1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: nemusicapi
-Version: 0.0.1
+Version: 0.0.2a1
 Summary: A Netsase music api
-License: Apache License
+Home-page: https://github.com/yuyi2439/NeteaseMusicApi
+License: Apache-2.0
 Author: yuyi2439
 Requires-Python: >=3.9,<4.0
-Classifier: License :: Other/Proprietary License
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pycryptodome (>=3.18.0,<4.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
+Project-URL: Repository, https://github.com/yuyi2439/NeteaseMusicApi
 Description-Content-Type: text/markdown
 
 # NeteaseMusicApi
 A netsase music api
```

