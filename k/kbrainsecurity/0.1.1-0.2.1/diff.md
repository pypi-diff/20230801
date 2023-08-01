# Comparing `tmp/kbrainsecurity-0.1.1.tar.gz` & `tmp/kbrainsecurity-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kbrainsecurity-0.1.1.tar", max compression
+gzip compressed data, was "kbrainsecurity-0.2.1.tar", max compression
```

## Comparing `kbrainsecurity-0.1.1.tar` & `kbrainsecurity-0.2.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    34353 2023-08-01 03:25:52.729279 kbrainsecurity-0.1.1/LICENSE.md
--rw-r--r--   0        0        0      982 2023-08-01 03:25:52.729279 kbrainsecurity-0.1.1/README.md
--rw-r--r--   0        0        0      655 2023-08-01 03:26:38.677915 kbrainsecurity-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1318 2023-08-01 03:25:52.733279 kbrainsecurity-0.1.1/src/kbrainsecurity/azure_authentication.py
--rw-r--r--   0        0        0     1336 2023-08-01 03:25:52.733279 kbrainsecurity-0.1.1/src/kbrainsecurity/bearer.py
--rw-r--r--   0        0        0     1556 1970-01-01 00:00:00.000000 kbrainsecurity-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    34353 2023-08-01 04:31:26.905665 kbrainsecurity-0.2.1/LICENSE.md
+-rw-r--r--   0        0        0      982 2023-08-01 04:31:26.905665 kbrainsecurity-0.2.1/README.md
+-rw-r--r--   0        0        0      655 2023-08-01 04:32:10.517854 kbrainsecurity-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1393 2023-08-01 04:31:26.905665 kbrainsecurity-0.2.1/src/kbrainsecurity/azure_authentication.py
+-rw-r--r--   0        0        0     1336 2023-08-01 04:31:26.905665 kbrainsecurity-0.2.1/src/kbrainsecurity/bearer.py
+-rw-r--r--   0        0        0     1556 1970-01-01 00:00:00.000000 kbrainsecurity-0.2.1/PKG-INFO
```

### Comparing `kbrainsecurity-0.1.1/LICENSE.md` & `kbrainsecurity-0.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `kbrainsecurity-0.1.1/README.md` & `kbrainsecurity-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `kbrainsecurity-0.1.1/pyproject.toml` & `kbrainsecurity-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kbrainsecurity"
-version = "0.1.1"
+version = "0.2.1"
 description = "Security and authentication functions for use in KBRAIN"
 authors = ["Daniel E. Fredriksen <daniel.fredriksen@us.kbr.com>"]
 license = "AGPLv3"
 readme = "README.md"
 packages = [{include = "kbrainsecurity", from="src"}]
 
 [tool.poetry.dependencies]
```

### Comparing `kbrainsecurity-0.1.1/src/kbrainsecurity/azure_authentication.py` & `kbrainsecurity-0.2.1/src/kbrainsecurity/azure_authentication.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,30 +7,33 @@
 from jose import JWTError
 
 from .bearer import AuthenticationTokenException
 from .bearer import extract_claims
 from .bearer import validate_claims
 
 
+def extract_authentication_claims(req: func.HttpRequest):
+    auth = req.headers.get("Authorization", None)
+    return extract_claims(auth)
+
 def authenticate_request(required_claims: dict[str, any]) -> func.HttpResponse:
     def argument_wrapper(callback: Callable[..., any]):
         @functools.wraps(callback)
         def wrapper(req: func.HttpRequest, *args, **kwargs) -> func.HttpResponse:
             try:
                 logging.info(
                     f"KBRAIN Authentication. Required claims: {json.dumps(required_claims)}"
                 )
                 try:
-                    auth = req.headers.get("Authorization", None)
-                    token_claims = extract_claims(auth)
+                    token_claims = extract_authentication_claims(req)
                     validate_claims(token_claims, required_claims)
                 except (AuthenticationTokenException, JWTError) as ae:
                     return func.HttpResponse(str(ae), status_code=401)
 
-                [data, status] = callback(req, token_claims, *args, **kwargs)
+                [data, status] = callback(req, *args, **kwargs)
                 return func.HttpResponse(data, status_code=status)
             except Exception as ex:
                 return func.HttpResponse(str(ex), status_code=500)
 
         return wrapper
 
     return argument_wrapper
```

### Comparing `kbrainsecurity-0.1.1/src/kbrainsecurity/bearer.py` & `kbrainsecurity-0.2.1/src/kbrainsecurity/bearer.py`

 * *Files identical despite different names*

### Comparing `kbrainsecurity-0.1.1/PKG-INFO` & `kbrainsecurity-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kbrainsecurity
-Version: 0.1.1
+Version: 0.2.1
 Summary: Security and authentication functions for use in KBRAIN
 License: AGPLv3
 Author: Daniel E. Fredriksen
 Author-email: daniel.fredriksen@us.kbr.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

