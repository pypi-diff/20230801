# Comparing `tmp/kodexa-6.3.35731213329.tar.gz` & `tmp/kodexa-6.3.35731243382.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kodexa-6.3.35731213329.tar", max compression
+gzip compressed data, was "kodexa-6.3.35731243382.tar", max compression
```

## Comparing `kodexa-6.3.35731213329.tar` & `kodexa-6.3.35731243382.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0    11357 2023-08-01 19:52:07.190440 kodexa-6.3.35731213329/LICENSE
--rw-r--r--   0        0        0     2804 2023-08-01 19:52:07.190440 kodexa-6.3.35731213329/README.md
--rw-r--r--   0        0        0      847 2023-08-01 19:52:07.194440 kodexa-6.3.35731213329/kodexa/__init__.py
--rw-r--r--   0        0        0      171 2023-08-01 19:52:07.194440 kodexa-6.3.35731213329/kodexa/assistant/__init__.py
--rw-r--r--   0        0        0    12530 2023-08-01 19:52:07.194440 kodexa-6.3.35731213329/kodexa/assistant/assistant.py
--rw-r--r--   0        0        0      297 2023-08-01 19:52:07.194440 kodexa-6.3.35731213329/kodexa/connectors/__init__.py
--rw-r--r--   0        0        0     7722 2023-08-01 19:52:07.194440 kodexa-6.3.35731213329/kodexa/connectors/connectors.py
--rw-r--r--   0        0        0      720 2023-08-01 19:52:07.194440 kodexa-6.3.35731213329/kodexa/model/__init__.py
--rw-r--r--   0        0        0      906 2023-08-01 19:52:07.194440 kodexa-6.3.35731213329/kodexa/model/base.py
--rw-r--r--   0        0        0    97073 2023-08-01 19:52:07.194440 kodexa-6.3.35731213329/kodexa/model/model.py
--rw-r--r--   0        0        0   118834 2023-08-01 19:52:07.194440 kodexa-6.3.35731213329/kodexa/model/objects.py
--rw-r--r--   0        0        0    38816 2023-08-01 19:52:07.198440 kodexa-6.3.35731213329/kodexa/model/persistence.py
--rw-r--r--   0        0        0      236 2023-08-01 19:52:07.198440 kodexa-6.3.35731213329/kodexa/pipeline/__init__.py
--rw-r--r--   0        0        0    19505 2023-08-01 19:52:07.198440 kodexa-6.3.35731213329/kodexa/pipeline/pipeline.py
--rw-r--r--   0        0        0      216 2023-08-01 19:52:07.198440 kodexa-6.3.35731213329/kodexa/platform/__init__.py
--rw-r--r--   0        0        0   112612 2023-08-01 19:52:07.198440 kodexa-6.3.35731213329/kodexa/platform/client.py
--rw-r--r--   0        0        0    25644 2023-08-01 19:52:07.198440 kodexa-6.3.35731213329/kodexa/platform/kodexa.py
--rw-r--r--   0        0        0      100 2023-08-01 19:52:07.198440 kodexa-6.3.35731213329/kodexa/selectors/__init__.py
--rw-r--r--   0        0        0    13499 2023-08-01 19:52:07.198440 kodexa-6.3.35731213329/kodexa/selectors/ast.py
--rw-r--r--   0        0        0     3698 2023-08-01 19:52:07.198440 kodexa-6.3.35731213329/kodexa/selectors/core.py
--rw-r--r--   0        0        0     3735 2023-08-01 19:52:07.198440 kodexa-6.3.35731213329/kodexa/selectors/lexrules.py
--rw-r--r--   0        0        0     2354 2023-08-01 19:52:07.198440 kodexa-6.3.35731213329/kodexa/selectors/lextab.py
--rw-r--r--   0        0        0       60 2023-08-01 19:52:07.198440 kodexa-6.3.35731213329/kodexa/selectors/lextab.pyi
--rw-r--r--   0        0        0     7054 2023-08-01 19:52:07.198440 kodexa-6.3.35731213329/kodexa/selectors/parserules.py
--rw-r--r--   0        0        0       60 2023-08-01 19:52:07.198440 kodexa-6.3.35731213329/kodexa/selectors/parserules.pyi
--rw-r--r--   0        0        0    21267 2023-08-01 19:52:07.198440 kodexa-6.3.35731213329/kodexa/selectors/parsetab.py
--rw-r--r--   0        0        0       60 2023-08-01 19:52:07.198440 kodexa-6.3.35731213329/kodexa/selectors/parsetab.pyi
--rw-r--r--   0        0        0        0 2023-08-01 19:52:07.198440 kodexa-6.3.35731213329/kodexa/spatial/__init__.py
--rw-r--r--   0        0        0    18991 2023-08-01 19:52:07.198440 kodexa-6.3.35731213329/kodexa/spatial/azure_models.py
--rw-r--r--   0        0        0     2738 2023-08-01 19:52:07.198440 kodexa-6.3.35731213329/kodexa/spatial/bbox_common.py
--rw-r--r--   0        0        0    34222 2023-08-01 19:52:07.198440 kodexa-6.3.35731213329/kodexa/spatial/table_form_common.py
--rw-r--r--   0        0        0      160 2023-08-01 19:52:07.198440 kodexa-6.3.35731213329/kodexa/steps/__init__.py
--rw-r--r--   0        0        0     9587 2023-08-01 19:52:07.198440 kodexa-6.3.35731213329/kodexa/steps/common.py
--rw-r--r--   0        0        0      159 2023-08-01 19:52:07.198440 kodexa-6.3.35731213329/kodexa/testing/__init__.py
--rw-r--r--   0        0        0      932 2023-08-01 19:52:07.198440 kodexa-6.3.35731213329/kodexa/testing/test_components.py
--rw-r--r--   0        0        0    13596 2023-08-01 19:52:07.198440 kodexa-6.3.35731213329/kodexa/testing/test_utils.py
--rw-r--r--   0        0        0       52 2023-08-01 19:52:07.198440 kodexa-6.3.35731213329/kodexa/training/__init__.py
--rw-r--r--   0        0        0        0 2023-08-01 19:52:07.198440 kodexa-6.3.35731213329/kodexa/training/train_utils.py
--rw-r--r--   0        0        0     1279 2023-08-01 19:52:24.174721 kodexa-6.3.35731213329/pyproject.toml
--rw-r--r--   0        0        0     4068 1970-01-01 00:00:00.000000 kodexa-6.3.35731213329/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-08-01 19:56:17.864668 kodexa-6.3.35731243382/LICENSE
+-rw-r--r--   0        0        0     2804 2023-08-01 19:56:17.864668 kodexa-6.3.35731243382/README.md
+-rw-r--r--   0        0        0      847 2023-08-01 19:56:17.872668 kodexa-6.3.35731243382/kodexa/__init__.py
+-rw-r--r--   0        0        0      171 2023-08-01 19:56:17.872668 kodexa-6.3.35731243382/kodexa/assistant/__init__.py
+-rw-r--r--   0        0        0    12530 2023-08-01 19:56:17.872668 kodexa-6.3.35731243382/kodexa/assistant/assistant.py
+-rw-r--r--   0        0        0      297 2023-08-01 19:56:17.872668 kodexa-6.3.35731243382/kodexa/connectors/__init__.py
+-rw-r--r--   0        0        0     7722 2023-08-01 19:56:17.872668 kodexa-6.3.35731243382/kodexa/connectors/connectors.py
+-rw-r--r--   0        0        0      720 2023-08-01 19:56:17.872668 kodexa-6.3.35731243382/kodexa/model/__init__.py
+-rw-r--r--   0        0        0      906 2023-08-01 19:56:17.872668 kodexa-6.3.35731243382/kodexa/model/base.py
+-rw-r--r--   0        0        0    97073 2023-08-01 19:56:17.872668 kodexa-6.3.35731243382/kodexa/model/model.py
+-rw-r--r--   0        0        0   118834 2023-08-01 19:56:17.872668 kodexa-6.3.35731243382/kodexa/model/objects.py
+-rw-r--r--   0        0        0    38816 2023-08-01 19:56:17.876668 kodexa-6.3.35731243382/kodexa/model/persistence.py
+-rw-r--r--   0        0        0      236 2023-08-01 19:56:17.876668 kodexa-6.3.35731243382/kodexa/pipeline/__init__.py
+-rw-r--r--   0        0        0    19505 2023-08-01 19:56:17.876668 kodexa-6.3.35731243382/kodexa/pipeline/pipeline.py
+-rw-r--r--   0        0        0      216 2023-08-01 19:56:17.876668 kodexa-6.3.35731243382/kodexa/platform/__init__.py
+-rw-r--r--   0        0        0   112700 2023-08-01 19:56:17.876668 kodexa-6.3.35731243382/kodexa/platform/client.py
+-rw-r--r--   0        0        0    25644 2023-08-01 19:56:17.876668 kodexa-6.3.35731243382/kodexa/platform/kodexa.py
+-rw-r--r--   0        0        0      100 2023-08-01 19:56:17.876668 kodexa-6.3.35731243382/kodexa/selectors/__init__.py
+-rw-r--r--   0        0        0    13499 2023-08-01 19:56:17.876668 kodexa-6.3.35731243382/kodexa/selectors/ast.py
+-rw-r--r--   0        0        0     3698 2023-08-01 19:56:17.876668 kodexa-6.3.35731243382/kodexa/selectors/core.py
+-rw-r--r--   0        0        0     3735 2023-08-01 19:56:17.876668 kodexa-6.3.35731243382/kodexa/selectors/lexrules.py
+-rw-r--r--   0        0        0     2354 2023-08-01 19:56:17.876668 kodexa-6.3.35731243382/kodexa/selectors/lextab.py
+-rw-r--r--   0        0        0       60 2023-08-01 19:56:17.876668 kodexa-6.3.35731243382/kodexa/selectors/lextab.pyi
+-rw-r--r--   0        0        0     7054 2023-08-01 19:56:17.876668 kodexa-6.3.35731243382/kodexa/selectors/parserules.py
+-rw-r--r--   0        0        0       60 2023-08-01 19:56:17.876668 kodexa-6.3.35731243382/kodexa/selectors/parserules.pyi
+-rw-r--r--   0        0        0    21267 2023-08-01 19:56:17.876668 kodexa-6.3.35731243382/kodexa/selectors/parsetab.py
+-rw-r--r--   0        0        0       60 2023-08-01 19:56:17.876668 kodexa-6.3.35731243382/kodexa/selectors/parsetab.pyi
+-rw-r--r--   0        0        0        0 2023-08-01 19:56:17.876668 kodexa-6.3.35731243382/kodexa/spatial/__init__.py
+-rw-r--r--   0        0        0    18991 2023-08-01 19:56:17.876668 kodexa-6.3.35731243382/kodexa/spatial/azure_models.py
+-rw-r--r--   0        0        0     2738 2023-08-01 19:56:17.876668 kodexa-6.3.35731243382/kodexa/spatial/bbox_common.py
+-rw-r--r--   0        0        0    34222 2023-08-01 19:56:17.876668 kodexa-6.3.35731243382/kodexa/spatial/table_form_common.py
+-rw-r--r--   0        0        0      160 2023-08-01 19:56:17.876668 kodexa-6.3.35731243382/kodexa/steps/__init__.py
+-rw-r--r--   0        0        0     9587 2023-08-01 19:56:17.876668 kodexa-6.3.35731243382/kodexa/steps/common.py
+-rw-r--r--   0        0        0      159 2023-08-01 19:56:17.876668 kodexa-6.3.35731243382/kodexa/testing/__init__.py
+-rw-r--r--   0        0        0      932 2023-08-01 19:56:17.876668 kodexa-6.3.35731243382/kodexa/testing/test_components.py
+-rw-r--r--   0        0        0    13596 2023-08-01 19:56:17.876668 kodexa-6.3.35731243382/kodexa/testing/test_utils.py
+-rw-r--r--   0        0        0       52 2023-08-01 19:56:17.876668 kodexa-6.3.35731243382/kodexa/training/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-01 19:56:17.876668 kodexa-6.3.35731243382/kodexa/training/train_utils.py
+-rw-r--r--   0        0        0     1279 2023-08-01 19:56:37.228480 kodexa-6.3.35731243382/pyproject.toml
+-rw-r--r--   0        0        0     4068 1970-01-01 00:00:00.000000 kodexa-6.3.35731243382/PKG-INFO
```

### Comparing `kodexa-6.3.35731213329/LICENSE` & `kodexa-6.3.35731243382/LICENSE`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35731213329/README.md` & `kodexa-6.3.35731243382/README.md`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35731213329/kodexa/__init__.py` & `kodexa-6.3.35731243382/kodexa/__init__.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35731213329/kodexa/assistant/assistant.py` & `kodexa-6.3.35731243382/kodexa/assistant/assistant.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35731213329/kodexa/connectors/connectors.py` & `kodexa-6.3.35731243382/kodexa/connectors/connectors.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35731213329/kodexa/model/__init__.py` & `kodexa-6.3.35731243382/kodexa/model/__init__.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35731213329/kodexa/model/base.py` & `kodexa-6.3.35731243382/kodexa/model/base.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35731213329/kodexa/model/model.py` & `kodexa-6.3.35731243382/kodexa/model/model.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35731213329/kodexa/model/objects.py` & `kodexa-6.3.35731243382/kodexa/model/objects.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35731213329/kodexa/model/persistence.py` & `kodexa-6.3.35731243382/kodexa/model/persistence.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35731213329/kodexa/pipeline/pipeline.py` & `kodexa-6.3.35731243382/kodexa/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35731213329/kodexa/platform/client.py` & `kodexa-6.3.35731243382/kodexa/platform/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1505,14 +1505,17 @@
         """Get the type of the endpoint"""
         return "executions"
 
     def cancel(self):
         """Cancel the execution"""
         self.client.put(f'/api/executions/{self.id}/cancel')
 
+    def logs(self):
+        return self.client.get(f'/api/executions/{self.id}/logs')
+
     def wait_for(self, status: str = 'SUCCEEDED', fail_on_statuses=None,
                  timeout: int = 300, follow_child_executions: bool = True) -> List["ExecutionEndpoint"]:
         if fail_on_statuses is None:
             fail_on_statuses = ['FAILED']
 
         logger.info("Waiting for status %s", status)
         start = time.time()
@@ -2722,17 +2725,14 @@
     @property
     def platform(self) -> PlatformOverview:
         return PlatformOverview.model_validate(self.get('/api').json())
 
     def change_password(self, old_password: str, new_password: str):
         return self.post("/api/account/passwordChange", body={"oldPassword": old_password, "newPassword": new_password})
 
-    def reindex(self):
-        self.post("/api/indices/_reindex")
-
     def __build_object(self, ref, object_type_metadata):
         url = f"/api/{object_type_metadata['plural']}/{ref.replace(':', '/')}"
         response = process_response(self.get(url))
 
         # We need to merge the use of the object type metadata
         # and the deserialize method better
 
@@ -2749,14 +2749,16 @@
 
     def get_object_endpoint(self, object_type: str) -> BaseModel:
         pass
 
     def get_platform(self):
         return PlatformOverview.model_validate(self.get(f"{self.base_url}/api").json())
 
+    # The followings methods are helpers for working with requests
+
     def exists(self, url, params=None) -> bool:
         response = requests.get(self.get_url(url), params=params, headers={"x-access-token": self.access_token,
                                                                            "content-type": "application/json"})
         if response.status_code == 200 or response.status_code == 404:
             return response.status_code == 200
         process_response(response)
```

### Comparing `kodexa-6.3.35731213329/kodexa/platform/kodexa.py` & `kodexa-6.3.35731243382/kodexa/platform/kodexa.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35731213329/kodexa/selectors/ast.py` & `kodexa-6.3.35731243382/kodexa/selectors/ast.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35731213329/kodexa/selectors/core.py` & `kodexa-6.3.35731243382/kodexa/selectors/core.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35731213329/kodexa/selectors/lexrules.py` & `kodexa-6.3.35731243382/kodexa/selectors/lexrules.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35731213329/kodexa/selectors/lextab.py` & `kodexa-6.3.35731243382/kodexa/selectors/lextab.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35731213329/kodexa/selectors/parserules.py` & `kodexa-6.3.35731243382/kodexa/selectors/parserules.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35731213329/kodexa/selectors/parsetab.py` & `kodexa-6.3.35731243382/kodexa/selectors/parsetab.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35731213329/kodexa/spatial/azure_models.py` & `kodexa-6.3.35731243382/kodexa/spatial/azure_models.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35731213329/kodexa/spatial/bbox_common.py` & `kodexa-6.3.35731243382/kodexa/spatial/bbox_common.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35731213329/kodexa/spatial/table_form_common.py` & `kodexa-6.3.35731243382/kodexa/spatial/table_form_common.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35731213329/kodexa/steps/common.py` & `kodexa-6.3.35731243382/kodexa/steps/common.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35731213329/kodexa/testing/test_components.py` & `kodexa-6.3.35731243382/kodexa/testing/test_components.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35731213329/kodexa/testing/test_utils.py` & `kodexa-6.3.35731243382/kodexa/testing/test_utils.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35731213329/pyproject.toml` & `kodexa-6.3.35731243382/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kodexa"
-version = "6.3.35731213329"
+version = "6.3.35731243382"
 description = "Python SDK for the Kodexa Platform"
 authors = ["Austin Redenbaugh <austin@kodexa.com>", "Philip Dodds <philip@kodexa.com>", "Romar Cablao <rcablao@kodexa.com>", "Amadea Paula Dodds <amadeapaula@kodexa.com>"]
 readme = "README.md"
 
 packages = [
     { include = "kodexa" }
 ]
```

### Comparing `kodexa-6.3.35731213329/PKG-INFO` & `kodexa-6.3.35731243382/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kodexa
-Version: 6.3.35731213329
+Version: 6.3.35731243382
 Summary: Python SDK for the Kodexa Platform
 Author: Austin Redenbaugh
 Author-email: austin@kodexa.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

