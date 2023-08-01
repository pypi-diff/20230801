# Comparing `tmp/privateai_client-1.2.0.tar.gz` & `tmp/privateai_client-1.3.0rc1.tar.gz`

## Comparing `privateai_client-1.2.0.tar` & `privateai_client-1.3.0rc1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 privateai_client-1.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 privateai_client-1.2.0/__init__.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 privateai_client-1.2.0/.github/pull-request-template.md
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 privateai_client-1.2.0/.vscode/settings.json
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 privateai_client-1.2.0/src/privateai_client/__init__.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 privateai_client-1.2.0/src/privateai_client/objects.py
--rw-r--r--   0        0        0     5058 2020-02-02 00:00:00.000000 privateai_client-1.2.0/src/privateai_client/pai_client.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 privateai_client-1.2.0/src/privateai_client/components/__init__.py
--rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 privateai_client-1.2.0/src/privateai_client/components/pai_requests.py
--rw-r--r--   0        0        0     3733 2020-02-02 00:00:00.000000 privateai_client-1.2.0/src/privateai_client/components/pai_responses.py
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 privateai_client-1.2.0/src/privateai_client/components/pai_uris.py
--rw-r--r--   0        0        0    23503 2020-02-02 00:00:00.000000 privateai_client-1.2.0/src/privateai_client/components/request_objects.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 privateai_client-1.2.0/src/privateai_client/tests/__init__.py
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 privateai_client-1.2.0/src/privateai_client/tests/test_client.py
--rw-r--r--   0        0        0    39761 2020-02-02 00:00:00.000000 privateai_client-1.2.0/src/privateai_client/tests/test_request_objects.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 privateai_client-1.2.0/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 privateai_client-1.2.0/LICENSE
--rw-r--r--   0        0        0    12896 2020-02-02 00:00:00.000000 privateai_client-1.2.0/README.md
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 privateai_client-1.2.0/pyproject.toml
--rw-r--r--   0        0        0    13527 2020-02-02 00:00:00.000000 privateai_client-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 privateai_client-1.3.0rc1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 privateai_client-1.3.0rc1/__init__.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 privateai_client-1.3.0rc1/.github/pull-request-template.md
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 privateai_client-1.3.0rc1/.vscode/settings.json
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 privateai_client-1.3.0rc1/src/privateai_client/__init__.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 privateai_client-1.3.0rc1/src/privateai_client/objects.py
+-rw-r--r--   0        0        0     5388 2020-02-02 00:00:00.000000 privateai_client-1.3.0rc1/src/privateai_client/pai_client.py
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 privateai_client-1.3.0rc1/src/privateai_client/components/__init__.py
+-rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 privateai_client-1.3.0rc1/src/privateai_client/components/pai_requests.py
+-rw-r--r--   0        0        0     5017 2020-02-02 00:00:00.000000 privateai_client-1.3.0rc1/src/privateai_client/components/pai_responses.py
+-rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 privateai_client-1.3.0rc1/src/privateai_client/components/pai_uris.py
+-rw-r--r--   0        0        0    24972 2020-02-02 00:00:00.000000 privateai_client-1.3.0rc1/src/privateai_client/components/request_objects.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 privateai_client-1.3.0rc1/src/privateai_client/tests/__init__.py
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 privateai_client-1.3.0rc1/src/privateai_client/tests/test_client.py
+-rw-r--r--   0        0        0    41229 2020-02-02 00:00:00.000000 privateai_client-1.3.0rc1/src/privateai_client/tests/test_request_objects.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 privateai_client-1.3.0rc1/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 privateai_client-1.3.0rc1/LICENSE
+-rw-r--r--   0        0        0    12634 2020-02-02 00:00:00.000000 privateai_client-1.3.0rc1/README.md
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 privateai_client-1.3.0rc1/pyproject.toml
+-rw-r--r--   0        0        0    13268 2020-02-02 00:00:00.000000 privateai_client-1.3.0rc1/PKG-INFO
```

### Comparing `privateai_client-1.2.0/.pre-commit-config.yaml` & `privateai_client-1.3.0rc1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `privateai_client-1.2.0/src/privateai_client/objects.py` & `privateai_client-1.3.0rc1/src/privateai_client/objects.py`

 * *Files identical despite different names*

### Comparing `privateai_client-1.2.0/src/privateai_client/pai_client.py` & `privateai_client-1.3.0rc1/src/privateai_client/pai_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,30 @@
 import logging
 from typing import Union
 
+from requests import HTTPError
+
 from .components import *
 
 
 class PAIClient:
     """
     Client used to connect to private-ai's deidentication service
     """
 
-    def __init__(self, scheme: str, host: str, port: str = None, **kwargs):
+    def __init__(
+        self,
+        scheme: str = None,
+        host: str = None,
+        port: str = None,
+        url: str = None,
+        **kwargs,
+    ):
         # Add source url
-        self.uris = PAIURIs(scheme, host, port)
+        self.uris = PAIURIs(url, scheme, host, port)
         self.get = PAIGetRequests(self.uris)
         self.post = PAIPostRequests(self.uris)
         if "api_key" in kwargs.keys():
             self.add_api_key(kwargs["api_key"])
         elif "bearer_token" in kwargs.keys():
             self.add_bearer_token(kwargs["bearer_token"])
 
@@ -28,18 +37,18 @@
         else:
             raise ValueError(
                 f"{auth_type} is not currently a supported method of authorization"
             )
         for subclass in [self.get, self.post]:
             subclass.headers = {**auth_header, **subclass.base_header}
 
-    def add_api_key(self, api_key):
+    def add_api_key(self, api_key: str):
         self._add_auth("api_key", api_key)
 
-    def add_bearer_token(self, token):
+    def add_bearer_token(self, token: str):
         self._add_auth("bearer_token", token)
 
     def ping(self):
         """
         Makes a call to the Private-AI service's health endpoint.
         Can be used as a validator to ensure the service is running.
         """
@@ -55,15 +64,21 @@
         """
         return MetricsResponse(self.get.metrics())
 
     def get_version(self):
         """
         Returns the version of the container application code
         """
-        return VersionResponse(self.get.version)
+        return VersionResponse(self.get.version())
+
+    def get_diagnostics(self):
+        """
+        Returns diagnostic information about the Private-AI container host
+        """
+        return DiagnosticResponse(self.get.diagnostics())
 
     def process_text(self, request_object: Union[dict, ProcessTextRequest]):
         """
         Used to deidentify text
         """
         if type(request_object) is ProcessTextRequest:
             response = TextResponse(self.post.process_text(request_object.to_dict()))
@@ -125,15 +140,15 @@
             raise ValueError(
                 "request_object can only be a dictionary or a ProcessFileBase64Request object"
             )
         return response
 
     def bleep(self, request_object: Union[dict, BleepRequest]):
         """
-        Used to deidentify files by uri
+        Used to deidentify audio files by uri
         """
         if type(request_object) is BleepRequest:
             response = BleepResponse(self.post.bleep(request_object.to_dict()))
         elif type(request_object) is dict:
             response = BleepResponse(self.post.bleep(request_object))
         else:
             raise ValueError(
```

### Comparing `privateai_client-1.2.0/src/privateai_client/components/pai_requests.py` & `privateai_client-1.3.0rc1/src/privateai_client/components/pai_requests.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,17 @@
 
     def make_request(
         self,
         request_type: Union[requests.get, requests.post],
         uri: str,
         payload: dict = None,
     ):
-        return request_type(uri, json=payload, headers=self.headers)
+        response = request_type(uri, json=payload, headers=self.headers)
+        response.raise_for_status()
+        return response
 
 
 class PAIGetRequests(PAIRequests):
     def __init__(self, uris: PAIURIs):
         """
         A class of get requests used by the client
         """
@@ -40,14 +42,17 @@
 
     def metrics(self):
         return self.make_request(self.request_type, self.uris.metrics)
 
     def version(self):
         return self.make_request(self.request_type, self.uris.version)
 
+    def diagnostics(self):
+        return self.make_request(self.request_type, self.uris.diagnostics)
+
 
 class PAIPostRequests(PAIRequests):
     def __init__(self, uris: PAIURIs):
         self.request_type = requests.post
         super(PAIPostRequests, self).__init__(uris)
 
     def process_text(self, request_object):
```

### Comparing `privateai_client-1.2.0/src/privateai_client/components/pai_uris.py` & `privateai_client-1.3.0rc1/src/privateai_client/components/pai_uris.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,27 @@
+import logging
+
+
 class PAIURIs:
-    def __init__(self, scheme, host, port=None):
-        self.valid_schemes = ["http", "https"]
-        scheme = scheme.split("://")[0]
-        if scheme not in self.valid_schemes:
+    def __init__(self, url=None, scheme=None, host=None, port=None, **kwargs):
+        if url:
+            self._pai_uri = url
+        elif scheme and host:
+            self.valid_schemes = ["http", "https"]
+            scheme = scheme.split("://")[0]
+            if scheme not in self.valid_schemes:
+                raise ValueError(
+                    f"Scheme must be one of the following: {', '.join(self.valid_schemes)}"
+                )
+            port = f":{port}" if port else ""
+            self._pai_uri = f"{scheme}://{host}{port}"
+        else:
             raise ValueError(
-                f"Scheme must be one of the following: {', '.join(self.valid_schemes)}"
+                "PAIClient needs either a url, or a scheme and host to initialize"
             )
-        port = f":{port}" if port else ""
-        self._pai_uri = f"{scheme}://{host}{port}"
 
     @property
     def pai_uri(self):
         return self._pai_uri
 
     @property
     def api_version(self):
@@ -26,14 +36,18 @@
         return self._create_uri(self.pai_uri, "healthz")
 
     @property
     def metrics(self):
         return self._create_uri(self.pai_uri, "metrics")
 
     @property
+    def diagnostics(self):
+        return self._create_uri(self.pai_uri, "diagnostics")
+
+    @property
     def process_text(self):
         return self._create_uri(self.pai_uri, self.api_version, "process", "text")
 
     @property
     def process_files_uri(self):
         return self._create_uri(
             self.pai_uri, self.api_version, "process", "files", "uri"
```

### Comparing `privateai_client-1.2.0/src/privateai_client/components/request_objects.py` & `privateai_client-1.3.0rc1/src/privateai_client/components/request_objects.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import inspect
-from typing import List
+from typing import List, Union
 
 
 class BaseRequestObject:
     def to_dict(self):
         dict_obj = dict()
         for key, value in self.__dict__.items():
             name = key if key[0] != "_" else key[1:]
@@ -220,51 +220,99 @@
             return cls._fromdict(values)
         except TypeError:
             raise TypeError("File can only accept the values 'data' and 'content_type'")
 
 
 class FilterSelector(BaseRequestObject):
     valid_types = ["ALLOW", "BLOCK"]
+    default_threshold = 1
 
-    def __init__(self, type: str, pattern: str):
+    def __init__(
+        self,
+        type: str,
+        pattern: str,
+        entity_type: str = None,
+        threshold: Union[int, float] = default_threshold,
+    ):
         if self._type_validator(type):
             self._type = type
         if self._pattern_validator(pattern):
             self._pattern = pattern
+        if self.type == "BLOCK":
+            if self._entity_type_validator(entity_type):
+                self._entity_type = entity_type
+            if self._threshold_validator(threshold):
+                self._threshold = threshold
 
     @property
     def type(self):
         return self._type
 
     @property
     def pattern(self):
         return self._pattern
 
+    @property
+    def entity_type(self):
+        if self.type != "BLOCK":
+            raise AttributeError(
+                f"FilterSelector of type {self.type} does not contain entity_type"
+            )
+        return self._entity_type
+
+    @property
+    def threshold(self):
+        if self.type != "BLOCK":
+            raise AttributeError(
+                f"FilterSelector of type {self.type} does not contain threshold"
+            )
+        return self._threshold
+
     @type.setter
     def type(self, var):
         if self._type_validator(var):
             self._type = var
 
     @pattern.setter
     def pattern(self, var):
         if self._pattern_validator(var):
             self._pattern = var
 
+    @entity_type.setter
+    def entity_type(self, var):
+        if self._entity_type_validator(var):
+            self._entity_type = var
+
+    @threshold.setter
+    def threshold(self, var):
+        if self._threshold_validator(var):
+            self._threshold = var
+
     def _type_validator(self, var):
         if var not in self.valid_types:
             raise ValueError(
                 f"{var} is not valid. FilterSelector.type can only be one of the following: {', '.join(self.valid_types)}"
             )
         return True
 
     def _pattern_validator(self, var):
         if type(var) is not str:
             raise TypeError("FilterSelector.pattern must be of type string")
         return True
 
+    def _entity_type_validator(self, var):
+        if type(var) is not str:
+            raise TypeError("FilterSelector.entity_type must be of type string")
+        return True
+
+    def _threshold_validator(self, var):
+        if var < 0:
+            raise TypeError("FilterSelector.threshold must be greater than 0")
+        return True
+
     @classmethod
     def fromdict(cls, values: dict):
         try:
             return cls._fromdict(values)
         except TypeError:
             raise TypeError(
                 "FilterSelector can only accept the values 'type' and 'pattern'"
```

### Comparing `privateai_client-1.2.0/src/privateai_client/tests/test_request_objects.py` & `privateai_client-1.3.0rc1/src/privateai_client/tests/test_request_objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,27 @@
     test_type = "ALLOW"
     test_pattern = "[A-Z]"
     filter_selector = FilterSelector(type=test_type, pattern=test_pattern)
     assert filter_selector.type == test_type
     assert filter_selector.pattern == test_pattern
 
 
+def test_filter_selector_initializer2():
+    test_type = "BLOCK"
+    test_pattern = "[A-Z]"
+    test_entity_type = "CHARACTER"
+    filter_selector = FilterSelector(
+        type=test_type, pattern=test_pattern, entity_type=test_entity_type
+    )
+    assert filter_selector.type == test_type
+    assert filter_selector.pattern == test_pattern
+    assert filter_selector.entity_type == "CHARACTER"
+    assert filter_selector.threshold == 1
+
+
 def test_filter_selector_initialize_fromdict():
     test_type = "ALLOW"
     test_pattern = "[A-Z]"
     test_dict = {"type": test_type, "pattern": test_pattern}
     filter_selector = FilterSelector.fromdict(test_dict)
     assert filter_selector.type == test_type
     assert filter_selector.pattern == test_pattern
@@ -77,17 +90,21 @@
 
 def test_filter_selector_setters():
     test_type = "ALLOW"
     test_pattern = "[A-Z]"
     filter_selector = FilterSelector(type=test_type, pattern=test_pattern)
     filter_selector.type = "BLOCK"
     filter_selector.pattern = "*1"
+    filter_selector.entity_type = "TEST"
+    filter_selector.threshold = 0.5
 
     assert filter_selector.type == "BLOCK"
     assert filter_selector.pattern == "*1"
+    assert filter_selector.entity_type == "TEST"
+    assert filter_selector.threshold == 0.5
 
 
 def test_filter_selector_type_validator():
     test_type = "JUNK"
     test_pattern = "[A-Z]"
     with pytest.raises(ValueError) as excinfo:
         FilterSelector(type=test_type, pattern=test_pattern)
@@ -101,14 +118,40 @@
     test_type = "ALLOW"
     test_pattern = 12
     with pytest.raises(TypeError) as excinfo:
         FilterSelector(type=test_type, pattern=test_pattern)
     assert "FilterSelector.pattern must be of type string" in str(excinfo.value)
 
 
+def test_filter_selector_entity_type_validator():
+    test_type = "BLOCK"
+    test_pattern = "[A-Z]"
+    test_entity_type = 30
+    with pytest.raises(TypeError) as excinfo:
+        FilterSelector(
+            type=test_type, pattern=test_pattern, entity_type=test_entity_type
+        )
+    assert "FilterSelector.entity_type must be of type string" in str(excinfo.value)
+
+
+def test_filter_selector_entity_type_validator():
+    test_type = "BLOCK"
+    test_pattern = "[A-Z]"
+    test_entity_type = "TEST"
+    test_threshold = -1
+    with pytest.raises(TypeError) as excinfo:
+        FilterSelector(
+            type=test_type,
+            pattern=test_pattern,
+            entity_type=test_entity_type,
+            threshold=test_threshold,
+        )
+    assert "FilterSelector.threshold must be greater than 0" in str(excinfo.value)
+
+
 def test_filter_to_dict():
     test_type = "ALLOW"
     test_pattern = "[A-Z]"
     filter_selector = FilterSelector(type=test_type, pattern=test_pattern)
     filter_dict = filter_selector.to_dict()
     assert filter_dict["type"] == test_type
     assert filter_dict["pattern"] == test_pattern
@@ -613,15 +656,15 @@
 def test_process_text_request_initialize_fromdict():
     request_obj = {
         "text": ["hey!"],
         "link_batch": False,
         "entity_detection": {
             "accuracy": "standard",
             "entity_types": [{"type": "DISABLE", "value": ["LOCATION"]}],
-            "filter": [{"type": "BLOCK", "pattern": "Roger"}],
+            "filter": [{"type": "BLOCK", "pattern": "Roger", "entity_type": "TEST"}],
             "return_entity": False,
         },
         "processed_text": {"type": "MARKER", "pattern": "ALL_ENTITY_TYPES"},
     }
     process_text_request = ProcessTextRequest.fromdict(request_obj)
     assert process_text_request.text == request_obj["text"]
     assert process_text_request.link_batch == request_obj["link_batch"]
```

### Comparing `privateai_client-1.2.0/LICENSE` & `privateai_client-1.3.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `privateai_client-1.2.0/README.md` & `privateai_client-1.3.0rc1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: privateai_client
+Version: 1.3.0rc1
+Summary: A thin client for communicating with the Private AI de-identication API.
+Project-URL: Homepage, https://github.com/privateai/pai-thin-client/
+Project-URL: Bug Tracker, https://github.com/privateai/pai-thin-client/issues
+Author-email: Adam Guiducci <adam.guiducci@private-ai.com>, Bryan Bell-Smith <bryan.bellsmith@private-ai.com>
+License-File: LICENSE
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+
 # Private AI Python Client
 
 A Python client library for communicating with the Private AI API. This document provides information about how to best use the client. For more information, see Private AI's [API Documentation.][1]
 
 ### Quick Links
 
 1. [Installation](#installation)
@@ -20,19 +34,17 @@
 ### Quick Start <a name=quick-start></a>
 
 ```python
 
 from privateai_client import PAIClient
 from privateai_client import request_objects
 
-scheme = "http"
-host = "localhost"
-port = "8080"
+url="http://localhost:8080"
 
-client = PAIClient(scheme=scheme, host=host, port=port)
+client = PAIClient(url="http://localhost:8080")
 text_request = request_objects.process_text_obj(text=["My sample name is John Smith"])
 response = client.process_text(text_request)
 
 print(text_request.text)
 print(response.processed_text)
 
 
@@ -58,59 +70,77 @@
 
 Alternatively, you can run automatically run all tests from the Testing window in Visual Studio Code.
 
 ### Working With The Client <a name=client></a>
 
 #### Initializing the Client
 
-The PAI client requires a scheme, host and optional port to initialize.
+The PAI client requires a scheme, host, and optional port to initialize. 
+Alternatively, a full url can be used.
 Once created, the connection can be tested with the client's `ping` function
 
 ```python
-from privateai_client import PAIClient
 scheme = 'http'
 host = 'localhost'
-port = '8080'
+port= '8080'
 client = PAIClient(scheme, host, port)
 
 client.ping()
+
+
+url = "http://localhost:8080"
+client = PAIClient(url=url)
+
+client.ping()
 ```
 
 Output:
 
 ```
 True
+True
 ```
 
 #### Adding Authorization to the Client
 
 ```python
 from privateai_client import PAIClient
 # On initialization
-client = PAIClient("http", "localhost", "8080", api_key='testkey')
+client = PAIClient(url="http://localhost:8080", api_key='testkey')
 
 # After initialization
-client = PAIClient("http", "localhost", "8080")
+client = PAIClient(url="http://localhost:8080")
+client.ping()
 client.add_api_key("testkey")
+client.ping()
+```
+Output:
+
 ```
+The request returned with a 401 Unauthorized
+True
+```
+
 
 #### Making Requests
 
 Once initialized the client can be used to make any request listed in the [Private-AI documentation][1]
 
 Available requests:
 
-| Client Function        | Endpoint                   |
-| ---------------------- | -------------------------- |
-| `get_version`          | `/`                        |
-| `get_metrics`          | `/metrics`                 |
-| `process_text`         | `/v3/process/text`         |
-| `process_files_uri`    | `/v3/process/files/uri`    |
-| `process_files_base64` | `/v3/process/files/base64` |
-| `bleep`                | `/v3/bleep`                |
+| Client Function          | Endpoint                   |
+| ------------------------ | -------------------------- |
+| `get_version()`          | `/`                        |
+| `ping()`                 | `/healthz`                 |
+| `get_metrics()`          | `/metrics`                 |
+| `get_diagnostics()`      | `/diagnostics`             |
+| `process_text()`         | `/v3/process/text`         |
+| `process_files_uri()`    | `/v3/process/files/uri`    |
+| `process_files_base64()` | `/v3/process/files/base64` |
+| `bleep()`                | `/v3/bleep`                |
 
 Requests can be made using dictionaries:
 
 ```python
 sample_text = ["This is John Smith's sample dictionary request"]
 text_dict_request = {"text": sample_text}
 
@@ -242,24 +272,22 @@
 ```python
 from privateai_client import PAIClient
 from privateai_client.objects import request_objects
 import os
 import logging
 
 file_dir = "/path/to/file/directory"
-client = PAIClient("http", "localhost", "8080")
+client = PAIClient(url="http://localhost:8080")
 for file_name in os.listdir(file_dir):
     filepath = os.path.join(file_dir, file_name)
     if not os.path.isfile(filepath):
         continue
     req_obj = request_objects.file_url_obj(uri=filepath)
     # NOTE this method of file processing requires the container to have an the input and output directories mounted
     resp = client.process_files_uri(req_obj)
-    if not resp.ok:
-        logging.error(f"response for file {file_name} returned with {resp.status_code}")
 ```
 
 #### Processing a Base64 file
 
 ```python
 from privateai_client import PAIClient
 from privateai_client.objects import request_objects
@@ -267,27 +295,25 @@
 import os
 import logging
 
 file_dir = "/path/to/your/file"
 file_name = 'sample_file.pdf'
 filepath = os.path.join(file_dir,file_name)
 file_type= "type/of_file" #eg. application/pdf
-client = PAIClient("http", "localhost", "8080")
+client = PAIClient(url="http://localhost:8080")
 
 # Read from file
 with open(filepath, "rb") as b64_file:
     file_data = base64.b64encode(b64_file.read())
     file_data = file_data.decode("ascii")
 
 # Make the request
 file_obj = request_objects.file_obj(data=file_data, content_type=file_type)
 request_obj = request_objects.file_base64_obj(file=file_obj)
 resp = client.process_files_base64(request_object=request_obj)
-if not resp.ok:
-    logging.error(f"response for file {file_name} returned with {resp.status_code}")
 
 # Write to file
 with open(os.path.join(file_dir,f"redacted-{file_name}"), 'wb') as redacted_file:
     processed_file = resp.processed_file.encode("ascii")
     processed_file = base64.b64decode(processed_file, validate=True)
     redacted_file.write(processed_file)
 ```
@@ -301,15 +327,15 @@
 import os
 import logging
 
 file_dir = "/path/to/your/file"
 file_name = 'sample_file.pdf'
 filepath = os.path.join(file_dir,file_name)
 file_type= "type/of_file" #eg. audio/mp3 or audio/wav
-client = PAIClient("http", "localhost", "8080")
+client = PAIClient(url="http://localhost:8080")
 
 
 file_dir = "/home/adam/workstation/file_processing/test_audio"
 file_name = "test_audio.mp3"
 filepath = os.path.join(file_dir,file_name)
 file_type = "audio/mp3"
 with open(filepath, "rb") as b64_file:
@@ -317,16 +343,14 @@
     file_data = file_data.decode("ascii")
 
 file_obj = request_objects.file_obj(data=file_data, content_type=file_type)
 timestamp = request_objects.timestamp_obj(start=1.12, end=2.14)
 request_obj = request_objects.bleep_obj(file=file_obj, timestamps=[timestamp])
 
 resp = client.bleep(request_object=request_obj)
-if not resp.ok:
-    logging.error(f"response for file {file_name} returned with {resp.status_code}")
 with open(os.path.join(file_dir,f"redacted-{file_name}"), 'wb') as redacted_file:
     processed_file = resp.bleeped_file.encode("ascii")
     processed_file = base64.b64decode(processed_file, validate=True)
     redacted_file.write(processed_file)
 ```
 
 #### Working with structured data
@@ -337,15 +361,15 @@
 
 ```python
 # Working with data frames
 import pandas as pd
 from privateai_client import PAIClient
 from privateai_client.objects import request_objects
 
-client = PAIClient("http", "localhost", "8080")
+client = PAIClient(url="http://localhost:8080")
 data_frame = pd.DataFrame(
     {
         "Name": [
             "Braund, Mr. Owen Harris",
             "Allen, Mr. William Henry",
             "Bonnell, Miss. Elizabeth",
         ],
@@ -371,15 +395,15 @@
 
 ```python
 # Working with data frames
 import pandas as pd
 from privateai_client import PAIClient
 from privateai_client.objects import request_objects
 
-client = PAIClient("http", "localhost", "8080")
+client = PAIClient(url="http://localhost:8080")
 data_frame = pd.DataFrame(
     {
         "Book": [
             "Treasure Island",
             "Moby Dick",
         ],
         "chapter": [1,1],
@@ -395,27 +419,22 @@
 ```
 
 Reidentifying Text
 ```python
 from privateai_client import PAIClient
 from privateai_client import request_objects
 
-client = PAIClient("http", "localhost", "8080")
+client = PAIClient(url="http://localhost:8080")
 
 # Deidentify the text
 initial_text = 'My name is John. I work for Private AI'
 request_obj = request_objects.process_text_obj(text=[initial_text])
 response_obj = client.process_text(request_obj)
 
-# Store the response data
-deidentified_text = response_obj.processed_text
-print(deidentified_text)
-entity_list = [request_objects.entity(row['processed_text'], row['text']) for row in response_obj.entities]
-print([row.to_dict() for row in entity_list])
-
-# # Call the reidentify Route
-request_obj = request_objects.reidentify_text_obj(processed_text=[deidentified_text], entities=entity_list)
-response_obj = client.reidentify_text(request_obj)
-print(response_obj.body)
+# Build reidentify request object from the deidentified response
+new_request_obj = response_obj.get_reidentify_request()
+# Call the reidentify Route
+new_response_obj = client.reidentify_text(new_request_obj)
+print(new_response_obj.body)
 ```
 
 [1]: https://docs.private-ai.com/reference/latest/operation/process_text_v3_process_text_post/
```

### Comparing `privateai_client-1.2.0/pyproject.toml` & `privateai_client-1.3.0rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "privateai_client"
-version = "1.2.0"
+version = "1.3.0rc1"
 authors = [
   { name="Adam Guiducci", email="adam.guiducci@private-ai.com" },
   { name="Bryan Bell-Smith", email="bryan.bellsmith@private-ai.com" },
 ]
 description = "A thin client for communicating with the Private AI de-identication API."
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `privateai_client-1.2.0/PKG-INFO` & `privateai_client-1.3.0rc1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: privateai_client
-Version: 1.2.0
-Summary: A thin client for communicating with the Private AI de-identication API.
-Project-URL: Homepage, https://github.com/privateai/pai-thin-client/
-Project-URL: Bug Tracker, https://github.com/privateai/pai-thin-client/issues
-Author-email: Adam Guiducci <adam.guiducci@private-ai.com>, Bryan Bell-Smith <bryan.bellsmith@private-ai.com>
-License-File: LICENSE
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-
 # Private AI Python Client
 
 A Python client library for communicating with the Private AI API. This document provides information about how to best use the client. For more information, see Private AI's [API Documentation.][1]
 
 ### Quick Links
 
 1. [Installation](#installation)
@@ -34,19 +20,17 @@
 ### Quick Start <a name=quick-start></a>
 
 ```python
 
 from privateai_client import PAIClient
 from privateai_client import request_objects
 
-scheme = "http"
-host = "localhost"
-port = "8080"
+url="http://localhost:8080"
 
-client = PAIClient(scheme=scheme, host=host, port=port)
+client = PAIClient(url="http://localhost:8080")
 text_request = request_objects.process_text_obj(text=["My sample name is John Smith"])
 response = client.process_text(text_request)
 
 print(text_request.text)
 print(response.processed_text)
 
 
@@ -72,59 +56,77 @@
 
 Alternatively, you can run automatically run all tests from the Testing window in Visual Studio Code.
 
 ### Working With The Client <a name=client></a>
 
 #### Initializing the Client
 
-The PAI client requires a scheme, host and optional port to initialize.
+The PAI client requires a scheme, host, and optional port to initialize. 
+Alternatively, a full url can be used.
 Once created, the connection can be tested with the client's `ping` function
 
 ```python
-from privateai_client import PAIClient
 scheme = 'http'
 host = 'localhost'
-port = '8080'
+port= '8080'
 client = PAIClient(scheme, host, port)
 
 client.ping()
+
+
+url = "http://localhost:8080"
+client = PAIClient(url=url)
+
+client.ping()
 ```
 
 Output:
 
 ```
 True
+True
 ```
 
 #### Adding Authorization to the Client
 
 ```python
 from privateai_client import PAIClient
 # On initialization
-client = PAIClient("http", "localhost", "8080", api_key='testkey')
+client = PAIClient(url="http://localhost:8080", api_key='testkey')
 
 # After initialization
-client = PAIClient("http", "localhost", "8080")
+client = PAIClient(url="http://localhost:8080")
+client.ping()
 client.add_api_key("testkey")
+client.ping()
+```
+Output:
+
 ```
+The request returned with a 401 Unauthorized
+True
+```
+
 
 #### Making Requests
 
 Once initialized the client can be used to make any request listed in the [Private-AI documentation][1]
 
 Available requests:
 
-| Client Function        | Endpoint                   |
-| ---------------------- | -------------------------- |
-| `get_version`          | `/`                        |
-| `get_metrics`          | `/metrics`                 |
-| `process_text`         | `/v3/process/text`         |
-| `process_files_uri`    | `/v3/process/files/uri`    |
-| `process_files_base64` | `/v3/process/files/base64` |
-| `bleep`                | `/v3/bleep`                |
+| Client Function          | Endpoint                   |
+| ------------------------ | -------------------------- |
+| `get_version()`          | `/`                        |
+| `ping()`                 | `/healthz`                 |
+| `get_metrics()`          | `/metrics`                 |
+| `get_diagnostics()`      | `/diagnostics`             |
+| `process_text()`         | `/v3/process/text`         |
+| `process_files_uri()`    | `/v3/process/files/uri`    |
+| `process_files_base64()` | `/v3/process/files/base64` |
+| `bleep()`                | `/v3/bleep`                |
 
 Requests can be made using dictionaries:
 
 ```python
 sample_text = ["This is John Smith's sample dictionary request"]
 text_dict_request = {"text": sample_text}
 
@@ -256,24 +258,22 @@
 ```python
 from privateai_client import PAIClient
 from privateai_client.objects import request_objects
 import os
 import logging
 
 file_dir = "/path/to/file/directory"
-client = PAIClient("http", "localhost", "8080")
+client = PAIClient(url="http://localhost:8080")
 for file_name in os.listdir(file_dir):
     filepath = os.path.join(file_dir, file_name)
     if not os.path.isfile(filepath):
         continue
     req_obj = request_objects.file_url_obj(uri=filepath)
     # NOTE this method of file processing requires the container to have an the input and output directories mounted
     resp = client.process_files_uri(req_obj)
-    if not resp.ok:
-        logging.error(f"response for file {file_name} returned with {resp.status_code}")
 ```
 
 #### Processing a Base64 file
 
 ```python
 from privateai_client import PAIClient
 from privateai_client.objects import request_objects
@@ -281,27 +281,25 @@
 import os
 import logging
 
 file_dir = "/path/to/your/file"
 file_name = 'sample_file.pdf'
 filepath = os.path.join(file_dir,file_name)
 file_type= "type/of_file" #eg. application/pdf
-client = PAIClient("http", "localhost", "8080")
+client = PAIClient(url="http://localhost:8080")
 
 # Read from file
 with open(filepath, "rb") as b64_file:
     file_data = base64.b64encode(b64_file.read())
     file_data = file_data.decode("ascii")
 
 # Make the request
 file_obj = request_objects.file_obj(data=file_data, content_type=file_type)
 request_obj = request_objects.file_base64_obj(file=file_obj)
 resp = client.process_files_base64(request_object=request_obj)
-if not resp.ok:
-    logging.error(f"response for file {file_name} returned with {resp.status_code}")
 
 # Write to file
 with open(os.path.join(file_dir,f"redacted-{file_name}"), 'wb') as redacted_file:
     processed_file = resp.processed_file.encode("ascii")
     processed_file = base64.b64decode(processed_file, validate=True)
     redacted_file.write(processed_file)
 ```
@@ -315,15 +313,15 @@
 import os
 import logging
 
 file_dir = "/path/to/your/file"
 file_name = 'sample_file.pdf'
 filepath = os.path.join(file_dir,file_name)
 file_type= "type/of_file" #eg. audio/mp3 or audio/wav
-client = PAIClient("http", "localhost", "8080")
+client = PAIClient(url="http://localhost:8080")
 
 
 file_dir = "/home/adam/workstation/file_processing/test_audio"
 file_name = "test_audio.mp3"
 filepath = os.path.join(file_dir,file_name)
 file_type = "audio/mp3"
 with open(filepath, "rb") as b64_file:
@@ -331,16 +329,14 @@
     file_data = file_data.decode("ascii")
 
 file_obj = request_objects.file_obj(data=file_data, content_type=file_type)
 timestamp = request_objects.timestamp_obj(start=1.12, end=2.14)
 request_obj = request_objects.bleep_obj(file=file_obj, timestamps=[timestamp])
 
 resp = client.bleep(request_object=request_obj)
-if not resp.ok:
-    logging.error(f"response for file {file_name} returned with {resp.status_code}")
 with open(os.path.join(file_dir,f"redacted-{file_name}"), 'wb') as redacted_file:
     processed_file = resp.bleeped_file.encode("ascii")
     processed_file = base64.b64decode(processed_file, validate=True)
     redacted_file.write(processed_file)
 ```
 
 #### Working with structured data
@@ -351,15 +347,15 @@
 
 ```python
 # Working with data frames
 import pandas as pd
 from privateai_client import PAIClient
 from privateai_client.objects import request_objects
 
-client = PAIClient("http", "localhost", "8080")
+client = PAIClient(url="http://localhost:8080")
 data_frame = pd.DataFrame(
     {
         "Name": [
             "Braund, Mr. Owen Harris",
             "Allen, Mr. William Henry",
             "Bonnell, Miss. Elizabeth",
         ],
@@ -385,15 +381,15 @@
 
 ```python
 # Working with data frames
 import pandas as pd
 from privateai_client import PAIClient
 from privateai_client.objects import request_objects
 
-client = PAIClient("http", "localhost", "8080")
+client = PAIClient(url="http://localhost:8080")
 data_frame = pd.DataFrame(
     {
         "Book": [
             "Treasure Island",
             "Moby Dick",
         ],
         "chapter": [1,1],
@@ -409,27 +405,22 @@
 ```
 
 Reidentifying Text
 ```python
 from privateai_client import PAIClient
 from privateai_client import request_objects
 
-client = PAIClient("http", "localhost", "8080")
+client = PAIClient(url="http://localhost:8080")
 
 # Deidentify the text
 initial_text = 'My name is John. I work for Private AI'
 request_obj = request_objects.process_text_obj(text=[initial_text])
 response_obj = client.process_text(request_obj)
 
-# Store the response data
-deidentified_text = response_obj.processed_text
-print(deidentified_text)
-entity_list = [request_objects.entity(row['processed_text'], row['text']) for row in response_obj.entities]
-print([row.to_dict() for row in entity_list])
-
-# # Call the reidentify Route
-request_obj = request_objects.reidentify_text_obj(processed_text=[deidentified_text], entities=entity_list)
-response_obj = client.reidentify_text(request_obj)
-print(response_obj.body)
+# Build reidentify request object from the deidentified response
+new_request_obj = response_obj.get_reidentify_request()
+# Call the reidentify Route
+new_response_obj = client.reidentify_text(new_request_obj)
+print(new_response_obj.body)
 ```
 
 [1]: https://docs.private-ai.com/reference/latest/operation/process_text_v3_process_text_post/
```

