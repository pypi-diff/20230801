# Comparing `tmp/kbrainsecurity-0.3.1.tar.gz` & `tmp/kbrainsecurity-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kbrainsecurity-0.3.1.tar", max compression
+gzip compressed data, was "kbrainsecurity-0.3.2.tar", max compression
```

## Comparing `kbrainsecurity-0.3.1.tar` & `kbrainsecurity-0.3.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    34353 2023-08-01 12:59:59.777007 kbrainsecurity-0.3.1/LICENSE.md
--rw-r--r--   0        0        0      982 2023-08-01 12:59:59.777007 kbrainsecurity-0.3.1/README.md
--rw-r--r--   0        0        0      655 2023-08-01 13:00:43.945617 kbrainsecurity-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     1498 2023-08-01 12:59:59.777007 kbrainsecurity-0.3.1/src/kbrainsecurity/azure_authentication.py
--rw-r--r--   0        0        0     1336 2023-08-01 12:59:59.777007 kbrainsecurity-0.3.1/src/kbrainsecurity/bearer.py
--rw-r--r--   0        0        0     1556 1970-01-01 00:00:00.000000 kbrainsecurity-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    34353 2023-08-01 13:08:21.721066 kbrainsecurity-0.3.2/LICENSE.md
+-rw-r--r--   0        0        0      982 2023-08-01 13:08:21.721066 kbrainsecurity-0.3.2/README.md
+-rw-r--r--   0        0        0      655 2023-08-01 13:09:17.164465 kbrainsecurity-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     1496 2023-08-01 13:08:21.721066 kbrainsecurity-0.3.2/src/kbrainsecurity/azure_authentication.py
+-rw-r--r--   0        0        0     1336 2023-08-01 13:08:21.721066 kbrainsecurity-0.3.2/src/kbrainsecurity/bearer.py
+-rw-r--r--   0        0        0     1556 1970-01-01 00:00:00.000000 kbrainsecurity-0.3.2/PKG-INFO
```

### Comparing `kbrainsecurity-0.3.1/LICENSE.md` & `kbrainsecurity-0.3.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `kbrainsecurity-0.3.1/README.md` & `kbrainsecurity-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `kbrainsecurity-0.3.1/pyproject.toml` & `kbrainsecurity-0.3.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kbrainsecurity"
-version = "0.3.1"
+version = "0.3.2"
 description = "Security and authentication functions for use in KBRAIN"
 authors = ["Daniel E. Fredriksen <daniel.fredriksen@us.kbr.com>"]
 license = "AGPLv3"
 readme = "README.md"
 packages = [{include = "kbrainsecurity", from="src"}]
 
 [tool.poetry.dependencies]
```

### Comparing `kbrainsecurity-0.3.1/src/kbrainsecurity/azure_authentication.py` & `kbrainsecurity-0.3.2/src/kbrainsecurity/azure_authentication.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,15 @@
                 )
                 try:
                     token_claims = extract_authentication_claims(req)
                     validate_claims(token_claims, required_claims)
                 except (AuthenticationTokenException, JWTError) as ae:
                     return func.HttpResponse(str(ae), status_code=401)
 
-                [data, status, headers] = callback(req, *args, **kwargs)
+                data, status, headers = callback(req, *args, **kwargs)
                 return func.HttpResponse(
                     data, 
                     status_code=status,
                     headers=headers
                 )
             except Exception as ex:
                 return func.HttpResponse(str(ex), status_code=500)
```

### Comparing `kbrainsecurity-0.3.1/src/kbrainsecurity/bearer.py` & `kbrainsecurity-0.3.2/src/kbrainsecurity/bearer.py`

 * *Files identical despite different names*

### Comparing `kbrainsecurity-0.3.1/PKG-INFO` & `kbrainsecurity-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kbrainsecurity
-Version: 0.3.1
+Version: 0.3.2
 Summary: Security and authentication functions for use in KBRAIN
 License: AGPLv3
 Author: Daniel E. Fredriksen
 Author-email: daniel.fredriksen@us.kbr.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

