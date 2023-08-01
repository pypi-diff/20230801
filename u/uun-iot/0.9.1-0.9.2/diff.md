# Comparing `tmp/uun-iot-0.9.1.tar.gz` & `tmp/uun-iot-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uun-iot-0.9.1.tar", last modified: Tue Aug  1 11:28:04 2023, max compression
+gzip compressed data, was "uun-iot-0.9.2.tar", last modified: Tue Aug  1 12:01:08 2023, max compression
```

## Comparing `uun-iot-0.9.1.tar` & `uun-iot-0.9.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 11:28:04.861788 uun-iot-0.9.1/
--rw-------   0 hello     (1000) hello     (1000)     1075 2023-01-22 14:43:51.000000 uun-iot-0.9.1/LICENSE.md
--rw-------   0 hello     (1000) hello     (1000)      468 2023-08-01 11:28:04.861788 uun-iot-0.9.1/PKG-INFO
--rw-------   0 hello     (1000) hello     (1000)     1965 2022-10-16 10:02:57.000000 uun-iot-0.9.1/README.md
--rw-------   0 hello     (1000) hello     (1000)       38 2023-08-01 11:28:04.861788 uun-iot-0.9.1/setup.cfg
--rw-------   0 hello     (1000) hello     (1000)      892 2023-01-22 14:43:43.000000 uun-iot-0.9.1/setup.py
-drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 11:28:04.861788 uun-iot-0.9.1/uun_iot/
--rw-------   0 hello     (1000) hello     (1000)    25084 2022-10-30 12:40:32.000000 uun-iot-0.9.1/uun_iot/Gateway.py
--rw-------   0 hello     (1000) hello     (1000)    20253 2023-06-24 09:53:33.000000 uun-iot-0.9.1/uun_iot/UuAppClient.py
--rw-------   0 hello     (1000) hello     (1000)      224 2023-08-01 10:00:52.000000 uun-iot-0.9.1/uun_iot/__init__.py
--rw-------   0 hello     (1000) hello     (1000)     9179 2023-08-01 07:17:17.000000 uun-iot-0.9.1/uun_iot/decorators.py
--rw-------   0 hello     (1000) hello     (1000)     1916 2022-10-16 10:02:57.000000 uun-iot-0.9.1/uun_iot/diagnostic.py
-drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 11:28:04.861788 uun-iot-0.9.1/uun_iot/modules/
--rw-------   0 hello     (1000) hello     (1000)    14058 2022-10-23 08:04:43.000000 uun-iot-0.9.1/uun_iot/modules/BaseHealthCheck.py
--rw-------   0 hello     (1000) hello     (1000)     2018 2022-10-16 10:02:57.000000 uun-iot-0.9.1/uun_iot/modules/Heartbeat.py
--rw-------   0 hello     (1000) hello     (1000)    10128 2022-10-31 07:37:38.000000 uun-iot-0.9.1/uun_iot/modules/Module.py
--rw-------   0 hello     (1000) hello     (1000)      362 2022-10-16 10:02:57.000000 uun-iot-0.9.1/uun_iot/modules/__init__.py
--rw-------   0 hello     (1000) hello     (1000)      367 2022-10-16 10:02:57.000000 uun-iot-0.9.1/uun_iot/typing.py
--rw-------   0 hello     (1000) hello     (1000)    12903 2023-08-01 09:53:25.000000 uun-iot-0.9.1/uun_iot/utils.py
-drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 11:28:04.861788 uun-iot-0.9.1/uun_iot.egg-info/
--rw-------   0 hello     (1000) hello     (1000)      468 2023-08-01 11:28:04.000000 uun-iot-0.9.1/uun_iot.egg-info/PKG-INFO
--rw-------   0 hello     (1000) hello     (1000)      442 2023-08-01 11:28:04.000000 uun-iot-0.9.1/uun_iot.egg-info/SOURCES.txt
--rw-------   0 hello     (1000) hello     (1000)        1 2023-08-01 11:28:04.000000 uun-iot-0.9.1/uun_iot.egg-info/dependency_links.txt
--rw-------   0 hello     (1000) hello     (1000)       56 2023-08-01 11:28:04.000000 uun-iot-0.9.1/uun_iot.egg-info/requires.txt
--rw-------   0 hello     (1000) hello     (1000)        8 2023-08-01 11:28:04.000000 uun-iot-0.9.1/uun_iot.egg-info/top_level.txt
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 12:01:08.193438 uun-iot-0.9.2/
+-rw-------   0 hello     (1000) hello     (1000)     1075 2023-01-22 14:43:51.000000 uun-iot-0.9.2/LICENSE.md
+-rw-------   0 hello     (1000) hello     (1000)      468 2023-08-01 12:01:08.193438 uun-iot-0.9.2/PKG-INFO
+-rw-------   0 hello     (1000) hello     (1000)     1965 2022-10-16 10:02:57.000000 uun-iot-0.9.2/README.md
+-rw-------   0 hello     (1000) hello     (1000)       38 2023-08-01 12:01:08.193438 uun-iot-0.9.2/setup.cfg
+-rw-------   0 hello     (1000) hello     (1000)      892 2023-01-22 14:43:43.000000 uun-iot-0.9.2/setup.py
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 12:01:08.193438 uun-iot-0.9.2/uun_iot/
+-rw-------   0 hello     (1000) hello     (1000)    25084 2022-10-30 12:40:32.000000 uun-iot-0.9.2/uun_iot/Gateway.py
+-rw-------   0 hello     (1000) hello     (1000)    20292 2023-08-01 11:59:34.000000 uun-iot-0.9.2/uun_iot/UuAppClient.py
+-rw-------   0 hello     (1000) hello     (1000)      224 2023-08-01 12:00:39.000000 uun-iot-0.9.2/uun_iot/__init__.py
+-rw-------   0 hello     (1000) hello     (1000)     9179 2023-08-01 07:17:17.000000 uun-iot-0.9.2/uun_iot/decorators.py
+-rw-------   0 hello     (1000) hello     (1000)     1916 2022-10-16 10:02:57.000000 uun-iot-0.9.2/uun_iot/diagnostic.py
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 12:01:08.193438 uun-iot-0.9.2/uun_iot/modules/
+-rw-------   0 hello     (1000) hello     (1000)    14058 2022-10-23 08:04:43.000000 uun-iot-0.9.2/uun_iot/modules/BaseHealthCheck.py
+-rw-------   0 hello     (1000) hello     (1000)     2018 2022-10-16 10:02:57.000000 uun-iot-0.9.2/uun_iot/modules/Heartbeat.py
+-rw-------   0 hello     (1000) hello     (1000)    10128 2022-10-31 07:37:38.000000 uun-iot-0.9.2/uun_iot/modules/Module.py
+-rw-------   0 hello     (1000) hello     (1000)      362 2022-10-16 10:02:57.000000 uun-iot-0.9.2/uun_iot/modules/__init__.py
+-rw-------   0 hello     (1000) hello     (1000)      367 2022-10-16 10:02:57.000000 uun-iot-0.9.2/uun_iot/typing.py
+-rw-------   0 hello     (1000) hello     (1000)    12903 2023-08-01 09:53:25.000000 uun-iot-0.9.2/uun_iot/utils.py
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 12:01:08.193438 uun-iot-0.9.2/uun_iot.egg-info/
+-rw-------   0 hello     (1000) hello     (1000)      468 2023-08-01 12:01:08.000000 uun-iot-0.9.2/uun_iot.egg-info/PKG-INFO
+-rw-------   0 hello     (1000) hello     (1000)      442 2023-08-01 12:01:08.000000 uun-iot-0.9.2/uun_iot.egg-info/SOURCES.txt
+-rw-------   0 hello     (1000) hello     (1000)        1 2023-08-01 12:01:08.000000 uun-iot-0.9.2/uun_iot.egg-info/dependency_links.txt
+-rw-------   0 hello     (1000) hello     (1000)       56 2023-08-01 12:01:08.000000 uun-iot-0.9.2/uun_iot.egg-info/requires.txt
+-rw-------   0 hello     (1000) hello     (1000)        8 2023-08-01 12:01:08.000000 uun-iot-0.9.2/uun_iot.egg-info/top_level.txt
```

### Comparing `uun-iot-0.9.1/LICENSE.md` & `uun-iot-0.9.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `uun-iot-0.9.1/README.md` & `uun-iot-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `uun-iot-0.9.1/setup.py` & `uun-iot-0.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `uun-iot-0.9.1/uun_iot/Gateway.py` & `uun-iot-0.9.2/uun_iot/Gateway.py`

 * *Files identical despite different names*

### Comparing `uun-iot-0.9.1/uun_iot/UuAppClient.py` & `uun-iot-0.9.2/uun_iot/UuAppClient.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,15 +193,15 @@
         uri = "/%s/%s/%s" % (uu_app_name, awid, uucmd)
         return "https://%s%s" % (gateway, uri)
 
     def get_request(
         self,
         uucmd: str,
         dto_in: dict = {},
-        http_error_level: int | None = logging.WARNING,
+        http_error_level: Optional[int] = logging.WARNING,
     ) -> requests.Response:
         """GET request with oidc2 authentication.
 
         Args:
             uucmd: uuCmd path of the target uuApp
             dto_in: data to be passed as JSON input to the uuApp
             http_error_level: logging library level of HTTP error (HTTP status
@@ -230,15 +230,15 @@
                     response.text,
                 )
 
         return response
 
     def get(
         self, uucmd: str, dto_in: dict = {}, log_level: int = logging.WARNING
-    ) -> Tuple[requests.Response | None, Tuple[bool, requests.RequestException | None]]:
+    ) -> Tuple[Optional[requests.Response], Tuple[bool, Optional[requests.RequestException]]]:
         """Get request
 
         Get request using a Bearer token. Connection errors are suppressed, logged and returned.
 
         Args:
             uucmd: UuCmd in relative path format, eg. "gateway/heartbeat"
             dto_in: data to send
@@ -274,15 +274,15 @@
 
         return response, (ok, exc)
 
     def post_request(
         self,
         uucmd: str,
         dto_in: dict = {},
-        http_error_level: int | None = logging.WARNING,
+        http_error_level: Optional[int] = logging.WARNING,
     ) -> requests.Response:
         """POST request with oidc2 authentication.
 
         Args:
             uucmd: uuCmd path of the target uuApp
             dto_in: data to be passed as JSON input to the uuApp
             http_error_level: logging library level of HTTP error (HTTP status
@@ -311,15 +311,15 @@
                     response.text,
                 )
 
         return response
 
     def post(
         self, uucmd: str, dto_in: dict = {}, log_level: int = logging.WARNING
-    ) -> Tuple[requests.Response | None, Tuple[bool, requests.RequestException | None]]:
+    ) -> Tuple[Optional[requests.Response], Tuple[bool, Optional[requests.RequestException]]]:
         """Post request
 
         Post request using a Bearer token. Connection errors are suppressed, logged and returned.
 
         Args:
             uucmd: UuCmd in relative path format, eg. "gateway/heartbeat"
             dto_in: data to send
@@ -352,15 +352,15 @@
         except requests.RequestException as e:
             logger.log(log_level, "`%s` POST RequestException: %s", uucmd, str(e))
             exc = e
 
         return response, (ok, exc)
 
     def multipart_request(
-        self, uucmd: str, dto_in: dict, http_error_level: int | None = logging.WARNING
+        self, uucmd: str, dto_in: dict, http_error_level: Optional[int] = logging.WARNING
     ):
         """POST request with oidc2 authentication and MULTIPART encoded data
         with oidc2 authentication. Useful for sending binary data (images, ...). See
         https://toolbelt.readthedocs.io/en/latest/user.html#multipart-form-data-encoder
         for information about multipart encoder.
 
         Args:
@@ -391,15 +391,15 @@
                     response.text,
                 )
 
         return response
 
     def multipart(
         self, uucmd: str, dto_in: dict = {}, log_level: int = logging.WARNING
-    ) -> Tuple[requests.Response | None, Tuple[bool, requests.RequestException | None]]:
+    ) -> Tuple[Optional[requests.Response], Tuple[bool, Optional[requests.RequestException]]]:
         """Multipart request
 
         Multipart request using a Bearer token. Connection errors are suppressed, logged and returned.
 
         Args:
             uucmd: UuCmd in relative path format, eg. "gateway/heartbeat"
             dto_in: data to send
@@ -453,15 +453,15 @@
                 "Content-type": "application/json",
                 "User-Agent": uuclient._user_agent,
             }
         )
 
     def get(
         self, data
-    ) -> Tuple[requests.Response | None, Tuple[bool, requests.RequestException | None]]:
+    ) -> Tuple[Optional[requests.Response], Tuple[bool, Optional[requests.RequestException]]]:
         """Get request."""
         logger.debug("`%s` GET request, payload: %s", self._uucmd, data)
 
         response = None
         ok = False
         exc = None
         try:
@@ -501,15 +501,15 @@
             )
             return response, False
 
         return response, True
 
     def post(
         self, data
-    ) -> Tuple[requests.Response | None, Tuple[bool, requests.RequestException | None]]:
+    ) -> Tuple[Optional[requests.Response], Tuple[bool, Optional[requests.RequestException]]]:
         """Post request."""
         logger.debug("`%s` POST request, payload: %s", self._uucmd, data)
 
         response = None
         ok = False
         exc = None
         try:
```

### Comparing `uun-iot-0.9.1/uun_iot/decorators.py` & `uun-iot-0.9.2/uun_iot/decorators.py`

 * *Files identical despite different names*

### Comparing `uun-iot-0.9.1/uun_iot/diagnostic.py` & `uun-iot-0.9.2/uun_iot/diagnostic.py`

 * *Files identical despite different names*

### Comparing `uun-iot-0.9.1/uun_iot/modules/BaseHealthCheck.py` & `uun-iot-0.9.2/uun_iot/modules/BaseHealthCheck.py`

 * *Files identical despite different names*

### Comparing `uun-iot-0.9.1/uun_iot/modules/Heartbeat.py` & `uun-iot-0.9.2/uun_iot/modules/Heartbeat.py`

 * *Files identical despite different names*

### Comparing `uun-iot-0.9.1/uun_iot/modules/Module.py` & `uun-iot-0.9.2/uun_iot/modules/Module.py`

 * *Files identical despite different names*

### Comparing `uun-iot-0.9.1/uun_iot/utils.py` & `uun-iot-0.9.2/uun_iot/utils.py`

 * *Files identical despite different names*

