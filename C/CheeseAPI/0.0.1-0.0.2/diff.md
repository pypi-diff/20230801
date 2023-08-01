# Comparing `tmp/CheeseAPI-0.0.1.tar.gz` & `tmp/CheeseAPI-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CheeseAPI-0.0.1.tar", last modified: Tue Aug  1 07:17:15 2023, max compression
+gzip compressed data, was "CheeseAPI-0.0.2.tar", last modified: Tue Aug  1 08:13:05 2023, max compression
```

## Comparing `CheeseAPI-0.0.1.tar` & `CheeseAPI-0.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 cheese     (501) staff       (20)        0 2023-08-01 07:17:15.722871 CheeseAPI-0.0.1/
-drwxr-xr-x   0 cheese     (501) staff       (20)        0 2023-08-01 07:17:15.721574 CheeseAPI-0.0.1/CheeseAPI/
--rw-r--r--   0 cheese     (501) staff       (20)      326 2023-08-01 07:10:30.000000 CheeseAPI-0.0.1/CheeseAPI/__init__.py
--rw-r--r--   0 cheese     (501) staff       (20)    20884 2023-08-01 06:26:40.000000 CheeseAPI-0.0.1/CheeseAPI/app.py
--rw-r--r--   0 cheese     (501) staff       (20)     1153 2023-08-01 07:06:19.000000 CheeseAPI-0.0.1/CheeseAPI/cSignal.py
--rw-r--r--   0 cheese     (501) staff       (20)      492 2023-07-31 08:17:28.000000 CheeseAPI-0.0.1/CheeseAPI/exception.py
--rw-r--r--   0 cheese     (501) staff       (20)     2434 2023-08-01 05:36:54.000000 CheeseAPI-0.0.1/CheeseAPI/file.py
--rw-r--r--   0 cheese     (501) staff       (20)     2287 2023-07-31 16:29:49.000000 CheeseAPI-0.0.1/CheeseAPI/module.py
--rw-r--r--   0 cheese     (501) staff       (20)     3674 2023-08-01 06:32:09.000000 CheeseAPI-0.0.1/CheeseAPI/request.py
--rw-r--r--   0 cheese     (501) staff       (20)    12439 2023-08-01 06:39:27.000000 CheeseAPI-0.0.1/CheeseAPI/response.py
--rw-r--r--   0 cheese     (501) staff       (20)     4317 2023-08-01 06:17:09.000000 CheeseAPI-0.0.1/CheeseAPI/route.py
--rw-r--r--   0 cheese     (501) staff       (20)     3525 2023-08-01 05:35:02.000000 CheeseAPI-0.0.1/CheeseAPI/server.py
--rw-r--r--   0 cheese     (501) staff       (20)      676 2023-07-31 08:11:41.000000 CheeseAPI-0.0.1/CheeseAPI/system.py
--rw-r--r--   0 cheese     (501) staff       (20)     1345 2023-08-01 07:01:25.000000 CheeseAPI-0.0.1/CheeseAPI/websocket.py
--rw-r--r--   0 cheese     (501) staff       (20)      295 2023-07-31 08:11:30.000000 CheeseAPI-0.0.1/CheeseAPI/workspace.py
-drwxr-xr-x   0 cheese     (501) staff       (20)        0 2023-08-01 07:17:15.722519 CheeseAPI-0.0.1/CheeseAPI.egg-info/
--rw-r--r--   0 cheese     (501) staff       (20)     7640 2023-08-01 07:17:15.000000 CheeseAPI-0.0.1/CheeseAPI.egg-info/PKG-INFO
--rw-r--r--   0 cheese     (501) staff       (20)      459 2023-08-01 07:17:15.000000 CheeseAPI-0.0.1/CheeseAPI.egg-info/SOURCES.txt
--rw-r--r--   0 cheese     (501) staff       (20)        1 2023-08-01 07:17:15.000000 CheeseAPI-0.0.1/CheeseAPI.egg-info/dependency_links.txt
--rw-r--r--   0 cheese     (501) staff       (20)       49 2023-08-01 07:17:15.000000 CheeseAPI-0.0.1/CheeseAPI.egg-info/requires.txt
--rw-r--r--   0 cheese     (501) staff       (20)       10 2023-08-01 07:17:15.000000 CheeseAPI-0.0.1/CheeseAPI.egg-info/top_level.txt
--rw-r--r--   0 cheese     (501) staff       (20)     1070 2023-07-26 13:50:19.000000 CheeseAPI-0.0.1/LICENSE
--rw-r--r--   0 cheese     (501) staff       (20)     7640 2023-08-01 07:17:15.722730 CheeseAPI-0.0.1/PKG-INFO
--rw-r--r--   0 cheese     (501) staff       (20)     7189 2023-08-01 07:14:47.000000 CheeseAPI-0.0.1/README.md
--rw-r--r--   0 cheese     (501) staff       (20)       38 2023-08-01 07:17:15.722921 CheeseAPI-0.0.1/setup.cfg
--rw-r--r--   0 cheese     (501) staff       (20)      846 2023-07-31 16:33:40.000000 CheeseAPI-0.0.1/setup.py
+drwxr-xr-x   0 cheese     (501) staff       (20)        0 2023-08-01 08:13:05.388426 CheeseAPI-0.0.2/
+drwxr-xr-x   0 cheese     (501) staff       (20)        0 2023-08-01 08:13:05.387276 CheeseAPI-0.0.2/CheeseAPI/
+-rw-r--r--   0 cheese     (501) staff       (20)      255 2023-08-01 08:05:36.000000 CheeseAPI-0.0.2/CheeseAPI/__init__.py
+-rw-r--r--   0 cheese     (501) staff       (20)    21070 2023-08-01 08:10:18.000000 CheeseAPI-0.0.2/CheeseAPI/app.py
+-rw-r--r--   0 cheese     (501) staff       (20)     1153 2023-08-01 07:06:19.000000 CheeseAPI-0.0.2/CheeseAPI/cSignal.py
+-rw-r--r--   0 cheese     (501) staff       (20)      492 2023-07-31 08:17:28.000000 CheeseAPI-0.0.2/CheeseAPI/exception.py
+-rw-r--r--   0 cheese     (501) staff       (20)     2434 2023-08-01 05:36:54.000000 CheeseAPI-0.0.2/CheeseAPI/file.py
+-rw-r--r--   0 cheese     (501) staff       (20)     2287 2023-07-31 16:29:49.000000 CheeseAPI-0.0.2/CheeseAPI/module.py
+-rw-r--r--   0 cheese     (501) staff       (20)     3675 2023-08-01 08:04:57.000000 CheeseAPI-0.0.2/CheeseAPI/request.py
+-rw-r--r--   0 cheese     (501) staff       (20)    12440 2023-08-01 08:05:03.000000 CheeseAPI-0.0.2/CheeseAPI/response.py
+-rw-r--r--   0 cheese     (501) staff       (20)     4317 2023-08-01 06:17:09.000000 CheeseAPI-0.0.2/CheeseAPI/route.py
+-rw-r--r--   0 cheese     (501) staff       (20)     3526 2023-08-01 08:05:19.000000 CheeseAPI-0.0.2/CheeseAPI/server.py
+-rw-r--r--   0 cheese     (501) staff       (20)      676 2023-07-31 08:11:41.000000 CheeseAPI-0.0.2/CheeseAPI/system.py
+-rw-r--r--   0 cheese     (501) staff       (20)     1345 2023-08-01 07:01:25.000000 CheeseAPI-0.0.2/CheeseAPI/websocket.py
+-rw-r--r--   0 cheese     (501) staff       (20)      295 2023-07-31 08:11:30.000000 CheeseAPI-0.0.2/CheeseAPI/workspace.py
+drwxr-xr-x   0 cheese     (501) staff       (20)        0 2023-08-01 08:13:05.387931 CheeseAPI-0.0.2/CheeseAPI.egg-info/
+-rw-r--r--   0 cheese     (501) staff       (20)     7852 2023-08-01 08:13:05.000000 CheeseAPI-0.0.2/CheeseAPI.egg-info/PKG-INFO
+-rw-r--r--   0 cheese     (501) staff       (20)      459 2023-08-01 08:13:05.000000 CheeseAPI-0.0.2/CheeseAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 cheese     (501) staff       (20)        1 2023-08-01 08:13:05.000000 CheeseAPI-0.0.2/CheeseAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 cheese     (501) staff       (20)       57 2023-08-01 08:13:05.000000 CheeseAPI-0.0.2/CheeseAPI.egg-info/requires.txt
+-rw-r--r--   0 cheese     (501) staff       (20)       10 2023-08-01 08:13:05.000000 CheeseAPI-0.0.2/CheeseAPI.egg-info/top_level.txt
+-rw-r--r--   0 cheese     (501) staff       (20)     1070 2023-07-26 13:50:19.000000 CheeseAPI-0.0.2/LICENSE
+-rw-r--r--   0 cheese     (501) staff       (20)     7852 2023-08-01 08:13:05.388221 CheeseAPI-0.0.2/PKG-INFO
+-rw-r--r--   0 cheese     (501) staff       (20)     7401 2023-08-01 07:41:22.000000 CheeseAPI-0.0.2/README.md
+-rw-r--r--   0 cheese     (501) staff       (20)       38 2023-08-01 08:13:05.388475 CheeseAPI-0.0.2/setup.cfg
+-rw-r--r--   0 cheese     (501) staff       (20)      865 2023-08-01 08:12:41.000000 CheeseAPI-0.0.2/setup.py
```

### Comparing `CheeseAPI-0.0.1/CheeseAPI/app.py` & `CheeseAPI-0.0.2/CheeseAPI/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 import os, time, inspect, traceback, multiprocessing
 from typing import Callable, AsyncIterator, Dict, List, Any, Set
 from multiprocessing.process import BaseProcess
 
 import uvicorn, CheeseLog, asyncio
 from CheeseLog import logger, Logger
 
-import exception
-from route import Route, matchPath
-from request import Request
-from response import Response, BaseResponse, FileResponse
-from file import File
-from websocket import websocket
-from module import LocalModule, Module
-from cSignal import signal
+from . import exception
+from .route import Route, matchPath
+from .request import Request
+from .response import Response, BaseResponse, FileResponse
+from .file import File
+from .websocket import websocket
+from .module import LocalModule, Module
+from .cSignal import signal
 
 class App:
     def __init__(self):
-        from system import System
-        from workspace import Workspace
-        from server import Server
+        from .system import System
+        from .workspace import Workspace
+        from .server import Server
 
         self.process: BaseProcess = multiprocessing.current_process()
         self.logger: Logger = logger
 
         self.system: System = System()
         self.workspace: Workspace = Workspace()
         self.server: Server = Server(self)
         self.modules: Set[Module] | Set[str] = set()
         self.localModules: Set[LocalModule] | Set[str] | bool = True
+        self.exclude_localModules: Set[LocalModule] = set()
 
         self.route: Route = Route('')
 
         self.server_startingHandles: List[Callable] = []
         self.server_endingHandles: List[Callable] = []
         # http
         self.http_response404Handles: List[Callable] = []
@@ -41,26 +42,14 @@
         self.http_afterResponseHandles: List[Callable] = []
         # websocket
         self.websocket_beforeConnectionHandles: List[Callable] = []
         self.websocket_afterDisconnectHandles: List[Callable] = []
         self.websocket_errorHandles: List[Callable] = []
         self.websocket_notFoundHandles: List[Callable] = []
 
-        signal.register('server_startingHandle')
-        signal.register('server_endingHandle')
-        signal.register('http_response404Handle')
-        signal.register('http_response405Handle')
-        signal.register('http_response500Handle')
-        signal.register('http_beforeRequestHandle')
-        signal.register('http_afterResponseHandle')
-        signal.register('websocket_beforeConnectionHandle')
-        signal.register('websocket_afterDisconnectHandle')
-        signal.register('websocket_errorHandle')
-        signal.register('websocket_notFoundHandle')
-
         if self.process.name != 'MainProcess':
             self.init()
 
     async def __call__(self, scope, receive, send):
         ''' Server started '''
         if scope['type'] == 'lifespan':
             message = await receive()
@@ -257,37 +246,51 @@
                 for websocket_errorHandle in self.websocket_errorHandles:
                     kwargs['exception'] = e
                     await self.doFunc(websocket_errorHandle, kwargs)
 
     def init(self):
         self.startTimer: float = time.time()
 
+        signal.register('server_startingHandle')
+        signal.register('server_endingHandle')
+        signal.register('http_response404Handle')
+        signal.register('http_response405Handle')
+        signal.register('http_response500Handle')
+        signal.register('http_beforeRequestHandle')
+        signal.register('http_afterResponseHandle')
+        signal.register('websocket_beforeConnectionHandle')
+        signal.register('websocket_afterDisconnectHandle')
+        signal.register('websocket_errorHandle')
+        signal.register('websocket_notFoundHandle')
+
         _modules = set()
         if self.process.name == 'MainProcess' and len(self.modules):
             CheeseLog.starting(f'Modules:\n{" | ".join(self.modules)}')
         for module in self.modules:
             _modules.add(Module(_modules, module))
         self.modules = _modules
 
         if self.localModules is True:
             self.localModules = set()
             for folderName in os.listdir(self.workspace.BASE_PATH):
                 if folderName[0] == '.':
                     continue
+                if folderName in self.exclude_localModules:
+                    continue
                 folderPath = os.path.join(self.workspace.BASE_PATH, folderName)
                 if os.path.isdir(folderPath) and folderPath not in [ self.workspace.BASE_PATH + self.workspace.STATIC_PATH[:-1], self.workspace.BASE_PATH + self.workspace.MEDIA_PATH[:-1], self.workspace.BASE_PATH + self.workspace.LOG_PATH[:-1], self.workspace.BASE_PATH + '/__pycache__' ]:
                     self.localModules.add(folderName)
         if self.process.name == 'MainProcess' and len(self.localModules):
             CheeseLog.starting(f'Local modules:\n{" | ".join(self.localModules)}')
         _localModules = set()
         for module in self.localModules:
             _localModules.add(LocalModule(self.workspace.BASE_PATH, module))
         self.localModules = _localModules
 
-    def run(self):
+    def run(self, applicaiton: str):
         global app
         app = self
 
         CheeseLog.starting(f'Started CheeseAPI master process {os.getpid()}', f'Started CheeseAPI master process \033[34m{os.getpid()}\033[0m')
         CheeseLog.starting('The application starts loading...')
 
         CheeseLog.starting('''System information:
@@ -336,15 +339,15 @@
 
         if signal.receiver('server_startingHandle'):
             signal.send('server_startingHandle')
         for server_startingHandle in self.server_startingHandles:
             server_startingHandle()
 
         uvicorn.run(
-            'app:app',
+            applicaiton,
             host = self.server.HOST,
             port = self.server.PORT,
             reload = self.server.IS_RELOAD,
             workers = self.server.WORKERS,
             log_level = 'critical'
         )
```

### Comparing `CheeseAPI-0.0.1/CheeseAPI/cSignal.py` & `CheeseAPI-0.0.2/CheeseAPI/cSignal.py`

 * *Files identical despite different names*

### Comparing `CheeseAPI-0.0.1/CheeseAPI/file.py` & `CheeseAPI-0.0.2/CheeseAPI/file.py`

 * *Files identical despite different names*

### Comparing `CheeseAPI-0.0.1/CheeseAPI/module.py` & `CheeseAPI-0.0.2/CheeseAPI/module.py`

 * *Files identical despite different names*

### Comparing `CheeseAPI-0.0.1/CheeseAPI/request.py` & `CheeseAPI-0.0.2/CheeseAPI/request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json, traceback, re
 from typing import TypeVar, overload, Dict
 
 import CheeseType.network, xmltodict, CheeseLog
 
-from file import File
+from .file import File
 
 T = TypeVar('T')
 
 class BaseItem:
     def __init__(self):
         self._values: Dict[str, str] = {}
```

### Comparing `CheeseAPI-0.0.1/CheeseAPI/response.py` & `CheeseAPI-0.0.2/CheeseAPI/response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 from typing import Dict, Any
 
-from file import File
+from .file import File
 
 CONTENT_TYPE = {
     'tif': 'image/tiff',
     '001': 'application/x-001',
     '301': 'application/x-301',
     '323': 'text/h323',
     '906': 'application/x-906',
```

### Comparing `CheeseAPI-0.0.1/CheeseAPI/route.py` & `CheeseAPI-0.0.2/CheeseAPI/route.py`

 * *Files identical despite different names*

### Comparing `CheeseAPI-0.0.1/CheeseAPI/server.py` & `CheeseAPI-0.0.2/CheeseAPI/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os, datetime
 
 import CheeseType, CheeseType.network
 
 class Server:
     def __init__(self, app):
-        from app import App
+        from .app import App
 
         self._app: App = app
         self.HOST: CheeseType.network.IPv4 = '127.0.0.1'
         self.PORT: CheeseType.network.Port = 5214
         self._WORKERS: CheeseType.NonNegativeInt = 1
         self.IS_RELOAD: bool = False
```

### Comparing `CheeseAPI-0.0.1/CheeseAPI/system.py` & `CheeseAPI-0.0.2/CheeseAPI/system.py`

 * *Files identical despite different names*

### Comparing `CheeseAPI-0.0.1/CheeseAPI/websocket.py` & `CheeseAPI-0.0.2/CheeseAPI/websocket.py`

 * *Files identical despite different names*

### Comparing `CheeseAPI-0.0.1/CheeseAPI.egg-info/PKG-INFO` & `CheeseAPI-0.0.2/CheeseAPI.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: CheeseAPI
-Version: 0.0.1
+Version: 0.0.2
 Summary: 一款基于uvicorn的web协程框架
 Home-page: https://github.com/CheeseUnknown/CheeseAPI
 Author: Cheese Unknown
 Author-email: cheese@cheese.ren
 License: MIT
 Keywords: api framework backend asyncio
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # **CheeseAPI**
 
+请注意，该文档是最新的beta版，如果你想要查看最新的发布版内容，请查看最新的tag。
+
 ## **介绍**
 
 一款基于uvicorn的web协程框架，目前仍处于开发阶段，一些基础功能已经可以使用。
 
 目前仅保证支持python3.11。
 
 ## **功能**
@@ -280,7 +282,9 @@
 ### 5. **[响应](https://github.com/CheeseUnknown/CheeseAPI/tree/master/documents/response.md)**
 
 ### 6. **[装饰器](https://github.com/CheeseUnknown/CheeseAPI/tree/master/documents/decorator.md)**
 
 ### 7. **[websocket](https://github.com/CheeseUnknown/CheeseAPI/tree/master/documents/websocket.md)**
 
 ### 8. **[信号](https://github.com/CheeseUnknown/CheeseAPI/tree/master/documents/signal.md)**
+
+### 9. **[文件](https://github.com/CheeseUnknown/CheeseAPI/tree/master/documents/file.md)**
```

### Comparing `CheeseAPI-0.0.1/LICENSE` & `CheeseAPI-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `CheeseAPI-0.0.1/PKG-INFO` & `CheeseAPI-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: CheeseAPI
-Version: 0.0.1
+Version: 0.0.2
 Summary: 一款基于uvicorn的web协程框架
 Home-page: https://github.com/CheeseUnknown/CheeseAPI
 Author: Cheese Unknown
 Author-email: cheese@cheese.ren
 License: MIT
 Keywords: api framework backend asyncio
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # **CheeseAPI**
 
+请注意，该文档是最新的beta版，如果你想要查看最新的发布版内容，请查看最新的tag。
+
 ## **介绍**
 
 一款基于uvicorn的web协程框架，目前仍处于开发阶段，一些基础功能已经可以使用。
 
 目前仅保证支持python3.11。
 
 ## **功能**
@@ -280,7 +282,9 @@
 ### 5. **[响应](https://github.com/CheeseUnknown/CheeseAPI/tree/master/documents/response.md)**
 
 ### 6. **[装饰器](https://github.com/CheeseUnknown/CheeseAPI/tree/master/documents/decorator.md)**
 
 ### 7. **[websocket](https://github.com/CheeseUnknown/CheeseAPI/tree/master/documents/websocket.md)**
 
 ### 8. **[信号](https://github.com/CheeseUnknown/CheeseAPI/tree/master/documents/signal.md)**
+
+### 9. **[文件](https://github.com/CheeseUnknown/CheeseAPI/tree/master/documents/file.md)**
```

### Comparing `CheeseAPI-0.0.1/README.md` & `CheeseAPI-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # **CheeseAPI**
 
+请注意，该文档是最新的beta版，如果你想要查看最新的发布版内容，请查看最新的tag。
+
 ## **介绍**
 
 一款基于uvicorn的web协程框架，目前仍处于开发阶段，一些基础功能已经可以使用。
 
 目前仅保证支持python3.11。
 
 ## **功能**
@@ -265,7 +267,9 @@
 ### 5. **[响应](https://github.com/CheeseUnknown/CheeseAPI/tree/master/documents/response.md)**
 
 ### 6. **[装饰器](https://github.com/CheeseUnknown/CheeseAPI/tree/master/documents/decorator.md)**
 
 ### 7. **[websocket](https://github.com/CheeseUnknown/CheeseAPI/tree/master/documents/websocket.md)**
 
 ### 8. **[信号](https://github.com/CheeseUnknown/CheeseAPI/tree/master/documents/signal.md)**
+
+### 9. **[文件](https://github.com/CheeseUnknown/CheeseAPI/tree/master/documents/file.md)**
```

### Comparing `CheeseAPI-0.0.1/setup.py` & `CheeseAPI-0.0.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('./README.md', 'r', encoding = 'utf-8') as f:
     longDescription = f.read()
 
 setuptools.setup(
     name = 'CheeseAPI',
-    version = '0.0.1',
+    version = '0.0.2',
     author = 'Cheese Unknown',
     author_email = 'cheese@cheese.ren',
     description = '一款基于uvicorn的web协程框架',
     long_description = longDescription,
     long_description_content_type = 'text/markdown',
     url = 'https://github.com/CheeseUnknown/CheeseAPI',
     license = 'MIT',
@@ -19,11 +19,12 @@
     ],
     keywords = 'api framework backend asyncio',
     python_requires = '>=3.11',
     install_requires = [
         'uvicorn[standard]',
         'CheeseType',
         'CheeseLog',
-        'xmltodict'
+        'xmltodict',
+        'blinker'
     ],
     packages = setuptools.find_packages()
 )
```

