# Comparing `tmp/elytra_ms-0.0.2.1.tar.gz` & `tmp/elytra_ms-0.0.3.tar.gz`

## Comparing `elytra_ms-0.0.2.1.tar` & `elytra_ms-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,22 @@
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 elytra_ms-0.0.2.1/elytra/__init__.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 elytra_ms-0.0.2.1/elytra/const.py
--rw-r--r--   0        0        0    14292 2020-02-02 00:00:00.000000 elytra_ms-0.0.2.1/elytra/core.py
--rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 elytra_ms-0.0.2.1/elytra/protocols.py
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 elytra_ms-0.0.2.1/elytra/bedrock_realms/__init__.py
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 elytra_ms-0.0.2.1/elytra/bedrock_realms/models.py
--rw-r--r--   0        0        0     3293 2020-02-02 00:00:00.000000 elytra_ms-0.0.2.1/elytra/scripts/authenticate.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 elytra_ms-0.0.2.1/elytra/xbox/__init__.py
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 elytra_ms-0.0.2.1/elytra/xbox/core.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 elytra_ms-0.0.2.1/elytra/xbox/club/__init__.py
--rw-r--r--   0        0        0     4188 2020-02-02 00:00:00.000000 elytra_ms-0.0.2.1/elytra/xbox/club/models.py
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 elytra_ms-0.0.2.1/elytra/xbox/peoplehub/__init__.py
--rw-r--r--   0        0        0     6098 2020-02-02 00:00:00.000000 elytra_ms-0.0.2.1/elytra/xbox/peoplehub/models.py
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 elytra_ms-0.0.2.1/elytra/xbox/profile/__init__.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 elytra_ms-0.0.2.1/elytra/xbox/profile/models.py
--rw-r--r--   0        0        0     3713 2020-02-02 00:00:00.000000 elytra_ms-0.0.2.1/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 elytra_ms-0.0.2.1/LICENSE
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 elytra_ms-0.0.2.1/README.md
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 elytra_ms-0.0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 elytra_ms-0.0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 elytra_ms-0.0.3/elytra/__init__.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 elytra_ms-0.0.3/elytra/const.py
+-rw-r--r--   0        0        0    17304 2020-02-02 00:00:00.000000 elytra_ms-0.0.3/elytra/core.py
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 elytra_ms-0.0.3/elytra/protocols.py
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 elytra_ms-0.0.3/elytra/bedrock_realms/__init__.py
+-rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 elytra_ms-0.0.3/elytra/bedrock_realms/models.py
+-rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 elytra_ms-0.0.3/elytra/scripts/auth_device_code.py
+-rw-r--r--   0        0        0     3291 2020-02-02 00:00:00.000000 elytra_ms-0.0.3/elytra/scripts/authenticate.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 elytra_ms-0.0.3/elytra/xbox/__init__.py
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 elytra_ms-0.0.3/elytra/xbox/core.py
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 elytra_ms-0.0.3/elytra/xbox/rta.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 elytra_ms-0.0.3/elytra/xbox/club/__init__.py
+-rw-r--r--   0        0        0     4231 2020-02-02 00:00:00.000000 elytra_ms-0.0.3/elytra/xbox/club/models.py
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 elytra_ms-0.0.3/elytra/xbox/peoplehub/__init__.py
+-rw-r--r--   0        0        0     6098 2020-02-02 00:00:00.000000 elytra_ms-0.0.3/elytra/xbox/peoplehub/models.py
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 elytra_ms-0.0.3/elytra/xbox/profile/__init__.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 elytra_ms-0.0.3/elytra/xbox/profile/models.py
+-rw-r--r--   0        0        0     3713 2020-02-02 00:00:00.000000 elytra_ms-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 elytra_ms-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 elytra_ms-0.0.3/README.md
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 elytra_ms-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 elytra_ms-0.0.3/PKG-INFO
```

### Comparing `elytra_ms-0.0.2.1/elytra/core.py` & `elytra_ms-0.0.3/elytra/core.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,26 +2,28 @@
 import datetime
 import functools
 import typing
 
 import aiohttp
 import aiohttp_retry
 import msgspec
+import typing_extensions as typing_ext
 from aiohttp import ClientResponse
 
 from elytra.protocols import HandlerProtocol
 
 __all__ = (
     "BaseModel",
     "CamelBaseModel",
     "PascalBaseModel",
     "ParsableModel",
     "ParsableCamelModel",
     "ParsablePascalModel",
     "add_decoder",
+    "OAuth2TokenResponse",
     "AuthenticationManager",
     "MicrosoftAPIException",
     "BaseMicrosoftAPI",
 )
 
 
 class BetterResponse(aiohttp.ClientResponse):
@@ -41,22 +43,26 @@
 
 def utc_now() -> datetime.datetime:
     return datetime.datetime.now(datetime.UTC)
 
 
 class ParsableBase:
     if typing.TYPE_CHECKING:
-        _decoder: msgspec.json.Decoder[typing.Self]
+        _decoder: msgspec.json.Decoder[typing_ext.Self]
 
     @classmethod
-    def from_bytes(cls, obj: bytes) -> typing.Self:
+    def from_data(cls, obj: dict) -> typing_ext.Self:
+        return cls(**obj)
+
+    @classmethod
+    def from_bytes(cls, obj: bytes) -> typing_ext.Self:
         return cls._decoder.decode(obj)  # type: ignore
 
     @classmethod
-    async def from_response(cls, resp: aiohttp.ClientResponse) -> typing.Self:
+    async def from_response(cls, resp: aiohttp.ClientResponse) -> typing_ext.Self:
         return cls.from_bytes(await resp.read())
 
 
 class ParsableModel(msgspec.Struct, ParsableBase, kw_only=True):
     pass
 
 
@@ -98,15 +104,15 @@
     user_id: str
     issued: datetime.datetime = msgspec.field(default_factory=utc_now)
 
     def is_valid(self) -> bool:
         return (self.issued + datetime.timedelta(seconds=self.expires_in)) > utc_now()
 
     @classmethod
-    def from_file(cls, path: str) -> typing.Self:
+    def from_file(cls, path: str) -> typing_ext.Self:
         with open(path, "rb") as f:
             return cls.from_bytes(f.read())
 
 
 class XTokenResponse(ParsablePascalModel):
     issue_instant: datetime.datetime
     not_after: datetime.datetime
@@ -191,22 +197,50 @@
         self.relying_party = relying_party
 
         self.oauth = None  # type: ignore
         self.user_token = None  # type: ignore
         self.xsts_token = None  # type: ignore
 
     @classmethod
+    async def from_ouath(
+        cls,
+        session: aiohttp_retry.RetryClient,
+        client_id: str,
+        client_secret: str,
+        relying_party: str,
+        oauth: OAuth2TokenResponse,
+    ) -> typing_ext.Self:
+        self = cls(session, client_id, client_secret, relying_party)
+        self.oauth = oauth
+        await self.refresh_tokens()
+        return self
+
+    @classmethod
+    async def from_data(
+        cls,
+        session: aiohttp_retry.RetryClient,
+        client_id: str,
+        client_secret: str,
+        relying_party: str,
+        oauth_data: dict,
+    ) -> typing_ext.Self:
+        self = cls(session, client_id, client_secret, relying_party)
+        self.oauth = OAuth2TokenResponse.from_data(oauth_data)
+        await self.refresh_tokens()
+        return self
+
+    @classmethod
     async def from_file(
         cls,
         session: aiohttp_retry.RetryClient,
         client_id: str,
         client_secret: str,
         relying_party: str,
         oauth_path: str,
-    ) -> typing.Self:
+    ) -> typing_ext.Self:
         self = cls(session, client_id, client_secret, relying_party)
         self.oauth = OAuth2TokenResponse.from_file(oauth_path)
         await self.refresh_tokens()
         return self
 
     async def _oauth2_token_request(self, data: dict) -> OAuth2TokenResponse:
         """Execute token requests."""
@@ -369,17 +403,59 @@
     def __init__(
         self, session: aiohttp_retry.RetryClient, auth_mgr: AuthenticationManager
     ) -> None:
         self.session = session
         self.auth_mgr = auth_mgr
 
     @classmethod
+    async def from_oauth(
+        cls, client_id: str, client_secret: str, oauth: OAuth2TokenResponse
+    ) -> typing_ext.Self:
+        session = aiohttp_retry.RetryClient(
+            retry_options=CustomRetry(
+                attempts=3,
+                start_timeout=0.1,
+                random_interval_size=0.35,
+            ),
+            response_class=BetterResponse,
+            json_serialize=_dumps_wrapper,
+        )
+        auth_mgr = await AuthenticationManager.from_ouath(
+            session, client_id, client_secret, cls.RELYING_PATH, oauth
+        )
+        session._retry_options.evaluate_response_callback = functools.partial(
+            evaluate_response_callback, auth_mgr
+        )
+        return cls(session, auth_mgr)
+
+    @classmethod
+    async def from_data(
+        cls, client_id: str, client_secret: str, oauth_data: dict
+    ) -> typing_ext.Self:
+        session = aiohttp_retry.RetryClient(
+            retry_options=CustomRetry(
+                attempts=3,
+                start_timeout=0.1,
+                random_interval_size=0.35,
+            ),
+            response_class=BetterResponse,
+            json_serialize=_dumps_wrapper,
+        )
+        auth_mgr = await AuthenticationManager.from_data(
+            session, client_id, client_secret, cls.RELYING_PATH, oauth_data
+        )
+        session._retry_options.evaluate_response_callback = functools.partial(
+            evaluate_response_callback, auth_mgr
+        )
+        return cls(session, auth_mgr)
+
+    @classmethod
     async def from_file(
         cls, client_id: str, client_secret: str, oauth_path: str = "oauth.json"
-    ) -> typing.Self:
+    ) -> typing_ext.Self:
         session = aiohttp_retry.RetryClient(
             retry_options=CustomRetry(
                 attempts=3,
                 start_timeout=0.1,
                 random_interval_size=0.35,
             ),
             response_class=BetterResponse,
@@ -475,14 +551,33 @@
             url,
             json=json,
             data=data,
             params=params,
             headers=headers,
             **kwargs,
         )
+
+    async def put(
+        self,
+        url: str,
+        json: typing.Any = None,
+        data: typing.Optional[dict] = None,
+        params: typing.Optional[dict] = None,
+        headers: typing.Optional[dict] = None,
+        **kwargs: typing.Any,
+    ) -> aiohttp.ClientResponse:
+        return await self.request(
+            "PUT",
+            url,
+            json=json,
+            data=data,
+            params=params,
+            headers=headers,
+            **kwargs,
+        )
 
     async def delete(
         self,
         url: str,
         json: typing.Any = None,
         data: typing.Optional[dict] = None,
         params: typing.Optional[dict] = None,
```

### Comparing `elytra_ms-0.0.2.1/elytra/protocols.py` & `elytra_ms-0.0.3/elytra/protocols.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,25 @@
         data: typing.Optional[dict] = None,
         params: typing.Optional[dict] = None,
         headers: typing.Optional[dict] = None,
         **kwargs: typing.Any,
     ) -> aiohttp.ClientResponse:  # type: ignore
         pass
 
+    async def put(
+        self,
+        url: str,
+        json: typing.Any = None,
+        data: typing.Optional[dict] = None,
+        params: typing.Optional[dict] = None,
+        headers: typing.Optional[dict] = None,
+        **kwargs: typing.Any,
+    ) -> aiohttp.ClientResponse:  # type: ignore
+        pass
+
     async def delete(
         self,
         url: str,
         json: typing.Any = None,
         data: typing.Optional[dict] = None,
         params: typing.Optional[dict] = None,
         headers: typing.Optional[dict] = None,
```

### Comparing `elytra_ms-0.0.2.1/elytra/bedrock_realms/__init__.py` & `elytra_ms-0.0.3/elytra/bedrock_realms/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,14 +8,16 @@
     "State",
     "WorldType",
     "FullRealm",
     "MultiRealmResponse",
     "Player",
     "PartialRealm",
     "ActivityListResponse",
+    "PendingInvite",
+    "PendingInviteResponse",
     "BedrockRealmsAPI",
 )
 
 
 class BedrockRealmsAPI(BaseMicrosoftAPI):
     RELYING_PATH: str = BEDROCK_REALMS_API_URL
     BASE_URL: str = BEDROCK_REALMS_API_URL
@@ -32,14 +34,39 @@
         return await FullRealm.from_response(
             await self.post(f"invites/v1/link/accept/{code}")
         )
 
     async def fetch_realms(self) -> MultiRealmResponse:
         return await MultiRealmResponse.from_response(await self.get("worlds"))
 
+    async def invite_player(
+        self, realm_id: str | int, player_xuid: str | int
+    ) -> FullRealm:
+        return await FullRealm.from_response(
+            await self.put(
+                f"invites/{realm_id}/invite/update",
+                json={"invites": {str(player_xuid): "ADD"}},
+            )
+        )
+
+    async def fetch_pending_invite_count(self) -> int:
+        resp = await self.get("invites/count/pending")
+        return int(await resp.text())
+
+    async def fetch_pending_invites(self) -> PendingInviteResponse:
+        return await PendingInviteResponse.from_response(
+            await self.get("invites/pending")
+        )
+
+    async def accept_invite(self, invitation_id: str) -> None:
+        await self.put(f"invites/accept/{invitation_id}")
+
+    async def reject_invite(self, invitation_id: str) -> None:
+        await self.put(f"invites/reject/{invitation_id}")
+
     async def fetch_activities(self) -> ActivityListResponse:
         return await ActivityListResponse.from_response(
             await self.get("activities/live/players")
         )
 
     async def leave_realm(self, realm_id: int | str) -> None:
         await self.delete(f"invites/{realm_id}")
```

### Comparing `elytra_ms-0.0.2.1/elytra/scripts/authenticate.py` & `elytra_ms-0.0.3/elytra/scripts/authenticate.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
 async def async_main() -> None:
     global code
 
     parser = argparse.ArgumentParser(description="Authenticate into Microsoft's APIs.")
     parser.add_argument(
         "--file",
-        "-t",
+        "-f",
         default="oauth.json",
         help="Filepath to put output of program. Default: 'oauth.json'.",
     )
     parser.add_argument(
         "--client-id",
         "-cid",
         default=os.environ.get("CLIENT_ID"),
@@ -104,15 +104,15 @@
         auth_mgr = AuthenticationManager(
             aiohttp_retry.RetryClient(),
             args.client_id,
             args.client_secret,
             "http://xboxlive.com",
         )
         oauth = await auth_mgr.request_oauth_token(code, redirect_uri)
-        with open(args.tokens, mode="wb") as f:
+        with open(args.file, mode="wb") as f:
             f.write(msgspec.json.encode(oauth))
 
         await auth_mgr.close()
         print("Authentication successful!")  # noqa: T201
     else:
         print("Authentication failed.")  # noqa: T201
```

### Comparing `elytra_ms-0.0.2.1/elytra/xbox/club/__init__.py` & `elytra_ms-0.0.3/elytra/xbox/club/__init__.py`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.0.2.1/elytra/xbox/club/models.py` & `elytra_ms-0.0.3/elytra/xbox/club/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import typing
 from datetime import datetime
 from enum import IntEnum
 from uuid import UUID
 
 import msgspec
+import typing_extensions as typing_ext
 
 from elytra.core import CamelBaseModel, ParsableCamelModel, add_decoder
 
 __all__ = (
     "ClubUserPresence",
     "ClubDeeplinkMetadata",
     "ClubDeeplinks",
@@ -33,15 +34,15 @@
     CHAT = 2
     FEED = 3
     ROSTER = 4
     PLAY = 5
     IN_GAME = 6
 
     @classmethod
-    def from_xbox_api(cls, value: str) -> typing.Self:
+    def from_xbox_api(cls, value: str) -> typing_ext.Self:
         try:
             return cls[_camel_to_const_snake(value)]
         except KeyError:
             # it's not like i forgot a value, it's just that some are
             # literally not documented
             return cls.UNKNOWN
```

### Comparing `elytra_ms-0.0.2.1/elytra/xbox/peoplehub/__init__.py` & `elytra_ms-0.0.3/elytra/xbox/peoplehub/__init__.py`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.0.2.1/elytra/xbox/peoplehub/models.py` & `elytra_ms-0.0.3/elytra/xbox/peoplehub/models.py`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.0.2.1/elytra/xbox/profile/__init__.py` & `elytra_ms-0.0.3/elytra/xbox/profile/__init__.py`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.0.2.1/.gitignore` & `elytra_ms-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.0.2.1/LICENSE` & `elytra_ms-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.0.2.1/README.md` & `elytra_ms-0.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 TODO: actually do this section.
 
 ### Install Package
 
 Requires Python 3.10+.
 
 ```sh
-pip install -U elyta-ms
+pip install -U elytra-ms
 ```
 
 ### Make An Application
 
 > Taken from [xbox-webapi-python](https://github.com/OpenXbox/xbox-webapi-python) for now, copyright 2020 OpenXbox under MIT.
 
 Authentication is supported via OAuth2.
```

### Comparing `elytra_ms-0.0.2.1/pyproject.toml` & `elytra_ms-0.0.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 path = "elytra/__init__.py"
 
 [project.optional-dependencies]
 orjson = ["orjson"]
 
 [project.scripts]
 elytra-authenticate = "elytra.scripts.authenticate:main"
+elytra-device-code-auth = "elytra.scripts.auth_device_code:main"
 
 [tool.hatch.metadata.hooks.requirements_txt]
 files = ["requirements.txt"]
 
 [tool.hatch.build]
 include = ["elytra/**/*"]
```

### Comparing `elytra_ms-0.0.2.1/PKG-INFO` & `elytra_ms-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elytra-ms
-Version: 0.0.2.1
+Version: 0.0.3
 Summary: A Python Library for various Microsoft APIs, including the Xbox and Bedrock Realms APIs.
 Project-URL: Homepage, https://github.com/AstreaTSS/elytra-ms
 Author: AstreaTSS
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -12,14 +12,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Typing :: Typed
 Requires-Python: >=3.10
 Requires-Dist: aiohttp
 Requires-Dist: aiohttp-retry
 Requires-Dist: msgspec
+Requires-Dist: typing-extensions
 Provides-Extra: orjson
 Requires-Dist: orjson; extra == 'orjson'
 Description-Content-Type: text/markdown
 
 # elytra-ms
 A Python Library for various Microsoft APIs, including the Xbox and Bedrock Realms APIs.
 
@@ -44,15 +45,15 @@
 TODO: actually do this section.
 
 ### Install Package
 
 Requires Python 3.10+.
 
 ```sh
-pip install -U elyta-ms
+pip install -U elytra-ms
 ```
 
 ### Make An Application
 
 > Taken from [xbox-webapi-python](https://github.com/OpenXbox/xbox-webapi-python) for now, copyright 2020 OpenXbox under MIT.
 
 Authentication is supported via OAuth2.
```

