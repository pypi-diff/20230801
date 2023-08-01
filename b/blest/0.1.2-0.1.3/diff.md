# Comparing `tmp/blest-0.1.2.tar.gz` & `tmp/blest-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blest-0.1.2.tar", last modified: Thu Jul 27 15:31:10 2023, max compression
+gzip compressed data, was "blest-0.1.3.tar", last modified: Tue Aug  1 09:11:11 2023, max compression
```

## Comparing `blest-0.1.2.tar` & `blest-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 admin      (501) wheel        (0)        0 2023-07-27 15:31:10.969360 blest-0.1.2/
--rw-r--r--   0 admin      (501) wheel        (0)     1061 2023-06-11 20:34:38.000000 blest-0.1.2/LICENSE
--rw-r--r--   0 admin      (501) wheel        (0)     4631 2023-07-27 15:31:10.968895 blest-0.1.2/PKG-INFO
--rw-r--r--   0 admin      (501) wheel        (0)     3888 2023-07-26 18:32:30.000000 blest-0.1.2/README.md
--rw-r--r--   0 admin      (501) wheel        (0)        0 2023-06-23 04:09:47.000000 blest-0.1.2/__init__.py
-drwxr-xr-x   0 admin      (501) wheel        (0)        0 2023-07-27 15:31:10.968101 blest-0.1.2/blest.egg-info/
--rw-r--r--   0 admin      (501) wheel        (0)     4631 2023-07-27 15:31:10.000000 blest-0.1.2/blest.egg-info/PKG-INFO
--rw-r--r--   0 admin      (501) wheel        (0)      212 2023-07-27 15:31:10.000000 blest-0.1.2/blest.egg-info/SOURCES.txt
--rw-r--r--   0 admin      (501) wheel        (0)        1 2023-07-27 15:31:10.000000 blest-0.1.2/blest.egg-info/dependency_links.txt
--rw-r--r--   0 admin      (501) wheel        (0)        8 2023-07-27 15:31:10.000000 blest-0.1.2/blest.egg-info/requires.txt
--rw-r--r--   0 admin      (501) wheel        (0)        1 2023-07-27 15:31:10.000000 blest-0.1.2/blest.egg-info/top_level.txt
--rw-r--r--   0 admin      (501) wheel        (0)    22313 2023-07-27 15:28:02.000000 blest-0.1.2/blest.py
--rw-r--r--   0 admin      (501) wheel        (0)       38 2023-07-27 15:31:10.969490 blest-0.1.2/setup.cfg
--rw-r--r--   0 admin      (501) wheel        (0)     1001 2023-07-27 15:29:49.000000 blest-0.1.2/setup.py
-drwxr-xr-x   0 admin      (501) wheel        (0)        0 2023-07-27 15:31:10.968465 blest-0.1.2/tests/
--rw-r--r--   0 admin      (501) wheel        (0)     8790 2023-07-26 18:27:14.000000 blest-0.1.2/tests/test_router.py
+drwxr-xr-x   0 admin      (501) wheel        (0)        0 2023-08-01 09:11:11.289599 blest-0.1.3/
+-rw-r--r--   0 admin      (501) wheel        (0)     1061 2023-06-11 20:34:38.000000 blest-0.1.3/LICENSE
+-rw-r--r--   0 admin      (501) wheel        (0)     4071 2023-08-01 09:11:11.289251 blest-0.1.3/PKG-INFO
+-rw-r--r--   0 admin      (501) wheel        (0)     3328 2023-08-01 00:21:56.000000 blest-0.1.3/README.md
+-rw-r--r--   0 admin      (501) wheel        (0)        0 2023-06-23 04:09:47.000000 blest-0.1.3/__init__.py
+drwxr-xr-x   0 admin      (501) wheel        (0)        0 2023-08-01 09:11:11.288110 blest-0.1.3/blest.egg-info/
+-rw-r--r--   0 admin      (501) wheel        (0)     4071 2023-08-01 09:11:11.000000 blest-0.1.3/blest.egg-info/PKG-INFO
+-rw-r--r--   0 admin      (501) wheel        (0)      212 2023-08-01 09:11:11.000000 blest-0.1.3/blest.egg-info/SOURCES.txt
+-rw-r--r--   0 admin      (501) wheel        (0)        1 2023-08-01 09:11:11.000000 blest-0.1.3/blest.egg-info/dependency_links.txt
+-rw-r--r--   0 admin      (501) wheel        (0)        8 2023-08-01 09:11:11.000000 blest-0.1.3/blest.egg-info/requires.txt
+-rw-r--r--   0 admin      (501) wheel        (0)        1 2023-08-01 09:11:11.000000 blest-0.1.3/blest.egg-info/top_level.txt
+-rw-r--r--   0 admin      (501) wheel        (0)    24326 2023-07-31 22:02:10.000000 blest-0.1.3/blest.py
+-rw-r--r--   0 admin      (501) wheel        (0)       38 2023-08-01 09:11:11.289744 blest-0.1.3/setup.cfg
+-rw-r--r--   0 admin      (501) wheel        (0)     1001 2023-08-01 09:10:46.000000 blest-0.1.3/setup.py
+drwxr-xr-x   0 admin      (501) wheel        (0)        0 2023-08-01 09:11:11.288495 blest-0.1.3/tests/
+-rw-r--r--   0 admin      (501) wheel        (0)     8790 2023-07-26 18:27:14.000000 blest-0.1.3/tests/test_router.py
```

### Comparing `blest-0.1.2/LICENSE` & `blest-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `blest-0.1.2/blest.py` & `blest-0.1.3/blest.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,23 +43,23 @@
 import json
 import copy
 import os
 import re
 import time
 import threading
 from datetime import datetime
+from functools import partial
 
 class Router:
 
   def __init__(self, options=None):
     self._middleware = []
     self._afterware = []
-    self._errorhandler = None
-    self._introspection = False
     self._timeout = 5000
+    self._introspection = False
     self.routes = {}
     if options:
       self._timeout = options['timeout'] if options and 'timeout' in options else 5000
       self._introspection = options['introspection'] if options and 'introspection' in options else False
 
   def route(self, route):
     def decorator(handler):
@@ -94,19 +94,14 @@
   def after_request(self):
     def decorator(afterware):
       self._afterware.append(afterware)
     return decorator
   afterware = after_request
   after = after_request
 
-  def errorhandler(self):
-    def decorator(errorhandler):
-      self._errorhandler = errorhandler
-    return decorator
-
   def describe(self, route: str, config: dict):
     if route not in self.routes:
       raise ValueError('Route does not exist')
     elif not isinstance(config, dict):
       raise ValueError('Configuration should be an object')
 
     if 'description' in config:
@@ -187,21 +182,28 @@
   async def handle(self, request, context=None):
     return await handle_request(self.routes, request, context)
 
 
 
 class Blest(Router):
 
-  def __init__(self, router_options=None, server_options=None):
-    self.server_options = server_options
-    super().__init__(router_options)
+  def __init__(self, options=None):
+    self._options = options
+    self._errorhandler = None
+    super().__init__(options)
+
+  def errorhandler(self):
+    def decorator(errorhandler):
+      self._errorhandler = errorhandler
+      print('The @errorhandler() decorator is not currently used')
+    return decorator
 
   def listen(self, **args):
-    request_handler = create_request_handler(self.routes, self._errorhandler)
-    server = create_http_server(request_handler, self.server_options)
+    request_handler = create_request_handler(self.routes)
+    server = create_http_server(request_handler, self._options)
     server(*args)
 
 
 
 def create_http_server(request_handler, options=None):
   if options:
     options_error = validate_server_options(options)
@@ -302,17 +304,75 @@
     self.status = status
     self.code = code
     self.data = data
     super().__init__(self.message)
 
 
 
+class HttpClient:
+  def __init__(self, url, max_batch_size=25, batch_delay=10, headers={}):
+    self._url = url
+    self._max_batch_size = max_batch_size
+    self._batch_delay = batch_delay
+    self._headers = headers
+    self._timer = False
+    self._queue = []
+    self._emitter = EventEmitter()
+
+  async def _delay(self, func, time):
+    await asyncio.sleep(time / 1000)
+    await func()
+
+  async def _process(self):
+    new_queue = self._queue[:self._max_batch_size]
+    del self._queue[:self._max_batch_size]
+    if len(self._queue) == 0:
+      self._timer = False
+    else:
+      self._timer = True
+      asyncio.create_task(self._delay(self._process, self._batch_delay))
+    async with aiohttp.ClientSession() as session:
+      try:
+        response = await session.post(self._url, json=new_queue, headers=self._headers.update({'Accept': 'application/json', 'Content-Type': 'application/json'}))
+        response.raise_for_status()
+        response_json = await response.json()
+        for r in response_json:
+          self._emitter.emit(r[0], r[2], r[3])
+      except aiohttp.ClientError as e:
+        for q in new_queue:
+          self._emitter.emit(q[0], None, response_json)
+  
+  async def request(self, route, params=None, selector=None):
+    if not route:
+      raise ValueError('Route is required')
+    elif params and not isinstance(params, dict):
+      raise ValueError('Params should be a dict')
+    elif selector and not isinstance(selector, list):
+      raise ValueError('Selector should be a list')
+    id = str(uuid.uuid4())
+    future = asyncio.Future()
+    def callback(result, error):
+      if error:
+        future.set_exception(Exception(error['message']))
+      else:
+        future.set_result(result)
+    self._emitter.once(id, callback)
+    self._queue.append([id, route, params, selector])
+    if self._timer == False:
+      self._timer = True
+      asyncio.create_task(self._delay(self._process, self._batch_delay))
+    result = await future
+    return result
+
+
+
 def create_http_client(url, options=None):
   if options:
     print('The "options" argument is not yet used, but may be used in the future')
+  print('create_http_client is deprecated - use the HttpClient class instead')
   max_batch_size = 100
   queue = []
   timer = None
   emitter = EventEmitter()
   async def process():
     nonlocal queue
     nonlocal timer
@@ -352,15 +412,15 @@
     if not timer:
       timer = asyncio.create_task(process())
     return await future
   return request
 
 
 
-def create_request_handler(routes, error_handler=None):
+def create_request_handler(routes):
   route_keys = list(routes.keys())
   my_routes = {}
 
   for i in range(len(route_keys)):
     key = route_keys[i]
     route_error = validate_route(key)
     if route_error:
@@ -398,15 +458,15 @@
     elif callable(route):
       my_routes[key] = {'handler': [route]}
     
     else:
       raise Exception(f'Route is missing handler: {key}')
 
   async def handler(requests, context={}):
-    return await handle_request(my_routes, requests, context, error_handler)
+    return await handle_request(my_routes, requests, context)
 
   return handler
 
 
 
 route_regex = r"^[a-zA-Z][a-zA-Z0-9_\-\/]*[a-zA-Z0-9]$"
 
@@ -435,17 +495,17 @@
         return 'Sub-routes should be at least two characters long'
     elif re.search(r"^[a-zA-Z0-9_\-]\/", route):
         return 'Sub-routes should be at least two characters long'
     return None
 
 
 
-async def handle_request(routes, requests, context, error_handler=None):
+async def handle_request(routes, requests, context):
   if not requests or not isinstance(requests, list):
-    return handle_error(400, 'Requests should be a list')
+    return handle_error(400, 'Request should be an array')
   unique_ids = []
   promises = []
   for i in range(len(requests)):
     request = requests[i]
     request_length = len(request)
     if not isinstance(request, list):
       return handle_error(400, 'Request item should be an array')
@@ -454,17 +514,17 @@
     parameters = request[2] if len(request) > 2 else None
     selector = request[3] if len(request) > 3 else None
     if not id or not isinstance(id, str):
       return handle_error(400, 'Request item should have an ID')
     if not route or not isinstance(route, str):
       return handle_error(400, 'Request items should have a route')
     if parameters and not isinstance(parameters, dict):
-      return handle_error(400, 'Request item parameters should be a dict')
+      return handle_error(400, 'Request item parameters should be an object')
     if selector and not isinstance(selector, list):
-      return handle_error(400, 'Request item selector should be a list')
+      return handle_error(400, 'Request item selector should be an array')
     if id in unique_ids:
       return handle_error(400, 'Request items should have unique IDs')
     unique_ids.append(id)
     this_route = routes.get(route)
     route_handler = None
     if isinstance(this_route, dict):
       route_handler = this_route.get('handler') or route_not_found
@@ -479,15 +539,15 @@
     my_context = {
       'requestId': id,
       'routeName': route,
       'selector': selector,
       'requestTime': int(datetime.now().timestamp()),
       **(context or {})
     }
-    promises.append(route_reducer(route_handler, request_object, my_context, this_route.get('timeout') if this_route else None, error_handler))
+    promises.append(route_reducer(route_handler, request_object, my_context, this_route.get('timeout') if this_route else None))
   results = await asyncio.gather(*promises)
   return handle_result(results)
 
 
 
 def handle_result(result):
   return result, None
@@ -503,15 +563,15 @@
 
 
 def route_not_found(*args):
   raise BlestError('Not Found', status=404)
 
 
 
-async def route_reducer(handler, request, context, timeout=None, error_handler=None):
+async def route_reducer(handler, request, context, timeout=None):
   
   safe_context = copy.deepcopy(context)
   route = request['route']
   result = None
 
   async def target():
     nonlocal result
```

### Comparing `blest-0.1.2/setup.py` & `blest-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", encoding="utf-8") as readme_file:
     readme = readme_file.read()
 
 setup(
     name="blest",
-    version="0.1.2",
+    version="0.1.3",
     author="JHunt",
     author_email="blest@jhunt.dev",
     description="The Python reference implementation of BLEST (Batch-able, Lightweight, Encrypted State Transfer), an improved communication protocol for web APIs which leverages JSON, supports request batching and selective returns, and provides a modern alternative to REST.",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://blest.jhunt.dev",
     packages=["."],
```

### Comparing `blest-0.1.2/tests/test_router.py` & `blest-0.1.3/tests/test_router.py`

 * *Files identical despite different names*

