# Comparing `tmp/superagent_py-0.0.38.tar.gz` & `tmp/superagent_py-0.0.39.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superagent_py-0.0.38.tar", max compression
+gzip compressed data, was "superagent_py-0.0.39.tar", max compression
```

## Comparing `superagent_py-0.0.38.tar` & `superagent_py-0.0.39.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1073 2023-07-31 18:33:46.692160 superagent_py-0.0.38/LICENSE
--rw-r--r--   0        0        0     3251 2023-07-31 18:33:46.692160 superagent_py-0.0.38/README.md
--rw-r--r--   0        0        0      380 2023-07-31 18:33:46.692160 superagent_py-0.0.38/pyproject.toml
--rw-r--r--   0        0        0      656 2023-07-31 18:33:46.692160 superagent_py-0.0.38/src/superagent/__init__.py
--rw-r--r--   0        0        0     3186 2023-07-31 18:33:46.692160 superagent_py-0.0.38/src/superagent/client.py
--rw-r--r--   0        0        0      348 2023-07-31 18:33:46.692160 superagent_py-0.0.38/src/superagent/core/__init__.py
--rw-r--r--   0        0        0      426 2023-07-31 18:33:46.692160 superagent_py-0.0.38/src/superagent/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-07-31 18:33:46.696160 superagent_py-0.0.38/src/superagent/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-07-31 18:33:46.696160 superagent_py-0.0.38/src/superagent/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-07-31 18:33:46.696160 superagent_py-0.0.38/src/superagent/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      170 2023-07-31 18:33:46.696160 superagent_py-0.0.38/src/superagent/errors/__init__.py
--rw-r--r--   0        0        0      313 2023-07-31 18:33:46.696160 superagent_py-0.0.38/src/superagent/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0        0 2023-07-31 18:33:46.696160 superagent_py-0.0.38/src/superagent/py.typed
--rw-r--r--   0        0        0      361 2023-07-31 18:33:46.696160 superagent_py-0.0.38/src/superagent/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-07-31 18:33:46.696160 superagent_py-0.0.38/src/superagent/resources/agent/__init__.py
--rw-r--r--   0        0        0    14309 2023-07-31 18:33:46.696160 superagent_py-0.0.38/src/superagent/resources/agent/client.py
--rw-r--r--   0        0        0       65 2023-07-31 18:33:46.696160 superagent_py-0.0.38/src/superagent/resources/agent_documents/__init__.py
--rw-r--r--   0        0        0     9260 2023-07-31 18:33:46.696160 superagent_py-0.0.38/src/superagent/resources/agent_documents/client.py
--rw-r--r--   0        0        0       65 2023-07-31 18:33:46.696160 superagent_py-0.0.38/src/superagent/resources/agent_tools/__init__.py
--rw-r--r--   0        0        0     9132 2023-07-31 18:33:46.696160 superagent_py-0.0.38/src/superagent/resources/agent_tools/client.py
--rw-r--r--   0        0        0       65 2023-07-31 18:33:46.696160 superagent_py-0.0.38/src/superagent/resources/api_token/__init__.py
--rw-r--r--   0        0        0     8538 2023-07-31 18:33:46.696160 superagent_py-0.0.38/src/superagent/resources/api_token/client.py
--rw-r--r--   0        0        0       65 2023-07-31 18:33:46.696160 superagent_py-0.0.38/src/superagent/resources/auth/__init__.py
--rw-r--r--   0        0        0     5901 2023-07-31 18:33:46.696160 superagent_py-0.0.38/src/superagent/resources/auth/client.py
--rw-r--r--   0        0        0       65 2023-07-31 18:33:46.696160 superagent_py-0.0.38/src/superagent/resources/documents/__init__.py
--rw-r--r--   0        0        0    12664 2023-07-31 18:33:46.696160 superagent_py-0.0.38/src/superagent/resources/documents/client.py
--rw-r--r--   0        0        0       65 2023-07-31 18:33:46.696160 superagent_py-0.0.38/src/superagent/resources/prompts/__init__.py
--rw-r--r--   0        0        0    10865 2023-07-31 18:33:46.696160 superagent_py-0.0.38/src/superagent/resources/prompts/client.py
--rw-r--r--   0        0        0       65 2023-07-31 18:33:46.696160 superagent_py-0.0.38/src/superagent/resources/tags/__init__.py
--rw-r--r--   0        0        0    10575 2023-07-31 18:33:46.696160 superagent_py-0.0.38/src/superagent/resources/tags/client.py
--rw-r--r--   0        0        0       65 2023-07-31 18:33:46.696160 superagent_py-0.0.38/src/superagent/resources/tools/__init__.py
--rw-r--r--   0        0        0    11638 2023-07-31 18:33:46.696160 superagent_py-0.0.38/src/superagent/resources/tools/client.py
--rw-r--r--   0        0        0       65 2023-07-31 18:33:46.696160 superagent_py-0.0.38/src/superagent/resources/traces/__init__.py
--rw-r--r--   0        0        0     2236 2023-07-31 18:33:46.696160 superagent_py-0.0.38/src/superagent/resources/traces/client.py
--rw-r--r--   0        0        0       65 2023-07-31 18:33:46.696160 superagent_py-0.0.38/src/superagent/resources/user/__init__.py
--rw-r--r--   0        0        0     4328 2023-07-31 18:33:46.696160 superagent_py-0.0.38/src/superagent/resources/user/client.py
--rw-r--r--   0        0        0      308 2023-07-31 18:33:46.696160 superagent_py-0.0.38/src/superagent/types/__init__.py
--rw-r--r--   0        0        0      843 2023-07-31 18:33:46.696160 superagent_py-0.0.38/src/superagent/types/http_validation_error.py
--rw-r--r--   0        0        0      869 2023-07-31 18:33:46.696160 superagent_py-0.0.38/src/superagent/types/validation_error.py
--rw-r--r--   0        0        0      128 2023-07-31 18:33:46.696160 superagent_py-0.0.38/src/superagent/types/validation_error_loc_item.py
--rw-r--r--   0        0        0     3762 1970-01-01 00:00:00.000000 superagent_py-0.0.38/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-31 23:06:16.440027 superagent_py-0.0.39/LICENSE
+-rw-r--r--   0        0        0     3251 2023-07-31 23:06:16.440027 superagent_py-0.0.39/README.md
+-rw-r--r--   0        0        0      380 2023-07-31 23:06:16.440027 superagent_py-0.0.39/pyproject.toml
+-rw-r--r--   0        0        0      656 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/__init__.py
+-rw-r--r--   0        0        0     3186 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/client.py
+-rw-r--r--   0        0        0      348 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      170 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/errors/__init__.py
+-rw-r--r--   0        0        0      313 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0        0 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/py.typed
+-rw-r--r--   0        0        0      361 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/resources/agent/__init__.py
+-rw-r--r--   0        0        0    14309 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/resources/agent/client.py
+-rw-r--r--   0        0        0       65 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/resources/agent_documents/__init__.py
+-rw-r--r--   0        0        0     9260 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/resources/agent_documents/client.py
+-rw-r--r--   0        0        0       65 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/resources/agent_tools/__init__.py
+-rw-r--r--   0        0        0     9132 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/resources/agent_tools/client.py
+-rw-r--r--   0        0        0       65 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/resources/api_token/__init__.py
+-rw-r--r--   0        0        0     8538 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/resources/api_token/client.py
+-rw-r--r--   0        0        0       65 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/resources/auth/__init__.py
+-rw-r--r--   0        0        0     5901 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/resources/auth/client.py
+-rw-r--r--   0        0        0       65 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/resources/documents/__init__.py
+-rw-r--r--   0        0        0    12664 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/resources/documents/client.py
+-rw-r--r--   0        0        0       65 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/resources/prompts/__init__.py
+-rw-r--r--   0        0        0    10865 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/resources/prompts/client.py
+-rw-r--r--   0        0        0       65 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/resources/tags/__init__.py
+-rw-r--r--   0        0        0    10575 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/resources/tags/client.py
+-rw-r--r--   0        0        0       65 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/resources/tools/__init__.py
+-rw-r--r--   0        0        0    11638 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/resources/tools/client.py
+-rw-r--r--   0        0        0       65 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/resources/traces/__init__.py
+-rw-r--r--   0        0        0     2236 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/resources/traces/client.py
+-rw-r--r--   0        0        0       65 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/resources/user/__init__.py
+-rw-r--r--   0        0        0     4328 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/resources/user/client.py
+-rw-r--r--   0        0        0      308 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/types/__init__.py
+-rw-r--r--   0        0        0      843 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/types/http_validation_error.py
+-rw-r--r--   0        0        0      869 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/types/validation_error.py
+-rw-r--r--   0        0        0      128 2023-07-31 23:06:16.444027 superagent_py-0.0.39/src/superagent/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0     3762 1970-01-01 00:00:00.000000 superagent_py-0.0.39/PKG-INFO
```

### Comparing `superagent_py-0.0.38/LICENSE` & `superagent_py-0.0.39/LICENSE`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.38/README.md` & `superagent_py-0.0.39/README.md`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.38/src/superagent/__init__.py` & `superagent_py-0.0.39/src/superagent/__init__.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.38/src/superagent/client.py` & `superagent_py-0.0.39/src/superagent/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.38/src/superagent/core/datetime_utils.py` & `superagent_py-0.0.39/src/superagent/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.38/src/superagent/core/jsonable_encoder.py` & `superagent_py-0.0.39/src/superagent/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.38/src/superagent/resources/agent/client.py` & `superagent_py-0.0.39/src/superagent/resources/agent/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.38/src/superagent/resources/agent_documents/client.py` & `superagent_py-0.0.39/src/superagent/resources/agent_documents/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.38/src/superagent/resources/agent_tools/client.py` & `superagent_py-0.0.39/src/superagent/resources/agent_tools/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.38/src/superagent/resources/api_token/client.py` & `superagent_py-0.0.39/src/superagent/resources/api_token/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.38/src/superagent/resources/auth/client.py` & `superagent_py-0.0.39/src/superagent/resources/auth/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.38/src/superagent/resources/documents/client.py` & `superagent_py-0.0.39/src/superagent/resources/documents/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.38/src/superagent/resources/prompts/client.py` & `superagent_py-0.0.39/src/superagent/resources/prompts/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.38/src/superagent/resources/tags/client.py` & `superagent_py-0.0.39/src/superagent/resources/tags/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.38/src/superagent/resources/tools/client.py` & `superagent_py-0.0.39/src/superagent/resources/tools/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.38/src/superagent/resources/traces/client.py` & `superagent_py-0.0.39/src/superagent/resources/traces/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.38/src/superagent/resources/user/client.py` & `superagent_py-0.0.39/src/superagent/resources/user/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.38/src/superagent/types/http_validation_error.py` & `superagent_py-0.0.39/src/superagent/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.38/src/superagent/types/validation_error.py` & `superagent_py-0.0.39/src/superagent/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.38/PKG-INFO` & `superagent_py-0.0.39/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superagent-py
-Version: 0.0.38
+Version: 0.0.39
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

