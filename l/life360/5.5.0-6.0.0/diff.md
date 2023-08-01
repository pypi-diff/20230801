# Comparing `tmp/life360-5.5.0.tar.gz` & `tmp/life360-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "life360-5.5.0.tar", last modified: Thu Jan  5 20:46:02 2023, max compression
+gzip compressed data, was "life360-6.0.0.tar", last modified: Tue Aug  1 01:57:48 2023, max compression
```

## Comparing `life360-5.5.0.tar` & `life360-6.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 pbruckner  (1000) pbruckner  (1000)        0 2023-01-05 20:46:02.602067 life360-5.5.0/
--rw-r--r--   0 pbruckner  (1000) pbruckner  (1000)     1068 2022-08-26 14:36:17.000000 life360-5.5.0/LICENSE
--rw-r--r--   0 pbruckner  (1000) pbruckner  (1000)     1027 2023-01-05 20:46:02.602067 life360-5.5.0/PKG-INFO
--rw-r--r--   0 pbruckner  (1000) pbruckner  (1000)      585 2022-08-26 14:36:17.000000 life360-5.5.0/README.md
-drwxr-xr-x   0 pbruckner  (1000) pbruckner  (1000)        0 2023-01-05 20:46:02.602067 life360-5.5.0/life360/
--rw-r--r--   0 pbruckner  (1000) pbruckner  (1000)      141 2022-08-26 19:26:53.000000 life360-5.5.0/life360/__init__.py
--rw-r--r--   0 pbruckner  (1000) pbruckner  (1000)     8172 2023-01-05 20:43:29.000000 life360-5.5.0/life360/api.py
--rw-r--r--   0 pbruckner  (1000) pbruckner  (1000)      233 2022-08-26 14:36:17.000000 life360-5.5.0/life360/exceptions.py
--rw-r--r--   0 pbruckner  (1000) pbruckner  (1000)       22 2023-01-05 20:44:39.000000 life360-5.5.0/life360/version.py
-drwxr-xr-x   0 pbruckner  (1000) pbruckner  (1000)        0 2023-01-05 20:46:02.602067 life360-5.5.0/life360.egg-info/
--rw-r--r--   0 pbruckner  (1000) pbruckner  (1000)     1027 2023-01-05 20:46:02.000000 life360-5.5.0/life360.egg-info/PKG-INFO
--rw-r--r--   0 pbruckner  (1000) pbruckner  (1000)      256 2023-01-05 20:46:02.000000 life360-5.5.0/life360.egg-info/SOURCES.txt
--rw-r--r--   0 pbruckner  (1000) pbruckner  (1000)        1 2023-01-05 20:46:02.000000 life360-5.5.0/life360.egg-info/dependency_links.txt
--rw-r--r--   0 pbruckner  (1000) pbruckner  (1000)        8 2023-01-05 20:46:02.000000 life360-5.5.0/life360.egg-info/requires.txt
--rw-r--r--   0 pbruckner  (1000) pbruckner  (1000)        8 2023-01-05 20:46:02.000000 life360-5.5.0/life360.egg-info/top_level.txt
--rw-r--r--   0 pbruckner  (1000) pbruckner  (1000)       38 2023-01-05 20:46:02.602067 life360-5.5.0/setup.cfg
--rw-r--r--   0 pbruckner  (1000) pbruckner  (1000)      756 2022-08-26 19:26:53.000000 life360-5.5.0/setup.py
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2023-08-01 01:57:48.332613 life360-6.0.0/
+-rw-rw-r--   0 phil      (1000) phil      (1000)     1068 2023-08-01 01:44:00.000000 life360-6.0.0/LICENSE
+-rw-rw-r--   0 phil      (1000) phil      (1000)     1027 2023-08-01 01:57:48.332613 life360-6.0.0/PKG-INFO
+-rw-rw-r--   0 phil      (1000) phil      (1000)      585 2023-08-01 01:44:00.000000 life360-6.0.0/README.md
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2023-08-01 01:57:48.332613 life360-6.0.0/life360/
+-rw-rw-r--   0 phil      (1000) phil      (1000)      141 2023-08-01 01:44:00.000000 life360-6.0.0/life360/__init__.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     8271 2023-08-01 01:44:00.000000 life360-6.0.0/life360/api.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)      233 2023-08-01 01:44:00.000000 life360-6.0.0/life360/exceptions.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)       22 2023-08-01 01:44:00.000000 life360-6.0.0/life360/version.py
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2023-08-01 01:57:48.332613 life360-6.0.0/life360.egg-info/
+-rw-rw-r--   0 phil      (1000) phil      (1000)     1027 2023-08-01 01:57:48.000000 life360-6.0.0/life360.egg-info/PKG-INFO
+-rw-rw-r--   0 phil      (1000) phil      (1000)      256 2023-08-01 01:57:48.000000 life360-6.0.0/life360.egg-info/SOURCES.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)        1 2023-08-01 01:57:48.000000 life360-6.0.0/life360.egg-info/dependency_links.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)        8 2023-08-01 01:57:48.000000 life360-6.0.0/life360.egg-info/requires.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)        8 2023-08-01 01:57:48.000000 life360-6.0.0/life360.egg-info/top_level.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)       38 2023-08-01 01:57:48.332613 life360-6.0.0/setup.cfg
+-rw-rw-r--   0 phil      (1000) phil      (1000)      756 2023-08-01 01:44:00.000000 life360-6.0.0/setup.py
```

### Comparing `life360-5.5.0/LICENSE` & `life360-6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `life360-5.5.0/PKG-INFO` & `life360-6.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: life360
-Version: 5.5.0
+Version: 6.0.0
 Summary: Life360 Communications Module
 Home-page: https://github.com/pnbruckner/life360
 Author: Phil Bruckner
 Author-email: pnbruckner@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `life360-5.5.0/README.md` & `life360-6.0.0/README.md`

 * *Files identical despite different names*

### Comparing `life360-5.5.0/life360/api.py` & `life360-6.0.0/life360/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import Any, Optional, Union, cast
 
 import aiohttp
 
 from .exceptions import *
 
 _PROTOCOL = "https://"
-_HOST = "api.life360.com"
+_HOST = "api-cloudfront.life360.com"
 _BASE_URL = f"{_PROTOCOL}{_HOST}"
 _BASE_CMD = f"{_BASE_URL}/v3/"
 _TOKEN_URL = f"{_BASE_CMD}oauth2/token.json"
 _CIRCLES_URL = f"{_BASE_CMD}circles.json"
 _CIRCLE_URL_FMT = f"{_BASE_CMD}circles/{{circle_id}}"
 _CIRCLE_MEMBERS_URL_FMT = f"{_CIRCLE_URL_FMT}/members"
 _CIRCLE_PLACES_URL_FMT = f"{_CIRCLE_URL_FMT}/places"
@@ -26,17 +26,18 @@
 _EXC_REPR_REDACTIONS = (
     _URL_REDACTION,
     (re.compile(r"('Bearer )[^']+'"), r"\1REDACTED'"),
     (re.compile(r"('L360-ETag': ')[^']*'"), r"\1REDACTED'"),
 )
 _LOGGER = logging.getLogger(__name__)
 
+USER_AGENT = "com.life360.android.safetymapd"
 CLIENT_TOKEN = (
-    "cFJFcXVnYWJSZXRyZTRFc3RldGhlcnVmcmVQdW1hbUV4dWNyRU"
-    "h1YzptM2ZydXBSZXRSZXN3ZXJFQ2hBUHJFOTZxYWtFZHI0Vg=="
+    "Y2F0aGFwYWNyQVBoZUtVc3RlOGV2ZXZldnVjSGFmZVRydVl1Zn"
+    "JhYzpkOEM5ZVlVdkE2dUZ1YnJ1SmVnZXRyZVZ1dFJlQ1JVWQ=="
 )
 HTTP_FORBIDDEN = 403
 HTTP_BAD_GATEWAY = 502
 HTTP_SERVICE_UNAVAILABLE = 503
 HTTP_GATEWAY_TIME_OUT = 504
 
 RETRY_CLIENT_RESPONSE_ERRORS = (
@@ -190,14 +191,15 @@
         if not msg:
             msg = f"Error {method.upper()}({_redact(url, _URL_REDACTIONS)})"
 
         kwargs = {
             "headers": {
                 "Accept": "application/json",
                 "cache-control": "no-cache",
+                "user-agent": USER_AGENT,
                 "Authorization": authorization
                 if authorization
                 else self._authorization,
             },
         }
         if data is not None:
             kwargs["data"] = data
```

### Comparing `life360-5.5.0/life360.egg-info/PKG-INFO` & `life360-6.0.0/life360.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: life360
-Version: 5.5.0
+Version: 6.0.0
 Summary: Life360 Communications Module
 Home-page: https://github.com/pnbruckner/life360
 Author: Phil Bruckner
 Author-email: pnbruckner@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `life360-5.5.0/setup.py` & `life360-6.0.0/setup.py`

 * *Files identical despite different names*

