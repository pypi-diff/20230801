# Comparing `tmp/aica_api-0.0.2.tar.gz` & `tmp/aica_api-0.0.3.tar.gz`

## Comparing `aica_api-0.0.2.tar` & `aica_api-0.0.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aica_api-0.0.2/src/aica_api/__init__.py
--rw-r--r--   0        0        0     9054 2020-02-02 00:00:00.000000 aica_api-0.0.2/src/aica_api/client.py
--rw-r--r--   0        0        0     6749 2020-02-02 00:00:00.000000 aica_api-0.0.2/src/aica_api/ws_client.py
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 aica_api-0.0.2/tests/test_api.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 aica_api-0.0.2/tests/test_ws.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 aica_api-0.0.2/.gitignore
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 aica_api-0.0.2/LICENSE
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 aica_api-0.0.2/README.md
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 aica_api-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 aica_api-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aica_api-0.0.3/src/aica_api/__init__.py
+-rw-r--r--   0        0        0     9398 2020-02-02 00:00:00.000000 aica_api-0.0.3/src/aica_api/client.py
+-rw-r--r--   0        0        0     6749 2020-02-02 00:00:00.000000 aica_api-0.0.3/src/aica_api/ws_client.py
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 aica_api-0.0.3/tests/test_api.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 aica_api-0.0.3/tests/test_ws.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 aica_api-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 aica_api-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 aica_api-0.0.3/README.md
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 aica_api-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 aica_api-0.0.3/PKG-INFO
```

### Comparing `aica_api-0.0.2/src/aica_api/client.py` & `aica_api-0.0.3/src/aica_api/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -32,51 +32,53 @@
     def _endpoint(self, endpoint=''):
         """
         Build the request address for a given endpoint.
 
         :param endpoint: The API endpoint
         :return: The constructed request address
         """
-        return f'{self._address}/{endpoint}'
+        return f'{self._address}/v1/{endpoint}'
 
     def _ws_endpoint(self, endpoint=''):
         """
         Build the connection address for a given websocket endpoint.
 
         :param endpoint: The websocket endpoint
         :return: The constructed connection address
         """
-        return f'{self._ws_address}/{endpoint}'
+        return f'{self._ws_address}/v1/{endpoint}'
 
     def check(self) -> requests.Response:
         """
         Make a GET request to the default endpoint to verify connectivity.
         """
         return requests.get(self._endpoint())
 
     def component_descriptions(self) -> requests.Response:
         """
         Retrieve the JSON descriptions of all available components.
         """
-        return requests.get(self._endpoint('component_descriptions'))
+        return requests.get(self._endpoint('components'))
 
     def call_service(self, component_name: str, service_name: str,
-                     payload: Union[None, str] = None) -> requests.Response:
+                     payload: str) -> requests.Response:
         """
         Call a service on a component.
 
         :param component_name: The name of the component
         :param service_name: The name of the service
-        :param payload: The optional service payload, formatted according to the respective service description
+        :param payload: The service payload, formatted according to the respective service description
         """
-        request = {"component_name": component_name, "service_name": service_name}
-        if payload:
-            request["payload"] = payload
-        return requests.post(self._endpoint('call_service'), json=request)
+        endpoint = 'application/components/' + component_name + '/service/' + service_name
+        data = {
+            "payload": payload
+        }
+        return requests.put(self._endpoint(endpoint), json=data)
 
+    # TODO: Missing v1 endpoint
     def init_application(self, auto_load_hardware: bool = True) -> requests.Response:
         """
         Initialize the currently set application.
 
         :param auto_load_hardware: If true, load hardware interfaces automatically when initializing the application.
         """
         return requests.post(self._endpoint('init_application'), json={"auto_load_hardware": auto_load_hardware})
@@ -84,104 +86,119 @@
     def load_component(self, component_name: str) -> requests.Response:
         """
         Load a component in the current application. If the component is already loaded, or if the component is not
         described in the application, nothing happens.
 
         :param component_name: The name of the component to load
         """
-        return requests.post(self._endpoint('load_component'), json={"component_name": component_name})
+        endpoint = 'application/components/' + component_name
+        return requests.put(self._endpoint(endpoint))
 
     def load_controller(self, interface_name: str, controller_name: str) -> requests.Response:
         """
         Load a controller for a given hardware interface. If the controller is already loaded, or if the controller
         is not listed in the hardware interface description, nothing happens.
 
         :param interface_name: The name of the hardware interface
         :param controller_name: The name of the controller to load
         """
-        return requests.post(self._endpoint('load_controller'),
-                             json={"interface_name": interface_name, "controller_name": controller_name})
+        endpoint = 'application/hardware/' + interface_name + '/controller/' + controller_name
+        return requests.put(self._endpoint(endpoint))
 
     def load_hardware(self, interface_name: str) -> requests.Response:
         """
         Load a hardware interface in the current application. If the hardware interface is already loaded, or if the
         interface is not described in the application, nothing happens.
 
         :param interface_name: The name of the hardware interface to load
         """
-        return requests.post(self._endpoint('load_hardware'), json={"interface_name": interface_name})
+        endpoint = 'application/hardware/' + interface_name
+        return requests.put(self._endpoint(endpoint))
 
-    def reset_application(self) -> requests.Response:
+    def pause_application(self) -> requests.Response:
         """
-        Reset the current application, removing all components and hardware interfaces.
+        Pause the current application. This prevents any events from being triggered or handled, but
+        does not pause the periodic execution of active components.
         """
-        return requests.post(self._endpoint('reset_application'))
+        endpoint = 'application/state?action=pause'
+        return requests.put(self._endpoint(endpoint))
 
     def set_application(self, payload: str) -> requests.Response:
         """
         Set an application to be the current application.
 
         :param payload: The filepath of an application on the AICA computer, or the application content as a
         YAML-formatted string
         """
-        return requests.post(self._endpoint('set_application'), json={"payload": payload})
+        data = {
+            "payload": payload
+        }
+        return requests.put(self._endpoint('application'), json=data)
 
     def start_application(self) -> requests.Response:
         """
         Start the AICA application engine.
         """
-        return requests.post(self._endpoint('start_application'))
+        endpoint = 'application/state?action=start'
+        return requests.put(self._endpoint(endpoint))
 
     def stop_application(self) -> requests.Response:
         """
-        Stop the AICA application engine.
+        Stop and reset the AICA application engine, removing all components and hardware interfaces.
         """
-        return requests.post(self._endpoint('stop_application'))
+        endpoint = 'application/state?action=stop'
+        return requests.put(self._endpoint(endpoint))
 
     def switch_controllers(self, interface_name: str, start: Union[None, List[str]] = None,
                            stop: Union[None, List[str]] = None) -> requests.Response:
         """
         Start and stop the controllers for a given hardware interface.
 
         :param interface_name: The name of the hardware interface to unload
         :param start: A list of controllers to start
         :param stop: A list of controllers to stop
         """
-        return requests.post(self._endpoint('call_service'),
-                             json={"interface_name": interface_name, "start": [] if not start else start,
-                                   "stop": [] if not stop else stop})
+        endpoint = 'application/controllers'
+        params = {
+            "interface_name": interface_name,
+            "start": [] if not start else start,
+            "stop": [] if not stop else stop
+        }
+        return requests.put(self._endpoint(endpoint), params=params)
 
     def unload_component(self, component_name: str) -> requests.Response:
         """
         Unload a component in the current application. If the component is not loaded, or if the component is not
         described in the application, nothing happens.
 
         :param component_name: The name of the component to unload
         """
-        return requests.post(self._endpoint('unload_component'), json={"component_name": component_name})
+        endpoint = 'application/components/' + component_name
+        return requests.delete(self._endpoint(endpoint))
 
     def unload_controller(self, interface_name: str, controller_name: str) -> requests.Response:
         """
         Unload a controller for a given hardware interface. If the controller is not loaded, or if the controller
         is not listed in the hardware interface description, nothing happens.
 
         :param interface_name: The name of the hardware interface
         :param controller_name: The name of the controller to unload
         """
-        return requests.post(self._endpoint('load_controller'),
-                             json={"interface_name": interface_name, "controller_name": controller_name})
+        endpoint = 'application/hardware/' + interface_name + '/controller/' + controller_name
+        return requests.delete(self._endpoint(endpoint))
 
     def unload_hardware(self, interface_name: str) -> requests.Response:
         """
         Unload a hardware interface in the current application. If the hardware interface is not loaded, or if the
         interface is not described in the application, nothing happens.
 
         :param interface_name: The name of the hardware interface to unload
         """
-        return requests.post(self._endpoint('unload_hardware'), json={"interface_name": interface_name})
+        endpoint = 'application/hardware/' + interface_name
+        return requests.delete(self._endpoint(endpoint))
 
     def wait_for_predicate(self, component, predicate, timeout: Union[None, int, float] = None):
         """
         Wait until a component predicate is true.
 
         :param component: The name of the component
         :param predicate: The name of the predicate
```

### Comparing `aica_api-0.0.2/src/aica_api/ws_client.py` & `aica_api-0.0.3/src/aica_api/ws_client.py`

 * *Files identical despite different names*

### Comparing `aica_api-0.0.2/LICENSE` & `aica_api-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aica_api-0.0.2/README.md` & `aica_api-0.0.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -9,22 +9,20 @@
 The client can be used to easily make API calls as shown below:
 
 ```python
 from aica_api.client import AICA
 aica = AICA()
 
 aica.set_application('my_application.yaml')
-aica.init_application()
 aica.start_application()
 
 aica.load_component('my_component')
 aica.unload_component('my_component')
 
 aica.stop_application()
-aica.reset_application()
 ```
 
 To check the status of component predicates and conditions, the following blocking methods can be employed:
 
 ```python
 from aica_api.client import AICA
 aica = AICA()
```

### Comparing `aica_api-0.0.2/pyproject.toml` & `aica_api-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "aica_api"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Enrico Eberhard", email="enrico@aica.tech" },
 ]
 description = "A client utility for the AICA API"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `aica_api-0.0.2/PKG-INFO` & `aica_api-0.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aica_api
-Version: 0.0.2
+Version: 0.0.3
 Summary: A client utility for the AICA API
 Project-URL: Homepage, https://github.com/aica-technology/api
 Project-URL: Bug Tracker, https://github.com/aica-technology/api/issues
 Author-email: Enrico Eberhard <enrico@aica.tech>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -25,22 +25,20 @@
 The client can be used to easily make API calls as shown below:
 
 ```python
 from aica_api.client import AICA
 aica = AICA()
 
 aica.set_application('my_application.yaml')
-aica.init_application()
 aica.start_application()
 
 aica.load_component('my_component')
 aica.unload_component('my_component')
 
 aica.stop_application()
-aica.reset_application()
 ```
 
 To check the status of component predicates and conditions, the following blocking methods can be employed:
 
 ```python
 from aica_api.client import AICA
 aica = AICA()
```

