# Comparing `tmp/superagent_py-0.0.39.tar.gz` & `tmp/superagent_py-0.0.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superagent_py-0.0.39.tar", max compression
+gzip compressed data, was "superagent_py-0.0.40.tar", max compression
```

## Comparing `superagent_py-0.0.39.tar` & `superagent_py-0.0.40.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1073 2023-07-31 23:06:16.440027 superagent_py-0.0.39/LICENSE
--rw-r--r--   0        0        0     3251 2023-07-31 23:06:16.440027 superagent_py-0.0.39/README.md
--rw-r--r--   0        0        0      380 2023-07-31 23:06:16.440027 superagent_py-0.0.39/pyproject.toml
--rw-r--r--   0        0        0      656 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/__init__.py
--rw-r--r--   0        0        0     3186 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/client.py
--rw-r--r--   0        0        0      348 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/core/__init__.py
--rw-r--r--   0        0        0      426 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      170 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/errors/__init__.py
--rw-r--r--   0        0        0      313 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0        0 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/py.typed
--rw-r--r--   0        0        0      361 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/resources/agent/__init__.py
--rw-r--r--   0        0        0    14309 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/resources/agent/client.py
--rw-r--r--   0        0        0       65 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/resources/agent_documents/__init__.py
--rw-r--r--   0        0        0     9260 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/resources/agent_documents/client.py
--rw-r--r--   0        0        0       65 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/resources/agent_tools/__init__.py
--rw-r--r--   0        0        0     9132 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/resources/agent_tools/client.py
--rw-r--r--   0        0        0       65 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/resources/api_token/__init__.py
--rw-r--r--   0        0        0     8538 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/resources/api_token/client.py
--rw-r--r--   0        0        0       65 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/resources/auth/__init__.py
--rw-r--r--   0        0        0     5901 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/resources/auth/client.py
--rw-r--r--   0        0        0       65 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/resources/documents/__init__.py
--rw-r--r--   0        0        0    12664 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/resources/documents/client.py
--rw-r--r--   0        0        0       65 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/resources/prompts/__init__.py
--rw-r--r--   0        0        0    10865 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/resources/prompts/client.py
--rw-r--r--   0        0        0       65 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/resources/tags/__init__.py
--rw-r--r--   0        0        0    10575 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/resources/tags/client.py
--rw-r--r--   0        0        0       65 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/resources/tools/__init__.py
--rw-r--r--   0        0        0    11638 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/resources/tools/client.py
--rw-r--r--   0        0        0       65 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/resources/traces/__init__.py
--rw-r--r--   0        0        0     2236 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/resources/traces/client.py
--rw-r--r--   0        0        0       65 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/resources/user/__init__.py
--rw-r--r--   0        0        0     4328 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/resources/user/client.py
--rw-r--r--   0        0        0      308 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/types/__init__.py
--rw-r--r--   0        0        0      843 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/types/http_validation_error.py
--rw-r--r--   0        0        0      869 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/types/validation_error.py
--rw-r--r--   0        0        0      128 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/types/validation_error_loc_item.py
--rw-r--r--   0        0        0     3762 1970-01-01 00:00:00.000000 superagent_py-0.0.39/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-08-01 13:21:44.119876 superagent_py-0.0.40/LICENSE
+-rw-r--r--   0        0        0     3251 2023-08-01 13:21:44.119876 superagent_py-0.0.40/README.md
+-rw-r--r--   0        0        0      380 2023-08-01 13:21:44.119876 superagent_py-0.0.40/pyproject.toml
+-rw-r--r--   0        0        0      656 2023-08-01 13:21:44.119876 superagent_py-0.0.40/src/superagent/__init__.py
+-rw-r--r--   0        0        0     3186 2023-08-01 13:21:44.119876 superagent_py-0.0.40/src/superagent/client.py
+-rw-r--r--   0        0        0      348 2023-08-01 13:21:44.119876 superagent_py-0.0.40/src/superagent/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-08-01 13:21:44.119876 superagent_py-0.0.40/src/superagent/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-08-01 13:21:44.119876 superagent_py-0.0.40/src/superagent/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-08-01 13:21:44.119876 superagent_py-0.0.40/src/superagent/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-08-01 13:21:44.119876 superagent_py-0.0.40/src/superagent/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      170 2023-08-01 13:21:44.119876 superagent_py-0.0.40/src/superagent/errors/__init__.py
+-rw-r--r--   0        0        0      313 2023-08-01 13:21:44.119876 superagent_py-0.0.40/src/superagent/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0        0 2023-08-01 13:21:44.119876 superagent_py-0.0.40/src/superagent/py.typed
+-rw-r--r--   0        0        0      361 2023-08-01 13:21:44.119876 superagent_py-0.0.40/src/superagent/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-08-01 13:21:44.119876 superagent_py-0.0.40/src/superagent/resources/agent/__init__.py
+-rw-r--r--   0        0        0    14615 2023-08-01 13:21:44.119876 superagent_py-0.0.40/src/superagent/resources/agent/client.py
+-rw-r--r--   0        0        0       65 2023-08-01 13:21:44.119876 superagent_py-0.0.40/src/superagent/resources/agent_documents/__init__.py
+-rw-r--r--   0        0        0     9260 2023-08-01 13:21:44.119876 superagent_py-0.0.40/src/superagent/resources/agent_documents/client.py
+-rw-r--r--   0        0        0       65 2023-08-01 13:21:44.119876 superagent_py-0.0.40/src/superagent/resources/agent_tools/__init__.py
+-rw-r--r--   0        0        0     9132 2023-08-01 13:21:44.123877 superagent_py-0.0.40/src/superagent/resources/agent_tools/client.py
+-rw-r--r--   0        0        0       65 2023-08-01 13:21:44.123877 superagent_py-0.0.40/src/superagent/resources/api_token/__init__.py
+-rw-r--r--   0        0        0     8538 2023-08-01 13:21:44.123877 superagent_py-0.0.40/src/superagent/resources/api_token/client.py
+-rw-r--r--   0        0        0       65 2023-08-01 13:21:44.123877 superagent_py-0.0.40/src/superagent/resources/auth/__init__.py
+-rw-r--r--   0        0        0     5901 2023-08-01 13:21:44.123877 superagent_py-0.0.40/src/superagent/resources/auth/client.py
+-rw-r--r--   0        0        0       65 2023-08-01 13:21:44.123877 superagent_py-0.0.40/src/superagent/resources/documents/__init__.py
+-rw-r--r--   0        0        0    12664 2023-08-01 13:21:44.123877 superagent_py-0.0.40/src/superagent/resources/documents/client.py
+-rw-r--r--   0        0        0       65 2023-08-01 13:21:44.123877 superagent_py-0.0.40/src/superagent/resources/prompts/__init__.py
+-rw-r--r--   0        0        0    10865 2023-08-01 13:21:44.123877 superagent_py-0.0.40/src/superagent/resources/prompts/client.py
+-rw-r--r--   0        0        0       65 2023-08-01 13:21:44.123877 superagent_py-0.0.40/src/superagent/resources/tags/__init__.py
+-rw-r--r--   0        0        0    10575 2023-08-01 13:21:44.123877 superagent_py-0.0.40/src/superagent/resources/tags/client.py
+-rw-r--r--   0        0        0       65 2023-08-01 13:21:44.123877 superagent_py-0.0.40/src/superagent/resources/tools/__init__.py
+-rw-r--r--   0        0        0    11638 2023-08-01 13:21:44.123877 superagent_py-0.0.40/src/superagent/resources/tools/client.py
+-rw-r--r--   0        0        0       65 2023-08-01 13:21:44.123877 superagent_py-0.0.40/src/superagent/resources/traces/__init__.py
+-rw-r--r--   0        0        0     2236 2023-08-01 13:21:44.123877 superagent_py-0.0.40/src/superagent/resources/traces/client.py
+-rw-r--r--   0        0        0       65 2023-08-01 13:21:44.123877 superagent_py-0.0.40/src/superagent/resources/user/__init__.py
+-rw-r--r--   0        0        0     4328 2023-08-01 13:21:44.123877 superagent_py-0.0.40/src/superagent/resources/user/client.py
+-rw-r--r--   0        0        0      308 2023-08-01 13:21:44.123877 superagent_py-0.0.40/src/superagent/types/__init__.py
+-rw-r--r--   0        0        0      843 2023-08-01 13:21:44.123877 superagent_py-0.0.40/src/superagent/types/http_validation_error.py
+-rw-r--r--   0        0        0      869 2023-08-01 13:21:44.123877 superagent_py-0.0.40/src/superagent/types/validation_error.py
+-rw-r--r--   0        0        0      128 2023-08-01 13:21:44.123877 superagent_py-0.0.40/src/superagent/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0     3762 1970-01-01 00:00:00.000000 superagent_py-0.0.40/PKG-INFO
```

### Comparing `superagent_py-0.0.39/LICENSE` & `superagent_py-0.0.40/LICENSE`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.39/README.md` & `superagent_py-0.0.40/README.md`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.39/src/superagent/__init__.py` & `superagent_py-0.0.40/src/superagent/__init__.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.39/src/superagent/client.py` & `superagent_py-0.0.40/src/superagent/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.39/src/superagent/core/datetime_utils.py` & `superagent_py-0.0.40/src/superagent/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.39/src/superagent/core/jsonable_encoder.py` & `superagent_py-0.0.40/src/superagent/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.39/src/superagent/resources/agent/client.py` & `superagent_py-0.0.40/src/superagent/resources/agent/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,19 +129,26 @@
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def prompt_agent(
-        self, agent_id: str, *, input: typing.Dict[str, typing.Any], has_streaming: typing.Optional[bool] = OMIT
+        self,
+        agent_id: str,
+        *,
+        input: typing.Dict[str, typing.Any],
+        has_streaming: typing.Optional[bool] = OMIT,
+        session: typing.Optional[str] = OMIT,
     ) -> typing.Any:
         _request: typing.Dict[str, typing.Any] = {"input": input}
         if has_streaming is not OMIT:
             _request["has_streaming"] = has_streaming
+        if session is not OMIT:
+            _request["session"] = session
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment}/", f"api/v1/agents/{agent_id}/predict"),
             json=jsonable_encoder(_request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
@@ -275,19 +282,26 @@
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def prompt_agent(
-        self, agent_id: str, *, input: typing.Dict[str, typing.Any], has_streaming: typing.Optional[bool] = OMIT
+        self,
+        agent_id: str,
+        *,
+        input: typing.Dict[str, typing.Any],
+        has_streaming: typing.Optional[bool] = OMIT,
+        session: typing.Optional[str] = OMIT,
     ) -> typing.Any:
         _request: typing.Dict[str, typing.Any] = {"input": input}
         if has_streaming is not OMIT:
             _request["has_streaming"] = has_streaming
+        if session is not OMIT:
+            _request["session"] = session
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment}/", f"api/v1/agents/{agent_id}/predict"),
                 json=jsonable_encoder(_request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
```

### Comparing `superagent_py-0.0.39/src/superagent/resources/agent_documents/client.py` & `superagent_py-0.0.40/src/superagent/resources/agent_documents/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.39/src/superagent/resources/agent_tools/client.py` & `superagent_py-0.0.40/src/superagent/resources/agent_tools/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.39/src/superagent/resources/api_token/client.py` & `superagent_py-0.0.40/src/superagent/resources/api_token/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.39/src/superagent/resources/auth/client.py` & `superagent_py-0.0.40/src/superagent/resources/auth/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.39/src/superagent/resources/documents/client.py` & `superagent_py-0.0.40/src/superagent/resources/documents/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.39/src/superagent/resources/prompts/client.py` & `superagent_py-0.0.40/src/superagent/resources/prompts/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.39/src/superagent/resources/tags/client.py` & `superagent_py-0.0.40/src/superagent/resources/tags/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.39/src/superagent/resources/tools/client.py` & `superagent_py-0.0.40/src/superagent/resources/tools/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.39/src/superagent/resources/traces/client.py` & `superagent_py-0.0.40/src/superagent/resources/traces/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.39/src/superagent/resources/user/client.py` & `superagent_py-0.0.40/src/superagent/resources/user/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.39/src/superagent/types/http_validation_error.py` & `superagent_py-0.0.40/src/superagent/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.39/src/superagent/types/validation_error.py` & `superagent_py-0.0.40/src/superagent/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.39/PKG-INFO` & `superagent_py-0.0.40/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superagent-py
-Version: 0.0.39
+Version: 0.0.40
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```
