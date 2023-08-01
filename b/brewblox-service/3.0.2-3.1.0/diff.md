# Comparing `tmp/brewblox_service-3.0.2.tar.gz` & `tmp/brewblox_service-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brewblox_service-3.0.2.tar", max compression
+gzip compressed data, was "brewblox_service-3.1.0.tar", max compression
```

## Comparing `brewblox_service-3.0.2.tar` & `brewblox_service-3.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    35140 2023-07-29 11:06:38.889748 brewblox_service-3.0.2/LICENSE.md
--rw-r--r--   0        0        0     3759 2023-07-29 11:06:38.889748 brewblox_service-3.0.2/README.md
--rw-r--r--   0        0        0     1147 2023-07-29 11:06:38.889748 brewblox_service-3.0.2/brewblox_service/__init__.py
--rw-r--r--   0        0        0     1503 2023-07-29 11:06:38.889748 brewblox_service-3.0.2/brewblox_service/cors.py
--rw-r--r--   0        0        0     9701 2023-07-29 11:06:38.889748 brewblox_service-3.0.2/brewblox_service/features.py
--rw-r--r--   0        0        0     1153 2023-07-29 11:06:38.889748 brewblox_service-3.0.2/brewblox_service/http.py
--rw-r--r--   0        0        0      362 2023-07-29 11:06:38.889748 brewblox_service-3.0.2/brewblox_service/models.py
--rw-r--r--   0        0        0    14239 2023-07-29 11:06:38.889748 brewblox_service-3.0.2/brewblox_service/mqtt.py
--rw-r--r--   0        0        0     5382 2023-07-29 11:06:38.889748 brewblox_service-3.0.2/brewblox_service/repeater.py
--rw-r--r--   0        0        0     5687 2023-07-29 11:06:38.889748 brewblox_service-3.0.2/brewblox_service/scheduler.py
--rw-r--r--   0        0        0     7358 2023-07-29 11:06:38.889748 brewblox_service-3.0.2/brewblox_service/service.py
--rw-r--r--   0        0        0     2805 2023-07-29 11:06:38.889748 brewblox_service-3.0.2/brewblox_service/testing.py
--rw-r--r--   0        0        0      681 2023-07-29 11:06:38.889748 brewblox_service-3.0.2/pyproject.toml
--rw-r--r--   0        0        0     4418 1970-01-01 00:00:00.000000 brewblox_service-3.0.2/PKG-INFO
+-rw-r--r--   0        0        0    35140 2023-08-01 10:50:26.727620 brewblox_service-3.1.0/LICENSE.md
+-rw-r--r--   0        0        0     3759 2023-08-01 10:50:26.727620 brewblox_service-3.1.0/README.md
+-rw-r--r--   0        0        0     1147 2023-08-01 10:50:26.727620 brewblox_service-3.1.0/brewblox_service/__init__.py
+-rw-r--r--   0        0        0     1503 2023-08-01 10:50:26.727620 brewblox_service-3.1.0/brewblox_service/cors.py
+-rw-r--r--   0        0        0     9701 2023-08-01 10:50:26.727620 brewblox_service-3.1.0/brewblox_service/features.py
+-rw-r--r--   0        0        0     1153 2023-08-01 10:50:26.727620 brewblox_service-3.1.0/brewblox_service/http.py
+-rw-r--r--   0        0        0      362 2023-08-01 10:50:26.727620 brewblox_service-3.1.0/brewblox_service/models.py
+-rw-r--r--   0        0        0    15460 2023-08-01 10:50:26.727620 brewblox_service-3.1.0/brewblox_service/mqtt.py
+-rw-r--r--   0        0        0     5382 2023-08-01 10:50:26.727620 brewblox_service-3.1.0/brewblox_service/repeater.py
+-rw-r--r--   0        0        0     5687 2023-08-01 10:50:26.727620 brewblox_service-3.1.0/brewblox_service/scheduler.py
+-rw-r--r--   0        0        0     7358 2023-08-01 10:50:26.727620 brewblox_service-3.1.0/brewblox_service/service.py
+-rw-r--r--   0        0        0     2573 2023-08-01 10:50:26.727620 brewblox_service-3.1.0/brewblox_service/testing.py
+-rw-r--r--   0        0        0      681 2023-08-01 10:50:26.727620 brewblox_service-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4418 1970-01-01 00:00:00.000000 brewblox_service-3.1.0/PKG-INFO
```

### Comparing `brewblox_service-3.0.2/LICENSE.md` & `brewblox_service-3.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `brewblox_service-3.0.2/README.md` & `brewblox_service-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `brewblox_service-3.0.2/brewblox_service/__init__.py` & `brewblox_service-3.1.0/brewblox_service/__init__.py`

 * *Files identical despite different names*

### Comparing `brewblox_service-3.0.2/brewblox_service/cors.py` & `brewblox_service-3.1.0/brewblox_service/cors.py`

 * *Files identical despite different names*

### Comparing `brewblox_service-3.0.2/brewblox_service/features.py` & `brewblox_service-3.1.0/brewblox_service/features.py`

 * *Files identical despite different names*

### Comparing `brewblox_service-3.0.2/brewblox_service/http.py` & `brewblox_service-3.1.0/brewblox_service/http.py`

 * *Files identical despite different names*

### Comparing `brewblox_service-3.0.2/brewblox_service/mqtt.py` & `brewblox_service-3.1.0/brewblox_service/mqtt.py`

 * *Files 13% similar despite different names*

```diff
@@ -57,16 +57,17 @@
 
 @dataclass
 class MQTTConfig:
     protocol: str
     host: str
     port: int
     path: str
-    client_will: Optional[dict] = None
+    client_will: Optional[Will] = None
     transport: str = field(init=False)
+    tls_params: Optional[TLSParameters] = field(init=False)
 
     def __post_init__(self):
         if self.protocol not in ['ws', 'wss', 'mqtt', 'mqtts']:
             raise ValueError(f'Invalid protocol: {self.protocol}')
 
         if self.protocol.startswith('ws'):
             self.transport = 'websockets'
@@ -74,41 +75,35 @@
         else:
             self.transport = 'tcp'
             self.path = ''
 
         if not self.port:
             self.port = DEFAULT_PORTS[self.protocol]
 
+        if self.protocol in ['mqtts', 'wss']:
+            self.tls_params = TLSParameters(cert_reqs=CERT_NONE)
+        else:
+            self.tls_params = None
+
     def __str__(self):
         return f'{self.protocol}://{self.host}:{self.port}{self.path}'
 
+    def make_client(self) -> Client:
+        client = Client(hostname=self.host,
+                        port=self.port,
+                        transport=self.transport,
+                        websocket_path=self.path,
+                        tls_params=self.tls_params,
+                        will=self.client_will,
+                        logger=MQTT_LOGGER)
 
-def _make_client(config: MQTTConfig) -> Client:
-    secure_protocol = config.protocol in ['mqtts', 'wss']
-    tls_params = None
-    will = None
-
-    if secure_protocol:
-        tls_params = TLSParameters(cert_reqs=CERT_NONE)
-
-    if config.client_will:
-        will = Will(**config.client_will)
-
-    client = Client(hostname=config.host,
-                    port=config.port,
-                    transport=config.transport,
-                    websocket_path=config.path,
-                    tls_params=tls_params,
-                    will=will,
-                    logger=MQTT_LOGGER)
+        if self.tls_params:
+            client._client.tls_insecure_set(True)
 
-    if secure_protocol:
-        client._client.tls_insecure_set(True)
-
-    return client
+        return client
 
 
 class EventHandler(repeater.RepeaterFeature):
     """
     Connection handler class for MQTT events.
     Handles both TCP and Websocket connections.
 
@@ -154,57 +149,50 @@
             Examples: (formatted as <protocol>://<host>:<port><path>)
                 ws://eventbus:15675/eventbus
                 wss://BREWBLOX_HOST:443/eventbus
     """
 
     def __init__(self,
                  app: web.Application,
-                 protocol: models.MqttProtocol = None,
-                 host: str = None,
-                 port: int = None,
-                 path: str = None,
+                 protocol: Optional[models.MqttProtocol] = None,
+                 host: Optional[str] = None,
+                 port: Optional[int] = None,
+                 path: Optional[str] = None,
+                 client_will: Optional[Will] = None,
+                 publish_will_before_shutdown: bool = True,
                  **kwargs):
         super().__init__(app, **kwargs)
 
         config: models.BaseServiceConfig = app['config']
-        protocol = protocol or config.mqtt_protocol
-        host = host or config.mqtt_host
-        port = port or config.mqtt_port
-        path = path or config.mqtt_path
-        self.config = MQTTConfig(protocol, host, port, path)
-        self.client: Client = None
+        self.config = MQTTConfig(protocol or config.mqtt_protocol,
+                                 host or config.mqtt_host,
+                                 port or config.mqtt_port,
+                                 path or config.mqtt_path,
+                                 client_will)
+        self.client: Client = self.config.make_client()
 
         self._ready_ev = asyncio.Event()
         self._connect_delay: int = 0
         self._subscribed_topics: list[str] = []
         self._listeners: list[tuple[str, ListenerCallback_]] = []
+        self._publish_will_before_shutdown = publish_will_before_shutdown
 
     def __str__(self):
         return f'<{type(self).__name__} for {self.config}>'
 
     @property
     def ready(self) -> asyncio.Event:
         return self._ready_ev
 
-    def set_client_will(self, topic: str, message: PayloadType, **kwargs):
-        if self.client:
-            raise RuntimeError('Client will must be set before startup')
-        self.config.client_will = dict(topic=topic,
-                                       payload=message,
-                                       **kwargs)
-
     async def _handle_callback(self, cb: ListenerCallback_, message: Message):
         try:
             await cb(str(message.topic), decoded(message.payload))
         except Exception as ex:
             LOGGER.error(f'Exception handling MQTT callback for {message.topic}: {strex(ex)}')
 
-    async def startup(self, app: web.Application):
-        self.client = _make_client(self.config)
-
     async def run(self):
         await asyncio.sleep(self._connect_delay)
         self._connect_delay = RECONNECT_INTERVAL_S
 
         try:
             async with self.client:
                 async with self.client.messages() as messages:
@@ -214,37 +202,45 @@
 
                     LOGGER.debug(f'{self} is ready')
                     self._ready_ev.set()
 
                     async for message in messages:  # pragma: no cover
                         matching = [cb
                                     for (topic, cb) in self._listeners
-                                    if message.topic.matches(topic)]
+                                    if message.topic.matches(topic)
+                                    # Workaround for a bug: https://github.com/sbtinstruments/aiomqtt/issues/239
+                                    # TODO(Bob) remove when fixed
+                                    or (topic.endswith('/#') and message.topic.matches(topic[:-2]))]
 
                         for cb in matching:
                             asyncio.create_task(self._handle_callback(cb, message))
 
                         if not matching:
                             LOGGER.debug(f'{self} recv {message}')
 
         finally:
             self._ready_ev.clear()
 
+    async def before_shutdown(self, app: web.Application):
+        if self._publish_will_before_shutdown:
+            with suppress(Exception):
+                await self.client.publish(**vars(self.config.client_will))
+
     async def publish(self,
                       topic: str,
-                      message: PayloadType,
-                      retain=False,
+                      payload: PayloadType,
                       qos=0,
+                      retain=False,
                       err=True,
                       **kwargs):
         try:
             await self.client.publish(topic,
-                                      message,
-                                      retain=retain,
+                                      payload,
                                       qos=qos,
+                                      retain=retain,
                                       timeout=INTERACTION_TIMEOUT_S,
                                       **kwargs)
             LOGGER.debug(f'publish({topic}) -> OK')
         except MqttError as ex:
             LOGGER.debug(f'publish({topic}) -> {strex(ex)}')
             if err:
                 raise ConnectionError(f'Publish error="{strex(ex)}", topic="{topic}"') from ex
@@ -268,80 +264,97 @@
 
     async def unlisten(self, topic: str, callback: ListenerCallback_):
         LOGGER.debug(f'unlisten({topic})')
         with suppress(ValueError):
             self._listeners.remove((topic, callback))
 
 
-def setup(app: web.Application, **kwargs):
+def setup(app: web.Application,
+          protocol: Optional[models.MqttProtocol] = None,
+          host: Optional[str] = None,
+          port: Optional[int] = None,
+          path: Optional[str] = None,
+          client_will: Optional[Will] = None,
+          publish_will_before_shutdown: bool = True,
+          **kwargs):
     """
     Initializes the EventHandler in the app context.
 
     Args:
         app (web.Application):
             The Aiohttp Application object.
-    """
-    features.add(app, EventHandler(app, **kwargs))
+
+        protocol (models.MqttProtocol, optional):
+            Override the connection protocol.
+            If not set, app['config']['mqtt_protocol'] is used.
+
+        host (str, optional):
+            Override the broker host.
+            If not set, app['config']['mqtt_host'] is used.
+
+        port (int, optional):
+            Override the broker port.
+            If not set, app['config']['mqtt_port'] is used.
+
+        path (str, optional):
+            Override the broker path for WS connections.
+            If not set, app['config']['mqtt_path'] is used.
+
+        client_will (Will, optional):
+            Set Last Will and Testament for the MQTT connection.
+
+        publish_will_before_shutdown (bool, optional):
+            If set, the handler will attempt to send `client_will`
+            before a normal shutdown.
+
+    """
+    features.add(app,
+                 EventHandler(app,
+                              protocol=protocol,
+                              host=host,
+                              port=port,
+                              path=path,
+                              client_will=client_will,
+                              publish_will_before_shutdown=publish_will_before_shutdown,
+                              **kwargs))
 
 
 def fget(app: web.Application) -> EventHandler:
     """
     Get registered EventHandler.
     Requires setup(app) to have been called first.
 
     Args:
         app (web.Application):
             The Aiohttp Application object.
     """
     return features.get(app, EventHandler)
 
 
-def set_client_will(app: web.Application,
-                    topic: str,
-                    message: PayloadType = None,
-                    **kwargs):
-    """
-    Set MQTT Last Will and Testament for client.
-    Requires setup(app) to have been called first.
-    Must be called before startup.
-
-    Args:
-        app (web.Application):
-            The Aiohttp Application object.
-
-        topic (str):
-            The MQTT message topic. Cannot include wildcards.
-
-        message (str, bytes, None):
-            The payload that will be published by the broker on our behalf after disconnecting.
-    """
-    fget(app).set_client_will(topic, message, **kwargs)
-
-
 async def publish(app: web.Application,
                   topic: str,
-                  message: PayloadType,
-                  retain=False,
+                  payload: PayloadType,
                   qos=0,
+                  retain=False,
                   err=True,
                   **kwargs):
     """
     Publish a new event message.
 
-    Shortcut for `handler(app).subscribe(topic, message)`.
+    Shortcut for `fget(app).subscribe(topic, message)`.
     Requires setup(app) to have been called first.
 
     Args:
         app (web.Application):
             The Aiohttp Application object.
 
         topic (str):
             The MQTT message topic. Cannot include wildcards.
 
-        message (str, bytes, None):
+        payload (str, bytes, None):
             The message payload.
 
         retain (bool):
             The MQTT retain flag.
             When a new listener subscribes to a topic,
             it is sent the last retained message by the broker.
 
@@ -349,19 +362,19 @@
             The MQTT quality-of-service flag.
             Must be 0, 1, or 2.
 
         err (bool):
             Local flag to determine error handling.
             If set to `False`, no exception is raised when the message could not be published.
     """
-    await fget(app).publish(topic,
-                            message,
-                            retain,
-                            qos,
-                            err,
+    await fget(app).publish(topic=topic,
+                            payload=payload,
+                            qos=qos,
+                            retain=retain,
+                            err=err,
                             **kwargs)
 
 
 async def subscribe(app: web.Application, topic: str):
     """
     Subscribe to event messages.
     Requires setup(app) to have been called first.
```

### Comparing `brewblox_service-3.0.2/brewblox_service/repeater.py` & `brewblox_service-3.1.0/brewblox_service/repeater.py`

 * *Files identical despite different names*

### Comparing `brewblox_service-3.0.2/brewblox_service/scheduler.py` & `brewblox_service-3.1.0/brewblox_service/scheduler.py`

 * *Files identical despite different names*

### Comparing `brewblox_service-3.0.2/brewblox_service/service.py` & `brewblox_service-3.1.0/brewblox_service/service.py`

 * *Files identical despite different names*

### Comparing `brewblox_service-3.0.2/pyproject.toml` & `brewblox_service-3.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "brewblox-service"
-version = "3.0.2"
+version = "3.1.0"
 description = "Scaffolding for Brewblox backend services"
 authors = ["BrewPi <development@brewpi.com>"]
 license = "GPL-3.0"
 readme = "README.md"
 
 [tool.pyright]
 include = ["brewblox_service"]
```

### Comparing `brewblox_service-3.0.2/PKG-INFO` & `brewblox_service-3.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brewblox-service
-Version: 3.0.2
+Version: 3.1.0
 Summary: Scaffolding for Brewblox backend services
 License: GPL-3.0
 Author: BrewPi
 Author-email: development@brewpi.com
 Requires-Python: >=3.9,<4
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

