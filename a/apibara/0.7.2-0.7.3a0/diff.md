# Comparing `tmp/apibara-0.7.2.tar.gz` & `tmp/apibara-0.7.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apibara-0.7.2.tar", max compression
+gzip compressed data, was "apibara-0.7.3a0.tar", max compression
```

## Comparing `apibara-0.7.2.tar` & `apibara-0.7.3a0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0    11358 2023-03-31 15:41:14.195812 apibara-0.7.2/LICENSE.txt
--rw-r--r--   0        0        0     1342 2023-03-31 15:41:14.195812 apibara-0.7.2/README.rst
--rw-r--r--   0        0        0     1073 2023-07-17 17:00:35.412895 apibara-0.7.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-31 15:41:14.195812 apibara-0.7.2/src/apibara/__init__.py
--rw-r--r--   0        0        0      514 2023-03-31 15:41:14.195812 apibara-0.7.2/src/apibara/cursor.py
--rw-r--r--   0        0        0      160 2023-04-14 02:19:36.816437 apibara-0.7.2/src/apibara/indexer/__init__.py
--rw-r--r--   0        0        0      375 2023-04-14 02:19:36.816437 apibara-0.7.2/src/apibara/indexer/configuration.py
--rw-r--r--   0        0        0     2393 2023-04-14 02:19:36.816437 apibara-0.7.2/src/apibara/indexer/indexer.py
--rw-r--r--   0        0        0     1026 2023-04-14 02:19:36.816437 apibara-0.7.2/src/apibara/indexer/info.py
--rw-r--r--   0        0        0    11043 2023-07-17 17:00:35.412895 apibara-0.7.2/src/apibara/indexer/runner.py
--rw-r--r--   0        0        0    10502 2023-07-17 15:35:32.998834 apibara-0.7.2/src/apibara/indexer/storage.py
--rw-r--r--   0        0        0      697 2023-07-17 15:49:47.686815 apibara-0.7.2/src/apibara/protocol/__init__.py
--rw-r--r--   0        0        0     3596 2023-07-17 15:49:47.684815 apibara-0.7.2/src/apibara/protocol/client.py
--rw-r--r--   0        0        0        0 2023-03-31 15:41:14.196812 apibara-0.7.2/src/apibara/protocol/proto/__init__.py
--rw-r--r--   0        0        0     3107 2023-03-31 15:41:14.196812 apibara-0.7.2/src/apibara/protocol/proto/stream_pb2.py
--rw-r--r--   0        0        0     9814 2023-03-31 15:41:14.196812 apibara-0.7.2/src/apibara/protocol/proto/stream_pb2.pyi
--rw-r--r--   0        0        0     2517 2023-03-31 15:41:14.196812 apibara-0.7.2/src/apibara/protocol/proto/stream_pb2_grpc.py
--rw-r--r--   0        0        0      878 2023-03-31 15:41:14.196812 apibara-0.7.2/src/apibara/protocol/proto/stream_pb2_grpc.pyi
--rw-r--r--   0        0        0      264 2023-03-31 15:41:14.196812 apibara-0.7.2/src/apibara/starknet/__init__.py
--rw-r--r--   0        0        0     1038 2023-03-31 15:41:14.196812 apibara-0.7.2/src/apibara/starknet/cursor.py
--rw-r--r--   0        0        0     1375 2023-03-31 15:41:14.196812 apibara-0.7.2/src/apibara/starknet/felt.py
--rw-r--r--   0        0        0    14725 2023-03-31 15:41:14.196812 apibara-0.7.2/src/apibara/starknet/filter.py
--rw-r--r--   0        0        0      404 2023-03-31 15:41:14.196812 apibara-0.7.2/src/apibara/starknet/indexer.py
--rw-r--r--   0        0        0        0 2023-03-31 15:41:14.196812 apibara-0.7.2/src/apibara/starknet/proto/__init__.py
--rw-r--r--   0        0        0     7836 2023-07-17 15:35:32.998834 apibara-0.7.2/src/apibara/starknet/proto/filter_pb2.py
--rw-r--r--   0        0        0    12814 2023-07-17 15:35:32.998834 apibara-0.7.2/src/apibara/starknet/proto/filter_pb2.pyi
--rw-r--r--   0        0        0      158 2023-03-31 15:41:14.196812 apibara-0.7.2/src/apibara/starknet/proto/filter_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-03-31 15:41:14.196812 apibara-0.7.2/src/apibara/starknet/proto/filter_pb2_grpc.pyi
--rw-r--r--   0        0        0    11734 2023-07-17 15:49:47.736816 apibara-0.7.2/src/apibara/starknet/proto/starknet_pb2.py
--rw-r--r--   0        0        0    20085 2023-07-17 15:35:32.998834 apibara-0.7.2/src/apibara/starknet/proto/starknet_pb2.pyi
--rw-r--r--   0        0        0      158 2023-03-31 15:41:14.196812 apibara-0.7.2/src/apibara/starknet/proto/starknet_pb2_grpc.py
--rw-r--r--   0        0        0      100 2023-03-31 15:41:14.196812 apibara-0.7.2/src/apibara/starknet/proto/starknet_pb2_grpc.pyi
--rw-r--r--   0        0        0     1096 2023-03-31 15:41:14.196812 apibara-0.7.2/src/apibara/starknet/proto/types_pb2.py
--rw-r--r--   0        0        0      732 2023-03-31 15:41:14.196812 apibara-0.7.2/src/apibara/starknet/proto/types_pb2.pyi
--rw-r--r--   0        0        0      158 2023-03-31 15:41:14.196812 apibara-0.7.2/src/apibara/starknet/proto/types_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-03-31 15:41:14.196812 apibara-0.7.2/src/apibara/starknet/proto/types_pb2_grpc.pyi
--rw-r--r--   0        0        0     2408 1970-01-01 00:00:00.000000 apibara-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-01-15 18:52:09.124336 apibara-0.7.3a0/LICENSE.txt
+-rw-r--r--   0        0        0     1685 2023-07-24 14:46:53.473584 apibara-0.7.3a0/README.rst
+-rw-r--r--   0        0        0     1270 2023-08-01 21:06:19.587210 apibara-0.7.3a0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-01 16:15:25.550565 apibara-0.7.3a0/src/apibara/__init__.py
+-rw-r--r--   0        0        0      514 2023-01-15 18:52:09.124336 apibara-0.7.3a0/src/apibara/cursor.py
+-rw-r--r--   0        0        0      160 2023-01-15 18:52:09.124336 apibara-0.7.3a0/src/apibara/indexer/__init__.py
+-rw-r--r--   0        0        0      375 2023-01-15 18:52:09.124336 apibara-0.7.3a0/src/apibara/indexer/configuration.py
+-rw-r--r--   0        0        0     2393 2023-03-16 21:14:54.127582 apibara-0.7.3a0/src/apibara/indexer/indexer.py
+-rw-r--r--   0        0        0     1026 2023-01-16 18:48:50.663792 apibara-0.7.3a0/src/apibara/indexer/info.py
+-rw-r--r--   0        0        0    12063 2023-08-01 21:01:19.923132 apibara-0.7.3a0/src/apibara/indexer/runner.py
+-rw-r--r--   0        0        0    10502 2023-06-08 12:55:13.026953 apibara-0.7.3a0/src/apibara/indexer/storage.py
+-rw-r--r--   0        0        0      687 2023-07-24 14:46:53.473584 apibara-0.7.3a0/src/apibara/protocol/__init__.py
+-rw-r--r--   0        0        0     4424 2023-08-01 19:15:18.318533 apibara-0.7.3a0/src/apibara/protocol/client.py
+-rw-r--r--   0        0        0        0 2023-01-15 18:52:09.125336 apibara-0.7.3a0/src/apibara/protocol/proto/__init__.py
+-rw-r--r--   0        0        0     3450 2023-08-01 21:01:03.928913 apibara-0.7.3a0/src/apibara/protocol/proto/stream_pb2.py
+-rw-r--r--   0        0        0     3608 2023-08-01 19:15:20.623565 apibara-0.7.3a0/src/apibara/protocol/proto/stream_pb2.pyi
+-rw-r--r--   0        0        0     4147 2023-08-01 21:00:10.094174 apibara-0.7.3a0/src/apibara/protocol/proto/stream_pb2_grpc.py
+-rw-r--r--   0        0        0      878 2023-01-15 18:52:09.125336 apibara-0.7.3a0/src/apibara/protocol/proto/stream_pb2_grpc.pyi
+-rw-r--r--   0        0        0      264 2023-01-15 18:52:09.125336 apibara-0.7.3a0/src/apibara/starknet/__init__.py
+-rw-r--r--   0        0        0     1038 2023-01-15 18:52:09.125336 apibara-0.7.3a0/src/apibara/starknet/cursor.py
+-rw-r--r--   0        0        0     1375 2023-01-15 18:52:09.125336 apibara-0.7.3a0/src/apibara/starknet/felt.py
+-rw-r--r--   0        0        0    14725 2023-03-16 21:14:54.127582 apibara-0.7.3a0/src/apibara/starknet/filter.py
+-rw-r--r--   0        0        0      404 2023-01-15 18:52:09.125336 apibara-0.7.3a0/src/apibara/starknet/indexer.py
+-rw-r--r--   0        0        0        0 2023-01-15 18:52:09.125336 apibara-0.7.3a0/src/apibara/starknet/proto/__init__.py
+-rw-r--r--   0        0        0     8286 2023-08-01 21:01:03.955913 apibara-0.7.3a0/src/apibara/starknet/proto/filter_pb2.py
+-rw-r--r--   0        0        0    12814 2023-08-01 21:00:10.076174 apibara-0.7.3a0/src/apibara/starknet/proto/filter_pb2.pyi
+-rw-r--r--   0        0        0      158 2023-01-15 18:52:09.125336 apibara-0.7.3a0/src/apibara/starknet/proto/filter_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-01-15 18:52:09.125336 apibara-0.7.3a0/src/apibara/starknet/proto/filter_pb2_grpc.pyi
+-rw-r--r--   0        0        0    12370 2023-08-01 21:01:03.974914 apibara-0.7.3a0/src/apibara/starknet/proto/starknet_pb2.py
+-rw-r--r--   0        0        0    20350 2023-08-01 21:00:10.084174 apibara-0.7.3a0/src/apibara/starknet/proto/starknet_pb2.pyi
+-rw-r--r--   0        0        0      158 2023-01-15 18:52:09.125336 apibara-0.7.3a0/src/apibara/starknet/proto/starknet_pb2_grpc.py
+-rw-r--r--   0        0        0      100 2023-01-15 18:52:09.125336 apibara-0.7.3a0/src/apibara/starknet/proto/starknet_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1138 2023-08-01 21:01:03.911913 apibara-0.7.3a0/src/apibara/starknet/proto/types_pb2.py
+-rw-r--r--   0        0        0      732 2023-08-01 19:15:20.609564 apibara-0.7.3a0/src/apibara/starknet/proto/types_pb2.pyi
+-rw-r--r--   0        0        0      158 2023-01-15 18:52:09.125336 apibara-0.7.3a0/src/apibara/starknet/proto/types_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-01-15 18:52:09.125336 apibara-0.7.3a0/src/apibara/starknet/proto/types_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2753 1970-01-01 00:00:00.000000 apibara-0.7.3a0/PKG-INFO
```

### Comparing `apibara-0.7.2/LICENSE.txt` & `apibara-0.7.3a0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `apibara-0.7.2/README.rst` & `apibara-0.7.3a0/README.rst`

 * *Files 27% similar despite different names*

```diff
@@ -5,18 +5,25 @@
     This SDK is alpha software. The API will change drastically until the beta.
 
     `Open an issue on GitHub <https://github.com/apibara/python-sdk>`_ to report bugs or provide feedback.
 
 
 Build web3-powered applications in Python. 
 
+
 Development
 -----------
 
-Install all dependencies with:
+Install the following packages using your OS package manager:
+
+* protobuf
+* poetry
+* docker (for testing)
+
+Install all Python dependencies with:
 
 .. code::
 
     poetry install
 
 Run tests with:
 
@@ -36,18 +43,30 @@
 .. code::
 
     protoc -I=protos/starknet/ \
         --python_out=src/apibara/starknet/proto/ \
         --pyi_out=src/apibara/starknet/proto protos/starknet/*
 
 
+Development (with Nix)
+----------------------
+
+This repository provides a Nix development environment. To use it simply run:
+
+.. code::
+
+   nix develop
+
+All dependencies, including pre-commit hooks, will be installed for you.
+
+
 License
 -------
 
-   Copyright 2022 GNC Labs Limited
+   Copyright 2023 GNC Labs Limited
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `apibara-0.7.2/pyproject.toml` & `apibara-0.7.3a0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "apibara"
-version = "0.7.2"
+version = "0.7.3a0"
 description = "Apibara cliend SDK. Stream and transform on-chain data with Python."
 authors = ["Francesco Ceccon <francesco@apibara.com>"]
 license = "Apache-2.0"
 readme = "README.rst"
 homepage = "https://www.apibara.com"
 repository= "https://github.com/apibara/python-sdk"
 keywords = [
@@ -33,11 +33,20 @@
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 black = "^22.12.0"
 isort = "^5.11.4"
 pytest-asyncio = "^0.20.3"
+grpcio-tools = ">=1.50,<2.0"
+testcontainers = {extras = ["mongodb"], version = "^3.7.1"}
+
+[tool.black]
+line-length = 88
+target-version = ['py38', 'py39', 'py310']
+
+[tool.isort]
+profile = "black"
 
 [build-system]
 requires = ["poetry-core>=1.2.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `apibara-0.7.2/src/apibara/cursor.py` & `apibara-0.7.3a0/src/apibara/cursor.py`

 * *Files identical despite different names*

### Comparing `apibara-0.7.2/src/apibara/indexer/indexer.py` & `apibara-0.7.3a0/src/apibara/indexer/indexer.py`

 * *Files identical despite different names*

### Comparing `apibara-0.7.2/src/apibara/indexer/info.py` & `apibara-0.7.3a0/src/apibara/indexer/info.py`

 * *Files identical despite different names*

### Comparing `apibara-0.7.2/src/apibara/indexer/runner.py` & `apibara-0.7.3a0/src/apibara/indexer/runner.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,25 +63,27 @@
     def __init__(
         self,
         *,
         reset_state: bool = False,
         config: Optional[IndexerRunnerConfiguration] = None,
         client_options: Optional[List[Tuple[str, Any]]] = None,
         timeout: Optional[int] = None,
+        _reconnect_to_avoid_disconnection: Optional[int] = None,
     ) -> None:
         if config is None:
             config = IndexerRunnerConfiguration()
         if client_options is None:
             client_options = DEFAULT_CLIENT_OPTIONS
         self._reset_state = reset_state
         self._config = config
         self._indexer_id = None
         self._indexer_storage = None
         self._timeout = timeout
         self._client_options = client_options
+        self._reconnect_to_avoid_disconnection = _reconnect_to_avoid_disconnection
 
     async def run(self, indexer: Indexer, *, ctx: Optional[UserContext] = None):
         """Run the indexer until stopped."""
         self._check_config()
         self._setup_storage(indexer)
         self._maybe_reset_state()
         await self._do_run(indexer, ctx)
@@ -144,23 +146,30 @@
         logger.debug("indexer configuration sent")
 
         previous_end_cursor = None
         pending_received = False
         additional_filter = None
         runner_state = "default"  # or "resync"
 
+        # Reconnect every few blocks to avoid disconnection
+        if self._reconnect_to_avoid_disconnection is not None:
+            _blocks_before_reconnect = self._reconnect_to_avoid_disconnection
+
         async for message in stream:
             logger.debug("received message")
             self._retry_count = 0
 
             if message.data is not None:
                 assert (
                     len(message.data.data) <= 1
                 ), "indexer runner requires batch_size == 1"
 
+                if self._reconnect_to_avoid_disconnection is not None:
+                    _blocks_before_reconnect -= 1
+
                 if runner_state == "resync":
                     logger.debug("handle block resync")
                     end_cursor = message.data.end_cursor
                     cursor = message.data.cursor
                     logger.debug(f"handle resync batch {cursor} - {end_cursor}")
                     with self._indexer_storage.create_storage_for_data(
                         message.data.end_cursor
@@ -254,14 +263,26 @@
                                 cursor=Cursor(order_key=end_cursor.order_key - 1),
                                 batch_size=1,
                             )
 
                 if not is_pending:
                     previous_end_cursor = message.data.end_cursor
 
+                if self._reconnect_to_avoid_disconnection is not None:
+                    if _blocks_before_reconnect <= 0:
+                        _blocks_before_reconnect = (
+                            self._reconnect_to_avoid_disconnection
+                        )
+                        await client.configure(
+                            filter=config.filter.encode(),
+                            finality=config.finality,
+                            cursor=end_cursor,
+                            batch_size=1,
+                        )
+
             elif message.invalidate is not None:
                 with self._indexer_storage.create_storage_for_invalidate(
                     message.invalidate.cursor
                 ) as storage:
                     cursor = message.invalidate.cursor
                     info = Info(
                         context=ctx, storage=storage, cursor=cursor, end_cursor=cursor
```

### Comparing `apibara-0.7.2/src/apibara/indexer/storage.py` & `apibara-0.7.3a0/src/apibara/indexer/storage.py`

 * *Files identical despite different names*

### Comparing `apibara-0.7.2/src/apibara/protocol/__init__.py` & `apibara-0.7.3a0/src/apibara/protocol/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,23 @@
 from dataclasses import dataclass
 from typing import ClassVar
 
-from .client import (BearerTokenAuth, StreamClient, StreamIter, StreamService,
-                     credentials_with_auth_token)
-from .proto.stream_pb2 import (Cursor, DataFinality, StreamDataRequest,
-                               StreamDataResponse)
+from .client import (
+    BearerTokenAuth,
+    StreamClient,
+    StreamIter,
+    StreamService,
+    credentials_with_auth_token,
+)
+from .proto.stream_pb2 import (
+    Cursor,
+    DataFinality,
+    StreamDataRequest,
+    StreamDataResponse,
+)
 
 
 @dataclass
 class StarkNetStreamAddress:
     Mainnet: ClassVar[str] = "mainnet.starknet.a5a.ch"
     Goerli: ClassVar[str] = "goerli.starknet.a5a.ch"
     Goerli2: ClassVar[str] = "goerli-2.starknet.a5a.ch"
```

### Comparing `apibara-0.7.2/src/apibara/protocol/client.py` & `apibara-0.7.3a0/src/apibara/protocol/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import asyncio
 from asyncio.queues import Queue
 from typing import AsyncIterable, Iterable, Optional, Tuple, Union
 
 import grpc
 from grpc.aio import Channel
 
-from apibara.protocol.proto.stream_pb2 import (Cursor, DataFinality,
-                                               StreamDataRequest,
-                                               StreamDataResponse)
+from apibara.protocol.proto.stream_pb2 import (
+    Cursor,
+    DataFinality,
+    StreamDataRequest,
+    StreamDataResponse,
+)
 from apibara.protocol.proto.stream_pb2_grpc import StreamStub
 
 DEFAULT_TIMEOUT = 45.0
 
 
 class BearerTokenAuth(grpc.AuthMetadataPlugin):
     def __init__(self, token: str):
@@ -59,14 +62,44 @@
             timeout = DEFAULT_TIMEOUT
         ctx = _Context()
         client = StreamClient(ctx)
         iter = self._stub.StreamData(client.client_stream)
         stream = StreamIter(ctx, iter, timeout)
         return client, stream
 
+    def stream_data_immutable(
+        self,
+        *,
+        filter: Optional[bytes] = None,
+        batch_size: Optional[int] = None,
+        finality: Optional[DataFinality.ValueType] = None,
+        cursor: Optional[Cursor] = None,
+        timeout=None,
+    ) -> "StreamIter":
+        """Start streaming data from the server.
+
+        Arguments
+        ---------
+        timeout: float
+            timeout in seconds for waiting messages from the server.
+        """
+        if timeout is None:
+            timeout = DEFAULT_TIMEOUT
+        ctx = _Context()
+        request = StreamDataRequest(
+            stream_id=ctx.stream_id,
+            filter=filter,
+            starting_cursor=cursor,
+            batch_size=batch_size,
+            finality=finality,
+        )
+        iter = self._stub.StreamDataImmutable(request)
+        stream = StreamIter(ctx, iter, timeout)
+        return stream
+
 
 class StreamClient:
     def __init__(self, ctx: "_Context") -> None:
         self._ctx = ctx
         self.client_stream = _RequestChannel()
 
     async def configure(
```

### Comparing `apibara-0.7.2/src/apibara/protocol/proto/stream_pb2.py` & `apibara-0.7.3a0/src/apibara/protocol/proto/stream_pb2.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,32 +9,32 @@
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x0cstream.proto\x12\x15\x61pibara.node.v1alpha2"\xf2\x01\n\x11StreamDataRequest\x12\x16\n\tstream_id\x18\x01 \x01(\x04H\x00\x88\x01\x01\x12\x17\n\nbatch_size\x18\x02 \x01(\x04H\x01\x88\x01\x01\x12\x36\n\x0fstarting_cursor\x18\x03 \x01(\x0b\x32\x1d.apibara.node.v1alpha2.Cursor\x12:\n\x08\x66inality\x18\x04 \x01(\x0e\x32#.apibara.node.v1alpha2.DataFinalityH\x02\x88\x01\x01\x12\x0e\n\x06\x66ilter\x18\x05 \x01(\x0c\x42\x0c\n\n_stream_idB\r\n\x0b_batch_sizeB\x0b\n\t_finality"\xcf\x01\n\x12StreamDataResponse\x12\x11\n\tstream_id\x18\x01 \x01(\x04\x12\x37\n\ninvalidate\x18\x02 \x01(\x0b\x32!.apibara.node.v1alpha2.InvalidateH\x00\x12+\n\x04\x64\x61ta\x18\x03 \x01(\x0b\x32\x1b.apibara.node.v1alpha2.DataH\x00\x12\x35\n\theartbeat\x18\x04 \x01(\x0b\x32 .apibara.node.v1alpha2.HeartbeatH\x00\x42\t\n\x07message"/\n\x06\x43ursor\x12\x11\n\torder_key\x18\x01 \x01(\x04\x12\x12\n\nunique_key\x18\x02 \x01(\x0c";\n\nInvalidate\x12-\n\x06\x63ursor\x18\x01 \x01(\x0b\x32\x1d.apibara.node.v1alpha2.Cursor"\xad\x01\n\x04\x44\x61ta\x12\x31\n\nend_cursor\x18\x01 \x01(\x0b\x32\x1d.apibara.node.v1alpha2.Cursor\x12\x35\n\x08\x66inality\x18\x02 \x01(\x0e\x32#.apibara.node.v1alpha2.DataFinality\x12\x0c\n\x04\x64\x61ta\x18\x03 \x03(\x0c\x12-\n\x06\x63ursor\x18\x04 \x01(\x0b\x32\x1d.apibara.node.v1alpha2.Cursor"\x0b\n\tHeartbeat*u\n\x0c\x44\x61taFinality\x12\x17\n\x13\x44\x41TA_STATUS_UNKNOWN\x10\x00\x12\x17\n\x13\x44\x41TA_STATUS_PENDING\x10\x01\x12\x18\n\x14\x44\x41TA_STATUS_ACCEPTED\x10\x02\x12\x19\n\x15\x44\x41TA_STATUS_FINALIZED\x10\x03\x32o\n\x06Stream\x12\x65\n\nStreamData\x12(.apibara.node.v1alpha2.StreamDataRequest\x1a).apibara.node.v1alpha2.StreamDataResponse(\x01\x30\x01\x62\x06proto3'
+    b'\n\x0cstream.proto\x12\x15\x61pibara.node.v1alpha2"\xf2\x01\n\x11StreamDataRequest\x12\x16\n\tstream_id\x18\x01 \x01(\x04H\x00\x88\x01\x01\x12\x17\n\nbatch_size\x18\x02 \x01(\x04H\x01\x88\x01\x01\x12\x36\n\x0fstarting_cursor\x18\x03 \x01(\x0b\x32\x1d.apibara.node.v1alpha2.Cursor\x12:\n\x08\x66inality\x18\x04 \x01(\x0e\x32#.apibara.node.v1alpha2.DataFinalityH\x02\x88\x01\x01\x12\x0e\n\x06\x66ilter\x18\x05 \x01(\x0c\x42\x0c\n\n_stream_idB\r\n\x0b_batch_sizeB\x0b\n\t_finality"\xcf\x01\n\x12StreamDataResponse\x12\x11\n\tstream_id\x18\x01 \x01(\x04\x12\x37\n\ninvalidate\x18\x02 \x01(\x0b\x32!.apibara.node.v1alpha2.InvalidateH\x00\x12+\n\x04\x64\x61ta\x18\x03 \x01(\x0b\x32\x1b.apibara.node.v1alpha2.DataH\x00\x12\x35\n\theartbeat\x18\x04 \x01(\x0b\x32 .apibara.node.v1alpha2.HeartbeatH\x00\x42\t\n\x07message"/\n\x06\x43ursor\x12\x11\n\torder_key\x18\x01 \x01(\x04\x12\x12\n\nunique_key\x18\x02 \x01(\x0c";\n\nInvalidate\x12-\n\x06\x63ursor\x18\x01 \x01(\x0b\x32\x1d.apibara.node.v1alpha2.Cursor"\xad\x01\n\x04\x44\x61ta\x12\x31\n\nend_cursor\x18\x01 \x01(\x0b\x32\x1d.apibara.node.v1alpha2.Cursor\x12\x35\n\x08\x66inality\x18\x02 \x01(\x0e\x32#.apibara.node.v1alpha2.DataFinality\x12\x0c\n\x04\x64\x61ta\x18\x03 \x03(\x0c\x12-\n\x06\x63ursor\x18\x04 \x01(\x0b\x32\x1d.apibara.node.v1alpha2.Cursor"\x0b\n\tHeartbeat*u\n\x0c\x44\x61taFinality\x12\x17\n\x13\x44\x41TA_STATUS_UNKNOWN\x10\x00\x12\x17\n\x13\x44\x41TA_STATUS_PENDING\x10\x01\x12\x18\n\x14\x44\x41TA_STATUS_ACCEPTED\x10\x02\x12\x19\n\x15\x44\x41TA_STATUS_FINALIZED\x10\x03\x32\xdd\x01\n\x06Stream\x12\x65\n\nStreamData\x12(.apibara.node.v1alpha2.StreamDataRequest\x1a).apibara.node.v1alpha2.StreamDataResponse(\x01\x30\x01\x12l\n\x13StreamDataImmutable\x12(.apibara.node.v1alpha2.StreamDataRequest\x1a).apibara.node.v1alpha2.StreamDataResponse0\x01\x62\x06proto3'
 )
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "stream_pb2", globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "stream_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
     DESCRIPTOR._options = None
-    _DATAFINALITY._serialized_start = 793
-    _DATAFINALITY._serialized_end = 910
-    _STREAMDATAREQUEST._serialized_start = 40
-    _STREAMDATAREQUEST._serialized_end = 282
-    _STREAMDATARESPONSE._serialized_start = 285
-    _STREAMDATARESPONSE._serialized_end = 492
-    _CURSOR._serialized_start = 494
-    _CURSOR._serialized_end = 541
-    _INVALIDATE._serialized_start = 543
-    _INVALIDATE._serialized_end = 602
-    _DATA._serialized_start = 605
-    _DATA._serialized_end = 778
-    _HEARTBEAT._serialized_start = 780
-    _HEARTBEAT._serialized_end = 791
-    _STREAM._serialized_start = 912
-    _STREAM._serialized_end = 1023
+    _globals["_DATAFINALITY"]._serialized_start = 793
+    _globals["_DATAFINALITY"]._serialized_end = 910
+    _globals["_STREAMDATAREQUEST"]._serialized_start = 40
+    _globals["_STREAMDATAREQUEST"]._serialized_end = 282
+    _globals["_STREAMDATARESPONSE"]._serialized_start = 285
+    _globals["_STREAMDATARESPONSE"]._serialized_end = 492
+    _globals["_CURSOR"]._serialized_start = 494
+    _globals["_CURSOR"]._serialized_end = 541
+    _globals["_INVALIDATE"]._serialized_start = 543
+    _globals["_INVALIDATE"]._serialized_end = 602
+    _globals["_DATA"]._serialized_start = 605
+    _globals["_DATA"]._serialized_end = 778
+    _globals["_HEARTBEAT"]._serialized_start = 780
+    _globals["_HEARTBEAT"]._serialized_end = 791
+    _globals["_STREAM"]._serialized_start = 913
+    _globals["_STREAM"]._serialized_end = 1134
 # @@protoc_insertion_point(module_scope)
```

### Comparing `apibara-0.7.2/src/apibara/protocol/proto/stream_pb2_grpc.pyi` & `apibara-0.7.3a0/src/apibara/protocol/proto/stream_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `apibara-0.7.2/src/apibara/starknet/cursor.py` & `apibara-0.7.3a0/src/apibara/starknet/cursor.py`

 * *Files identical despite different names*

### Comparing `apibara-0.7.2/src/apibara/starknet/felt.py` & `apibara-0.7.3a0/src/apibara/starknet/felt.py`

 * *Files identical despite different names*

### Comparing `apibara-0.7.2/src/apibara/starknet/filter.py` & `apibara-0.7.3a0/src/apibara/starknet/filter.py`

 * *Files identical despite different names*

### Comparing `apibara-0.7.2/src/apibara/starknet/proto/filter_pb2.py` & `apibara-0.7.3a0/src/apibara/starknet/proto/filter_pb2.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,49 +12,49 @@
 _sym_db = _symbol_database.Default()
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
     b"\n\x0c\x66ilter.proto\x12\x19\x61pibara.starknet.v1alpha2\x1a\x0btypes.proto\"\xc3\x02\n\x06\x46ilter\x12\x37\n\x06header\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.HeaderFilter\x12\x42\n\x0ctransactions\x18\x02 \x03(\x0b\x32,.apibara.starknet.v1alpha2.TransactionFilter\x12\x42\n\x0cstate_update\x18\x03 \x01(\x0b\x32,.apibara.starknet.v1alpha2.StateUpdateFilter\x12\x36\n\x06\x65vents\x18\x04 \x03(\x0b\x32&.apibara.starknet.v1alpha2.EventFilter\x12@\n\x08messages\x18\x05 \x03(\x0b\x32..apibara.starknet.v1alpha2.L2ToL1MessageFilter\"\x1c\n\x0cHeaderFilter\x12\x0c\n\x04weak\x18\x01 \x01(\x08\"\xe3\x03\n\x11TransactionFilter\x12I\n\tinvoke_v0\x18\x01 \x01(\x0b\x32\x34.apibara.starknet.v1alpha2.InvokeTransactionV0FilterH\x00\x12I\n\tinvoke_v1\x18\x02 \x01(\x0b\x32\x34.apibara.starknet.v1alpha2.InvokeTransactionV1FilterH\x00\x12\x44\n\x06\x64\x65ploy\x18\x03 \x01(\x0b\x32\x32.apibara.starknet.v1alpha2.DeployTransactionFilterH\x00\x12\x46\n\x07\x64\x65\x63lare\x18\x04 \x01(\x0b\x32\x33.apibara.starknet.v1alpha2.DeclareTransactionFilterH\x00\x12K\n\nl1_handler\x18\x05 \x01(\x0b\x32\x35.apibara.starknet.v1alpha2.L1HandlerTransactionFilterH\x00\x12S\n\x0e\x64\x65ploy_account\x18\x06 \x01(\x0b\x32\x39.apibara.starknet.v1alpha2.DeployAccountTransactionFilterH\x00\x42\x08\n\x06\x66ilter\"\xe0\x01\n\x19InvokeTransactionV0Filter\x12\x41\n\x10\x63ontract_address\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x45\n\x14\x65ntry_point_selector\x18\x02 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x39\n\x08\x63\x61lldata\x18\x03 \x03(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\x97\x01\n\x19InvokeTransactionV1Filter\x12?\n\x0esender_address\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x39\n\x08\x63\x61lldata\x18\x03 \x03(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\xe5\x01\n\x17\x44\x65ployTransactionFilter\x12\x46\n\x15\x63ontract_address_salt\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12;\n\nclass_hash\x18\x02 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x45\n\x14\x63onstructor_calldata\x18\x04 \x03(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\x98\x01\n\x18\x44\x65\x63lareTransactionFilter\x12;\n\nclass_hash\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12?\n\x0esender_address\x18\x02 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\xe1\x01\n\x1aL1HandlerTransactionFilter\x12\x41\n\x10\x63ontract_address\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x45\n\x14\x65ntry_point_selector\x18\x02 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x39\n\x08\x63\x61lldata\x18\x03 \x03(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\xec\x01\n\x1e\x44\x65ployAccountTransactionFilter\x12\x46\n\x15\x63ontract_address_salt\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12;\n\nclass_hash\x18\x02 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x45\n\x14\x63onstructor_calldata\x18\x04 \x03(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\x8c\x01\n\x13L2ToL1MessageFilter\x12;\n\nto_address\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x38\n\x07payload\x18\x02 \x03(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\xba\x01\n\x0b\x45ventFilter\x12=\n\x0c\x66rom_address\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x35\n\x04keys\x18\x02 \x03(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x35\n\x04\x64\x61ta\x18\x03 \x03(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\xc8\x03\n\x11StateUpdateFilter\x12\x43\n\rstorage_diffs\x18\x01 \x03(\x0b\x32,.apibara.starknet.v1alpha2.StorageDiffFilter\x12M\n\x12\x64\x65\x63lared_contracts\x18\x02 \x03(\x0b\x32\x31.apibara.starknet.v1alpha2.DeclaredContractFilter\x12M\n\x12\x64\x65ployed_contracts\x18\x03 \x03(\x0b\x32\x31.apibara.starknet.v1alpha2.DeployedContractFilter\x12<\n\x06nonces\x18\x04 \x03(\x0b\x32,.apibara.starknet.v1alpha2.NonceUpdateFilter\x12H\n\x10\x64\x65\x63lared_classes\x18\x05 \x03(\x0b\x32..apibara.starknet.v1alpha2.DeclaredClassFilter\x12H\n\x10replaced_classes\x18\x06 \x03(\x0b\x32..apibara.starknet.v1alpha2.ReplacedClassFilter\"V\n\x11StorageDiffFilter\x12\x41\n\x10\x63ontract_address\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"U\n\x16\x44\x65\x63laredContractFilter\x12;\n\nclass_hash\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\x98\x01\n\x13\x44\x65\x63laredClassFilter\x12;\n\nclass_hash\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x44\n\x13\x63ompiled_class_hash\x18\x02 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\x95\x01\n\x13ReplacedClassFilter\x12\x41\n\x10\x63ontract_address\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12;\n\nclass_hash\x18\x02 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\x98\x01\n\x16\x44\x65ployedContractFilter\x12\x41\n\x10\x63ontract_address\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12;\n\nclass_hash\x18\x02 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\x8e\x01\n\x11NonceUpdateFilter\x12\x41\n\x10\x63ontract_address\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x36\n\x05nonce\x18\x02 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElementb\x06proto3"
 )
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "filter_pb2", globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "filter_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
     DESCRIPTOR._options = None
-    _FILTER._serialized_start = 57
-    _FILTER._serialized_end = 380
-    _HEADERFILTER._serialized_start = 382
-    _HEADERFILTER._serialized_end = 410
-    _TRANSACTIONFILTER._serialized_start = 413
-    _TRANSACTIONFILTER._serialized_end = 896
-    _INVOKETRANSACTIONV0FILTER._serialized_start = 899
-    _INVOKETRANSACTIONV0FILTER._serialized_end = 1123
-    _INVOKETRANSACTIONV1FILTER._serialized_start = 1126
-    _INVOKETRANSACTIONV1FILTER._serialized_end = 1277
-    _DEPLOYTRANSACTIONFILTER._serialized_start = 1280
-    _DEPLOYTRANSACTIONFILTER._serialized_end = 1509
-    _DECLARETRANSACTIONFILTER._serialized_start = 1512
-    _DECLARETRANSACTIONFILTER._serialized_end = 1664
-    _L1HANDLERTRANSACTIONFILTER._serialized_start = 1667
-    _L1HANDLERTRANSACTIONFILTER._serialized_end = 1892
-    _DEPLOYACCOUNTTRANSACTIONFILTER._serialized_start = 1895
-    _DEPLOYACCOUNTTRANSACTIONFILTER._serialized_end = 2131
-    _L2TOL1MESSAGEFILTER._serialized_start = 2134
-    _L2TOL1MESSAGEFILTER._serialized_end = 2274
-    _EVENTFILTER._serialized_start = 2277
-    _EVENTFILTER._serialized_end = 2463
-    _STATEUPDATEFILTER._serialized_start = 2466
-    _STATEUPDATEFILTER._serialized_end = 2922
-    _STORAGEDIFFFILTER._serialized_start = 2924
-    _STORAGEDIFFFILTER._serialized_end = 3010
-    _DECLAREDCONTRACTFILTER._serialized_start = 3012
-    _DECLAREDCONTRACTFILTER._serialized_end = 3097
-    _DECLAREDCLASSFILTER._serialized_start = 3100
-    _DECLAREDCLASSFILTER._serialized_end = 3252
-    _REPLACEDCLASSFILTER._serialized_start = 3255
-    _REPLACEDCLASSFILTER._serialized_end = 3404
-    _DEPLOYEDCONTRACTFILTER._serialized_start = 3407
-    _DEPLOYEDCONTRACTFILTER._serialized_end = 3559
-    _NONCEUPDATEFILTER._serialized_start = 3562
-    _NONCEUPDATEFILTER._serialized_end = 3704
+    _globals["_FILTER"]._serialized_start = 57
+    _globals["_FILTER"]._serialized_end = 380
+    _globals["_HEADERFILTER"]._serialized_start = 382
+    _globals["_HEADERFILTER"]._serialized_end = 410
+    _globals["_TRANSACTIONFILTER"]._serialized_start = 413
+    _globals["_TRANSACTIONFILTER"]._serialized_end = 896
+    _globals["_INVOKETRANSACTIONV0FILTER"]._serialized_start = 899
+    _globals["_INVOKETRANSACTIONV0FILTER"]._serialized_end = 1123
+    _globals["_INVOKETRANSACTIONV1FILTER"]._serialized_start = 1126
+    _globals["_INVOKETRANSACTIONV1FILTER"]._serialized_end = 1277
+    _globals["_DEPLOYTRANSACTIONFILTER"]._serialized_start = 1280
+    _globals["_DEPLOYTRANSACTIONFILTER"]._serialized_end = 1509
+    _globals["_DECLARETRANSACTIONFILTER"]._serialized_start = 1512
+    _globals["_DECLARETRANSACTIONFILTER"]._serialized_end = 1664
+    _globals["_L1HANDLERTRANSACTIONFILTER"]._serialized_start = 1667
+    _globals["_L1HANDLERTRANSACTIONFILTER"]._serialized_end = 1892
+    _globals["_DEPLOYACCOUNTTRANSACTIONFILTER"]._serialized_start = 1895
+    _globals["_DEPLOYACCOUNTTRANSACTIONFILTER"]._serialized_end = 2131
+    _globals["_L2TOL1MESSAGEFILTER"]._serialized_start = 2134
+    _globals["_L2TOL1MESSAGEFILTER"]._serialized_end = 2274
+    _globals["_EVENTFILTER"]._serialized_start = 2277
+    _globals["_EVENTFILTER"]._serialized_end = 2463
+    _globals["_STATEUPDATEFILTER"]._serialized_start = 2466
+    _globals["_STATEUPDATEFILTER"]._serialized_end = 2922
+    _globals["_STORAGEDIFFFILTER"]._serialized_start = 2924
+    _globals["_STORAGEDIFFFILTER"]._serialized_end = 3010
+    _globals["_DECLAREDCONTRACTFILTER"]._serialized_start = 3012
+    _globals["_DECLAREDCONTRACTFILTER"]._serialized_end = 3097
+    _globals["_DECLAREDCLASSFILTER"]._serialized_start = 3100
+    _globals["_DECLAREDCLASSFILTER"]._serialized_end = 3252
+    _globals["_REPLACEDCLASSFILTER"]._serialized_start = 3255
+    _globals["_REPLACEDCLASSFILTER"]._serialized_end = 3404
+    _globals["_DEPLOYEDCONTRACTFILTER"]._serialized_start = 3407
+    _globals["_DEPLOYEDCONTRACTFILTER"]._serialized_end = 3559
+    _globals["_NONCEUPDATEFILTER"]._serialized_start = 3562
+    _globals["_NONCEUPDATEFILTER"]._serialized_end = 3704
 # @@protoc_insertion_point(module_scope)
```

### Comparing `apibara-0.7.2/src/apibara/starknet/proto/filter_pb2.pyi` & `apibara-0.7.3a0/src/apibara/starknet/proto/filter_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -8,249 +8,226 @@
 from google.protobuf import message as _message
 from google.protobuf.internal import containers as _containers
 
 import apibara.starknet.proto.types_pb2 as _types_pb2
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class DeclareTransactionFilter(_message.Message):
-    __slots__ = ["class_hash", "sender_address"]
-    CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
-    SENDER_ADDRESS_FIELD_NUMBER: _ClassVar[int]
-    class_hash: _types_pb2.FieldElement
-    sender_address: _types_pb2.FieldElement
+class Filter(_message.Message):
+    __slots__ = ["header", "transactions", "state_update", "events", "messages"]
+    HEADER_FIELD_NUMBER: _ClassVar[int]
+    TRANSACTIONS_FIELD_NUMBER: _ClassVar[int]
+    STATE_UPDATE_FIELD_NUMBER: _ClassVar[int]
+    EVENTS_FIELD_NUMBER: _ClassVar[int]
+    MESSAGES_FIELD_NUMBER: _ClassVar[int]
+    header: HeaderFilter
+    transactions: _containers.RepeatedCompositeFieldContainer[TransactionFilter]
+    state_update: StateUpdateFilter
+    events: _containers.RepeatedCompositeFieldContainer[EventFilter]
+    messages: _containers.RepeatedCompositeFieldContainer[L2ToL1MessageFilter]
     def __init__(
         self,
-        class_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
-        sender_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+        header: _Optional[_Union[HeaderFilter, _Mapping]] = ...,
+        transactions: _Optional[_Iterable[_Union[TransactionFilter, _Mapping]]] = ...,
+        state_update: _Optional[_Union[StateUpdateFilter, _Mapping]] = ...,
+        events: _Optional[_Iterable[_Union[EventFilter, _Mapping]]] = ...,
+        messages: _Optional[_Iterable[_Union[L2ToL1MessageFilter, _Mapping]]] = ...,
     ) -> None: ...
 
-class DeclaredClassFilter(_message.Message):
-    __slots__ = ["class_hash", "compiled_class_hash"]
-    CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
-    COMPILED_CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
-    class_hash: _types_pb2.FieldElement
-    compiled_class_hash: _types_pb2.FieldElement
+class HeaderFilter(_message.Message):
+    __slots__ = ["weak"]
+    WEAK_FIELD_NUMBER: _ClassVar[int]
+    weak: bool
+    def __init__(self, weak: bool = ...) -> None: ...
+
+class TransactionFilter(_message.Message):
+    __slots__ = [
+        "invoke_v0",
+        "invoke_v1",
+        "deploy",
+        "declare",
+        "l1_handler",
+        "deploy_account",
+    ]
+    INVOKE_V0_FIELD_NUMBER: _ClassVar[int]
+    INVOKE_V1_FIELD_NUMBER: _ClassVar[int]
+    DEPLOY_FIELD_NUMBER: _ClassVar[int]
+    DECLARE_FIELD_NUMBER: _ClassVar[int]
+    L1_HANDLER_FIELD_NUMBER: _ClassVar[int]
+    DEPLOY_ACCOUNT_FIELD_NUMBER: _ClassVar[int]
+    invoke_v0: InvokeTransactionV0Filter
+    invoke_v1: InvokeTransactionV1Filter
+    deploy: DeployTransactionFilter
+    declare: DeclareTransactionFilter
+    l1_handler: L1HandlerTransactionFilter
+    deploy_account: DeployAccountTransactionFilter
     def __init__(
         self,
-        class_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
-        compiled_class_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+        invoke_v0: _Optional[_Union[InvokeTransactionV0Filter, _Mapping]] = ...,
+        invoke_v1: _Optional[_Union[InvokeTransactionV1Filter, _Mapping]] = ...,
+        deploy: _Optional[_Union[DeployTransactionFilter, _Mapping]] = ...,
+        declare: _Optional[_Union[DeclareTransactionFilter, _Mapping]] = ...,
+        l1_handler: _Optional[_Union[L1HandlerTransactionFilter, _Mapping]] = ...,
+        deploy_account: _Optional[
+            _Union[DeployAccountTransactionFilter, _Mapping]
+        ] = ...,
     ) -> None: ...
 
-class DeclaredContractFilter(_message.Message):
-    __slots__ = ["class_hash"]
-    CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
-    class_hash: _types_pb2.FieldElement
+class InvokeTransactionV0Filter(_message.Message):
+    __slots__ = ["contract_address", "entry_point_selector", "calldata"]
+    CONTRACT_ADDRESS_FIELD_NUMBER: _ClassVar[int]
+    ENTRY_POINT_SELECTOR_FIELD_NUMBER: _ClassVar[int]
+    CALLDATA_FIELD_NUMBER: _ClassVar[int]
+    contract_address: _types_pb2.FieldElement
+    entry_point_selector: _types_pb2.FieldElement
+    calldata: _containers.RepeatedCompositeFieldContainer[_types_pb2.FieldElement]
     def __init__(
-        self, class_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...
+        self,
+        contract_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+        entry_point_selector: _Optional[
+            _Union[_types_pb2.FieldElement, _Mapping]
+        ] = ...,
+        calldata: _Optional[_Iterable[_Union[_types_pb2.FieldElement, _Mapping]]] = ...,
     ) -> None: ...
 
-class DeployAccountTransactionFilter(_message.Message):
-    __slots__ = ["class_hash", "constructor_calldata", "contract_address_salt"]
-    CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
-    CONSTRUCTOR_CALLDATA_FIELD_NUMBER: _ClassVar[int]
-    CONTRACT_ADDRESS_SALT_FIELD_NUMBER: _ClassVar[int]
-    class_hash: _types_pb2.FieldElement
-    constructor_calldata: _containers.RepeatedCompositeFieldContainer[
-        _types_pb2.FieldElement
-    ]
-    contract_address_salt: _types_pb2.FieldElement
+class InvokeTransactionV1Filter(_message.Message):
+    __slots__ = ["sender_address", "calldata"]
+    SENDER_ADDRESS_FIELD_NUMBER: _ClassVar[int]
+    CALLDATA_FIELD_NUMBER: _ClassVar[int]
+    sender_address: _types_pb2.FieldElement
+    calldata: _containers.RepeatedCompositeFieldContainer[_types_pb2.FieldElement]
     def __init__(
         self,
-        contract_address_salt: _Optional[
-            _Union[_types_pb2.FieldElement, _Mapping]
-        ] = ...,
-        class_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
-        constructor_calldata: _Optional[
-            _Iterable[_Union[_types_pb2.FieldElement, _Mapping]]
-        ] = ...,
+        sender_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+        calldata: _Optional[_Iterable[_Union[_types_pb2.FieldElement, _Mapping]]] = ...,
     ) -> None: ...
 
 class DeployTransactionFilter(_message.Message):
-    __slots__ = ["class_hash", "constructor_calldata", "contract_address_salt"]
+    __slots__ = ["contract_address_salt", "class_hash", "constructor_calldata"]
+    CONTRACT_ADDRESS_SALT_FIELD_NUMBER: _ClassVar[int]
     CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
     CONSTRUCTOR_CALLDATA_FIELD_NUMBER: _ClassVar[int]
-    CONTRACT_ADDRESS_SALT_FIELD_NUMBER: _ClassVar[int]
+    contract_address_salt: _types_pb2.FieldElement
     class_hash: _types_pb2.FieldElement
     constructor_calldata: _containers.RepeatedCompositeFieldContainer[
         _types_pb2.FieldElement
     ]
-    contract_address_salt: _types_pb2.FieldElement
     def __init__(
         self,
         contract_address_salt: _Optional[
             _Union[_types_pb2.FieldElement, _Mapping]
         ] = ...,
         class_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
         constructor_calldata: _Optional[
             _Iterable[_Union[_types_pb2.FieldElement, _Mapping]]
         ] = ...,
     ) -> None: ...
 
-class DeployedContractFilter(_message.Message):
-    __slots__ = ["class_hash", "contract_address"]
+class DeclareTransactionFilter(_message.Message):
+    __slots__ = ["class_hash", "sender_address"]
     CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
-    CONTRACT_ADDRESS_FIELD_NUMBER: _ClassVar[int]
+    SENDER_ADDRESS_FIELD_NUMBER: _ClassVar[int]
     class_hash: _types_pb2.FieldElement
-    contract_address: _types_pb2.FieldElement
+    sender_address: _types_pb2.FieldElement
     def __init__(
         self,
-        contract_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
         class_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+        sender_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
     ) -> None: ...
 
-class EventFilter(_message.Message):
-    __slots__ = ["data", "from_address", "keys"]
-    DATA_FIELD_NUMBER: _ClassVar[int]
-    FROM_ADDRESS_FIELD_NUMBER: _ClassVar[int]
-    KEYS_FIELD_NUMBER: _ClassVar[int]
-    data: _containers.RepeatedCompositeFieldContainer[_types_pb2.FieldElement]
-    from_address: _types_pb2.FieldElement
-    keys: _containers.RepeatedCompositeFieldContainer[_types_pb2.FieldElement]
-    def __init__(
-        self,
-        from_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
-        keys: _Optional[_Iterable[_Union[_types_pb2.FieldElement, _Mapping]]] = ...,
-        data: _Optional[_Iterable[_Union[_types_pb2.FieldElement, _Mapping]]] = ...,
-    ) -> None: ...
-
-class Filter(_message.Message):
-    __slots__ = ["events", "header", "messages", "state_update", "transactions"]
-    EVENTS_FIELD_NUMBER: _ClassVar[int]
-    HEADER_FIELD_NUMBER: _ClassVar[int]
-    MESSAGES_FIELD_NUMBER: _ClassVar[int]
-    STATE_UPDATE_FIELD_NUMBER: _ClassVar[int]
-    TRANSACTIONS_FIELD_NUMBER: _ClassVar[int]
-    events: _containers.RepeatedCompositeFieldContainer[EventFilter]
-    header: HeaderFilter
-    messages: _containers.RepeatedCompositeFieldContainer[L2ToL1MessageFilter]
-    state_update: StateUpdateFilter
-    transactions: _containers.RepeatedCompositeFieldContainer[TransactionFilter]
-    def __init__(
-        self,
-        header: _Optional[_Union[HeaderFilter, _Mapping]] = ...,
-        transactions: _Optional[_Iterable[_Union[TransactionFilter, _Mapping]]] = ...,
-        state_update: _Optional[_Union[StateUpdateFilter, _Mapping]] = ...,
-        events: _Optional[_Iterable[_Union[EventFilter, _Mapping]]] = ...,
-        messages: _Optional[_Iterable[_Union[L2ToL1MessageFilter, _Mapping]]] = ...,
-    ) -> None: ...
-
-class HeaderFilter(_message.Message):
-    __slots__ = ["weak"]
-    WEAK_FIELD_NUMBER: _ClassVar[int]
-    weak: bool
-    def __init__(self, weak: bool = ...) -> None: ...
-
-class InvokeTransactionV0Filter(_message.Message):
-    __slots__ = ["calldata", "contract_address", "entry_point_selector"]
-    CALLDATA_FIELD_NUMBER: _ClassVar[int]
+class L1HandlerTransactionFilter(_message.Message):
+    __slots__ = ["contract_address", "entry_point_selector", "calldata"]
     CONTRACT_ADDRESS_FIELD_NUMBER: _ClassVar[int]
     ENTRY_POINT_SELECTOR_FIELD_NUMBER: _ClassVar[int]
-    calldata: _containers.RepeatedCompositeFieldContainer[_types_pb2.FieldElement]
+    CALLDATA_FIELD_NUMBER: _ClassVar[int]
     contract_address: _types_pb2.FieldElement
     entry_point_selector: _types_pb2.FieldElement
+    calldata: _containers.RepeatedCompositeFieldContainer[_types_pb2.FieldElement]
     def __init__(
         self,
         contract_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
         entry_point_selector: _Optional[
             _Union[_types_pb2.FieldElement, _Mapping]
         ] = ...,
         calldata: _Optional[_Iterable[_Union[_types_pb2.FieldElement, _Mapping]]] = ...,
     ) -> None: ...
 
-class InvokeTransactionV1Filter(_message.Message):
-    __slots__ = ["calldata", "sender_address"]
-    CALLDATA_FIELD_NUMBER: _ClassVar[int]
-    SENDER_ADDRESS_FIELD_NUMBER: _ClassVar[int]
-    calldata: _containers.RepeatedCompositeFieldContainer[_types_pb2.FieldElement]
-    sender_address: _types_pb2.FieldElement
-    def __init__(
-        self,
-        sender_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
-        calldata: _Optional[_Iterable[_Union[_types_pb2.FieldElement, _Mapping]]] = ...,
-    ) -> None: ...
-
-class L1HandlerTransactionFilter(_message.Message):
-    __slots__ = ["calldata", "contract_address", "entry_point_selector"]
-    CALLDATA_FIELD_NUMBER: _ClassVar[int]
-    CONTRACT_ADDRESS_FIELD_NUMBER: _ClassVar[int]
-    ENTRY_POINT_SELECTOR_FIELD_NUMBER: _ClassVar[int]
-    calldata: _containers.RepeatedCompositeFieldContainer[_types_pb2.FieldElement]
-    contract_address: _types_pb2.FieldElement
-    entry_point_selector: _types_pb2.FieldElement
+class DeployAccountTransactionFilter(_message.Message):
+    __slots__ = ["contract_address_salt", "class_hash", "constructor_calldata"]
+    CONTRACT_ADDRESS_SALT_FIELD_NUMBER: _ClassVar[int]
+    CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
+    CONSTRUCTOR_CALLDATA_FIELD_NUMBER: _ClassVar[int]
+    contract_address_salt: _types_pb2.FieldElement
+    class_hash: _types_pb2.FieldElement
+    constructor_calldata: _containers.RepeatedCompositeFieldContainer[
+        _types_pb2.FieldElement
+    ]
     def __init__(
         self,
-        contract_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
-        entry_point_selector: _Optional[
+        contract_address_salt: _Optional[
             _Union[_types_pb2.FieldElement, _Mapping]
         ] = ...,
-        calldata: _Optional[_Iterable[_Union[_types_pb2.FieldElement, _Mapping]]] = ...,
+        class_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+        constructor_calldata: _Optional[
+            _Iterable[_Union[_types_pb2.FieldElement, _Mapping]]
+        ] = ...,
     ) -> None: ...
 
 class L2ToL1MessageFilter(_message.Message):
-    __slots__ = ["payload", "to_address"]
-    PAYLOAD_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["to_address", "payload"]
     TO_ADDRESS_FIELD_NUMBER: _ClassVar[int]
-    payload: _containers.RepeatedCompositeFieldContainer[_types_pb2.FieldElement]
+    PAYLOAD_FIELD_NUMBER: _ClassVar[int]
     to_address: _types_pb2.FieldElement
+    payload: _containers.RepeatedCompositeFieldContainer[_types_pb2.FieldElement]
     def __init__(
         self,
         to_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
         payload: _Optional[_Iterable[_Union[_types_pb2.FieldElement, _Mapping]]] = ...,
     ) -> None: ...
 
-class NonceUpdateFilter(_message.Message):
-    __slots__ = ["contract_address", "nonce"]
-    CONTRACT_ADDRESS_FIELD_NUMBER: _ClassVar[int]
-    NONCE_FIELD_NUMBER: _ClassVar[int]
-    contract_address: _types_pb2.FieldElement
-    nonce: _types_pb2.FieldElement
-    def __init__(
-        self,
-        contract_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
-        nonce: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
-    ) -> None: ...
-
-class ReplacedClassFilter(_message.Message):
-    __slots__ = ["class_hash", "contract_address"]
-    CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
-    CONTRACT_ADDRESS_FIELD_NUMBER: _ClassVar[int]
-    class_hash: _types_pb2.FieldElement
-    contract_address: _types_pb2.FieldElement
+class EventFilter(_message.Message):
+    __slots__ = ["from_address", "keys", "data"]
+    FROM_ADDRESS_FIELD_NUMBER: _ClassVar[int]
+    KEYS_FIELD_NUMBER: _ClassVar[int]
+    DATA_FIELD_NUMBER: _ClassVar[int]
+    from_address: _types_pb2.FieldElement
+    keys: _containers.RepeatedCompositeFieldContainer[_types_pb2.FieldElement]
+    data: _containers.RepeatedCompositeFieldContainer[_types_pb2.FieldElement]
     def __init__(
         self,
-        contract_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
-        class_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+        from_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+        keys: _Optional[_Iterable[_Union[_types_pb2.FieldElement, _Mapping]]] = ...,
+        data: _Optional[_Iterable[_Union[_types_pb2.FieldElement, _Mapping]]] = ...,
     ) -> None: ...
 
 class StateUpdateFilter(_message.Message):
     __slots__ = [
-        "declared_classes",
+        "storage_diffs",
         "declared_contracts",
         "deployed_contracts",
         "nonces",
+        "declared_classes",
         "replaced_classes",
-        "storage_diffs",
     ]
-    DECLARED_CLASSES_FIELD_NUMBER: _ClassVar[int]
+    STORAGE_DIFFS_FIELD_NUMBER: _ClassVar[int]
     DECLARED_CONTRACTS_FIELD_NUMBER: _ClassVar[int]
     DEPLOYED_CONTRACTS_FIELD_NUMBER: _ClassVar[int]
     NONCES_FIELD_NUMBER: _ClassVar[int]
+    DECLARED_CLASSES_FIELD_NUMBER: _ClassVar[int]
     REPLACED_CLASSES_FIELD_NUMBER: _ClassVar[int]
-    STORAGE_DIFFS_FIELD_NUMBER: _ClassVar[int]
-    declared_classes: _containers.RepeatedCompositeFieldContainer[DeclaredClassFilter]
+    storage_diffs: _containers.RepeatedCompositeFieldContainer[StorageDiffFilter]
     declared_contracts: _containers.RepeatedCompositeFieldContainer[
         DeclaredContractFilter
     ]
     deployed_contracts: _containers.RepeatedCompositeFieldContainer[
         DeployedContractFilter
     ]
     nonces: _containers.RepeatedCompositeFieldContainer[NonceUpdateFilter]
+    declared_classes: _containers.RepeatedCompositeFieldContainer[DeclaredClassFilter]
     replaced_classes: _containers.RepeatedCompositeFieldContainer[ReplacedClassFilter]
-    storage_diffs: _containers.RepeatedCompositeFieldContainer[StorageDiffFilter]
     def __init__(
         self,
         storage_diffs: _Optional[_Iterable[_Union[StorageDiffFilter, _Mapping]]] = ...,
         declared_contracts: _Optional[
             _Iterable[_Union[DeclaredContractFilter, _Mapping]]
         ] = ...,
         deployed_contracts: _Optional[
@@ -270,39 +247,62 @@
     CONTRACT_ADDRESS_FIELD_NUMBER: _ClassVar[int]
     contract_address: _types_pb2.FieldElement
     def __init__(
         self,
         contract_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
     ) -> None: ...
 
-class TransactionFilter(_message.Message):
-    __slots__ = [
-        "declare",
-        "deploy",
-        "deploy_account",
-        "invoke_v0",
-        "invoke_v1",
-        "l1_handler",
-    ]
-    DECLARE_FIELD_NUMBER: _ClassVar[int]
-    DEPLOY_ACCOUNT_FIELD_NUMBER: _ClassVar[int]
-    DEPLOY_FIELD_NUMBER: _ClassVar[int]
-    INVOKE_V0_FIELD_NUMBER: _ClassVar[int]
-    INVOKE_V1_FIELD_NUMBER: _ClassVar[int]
-    L1_HANDLER_FIELD_NUMBER: _ClassVar[int]
-    declare: DeclareTransactionFilter
-    deploy: DeployTransactionFilter
-    deploy_account: DeployAccountTransactionFilter
-    invoke_v0: InvokeTransactionV0Filter
-    invoke_v1: InvokeTransactionV1Filter
-    l1_handler: L1HandlerTransactionFilter
+class DeclaredContractFilter(_message.Message):
+    __slots__ = ["class_hash"]
+    CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
+    class_hash: _types_pb2.FieldElement
+    def __init__(
+        self, class_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...
+    ) -> None: ...
+
+class DeclaredClassFilter(_message.Message):
+    __slots__ = ["class_hash", "compiled_class_hash"]
+    CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
+    COMPILED_CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
+    class_hash: _types_pb2.FieldElement
+    compiled_class_hash: _types_pb2.FieldElement
     def __init__(
         self,
-        invoke_v0: _Optional[_Union[InvokeTransactionV0Filter, _Mapping]] = ...,
-        invoke_v1: _Optional[_Union[InvokeTransactionV1Filter, _Mapping]] = ...,
-        deploy: _Optional[_Union[DeployTransactionFilter, _Mapping]] = ...,
-        declare: _Optional[_Union[DeclareTransactionFilter, _Mapping]] = ...,
-        l1_handler: _Optional[_Union[L1HandlerTransactionFilter, _Mapping]] = ...,
-        deploy_account: _Optional[
-            _Union[DeployAccountTransactionFilter, _Mapping]
-        ] = ...,
+        class_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+        compiled_class_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+    ) -> None: ...
+
+class ReplacedClassFilter(_message.Message):
+    __slots__ = ["contract_address", "class_hash"]
+    CONTRACT_ADDRESS_FIELD_NUMBER: _ClassVar[int]
+    CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
+    contract_address: _types_pb2.FieldElement
+    class_hash: _types_pb2.FieldElement
+    def __init__(
+        self,
+        contract_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+        class_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+    ) -> None: ...
+
+class DeployedContractFilter(_message.Message):
+    __slots__ = ["contract_address", "class_hash"]
+    CONTRACT_ADDRESS_FIELD_NUMBER: _ClassVar[int]
+    CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
+    contract_address: _types_pb2.FieldElement
+    class_hash: _types_pb2.FieldElement
+    def __init__(
+        self,
+        contract_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+        class_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+    ) -> None: ...
+
+class NonceUpdateFilter(_message.Message):
+    __slots__ = ["contract_address", "nonce"]
+    CONTRACT_ADDRESS_FIELD_NUMBER: _ClassVar[int]
+    NONCE_FIELD_NUMBER: _ClassVar[int]
+    contract_address: _types_pb2.FieldElement
+    nonce: _types_pb2.FieldElement
+    def __init__(
+        self,
+        contract_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+        nonce: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
     ) -> None: ...
```

### Comparing `apibara-0.7.2/src/apibara/starknet/proto/starknet_pb2.py` & `apibara-0.7.3a0/src/apibara/starknet/proto/starknet_pb2.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,72 +8,71 @@
 from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from google.protobuf import \
-    timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
+from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
     b"\n\x0estarknet.proto\x12\x19\x61pibara.starknet.v1alpha2\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x0btypes.proto\"\x93\x03\n\x05\x42lock\x12\x36\n\x06status\x18\x01 \x01(\x0e\x32&.apibara.starknet.v1alpha2.BlockStatus\x12\x36\n\x06header\x18\x02 \x01(\x0b\x32&.apibara.starknet.v1alpha2.BlockHeader\x12G\n\x0ctransactions\x18\x03 \x03(\x0b\x32\x31.apibara.starknet.v1alpha2.TransactionWithReceipt\x12<\n\x0cstate_update\x18\x04 \x01(\x0b\x32&.apibara.starknet.v1alpha2.StateUpdate\x12?\n\x06\x65vents\x18\x05 \x03(\x0b\x32/.apibara.starknet.v1alpha2.EventWithTransaction\x12R\n\x11l2_to_l1_messages\x18\x06 \x03(\x0b\x32\x37.apibara.starknet.v1alpha2.L2ToL1MessageWithTransaction\"\xd2\x02\n\x0b\x42lockHeader\x12;\n\nblock_hash\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x42\n\x11parent_block_hash\x18\x02 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x14\n\x0c\x62lock_number\x18\x03 \x01(\x04\x12\x42\n\x11sequencer_address\x18\x04 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x39\n\x08new_root\x18\x05 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12-\n\ttimestamp\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\x95\x01\n\x16TransactionWithReceipt\x12;\n\x0btransaction\x18\x01 \x01(\x0b\x32&.apibara.starknet.v1alpha2.Transaction\x12>\n\x07receipt\x18\x02 \x01(\x0b\x32-.apibara.starknet.v1alpha2.TransactionReceipt\"\xf8\x03\n\x0bTransaction\x12\x38\n\x04meta\x18\x01 \x01(\x0b\x32*.apibara.starknet.v1alpha2.TransactionMeta\x12\x43\n\tinvoke_v0\x18\x02 \x01(\x0b\x32..apibara.starknet.v1alpha2.InvokeTransactionV0H\x00\x12\x43\n\tinvoke_v1\x18\x03 \x01(\x0b\x32..apibara.starknet.v1alpha2.InvokeTransactionV1H\x00\x12>\n\x06\x64\x65ploy\x18\x04 \x01(\x0b\x32,.apibara.starknet.v1alpha2.DeployTransactionH\x00\x12@\n\x07\x64\x65\x63lare\x18\x05 \x01(\x0b\x32-.apibara.starknet.v1alpha2.DeclareTransactionH\x00\x12\x45\n\nl1_handler\x18\x06 \x01(\x0b\x32/.apibara.starknet.v1alpha2.L1HandlerTransactionH\x00\x12M\n\x0e\x64\x65ploy_account\x18\x07 \x01(\x0b\x32\x33.apibara.starknet.v1alpha2.DeployAccountTransactionH\x00\x42\r\n\x0btransaction\"\x87\x02\n\x0fTransactionMeta\x12\x35\n\x04hash\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x38\n\x07max_fee\x18\x02 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12:\n\tsignature\x18\x03 \x03(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x36\n\x05nonce\x18\x04 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x0f\n\x07version\x18\x05 \x01(\x04\"\xda\x01\n\x13InvokeTransactionV0\x12\x41\n\x10\x63ontract_address\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x45\n\x14\x65ntry_point_selector\x18\x02 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x39\n\x08\x63\x61lldata\x18\x03 \x03(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\x91\x01\n\x13InvokeTransactionV1\x12?\n\x0esender_address\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x39\n\x08\x63\x61lldata\x18\x02 \x03(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\xdf\x01\n\x11\x44\x65ployTransaction\x12\x45\n\x14\x63onstructor_calldata\x18\x02 \x03(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x46\n\x15\x63ontract_address_salt\x18\x03 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12;\n\nclass_hash\x18\x04 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\xd8\x01\n\x12\x44\x65\x63lareTransaction\x12;\n\nclass_hash\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12?\n\x0esender_address\x18\x02 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x44\n\x13\x63ompiled_class_hash\x18\x03 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\xdb\x01\n\x14L1HandlerTransaction\x12\x41\n\x10\x63ontract_address\x18\x02 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x45\n\x14\x65ntry_point_selector\x18\x03 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x39\n\x08\x63\x61lldata\x18\x04 \x03(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\xe6\x01\n\x18\x44\x65ployAccountTransaction\x12\x45\n\x14\x63onstructor_calldata\x18\x02 \x03(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x46\n\x15\x63ontract_address_salt\x18\x03 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12;\n\nclass_hash\x18\x04 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\xe9\x02\n\x12TransactionReceipt\x12\x41\n\x10transaction_hash\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x19\n\x11transaction_index\x18\x02 \x01(\x04\x12;\n\nactual_fee\x18\x03 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x43\n\x11l2_to_l1_messages\x18\x04 \x03(\x0b\x32(.apibara.starknet.v1alpha2.L2ToL1Message\x12\x30\n\x06\x65vents\x18\x05 \x03(\x0b\x32 .apibara.starknet.v1alpha2.Event\x12\x41\n\x10\x63ontract_address\x18\x06 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\xd6\x01\n\x1cL2ToL1MessageWithTransaction\x12;\n\x0btransaction\x18\x01 \x01(\x0b\x32&.apibara.starknet.v1alpha2.Transaction\x12>\n\x07receipt\x18\x02 \x01(\x0b\x32-.apibara.starknet.v1alpha2.TransactionReceipt\x12\x39\n\x07message\x18\x03 \x01(\x0b\x32(.apibara.starknet.v1alpha2.L2ToL1Message\"\xd4\x01\n\rL2ToL1Message\x12;\n\nto_address\x18\x03 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x38\n\x07payload\x18\x04 \x03(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\r\n\x05index\x18\x05 \x01(\x04\x12=\n\x0c\x66rom_address\x18\x06 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\xc4\x01\n\x14\x45ventWithTransaction\x12;\n\x0btransaction\x18\x01 \x01(\x0b\x32&.apibara.starknet.v1alpha2.Transaction\x12>\n\x07receipt\x18\x02 \x01(\x0b\x32-.apibara.starknet.v1alpha2.TransactionReceipt\x12/\n\x05\x65vent\x18\x03 \x01(\x0b\x32 .apibara.starknet.v1alpha2.Event\"\xc3\x01\n\x05\x45vent\x12=\n\x0c\x66rom_address\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x35\n\x04keys\x18\x02 \x03(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x35\n\x04\x64\x61ta\x18\x03 \x03(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\r\n\x05index\x18\x04 \x01(\x04\"\xbd\x01\n\x0bStateUpdate\x12\x39\n\x08new_root\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x39\n\x08old_root\x18\x02 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x38\n\nstate_diff\x18\x03 \x01(\x0b\x32$.apibara.starknet.v1alpha2.StateDiff\"\x9c\x03\n\tStateDiff\x12=\n\rstorage_diffs\x18\x01 \x03(\x0b\x32&.apibara.starknet.v1alpha2.StorageDiff\x12G\n\x12\x64\x65\x63lared_contracts\x18\x02 \x03(\x0b\x32+.apibara.starknet.v1alpha2.DeclaredContract\x12G\n\x12\x64\x65ployed_contracts\x18\x03 \x03(\x0b\x32+.apibara.starknet.v1alpha2.DeployedContract\x12\x36\n\x06nonces\x18\x04 \x03(\x0b\x32&.apibara.starknet.v1alpha2.NonceUpdate\x12\x42\n\x10\x64\x65\x63lared_classes\x18\x05 \x03(\x0b\x32(.apibara.starknet.v1alpha2.DeclaredClass\x12\x42\n\x10replaced_classes\x18\x06 \x03(\x0b\x32(.apibara.starknet.v1alpha2.ReplacedClass\"\x92\x01\n\x0bStorageDiff\x12\x41\n\x10\x63ontract_address\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12@\n\x0fstorage_entries\x18\x02 \x03(\x0b\x32'.apibara.starknet.v1alpha2.StorageEntry\"|\n\x0cStorageEntry\x12\x34\n\x03key\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x36\n\x05value\x18\x02 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"O\n\x10\x44\x65\x63laredContract\x12;\n\nclass_hash\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\x92\x01\n\rDeclaredClass\x12;\n\nclass_hash\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x44\n\x13\x63ompiled_class_hash\x18\x02 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\x8f\x01\n\rReplacedClass\x12\x41\n\x10\x63ontract_address\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12;\n\nclass_hash\x18\x02 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\x92\x01\n\x10\x44\x65ployedContract\x12\x41\n\x10\x63ontract_address\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12;\n\nclass_hash\x18\x02 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\"\x88\x01\n\x0bNonceUpdate\x12\x41\n\x10\x63ontract_address\x18\x01 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement\x12\x36\n\x05nonce\x18\x02 \x01(\x0b\x32'.apibara.starknet.v1alpha2.FieldElement*\xa2\x01\n\x0b\x42lockStatus\x12\x1c\n\x18\x42LOCK_STATUS_UNSPECIFIED\x10\x00\x12\x18\n\x14\x42LOCK_STATUS_PENDING\x10\x01\x12\x1f\n\x1b\x42LOCK_STATUS_ACCEPTED_ON_L2\x10\x02\x12\x1f\n\x1b\x42LOCK_STATUS_ACCEPTED_ON_L1\x10\x03\x12\x19\n\x15\x42LOCK_STATUS_REJECTED\x10\x04\x62\x06proto3"
 )
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "starknet_pb2", globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "starknet_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
     DESCRIPTOR._options = None
-    _BLOCKSTATUS._serialized_start = 5772
-    _BLOCKSTATUS._serialized_end = 5934
-    _BLOCK._serialized_start = 92
-    _BLOCK._serialized_end = 495
-    _BLOCKHEADER._serialized_start = 498
-    _BLOCKHEADER._serialized_end = 836
-    _TRANSACTIONWITHRECEIPT._serialized_start = 839
-    _TRANSACTIONWITHRECEIPT._serialized_end = 988
-    _TRANSACTION._serialized_start = 991
-    _TRANSACTION._serialized_end = 1495
-    _TRANSACTIONMETA._serialized_start = 1498
-    _TRANSACTIONMETA._serialized_end = 1761
-    _INVOKETRANSACTIONV0._serialized_start = 1764
-    _INVOKETRANSACTIONV0._serialized_end = 1982
-    _INVOKETRANSACTIONV1._serialized_start = 1985
-    _INVOKETRANSACTIONV1._serialized_end = 2130
-    _DEPLOYTRANSACTION._serialized_start = 2133
-    _DEPLOYTRANSACTION._serialized_end = 2356
-    _DECLARETRANSACTION._serialized_start = 2359
-    _DECLARETRANSACTION._serialized_end = 2575
-    _L1HANDLERTRANSACTION._serialized_start = 2578
-    _L1HANDLERTRANSACTION._serialized_end = 2797
-    _DEPLOYACCOUNTTRANSACTION._serialized_start = 2800
-    _DEPLOYACCOUNTTRANSACTION._serialized_end = 3030
-    _TRANSACTIONRECEIPT._serialized_start = 3033
-    _TRANSACTIONRECEIPT._serialized_end = 3394
-    _L2TOL1MESSAGEWITHTRANSACTION._serialized_start = 3397
-    _L2TOL1MESSAGEWITHTRANSACTION._serialized_end = 3611
-    _L2TOL1MESSAGE._serialized_start = 3614
-    _L2TOL1MESSAGE._serialized_end = 3826
-    _EVENTWITHTRANSACTION._serialized_start = 3829
-    _EVENTWITHTRANSACTION._serialized_end = 4025
-    _EVENT._serialized_start = 4028
-    _EVENT._serialized_end = 4223
-    _STATEUPDATE._serialized_start = 4226
-    _STATEUPDATE._serialized_end = 4415
-    _STATEDIFF._serialized_start = 4418
-    _STATEDIFF._serialized_end = 4830
-    _STORAGEDIFF._serialized_start = 4833
-    _STORAGEDIFF._serialized_end = 4979
-    _STORAGEENTRY._serialized_start = 4981
-    _STORAGEENTRY._serialized_end = 5105
-    _DECLAREDCONTRACT._serialized_start = 5107
-    _DECLAREDCONTRACT._serialized_end = 5186
-    _DECLAREDCLASS._serialized_start = 5189
-    _DECLAREDCLASS._serialized_end = 5335
-    _REPLACEDCLASS._serialized_start = 5338
-    _REPLACEDCLASS._serialized_end = 5481
-    _DEPLOYEDCONTRACT._serialized_start = 5484
-    _DEPLOYEDCONTRACT._serialized_end = 5630
-    _NONCEUPDATE._serialized_start = 5633
-    _NONCEUPDATE._serialized_end = 5769
+    _globals["_BLOCKSTATUS"]._serialized_start = 5772
+    _globals["_BLOCKSTATUS"]._serialized_end = 5934
+    _globals["_BLOCK"]._serialized_start = 92
+    _globals["_BLOCK"]._serialized_end = 495
+    _globals["_BLOCKHEADER"]._serialized_start = 498
+    _globals["_BLOCKHEADER"]._serialized_end = 836
+    _globals["_TRANSACTIONWITHRECEIPT"]._serialized_start = 839
+    _globals["_TRANSACTIONWITHRECEIPT"]._serialized_end = 988
+    _globals["_TRANSACTION"]._serialized_start = 991
+    _globals["_TRANSACTION"]._serialized_end = 1495
+    _globals["_TRANSACTIONMETA"]._serialized_start = 1498
+    _globals["_TRANSACTIONMETA"]._serialized_end = 1761
+    _globals["_INVOKETRANSACTIONV0"]._serialized_start = 1764
+    _globals["_INVOKETRANSACTIONV0"]._serialized_end = 1982
+    _globals["_INVOKETRANSACTIONV1"]._serialized_start = 1985
+    _globals["_INVOKETRANSACTIONV1"]._serialized_end = 2130
+    _globals["_DEPLOYTRANSACTION"]._serialized_start = 2133
+    _globals["_DEPLOYTRANSACTION"]._serialized_end = 2356
+    _globals["_DECLARETRANSACTION"]._serialized_start = 2359
+    _globals["_DECLARETRANSACTION"]._serialized_end = 2575
+    _globals["_L1HANDLERTRANSACTION"]._serialized_start = 2578
+    _globals["_L1HANDLERTRANSACTION"]._serialized_end = 2797
+    _globals["_DEPLOYACCOUNTTRANSACTION"]._serialized_start = 2800
+    _globals["_DEPLOYACCOUNTTRANSACTION"]._serialized_end = 3030
+    _globals["_TRANSACTIONRECEIPT"]._serialized_start = 3033
+    _globals["_TRANSACTIONRECEIPT"]._serialized_end = 3394
+    _globals["_L2TOL1MESSAGEWITHTRANSACTION"]._serialized_start = 3397
+    _globals["_L2TOL1MESSAGEWITHTRANSACTION"]._serialized_end = 3611
+    _globals["_L2TOL1MESSAGE"]._serialized_start = 3614
+    _globals["_L2TOL1MESSAGE"]._serialized_end = 3826
+    _globals["_EVENTWITHTRANSACTION"]._serialized_start = 3829
+    _globals["_EVENTWITHTRANSACTION"]._serialized_end = 4025
+    _globals["_EVENT"]._serialized_start = 4028
+    _globals["_EVENT"]._serialized_end = 4223
+    _globals["_STATEUPDATE"]._serialized_start = 4226
+    _globals["_STATEUPDATE"]._serialized_end = 4415
+    _globals["_STATEDIFF"]._serialized_start = 4418
+    _globals["_STATEDIFF"]._serialized_end = 4830
+    _globals["_STORAGEDIFF"]._serialized_start = 4833
+    _globals["_STORAGEDIFF"]._serialized_end = 4979
+    _globals["_STORAGEENTRY"]._serialized_start = 4981
+    _globals["_STORAGEENTRY"]._serialized_end = 5105
+    _globals["_DECLAREDCONTRACT"]._serialized_start = 5107
+    _globals["_DECLAREDCONTRACT"]._serialized_end = 5186
+    _globals["_DECLAREDCLASS"]._serialized_start = 5189
+    _globals["_DECLAREDCLASS"]._serialized_end = 5335
+    _globals["_REPLACEDCLASS"]._serialized_start = 5338
+    _globals["_REPLACEDCLASS"]._serialized_end = 5481
+    _globals["_DEPLOYEDCONTRACT"]._serialized_start = 5484
+    _globals["_DEPLOYEDCONTRACT"]._serialized_end = 5630
+    _globals["_NONCEUPDATE"]._serialized_start = 5633
+    _globals["_NONCEUPDATE"]._serialized_end = 5769
 # @@protoc_insertion_point(module_scope)
```

### Comparing `apibara-0.7.2/src/apibara/starknet/proto/starknet_pb2.pyi` & `apibara-0.7.3a0/src/apibara/starknet/proto/starknet_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -8,44 +8,53 @@
 from google.protobuf import message as _message
 from google.protobuf import timestamp_pb2 as _timestamp_pb2
 from google.protobuf.internal import containers as _containers
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 
 import apibara.starknet.proto.types_pb2 as _types_pb2
 
-BLOCK_STATUS_ACCEPTED_ON_L1: BlockStatus
-BLOCK_STATUS_ACCEPTED_ON_L2: BlockStatus
+DESCRIPTOR: _descriptor.FileDescriptor
+
+class BlockStatus(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+    __slots__ = []
+    BLOCK_STATUS_UNSPECIFIED: _ClassVar[BlockStatus]
+    BLOCK_STATUS_PENDING: _ClassVar[BlockStatus]
+    BLOCK_STATUS_ACCEPTED_ON_L2: _ClassVar[BlockStatus]
+    BLOCK_STATUS_ACCEPTED_ON_L1: _ClassVar[BlockStatus]
+    BLOCK_STATUS_REJECTED: _ClassVar[BlockStatus]
+
+BLOCK_STATUS_UNSPECIFIED: BlockStatus
 BLOCK_STATUS_PENDING: BlockStatus
+BLOCK_STATUS_ACCEPTED_ON_L2: BlockStatus
+BLOCK_STATUS_ACCEPTED_ON_L1: BlockStatus
 BLOCK_STATUS_REJECTED: BlockStatus
-BLOCK_STATUS_UNSPECIFIED: BlockStatus
-DESCRIPTOR: _descriptor.FileDescriptor
 
 class Block(_message.Message):
     __slots__ = [
-        "events",
-        "header",
-        "l2_to_l1_messages",
-        "state_update",
         "status",
+        "header",
         "transactions",
+        "state_update",
+        "events",
+        "l2_to_l1_messages",
     ]
-    EVENTS_FIELD_NUMBER: _ClassVar[int]
-    HEADER_FIELD_NUMBER: _ClassVar[int]
-    L2_TO_L1_MESSAGES_FIELD_NUMBER: _ClassVar[int]
-    STATE_UPDATE_FIELD_NUMBER: _ClassVar[int]
     STATUS_FIELD_NUMBER: _ClassVar[int]
+    HEADER_FIELD_NUMBER: _ClassVar[int]
     TRANSACTIONS_FIELD_NUMBER: _ClassVar[int]
-    events: _containers.RepeatedCompositeFieldContainer[EventWithTransaction]
+    STATE_UPDATE_FIELD_NUMBER: _ClassVar[int]
+    EVENTS_FIELD_NUMBER: _ClassVar[int]
+    L2_TO_L1_MESSAGES_FIELD_NUMBER: _ClassVar[int]
+    status: BlockStatus
     header: BlockHeader
+    transactions: _containers.RepeatedCompositeFieldContainer[TransactionWithReceipt]
+    state_update: StateUpdate
+    events: _containers.RepeatedCompositeFieldContainer[EventWithTransaction]
     l2_to_l1_messages: _containers.RepeatedCompositeFieldContainer[
         L2ToL1MessageWithTransaction
     ]
-    state_update: StateUpdate
-    status: BlockStatus
-    transactions: _containers.RepeatedCompositeFieldContainer[TransactionWithReceipt]
     def __init__(
         self,
         status: _Optional[_Union[BlockStatus, str]] = ...,
         header: _Optional[_Union[BlockHeader, _Mapping]] = ...,
         transactions: _Optional[
             _Iterable[_Union[TransactionWithReceipt, _Mapping]]
         ] = ...,
@@ -55,317 +64,362 @@
             _Iterable[_Union[L2ToL1MessageWithTransaction, _Mapping]]
         ] = ...,
     ) -> None: ...
 
 class BlockHeader(_message.Message):
     __slots__ = [
         "block_hash",
-        "block_number",
-        "new_root",
         "parent_block_hash",
+        "block_number",
         "sequencer_address",
+        "new_root",
         "timestamp",
     ]
     BLOCK_HASH_FIELD_NUMBER: _ClassVar[int]
-    BLOCK_NUMBER_FIELD_NUMBER: _ClassVar[int]
-    NEW_ROOT_FIELD_NUMBER: _ClassVar[int]
     PARENT_BLOCK_HASH_FIELD_NUMBER: _ClassVar[int]
+    BLOCK_NUMBER_FIELD_NUMBER: _ClassVar[int]
     SEQUENCER_ADDRESS_FIELD_NUMBER: _ClassVar[int]
+    NEW_ROOT_FIELD_NUMBER: _ClassVar[int]
     TIMESTAMP_FIELD_NUMBER: _ClassVar[int]
     block_hash: _types_pb2.FieldElement
-    block_number: int
-    new_root: _types_pb2.FieldElement
     parent_block_hash: _types_pb2.FieldElement
+    block_number: int
     sequencer_address: _types_pb2.FieldElement
+    new_root: _types_pb2.FieldElement
     timestamp: _timestamp_pb2.Timestamp
     def __init__(
         self,
         block_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
         parent_block_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
         block_number: _Optional[int] = ...,
         sequencer_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
         new_root: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
         timestamp: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ...,
     ) -> None: ...
 
-class DeclareTransaction(_message.Message):
-    __slots__ = ["class_hash", "compiled_class_hash", "sender_address"]
-    CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
-    COMPILED_CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
-    SENDER_ADDRESS_FIELD_NUMBER: _ClassVar[int]
-    class_hash: _types_pb2.FieldElement
-    compiled_class_hash: _types_pb2.FieldElement
-    sender_address: _types_pb2.FieldElement
+class TransactionWithReceipt(_message.Message):
+    __slots__ = ["transaction", "receipt"]
+    TRANSACTION_FIELD_NUMBER: _ClassVar[int]
+    RECEIPT_FIELD_NUMBER: _ClassVar[int]
+    transaction: Transaction
+    receipt: TransactionReceipt
     def __init__(
         self,
-        class_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
-        sender_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
-        compiled_class_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+        transaction: _Optional[_Union[Transaction, _Mapping]] = ...,
+        receipt: _Optional[_Union[TransactionReceipt, _Mapping]] = ...,
     ) -> None: ...
 
-class DeclaredClass(_message.Message):
-    __slots__ = ["class_hash", "compiled_class_hash"]
-    CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
-    COMPILED_CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
-    class_hash: _types_pb2.FieldElement
-    compiled_class_hash: _types_pb2.FieldElement
+class Transaction(_message.Message):
+    __slots__ = [
+        "meta",
+        "invoke_v0",
+        "invoke_v1",
+        "deploy",
+        "declare",
+        "l1_handler",
+        "deploy_account",
+    ]
+    META_FIELD_NUMBER: _ClassVar[int]
+    INVOKE_V0_FIELD_NUMBER: _ClassVar[int]
+    INVOKE_V1_FIELD_NUMBER: _ClassVar[int]
+    DEPLOY_FIELD_NUMBER: _ClassVar[int]
+    DECLARE_FIELD_NUMBER: _ClassVar[int]
+    L1_HANDLER_FIELD_NUMBER: _ClassVar[int]
+    DEPLOY_ACCOUNT_FIELD_NUMBER: _ClassVar[int]
+    meta: TransactionMeta
+    invoke_v0: InvokeTransactionV0
+    invoke_v1: InvokeTransactionV1
+    deploy: DeployTransaction
+    declare: DeclareTransaction
+    l1_handler: L1HandlerTransaction
+    deploy_account: DeployAccountTransaction
     def __init__(
         self,
-        class_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
-        compiled_class_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+        meta: _Optional[_Union[TransactionMeta, _Mapping]] = ...,
+        invoke_v0: _Optional[_Union[InvokeTransactionV0, _Mapping]] = ...,
+        invoke_v1: _Optional[_Union[InvokeTransactionV1, _Mapping]] = ...,
+        deploy: _Optional[_Union[DeployTransaction, _Mapping]] = ...,
+        declare: _Optional[_Union[DeclareTransaction, _Mapping]] = ...,
+        l1_handler: _Optional[_Union[L1HandlerTransaction, _Mapping]] = ...,
+        deploy_account: _Optional[_Union[DeployAccountTransaction, _Mapping]] = ...,
     ) -> None: ...
 
-class DeclaredContract(_message.Message):
-    __slots__ = ["class_hash"]
-    CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
-    class_hash: _types_pb2.FieldElement
+class TransactionMeta(_message.Message):
+    __slots__ = ["hash", "max_fee", "signature", "nonce", "version"]
+    HASH_FIELD_NUMBER: _ClassVar[int]
+    MAX_FEE_FIELD_NUMBER: _ClassVar[int]
+    SIGNATURE_FIELD_NUMBER: _ClassVar[int]
+    NONCE_FIELD_NUMBER: _ClassVar[int]
+    VERSION_FIELD_NUMBER: _ClassVar[int]
+    hash: _types_pb2.FieldElement
+    max_fee: _types_pb2.FieldElement
+    signature: _containers.RepeatedCompositeFieldContainer[_types_pb2.FieldElement]
+    nonce: _types_pb2.FieldElement
+    version: int
     def __init__(
-        self, class_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...
+        self,
+        hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+        max_fee: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+        signature: _Optional[
+            _Iterable[_Union[_types_pb2.FieldElement, _Mapping]]
+        ] = ...,
+        nonce: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+        version: _Optional[int] = ...,
     ) -> None: ...
 
-class DeployAccountTransaction(_message.Message):
-    __slots__ = ["class_hash", "constructor_calldata", "contract_address_salt"]
-    CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
-    CONSTRUCTOR_CALLDATA_FIELD_NUMBER: _ClassVar[int]
-    CONTRACT_ADDRESS_SALT_FIELD_NUMBER: _ClassVar[int]
-    class_hash: _types_pb2.FieldElement
-    constructor_calldata: _containers.RepeatedCompositeFieldContainer[
-        _types_pb2.FieldElement
-    ]
-    contract_address_salt: _types_pb2.FieldElement
+class InvokeTransactionV0(_message.Message):
+    __slots__ = ["contract_address", "entry_point_selector", "calldata"]
+    CONTRACT_ADDRESS_FIELD_NUMBER: _ClassVar[int]
+    ENTRY_POINT_SELECTOR_FIELD_NUMBER: _ClassVar[int]
+    CALLDATA_FIELD_NUMBER: _ClassVar[int]
+    contract_address: _types_pb2.FieldElement
+    entry_point_selector: _types_pb2.FieldElement
+    calldata: _containers.RepeatedCompositeFieldContainer[_types_pb2.FieldElement]
     def __init__(
         self,
-        constructor_calldata: _Optional[
-            _Iterable[_Union[_types_pb2.FieldElement, _Mapping]]
-        ] = ...,
-        contract_address_salt: _Optional[
+        contract_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+        entry_point_selector: _Optional[
             _Union[_types_pb2.FieldElement, _Mapping]
         ] = ...,
-        class_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+        calldata: _Optional[_Iterable[_Union[_types_pb2.FieldElement, _Mapping]]] = ...,
+    ) -> None: ...
+
+class InvokeTransactionV1(_message.Message):
+    __slots__ = ["sender_address", "calldata"]
+    SENDER_ADDRESS_FIELD_NUMBER: _ClassVar[int]
+    CALLDATA_FIELD_NUMBER: _ClassVar[int]
+    sender_address: _types_pb2.FieldElement
+    calldata: _containers.RepeatedCompositeFieldContainer[_types_pb2.FieldElement]
+    def __init__(
+        self,
+        sender_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+        calldata: _Optional[_Iterable[_Union[_types_pb2.FieldElement, _Mapping]]] = ...,
     ) -> None: ...
 
 class DeployTransaction(_message.Message):
-    __slots__ = ["class_hash", "constructor_calldata", "contract_address_salt"]
-    CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["constructor_calldata", "contract_address_salt", "class_hash"]
     CONSTRUCTOR_CALLDATA_FIELD_NUMBER: _ClassVar[int]
     CONTRACT_ADDRESS_SALT_FIELD_NUMBER: _ClassVar[int]
-    class_hash: _types_pb2.FieldElement
+    CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
     constructor_calldata: _containers.RepeatedCompositeFieldContainer[
         _types_pb2.FieldElement
     ]
     contract_address_salt: _types_pb2.FieldElement
+    class_hash: _types_pb2.FieldElement
     def __init__(
         self,
         constructor_calldata: _Optional[
             _Iterable[_Union[_types_pb2.FieldElement, _Mapping]]
         ] = ...,
         contract_address_salt: _Optional[
             _Union[_types_pb2.FieldElement, _Mapping]
         ] = ...,
         class_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
     ) -> None: ...
 
-class DeployedContract(_message.Message):
-    __slots__ = ["class_hash", "contract_address"]
+class DeclareTransaction(_message.Message):
+    __slots__ = ["class_hash", "sender_address", "compiled_class_hash"]
     CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
-    CONTRACT_ADDRESS_FIELD_NUMBER: _ClassVar[int]
+    SENDER_ADDRESS_FIELD_NUMBER: _ClassVar[int]
+    COMPILED_CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
     class_hash: _types_pb2.FieldElement
-    contract_address: _types_pb2.FieldElement
+    sender_address: _types_pb2.FieldElement
+    compiled_class_hash: _types_pb2.FieldElement
     def __init__(
         self,
-        contract_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
         class_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+        sender_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+        compiled_class_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
     ) -> None: ...
 
-class Event(_message.Message):
-    __slots__ = ["data", "from_address", "index", "keys"]
-    DATA_FIELD_NUMBER: _ClassVar[int]
-    FROM_ADDRESS_FIELD_NUMBER: _ClassVar[int]
-    INDEX_FIELD_NUMBER: _ClassVar[int]
-    KEYS_FIELD_NUMBER: _ClassVar[int]
-    data: _containers.RepeatedCompositeFieldContainer[_types_pb2.FieldElement]
-    from_address: _types_pb2.FieldElement
-    index: int
-    keys: _containers.RepeatedCompositeFieldContainer[_types_pb2.FieldElement]
-    def __init__(
-        self,
-        from_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
-        keys: _Optional[_Iterable[_Union[_types_pb2.FieldElement, _Mapping]]] = ...,
-        data: _Optional[_Iterable[_Union[_types_pb2.FieldElement, _Mapping]]] = ...,
-        index: _Optional[int] = ...,
-    ) -> None: ...
-
-class EventWithTransaction(_message.Message):
-    __slots__ = ["event", "receipt", "transaction"]
-    EVENT_FIELD_NUMBER: _ClassVar[int]
-    RECEIPT_FIELD_NUMBER: _ClassVar[int]
-    TRANSACTION_FIELD_NUMBER: _ClassVar[int]
-    event: Event
-    receipt: TransactionReceipt
-    transaction: Transaction
-    def __init__(
-        self,
-        transaction: _Optional[_Union[Transaction, _Mapping]] = ...,
-        receipt: _Optional[_Union[TransactionReceipt, _Mapping]] = ...,
-        event: _Optional[_Union[Event, _Mapping]] = ...,
-    ) -> None: ...
-
-class InvokeTransactionV0(_message.Message):
-    __slots__ = ["calldata", "contract_address", "entry_point_selector"]
-    CALLDATA_FIELD_NUMBER: _ClassVar[int]
+class L1HandlerTransaction(_message.Message):
+    __slots__ = ["contract_address", "entry_point_selector", "calldata"]
     CONTRACT_ADDRESS_FIELD_NUMBER: _ClassVar[int]
     ENTRY_POINT_SELECTOR_FIELD_NUMBER: _ClassVar[int]
-    calldata: _containers.RepeatedCompositeFieldContainer[_types_pb2.FieldElement]
+    CALLDATA_FIELD_NUMBER: _ClassVar[int]
     contract_address: _types_pb2.FieldElement
     entry_point_selector: _types_pb2.FieldElement
+    calldata: _containers.RepeatedCompositeFieldContainer[_types_pb2.FieldElement]
     def __init__(
         self,
         contract_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
         entry_point_selector: _Optional[
             _Union[_types_pb2.FieldElement, _Mapping]
         ] = ...,
         calldata: _Optional[_Iterable[_Union[_types_pb2.FieldElement, _Mapping]]] = ...,
     ) -> None: ...
 
-class InvokeTransactionV1(_message.Message):
-    __slots__ = ["calldata", "sender_address"]
-    CALLDATA_FIELD_NUMBER: _ClassVar[int]
-    SENDER_ADDRESS_FIELD_NUMBER: _ClassVar[int]
-    calldata: _containers.RepeatedCompositeFieldContainer[_types_pb2.FieldElement]
-    sender_address: _types_pb2.FieldElement
+class DeployAccountTransaction(_message.Message):
+    __slots__ = ["constructor_calldata", "contract_address_salt", "class_hash"]
+    CONSTRUCTOR_CALLDATA_FIELD_NUMBER: _ClassVar[int]
+    CONTRACT_ADDRESS_SALT_FIELD_NUMBER: _ClassVar[int]
+    CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
+    constructor_calldata: _containers.RepeatedCompositeFieldContainer[
+        _types_pb2.FieldElement
+    ]
+    contract_address_salt: _types_pb2.FieldElement
+    class_hash: _types_pb2.FieldElement
     def __init__(
         self,
-        sender_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
-        calldata: _Optional[_Iterable[_Union[_types_pb2.FieldElement, _Mapping]]] = ...,
+        constructor_calldata: _Optional[
+            _Iterable[_Union[_types_pb2.FieldElement, _Mapping]]
+        ] = ...,
+        contract_address_salt: _Optional[
+            _Union[_types_pb2.FieldElement, _Mapping]
+        ] = ...,
+        class_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
     ) -> None: ...
 
-class L1HandlerTransaction(_message.Message):
-    __slots__ = ["calldata", "contract_address", "entry_point_selector"]
-    CALLDATA_FIELD_NUMBER: _ClassVar[int]
+class TransactionReceipt(_message.Message):
+    __slots__ = [
+        "transaction_hash",
+        "transaction_index",
+        "actual_fee",
+        "l2_to_l1_messages",
+        "events",
+        "contract_address",
+    ]
+    TRANSACTION_HASH_FIELD_NUMBER: _ClassVar[int]
+    TRANSACTION_INDEX_FIELD_NUMBER: _ClassVar[int]
+    ACTUAL_FEE_FIELD_NUMBER: _ClassVar[int]
+    L2_TO_L1_MESSAGES_FIELD_NUMBER: _ClassVar[int]
+    EVENTS_FIELD_NUMBER: _ClassVar[int]
     CONTRACT_ADDRESS_FIELD_NUMBER: _ClassVar[int]
-    ENTRY_POINT_SELECTOR_FIELD_NUMBER: _ClassVar[int]
-    calldata: _containers.RepeatedCompositeFieldContainer[_types_pb2.FieldElement]
+    transaction_hash: _types_pb2.FieldElement
+    transaction_index: int
+    actual_fee: _types_pb2.FieldElement
+    l2_to_l1_messages: _containers.RepeatedCompositeFieldContainer[L2ToL1Message]
+    events: _containers.RepeatedCompositeFieldContainer[Event]
     contract_address: _types_pb2.FieldElement
-    entry_point_selector: _types_pb2.FieldElement
     def __init__(
         self,
+        transaction_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+        transaction_index: _Optional[int] = ...,
+        actual_fee: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+        l2_to_l1_messages: _Optional[_Iterable[_Union[L2ToL1Message, _Mapping]]] = ...,
+        events: _Optional[_Iterable[_Union[Event, _Mapping]]] = ...,
         contract_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
-        entry_point_selector: _Optional[
-            _Union[_types_pb2.FieldElement, _Mapping]
-        ] = ...,
-        calldata: _Optional[_Iterable[_Union[_types_pb2.FieldElement, _Mapping]]] = ...,
+    ) -> None: ...
+
+class L2ToL1MessageWithTransaction(_message.Message):
+    __slots__ = ["transaction", "receipt", "message"]
+    TRANSACTION_FIELD_NUMBER: _ClassVar[int]
+    RECEIPT_FIELD_NUMBER: _ClassVar[int]
+    MESSAGE_FIELD_NUMBER: _ClassVar[int]
+    transaction: Transaction
+    receipt: TransactionReceipt
+    message: L2ToL1Message
+    def __init__(
+        self,
+        transaction: _Optional[_Union[Transaction, _Mapping]] = ...,
+        receipt: _Optional[_Union[TransactionReceipt, _Mapping]] = ...,
+        message: _Optional[_Union[L2ToL1Message, _Mapping]] = ...,
     ) -> None: ...
 
 class L2ToL1Message(_message.Message):
-    __slots__ = ["from_address", "index", "payload", "to_address"]
-    FROM_ADDRESS_FIELD_NUMBER: _ClassVar[int]
-    INDEX_FIELD_NUMBER: _ClassVar[int]
-    PAYLOAD_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["to_address", "payload", "index", "from_address"]
     TO_ADDRESS_FIELD_NUMBER: _ClassVar[int]
-    from_address: _types_pb2.FieldElement
-    index: int
-    payload: _containers.RepeatedCompositeFieldContainer[_types_pb2.FieldElement]
+    PAYLOAD_FIELD_NUMBER: _ClassVar[int]
+    INDEX_FIELD_NUMBER: _ClassVar[int]
+    FROM_ADDRESS_FIELD_NUMBER: _ClassVar[int]
     to_address: _types_pb2.FieldElement
+    payload: _containers.RepeatedCompositeFieldContainer[_types_pb2.FieldElement]
+    index: int
+    from_address: _types_pb2.FieldElement
     def __init__(
         self,
         to_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
         payload: _Optional[_Iterable[_Union[_types_pb2.FieldElement, _Mapping]]] = ...,
         index: _Optional[int] = ...,
         from_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
     ) -> None: ...
 
-class L2ToL1MessageWithTransaction(_message.Message):
-    __slots__ = ["message", "receipt", "transaction"]
-    MESSAGE_FIELD_NUMBER: _ClassVar[int]
-    RECEIPT_FIELD_NUMBER: _ClassVar[int]
+class EventWithTransaction(_message.Message):
+    __slots__ = ["transaction", "receipt", "event"]
     TRANSACTION_FIELD_NUMBER: _ClassVar[int]
-    message: L2ToL1Message
-    receipt: TransactionReceipt
+    RECEIPT_FIELD_NUMBER: _ClassVar[int]
+    EVENT_FIELD_NUMBER: _ClassVar[int]
     transaction: Transaction
+    receipt: TransactionReceipt
+    event: Event
     def __init__(
         self,
         transaction: _Optional[_Union[Transaction, _Mapping]] = ...,
         receipt: _Optional[_Union[TransactionReceipt, _Mapping]] = ...,
-        message: _Optional[_Union[L2ToL1Message, _Mapping]] = ...,
+        event: _Optional[_Union[Event, _Mapping]] = ...,
     ) -> None: ...
 
-class NonceUpdate(_message.Message):
-    __slots__ = ["contract_address", "nonce"]
-    CONTRACT_ADDRESS_FIELD_NUMBER: _ClassVar[int]
-    NONCE_FIELD_NUMBER: _ClassVar[int]
-    contract_address: _types_pb2.FieldElement
-    nonce: _types_pb2.FieldElement
+class Event(_message.Message):
+    __slots__ = ["from_address", "keys", "data", "index"]
+    FROM_ADDRESS_FIELD_NUMBER: _ClassVar[int]
+    KEYS_FIELD_NUMBER: _ClassVar[int]
+    DATA_FIELD_NUMBER: _ClassVar[int]
+    INDEX_FIELD_NUMBER: _ClassVar[int]
+    from_address: _types_pb2.FieldElement
+    keys: _containers.RepeatedCompositeFieldContainer[_types_pb2.FieldElement]
+    data: _containers.RepeatedCompositeFieldContainer[_types_pb2.FieldElement]
+    index: int
     def __init__(
         self,
-        contract_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
-        nonce: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+        from_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+        keys: _Optional[_Iterable[_Union[_types_pb2.FieldElement, _Mapping]]] = ...,
+        data: _Optional[_Iterable[_Union[_types_pb2.FieldElement, _Mapping]]] = ...,
+        index: _Optional[int] = ...,
     ) -> None: ...
 
-class ReplacedClass(_message.Message):
-    __slots__ = ["class_hash", "contract_address"]
-    CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
-    CONTRACT_ADDRESS_FIELD_NUMBER: _ClassVar[int]
-    class_hash: _types_pb2.FieldElement
-    contract_address: _types_pb2.FieldElement
+class StateUpdate(_message.Message):
+    __slots__ = ["new_root", "old_root", "state_diff"]
+    NEW_ROOT_FIELD_NUMBER: _ClassVar[int]
+    OLD_ROOT_FIELD_NUMBER: _ClassVar[int]
+    STATE_DIFF_FIELD_NUMBER: _ClassVar[int]
+    new_root: _types_pb2.FieldElement
+    old_root: _types_pb2.FieldElement
+    state_diff: StateDiff
     def __init__(
         self,
-        contract_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
-        class_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+        new_root: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+        old_root: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+        state_diff: _Optional[_Union[StateDiff, _Mapping]] = ...,
     ) -> None: ...
 
 class StateDiff(_message.Message):
     __slots__ = [
-        "declared_classes",
+        "storage_diffs",
         "declared_contracts",
         "deployed_contracts",
         "nonces",
+        "declared_classes",
         "replaced_classes",
-        "storage_diffs",
     ]
-    DECLARED_CLASSES_FIELD_NUMBER: _ClassVar[int]
+    STORAGE_DIFFS_FIELD_NUMBER: _ClassVar[int]
     DECLARED_CONTRACTS_FIELD_NUMBER: _ClassVar[int]
     DEPLOYED_CONTRACTS_FIELD_NUMBER: _ClassVar[int]
     NONCES_FIELD_NUMBER: _ClassVar[int]
+    DECLARED_CLASSES_FIELD_NUMBER: _ClassVar[int]
     REPLACED_CLASSES_FIELD_NUMBER: _ClassVar[int]
-    STORAGE_DIFFS_FIELD_NUMBER: _ClassVar[int]
-    declared_classes: _containers.RepeatedCompositeFieldContainer[DeclaredClass]
+    storage_diffs: _containers.RepeatedCompositeFieldContainer[StorageDiff]
     declared_contracts: _containers.RepeatedCompositeFieldContainer[DeclaredContract]
     deployed_contracts: _containers.RepeatedCompositeFieldContainer[DeployedContract]
     nonces: _containers.RepeatedCompositeFieldContainer[NonceUpdate]
+    declared_classes: _containers.RepeatedCompositeFieldContainer[DeclaredClass]
     replaced_classes: _containers.RepeatedCompositeFieldContainer[ReplacedClass]
-    storage_diffs: _containers.RepeatedCompositeFieldContainer[StorageDiff]
     def __init__(
         self,
         storage_diffs: _Optional[_Iterable[_Union[StorageDiff, _Mapping]]] = ...,
         declared_contracts: _Optional[
             _Iterable[_Union[DeclaredContract, _Mapping]]
         ] = ...,
         deployed_contracts: _Optional[
             _Iterable[_Union[DeployedContract, _Mapping]]
         ] = ...,
         nonces: _Optional[_Iterable[_Union[NonceUpdate, _Mapping]]] = ...,
         declared_classes: _Optional[_Iterable[_Union[DeclaredClass, _Mapping]]] = ...,
         replaced_classes: _Optional[_Iterable[_Union[ReplacedClass, _Mapping]]] = ...,
     ) -> None: ...
 
-class StateUpdate(_message.Message):
-    __slots__ = ["new_root", "old_root", "state_diff"]
-    NEW_ROOT_FIELD_NUMBER: _ClassVar[int]
-    OLD_ROOT_FIELD_NUMBER: _ClassVar[int]
-    STATE_DIFF_FIELD_NUMBER: _ClassVar[int]
-    new_root: _types_pb2.FieldElement
-    old_root: _types_pb2.FieldElement
-    state_diff: StateDiff
-    def __init__(
-        self,
-        new_root: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
-        old_root: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
-        state_diff: _Optional[_Union[StateDiff, _Mapping]] = ...,
-    ) -> None: ...
-
 class StorageDiff(_message.Message):
     __slots__ = ["contract_address", "storage_entries"]
     CONTRACT_ADDRESS_FIELD_NUMBER: _ClassVar[int]
     STORAGE_ENTRIES_FIELD_NUMBER: _ClassVar[int]
     contract_address: _types_pb2.FieldElement
     storage_entries: _containers.RepeatedCompositeFieldContainer[StorageEntry]
     def __init__(
@@ -382,110 +436,62 @@
     value: _types_pb2.FieldElement
     def __init__(
         self,
         key: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
         value: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
     ) -> None: ...
 
-class Transaction(_message.Message):
-    __slots__ = [
-        "declare",
-        "deploy",
-        "deploy_account",
-        "invoke_v0",
-        "invoke_v1",
-        "l1_handler",
-        "meta",
-    ]
-    DECLARE_FIELD_NUMBER: _ClassVar[int]
-    DEPLOY_ACCOUNT_FIELD_NUMBER: _ClassVar[int]
-    DEPLOY_FIELD_NUMBER: _ClassVar[int]
-    INVOKE_V0_FIELD_NUMBER: _ClassVar[int]
-    INVOKE_V1_FIELD_NUMBER: _ClassVar[int]
-    L1_HANDLER_FIELD_NUMBER: _ClassVar[int]
-    META_FIELD_NUMBER: _ClassVar[int]
-    declare: DeclareTransaction
-    deploy: DeployTransaction
-    deploy_account: DeployAccountTransaction
-    invoke_v0: InvokeTransactionV0
-    invoke_v1: InvokeTransactionV1
-    l1_handler: L1HandlerTransaction
-    meta: TransactionMeta
+class DeclaredContract(_message.Message):
+    __slots__ = ["class_hash"]
+    CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
+    class_hash: _types_pb2.FieldElement
     def __init__(
-        self,
-        meta: _Optional[_Union[TransactionMeta, _Mapping]] = ...,
-        invoke_v0: _Optional[_Union[InvokeTransactionV0, _Mapping]] = ...,
-        invoke_v1: _Optional[_Union[InvokeTransactionV1, _Mapping]] = ...,
-        deploy: _Optional[_Union[DeployTransaction, _Mapping]] = ...,
-        declare: _Optional[_Union[DeclareTransaction, _Mapping]] = ...,
-        l1_handler: _Optional[_Union[L1HandlerTransaction, _Mapping]] = ...,
-        deploy_account: _Optional[_Union[DeployAccountTransaction, _Mapping]] = ...,
+        self, class_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...
     ) -> None: ...
 
-class TransactionMeta(_message.Message):
-    __slots__ = ["hash", "max_fee", "nonce", "signature", "version"]
-    HASH_FIELD_NUMBER: _ClassVar[int]
-    MAX_FEE_FIELD_NUMBER: _ClassVar[int]
-    NONCE_FIELD_NUMBER: _ClassVar[int]
-    SIGNATURE_FIELD_NUMBER: _ClassVar[int]
-    VERSION_FIELD_NUMBER: _ClassVar[int]
-    hash: _types_pb2.FieldElement
-    max_fee: _types_pb2.FieldElement
-    nonce: _types_pb2.FieldElement
-    signature: _containers.RepeatedCompositeFieldContainer[_types_pb2.FieldElement]
-    version: int
+class DeclaredClass(_message.Message):
+    __slots__ = ["class_hash", "compiled_class_hash"]
+    CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
+    COMPILED_CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
+    class_hash: _types_pb2.FieldElement
+    compiled_class_hash: _types_pb2.FieldElement
     def __init__(
         self,
-        hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
-        max_fee: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
-        signature: _Optional[
-            _Iterable[_Union[_types_pb2.FieldElement, _Mapping]]
-        ] = ...,
-        nonce: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
-        version: _Optional[int] = ...,
+        class_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+        compiled_class_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
     ) -> None: ...
 
-class TransactionReceipt(_message.Message):
-    __slots__ = [
-        "actual_fee",
-        "contract_address",
-        "events",
-        "l2_to_l1_messages",
-        "transaction_hash",
-        "transaction_index",
-    ]
-    ACTUAL_FEE_FIELD_NUMBER: _ClassVar[int]
+class ReplacedClass(_message.Message):
+    __slots__ = ["contract_address", "class_hash"]
     CONTRACT_ADDRESS_FIELD_NUMBER: _ClassVar[int]
-    EVENTS_FIELD_NUMBER: _ClassVar[int]
-    L2_TO_L1_MESSAGES_FIELD_NUMBER: _ClassVar[int]
-    TRANSACTION_HASH_FIELD_NUMBER: _ClassVar[int]
-    TRANSACTION_INDEX_FIELD_NUMBER: _ClassVar[int]
-    actual_fee: _types_pb2.FieldElement
+    CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
     contract_address: _types_pb2.FieldElement
-    events: _containers.RepeatedCompositeFieldContainer[Event]
-    l2_to_l1_messages: _containers.RepeatedCompositeFieldContainer[L2ToL1Message]
-    transaction_hash: _types_pb2.FieldElement
-    transaction_index: int
+    class_hash: _types_pb2.FieldElement
     def __init__(
         self,
-        transaction_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
-        transaction_index: _Optional[int] = ...,
-        actual_fee: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
-        l2_to_l1_messages: _Optional[_Iterable[_Union[L2ToL1Message, _Mapping]]] = ...,
-        events: _Optional[_Iterable[_Union[Event, _Mapping]]] = ...,
         contract_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+        class_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
     ) -> None: ...
 
-class TransactionWithReceipt(_message.Message):
-    __slots__ = ["receipt", "transaction"]
-    RECEIPT_FIELD_NUMBER: _ClassVar[int]
-    TRANSACTION_FIELD_NUMBER: _ClassVar[int]
-    receipt: TransactionReceipt
-    transaction: Transaction
+class DeployedContract(_message.Message):
+    __slots__ = ["contract_address", "class_hash"]
+    CONTRACT_ADDRESS_FIELD_NUMBER: _ClassVar[int]
+    CLASS_HASH_FIELD_NUMBER: _ClassVar[int]
+    contract_address: _types_pb2.FieldElement
+    class_hash: _types_pb2.FieldElement
     def __init__(
         self,
-        transaction: _Optional[_Union[Transaction, _Mapping]] = ...,
-        receipt: _Optional[_Union[TransactionReceipt, _Mapping]] = ...,
+        contract_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+        class_hash: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
     ) -> None: ...
 
-class BlockStatus(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
-    __slots__ = []
+class NonceUpdate(_message.Message):
+    __slots__ = ["contract_address", "nonce"]
+    CONTRACT_ADDRESS_FIELD_NUMBER: _ClassVar[int]
+    NONCE_FIELD_NUMBER: _ClassVar[int]
+    contract_address: _types_pb2.FieldElement
+    nonce: _types_pb2.FieldElement
+    def __init__(
+        self,
+        contract_address: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+        nonce: _Optional[_Union[_types_pb2.FieldElement, _Mapping]] = ...,
+    ) -> None: ...
```

### Comparing `apibara-0.7.2/src/apibara/starknet/proto/types_pb2.pyi` & `apibara-0.7.3a0/src/apibara/starknet/proto/types_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class FieldElement(_message.Message):
-    __slots__ = ["hi_hi", "hi_lo", "lo_hi", "lo_lo"]
-    HI_HI_FIELD_NUMBER: _ClassVar[int]
-    HI_LO_FIELD_NUMBER: _ClassVar[int]
-    LO_HI_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["lo_lo", "lo_hi", "hi_lo", "hi_hi"]
     LO_LO_FIELD_NUMBER: _ClassVar[int]
-    hi_hi: int
-    hi_lo: int
-    lo_hi: int
+    LO_HI_FIELD_NUMBER: _ClassVar[int]
+    HI_LO_FIELD_NUMBER: _ClassVar[int]
+    HI_HI_FIELD_NUMBER: _ClassVar[int]
     lo_lo: int
+    lo_hi: int
+    hi_lo: int
+    hi_hi: int
     def __init__(
         self,
         lo_lo: _Optional[int] = ...,
         lo_hi: _Optional[int] = ...,
         hi_lo: _Optional[int] = ...,
         hi_hi: _Optional[int] = ...,
     ) -> None: ...
```

### Comparing `apibara-0.7.2/PKG-INFO` & `apibara-0.7.3a0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apibara
-Version: 0.7.2
+Version: 0.7.3a0
 Summary: Apibara cliend SDK. Stream and transform on-chain data with Python.
 Home-page: https://www.apibara.com
 License: Apache-2.0
 Keywords: ethereum,web3,starknet
 Author: Francesco Ceccon
 Author-email: francesco@apibara.com
 Requires-Python: >=3.8,<3.11
@@ -32,18 +32,25 @@
     This SDK is alpha software. The API will change drastically until the beta.
 
     `Open an issue on GitHub <https://github.com/apibara/python-sdk>`_ to report bugs or provide feedback.
 
 
 Build web3-powered applications in Python. 
 
+
 Development
 -----------
 
-Install all dependencies with:
+Install the following packages using your OS package manager:
+
+* protobuf
+* poetry
+* docker (for testing)
+
+Install all Python dependencies with:
 
 .. code::
 
     poetry install
 
 Run tests with:
 
@@ -63,18 +70,30 @@
 .. code::
 
     protoc -I=protos/starknet/ \
         --python_out=src/apibara/starknet/proto/ \
         --pyi_out=src/apibara/starknet/proto protos/starknet/*
 
 
+Development (with Nix)
+----------------------
+
+This repository provides a Nix development environment. To use it simply run:
+
+.. code::
+
+   nix develop
+
+All dependencies, including pre-commit hooks, will be installed for you.
+
+
 License
 -------
 
-   Copyright 2022 GNC Labs Limited
+   Copyright 2023 GNC Labs Limited
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

