# Comparing `tmp/discordproxy-1.3.0.tar.gz` & `tmp/discordproxy-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discordproxy-1.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "discordproxy-1.3.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `discordproxy-1.3.0.tar` & `discordproxy-1.3.1.tar`

### file list

```diff
@@ -1,17 +1,29 @@
--rw-r--r--   0        0        0     1070 2023-04-29 14:16:52.177131 discordproxy-1.3.0/LICENSE
--rw-r--r--   0        0        0     1890 2021-03-13 18:29:37.317667 discordproxy-1.3.0/README.md
--rw-r--r--   0        0        0      110 2023-06-22 19:01:39.102674 discordproxy-1.3.0/discordproxy/__init__.py
--rw-r--r--   0        0        0     5721 2023-06-22 17:58:52.090919 discordproxy-1.3.0/discordproxy/_api.py
--rw-r--r--   0        0        0     1946 2022-04-08 13:27:28.023968 discordproxy-1.3.0/discordproxy/_cli.py
--rw-r--r--   0        0        0     3802 2021-12-28 15:54:50.403316 discordproxy-1.3.0/discordproxy/_config.py
--rw-r--r--   0        0        0       48 2021-12-28 15:54:50.407316 discordproxy-1.3.0/discordproxy/_constants.py
--rw-r--r--   0        0        0     2846 2021-12-29 19:54:56.084119 discordproxy-1.3.0/discordproxy/_decorators.py
--rw-r--r--   0        0        0      458 2021-12-28 15:54:50.407316 discordproxy-1.3.0/discordproxy/_discord_client.py
--rw-r--r--   0        0        0     3575 2021-12-29 20:20:01.968360 discordproxy-1.3.0/discordproxy/_server.py
--rw-r--r--   0        0        0     4031 2021-12-29 20:20:01.968360 discordproxy-1.3.0/discordproxy/client.py
--rw-r--r--   0        0        0    24933 2023-06-22 14:14:27.248149 discordproxy-1.3.0/discordproxy/discord_api_pb2.py
--rw-r--r--   0        0        0     5883 2023-06-22 14:14:27.248149 discordproxy-1.3.0/discordproxy/discord_api_pb2_grpc.py
--rw-r--r--   0        0        0     2611 2022-01-12 18:15:39.779155 discordproxy-1.3.0/discordproxy/exceptions.py
--rw-r--r--   0        0        0      733 2021-11-16 18:15:22.015918 discordproxy-1.3.0/discordproxy/helpers.py
--rw-r--r--   0        0        0     1394 2023-06-22 17:58:52.090919 discordproxy-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     2743 1970-01-01 00:00:00.000000 discordproxy-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-08-01 21:31:12.819419 discordproxy-1.3.1/LICENSE
+-rw-r--r--   0        0        0     1890 2023-08-01 21:31:12.819419 discordproxy-1.3.1/README.md
+-rw-r--r--   0        0        0      110 2023-08-01 21:31:12.819419 discordproxy-1.3.1/discordproxy/__init__.py
+-rw-r--r--   0        0        0     6096 2023-08-01 21:31:12.819419 discordproxy-1.3.1/discordproxy/_api.py
+-rw-r--r--   0        0        0     2003 2023-08-01 21:31:12.819419 discordproxy-1.3.1/discordproxy/_cli.py
+-rw-r--r--   0        0        0     3855 2023-08-01 21:31:12.819419 discordproxy-1.3.1/discordproxy/_config.py
+-rw-r--r--   0        0        0       90 2023-08-01 21:31:12.819419 discordproxy-1.3.1/discordproxy/_constants.py
+-rw-r--r--   0        0        0     2940 2023-08-01 21:31:12.819419 discordproxy-1.3.1/discordproxy/_decorators.py
+-rw-r--r--   0        0        0      630 2023-08-01 21:31:12.819419 discordproxy-1.3.1/discordproxy/_discord_client.py
+-rw-r--r--   0        0        0     3637 2023-08-01 21:31:12.819419 discordproxy-1.3.1/discordproxy/_server.py
+-rw-r--r--   0        0        0     4087 2023-08-01 21:31:12.819419 discordproxy-1.3.1/discordproxy/client.py
+-rw-r--r--   0        0        0    24933 2023-08-01 21:31:12.823420 discordproxy-1.3.1/discordproxy/discord_api_pb2.py
+-rw-r--r--   0        0        0     5883 2023-08-01 21:31:12.823420 discordproxy-1.3.1/discordproxy/discord_api_pb2_grpc.py
+-rw-r--r--   0        0        0     2780 2023-08-01 21:31:12.823420 discordproxy-1.3.1/discordproxy/exceptions.py
+-rw-r--r--   0        0        0      733 2023-08-01 21:31:12.823420 discordproxy-1.3.1/discordproxy/helpers.py
+-rw-r--r--   0        0        0        0 2023-08-01 21:49:47.819238 discordproxy-1.3.1/discordproxy/tests/__init__.py
+-rw-r--r--   0        0        0      930 2023-08-01 21:31:12.823420 discordproxy-1.3.1/discordproxy/tests/factories.py
+-rw-r--r--   0        0        0      841 2023-08-01 21:31:12.823420 discordproxy-1.3.1/discordproxy/tests/helpers.py
+-rw-r--r--   0        0        0     8290 2023-08-01 21:31:12.823420 discordproxy-1.3.1/discordproxy/tests/stubs.py
+-rw-r--r--   0        0        0     6732 2023-08-01 21:31:12.823420 discordproxy-1.3.1/discordproxy/tests/test_api.py
+-rw-r--r--   0        0        0     1551 2023-08-01 21:31:12.823420 discordproxy-1.3.1/discordproxy/tests/test_cli.py
+-rw-r--r--   0        0        0     4501 2023-08-01 21:31:12.823420 discordproxy-1.3.1/discordproxy/tests/test_client.py
+-rw-r--r--   0        0        0     2018 2023-08-01 21:31:12.823420 discordproxy-1.3.1/discordproxy/tests/test_config.py
+-rw-r--r--   0        0        0     1905 2023-08-01 21:31:12.823420 discordproxy-1.3.1/discordproxy/tests/test_end2end.py
+-rw-r--r--   0        0        0     2556 2023-08-01 21:31:12.823420 discordproxy-1.3.1/discordproxy/tests/test_exceptions.py
+-rw-r--r--   0        0        0     1073 2023-08-01 21:31:12.823420 discordproxy-1.3.1/discordproxy/tests/test_helpers.py
+-rw-r--r--   0        0        0     1886 2023-08-01 21:31:12.823420 discordproxy-1.3.1/discordproxy/tests/test_server.py
+-rw-r--r--   0        0        0     1411 2023-08-01 21:31:12.827420 discordproxy-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2743 1970-01-01 00:00:00.000000 discordproxy-1.3.1/PKG-INFO
```

### Comparing `discordproxy-1.3.0/LICENSE` & `discordproxy-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `discordproxy-1.3.0/README.md` & `discordproxy-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `discordproxy-1.3.0/discordproxy/_api.py` & `discordproxy-1.3.1/discordproxy/_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,18 @@
+"""Transform gRPC calls to Discord API calls."""
+
 import discord
 from google.protobuf import json_format
 
-from discordproxy import discord_api_pb2, discord_api_pb2_grpc
-from discordproxy._decorators import handle_discord_exceptions, log_request
+from . import discord_api_pb2, discord_api_pb2_grpc
+from ._decorators import handle_discord_exceptions, log_request
 
 
 def discord_to_grpc_embed(embed) -> discord_api_pb2.Embed:
+    """Convert a Discord embed to it's protobuf pendant."""
     embed_dict = embed.to_dict()
     return json_format.ParseDict(embed_dict, discord_api_pb2.Embed())
 
 
 # def discord_to_grpc_role(role) -> discord_api_pb2.Role:
 #     grpc_role = discord_api_pb2.Role(
 #         id=role.id,
@@ -31,14 +34,15 @@
 #         id=role_tag.bot_id,
 #         integration_id=role_tag.integration_id,
 #         premium_subscriber=role_tag.is_premium_subscriber(),
 #     )
 
 
 def discord_to_grpc_message(message) -> discord_api_pb2.Message:
+    """Convert a Discord message to it's protobuf pendant."""
     try:
         avatar = message.author.avatar.key
     except AttributeError:
         avatar = ""
     author = discord_api_pb2.User(
         id=message.author.id,
         username=message.author.name,
@@ -69,14 +73,15 @@
         embeds=[discord_to_grpc_embed(obj) for obj in message.embeds],
     )
 
 
 def discord_to_grpc_channel_type(
     channel_type: discord.ChannelType,
 ) -> discord_api_pb2.Channel.Type:
+    """Convert a Discord channel type to it's protobuf pendant."""
     type_map = {
         discord.ChannelType.text: discord_api_pb2.Channel.Type.GUILD_TEXT,
         discord.ChannelType.private: discord_api_pb2.Channel.Type.DM,
         discord.ChannelType.voice: discord_api_pb2.Channel.Type.GUILD_VOICE,
         discord.ChannelType.group: discord_api_pb2.Channel.Type.GROUP_DM,
         discord.ChannelType.category: discord_api_pb2.Channel.Type.GUILD_CATEGORY,
         discord.ChannelType.news: discord_api_pb2.Channel.Type.GUILD_NEWS,
@@ -85,14 +90,15 @@
     }
     return type_map.get(channel_type, discord_api_pb2.Channel.Type.UNDEFINED)
 
 
 def discord_to_grpc_channel(
     channel: discord.abc.GuildChannel,
 ) -> discord_api_pb2.Channel:
+    """Convert a Discord channel to it's protobuf pendant."""
     try:
         guild_id = channel.guild.id
     except AttributeError:
         guild_id = None
     try:
         topic = channel.topic
     except AttributeError:
@@ -112,15 +118,18 @@
         topic=topic,
         nsfw=nsfw,
         last_message_id=last_message_id,
         parent_id=channel.category_id,
     )
 
 
+# pylint: disable = invalid-overridden-method
 class DiscordApi(discord_api_pb2_grpc.DiscordApiServicer):
+    """Implementation of the discordproxy API."""
+
     def __init__(self, discord_client) -> None:
         super().__init__()
         self.discord_client = discord_client
 
     @log_request
     @handle_discord_exceptions(discord_api_pb2.SendChannelMessageResponse)
     async def SendChannelMessage(self, request, context):
```

### Comparing `discordproxy-1.3.0/discordproxy/_cli.py` & `discordproxy-1.3.1/discordproxy/_cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-"""Command line tool for sending messages to Discord server via gRPC."""
+"""Command line tools for sending messages to Discord server via gRPC."""
+
 import argparse
 import sys
 
 from discordproxy.client import DiscordClient
 from discordproxy.exceptions import DiscordProxyException
 
 from . import _constants
 
 
 def main():
+    """Main entry point for command line tools."""
     my_args = _parse_args(sys.argv[1:])
     target = f"{my_args.host}:{my_args.port}"
     client = DiscordClient(target=target)
     try:
         if my_args.type == "direct":
             client.create_direct_message(
                 user_id=my_args.recipient_id, content=my_args.content
@@ -21,15 +23,15 @@
             client.create_channel_message(
                 channel_id=my_args.recipient_id, content=my_args.content
             )
         else:
             raise NotImplementedError(my_args.type)
     except DiscordProxyException as ex:
         print(f"ERROR: {ex}")
-        exit(1)
+        sys.exit(1)
     else:
         print("Message sent")
 
 
 def _parse_args(sys_args: list) -> argparse.Namespace:
     parser = argparse.ArgumentParser(
         description=(
```

### Comparing `discordproxy-1.3.0/discordproxy/_config.py` & `discordproxy-1.3.1/discordproxy/_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,14 @@
+"""Configure discordproxy server."""
+
 import argparse
 import logging
 import logging.config
 import os
+import sys
 from pathlib import Path
 from typing import Tuple
 
 from . import __version__, _constants
 
 _LOG_FILE_NAME = "discordproxyserver.log"
 
@@ -14,15 +17,15 @@
     """Parse all command line arguments and configures logging."""
     my_args = _parse_args(args_list)
     token = (
         os.environ.get("DISCORD_BOT_TOKEN") if my_args.token is None else my_args.token
     )
     if not token:
         print("ERROR: No Discord bot token provided")
-        exit(1)
+        sys.exit(1)
     logging.config.dictConfig(_logging_config(my_args))
     return token, my_args
 
 
 def _parse_args(args_list: list) -> argparse.Namespace:
     """Return parsed command line arguments."""
     my_arg_parser = argparse.ArgumentParser(
```

### Comparing `discordproxy-1.3.0/discordproxy/_decorators.py` & `discordproxy-1.3.1/discordproxy/_decorators.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,25 @@
+"""Decorators for discordproxy."""
+
 import functools
 import json
 import logging
 
 import discord
 import grpc
 
 from discordproxy import discord_api_pb2
 
 logger = logging.getLogger(__name__)
 
 
-def handle_discord_exceptions(Response):
+def handle_discord_exceptions(response_class):
     """converts discord HTTP exceptions into gRPC context"""
 
-    _CODES_MAPPING = {
+    codes_mapping = {
         400: grpc.StatusCode.INVALID_ARGUMENT,
         401: grpc.StatusCode.UNAUTHENTICATED,
         403: grpc.StatusCode.PERMISSION_DENIED,
         404: grpc.StatusCode.NOT_FOUND,
         405: grpc.StatusCode.INVALID_ARGUMENT,
         429: grpc.StatusCode.RESOURCE_EXHAUSTED,
         500: grpc.StatusCode.INTERNAL,
@@ -36,25 +38,25 @@
                     func.__name__,
                     ex,
                     request,
                 )
                 details = _gen_grpc_error_details(
                     status=ex.status, code=ex.code, text=ex.text
                 )
-                context.set_code(_CODES_MAPPING.get(ex.status, grpc.StatusCode.UNKNOWN))
+                context.set_code(codes_mapping.get(ex.status, grpc.StatusCode.UNKNOWN))
                 context.set_details(json.dumps(details))
-                return Response()
-            except Exception as ex:
+                return response_class()
+            except Exception as ex:  # pylint: disable=broad-exception-caught
                 logger.warning(
                     "%s: Unexpected exception: %s:\n%s",
                     func.__name__,
                     ex,
                     request,
                 )
-                return Response()
+                return response_class()
 
         return decorated
 
     return wrapper
 
 
 def _gen_grpc_error_details(status: int, code: int, text: str):
```

### Comparing `discordproxy-1.3.0/discordproxy/_server.py` & `discordproxy-1.3.1/discordproxy/_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Server loop for discord proxy."""
+
 import argparse
 import asyncio
 import functools
 import logging
 import signal
 import sys
 import traceback
@@ -45,18 +47,18 @@
     logger.info("gRPC server has shut down")
 
 
 def _setup_handlers(grpc_server: grpc.aio.server, discord_client: DiscordClient):
     """Setup signal and exception handlers for the event loop."""
     loop = asyncio.get_running_loop()
     signals = (signal.SIGHUP, signal.SIGTERM, signal.SIGINT)
-    for s in signals:
+    for my_signal in signals:
         loop.add_signal_handler(
-            s,
-            lambda s=s: asyncio.create_task(
+            my_signal,
+            lambda s=my_signal: asyncio.create_task(
                 _shutdown_server(grpc_server, discord_client, s)
             ),
         )
     custom_exception_handler = functools.partial(
         _handle_uncaught_exception,
         grpc_server=grpc_server,
         discord_client=discord_client,
```

### Comparing `discordproxy-1.3.0/discordproxy/client.py` & `discordproxy-1.3.1/discordproxy/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Client API for external apps using discordproxy."""
+
 from typing import Iterable
 
 import grpc
 
 from .discord_api_pb2 import (
     Channel,
     Embed,
```

### Comparing `discordproxy-1.3.0/discordproxy/discord_api_pb2.py` & `discordproxy-1.3.1/discordproxy/discord_api_pb2.py`

 * *Files identical despite different names*

### Comparing `discordproxy-1.3.0/discordproxy/discord_api_pb2_grpc.py` & `discordproxy-1.3.1/discordproxy/discord_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `discordproxy-1.3.0/discordproxy/exceptions.py` & `discordproxy-1.3.1/discordproxy/exceptions.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,32 @@
+"""Custom exceptions for discordproxy."""
+
 from grpc import StatusCode as GrpcStatusCode
 
 from .helpers import parse_error_details
 
 
 def to_discord_proxy_exception(ex: Exception) -> "DiscordProxyException":
+    """Convert gRPC exception to a discordproxy exception.
+
+    Will remain unchanged if it is not a gRPC exception.
+    """
     if not hasattr(ex, "details"):
         return ex
+
     details = parse_error_details(ex)
     status = ex.code()
     if details.type == "HTTPException":
         return DiscordProxyHttpError(
             status=details.status, code=details.code, text=details.text
         )
-    elif status is GrpcStatusCode.DEADLINE_EXCEEDED:
+
+    if status is GrpcStatusCode.DEADLINE_EXCEEDED:
         return DiscordProxyTimeoutError(status=status, details=ex.details())
+
     return DiscordProxyGrpcError(status=status, details=ex.details())
 
 
 class DiscordProxyException(Exception):
     """An exception generated by Discord Proxy."""
```

### Comparing `discordproxy-1.3.0/discordproxy/helpers.py` & `discordproxy-1.3.1/discordproxy/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-"""Helpers for gRPC clients"""
+"""Helpers for client apps."""
+
 import json
 from collections import namedtuple
 
 import grpc
 
 GrpcErrorDetails = namedtuple("GrpcErrorDetails", ["type", "status", "code", "text"])
 
 
 def parse_error_details(grpc_error: grpc.RpcError) -> GrpcErrorDetails:
-    """Helper for parsing the details of a gRPC error exception into a nammed tuple.
+    """Helper for parsing the details of a gRPC error exception into a named tuple.
     Recognizes a Discord error encoded as JSON
     """
     details = grpc_error.details()
     try:
         data = json.loads(details)
     except json.decoder.JSONDecodeError:
         data = {"text": details}
```

### Comparing `discordproxy-1.3.0/PKG-INFO` & `discordproxy-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discordproxy
-Version: 1.3.0
+Version: 1.3.1
 Summary: Proxy server for accessing the Discord API via gRPC.
 Author-email: Erik Kalkoken <kalkoken87@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

