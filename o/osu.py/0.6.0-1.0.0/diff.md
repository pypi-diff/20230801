# Comparing `tmp/osu.py-0.6.0.tar.gz` & `tmp/osu.py-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osu.py-0.6.0.tar", last modified: Sat Mar 11 04:48:53 2023, max compression
+gzip compressed data, was "osu.py-1.0.0.tar", last modified: Tue Aug  1 01:17:49 2023, max compression
```

## Comparing `osu.py-0.6.0.tar` & `osu.py-1.0.0.tar`

### file list

```diff
@@ -1,50 +1,53 @@
-drwxrwxrwx   0        0        0        0 2023-03-11 04:48:53.369063 osu.py-0.6.0/
--rw-rw-rw-   0        0        0     1094 2022-06-04 07:49:48.000000 osu.py-0.6.0/LICENSE
--rw-rw-rw-   0        0        0      752 2023-03-11 04:48:53.368063 osu.py-0.6.0/PKG-INFO
--rw-rw-rw-   0        0        0     2858 2023-02-22 18:05:54.000000 osu.py-0.6.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-03-11 04:48:53.305065 osu.py-0.6.0/osu/
--rw-rw-rw-   0        0        0      395 2023-03-11 04:45:20.000000 osu.py-0.6.0/osu/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-11 04:48:53.321068 osu.py-0.6.0/osu/asyncio/
--rw-rw-rw-   0        0        0       40 2022-02-10 01:20:57.000000 osu.py-0.6.0/osu/asyncio/__init__.py
--rw-rw-rw-   0        0        0    85935 2023-03-11 04:01:24.000000 osu.py-0.6.0/osu/asyncio/client.py
--rw-rw-rw-   0        0        0     4389 2023-03-08 07:44:10.000000 osu.py-0.6.0/osu/asyncio/http.py
--rw-rw-rw-   0        0        0    10416 2022-12-28 20:34:54.000000 osu.py-0.6.0/osu/auth.py
--rw-rw-rw-   0        0        0    86095 2023-03-11 04:32:19.000000 osu.py-0.6.0/osu/client.py
--rw-rw-rw-   0        0        0     1144 2022-12-28 02:55:37.000000 osu.py-0.6.0/osu/constants.py
--rw-rw-rw-   0        0        0    27447 2023-03-11 04:13:13.000000 osu.py-0.6.0/osu/enums.py
--rw-rw-rw-   0        0        0       97 2021-06-15 19:50:18.000000 osu.py-0.6.0/osu/exceptions.py
--rw-rw-rw-   0        0        0     3718 2023-03-08 06:08:13.000000 osu.py-0.6.0/osu/http.py
--rw-rw-rw-   0        0        0     7386 2023-03-11 02:29:58.000000 osu.py-0.6.0/osu/notification.py
-drwxrwxrwx   0        0        0        0 2023-03-11 04:48:53.366063 osu.py-0.6.0/osu/objects/
--rw-rw-rw-   0        0        0      486 2023-02-22 18:22:11.000000 osu.py-0.6.0/osu/objects/__init__.py
--rw-rw-rw-   0        0        0    18227 2022-10-01 08:17:07.000000 osu.py-0.6.0/osu/objects/beatmap.py
--rw-rw-rw-   0        0        0     9443 2022-08-06 15:58:29.000000 osu.py-0.6.0/osu/objects/beatmapset_event.py
--rw-rw-rw-   0        0        0     5631 2022-08-04 12:22:52.000000 osu.py-0.6.0/osu/objects/build.py
--rw-rw-rw-   0        0        0     4191 2022-12-29 02:33:17.000000 osu.py-0.6.0/osu/objects/chat.py
--rw-rw-rw-   0        0        0     6659 2023-01-24 09:11:08.000000 osu.py-0.6.0/osu/objects/comment.py
--rw-rw-rw-   0        0        0     5891 2022-08-04 12:22:52.000000 osu.py-0.6.0/osu/objects/discussion.py
--rw-rw-rw-   0        0        0     4803 2022-08-04 13:44:11.000000 osu.py-0.6.0/osu/objects/event.py
--rw-rw-rw-   0        0        0     4915 2022-09-10 22:15:30.000000 osu.py-0.6.0/osu/objects/forum.py
--rw-rw-rw-   0        0        0     2458 2022-08-04 12:22:52.000000 osu.py-0.6.0/osu/objects/group.py
--rw-rw-rw-   0        0        0     1944 2022-08-04 13:35:30.000000 osu.py-0.6.0/osu/objects/kudosu.py
--rw-rw-rw-   0        0        0     2384 2022-08-06 06:00:57.000000 osu.py-0.6.0/osu/objects/match.py
--rw-rw-rw-   0        0        0    11960 2023-02-22 18:47:54.000000 osu.py-0.6.0/osu/objects/multiplayer.py
--rw-rw-rw-   0        0        0     2190 2023-01-24 07:59:10.000000 osu.py-0.6.0/osu/objects/news.py
--rw-rw-rw-   0        0        0    15924 2023-03-11 04:18:32.000000 osu.py-0.6.0/osu/objects/notification.py
--rw-rw-rw-   0        0        0     2869 2023-02-22 18:30:42.000000 osu.py-0.6.0/osu/objects/ranking.py
--rw-rw-rw-   0        0        0     1639 2022-12-28 02:53:50.000000 osu.py-0.6.0/osu/objects/scope.py
--rw-rw-rw-   0        0        0    10203 2023-02-22 19:23:52.000000 osu.py-0.6.0/osu/objects/score.py
--rw-rw-rw-   0        0        0     1175 2022-08-06 13:42:05.000000 osu.py-0.6.0/osu/objects/seasonal_background.py
--rw-rw-rw-   0        0        0    18844 2023-02-24 05:36:49.000000 osu.py-0.6.0/osu/objects/user.py
--rw-rw-rw-   0        0        0     1735 2023-01-24 08:11:16.000000 osu.py-0.6.0/osu/objects/wiki.py
--rw-rw-rw-   0        0        0     9884 2022-12-31 18:37:50.000000 osu.py-0.6.0/osu/path.py
--rw-rw-rw-   0        0        0    10692 2023-03-11 03:53:22.000000 osu.py-0.6.0/osu/util.py
-drwxrwxrwx   0        0        0        0 2023-03-11 04:48:53.314063 osu.py-0.6.0/osu.py.egg-info/
--rw-rw-rw-   0        0        0      752 2023-03-11 04:48:53.000000 osu.py-0.6.0/osu.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      893 2023-03-11 04:48:53.000000 osu.py-0.6.0/osu.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-11 04:48:53.000000 osu.py-0.6.0/osu.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      104 2023-03-11 04:48:53.000000 osu.py-0.6.0/osu.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-03-11 04:48:53.000000 osu.py-0.6.0/osu.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2021-04-22 23:57:23.000000 osu.py-0.6.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-11 04:48:53.369063 osu.py-0.6.0/setup.cfg
--rw-rw-rw-   0        0        0     1426 2023-01-25 22:37:21.000000 osu.py-0.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:17:49.485554 osu.py-1.0.0/
+-rw-rw-rw-   0        0        0     1094 2022-06-04 07:49:48.000000 osu.py-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0      752 2023-08-01 01:17:49.484556 osu.py-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2920 2023-04-10 17:44:41.000000 osu.py-1.0.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-08-01 01:17:49.447655 osu.py-1.0.0/osu/
+-rw-rw-rw-   0        0        0      419 2023-07-31 18:22:11.000000 osu.py-1.0.0/osu/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:17:49.463612 osu.py-1.0.0/osu/asyncio/
+-rw-rw-rw-   0        0        0       40 2022-02-10 01:20:57.000000 osu.py-1.0.0/osu/asyncio/__init__.py
+-rw-rw-rw-   0        0        0    84197 2023-08-01 00:30:22.000000 osu.py-1.0.0/osu/asyncio/client.py
+-rw-rw-rw-   0        0        0     4534 2023-07-31 03:17:18.000000 osu.py-1.0.0/osu/asyncio/http.py
+-rw-rw-rw-   0        0        0    10674 2023-07-09 07:36:16.000000 osu.py-1.0.0/osu/auth.py
+-rw-rw-rw-   0        0        0    83078 2023-08-01 00:29:26.000000 osu.py-1.0.0/osu/client.py
+-rw-rw-rw-   0        0        0     1145 2023-07-09 07:14:02.000000 osu.py-1.0.0/osu/constants.py
+-rw-rw-rw-   0        0        0    31450 2023-08-01 00:29:23.000000 osu.py-1.0.0/osu/enums.py
+-rw-rw-rw-   0        0        0       97 2021-06-15 19:50:18.000000 osu.py-1.0.0/osu/exceptions.py
+-rw-rw-rw-   0        0        0     3942 2023-07-21 05:54:31.000000 osu.py-1.0.0/osu/http.py
+-rw-rw-rw-   0        0        0     7488 2023-07-31 23:57:00.000000 osu.py-1.0.0/osu/notification.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:17:49.483559 osu.py-1.0.0/osu/objects/
+-rw-rw-rw-   0        0        0      554 2023-07-31 18:42:39.000000 osu.py-1.0.0/osu/objects/__init__.py
+-rw-rw-rw-   0        0        0     1222 2023-07-09 07:14:02.000000 osu.py-1.0.0/osu/objects/achievement.py
+-rw-rw-rw-   0        0        0    25325 2023-07-31 23:58:16.000000 osu.py-1.0.0/osu/objects/beatmap.py
+-rw-rw-rw-   0        0        0     9870 2023-07-09 07:36:16.000000 osu.py-1.0.0/osu/objects/beatmapset_event.py
+-rw-rw-rw-   0        0        0     6006 2023-07-09 07:36:16.000000 osu.py-1.0.0/osu/objects/build.py
+-rw-rw-rw-   0        0        0     4966 2023-07-31 18:23:23.000000 osu.py-1.0.0/osu/objects/chat.py
+-rw-rw-rw-   0        0        0     7460 2023-07-09 07:36:16.000000 osu.py-1.0.0/osu/objects/comment.py
+-rw-rw-rw-   0        0        0     4826 2023-07-09 07:36:16.000000 osu.py-1.0.0/osu/objects/current_user_attributes.py
+-rw-rw-rw-   0        0        0     8463 2023-07-31 18:23:24.000000 osu.py-1.0.0/osu/objects/discussion.py
+-rw-rw-rw-   0        0        0     8203 2023-07-31 18:44:40.000000 osu.py-1.0.0/osu/objects/event.py
+-rw-rw-rw-   0        0        0     5810 2023-07-31 23:59:49.000000 osu.py-1.0.0/osu/objects/forum.py
+-rw-rw-rw-   0        0        0     2416 2023-07-09 07:40:37.000000 osu.py-1.0.0/osu/objects/group.py
+-rw-rw-rw-   0        0        0     2138 2023-07-09 07:41:54.000000 osu.py-1.0.0/osu/objects/kudosu.py
+-rw-rw-rw-   0        0        0     5432 2023-08-01 00:00:54.000000 osu.py-1.0.0/osu/objects/match.py
+-rw-rw-rw-   0        0        0    12031 2023-07-31 18:23:24.000000 osu.py-1.0.0/osu/objects/multiplayer.py
+-rw-rw-rw-   0        0        0     2427 2023-07-09 08:22:08.000000 osu.py-1.0.0/osu/objects/news.py
+-rw-rw-rw-   0        0        0    17563 2023-07-09 08:22:51.000000 osu.py-1.0.0/osu/objects/notification.py
+-rw-rw-rw-   0        0        0     3165 2023-07-09 08:23:43.000000 osu.py-1.0.0/osu/objects/ranking.py
+-rw-rw-rw-   0        0        0     1691 2023-07-09 07:36:16.000000 osu.py-1.0.0/osu/objects/scope.py
+-rw-rw-rw-   0        0        0    12943 2023-08-01 00:03:25.000000 osu.py-1.0.0/osu/objects/score.py
+-rw-rw-rw-   0        0        0     1327 2023-07-09 07:36:16.000000 osu.py-1.0.0/osu/objects/seasonal_background.py
+-rw-rw-rw-   0        0        0    29154 2023-07-15 04:24:26.000000 osu.py-1.0.0/osu/objects/user.py
+-rw-rw-rw-   0        0        0     2001 2023-07-09 07:36:16.000000 osu.py-1.0.0/osu/objects/wiki.py
+-rw-rw-rw-   0        0        0    10122 2023-07-31 18:23:24.000000 osu.py-1.0.0/osu/path.py
+-rw-rw-rw-   0        0        0    11652 2023-07-31 23:57:23.000000 osu.py-1.0.0/osu/results.py
+-rw-rw-rw-   0        0        0    12076 2023-08-01 00:05:52.000000 osu.py-1.0.0/osu/util.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:17:49.460620 osu.py-1.0.0/osu.py.egg-info/
+-rw-rw-rw-   0        0        0      752 2023-08-01 01:17:49.000000 osu.py-1.0.0/osu.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      974 2023-08-01 01:17:49.000000 osu.py-1.0.0/osu.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 01:17:49.000000 osu.py-1.0.0/osu.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      104 2023-08-01 01:17:49.000000 osu.py-1.0.0/osu.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-08-01 01:17:49.000000 osu.py-1.0.0/osu.py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      143 2023-07-09 07:36:04.000000 osu.py-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-01 01:17:49.485554 osu.py-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1426 2023-01-25 22:37:21.000000 osu.py-1.0.0/setup.py
```

### Comparing `osu.py-0.6.0/LICENSE` & `osu.py-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `osu.py-0.6.0/PKG-INFO` & `osu.py-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osu.py
-Version: 0.6.0
+Version: 1.0.0
 Summary: API Wrapper for osu!api v2 written in Python.
 Home-page: https://github.com/Sheepposu/osu.py
 Author: Sheepposu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Sheepposu/osu.py/issues
 Project-URL: osu.py documentation, https://osupy.readthedocs.io/
 Project-URL: osu!api v2 documentation, https://osu.ppy.sh/docs/index.html
```

### Comparing `osu.py-0.6.0/README.rst` & `osu.py-1.0.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,15 @@
  - NotificationWebsocket class for using the notification websocket feature of osu api v2.
  - Support for Authorization Code Grant, Client Credentials Grant, and Password Grant (lazer auth).
  - Support for lazer authentication, giving access to all endpoints including those with lazer scope.
  - Currently implements most if not all endpoints including undocumented ones.
  - Builtin rate limit handling
  - Storage efficient objects used to contain almost all the data returned from osu.py for any given api request.
  - Refresh and access token is automatically managed.
+ - Utility functions and classes that make your life easier.
  - Documentation that covers everything osu.py is capable of.
 This uses osu!api v2, which is still under development. 
 So some code that was originally working may break overnight. 
 However, I'll do my best to fix any issues I find as quick as possible. 
 You can report issues `here <https://github.com/Sheepposu/osu.py/issues>`_
 or make a `pull requests <https://github.com/Sheepposu/osu.py/pulls>`_
 if you'd like to contribute. General discussion can go `here <https://github.com/Sheepposu/osu.py/discussions>`_
```

### Comparing `osu.py-0.6.0/osu/asyncio/client.py` & `osu.py-1.0.0/osu/asyncio/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,116 +1,169 @@
-"""
-Note: Docstrings in this file may be outdated due to laziness of not copying
-over docstring edits in the osu/client.py file.
-"""
-from .http import AsynchronousHTTPHandler as HTTPHandler
+from .http import AsynchronousHTTPHandler
 from ..objects import *
 from ..path import Path
 from ..enums import *
 from ..auth import AuthHandler, LazerAuthHandler
 from ..util import (
-    parse_mods_arg, parse_enum_args, BeatmapsetSearchFilter,
-    create_multipart_formdata, PlaylistItemUtil,
-    NotificationsUtil, IdentitiesUtil, JsonUtil
+    parse_mods_arg,
+    parse_enum_args,
+    BeatmapsetSearchFilter,
+    create_multipart_formdata,
+    PlaylistItemUtil,
+    IdentitiesUtil,
+    NotificationsUtil,
+    JsonUtil,
+    get_optional_list,
 )
-from typing import Union, Optional, Sequence, Dict
+from ..results import *
+
+from typing import Union, Optional, Sequence, Dict, List
 from datetime import datetime
 from osrparse import Replay
+from dateutil import parser
 import json
 
 
 class AsynchronousClient:
     """
-    Asyncio version of :class:`Client`. Functionality is all the same, but all functions are asynchronous.
+    Main object for interacting with osu!api, which uses asynchronous requests.
+    If you're looking for synchronous requests, use :class:`Client`.
+
+    All the functions of this class are documented under :class:`Client` and function the exact same.
+
+    **Init Parameters**
+
+    auth: :class:`AuthHandler`
+        The AuthHandler object passed in when initiating the Client object
+
+    request_wait_time: Optional[:class:`float`]
+        Default is 1.
+
+        This defines the amount of time that the client should wait before making another request.
+        It can make it easier to stay within the rate limits without using all your requests up quickly
+        and then waiting forever to make another. It's most applicable in bot-type apps.
+
+    limit_per_minute: Optional[:class:`float`]
+        Default is 60 because that's the limit peppy requests that we stay under.
+
+        This sets a cap on the number of requests the client is allowed to make within 1 minute of time.
+
+    use_lazer: Optional[:class:`bool`]
+        Default is False. This changes which base api endpoint the client will use.
+
+        Uses lazer.ppy.sh when True and osu.ppy.sh when False.
+
+    Make sure if you are changing the ratelimit handling that you are still following peppy's
+    TOU for using the API:
+
+    Use the API for good. Don't overdo it. If in doubt, ask before (ab)using :).
+    this section may expand as necessary.
+
+    Current rate limit is set at an insanely high 1200 requests per minute,
+    with burst capability of up to 200 beyond that.
+    If you require more, you probably fall into the above category of abuse.
+    If you are doing more than 60 requests a minute,
+    you should probably give peppy a yell.
     """
 
-    def __init__(self, auth: Union[AuthHandler, LazerAuthHandler] = None, request_wait_time: Optional[float] = 1.0,
-                 limit_per_minute: Optional[float] = 60.0, use_lazer: Optional[bool] = False):
+    def __init__(
+        self,
+        auth: Union[AuthHandler, LazerAuthHandler] = None,
+        request_wait_time: Optional[float] = 1.0,
+        limit_per_minute: Optional[float] = 60.0,
+        use_lazer: Optional[bool] = False,
+    ):
         self.auth = auth
-        self.http = HTTPHandler(self, request_wait_time, limit_per_minute, use_lazer)
+        self.http = AsynchronousHTTPHandler(self, request_wait_time, limit_per_minute, use_lazer)
 
     @classmethod
-    def from_client_credentials(cls, client_id: int, client_secret: str, redirect_url: str,
-                                scope: Optional[Scope] = Scope.default(), code: Optional[str] = None,
-                                request_wait_time: Optional[float] = 1.0,
-                                limit_per_minute: Optional[float] = 60.0):
+    def from_client_credentials(
+        cls,
+        client_id: int,
+        client_secret: str,
+        redirect_url: Optional[str],
+        scope: Optional[Scope] = Scope.default(),
+        code: Optional[str] = None,
+        request_wait_time: Optional[float] = 1.0,
+        limit_per_minute: Optional[float] = 60.0,
+    ) -> "AsynchronousClient":
         """
         Returns a :class:`Client` object from client id, client secret, redirect uri, and scope.
 
         **Parameters**
 
         client_id: :class:`int`
             API Client id
 
         client_secret: :class:`int`
             API Client secret
 
-        redirect_uri: :class:`str`
+        redirect_uri: Optional[:class:`str`]
             API redirect uri
 
         scope: Optional[:class:`Scope`]
             Scopes to use. Default is Scope.default() which is just the public scope.
 
         code: Optional[:class:`str`]
             If provided, is used to authorize. Read more about this under :class:`AuthHandler.get_auth_token`
 
         request_wait_time: Optional[:class:`float`]
-            Read under Client init parameters.
+            Default is 1.
+
+            This defines the amount of time that the client should wait before making another request.
+            It can make it easier to stay within the rate limits without using all your requests up quickly
+            and then waiting forever to make another. It's most applicable in bot-type apps.
 
         limit_per_minute: Optional[:class:`float`]
-            Read under Client init parameters.
+            Default is 60 because that's the limit peppy requests that we stay under.
+
+            This sets a cap on the number of requests the client is allowed to make within 1 minute of time.
 
         **Returns**
 
         :class:`Client`
         """
         auth = AuthHandler(client_id, client_secret, redirect_url, scope)
         auth.get_auth_token(code)
         return cls(auth, request_wait_time, limit_per_minute)
 
     @classmethod
-    def from_osu_credentials(cls, username: str, password: str,
-                             request_wait_time: Optional[float] = 1.0,
-                             limit_per_minute: Optional[float] = 60.0):
+    def from_osu_credentials(
+        cls,
+        username: str,
+        password: str,
+        request_wait_time: Optional[float] = 1.0,
+        limit_per_minute: Optional[float] = 60.0,
+    ) -> "AsynchronousClient":
         """
-        Returns a :class:`Client` object from client id, client secret, redirect uri, and scope.
-
-        **Parameters**
+        Returns a :class:`Client` object which will make authorize and make requests to
+        lazer.ppy.sh
 
-        client_id: :class:`int`
-            API Client id
+        username: :class:`str`
+            osu! username login
 
-        client_secret: :class:`int`
-            API Client secret
-
-        redirect_uri: :class:`str`
-            API redirect uri
-
-        scope: Optional[:class:`Scope`]
-            Scopes to use. Default is Scope.default() which is just the public scope.
-
-        code: Optional[:class:`str`]
-            If provided, is used to authorize. Read more about this under :class:`AuthHandler.get_auth_token`
+        password: :class:`str`
+            osu! password login
 
         request_wait_time: Optional[:class:`float`]
             Read under Client init parameters.
 
         limit_per_minute: Optional[:class:`float`]
             Read under Client init parameters.
-
-        **Returns**
-
-        :class:`Client`
         """
         auth = LazerAuthHandler(username, password)
         auth.get_auth_token()
         return cls(auth, request_wait_time, limit_per_minute, True)
 
-    async def lookup_beatmap(self, checksum: Optional[str] = None, filename: Optional[str] = None,
-                       id: Optional[int] = None) -> Beatmap:
+    async def lookup_beatmap(
+        self,
+        checksum: Optional[str] = None,
+        filename: Optional[str] = None,
+        id: Optional[int] = None,
+    ) -> Beatmap:
         """
         Returns beatmap.
 
         Requires OAuth and scope public
 
         **Parameters**
 
@@ -123,19 +176,23 @@
         id: Optional[:class:`int`]
             A beatmap ID to lookup
 
         **Returns**
 
         :class:`Beatmap`
         """
-        return Beatmap(await self.http.make_request(Path.beatmap_lookup(), checksum=checksum,
-                                              filename=filename, id=id))
+        return Beatmap(await self.http.make_request(Path.beatmap_lookup(), checksum=checksum, filename=filename, id=id))
 
-    async def get_user_beatmap_score(self, beatmap: int, user: int, mode: Optional[Union[str, GameModeStr]] = None,
-                               mods: Optional[Sequence[str]] = None) -> BeatmapUserScore:
+    async def get_user_beatmap_score(
+        self,
+        beatmap: int,
+        user: int,
+        mode: Optional[Union[str, GameModeStr]] = None,
+        mods: Optional[Sequence[str]] = None,
+    ) -> BeatmapUserScore:
         """
         Returns a user's score on a Beatmap
 
         Requires OAuth and scope public
 
         **Parameters**
 
@@ -152,19 +209,21 @@
             An array of matching mods, or none. Currently doesn't do anything.
 
         **Returns**
 
         :class:`BeatmapUserScore`
         """
         mode = parse_enum_args(mode)
-        return BeatmapUserScore(await self.http.make_request(Path.user_beatmap_score(beatmap, user),
-                                                       mode=mode, mods=mods))
-
-    async def get_user_beatmap_scores(self, beatmap: int, user: int,
-                                mode: Optional[Union[str, GameModeStr]] = None) -> Sequence[LegacyScore]:
+        return BeatmapUserScore(
+            await self.http.make_request(Path.user_beatmap_score(beatmap, user), mode=mode, mods=mods)
+        )
+
+    async def get_user_beatmap_scores(
+        self, beatmap: int, user: int, mode: Optional[Union[str, GameModeStr]] = None
+    ) -> List[Union[LegacyScore, SoloScore]]:
         """
         Returns a user's scores on a Beatmap
 
         Requires OAuth and scope public
 
         **Parameters**
 
@@ -175,81 +234,123 @@
             Id of the user
 
         mode: Optional[Union[:class:`str`, :class:`GameModeStr`]]
             The game mode to get scores for
 
         **Returns**
 
-        Sequence[:class:`LegacyScore`]
+        List[Union[:class:`LegacyScore`, :class:`SoloScore`]]
         """
         mode = parse_enum_args(mode)
-        return list(map(LegacyScore, (await self.http.make_request(Path.user_beatmap_scores(beatmap, user),
-                                                                   mode=mode))["scores"]))
-
-    async def get_beatmap_scores(self, beatmap: int, mode: Optional[Union[str, GameModeStr]] = None,
-                           mods: Optional[Sequence[str]] = None,
-                           type: Optional[Sequence[str]] = None) -> BeatmapScores:
+        resp = await self.http.make_request(Path.user_beatmap_scores(beatmap, user), mode=mode)
+        return list(
+            map(
+                get_score_object,
+                resp["scores"],
+            )
+        )
+
+    def _parse_mods_list(self, mods) -> Optional[List[str]]:
+        if mods is None:
+            return
+        return list(
+            map(
+                lambda mod: (Mod[mod.name].value if not isinstance(mod, Mod) else mod.value)
+                if type(mod) != str
+                else mod,
+                mods,
+            )
+        )
+
+    async def get_beatmap_scores(
+        self,
+        beatmap: int,
+        mode: Optional[Union[str, GameModeStr]] = None,
+        mods: Optional[Union[Mods, Sequence[Union[Mods, Mod, str]]]] = None,
+        ranking_type: Optional[str] = None,
+    ) -> BeatmapScores:
         """
         Returns the top scores for a beatmap
 
         Requires OAuth and scope public
 
         **Parameters**
 
         beatmap: :class:`int`
             Id of the beatmap
 
         mode: Optional[Union[:class:`str`, :class:`GameModeStr`]]
             The game mode to get scores for
 
-        mods: Optional[Sequence[:class:`str`]]
-            An array of matching mods, or none. Currently doesn't do anything.
+        mods: Optional[Union[:class:`Mods`, Sequence[Union[:class:`Mods`, :class:`Mod`, :class:`str`]]]]
+            Must pass one of:
+            a :class:`Mods` object,
+            a list of string mod abbreviations,
+            a list of :class:`Mods` objects,
+            a list of :classL`Mod` objects
 
-        type: Optional[Sequence[:class:`str`]]
+        ranking_type: Optional[:class:`str`]
             Beatmap score ranking type. Currently doesn't do anything.
 
         **Returns**
 
         :class:`BeatmapScores`
             :class:`LegacyScore` object inside includes "user" and the included user includes "country" and "cover".
         """
         mode = parse_enum_args(mode)
-        return BeatmapScores(await self.http.make_request(Path.beatmap_scores(beatmap), mode=mode,
-                                                    mods=mods, type=type))
-
-    async def get_lazer_beatmap_scores(self, beatmap: int, mode: Optional[Union[str, GameModeStr]] = None,
-                                 mods: Optional[Sequence[str]] = None,
-                                 type: Optional[Sequence[str]] = None) -> BeatmapScores:
+        mods = self._parse_mods_list(mods)
+        return BeatmapScores(
+            await self.http.make_request(
+                Path.beatmap_scores(beatmap),
+                mode=mode,
+                **{"mods[]": mods},
+                type=ranking_type,
+            )
+        )
+
+    async def get_lazer_beatmap_scores(
+        self,
+        beatmap: int,
+        mode: Optional[Union[str, GameModeStr]] = None,
+        mods: Optional[str] = None,
+        type: Optional[str] = None,
+    ) -> BeatmapScores:
         """
         Returns the top scores for a beatmap on the lazer client.
 
         Requires OAuth and scope public
 
         **Parameters**
 
         beatmap: :class:`int`
-            Id of the beatmap
+            ID of the beatmap
 
         mode: Optional[Union[:class:`str`, :class:`GameModeStr`]]
             The game mode to get scores for
 
-        mods: Optional[Sequence[:class:`str`]]
-            An array of matching mods, or none. Currently doesn't do anything.
+        mods: Optional[:class:`str`]
+            Must pass one of:
+            a :class:`Mods` object,
+            a list of string mod abbreviations,
+            a list of :class:`Mods` objects,
+            a list of :classL`Mod` objects
 
-        type: Optional[Sequence[:class:`str`]]
+        type: Optional[:class:`str`]
             Beatmap score ranking type. Currently doesn't do anything.
 
         **Returns**
 
         :class:`BeatmapScores`
-            :class:`LazerScore` object inside includes "user" and the included user includes "country" and "cover".
+            :class:`SoloScore` object inside includes "user" and the included user includes "country" and "cover".
         """
         mode = parse_enum_args(mode)
-        return BeatmapScores(await self.http.make_request(Path.lazer_beatmap_scores(beatmap), mode=mode,
-                                                    mods=mods, type=type), "lazer")
+        mods = self._parse_mods_list(mods)
+        return BeatmapScores(
+            await self.http.make_request(Path.lazer_beatmap_scores(beatmap), mode=mode, mods=mods, type=type)
+        )
 
     async def get_beatmap(self, beatmap: int) -> Beatmap:
         """
         Gets beatmap data for the specified beatmap ID.
 
         Requires OAuth and scope public
 
@@ -257,71 +358,79 @@
 
         beatmap: :class:`int`
             The ID of the beatmap
 
         **Returns**
 
         :class:`Beatmap`
-            Includes attributes beatmapset, failtimes, and max_combo
+            Includes attributes `beatmapset`, `beatmapset.ratings`, `failtimes`, `max_combo`.
         """
         return Beatmap(await self.http.make_request(Path.beatmap(beatmap)))
 
-    async def get_beatmaps(self, ids: Optional[Sequence[int]] = None) -> Sequence[Beatmap]:
+    async def get_beatmaps(self, ids: Optional[Sequence[int]] = None) -> List[Beatmap]:
         """
         Returns list of beatmaps.
 
         Requires OAuth and scope public
 
         **Parameters**
 
         ids: Optional[List[:class:`int`]]
             Beatmap id to be returned. Specify once for each beatmap id requested.
             Up to 50 beatmaps can be requested at once.
 
         **Returns**
 
-        Sequence[:class:`BeatmapCompact`]
-            Includes: beatmapset (with ratings), failtimes, max_combo.
+        List[:class:`Beatmap`]
+            Includes attributes `beatmapset`, `beatmapset.ratings`, `failtimes`, `max_combo`.
         """
-        results = await self.http.make_request(Path.beatmaps(), **{"ids[]": ids})
-        return list(map(Beatmap, results['beatmaps'])) if results else []
+        results = await self.http.make_request(Path.beatmaps(), **{"ids[]": list(ids)})
+        return list(map(Beatmap, results["beatmaps"])) if results else []
 
-    async def get_beatmap_attributes(self, beatmap: int,
-                               mods: Optional[Union[int, Mods, Sequence[Union[str, Mods, int]]]] = None,
-                               ruleset: Optional[Union[str, GameModeStr]] = None,
-                               ruleset_id: Optional[Union[int, GameModeInt]] = None) -> BeatmapDifficultyAttributes:
+    async def get_beatmap_attributes(
+        self,
+        beatmap: int,
+        mods: Optional[Union[int, Mods, Sequence[Union[str, Mods, int]]]] = None,
+        ruleset: Optional[Union[str, GameModeStr]] = None,
+        ruleset_id: Optional[Union[int, GameModeInt]] = None,
+    ) -> BeatmapDifficultyAttributes:
         """
         Returns difficulty attributes of beatmap with specific mode and mods combination.
 
         Requires OAuth and scope public
 
         **Parameters**
 
         beatmap: :class:`int`
             Beatmap id.
 
         mods: Optional[Union[:class:`int`, Sequence[Union[:class:`str`, :class:`Mods`, :class:`int`]], :class:`Mods`]]
             Mod combination. Can be either a bitset of mods, a Mods enum, or array of any. Defaults to no mods.
             Some mods may cause the api to throw an HTTP 422 error depending on the map's gamemode.
 
-        ruleset: Optional[Union[:class:`GameModeStr`, :class:`int`]]
+        ruleset: Optional[Union[:class:`GameModeStr`, :class:`str`]]
             Ruleset of the difficulty attributes. Only valid if it's the beatmap ruleset or the beatmap can be
             converted to the specified ruleset. Defaults to ruleset of the specified beatmap.
 
         ruleset_id: Optional[Union[:class:`GameModeInt`, :class:`int`]]
-            The same as ruleset but in integer form.
+            The same as `ruleset` but in integer form.
 
         **Returns**
 
         :class:`BeatmapDifficultyAttributes`
         """
         ruleset, ruleset_id = parse_enum_args(ruleset, ruleset_id)
-        return BeatmapDifficultyAttributes(await self.http.make_request(Path.get_beatmap_attributes(beatmap),
-                                                                  mods=parse_mods_arg(mods), ruleset=ruleset,
-                                                                  ruleset_id=ruleset_id))
+        return BeatmapDifficultyAttributes(
+            await self.http.make_request(
+                Path.get_beatmap_attributes(beatmap),
+                mods=parse_mods_arg(mods),
+                ruleset=ruleset,
+                ruleset_id=ruleset_id,
+            )
+        )
 
     async def get_beatmapset(self, beatmapset_id: int) -> Beatmapset:
         """
         Get beatmapset by id.
 
         Requires OAuth and scope public
 
@@ -331,18 +440,25 @@
 
         **Returns**
 
         :class:`Beatmapset`
         """
         return Beatmapset(await self.http.make_request(Path.get_beatmapset(beatmapset_id)))
 
-    async def get_beatmapset_discussion_posts(self, beatmapset_discussion_id: Optional[int] = None,
-                                        limit: Optional[int] = None, page: Optional[int] = None,
-                                        sort: Optional[str] = None, user: Optional[int] = None,
-                                        with_deleted: Optional[str] = None) -> dict:
+    async def get_beatmapset_discussion_posts(
+        self,
+        beatmapset_discussion_id: Optional[int] = None,
+        limit: Optional[int] = None,
+        page: Optional[int] = None,
+        sort: Optional[str] = None,
+        types: Optional[Sequence[str]] = None,
+        user: Optional[int] = None,
+        with_deleted: Optional[str] = None,
+        cursor: Optional[Dict[str, int]] = None,
+    ) -> BeatmapsetDiscussionPostsResult:
         """
         Returns the posts of the beatmapset discussions
 
         Requires OAuth and scope public
 
         **Parameters**
 
@@ -352,52 +468,68 @@
         limit: Optional[:class:`int`]
             Maximum number of results
 
         page: Optional[:class:`int`]
             Search results page.
 
         sort: Optional[:class:`str`]
-            id_desc for newest first; id_asc for oldest first. Defaults to id_desc
+            `id_desc` for newest first; `id_asc` for oldest first. Defaults to `id_desc`
+
+        type: Optional[Sequence[:class:`str`]]
+            `first`, `reply`, `system` are the valid values. Defaults to `reply`.
 
         user: Optional[:class:`int`]
-            The id of the User
+            The id of the user
 
         with_deleted: Optional[:class:`str`]
-            The param has no effect as api calls do not currently receive group permissions
-
-        **Returns**
-
-        :class:`dict`
-            {
-            beatmapsets: :class:`BeatmapsetCompact`,
-
-            cursor: :class:`dict`,
+            This param has no effect as api calls do not currently receive group permissions.
 
-            posts: Sequence[:class:`BeatmapsetDiscussionPost`],
+        cursor: Optional[Dict[:class:`str`, :class:`int`]]
+            A cursor object received from a previous call to get_beatmapset_discussion_posts
+            (:class:`BeatmapsetDiscussionPostsResult`.cursor)
 
-            users: :class:`UserCompact`
-            }
-        """
-        # TODO: Change is supposed to occur on the response given back from the server,
-        #  make sure to change it when that happens.
-        resp = await self.http.make_request(Path.beatmapset_discussion_posts(),
-                                      beatmapset_discussion_id=beatmapset_discussion_id,
-                                      limit=limit, page=page, sort=sort, user=user, with_deleted=with_deleted)
-        return {
-            'beatmapsets': list(map(BeatmapsetCompact, resp['beatmapsets'])),
-            'cursor': resp['cursor'],
-            'posts': list(map(BeatmapsetDiscussionPost, resp['posts'])),
-            'users': list(map(UserCompact, resp['users']))
-        }
+        **Returns**
 
-    async def get_beatmapset_discussion_votes(self, beatmapset_discussion_id: Optional[int] = None,
-                                        limit: Optional[int] = None, page: Optional[int] = None,
-                                        receiver: Optional[int] = None, score: Optional[int] = None,
-                                        sort: Optional[str] = None, user: Optional[int] = None,
-                                        with_deleted: Optional[str] = None) -> dict:
+        :class:`BeatmapsetDiscussionsPostsResult`
+        """
+        if cursor is None:
+            cursor = {}
+        if "page" in cursor:
+            page = cursor["page"]
+        if "limit" in cursor:
+            limit = cursor["limit"]
+        resp = await self.http.make_request(
+            Path.beatmapset_discussion_posts(),
+            beatmapset_discussion_id=beatmapset_discussion_id,
+            limit=limit,
+            page=page,
+            sort=sort,
+            user=user,
+            with_deleted=with_deleted,
+            **{"types[]": types},
+        )
+        return BeatmapsetDiscussionPostsResult(
+            list(map(BeatmapsetCompact, resp["beatmapsets"])),
+            list(map(BeatmapsetDiscussionPost, resp["posts"])),
+            list(map(UserCompact, resp["users"])),
+            resp["cursor_string"],
+        )
+
+    async def get_beatmapset_discussion_votes(
+        self,
+        beatmapset_discussion_id: Optional[int] = None,
+        limit: Optional[int] = None,
+        page: Optional[int] = None,
+        receiver: Optional[int] = None,
+        score: Optional[int] = None,
+        sort: Optional[str] = None,
+        user: Optional[int] = None,
+        with_deleted: Optional[str] = None,
+        cursor: Optional[Dict[str, int]] = None,
+    ) -> BeatmapsetDiscussionVotesResult:
         """
         Returns the votes given to beatmapset discussions
 
         Requires OAuth and scope public
 
         **Parameters**
 
@@ -413,130 +545,144 @@
         receiver: Optional[:class:`int`]
             The id of the User receiving the votes.
 
         score: Optional[:class:`int`]
             1 for upvote, -1 for downvote
 
         sort: Optional[:class:`str`]
-            id_desc for newest first; id_asc for oldest first. Defaults to id_desc
+            `id_desc` for newest first; `id_asc` for oldest first. Defaults to `id_desc`
 
         user: Optional[:class:`int`]
             The id of the User giving the votes.
 
         with_deleted: Optional[:class:`str`]
-            The param has no effect as api calls do not currently receive group permissions
-
-        **Returns**
+            This param has no effect as api calls do not currently receive group permissions
 
-        :class:`dict`
-            {
-            cursor: :class:`dict`,
+        cursor: Optional[Dict[:class:`str`, :class:`int`]]
+            A cursor object received from a previous call to get_beatmapset_discussion_votes
+            (:class:`BeatmapsetDiscussionVotesResult`.cursor)
 
-            discussions: Sequence[:class:`BeatmapsetDiscussion`],
-
-            users: Sequence[:class:`UserCompact`],
-
-            votes: Sequence[:class:`BeatmapsetDiscussionVote`]
-            }
-        """
-        # TODO: Change is supposed to occur on the response given back from the server,
-        #  make sure to change it when that happens.
-        resp = await self.http.make_request(Path.beatmapset_discussion_votes(),
-                                      beatmapset_discussion_id=beatmapset_discussion_id,
-                                      limit=limit, receiver=receiver, score=score, page=page,
-                                      sort=sort, user=user, with_deleted=with_deleted)
-        return {
-            'cursor': resp['cursor'],
-            'discussions': list(map(BeatmapsetDiscussion, resp['discussions'])),
-            'users': list(map(UserCompact, resp['users'])),
-            'votes': list(map(BeatmapsetDiscussionVote, resp['votes']))
-        }
+        **Returns**
 
-    async def get_beatmapset_discussions(self, beatmap_id: Optional[int] = None, beatmapset_id: Optional[int] = None,
-                                   beatmapset_status: Optional[str] = None, limit: Optional[int] = None,
-                                   message_types: Optional[Sequence[str]] = None,
-                                   only_unresolved: Optional[bool] = None, page: Optional[int] = None,
-                                   sort: Optional[str] = None, user: Optional[int] = None,
-                                   with_deleted: Optional[str] = None) -> dict:
+        :class:`BeatmapsetDiscussionVotesResult`
+        """
+        if cursor is None:
+            cursor = {}
+        if "page" in cursor:
+            page = cursor["page"]
+        if "limit" in cursor:
+            limit = cursor["limit"]
+        resp = await self.http.make_request(
+            Path.beatmapset_discussion_votes(),
+            beatmapset_discussion_id=beatmapset_discussion_id,
+            limit=limit,
+            receiver=receiver,
+            score=score,
+            page=page,
+            sort=sort,
+            user=user,
+            with_deleted=with_deleted,
+        )
+        return BeatmapsetDiscussionVotesResult(
+            list(map(BeatmapsetDiscussion, resp["discussions"])),
+            list(map(BeatmapsetDiscussionVote, resp["votes"])),
+            list(map(UserCompact, resp["users"])),
+            resp["cursor"],
+        )
+
+    async def get_beatmapset_discussions(
+        self,
+        beatmap_id: Optional[int] = None,
+        beatmapset_id: Optional[int] = None,
+        beatmapset_status: Optional[str] = None,
+        limit: Optional[int] = None,
+        message_types: Optional[Sequence[Union[str, MessageType]]] = None,
+        only_unresolved: Optional[bool] = None,
+        page: Optional[int] = None,
+        sort: Optional[str] = None,
+        user: Optional[int] = None,
+        with_deleted: Optional[str] = None,
+        cursor: Optional[Dict[str, int]] = None,
+    ) -> BeatmapsetDiscussionsResult:
         """
         Returns a list of beatmapset discussions
 
         Requires OAuth and scope public
 
         **Parameters**
 
         beatmap_id: Optional[:class:`int`]
-            id of the Beatmap
+            id of the beatmap
 
         beatmapset_id: Optional[:class:`int`]
-            id of the Beatmapset
+            id of the beatmapset
 
         beatmapset_status: Optional[:class:`str`]
-            One of all, ranked, qualified, disqualified, never_qualified. Defaults to all.
+            One of `all`, `ranked`, `qualified`, `disqualified`, `never_qualified`. Defaults to `all`.
 
         limit: Optional[:class:`int`]
             Maximum number of results.
 
-        message_types: Optional[Sequence[:class:`str`]]
-            suggestion, problem, mapper_note, praise, hype, review. Blank defaults to all types.
+        message_types: Optional[Sequence[Union[:class:`str`, :class:`MessageType`]]]
+            None defaults to all types.
 
         only_unresolved: Optional[:class:`bool`]
             true to show only unresolved issues; false, otherwise. Defaults to false.
 
         page: Optional[:class:`int`]
             Search result page.
 
         sort: Optional[:class:`str`]
-            id_desc for newest first; id_asc for oldest first. Defaults to id_desc.
+            `id_desc` for newest first; `id_asc` for oldest first. Defaults to `id_desc`.
 
         user: Optional[:class:`int`]
             The id of the User.
 
         with_deleted: Optional[:class:`str`]
             This param has no effect as api calls do not currently receive group permissions.
 
-        **Returns**
-
-        :class:`dict`
-            {
-
-            beatmaps: Sequence[:class:`Beatmap`],
-                List of beatmaps associated with the discussions returned.
-
-            cursor: :class:`dict`,
+        cursor: Optional[Dict[:class:`str`, :class:`int`]]
+            A cursor object received from a previous call to get_beatmapset_discussions
+            (:class:`BeatmapsetDiscussionsResult`.cursor)
 
-            discussions: Sequence[:class:`BeatmapsetDiscussion`],
-                List of discussions according to sort order.
-
-            included_discussions: Sequence[:class:`BeatmapsetDiscussion`],
-                Additional discussions related to discussions.
-
-            reviews_config.max_blocks: :class:`int`,
-                Maximum number of blocks allowed in a review.
-
-            users: Sequence[:class:`UserCompact`]
-                List of users associated with the discussions returned.
+        **Returns**
 
-            }
-        """
-        # TODO: Change is supposed to occur on the response given back from the server,
-        #  make sure to change it when that happens.
-        message_types = {"message_types[]": message_types}
-        resp = await self.http.make_request(Path.beatmapset_discussions(), beatmap_id=beatmap_id,
-                                      beatmapset_id=beatmapset_id, beatmapset_status=beatmapset_status,
-                                      limit=limit, only_unresolved=only_unresolved, page=page, sort=sort,
-                                      user=user, with_deleted=with_deleted, **message_types)
-        return {
-            'beatmaps': list(map(Beatmap, resp['beatmaps'])),
-            'cursor': resp['cursor'],
-            'discussions': list(map(BeatmapsetDiscussion, resp['discussions'])),
-            'included_discussions': list(map(BeatmapsetDiscussion, resp['included_discussions'])),
-            'reviews_config.max_blocks': resp['reviews_config'],
-            'users': list(map(UserCompact, resp['users']))
-        }
+        :class:`BeatmapsetDiscussionsResult`
+        """
+        if cursor is None:
+            cursor = {}
+        if "page" in cursor:
+            page = cursor["page"]
+        if "limit" in cursor:
+            limit = cursor["limit"]
+        params = {}
+        if message_types is not None:
+            message_types = list(map(lambda t: t.value if isinstance(t, MessageType) else t, message_types))
+            params = {"message_types[]": message_types}
+        resp = await self.http.make_request(
+            Path.beatmapset_discussions(),
+            beatmap_id=beatmap_id,
+            beatmapset_id=beatmapset_id,
+            beatmapset_status=beatmapset_status,
+            limit=limit,
+            only_unresolved=only_unresolved,
+            page=page,
+            sort=sort,
+            user=user,
+            with_deleted=with_deleted,
+            **params,
+        )
+        return BeatmapsetDiscussionsResult(
+            list(map(Beatmap, resp["beatmaps"])),
+            list(map(BeatmapsetDiscussion, resp["discussions"])),
+            list(map(BeatmapsetDiscussion, resp["included_discussions"])),
+            list(map(UserCompact, resp["users"])),
+            ReviewsConfig(resp["reviews_config"]),
+            resp["cursor"],
+        )
 
     async def get_changelog_build(self, stream: str, build: str) -> Build:
         """
         Returns details of the specified build.
 
         **Parameters**
 
@@ -544,117 +690,126 @@
             Update stream name.
 
         build: :class:`str`
             Build version.
 
         **Returns**
 
-        A :class:`Build` with changelog_entries, changelog_entries.github_user, and versions included.
+        A :class:`Build` with `changelog_entries`, `changelog_entries.github_user`, and `versions` included.
         """
         return Build(await self.http.make_request(Path.get_changelog_build(stream, build)))
 
-    async def get_changelog_listing(self, from_version: Optional[str] = None, max_id: Optional[int] = None,
-                              stream: Optional[str] = None, to: Optional[str] = None,
-                              message_formats: Optional[Sequence[str]] = None) -> \
-            Dict[str, Union[Sequence[Build], Sequence[UpdateStream], Dict[str, Union[str, int, None]]]]:
+    async def get_changelog_listing(
+        self,
+        start: Optional[str] = None,
+        max_id: Optional[int] = None,
+        stream: Optional[str] = None,
+        end: Optional[str] = None,
+        message_formats: Optional[Sequence[str]] = None,
+    ) -> ChangelogListingResult:
         """
         Returns a listing of update streams, builds, and changelog entries.
 
         **Parameters**
 
-        from_version: Optional[:class:`str`]
+        start: Optional[:class:`str`]
             Minimum build version.
 
         max_id: Optional[:class:`int`]
             Maximum build ID.
 
         stream: Optional[:class:`str`]
             Stream name to return builds from.
 
-        to: Optional[:class:`str`]
+        end: Optional[:class:`str`]
             Maximum build version.
 
         message_formats: Optional[Sequence[:class:`str`]]
-            html, markdown. Default to both.
+            `html`, `markdown`. Default to both.
 
         **Returns**
 
-        {
-
-        "build": Sequence[:class:`Build`]
-
-        "search": {
-
-            "from": :class:`str`
-                from_version input.
-
-            "limit": :class:`int`
-                Always 21.
-
-            "max_id": :class:`int`
-                max_id input.
-
-            "stream": :class:`str`
-                stream input.
-
-            "to": :class:`str`
-                to input.
-
-        }
-
-        "streams": Sequence[:class:`UpdateStream`]
-
-        }
+        :class:`ChangelogListingResult`
         """
-        response = await self.http.make_request(Path.get_changelog_listing(), max_id=max_id,
-                                          stream=stream, to=to, message_formats=message_formats,
-                                          **{"from": from_version})
-        return {
-            "build": list(map(Build, response['builds'])),
-            "search": response['search'],
-            "streams": list(map(UpdateStream, response['streams'])),
-        }
-
-    async def lookup_changelog_build(self, changelog: str, key: Optional[str] = None,
-                               message_formats: Optional[Sequence[str]] = None) -> Build:
+        response = await self.http.make_request(
+            Path.get_changelog_listing(),
+            max_id=max_id,
+            stream=stream,
+            to=end,
+            **{"from": start, "message_formats[]": message_formats},
+        )
+        return ChangelogListingResult(
+            list(map(Build, response["builds"])),
+            list(map(UpdateStream, response["streams"])),
+            ChangelogListingSearch(
+                response["search"]["from"],
+                response["search"]["to"],
+                response["search"]["limit"],
+                response["search"]["max_id"],
+                response["search"]["stream"],
+            ),
+        )
+
+    async def lookup_changelog_build(
+        self,
+        changelog: str,
+        key: Optional[str] = None,
+        message_formats: Optional[Sequence[str]] = None,
+    ) -> Build:
         """
         Returns details of the specified build.
 
-        **Parameter**
+        **Parameters**
 
         changelog: :class:`str`
             Build version, update stream name, or build ID.
 
         key: Optional[:class:`str`]
-            Unset to query by build version or stream name, or id to query by build ID.
+            Leave blank to query by build version or stream name, or `id` to query by build ID.
 
         message_formats: Optional[Sequence[:class:`str`]]
-            html, markdown. Default to both.
+            `html`, `markdown`. Default to both.
 
         **Returns**
 
         A :class:`Build` with changelog_entries, changelog_entries.github_user, and versions included.
         """
-        return Build(await self.http.make_request(Path.lookup_changelog_build(changelog),
-                                            key=key, message_formats=message_formats))
-
-    async def chat_acknowledge(self) -> Sequence[UserSilence]:
+        return Build(
+            await self.http.make_request(
+                Path.lookup_changelog_build(changelog), key=key, **{"message_formats[]": message_formats}
+            )
+        )
+
+    async def chat_acknowledge(
+        self, history_since: Optional[int] = None, since: Optional[int] = None
+    ) -> Sequence[UserSilence]:
         """
         Send a chat ack.
 
         Requires OAuth, scope lazer, and a user (authorization code grant, delegate scope, or password auth)
 
+        **Parameters**
+
+        history_since: Optional[:class:`int`]
+            :class:`UserSilence` s after the specified id to return.
+            This field is preferred and takes precedence over since.
+
+        since: Optional[:class:`int`]
+            :class:`UserSilence` s after the specified :class:`ChatMessage`.message_id to return.
+
         **Returns**
 
-        Sequence[:class:`UserSilence`]
+        List[:class:`UserSilence`]
         """
-        resp = await self.http.make_request(Path.chat_ack())
+        resp = await self.http.make_request(Path.chat_ack(), history_since=history_since, since=since)
         return list(map(UserSilence, resp["silences"]))
 
-    async def create_new_pm(self, target_id: int, message: str, is_action: bool, uuid: Optional[str] = None) -> dict:
+    async def create_new_pm(
+        self, target_id: int, message: str, is_action: bool, uuid: Optional[str] = None
+    ) -> CreateNewPmResult:
         """
         This endpoint allows you to create a new PM channel.
 
         Requires OAuth, scope chat.write, and a user (authorization code grant, delegate scope, or password auth)
 
         **Parameters**
 
@@ -668,82 +823,78 @@
             whether the message is an action
 
         uuid: Optional[:class:`str`]
             client-side message identifier which will be sent back in response and websocket json.
 
         **Returns**
 
-        :class:`dict`
-            {
-
-            channel: :class:`ChatChannel`
-                channel the message was sent in
-
-            message: :class:`ChatMessage`
-                the sent message
-
-            new_channel_id: :class:`int`
-                channel_id of newly created channel
-
-            }
+        :class:`CreateNewPmResult`
         """
-        data = {'target_id': target_id, 'message': message, 'is_action': is_action}
+        data = {"target_id": target_id, "message": message, "is_action": is_action}
         if uuid is not None:
-            data['uuid'] = uuid
+            data["uuid"] = uuid
         resp = await self.http.make_request(Path.create_new_pm(), files=create_multipart_formdata(data))
-        return {
-            'channel': ChatChannel(resp['channel']),
-            'message': ChatMessage(resp['message']),
-            'new_channel_id': resp['new_channel_id'],
-        }
-
-    async def get_updates(self, since: int, includes: Optional[Sequence[str]] = None,
-                    history_since: Optional[int] = None) -> dict:
+        return CreateNewPmResult(
+            ChatChannel(resp["channel"]),
+            ChatMessage(resp["message"]),
+            resp["new_channel_id"],
+        )
+
+    async def get_updates(
+        self,
+        since: int = 0,
+        includes: Optional[Sequence[str]] = None,
+        history_since: Optional[int] = None,
+    ) -> GetUpdatesResult:
         """
         This endpoint returns new messages since the given message_id along with updated channel 'presence' data.
 
         Requires OAuth, scope lazer, a user (authorization code grant, delegate scope, or password auth)
 
         **Parameters**
 
         since: :class:`int`
-            Messages after the specified message_id to return.
+            Defaults to 0. :class:`UserSilence`s after the specified `ChatMessage.message_id` to return.
 
         includes: Optional[Sequence[:class:`str`]]
-            List of fields from presence, silences to include in the response. Returns presence if not specified.
-            Specifying silences may cause the api to return blank content for both presence and silences.
+            List of fields from `presence`, `silences` to include in the response. Uses `presences` if not specified.
 
         history_since: Optional[:class:`int`]
             :class:`UserSilence`s after the specified id to return.
+            This field is preferred and takes precedence over `since`.
 
         **Returns**
 
-        :class:`dict`
-            {
-            presence: List[:class:`ChatChannel`],
-
-            silences: List[:class:`UserSilence`]
-
-            }
+        :class:`GetUpdatesResult`
         """
         if includes is None:
             includes = ["presence"]
-        resp = await self.http.make_request(Path.get_updates(), since=since, history_since=history_since,
-                                      **{"includes[]": ",".join(includes)})
+        resp = await self.http.make_request(
+            Path.get_updates(),
+            since=since,
+            history_since=history_since,
+            **{"includes[]": includes},
+        )
         if resp is None:
             resp = {}
-        return {
-            'presence': list(map(ChatChannel, resp['presence'])) if 'presence' in resp else None,
-            'silences': list(map(UserSilence, resp['silences'])) if 'silences' in resp else None
-        }
-
-    async def get_channel_messages(self, channel_id: int, limit: Optional[int] = None, since: Optional[int] = None,
-                             until: Optional[int] = None) -> Sequence[ChatMessage]:
+        return GetUpdatesResult(
+            get_optional_list(resp, "presence", ChatChannel),
+            get_optional_list(resp, "silences", UserSilence),
+        )
+
+    async def get_channel_messages(
+        self,
+        channel_id: int,
+        limit: Optional[int] = None,
+        since: Optional[int] = None,
+        until: Optional[int] = None,
+    ) -> List[ChatMessage]:
         """
         This endpoint returns the chat messages for a specific channel.
+        You may need to first join the channel with :func:`osu.Client.join_channel`.
 
         Requires OAuth, scope lazer, and a user (authorization code grant, delegate scope, or password auth)
 
         **Parameter**
 
         channel_id: :class:`int`
             The ID of the channel to retrieve messages for
@@ -755,22 +906,29 @@
             messages after the specified message id will be returned
 
         until: Optional[:class:`int`]
             messages up to but not including the specified message id will be returned
 
         **Returns**
 
-        Sequence[:class:`ChatMessage`]
-            list containing :class:`ChatMessage` objects
+        List[:class:`ChatMessage`]
         """
-        return list(map(ChatMessage, await self.http.make_request(Path.get_channel_messages(channel_id),
-                                                            limit=limit, since=since, until=until)))
+        return list(
+            map(
+                ChatMessage,
+                await self.http.make_request(
+                    Path.get_channel_messages(channel_id),
+                    limit=limit,
+                    since=since,
+                    until=until,
+                ),
+            )
+        )
 
-    async def send_message_to_channel(self, channel_id: int, message: str, is_action: bool,
-                                uuid: Optional[str] = None) -> ChatMessage:
+    async def send_message_to_channel(self, channel_id: int, message: str, is_action: bool) -> ChatMessage:
         """
         This endpoint sends a message to the specified channel.
 
         Requires OAuth, scope lazer, and a user (authorization code grant, delegate scope, or password auth)
 
         **Parameters**
 
@@ -779,113 +937,112 @@
 
         message: :class:`str`
             message to send
 
         is_action: :class:`bool`
             whether the message is an action
 
-        uuid: Optional[:class:`str`]
-
         **Returns**
 
         :class:`ChatMessage`
         """
-        data = {'is_action': str(is_action).lower(), 'message': message}
-        if uuid is not None:
-            data["uuid"] = uuid
+        data = {"is_action": str(is_action).lower(), "message": message}
         data = create_multipart_formdata(data)
         return ChatMessage(await self.http.make_request(Path.send_message_to_channel(channel_id), files=data))
 
-    async def join_channel(self, channel: str, user: str) -> ChatChannel:
+    async def join_channel(self, channel: int, user: int) -> ChatChannel:
         """
-        This endpoint allows you to join a public channel.
+        This endpoint allows you (or someone else) to join a public channel.
 
         Requires OAuth, scope lazer, and a user (authorization code grant, delegate scope, or password auth)
 
         **Parameters**
 
-        channel: :class:`str`
+        channel: :class:`int`
             channel id of channel to join
 
-        user: :class:`str`
-            user joining (you)
+        user: :class:`int`
+            user id of user joining
 
         **Returns**
 
         :class:`ChatChannel`
         """
         return ChatChannel(await self.http.make_request(Path.join_channel(channel, user)))
 
-    async def leave_channel(self, channel: str, user: str):
+    async def leave_channel(self, channel: int, user: int) -> None:
         """
-        This endpoint allows you to leave a public channel.
+        This endpoint allows you (or someone else) to leave a public channel.
 
         Requires OAuth, scope lazer, and a user (authorization code grant, delegate scope, or password auth)
 
         **Parameters**
 
-        channel: :class:`str`
+        channel: :class:`int`
             channel id of channel to leave
 
-        user: :class:`str`
-            user leaving (you)
+        user: :class:`int`
+            user id of user leaving
         """
-        # is_download=True because the api does not return a json response
-        await self.http.make_request(Path.leave_channel(channel, user), is_download=True)
+        await self.http.make_request(Path.leave_channel(channel, user))
 
-    async def mark_channel_as_read(self, channel_id: int, message_id: int):
+    async def mark_channel_as_read(self, channel_id: int, message_id: int) -> None:
         """
         This endpoint marks the channel as having being read up to the given message_id.
 
         Requires OAuth, scope lazer, and a user (authorization code grant, delegate scope, or password auth)
 
         **Parameters**
 
         channel_id: :class:`int`
             The channel_id of the channel to mark as read
 
         message_id: :class:`int`
             The message_id of the message to mark as read up to
         """
-        # is_download=True because the api does not return a json response
-        await self.http.make_request(Path.mark_channel_as_read(channel_id, message_id), is_download=True)
+        await self.http.make_request(Path.mark_channel_as_read(channel_id, message_id))
 
-    async def get_channel_list(self) -> Sequence[ChatChannel]:
+    async def get_channel_list(self) -> List[ChatChannel]:
         """
         This endpoint returns a list of all joinable public channels.
 
         Requires OAuth, scope lazer, and a user (authorization code grant, delegate scope, or password auth)
 
         **Returns**
 
         Sequence[:class:`ChatChannel`]
         """
         return list(map(ChatChannel, await self.http.make_request(Path.get_channel_list())))
 
-    async def create_channel(self, channel_type: Union[ChatChannelType, str], target_id: Optional[int] = None,
-                       target_ids: Optional[Sequence[int]] = None, message: Optional[str] = None,
-                       channel: Optional[Dict[str, str]] = None) -> ChatChannel:
+    async def create_channel(
+        self,
+        channel_type: Union[ChatChannelType, str],
+        target_id: Optional[int] = None,
+        target_ids: Optional[Sequence[int]] = None,
+        message: Optional[str] = None,
+        channel: Optional[Dict[str, str]] = None,
+    ) -> ChatChannel:
         """
         [This description may be outdated]
 
         This endpoint creates a new channel if doesn't exist and joins it.
         Currently only for rejoining existing PM channels which the user has left.
 
         Requires OAuth, scope lazer, and a user (authorization code grant, delegate scope, or password auth)
 
         **Parameter**
 
         channel_type: Union[:class:`ChatChannelType`, :class:`str`]
-            channel type (currently only supports "PM" and "ANNOUNCE")
+            channel type (currently only supports `PM` and `ANNOUNCE`)
 
         target_id: Optional[:class:`int`]
             target user id; required if type is PM; ignored, otherwise.
 
         target_ids: Optional[Sequence[:class:`int`]]
-            target user ids; required if type is PM; ignored, otherwise.
+            target user ids; required if type is ANNOUNCE; ignored, otherwise.
 
         message: Optional[:class:`str`]
             message to send with the announcement; required if type is ANNOUNCE.
 
         channel: Optional[Dict[str, str]]
             channel details; required if type is ANNOUNCE.
 
@@ -894,66 +1051,57 @@
 
             description: :class:`str`
                 the channel description
 
         **Returns**
 
         :class:`ChatChannel`
-             contains recent_messages attribute. Note that if there's no existing PM channel,
-             most of the fields will be blank. In that case, send a message (create_new_pm)
-             instead to create the channel.
+             contains recent_messages attribute (which is deprecated).
         """
         channel_type = parse_enum_args(channel_type)
         if channel_type == "PM":
-            if target_id is None and target_ids is None:
-                raise ValueError("target_id and target_ids cannot both be null if the channel type is PM")
-            data = {"type": channel_type,
-                    **({"target_ids": target_ids} if target_ids is not None else {"target_id": target_id})}
+            data = {"type": "PM", "target_id": target_id}
         elif channel_type == "ANNOUNCE":
-            if message is None:
-                raise ValueError("message cannot be null when the channel type is ANNOUNCE")
-            elif channel is None or channel["name"] is None or channel["description"] is None:
-                raise ValueError("channel and it's items cannot be null when the channel type is ANNOUNCEMENT")
-            data = {"type": channel_type, "message": message, "channel": channel}
+            data = {
+                "type": channel_type,
+                "message": message,
+                "channel": json.dumps(channel),
+                "target_ids": json.dumps(target_ids),
+            }
         else:
-            raise ValueError(f"{channel_type} is not a valid channel type that can be created. "
-                             f"Check for casing (uppercase) if the type is correct.")
-        return ChatChannel(await self.http.make_request(Path.create_channel(), data=data))
+            raise ValueError(
+                f"{channel_type} is not a valid channel type that can be created. " f"Check for casing (uppercase)."
+            )
+        return ChatChannel(await self.http.make_request(Path.create_channel(), files=create_multipart_formdata(data)))
 
-    async def get_channel(self, channel: str) -> dict:
+    async def get_channel(self, channel_id: int) -> GetChannelResult:
         """
         Gets details of a chat channel.
 
         Requires OAuth, scope lazer, and a user (authorization code grant, delegate scope, or password auth)
 
         **Parameter**
 
-        channel: :class:`str`
+        channel_id: :class:`int`
 
         **Returns**
 
-        :class:`dict`
-            {
-            channel: :class:`ChatChannel`,
-
-            users: :class:`UserCompact`
-                Only visible for PM channels
-
-            }
+        :class:`GetChannelResult`
         """
-        resp = await self.http.make_request(Path.get_channel(channel))
-        return {
-            'channel': ChatChannel(resp['channel']),
-            'users': list(map(UserCompact, resp['users'])),
-        }
+        resp = await self.http.make_request(Path.get_channel(channel_id))
+        return GetChannelResult(ChatChannel(resp["channel"]), list(map(UserCompact, resp["users"])))
 
-    async def get_comments(self, commentable_type: Optional[Union[ObjectType, str]] = None,
-                     commentable_id: Optional[int] = None, cursor: Optional[dict] = None,
-                     parent_id: Optional[int] = None,
-                     sort: Optional[Union[str, CommentSort]] = None) -> CommentBundle:
+    async def get_comments(
+        self,
+        commentable_type: Optional[Union[ObjectType, str]] = None,
+        commentable_id: Optional[int] = None,
+        cursor: Optional[dict] = None,
+        parent_id: Optional[int] = None,
+        sort: Optional[Union[str, CommentSort]] = None,
+    ) -> CommentBundle:
         """
         Returns a list comments and their replies up to 2 levels deep.
 
         Does not require OAuth
 
         **Parameter**
 
@@ -977,23 +1125,38 @@
 
         **Returns**
 
         :class:`CommentBundle`
             pinned_comments is only included when commentable_type and commentable_id are specified.
         """
         commentable_type, sort = parse_enum_args(commentable_type, sort)
-        if commentable_type is not None and commentable_type not in ("beatmapset", "build", "news_post"):
+        if commentable_type is not None and commentable_type not in (
+            "beatmapset",
+            "build",
+            "news_post",
+        ):
             raise ValueError("commentable_type, if not null, must be of the following: beatmapset, build, new_post")
-        return CommentBundle(await self.http.make_request(Path.get_comments(), commentable_type=commentable_type,
-                                                    commentable_id=commentable_id, **(cursor if cursor else {}),
-                                                    parent_id=parent_id, sort=sort))
-
-    async def post_comment(self, commentable_type: Optional[Union[ObjectType, str]] = None,
-                     commentable_id: Optional[int] = None, message: Optional[str] = None,
-                     parent_id: Optional[int] = None) -> CommentBundle:
+        return CommentBundle(
+            await self.http.make_request(
+                Path.get_comments(),
+                commentable_type=commentable_type,
+                commentable_id=commentable_id,
+                parent_id=parent_id,
+                sort=sort,
+                **(cursor if cursor else {}),
+            )
+        )
+
+    async def post_comment(
+        self,
+        commentable_type: Optional[Union[ObjectType, str]] = None,
+        commentable_id: Optional[int] = None,
+        message: Optional[str] = None,
+        parent_id: Optional[int] = None,
+    ) -> CommentBundle:
         """
         Posts a new comment to a comment thread.
 
         Requires OAuth, scope lazer, and a user (authorization code grant, delegate scope, or password auth)
 
         **Parameter**
 
@@ -1010,21 +1173,23 @@
         parent_id: Optional[:class:`int`]
             The id of the comment to reply to, null if not a reply
 
         **Returns**
 
         :class:`CommentBundle`
         """
-        params = {
+        data = {
             "comment[commentable_type]": parse_enum_args(commentable_type),
             "comment[commentable_id]": commentable_id,
             "comment[message]": message,
-            "comment[parent_id]": parent_id
+            "comment[parent_id]": parent_id,
         }
-        return CommentBundle(await self.http.make_request(Path.post_new_comment(), **params))
+        return CommentBundle(
+            await self.http.make_request(Path.post_new_comment(), files=create_multipart_formdata(data))
+        )
 
     async def get_comment(self, comment: int) -> CommentBundle:
         """
         Gets a comment and its replies up to 2 levels deep.
 
         Does not require OAuth
 
@@ -1053,16 +1218,19 @@
         message: Optional[:class:`str`]
             New text of the comment
 
         **Returns**
 
         :class:`CommentBundle`
         """
-        return CommentBundle(await self.http.make_request(Path.edit_comment(comment),
-                                                    **{"comment[message]": message}))
+        return CommentBundle(
+            await self.http.make_request(
+                Path.edit_comment(comment), files=create_multipart_formdata({"comment[message]": message})
+            )
+        )
 
     async def delete_comment(self, comment: int) -> CommentBundle:
         """
         Deletes the specified comment.
 
         Requires OAuth, scope lazer, and a user (authorization code grant, delegate scope, or password auth)
 
@@ -1126,21 +1294,30 @@
             Content of the reply post.
 
         **Returns**
 
         :class:`ForumPost`
             body attributes included
         """
-        data = {'body': body}
-        return ForumPost(await self.http.make_request(Path.reply_topic(topic), data=data))
+        data = {"body": body}
+        return ForumPost(await self.http.make_request(Path.reply_topic(topic), files=create_multipart_formdata(data)))
 
-    async def create_topic(self, body: str, forum_id: int, title: str, with_poll: Optional[bool] = None,
-                     hide_results: Optional[bool] = None, length_days: Optional[int] = None,
-                     max_options: Optional[int] = None, poll_options: Optional[str] = None,
-                     poll_title: Optional[str] = None, vote_change: Optional[bool] = None) -> dict:
+    async def create_topic(
+        self,
+        body: str,
+        forum_id: int,
+        title: str,
+        with_poll: Optional[bool] = None,
+        hide_results: Optional[bool] = None,
+        length_days: Optional[int] = None,
+        max_options: Optional[int] = None,
+        poll_options: Optional[str] = None,
+        poll_title: Optional[str] = None,
+        vote_change: Optional[bool] = None,
+    ) -> CreateTopicResult:
         """
         Create a new topic.
 
         Requires OAuth, scope forum.write, and a user (authorization code grant, delegate scope, or password auth)
 
         **Parameters**
 
@@ -1173,90 +1350,92 @@
             Title of the poll.
 
         vote_change: Optional[:class:`bool`]
             Enable this to allow user to change their votes (default: false).
 
         **Returns**
 
-        :class:`dict`
-            {
-            topic: :class:`ForumTopic`
-
-            post: :class:`ForumPost`
-                includes body
-
-            }
+        :class:`CreateTopicResult`
         """
-        data = {'body': body, 'forum_id': forum_id, 'title': title, 'with_poll': with_poll}
+        data = {
+            "body": body,
+            "forum_id": forum_id,
+            "title": title,
+            "with_poll": with_poll,
+        }
         if with_poll:
             if poll_options is None or poll_title is None:
                 raise TypeError("poll_options and poll_title are required since the topic has a poll.")
-            data.update({'forum_topic_poll': {
-                'hide_results': hide_results, 'length_days': length_days,
-                'max_options': max_options, 'poll_options': poll_options,
-                'poll_title': poll_title, 'vote_change': vote_change
-            }})
-        resp = await self.http.make_request(Path.create_topic(), data=json.dumps(data))
-        return {
-            'topic': ForumTopic(resp['topic']),
-            'post': ForumPost(resp['post'])
-        }
-
-    async def get_topic_and_posts(self, topic: int, cursor: Optional[dict] = None, sort: Optional[str] = None,
-                            limit: Optional[int] = None, start: Optional[int] = None,
-                            end: Optional[int] = None) -> dict:
+            data.update(
+                {
+                    "forum_topic_poll[hide_results]": hide_results,
+                    "forum_topic_poll[length_days]": length_days,
+                    "forum_topic_poll[max_options]": max_options,
+                    "forum_topic_poll[poll_options]": poll_options,
+                    "forum_topic_poll[poll_title]": poll_title,
+                    "forum_topic_poll[vote_change]": vote_change,
+                }
+            )
+        resp = await self.http.make_request(Path.create_topic(), files=create_multipart_formdata(data))
+        return CreateTopicResult(ForumTopic(resp["topic"]), ForumPost(resp["post"]))
+
+    async def get_topic_and_posts(
+        self,
+        topic: int,
+        cursor: Optional[str] = None,
+        sort: Optional[str] = None,
+        limit: Optional[int] = None,
+        start: Optional[int] = None,
+        end: Optional[int] = None,
+    ) -> GetTopicAndPostsResult:
         """
         Get topic and its posts.
 
         Requires OAuth and scope public
 
         **Parameters**
 
         topic: :class:`int`
             Id of the topic.
 
-        cursor: Optional[:class:`dict`]
-            To be used to fetch the next page of results
+        cursor: Optional[:class:`str`]
+            Parameter for pagination.
 
         sort: Optional[:class:`str`]
             Post sorting option. Valid values are id_asc (default) and id_desc.
 
         limit: Optional[:class:`int`]
             Maximum number of posts to be returned (20 default, 50 at most).
 
         start: Optional[:class:`int`]
             First post id to be returned with sort set to id_asc.
-            This parameter is ignored if cursor is specified.
+            This parameter is ignored if cursor_string is specified.
 
         end: Optional[:class:`int`]
             First post id to be returned with sort set to id_desc.
-            This parameter is ignored if cursor is specified.
+            This parameter is ignored if cursor_string is specified.
 
         **Returns**
 
-        :class:`dict`
-            {
-            cursor: :class:`dict`,
-
-            search: :class:`dict`,
-
-            posts: Sequence[:class:`ForumPost`],
-
-            topic: :class:`ForumTopic`
-
-            }
+        :class:`GetTopicAndPostsResult`
         """
-        resp = await self.http.make_request(Path.get_topic_and_posts(topic), **(cursor if cursor else {}),
-                                      sort=sort, limit=limit, start=start, end=end)
-        return {
-            'cursor': resp['cursor'],
-            'search': resp['search'],
-            'posts': list(map(ForumPost, resp['posts'])),
-            'topic': ForumTopic(resp['topic'])
-        }
+        resp = await self.http.make_request(
+            Path.get_topic_and_posts(topic),
+            **(cursor if cursor else {}),
+            sort=sort,
+            limit=limit,
+            start=start,
+            end=end,
+        )
+        return GetTopicAndPostsResult(
+            resp["cursor_string"],
+            resp["search"],
+            ForumTopic(resp["topic"]),
+            list(map(ForumPost, resp["posts"])),
+        )
 
     async def edit_topic(self, topic: int, topic_title: str) -> ForumTopic:
         """
         Edit topic. Only title can be edited through this endpoint.
 
         Requires OAuth and scope forum.write
 
@@ -1268,16 +1447,16 @@
         topic_title: :class:`str`
             New topic title.
 
         **Returns**
 
         :class:`ForumTopic`
         """
-        data = {'forum_topic': {'topic_title': topic_title}}
-        return ForumTopic(await self.http.make_request(Path.edit_topic(topic), data=json.dumps(data)))
+        data = {"forum_topic[topic_title]": topic_title}
+        return ForumTopic(await self.http.make_request(Path.edit_topic(topic), files=create_multipart_formdata(data)))
 
     async def edit_post(self, post: int, body: str) -> ForumPost:
         """
         Edit specified forum post.
 
         Requires OAuth and scope forum.write
 
@@ -1287,19 +1466,23 @@
         body: :class:`str`
             New post content in BBCode format.
 
         **Returns**
 
         :class:`ForumPost`
         """
-        data = {'body': body}
-        return ForumPost(await self.http.make_request(Path.edit_post(post), data=data))
+        data = {"body": body}
+        return ForumPost(await self.http.make_request(Path.edit_post(post), files=create_multipart_formdata(data)))
 
-    async def search(self, mode: Optional[Union[str, WikiSearchMode]] = None, query: Optional[str] = None,
-               page: Optional[int] = None) -> Dict[str, SearchResults]:
+    async def search(
+        self,
+        mode: Optional[Union[str, WikiSearchMode]] = None,
+        query: Optional[str] = None,
+        page: Optional[int] = None,
+    ) -> SearchResult:
         """
         Searches users and wiki pages.
 
         Requires OAuth and scope public
 
         **Parameters**
 
@@ -1310,29 +1493,22 @@
             Search keyword.
 
         page: Optional[:class:`int`]
             Search result page. Ignored for mode all.
 
         **Returns**
 
-        Dict[:class:`str`, :class:`SearchResults`]
-            {
-
-            "user": Union[:class:`SearchResults`, :class:`None`]
-
-            "wiki_page": Union[:class:`SearchResults`, :class:`None`]
-
-            }
+        :class:`SearchResult`
         """
         mode = parse_enum_args(mode)
         resp = await self.http.make_request(Path.search(), mode=mode, query=query, page=page)
-        return {
-            'user': SearchResults(resp["user"], UserCompact) if 'user' in resp else None,
-            'wiki_page': SearchResults(resp["wiki_page"], WikiPage) if 'wiki_page' in resp else None,
-        }
+        return SearchResult(
+            get_optional_list(resp.get("user", {}), "data", UserCompact),
+            get_optional_list(resp.get("wiki_page", {}), "data", WikiPage),
+        )
 
     async def get_user_highscore(self, room: int, playlist: int, user: int) -> MultiplayerScore:
         """
         Requires OAuth, scope lazer, and a user (authorization code grant, delegate scope, or password auth)
 
         **Parameters**
 
@@ -1347,17 +1523,22 @@
 
         **Returns**
 
         :class:`MultiplayerScores`
         """
         return MultiplayerScore(await self.http.make_request(Path.get_user_high_score(room, playlist, user)))
 
-    async def get_scores(self, room: int, playlist: int, limit: Optional[int] = None,
-                   sort: Optional[Union[str, MultiplayerScoresSort]] = None,
-                   cursor: Optional[dict] = None) -> MultiplayerScores:
+    async def get_scores(
+        self,
+        room: int,
+        playlist: int,
+        limit: Optional[int] = None,
+        sort: Optional[Union[str, MultiplayerScoresSort]] = None,
+        cursor: Optional[str] = None,
+    ) -> MultiplayerScores:
         """
         Requires OAuth, scope public, and a user (authorization code grant, delegate scope, or password auth)
 
         **Parameters**
 
         room: :class:`int`
             Id of the room.
@@ -1366,24 +1547,30 @@
             Id of the playlist item.
 
         limit: Optional[:class:`int`]
             Number of scores to be returned.
 
         sort: Optional[Union[:class:`str`, :class:`MultiplayerScoresSort`]]
 
-
-        cursor: Optional[:class:`dict`]
+        cursor: Optional[:class:`str`]
+            :class:`MultiplayerScores`.cursor value from a previous call to get next page.
 
         **Returns**
 
         :class:`MultiplayerScores`
         """
         sort = parse_enum_args(sort)
-        return MultiplayerScores(await self.http.make_request(Path.get_scores(room, playlist),
-                                                        limit=limit, sort=sort, **(cursor if cursor else {})))
+        return MultiplayerScores(
+            await self.http.make_request(
+                Path.get_scores(room, playlist),
+                limit=limit,
+                sort=sort,
+                cursor_string=cursor,
+            )
+        )
 
     async def get_score(self, room: int, playlist: int, score: int) -> MultiplayerScore:
         """
         Requires OAuth, scope lazer, and a user (authorization code grant, delegate scope, or password auth)
 
         **Parameters**
 
@@ -1398,206 +1585,187 @@
 
         **Returns**
 
         :class:`MultiplayerScore`
         """
         return MultiplayerScore(await self.http.make_request(Path.get_score(room, playlist, score)))
 
-    async def get_news_listing(self, limit: Optional[int] = None, year: Optional[int] = None,
-                         cursor: Optional[dict] = None) -> dict:
+    async def get_news_listing(
+        self,
+        limit: Optional[int] = None,
+        year: Optional[int] = None,
+        cursor: Optional[dict] = None,
+    ) -> GetNewsListingResult:
         """
         Returns a list of news posts and related metadata.
 
         **Parameters**
 
         limit: Optional[:class:`int`]
             Maximum number of posts (12 default, 1 minimum, 21 maximum).
 
         year: Optional[:class:`int`]
             Year to return posts from.
 
-        cursor: Optional[:class:`dict`]
+        cursor: Optional[:class:`str`]
             Cursor for pagination.
 
         **Returns**
 
-        {
-
-        cursor: :class:`dict`
-
-        news_posts: Sequence[:class:`NewsPost`]
-            Includes preview.
-
-        news_sidebar: {
-
-            current_year: :class:`int`
-                Year of the first post's publish time, or current year if no posts returned.
-
-            years: :class:`int`
-                All years during which posts have been published.
-
-            news_posts: Sequence[:class:`NewsPost`]
-                All posts published during current_year.
-
-        }
-
-        search: {
-
-            limit: :class:`int`
-                Clamped limit input.
-
-            sort: :class:`str`
-                Always published_desc.
-
-            }
-
-        }
+        :class:`GetNewsListingResult`
         """
-        response = await self.http.make_request(Path.get_news_listing(), limit=limit, year=year, cursor=cursor)
-        return {
-            "cursor": response['cursor'],
-            "news_posts": list(map(NewsPost, response["news_posts"])),
-            "news_sidebar": {
-                "current_year": response['news_sidebar']['current_year'],
-                "years": response['news_sidebar']['years'],
-                "news_posts": list(map(NewsPost, response['news_sidebar']['news_posts'])),
-            },
-            "search": response['search']
-        }
+        resp = await self.http.make_request(Path.get_news_listing(), limit=limit, year=year, cursor=cursor)
+        return GetNewsListingResult(
+            resp["cursor_string"],
+            list(map(NewsPost, resp["news_posts"])),
+            NewsSidebar(
+                resp["news_sidebar"]["current_year"],
+                list(map(NewsPost, resp["news_sidebar"]["news_posts"])),
+                resp["news_sidebar"]["years"],
+            ),
+            SearchInfo(resp["search"]["sort"], resp["search"]["limit"], None, None),
+        )
 
     async def get_news_post(self, news: str, key: Optional[str] = None) -> NewsPost:
         """
         Returns details of the specified news post.
 
         **Parameters**
 
         news: class:`str`
             News post slug or ID.
 
         key: Optional[:class:`str`]
-            Unset to query by slug, or id to query by ID.
+            Unset to query by slug, or `id` to query by ID.
 
         **Returns**
 
         Returns a :class:`NewsPost` with content and navigation included.
         """
         return NewsPost(await self.http.make_request(Path.get_news_post(news), key=key))
 
-    async def get_notifications(self, max_id: Optional[int] = None) -> dict:
+    async def get_notifications(self, max_id: Optional[int] = None) -> GetNotificationsResult:
         """
         This endpoint returns a list of the user's unread notifications. Sorted descending by id with limit of 50.
 
         Requires OAuth, scope lazer, a user (authorization code grant, delegate scope, or password auth)
 
         **Parameters**
 
         max_id: Optional[:class:`int`]
             Maximum id fetched. Can be used to load earlier notifications.
             Defaults to no limit (fetch latest notifications)
 
         **Returns**
 
-        :class:`dict`
-            {
-
-            has_more: :class:`bool`,
-                whether or not there are more notifications
-
-            notifications: Sequence[:class:`Notification`],
-
-            unread_count: :class:`bool`
-                total unread notifications
-
-            notification_endpoint: :class:`str`
-                url to connect to websocket server
-
-            }
+        :class:`GetNotificationsResult`
         """
         resp = await self.http.make_request(Path.get_notifications(), max_id=max_id)
-        return {
-            "notifications": list(map(Notification, resp['notifications'])),
-            "stacks": resp["stacks"],
-            "timestamp": resp["timestamp"],
-            "types": resp["types"],
-            "notification_endpoint": resp['notification_endpoint'],
-        }
-
-    async def mark_notifications_read(self, identities: Optional[Sequence[Union[
-        IdentitiesUtil, Dict[str, Union[str, int]]]]] = None,
-        notifications: Optional[Sequence[Union[
-            NotificationsUtil, Dict[str, str]]]] = None):
+        return GetNotificationsResult(
+            list(map(Notification, resp["notifications"])),
+            [
+                NotificationStackResult(
+                    NotificationType(category)
+                    if (category := stack["category"]).upper() in NotificationType.__members__
+                    else ObjectType(category),
+                    stack["cursor"],
+                    ObjectType(stack["object_type"]),
+                    stack["object_id"],
+                    stack["total"],
+                )
+                for stack in resp["stacks"]
+            ],
+            parser.parse(resp["timestamp"]),
+            [
+                NotificationTypeResult(t["cursor"], get_optional(t, "name", ObjectType), t["total"])
+                for t in resp["types"]
+            ],
+            resp.get("unread_count"),
+            resp["notification_endpoint"],
+        )
+
+    async def mark_notifications_read(
+        self,
+        identities: Optional[Sequence[Union[IdentitiesUtil, Dict[str, Union[str, int]]]]] = None,
+        notifications: Optional[Sequence[Union[NotificationsUtil, Dict[str, str]]]] = None,
+    ) -> None:
         """
         This endpoint allows you to mark notifications read. Should only supply one of the arguments.
 
         Requires OAuth, scope lazer, a user (authorization code grant, delegate scope, or password auth)
 
         **Parameters**
 
-        identities: Sequence[Union[:class:`ReadNotifIdentitiesUtil`,
-        Dict[:class:`str`, Union[:class:`str`, :class:`int`]]]]
+        identities: Optional[Sequence[Union[:class:`IdentitiesUtil`, Dict[:class:`str`, :class:`str`]]]]
 
-        notifications: Sequence[Union[:class:`ReadNotifNotificationsUtil`, Dict[:class:`str`, :class:`str`]]]
+        notifications: Optional[Sequence[Union[:class:`NotificationsUtil`, Dict[:class:`str`, :class:`str`]]]]
         """
-        if identities is not None and notifications is not None:
-            raise ValueError("Should only supply one argument, either identities or notifications.")
-        elif identities is None and notifications is None:
-            raise ValueError("Must supply at least one argument, either identities or notifications.")
-        try:
-            name = "identities" if notifications is None else "notifications"
-            params = JsonUtil.list_to_labeled_dict(locals()[name], name)
-        except Exception as exc:
-            raise ValueError("An error occurred while parsing the argument you provided.") from exc
+        name = "identities" if notifications is None else "notifications"
+        params = JsonUtil.list_to_labeled_dict(locals()[name], name)
         await self.http.make_request(Path.mark_notifications_as_read(), **params)
 
-    async def revoke_current_token(self):
+    async def revoke_current_token(self) -> None:
         """
         Revokes currently authenticated token.
 
         Requires OAuth
         """
-        await self.http.make_request(self, Path.revoke_current_token())
+        await self.http.make_request(Path.revoke_current_token())
 
-    async def get_ranking(self, mode: Union[str, GameModeStr], type: Union[str, RankingType],
-                    country: Optional[str] = None, cursor: Optional[dict] = None,
-                    filter: Optional[str] = None, spotlight: Optional[int] = None,
-                    variant: Optional[str] = None) -> Rankings:
+    async def get_ranking(
+        self,
+        mode: Union[str, GameModeStr],
+        type: Union[str, RankingType],
+        country: Optional[str] = None,
+        cursor: Optional[dict] = None,
+        filter: Optional[str] = None,
+        spotlight: Optional[int] = None,
+        variant: Optional[str] = None,
+    ) -> Rankings:
         """
         Gets the current ranking for the specified type and game mode.
 
         Requires OAuth and scope public
 
         mode: Union[:class:`str`, :class:`GameModeStr`]
 
         type: Union[:class:`str`, :class:`RankingType`]
             :class:`RankingType`
 
         country: Optional[:class:`str`]
-            Filter ranking by country code. Only available for type of performance.
+            Filter ranking by country code. Only available for `type` of `performance`.
 
         cursor: Optional[:class:`dict`]
 
         filter: Optional[:class:`str`]
-            Either all (default) or friends.
+            Either `all` (default) or `friends`.
 
         spotlight: Optional[:class:`int`]
-            The id of the spotlight if type is charts.
+            The id of the spotlight if `type` is `charts`.
             Ranking for latest spotlight will be returned if not specified.
 
         variant: Optional[:class:`str`]
             Filter ranking to specified mode variant.
-            For mode of mania, it's either 4k or 7k. Only available for type of performance.
+            For `mode` of `mania`, it's either `4k` or `7k`. Only available for `type` of `performance`.
 
         **Returns**
 
         :class:`Rankings`
         """
         mode, type = parse_enum_args(mode, type)
-        return Rankings(await self.http.make_request(Path.get_ranking(mode, type), country=country,
-                                                     **(cursor if cursor else {}), filter=filter,
-                                                     spotlight=spotlight, variant=variant))
+        return Rankings(
+            await self.http.make_request(
+                Path.get_ranking(mode, type),
+                country=country,
+                **(cursor if cursor else {}),
+                filter=filter,
+                spotlight=spotlight,
+                variant=variant,
+            )
+        )
 
     async def get_spotlights(self) -> Spotlights:
         """
         Gets the list of spotlights.
 
         Requires OAuth and scope public
 
@@ -1642,90 +1810,116 @@
         offset: Optional[:class:`int`]
             Result offset for pagination.
 
         **Returns**
 
         Sequence[:class:`KudosuHistory`]
         """
-        return list(map(KudosuHistory, await self.http.make_request(Path.get_user_kudosu(user),
-                                                              limit=limit, offset=offset)))
-
-    async def get_user_scores(self, user: int, type: Union[UserScoreType, str], include_fails: Optional[int] = None,
-                        mode: Optional[Union[str, GameModeStr]] = None, limit: Optional[int] = None,
-                        offset: Optional[int] = None) -> Sequence[LegacyScore]:
+        return list(
+            map(
+                KudosuHistory,
+                await self.http.make_request(Path.get_user_kudosu(user), limit=limit, offset=offset),
+            )
+        )
+
+    async def get_user_scores(
+        self,
+        user: int,
+        type: Union[UserScoreType, str],
+        include_fails: Optional[bool] = False,
+        mode: Optional[Union[str, GameModeStr]] = None,
+        limit: Optional[int] = None,
+        offset: Optional[int] = None,
+    ) -> List[Union[LegacyScore, SoloScore]]:
         """
         This endpoint returns the scores of specified user.
 
         Requires OAuth and scope public
 
         **Parameters**
 
         user: :class:`int`
             Id of the user.
 
-        type: union[:class:`UserScoreType` :class:`str`]
-            Score type. Must be one of these: best, firsts, recent
+        type: Union[:class:`UserScoreType` :class:`str`]
+            Score type. Must be one of `best`, `firsts`, `recent`
 
-        include_fails: Optional[:class:`int`]
-            Only for recent scores, include scores of failed plays. Set to 1 to include them. Defaults to 0.
+        include_fails: Optional[:class:`bool`]
+            Only for recent scores, include scores of failed plays. Defaults to False.
 
         mode: Optional[Union[:class:`GameModeStr`, :class:`str`]]
             game mode of the scores to be returned. Defaults to the specified user's mode.
 
         limit: Optional[:class:`int`]
             Maximum number of results.
 
         offset: Optional[:class:`int`]
             Result offset for pagination.
 
         **Returns**
 
-        Sequence[:class:`LegacyScore`]
-            Includes attributes beatmap, beatmapset, weight: Only for type best, user
+        Sequence[Union[:class:`LegacyScore`, :class:`SoloScore`]]
+            Includes attributes `beatmap`, `beatmapset`. Additionally includes `weight` if `type` is `best`.
         """
         mode, type = parse_enum_args(mode, type)
-        return [LegacyScore(score) for score in await self.http.make_request(Path.get_user_scores(user, type),
-                                                                       include_fails=include_fails, mode=mode,
-                                                                       limit=limit, offset=offset)]
-
-    async def get_user_beatmaps(self, user: int, type: Union[str, UserBeatmapType], limit: Optional[int] = None,
-                          offset: Optional[int] = None) -> Sequence[Union[BeatmapPlaycount, Beatmapset]]:
+        return list(
+            map(
+                get_score_object,
+                await self.http.make_request(
+                    Path.get_user_scores(user, type),
+                    include_fails=int(include_fails),
+                    mode=mode,
+                    limit=limit,
+                    offset=offset,
+                ),
+            )
+        )
+
+    async def get_user_beatmaps(
+        self,
+        user: int,
+        type: Union[str, UserBeatmapType],
+        limit: Optional[int] = None,
+        offset: Optional[int] = None,
+    ) -> List[Union[BeatmapPlaycount, Beatmapset]]:
         """
         Returns the beatmaps of specified user.
 
         Requires OAuth and scope public
 
         **Parameters**
 
         user: :class:`int`
             Id of the user.
 
         type: Union[:class:`str`, :class:`UserBeatmapType`]
-            Beatmap type. Can be one of the following - favourite, graveyard, loved, most_played, pending, ranked.
+            Beatmap type. Can be one of `favourite`, `graveyard`, `loved`, `most_played`, `pending`, `ranked`.
 
         limit: Optional[:class:`int`]
             Maximum number of results.
 
         offset: Optional[:class:`int`]
             Result offset for pagination.
 
         **Returns**
 
-        Sequence[Union[:class:`BeatmapPlaycount`, :class:`Beatmapset`]]
-            :class:`BeatmapPlaycount` for type most_played or :class:`Beatmapset` for any other type.
+        List[Union[:class:`BeatmapPlaycount`, :class:`Beatmapset`]]
+            :class:`BeatmapPlaycount` for `type` `most_played` and :class:`Beatmapset` for any other type.
         """
-        object_type = Beatmapset
         type = parse_enum_args(type)
-        if type == 'most_played':
-            object_type = BeatmapPlaycount
-        return list(map(object_type, await self.http.make_request(Path.get_user_beatmaps(user, type),
-                                                            limit=limit, offset=offset)))
-
-    async def get_user_recent_activity(self, user: int, limit: Optional[int] = None,
-                                 offset: Optional[int] = None) -> Sequence[Event]:
+        return list(
+            map(
+                BeatmapPlaycount if type == "most_played" else Beatmapset,
+                await self.http.make_request(Path.get_user_beatmaps(user, type), limit=limit, offset=offset),
+            )
+        )
+
+    async def get_user_recent_activity(
+        self, user: int, limit: Optional[int] = None, offset: Optional[int] = None
+    ) -> List[EVENT_TYPE]:
         """
         Returns recent activity.
 
         Requires OAuth and scope public
 
         **Parameters**
 
@@ -1736,57 +1930,69 @@
             Maximum number of results.
 
         offset: Optional[:class:`int`]
             Result offset for pagination.
 
         **Returns**
 
-        Sequence[:class:`Event`]
+        List[:class:`Event`]
             list of :class:`Event` objects
         """
-        return list(map(Event, await self.http.make_request(Path.get_user_recent_activity(user),
-                                                      limit=limit, offset=offset)))
-
-    async def get_user(self, user: int, mode: Optional[Union[str, GameModeStr]] = '',
-                       key: Optional[str] = None) -> User:
+        return list(
+            map(
+                get_event_object,
+                await self.http.make_request(Path.get_user_recent_activity(user), limit=limit, offset=offset),
+            )
+        )
+
+    async def get_user(
+        self,
+        user: int,
+        mode: Optional[Union[str, GameModeStr]] = "",
+        key: Optional[str] = None,
+    ) -> User:
         """
         This endpoint returns the detail of specified user.
 
+        NOTE: It's highly recommended to pass key parameter
+        to avoid getting unexpected result (mainly when
+        looking up user with numeric username or nonexistent user id).
+
         Requires OAuth and scope public
 
         **Parameters**
 
         user: Union[:class:`int`, :class:`str`]
             Id or username of the user. Id lookup is prioritised unless key parameter is specified.
             Previous usernames are also checked in some cases.
 
         mode: Optional[Union[:class:`str`, :class:`GameModeStr`]
             User default mode will be used if not specified.
 
         key: Optional[:class:`str`]
-            Type of user passed in url parameter. Can be either id or username
+            Type of user passed in url parameter. Can be either `id` or `username`
             to limit lookup by their respective type. Passing empty or invalid
             value will result in id lookup followed by username lookup if not found.
 
         **Returns**
 
         :class:`User`
-            Includes following attributes: account_history, active_tournament_banner,
-            badges, beatmap_playcounts_count, favourite_beatmapset_count, follower_count,
-            graveyard_beatmapset_count, groups, loved_beatmapset_count,
-            mapping_follower_count, monthly_playcounts, page, pending_beatmapset_count,
-            previous_usernames, rank_history, ranked_beatmapset_count, replays_watched_counts,
-            scores_best_count, scores_first_count, scores_recent_count, statistics,
-            statistics.country_rank, statistics.rank, statistics.variants, support_level,
-            user_achievements.
+            Includes attributes `account_history`, `active_tournament_banner`, `badges`,
+            `beatmap_playcounts_count`, `favourite_beatmapset_count`, `follower_count`,
+            `graveyard_beatmapset_count`, `groups`, `loved_beatmapset_count`, `mapping_follower_count`,
+            `monthly_playcounts`, `page`, `pending_beatmapset_count`, `previous_usernames`,
+            `rank_highest`, `rank_history`, `ranked_beatmapset_count`, `replays_watched_counts`,
+            `scores_best_count`, `scores_first_count`, `scores_recent_count`, `statistics`,
+            `statistics.country_rank`, `statistics.rank`, `statistics.variants`, `support_level`,
+            `user_achievements`.
         """
         mode = parse_enum_args(mode)
         return User(await self.http.make_request(Path.get_user(user, mode), key=key))
 
-    async def get_users(self, ids: Sequence[int]) -> Sequence[UserCompact]:
+    async def get_users(self, ids: Sequence[int]) -> List[UserCompact]:
         """
         Returns list of users.
 
         Requires OAuth and scope public
 
         **Parameters**
 
@@ -1818,20 +2024,23 @@
 
         **Returns**
 
         :class:`WikiPage`
         """
         return WikiPage(await self.http.make_request(Path.get_wiki_page(locale, path)))
 
-    async def get_beatmapset_events(self, page: Optional[int] = None, limit: Optional[int] = None,
-                              sort: Optional[Union[str, BeatmapsetEventSort]] = None,
-                              type: Optional[Union[str, BeatmapsetEventType]] = None,
-                              min_date: Optional[Union[str, datetime]] = None,
-                              max_date: Optional[Union[str, datetime]] = None) -> \
-            Dict[str, Union[Sequence[BeatmapsetEvent], Dict, Sequence[UserCompact]]]:
+    async def get_beatmapset_events(
+        self,
+        page: Optional[int] = None,
+        limit: Optional[int] = None,
+        sort: Optional[Union[str, BeatmapsetEventSort]] = None,
+        type: Optional[Union[str, BeatmapsetEventType]] = None,
+        min_date: Optional[Union[str, datetime]] = None,
+        max_date: Optional[Union[str, datetime]] = None,
+    ) -> GetBeatmapsetEventsResult:
         """
         Returns a list of beatmapset events.
 
         Requires OAuth and scope public.
 
         **Parameters**
 
@@ -1843,65 +2052,59 @@
             Specified a sort order.
 
         type: Optional[Union[:class:`str`, :class:`BeatmapsetEventType`]]
             Specifies for only a certain type of event to be returned.
 
         **Returns**
 
-        Dict[str, Union[Sequence[BeatmapsetEvent], Dict, Sequence[UserCompact]]]
-
-        {
-
-            'events': Sequence[BeatmapsetEvent],
-
-            'reviews_config': Dict,
-
-            'users': Sequence[UserCompact]
-
-        }
+        :class:`GetBeatmapsetEventsResult`
         """
         sort, type = parse_enum_args(sort, type)
         if isinstance(min_date, datetime):
             min_date = min_date.isoformat()
         if isinstance(max_date, datetime):
             max_date = max_date.isoformat()
-        resp = await self.http.make_request(Path.get_beatmapset_events(), page=page, limit=limit, sort=sort,
-                                      type=type, min_date=min_date, max_date=max_date)
-        return {
-            "events": [BeatmapsetEvent(event) for event in resp['events']],
-            "reviews_config": resp['reviewsConfig'],
-            "users": [UserCompact(user) for user in resp['users']],
-        }
-
-    async def get_matches(self, limit: Optional[int] = None, sort: Optional[Union[str, MatchSort]] = None) \
-            -> Dict[str, Union[Sequence[Match], Dict]]:
+        resp = await self.http.make_request(
+            Path.get_beatmapset_events(),
+            page=page,
+            limit=limit,
+            sort=sort,
+            type=type,
+            min_date=min_date,
+            max_date=max_date,
+        )
+        return GetBeatmapsetEventsResult(
+            list(map(BeatmapsetEvent, resp["events"])),
+            Review(resp["reviewsConfig"]),
+            list(map(UserCompact, resp["users"])),
+        )
+
+    async def get_matches(
+        self, limit: Optional[int] = None, sort: Optional[Union[str, MatchSort]] = None
+    ) -> GetMatchesResult:
         """
         Returns a list of matches.
 
         Requires OAuth and scope public.
 
         **Parameters**
 
         limit: Optional[:class:`int`]
 
         sort: Optional[Union[:class:`str`, :class:`MatchSort`]]
 
         **Returns**
 
-        Dict[:class:`str`, Union[Dict, Sequence[:class:`Match`]]]
+        :class:`GetMatchesResult`
         """
         sort = parse_enum_args(sort)
         resp = await self.http.make_request(Path.get_matches(), limit=limit, sort=sort)
-        return {
-            "matches": list(map(Match, resp['matches'])),
-            "cursor": resp['cursor'],
-            "params": resp['params'],
-        }
+        return GetMatchesResult(list(map(Match, resp["matches"])), resp["params"], resp["cursor"])
 
-    async def get_match(self, match_id: int) -> Match:
+    async def get_match(self, match_id: int) -> MatchExtended:
         """
         Returns a match by id.
 
         Requires OAuth and scope public.
 
         **Parameters**
 
@@ -1910,19 +2113,23 @@
 
         **Returns**
 
         :class:`Match`
         """
         return MatchExtended(await self.http.make_request(Path.get_match(match_id)))
 
-    async def get_rooms(self, mode: Union[str, GameModeStr] = '', sort: Optional[Union[str, RoomSort]] = None,
-                  limit: Optional[int] = None,
-                  room_type: Optional[Union[RoomType, str]] = None,
-                  category: Optional[Union[RoomCategory, str]] = None,
-                  filter_mode: Optional[Union[RoomFilterMode, str]] = None) -> Sequence[Room]:
+    async def get_rooms(
+        self,
+        mode: Union[str, GameModeStr] = "",
+        sort: Optional[Union[str, RoomSort]] = None,
+        limit: Optional[int] = None,
+        room_type: Optional[Union[RoomType, str]] = None,
+        category: Optional[Union[RoomCategory, str]] = None,
+        filter_mode: Optional[Union[RoomFilterMode, str]] = None,
+    ) -> List[Room]:
         """
         Returns a list of rooms.
 
         Requires OAuth, scope public, and a user (authorization code grant, delegate scope, or password auth).
 
         **Parameters**
 
@@ -1939,18 +2146,28 @@
             type of room to look for
 
         category: Optional[Union[:class:`RoomCategory`, :class:`str`]]
             type of category of room to look for
 
         filter_mode: Optional[Union[:class:`RoomFilterMode`, :class:`str`]]
         """
-        mode, sort, room_type, category, filter_mode = parse_enum_args(
-            mode, sort, room_type, category, filter_mode)
-        return list(map(Room, await self.http.make_request(Path.get_rooms(mode), sort=sort, limit=limit,
-                                                     type_group=room_type, category=category, mode=filter_mode)))
+        mode, sort, room_type, category, filter_mode = parse_enum_args(mode, sort, room_type, category, filter_mode)
+        return list(
+            map(
+                Room,
+                await self.http.make_request(
+                    Path.get_rooms(mode),
+                    sort=sort,
+                    limit=limit,
+                    type_group=room_type,
+                    category=category,
+                    mode=filter_mode,
+                ),
+            )
+        )
 
     async def get_seasonal_backgrounds(self) -> SeasonalBackgrounds:
         """
         Get the season backgrounds.
 
         Doesn't require OAuth
 
@@ -1973,108 +2190,83 @@
 
         **Returns**
 
         :class:`Room`
         """
         return Room(await self.http.make_request(Path.get_room(room_id)))
 
-    async def get_score_by_id(self, mode, score_id) -> LegacyScore:
+    async def get_score_by_id(self, mode, score_id) -> Union[LegacyScore, SoloScore]:
         """
         Returns a score by id.
 
         Requires OAuth and scope public.
 
         **Parameters**
 
         mode: Union[:class:`str`, :class:`GameModeStr`]
 
         score_id: :class:`int`
 
         **Returns**
 
-        :class:`LegacyScore`
+        Union[:class:`SoloScore`, :class:`LegacyScore`]
         """
         mode = parse_enum_args(mode)
-        return LegacyScore(await self.http.make_request(Path.get_score_by_id(mode, score_id)))
+        return get_score_object(await self.http.make_request(Path.get_score_by_id(mode, score_id)))
 
-    async def search_beatmapsets(self, filters=None, page=None) -> dict:
+    async def search_beatmapsets(self, filters=None, page=None) -> BeatmapsetSearchResult:
         """
         Search for beatmapsets.
 
         Requires OAuth and scope public.
 
         **Attributes**
 
         filters: Optional[:class:`BeatmapsetSearchFilter`]
 
         page: Optional[:class:`int`]
 
         **Returns**
 
-        {
-
-        "beatmapsets": Sequence[:class:`Beatmapset`]
-
-        "cursor": :class:`dict`,
-
-        "search": :class:`dict`,
-
-        "recommended_difficulty": Union[:class:`float`, :class:`None`]
-
-        "error": Union[:class:`str`, :class:`None`]
-
-        "total": :class:`int`
-
-        }
+        :class:`BeatmapsetSearchResult`
         """
         if filters is None:
             filters = {}
         if isinstance(filters, BeatmapsetSearchFilter):
             filters = filters.filters
         resp = await self.http.make_request(Path.beatmapset_search(), page=page, **filters)
-        return {
-            'beatmapsets': [Beatmapset(beatmapset) for beatmapset in resp['beatmapsets']],
-            'cursor': resp['cursor'],
-            'search': resp['search'],
-            'recommended_difficulty': resp['recommended_difficulty'],
-            'error': resp['error'],
-            'total': resp['total'],
-        }
+        return BeatmapsetSearchResult(
+            list(map(Beatmapset, resp["beatmapsets"])),
+            resp["cursor"],
+            resp["search"],
+            resp["recommended_difficulty"],
+            resp["error"],
+            resp["total"],
+        )
 
-    async def get_room_leaderboard(self, room_id: int) -> \
-            Dict[str, Union[Sequence[UserScoreAggregate], Union[UserScoreAggregate, None]]]:
+    async def get_room_leaderboard(self, room_id: int) -> GetRoomLeaderboardResult:
         """
         Return a room's leaderboard. The :class:`UserScoreAggregate` objects returned under the "leaderboard"
         key contain the "user" attribute. The :class:`UserScoreAggregate` object under the "user_score" key
         contains the "user" and "position" attributes.
 
         Requires OAuth, scope public, and a user (authorization code grant, delegate scope, or password auth).
 
         **Parameters**
 
         room_id: :class:`int`
 
         **Returns**
 
-        Dict[:class:`str`, Union[Sequence[:class:`UserScoreAggregate`],
-        Union[:class:`UserScoreAggregate`, :class:`NoneType`]]]
-
-        {
-
-            'leaderboard': Sequence[:class:`UserScoreAggregate`],
-
-            'user_score': Union[:class:`UserScoreAggregate`, :class:`NoneType`]
-
-        }
+        :class:`GetRoomLeaderboard`
         """
         resp = await self.http.make_request(Path.get_room_leaderboard(room_id))
-        return {
-            'leaderboard': list(map(UserScoreAggregate, resp['leaderboard'])),
-            'user_score': UserScoreAggregate(resp['user_score']) if resp['user_score'] is not None else None,
-        }
+        return GetRoomLeaderboardResult(
+            list(map(UserScoreAggregate, resp["leaderboard"])), get_optional(resp, "user_score", UserScoreAggregate)
+        )
 
     async def get_replay_data(self, mode, score_id):
         """
         Returns replay data for a score.
 
         Requires OAuth, scope public, and a user (authorization code grant, delegate scope, or password auth).
 
@@ -2095,82 +2287,18 @@
         """
         Returns a list of friends.
 
         Requires OAuth, scope friends.read, and a user (authorization code grant, delegate scope, or password auth).
 
         **Returns**
 
-        Sequence[:class:`User`]
+        List[:class:`User`]
         """
         return list(map(UserCompact, await self.http.make_request(Path.get_friends())))
 
-    async def get_new_score_token(self, beatmap_id: int, version_hash: str, beatmap_hash: str,
-                            ruleset: Union[GameModeInt, GameModeStr, int]) -> dict:
-        """
-        Creates a score token with which can be used to submit a score.
-
-        Requires OAuth, lazer scope, and a user (authorization code grant, delegate scope, or password auth).
-
-        **Parameters**
-
-        beatmap_id: :class:`int`
-            id of the beatmap
-
-        version_hash: :class:`str`
-            version hash is the md5 checksum of f"{game_version}{os_enum}"
-            os_enum is Windows = 1, Linux = 2, macOS = 3, iOS = 4, Android = 5
-
-        beatmap_hash: :class:`str`
-            md5 hash of the beatmap
-
-        ruleset: Union[:class:`GameModeStr`, :class:`GameModeInt`, :class:`int`]
-
-        **Returns**
-
-        :class:`dict`
-
-        {
-
-        "beatmap_id": :class:`int`,
-
-        "created_at": :class:`datetime.datetime`
-
-        "id": :class:`int`
-
-        "user_id": :class:`int`
-
-        }
-        """
-        if isinstance(ruleset, GameModeStr):
-            ruleset = GameModeStr.get_int_equivalent(ruleset)
-        ruleset = parse_enum_args(ruleset)
-        data = {"version_hash": version_hash, "beatmap_hash": beatmap_hash, "ruleset_id": ruleset}
-        resp = await self.http.make_request(Path.get_new_score_id(beatmap_id), files=create_multipart_formdata(data))
-        resp["created_at"] = parser.parse(resp["created_at"])
-        return resp
-
-    async def submit_score(self, beatmap_id, token, score_data) -> SoloScore:
-        """
-        Submits a score
-
-        Requires OAuth, lazer scope, and a user (authorization code grant, delegate scope, or password auth).
-
-        **Parameters**
-
-        beatmap_id: :class:`int`
-            id of the beatmap
-
-        token: :class:`str`
-            score token which can be obtained from Client.get_new_score_token
-
-        score_data: :class:`dict`
-            data of the score which is being submitted
-        """
-        return SoloScore(await self.http.make_request(Path.submit_score(beatmap_id, token), data=score_data))
-
     async def favourite_beatmapset(self, beatmapset_id: int, favourite: bool) -> int:
         """
         Add or remove a favourite beatmapset
 
         Requires OAuth, lazer scope, and a user (authorization code grant, delegate scope, or password auth).
 
         **Parameters**
@@ -2181,61 +2309,69 @@
             whether to favourite (true) or unfavourite (false)
 
         **Returns**
 
         :class:`int`
             The number of favourites on the beatmapsets
         """
-        resp = await self.http.make_request(Path.favourite_beatmapset(beatmapset_id),
-                                      data={"action": "favourite" if favourite else "unfavourite"})
+        resp = await self.http.make_request(
+            Path.favourite_beatmapset(beatmapset_id),
+            data={"action": "favourite" if favourite else "unfavourite"},
+        )
         return resp["favourite_count"]
 
     async def get_open_chat_channels(self):
         """
         Get a list of chat channels that you have open. Includes recent DMs and public chat channels.
 
         Requires OAuth, lazer scope, and a user (authorization code grant, delegate scope, or password auth).
 
         **Returns**
 
-        Sequence[:class:`ChatChannel`]
+        List[:class:`ChatChannel`]
         """
         return list(map(ChatChannel, await self.http.make_request(Path.get_chat_presence())))
 
-    async def join_user_to_room(self, room: int, user: int, password: Optional[str] = None):
+    async def join_user_to_room(self, room: int, user: int, password: Optional[str] = None) -> None:
         """
-        Invite a user to a room.
+        Join a user to a room.
 
         Requires OAuth, lazer scope, and a user (authorization code grant, delegate scope, or password auth).
 
         **Parameters**
 
         room: :class:`int`
 
         user: :class:`int`
 
         password: Optional[:class:`str`]
         """
-        return await self.http.make_request(Path.join_to_room(room, user), password=password)
+        await self.http.make_request(Path.join_to_room(room, user), password=password)
 
-    async def kick_user_from_room(self, room: int, user: int):
+    async def kick_user_from_room(self, room: int, user: int) -> None:
         """
-        Kick a user from a room (or leave by kicking yourself).
+        Kick a user from a room.
 
         Requires OAuth, lazer scope, and a user (authorization code grant, delegate scope, or password auth).
 
         **Parameters**
 
         room: :class:`int`
 
         user: :class:`int`
         """
-        return await self.http.make_request(Path.kick_from_room(room, user))
+        await self.http.make_request(Path.kick_from_room(room, user))
 
-    async def report(self, comments: str, reason: str, reportable_id: int, reportable_type: Union[ObjectType, str]):
+    async def report(
+        self,
+        comments: str,
+        reason: str,
+        reportable_id: int,
+        reportable_type: Union[ObjectType, str],
+    ) -> None:
         """
         Send a report.
 
         Requires OAuth, lazer scope, and a user (authorization code grant, delegate scope, or password auth).
 
         **Parameters**
 
@@ -2244,25 +2380,31 @@
         reason: :class:`str`
 
         reportable_id: :class:`id`
 
         reportable_type: Union[:class:`str`, :class:`ObjectType`]
         """
         params = {
-            "comments": comments, "reason": reason, "reportable_id": reportable_id,
-            "reportable_type": parse_enum_args(reportable_type)
+            "comments": comments,
+            "reason": reason,
+            "reportable_id": reportable_id,
+            "reportable_type": parse_enum_args(reportable_type),
         }
         await self.http.make_request(Path.send_report(), **params)
 
-    async def create_multiplayer_room(self, name: str, starting_map: Union[PlaylistItemUtil, dict],
-                                password: Optional[str] = None,
-                                queue_mode: Optional[Union[RealTimeQueueMode, str]] = RealTimeQueueMode.HOST_ONLY,
-                                auto_start_duration: Optional[int] = 0,
-                                room_type: Optional[Union[RealTimeType, str]] = RealTimeType.HEAD_TO_HEAD,
-                                auto_skip: Optional[bool] = False) -> Room:
+    async def create_multiplayer_room(
+        self,
+        name: str,
+        starting_map: Union[PlaylistItemUtil, dict],
+        password: Optional[str] = None,
+        queue_mode: Optional[Union[RealTimeQueueMode, str]] = RealTimeQueueMode.HOST_ONLY,
+        auto_start_duration: Optional[int] = 0,
+        room_type: Optional[Union[RoomType, str]] = RoomType.HEAD_TO_HEAD,
+        auto_skip: Optional[bool] = False,
+    ) -> Room:
         """
         Create a multiplayer (realtime) room.
 
         Requires OAuth, lazer scope, and a user (authorization code grant, delegate scope, or password auth).
 
         **Parameters**
 
@@ -2275,38 +2417,48 @@
             Password to enter the room which is optional.
 
         queue_mode: Optional[Union[:class:`RealTimeQueueMode`, :class:`str`]]
             The mode for queuing maps.
 
         auto_start_duration: Optional[:class:`int`]
 
-        room_type: Optional[Union[:class:`RealTimeType`, :class:`str`]]
+        room_type: Optional[Union[:class:`RoomType`, :class:`str`]]
 
         auto_skip: Optional[:class:`bool`]
             Whether to automatically skip intro or not.
 
         **Returns**
 
         :class:`Room`
         """
         if isinstance(starting_map, PlaylistItemUtil):
             starting_map = starting_map.json
         queue_mode, room_type = parse_enum_args(queue_mode, room_type)
         data = {
-            "name": name, "password": password, "playlist": [starting_map],
-            "queue_mode": queue_mode, "auto_start_duration": auto_start_duration,
-            "category": "realtime", "type": room_type, "auto_skip": auto_skip,
+            "name": name,
+            "password": password,
+            "playlist": [starting_map],
+            "queue_mode": queue_mode,
+            "auto_start_duration": auto_start_duration,
+            "category": "realtime",
+            "type": room_type,
+            "auto_skip": auto_skip,
         }
         return Room(await self.http.make_request(Path.create_room(), data=json.dumps(data)))
 
-    async def create_playlist(self, name: str, playlist_items: Sequence[Union[PlaylistItemUtil, dict]],
-                        duration: Optional[int] = None, ends_at: Optional[Union[str, datetime]] = None,
-                        max_attempts: Optional[int] = None,
-                        queue_mode: Optional[Union[PlaylistQueueMode, str]] = PlaylistQueueMode.HOST_ONLY,
-                        auto_start_duration: Optional[int] = 0):
+    async def create_playlist(
+        self,
+        name: str,
+        playlist_items: Sequence[Union[PlaylistItemUtil, dict]],
+        duration: Optional[int] = None,
+        ends_at: Optional[Union[str, datetime]] = None,
+        max_attempts: Optional[int] = None,
+        queue_mode: Optional[Union[PlaylistQueueMode, str]] = PlaylistQueueMode.HOST_ONLY,
+        auto_start_duration: Optional[int] = 0,
+    ) -> Room:
         """
         Create a playlist
 
         Requires OAuth, lazer scope, and a user (authorization code grant, delegate scope, or password auth).
 
         **Parameters**
 
@@ -2328,34 +2480,41 @@
         max_attempts: Optional[:class:`int`]
             Null means infinite attempts.
 
         queue_mode: Optional[Union[:class:`PlaylistQueueMode`, :class:`str`]]
             PlaylistQueueMode.HOST_ONLY is the only option
 
         auto_start_duration: Optional[:class:`int`]
+
+        **Returns**
+
+        :class:`Room`
         """
         if duration is None and ends_at is None:
             raise ValueError("Either duration or ends_at must be not null.")
         if ends_at is not None and isinstance(ends_at, datetime):
             ends_at = ends_at.isoformat()
         playlist_items = [item.json if isinstance(item, PlaylistItemUtil) else item for item in playlist_items]
         data = {
-            "name": name, "max_attempts": max_attempts, "duration": duration,
-            "ends_at": ends_at, "queue_mode": parse_enum_args(queue_mode),
-            "auto_start_duration": auto_start_duration, "category": "playlists",
+            "name": name,
+            "max_attempts": max_attempts,
+            "duration": duration,
+            "ends_at": ends_at,
+            "queue_mode": parse_enum_args(queue_mode),
+            "auto_start_duration": auto_start_duration,
+            "category": "playlists",
             "playlist": playlist_items,
         }
         return Room(await self.http.make_request(Path.create_room(), data=json.dumps(data)))
 
-    async def check_download_quota(self):
+    async def check_download_quota(self) -> int:
         """
         Get the amount of quota you've used.
 
         Requires OAuth, lazer scope, and a user (authorization code grant, delegate scope, or password auth).
 
-        Requires
-
         **Returns**
 
         :class:`int`
         """
-        return (await self.http.make_request(Path.download_quota_check()))["quota_used"]
+        resp = await self.http.make_request(Path.download_quota_check())
+        return resp["quota_used"]
```

### Comparing `osu.py-0.6.0/osu/asyncio/http.py` & `osu.py-1.0.0/osu/asyncio/http.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,23 +8,27 @@
 
 class AsynchronousHTTPHandler:
     def __init__(self, client, request_wait_time, limit_per_minute, use_lazer=False):
         self.client = client
         self.rate_limit = RateLimitHandler(request_wait_time, limit_per_minute)
         self.use_lazer = use_lazer
 
-    def get_headers(self, requires_auth=True, is_files=False, **kwargs):
+    def get_headers(self, path, is_files=False, **kwargs):
         headers = {
-            'charset': 'utf-8',
-            **{str(key): str(value) for key, value in kwargs.items() if value is not None}
+            "charset": "utf-8",
+            "x-api-version": "20220705",
+            "Accept": path.accept,
         }
-        if not is_files and "Content-Type" not in headers:
-            headers["Content-Type"] = "application/json"
-        if requires_auth and "Authorization" not in headers:
-            headers['Authorization'] = f"Bearer {self.client.auth.token}"
+        if not is_files:  # otherwise let requests library handle it
+            headers["Content-Type"] = path.content_type
+        if path.requires_auth and "Authorization" not in headers:
+            headers["Authorization"] = f"Bearer {self.client.auth.token}"
+        for key, value in kwargs.items():
+            if value is not None:
+                headers[str(key)] = str(value)
         return headers
 
     async def make_request(self, path, data=None, headers=None, is_download=False, files=None, **kwargs):
         if headers is None:
             headers = {}
         if data is None:
             data = {}
@@ -32,75 +36,81 @@
         if path.requires_auth and self.client.auth is None:
             raise ScopeException("You need to be authenticated to make this request.")
 
         if path.requires_auth and path.scope not in self.client.auth.scope:
             raise ScopeException(f"You don't have the {path.scope} scope, which is required to make this request.")
 
         if path.requires_user and not self.client.auth.has_user:
-            raise ScopeException("This request requires a user. You need either a delegate scope or "
-                                 "to register OAuth with Authorization Code Grant.")
+            raise ScopeException(
+                "This request requires a user. You need either a delegate scope or "
+                "to register OAuth with Authorization Code Grant."
+            )
 
-        headers = self.get_headers(path.requires_auth, files is not None, **headers)
+        headers = self.get_headers(path, files is not None, **headers)
         params = {str(key): value for key, value in kwargs.items() if value is not None}
         if files is not None:
             data = dict(map(lambda item: (item[0], item[1][1]), files.items()))
 
         async with aiohttp.ClientSession() as session:
             if not self.rate_limit.can_request:
                 await self.rate_limit.wait()
 
             self.rate_limit.request_used()
-            async with session.request(path.method,
-                                       (lazer_base_url if self.use_lazer else base_url) + path.path,
-                                       headers=headers, data=data, params=params) as resp:
+            async with session.request(
+                path.method,
+                (lazer_base_url if self.use_lazer else base_url) + path.path,
+                headers=headers,
+                data=data,
+                params=params,
+            ) as resp:
                 try:
                     resp.raise_for_status()
                 except Exception as e:
                     try:
-                        err = (await resp.json())['error']
+                        err = (await resp.json())["error"]
                     except:
                         err = None
-                    raise type(e)(str(e) + ": " + err) if err is not None else e
+                    raise type(e)(str(e) + ": " + err) if err is not None else e from None
                 if resp.content_length == 0:
                     return
                 return await resp.json() if not is_download else await resp.content.read()
 
 
 class RateLimitHandler:
     def __init__(self, request_wait_limit, limit_per_minute):
         self.wait_limit = request_wait_limit
         self.limit = limit_per_minute
         self.requests = []
-        self.waiting = False
+        self._wait = asyncio.Event()
+        self._wait.set()
 
     def request_used(self):
         self.requests.append(time.perf_counter())
         self.reset()
 
     async def wait(self):
-        while self.waiting:
-            await asyncio.sleep(0.1)
-        self.waiting = True
+        await self._wait.wait()
+        self._wait.clear()
         if self.can_request:  # Check again due to asynchronous running
-            self.waiting = False
+            self._wait.set()
             return
-        next_available_request = self.wait_limit-(time.perf_counter()-self.last_request)
+        next_available_request = self.wait_limit - (time.perf_counter() - self.last_request)
         if len(self.requests) >= self.limit:
-            next_available_request = max(next_available_request, self.requests[0]+60-time.perf_counter())
+            next_available_request = max(next_available_request, self.requests[0] + 60 - time.perf_counter())
         await asyncio.sleep(next_available_request)
-        self.waiting = False
+        self._wait.set()
 
     def reset(self):
         while len(self.requests) > 0:
             if self.requests[0] + 60 < time.perf_counter():
                 self.requests.pop(0)
             else:
                 break
 
     @property
     def can_request(self):
         self.reset()
-        return time.perf_counter()-self.last_request >= self.wait_limit and len(self.requests) < self.limit
+        return time.perf_counter() - self.last_request >= self.wait_limit and len(self.requests) < self.limit
 
     @property
     def last_request(self):
         return self.requests[-1] if len(self.requests) > 0 else 0
```

### Comparing `osu.py-0.6.0/osu/auth.py` & `osu.py-1.0.0/osu/auth.py`

 * *Files 11% similar despite different names*

```diff
@@ -32,49 +32,56 @@
     redirect_uri: :class:`str`
         Redirect uri
 
     scope: Optional[:class:`Scope`]
         Scope object helps the program identify what requests you can
         and can't make with your scope. Default is 'public' (Scope.default())
     """
+
     SAVE_VERSION = 1
 
-    def __init__(self, client_id: int, client_secret: str, redirect_url: str, scope: Optional[Scope] = Scope.default()):
-        if scope == 'lazer':
+    def __init__(
+        self,
+        client_id: int,
+        client_secret: str,
+        redirect_url: str,
+        scope: Optional[Scope] = Scope.default(),
+    ):
+        if scope == "lazer":
             raise ScopeException("The lazer scope signifies that an endpoint only meant for use by the lazer client.")
         self.client_id = client_id
         self.client_secret = client_secret
         self.redirect_url = redirect_url
         self.scope = scope
 
         self.refresh_token = None
         self._token = None
         self.expire_time = perf_counter()
         self._refresh_callback = None
 
-    def get_auth_url(self, state: Optional[str] = ''):
+    def get_auth_url(self, state: Optional[str] = ""):
         """
         Returns a url that a user can authorize their account at. They'll then be returned to
         the redirect_uri with a code that can be used under get_auth_token.
 
         **Parameters**
 
         state: Optional[:class:`str`]
             Will be returned to the redirect_uri along with the code.
         """
         params = {
-            'client_id': self.client_id,
-            'redirect_uri': self.redirect_url,
-            'response_type': 'code',
-            'scope': self.scope.scopes,
-            'state': state,
+            "client_id": self.client_id,
+            "redirect_uri": self.redirect_url,
+            "response_type": "code",
+            "scope": self.scope.scopes,
+            "state": state,
         }
-        if not params['state']:
-            del params['state']
-        return auth_url + "?" + "&".join([f'{key}={value}' for key, value in params.items()])
+        if not params["state"]:
+            del params["state"]
+        return auth_url + "?" + "&".join([f"{key}={value}" for key, value in params.items()])
 
     def get_auth_token(self, code: Optional[str] = None):
         """
         `code` parameter is not required, but without a code the scopes are restricted to
         public and delegate (more on delegation below). You can obtain a code by having
         a user authorize themselves under a url which you can get with get_auth_url.
         Read more about it under that function.
@@ -89,37 +96,41 @@
 
         **Parameters**
 
         code: Optional[:class:`str`]
             code from user authorizing at a specific url
         """
         data = {
-            'client_id': self.client_id,
-            'client_secret': self.client_secret,
+            "client_id": self.client_id,
+            "client_secret": self.client_secret,
         }
 
         if code is None:
-            data.update({
-                'grant_type': 'client_credentials',
-                'scope': 'public' if 'delegate' not in self.scope else self.scope.scopes,
-            })
+            data.update(
+                {
+                    "grant_type": "client_credentials",
+                    "scope": "public" if "delegate" not in self.scope else self.scope.scopes,
+                }
+            )
         else:
-            data.update({
-                'code': code,
-                'grant_type': 'authorization_code',
-                'redirect_uri': self.redirect_url,
-            })
+            data.update(
+                {
+                    "code": code,
+                    "grant_type": "authorization_code",
+                    "redirect_uri": self.redirect_url,
+                }
+            )
 
         response = requests.post(token_url, data=data)
         response.raise_for_status()
         response = response.json()
-        if 'refresh_token' in response:
-            self.refresh_token = response['refresh_token']
-        self._token = response['access_token']
-        self.expire_time = perf_counter() + response['expires_in']
+        if "refresh_token" in response:
+            self.refresh_token = response["refresh_token"]
+        self._token = response["access_token"]
+        self.expire_time = perf_counter() + response["expires_in"]
 
     def refresh_access_token(self, refresh_token: Optional[str] = None):
         """
         This function is usually executed by HTTPHandler, but if you have a
         refresh token saved from the last session, then you can fill in the
         `refresh_token` argument which this function will use to get a valid token.
 
@@ -129,51 +140,55 @@
             A refresh token used to get a new access token.
         """
         if refresh_token:
             self.refresh_token = refresh_token
         if perf_counter() < self.expire_time:
             return
         data = {
-            'client_id': self.client_id,
-            'client_secret': self.client_secret,
+            "client_id": self.client_id,
+            "client_secret": self.client_secret,
         }
         if self.refresh_token:
-            data.update({
-                'grant_type': 'refresh_token',
-                'refresh_token': self.refresh_token,
-            })
+            data.update(
+                {
+                    "grant_type": "refresh_token",
+                    "refresh_token": self.refresh_token,
+                }
+            )
         else:
-            data.update({
-                'grant_type': 'client_credentials',
-                'scope': 'public',
-            })
+            data.update(
+                {
+                    "grant_type": "client_credentials",
+                    "scope": "public",
+                }
+            )
         response = requests.post(token_url, data=data)
         response.raise_for_status()
         response = response.json()
-        if 'refresh_token' in response:
-            self.refresh_token = response['refresh_token']
-        self._token = response['access_token']
-        self.expire_time = perf_counter() + response['expires_in']
+        if "refresh_token" in response:
+            self.refresh_token = response["refresh_token"]
+        self._token = response["access_token"]
+        self.expire_time = perf_counter() + response["expires_in"]
         if self._refresh_callback:
             self._refresh_callback(self)
 
     @property
     def token(self):
         """
         Returns the access token. If the token is expired, it will be refreshed before being returned.
         """
-        if self.expire_time-5 <= perf_counter():
+        if self.expire_time - 5 <= perf_counter():
             self.refresh_access_token()
         return self._token
 
     @property
     def has_user(self):
-        return 'delegate' in self.scope or self.refresh_token is not None
+        return "delegate" in self.scope or self.refresh_token is not None
 
-    def set_refresh_callback(self, callback: Callable[['AuthHandler'], None]):
+    def set_refresh_callback(self, callback: Callable[["AuthHandler"], None]):
         """
         Set a callback to be called everytime the access token is refreshed.
 
         **Parameters**
 
         callback: :class:`Callable[['AuthHandler'], None]`
         """
@@ -199,38 +214,40 @@
         'scope': :class:`str`,
 
         'refresh_token': :class:`str`,
 
         }
         """
         return {
-            'save_version': self.SAVE_VERSION,
-            'client_id': self.client_id,
-            'client_secret': self.client_secret,
-            'redirect_url': self.redirect_url,
-            'scope': self.scope.scopes,
-            'refresh_token': self.refresh_token,
+            "save_version": self.SAVE_VERSION,
+            "client_id": self.client_id,
+            "client_secret": self.client_secret,
+            "redirect_url": self.redirect_url,
+            "scope": self.scope.scopes,
+            "refresh_token": self.refresh_token,
         }
 
     @classmethod
     def from_save_data(cls, save_data: dict):
         """
         Create a new :class:`AuthHandler` object from save data.
         """
-        save_version = save_data['save_version']
+        save_version = save_data["save_version"]
         if save_version != cls.SAVE_VERSION:
-            raise ValueError(f"The version of this save data ({save_version}) is not compatible "
-                             f"with the save data version of this AuthHandler object ({cls.SAVE_VERSION}).")
-
-        client_id = save_data['client_id']
-        client_secret = save_data['client_secret']
-        redirect_url = save_data['redirect_url']
-        scope = Scope(*save_data['scope'].split())
+            raise ValueError(
+                f"The version of this save data ({save_version}) is not compatible "
+                f"with the save data version of this AuthHandler object ({cls.SAVE_VERSION})."
+            )
+
+        client_id = save_data["client_id"]
+        client_secret = save_data["client_secret"]
+        redirect_url = save_data["redirect_url"]
+        scope = Scope(*save_data["scope"].split())
         auth = cls(client_id, client_secret, redirect_url, scope)
-        auth.refresh_access_token(save_data['refresh_token'])
+        auth.refresh_access_token(save_data["refresh_token"])
         return auth
 
 
 class LazerAuthHandler:
     # https://github.com/ppy/osu/blob/master/osu.Game/Online/ProductionEndpointConfiguration.cs
     LAZER_CLIENT_ID = 5
     LAZER_CLIENT_SECRET = "FGc9GAtyHzeQDshWP5Ah7dega8hJACAJpQtw6OXk"
@@ -276,14 +293,14 @@
         resp = resp.json()
         self._token = resp["access_token"]
         self.refresh_token = resp["refresh_token"]
         self.expire_time = perf_counter() + resp["expires_in"]
 
     @property
     def token(self):
-        if self.expire_time-5 <= perf_counter():
+        if self.expire_time - 5 <= perf_counter():
             self.refresh_access_token()
         return self._token
 
     @property
     def has_user(self):
         return self._token is not None
```

### Comparing `osu.py-0.6.0/osu/client.py` & `osu.py-1.0.0/osu/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,36 @@
 from .http import HTTPHandler
 from .objects import *
 from .path import Path
 from .enums import *
 from .auth import AuthHandler, LazerAuthHandler
 from .util import (
-    parse_mods_arg, parse_enum_args,
-    BeatmapsetSearchFilter, create_multipart_formdata,
-    PlaylistItemUtil, IdentitiesUtil, NotificationsUtil,
-    JsonUtil
+    parse_mods_arg,
+    parse_enum_args,
+    BeatmapsetSearchFilter,
+    create_multipart_formdata,
+    PlaylistItemUtil,
+    IdentitiesUtil,
+    NotificationsUtil,
+    JsonUtil,
+    get_optional_list,
 )
-from typing import Union, Optional, Sequence, Dict
+from .results import *
+
+from typing import Union, Optional, Sequence, Dict, List
 from datetime import datetime
 from osrparse import Replay
+from dateutil import parser
 import json
 
 
 class Client:
     """
-    Main object for interacting with osu!api
+    Main object for interacting with osu!api, which uses synchronous requests.
+    If you're looking for asynchronous requests, use :class:`AsynchronousClient`.
 
     **Init Parameters**
 
     auth: :class:`AuthHandler`
         The AuthHandler object passed in when initiating the Client object
 
     request_wait_time: Optional[:class:`float`]
@@ -49,62 +58,84 @@
 
     Current rate limit is set at an insanely high 1200 requests per minute,
     with burst capability of up to 200 beyond that.
     If you require more, you probably fall into the above category of abuse.
     If you are doing more than 60 requests a minute,
     you should probably give peppy a yell.
     """
-    def __init__(self, auth: Union[AuthHandler, LazerAuthHandler] = None, request_wait_time: Optional[float] = 1.0,
-                 limit_per_minute: Optional[float] = 60.0, use_lazer: Optional[bool] = False):
+
+    def __init__(
+        self,
+        auth: Union[AuthHandler, LazerAuthHandler] = None,
+        request_wait_time: Optional[float] = 1.0,
+        limit_per_minute: Optional[float] = 60.0,
+        use_lazer: Optional[bool] = False,
+    ):
         self.auth = auth
         self.http = HTTPHandler(self, request_wait_time, limit_per_minute, use_lazer)
 
     @classmethod
-    def from_client_credentials(cls, client_id: int, client_secret: str, redirect_url: str,
-                                scope: Optional[Scope] = Scope.default(), code: Optional[str] = None,
-                                request_wait_time: Optional[float] = 1.0,
-                                limit_per_minute: Optional[float] = 60.0):
+    def from_client_credentials(
+        cls,
+        client_id: int,
+        client_secret: str,
+        redirect_url: Optional[str],
+        scope: Optional[Scope] = Scope.default(),
+        code: Optional[str] = None,
+        request_wait_time: Optional[float] = 1.0,
+        limit_per_minute: Optional[float] = 60.0,
+    ) -> "Client":
         """
         Returns a :class:`Client` object from client id, client secret, redirect uri, and scope.
 
         **Parameters**
 
         client_id: :class:`int`
             API Client id
 
         client_secret: :class:`int`
             API Client secret
 
-        redirect_uri: :class:`str`
+        redirect_uri: Optional[:class:`str`]
             API redirect uri
 
         scope: Optional[:class:`Scope`]
             Scopes to use. Default is Scope.default() which is just the public scope.
 
         code: Optional[:class:`str`]
             If provided, is used to authorize. Read more about this under :class:`AuthHandler.get_auth_token`
 
         request_wait_time: Optional[:class:`float`]
-            Read under Client init parameters.
+            Default is 1.
+
+            This defines the amount of time that the client should wait before making another request.
+            It can make it easier to stay within the rate limits without using all your requests up quickly
+            and then waiting forever to make another. It's most applicable in bot-type apps.
 
         limit_per_minute: Optional[:class:`float`]
-            Read under Client init parameters.
+            Default is 60 because that's the limit peppy requests that we stay under.
+
+            This sets a cap on the number of requests the client is allowed to make within 1 minute of time.
 
         **Returns**
 
         :class:`Client`
         """
         auth = AuthHandler(client_id, client_secret, redirect_url, scope)
         auth.get_auth_token(code)
         return cls(auth, request_wait_time, limit_per_minute)
 
     @classmethod
-    def from_osu_credentials(cls, username: str, password: str,
-                             request_wait_time: Optional[float] = 1.0,
-                             limit_per_minute: Optional[float] = 60.0):
+    def from_osu_credentials(
+        cls,
+        username: str,
+        password: str,
+        request_wait_time: Optional[float] = 1.0,
+        limit_per_minute: Optional[float] = 60.0,
+    ) -> "Client":
         """
         Returns a :class:`Client` object which will make authorize and make requests to
         lazer.ppy.sh
 
         username: :class:`str`
             osu! username login
 
@@ -117,16 +148,20 @@
         limit_per_minute: Optional[:class:`float`]
             Read under Client init parameters.
         """
         auth = LazerAuthHandler(username, password)
         auth.get_auth_token()
         return cls(auth, request_wait_time, limit_per_minute, True)
 
-    def lookup_beatmap(self, checksum: Optional[str] = None, filename: Optional[str] = None,
-                       id: Optional[int] = None) -> Beatmap:
+    def lookup_beatmap(
+        self,
+        checksum: Optional[str] = None,
+        filename: Optional[str] = None,
+        id: Optional[int] = None,
+    ) -> Beatmap:
         """
         Returns beatmap.
 
         Requires OAuth and scope public
 
         **Parameters**
 
@@ -139,19 +174,23 @@
         id: Optional[:class:`int`]
             A beatmap ID to lookup
 
         **Returns**
 
         :class:`Beatmap`
         """
-        return Beatmap(self.http.make_request(Path.beatmap_lookup(), checksum=checksum,
-                                              filename=filename, id=id))
+        return Beatmap(self.http.make_request(Path.beatmap_lookup(), checksum=checksum, filename=filename, id=id))
 
-    def get_user_beatmap_score(self, beatmap: int, user: int, mode: Optional[Union[str, GameModeStr]] = None,
-                               mods: Optional[Sequence[str]] = None) -> BeatmapUserScore:
+    def get_user_beatmap_score(
+        self,
+        beatmap: int,
+        user: int,
+        mode: Optional[Union[str, GameModeStr]] = None,
+        mods: Optional[Sequence[str]] = None,
+    ) -> BeatmapUserScore:
         """
         Returns a user's score on a Beatmap
 
         Requires OAuth and scope public
 
         **Parameters**
 
@@ -168,19 +207,19 @@
             An array of matching mods, or none. Currently doesn't do anything.
 
         **Returns**
 
         :class:`BeatmapUserScore`
         """
         mode = parse_enum_args(mode)
-        return BeatmapUserScore(self.http.make_request(Path.user_beatmap_score(beatmap, user),
-                                                       mode=mode, mods=mods))
+        return BeatmapUserScore(self.http.make_request(Path.user_beatmap_score(beatmap, user), mode=mode, mods=mods))
 
-    def get_user_beatmap_scores(self, beatmap: int, user: int,
-                                mode: Optional[Union[str, GameModeStr]] = None) -> Sequence[LegacyScore]:
+    def get_user_beatmap_scores(
+        self, beatmap: int, user: int, mode: Optional[Union[str, GameModeStr]] = None
+    ) -> List[Union[LegacyScore, SoloScore]]:
         """
         Returns a user's scores on a Beatmap
 
         Requires OAuth and scope public
 
         **Parameters**
 
@@ -191,81 +230,123 @@
             Id of the user
 
         mode: Optional[Union[:class:`str`, :class:`GameModeStr`]]
             The game mode to get scores for
 
         **Returns**
 
-        Sequence[:class:`LegacyScore`]
+        List[Union[:class:`LegacyScore`, :class:`SoloScore`]]
         """
         mode = parse_enum_args(mode)
-        return list(map(LegacyScore, self.http.make_request(Path.user_beatmap_scores(beatmap, user),
-                                                            mode=mode)["scores"]))
-
-    def get_beatmap_scores(self, beatmap: int, mode: Optional[Union[str, GameModeStr]] = None,
-                           mods: Optional[Sequence[str]] = None,
-                           type: Optional[Sequence[str]] = None) -> BeatmapScores:
+        resp = self.http.make_request(Path.user_beatmap_scores(beatmap, user), mode=mode)
+        return list(
+            map(
+                get_score_object,
+                resp["scores"],
+            )
+        )
+
+    def _parse_mods_list(self, mods) -> Optional[List[str]]:
+        if mods is None:
+            return
+        return list(
+            map(
+                lambda mod: (Mod[mod.name].value if not isinstance(mod, Mod) else mod.value)
+                if type(mod) != str
+                else mod,
+                mods,
+            )
+        )
+
+    def get_beatmap_scores(
+        self,
+        beatmap: int,
+        mode: Optional[Union[str, GameModeStr]] = None,
+        mods: Optional[Union[Mods, Sequence[Union[Mods, Mod, str]]]] = None,
+        ranking_type: Optional[str] = None,
+    ) -> BeatmapScores:
         """
         Returns the top scores for a beatmap
 
         Requires OAuth and scope public
 
         **Parameters**
 
         beatmap: :class:`int`
             Id of the beatmap
 
         mode: Optional[Union[:class:`str`, :class:`GameModeStr`]]
             The game mode to get scores for
 
-        mods: Optional[Sequence[:class:`str`]]
-            An array of matching mods, or none. Currently doesn't do anything.
+        mods: Optional[Union[:class:`Mods`, Sequence[Union[:class:`Mods`, :class:`Mod`, :class:`str`]]]]
+            Must pass one of:
+            a :class:`Mods` object,
+            a list of string mod abbreviations,
+            a list of :class:`Mods` objects,
+            a list of :classL`Mod` objects
 
-        type: Optional[Sequence[:class:`str`]]
+        ranking_type: Optional[:class:`str`]
             Beatmap score ranking type. Currently doesn't do anything.
 
         **Returns**
 
         :class:`BeatmapScores`
             :class:`LegacyScore` object inside includes "user" and the included user includes "country" and "cover".
         """
         mode = parse_enum_args(mode)
-        return BeatmapScores(self.http.make_request(Path.beatmap_scores(beatmap), mode=mode,
-                                                    mods=mods, type=type))
-
-    def get_lazer_beatmap_scores(self, beatmap: int, mode: Optional[Union[str, GameModeStr]] = None,
-                                 mods: Optional[Sequence[str]] = None,
-                                 type: Optional[Sequence[str]] = None) -> BeatmapScores:
+        mods = self._parse_mods_list(mods)
+        return BeatmapScores(
+            self.http.make_request(
+                Path.beatmap_scores(beatmap),
+                mode=mode,
+                **{"mods[]": mods},
+                type=ranking_type,
+            )
+        )
+
+    def get_lazer_beatmap_scores(
+        self,
+        beatmap: int,
+        mode: Optional[Union[str, GameModeStr]] = None,
+        mods: Optional[str] = None,
+        type: Optional[str] = None,
+    ) -> BeatmapScores:
         """
         Returns the top scores for a beatmap on the lazer client.
 
         Requires OAuth and scope public
 
         **Parameters**
 
         beatmap: :class:`int`
-            Id of the beatmap
+            ID of the beatmap
 
         mode: Optional[Union[:class:`str`, :class:`GameModeStr`]]
             The game mode to get scores for
 
-        mods: Optional[Sequence[:class:`str`]]
-            An array of matching mods, or none. Currently doesn't do anything.
+        mods: Optional[:class:`str`]
+            Must pass one of:
+            a :class:`Mods` object,
+            a list of string mod abbreviations,
+            a list of :class:`Mods` objects,
+            a list of :classL`Mod` objects
 
-        type: Optional[Sequence[:class:`str`]]
+        type: Optional[:class:`str`]
             Beatmap score ranking type. Currently doesn't do anything.
 
         **Returns**
 
         :class:`BeatmapScores`
-            :class:`LazerScore` object inside includes "user" and the included user includes "country" and "cover".
+            :class:`SoloScore` object inside includes "user" and the included user includes "country" and "cover".
         """
         mode = parse_enum_args(mode)
-        return BeatmapScores(self.http.make_request(Path.lazer_beatmap_scores(beatmap), mode=mode,
-                                                    mods=mods, type=type), "lazer")
+        mods = self._parse_mods_list(mods)
+        return BeatmapScores(
+            self.http.make_request(Path.lazer_beatmap_scores(beatmap), mode=mode, mods=mods, type=type)
+        )
 
     def get_beatmap(self, beatmap: int) -> Beatmap:
         """
         Gets beatmap data for the specified beatmap ID.
 
         Requires OAuth and scope public
 
@@ -273,71 +354,79 @@
 
         beatmap: :class:`int`
             The ID of the beatmap
 
         **Returns**
 
         :class:`Beatmap`
-            Includes attributes beatmapset, failtimes, and max_combo
+            Includes attributes `beatmapset`, `beatmapset.ratings`, `failtimes`, `max_combo`.
         """
         return Beatmap(self.http.make_request(Path.beatmap(beatmap)))
 
-    def get_beatmaps(self, ids: Optional[Sequence[int]] = None) -> Sequence[Beatmap]:
+    def get_beatmaps(self, ids: Optional[Sequence[int]] = None) -> List[Beatmap]:
         """
         Returns list of beatmaps.
 
         Requires OAuth and scope public
 
         **Parameters**
 
         ids: Optional[List[:class:`int`]]
             Beatmap id to be returned. Specify once for each beatmap id requested.
             Up to 50 beatmaps can be requested at once.
 
         **Returns**
 
-        Sequence[:class:`BeatmapCompact`]
-            Includes: beatmapset (with ratings), failtimes, max_combo.
+        List[:class:`Beatmap`]
+            Includes attributes `beatmapset`, `beatmapset.ratings`, `failtimes`, `max_combo`.
         """
-        results = self.http.make_request(Path.beatmaps(), **{"ids[]": ids})
-        return list(map(Beatmap, results['beatmaps'])) if results else []
+        results = self.http.make_request(Path.beatmaps(), **{"ids[]": list(ids)})
+        return list(map(Beatmap, results["beatmaps"])) if results else []
 
-    def get_beatmap_attributes(self, beatmap: int,
-                               mods: Optional[Union[int, Mods, Sequence[Union[str, Mods, int]]]] = None,
-                               ruleset: Optional[Union[str, GameModeStr]] = None,
-                               ruleset_id: Optional[Union[int, GameModeInt]] = None) -> BeatmapDifficultyAttributes:
+    def get_beatmap_attributes(
+        self,
+        beatmap: int,
+        mods: Optional[Union[int, Mods, Sequence[Union[str, Mods, int]]]] = None,
+        ruleset: Optional[Union[str, GameModeStr]] = None,
+        ruleset_id: Optional[Union[int, GameModeInt]] = None,
+    ) -> BeatmapDifficultyAttributes:
         """
         Returns difficulty attributes of beatmap with specific mode and mods combination.
 
         Requires OAuth and scope public
 
         **Parameters**
 
         beatmap: :class:`int`
             Beatmap id.
 
         mods: Optional[Union[:class:`int`, Sequence[Union[:class:`str`, :class:`Mods`, :class:`int`]], :class:`Mods`]]
             Mod combination. Can be either a bitset of mods, a Mods enum, or array of any. Defaults to no mods.
             Some mods may cause the api to throw an HTTP 422 error depending on the map's gamemode.
 
-        ruleset: Optional[Union[:class:`GameModeStr`, :class:`int`]]
+        ruleset: Optional[Union[:class:`GameModeStr`, :class:`str`]]
             Ruleset of the difficulty attributes. Only valid if it's the beatmap ruleset or the beatmap can be
             converted to the specified ruleset. Defaults to ruleset of the specified beatmap.
 
         ruleset_id: Optional[Union[:class:`GameModeInt`, :class:`int`]]
-            The same as ruleset but in integer form.
+            The same as `ruleset` but in integer form.
 
         **Returns**
 
         :class:`BeatmapDifficultyAttributes`
         """
         ruleset, ruleset_id = parse_enum_args(ruleset, ruleset_id)
-        return BeatmapDifficultyAttributes(self.http.make_request(Path.get_beatmap_attributes(beatmap),
-                                                                  mods=parse_mods_arg(mods), ruleset=ruleset,
-                                                                  ruleset_id=ruleset_id))
+        return BeatmapDifficultyAttributes(
+            self.http.make_request(
+                Path.get_beatmap_attributes(beatmap),
+                mods=parse_mods_arg(mods),
+                ruleset=ruleset,
+                ruleset_id=ruleset_id,
+            )
+        )
 
     def get_beatmapset(self, beatmapset_id: int) -> Beatmapset:
         """
         Get beatmapset by id.
 
         Requires OAuth and scope public
 
@@ -347,18 +436,25 @@
 
         **Returns**
 
         :class:`Beatmapset`
         """
         return Beatmapset(self.http.make_request(Path.get_beatmapset(beatmapset_id)))
 
-    def get_beatmapset_discussion_posts(self, beatmapset_discussion_id: Optional[int] = None,
-                                        limit: Optional[int] = None, page: Optional[int] = None,
-                                        sort: Optional[str] = None, user: Optional[int] = None,
-                                        with_deleted: Optional[str] = None) -> dict:
+    def get_beatmapset_discussion_posts(
+        self,
+        beatmapset_discussion_id: Optional[int] = None,
+        limit: Optional[int] = None,
+        page: Optional[int] = None,
+        sort: Optional[str] = None,
+        types: Optional[Sequence[str]] = None,
+        user: Optional[int] = None,
+        with_deleted: Optional[str] = None,
+        cursor: Optional[Dict[str, int]] = None,
+    ) -> BeatmapsetDiscussionPostsResult:
         """
         Returns the posts of the beatmapset discussions
 
         Requires OAuth and scope public
 
         **Parameters**
 
@@ -368,52 +464,68 @@
         limit: Optional[:class:`int`]
             Maximum number of results
 
         page: Optional[:class:`int`]
             Search results page.
 
         sort: Optional[:class:`str`]
-            id_desc for newest first; id_asc for oldest first. Defaults to id_desc
+            `id_desc` for newest first; `id_asc` for oldest first. Defaults to `id_desc`
+
+        type: Optional[Sequence[:class:`str`]]
+            `first`, `reply`, `system` are the valid values. Defaults to `reply`.
 
         user: Optional[:class:`int`]
-            The id of the User
+            The id of the user
 
         with_deleted: Optional[:class:`str`]
-            The param has no effect as api calls do not currently receive group permissions
-
-        **Returns**
-
-        :class:`dict`
-            {
-            beatmapsets: :class:`BeatmapsetCompact`,
-
-            cursor: :class:`dict`,
+            This param has no effect as api calls do not currently receive group permissions.
 
-            posts: Sequence[:class:`BeatmapsetDiscussionPost`],
+        cursor: Optional[Dict[:class:`str`, :class:`int`]]
+            A cursor object received from a previous call to get_beatmapset_discussion_posts
+            (:class:`BeatmapsetDiscussionPostsResult`.cursor)
 
-            users: :class:`UserCompact`
-            }
-        """
-        # TODO: Change is supposed to occur on the response given back from the server,
-        #  make sure to change it when that happens.
-        resp = self.http.make_request(Path.beatmapset_discussion_posts(),
-                                      beatmapset_discussion_id=beatmapset_discussion_id,
-                                      limit=limit, page=page, sort=sort, user=user, with_deleted=with_deleted)
-        return {
-            'beatmapsets': list(map(BeatmapsetCompact, resp['beatmapsets'])),
-            'cursor': resp['cursor'],
-            'posts': list(map(BeatmapsetDiscussionPost, resp['posts'])),
-            'users': list(map(UserCompact, resp['users']))
-        }
+        **Returns**
 
-    def get_beatmapset_discussion_votes(self, beatmapset_discussion_id: Optional[int] = None,
-                                        limit: Optional[int] = None, page: Optional[int] = None,
-                                        receiver: Optional[int] = None, score: Optional[int] = None,
-                                        sort: Optional[str] = None, user: Optional[int] = None,
-                                        with_deleted: Optional[str] = None) -> dict:
+        :class:`BeatmapsetDiscussionsPostsResult`
+        """
+        if cursor is None:
+            cursor = {}
+        if "page" in cursor:
+            page = cursor["page"]
+        if "limit" in cursor:
+            limit = cursor["limit"]
+        resp = self.http.make_request(
+            Path.beatmapset_discussion_posts(),
+            beatmapset_discussion_id=beatmapset_discussion_id,
+            limit=limit,
+            page=page,
+            sort=sort,
+            user=user,
+            with_deleted=with_deleted,
+            **{"types[]": types},
+        )
+        return BeatmapsetDiscussionPostsResult(
+            list(map(BeatmapsetCompact, resp["beatmapsets"])),
+            list(map(BeatmapsetDiscussionPost, resp["posts"])),
+            list(map(UserCompact, resp["users"])),
+            resp["cursor_string"],
+        )
+
+    def get_beatmapset_discussion_votes(
+        self,
+        beatmapset_discussion_id: Optional[int] = None,
+        limit: Optional[int] = None,
+        page: Optional[int] = None,
+        receiver: Optional[int] = None,
+        score: Optional[int] = None,
+        sort: Optional[str] = None,
+        user: Optional[int] = None,
+        with_deleted: Optional[str] = None,
+        cursor: Optional[Dict[str, int]] = None,
+    ) -> BeatmapsetDiscussionVotesResult:
         """
         Returns the votes given to beatmapset discussions
 
         Requires OAuth and scope public
 
         **Parameters**
 
@@ -429,130 +541,144 @@
         receiver: Optional[:class:`int`]
             The id of the User receiving the votes.
 
         score: Optional[:class:`int`]
             1 for upvote, -1 for downvote
 
         sort: Optional[:class:`str`]
-            id_desc for newest first; id_asc for oldest first. Defaults to id_desc
+            `id_desc` for newest first; `id_asc` for oldest first. Defaults to `id_desc`
 
         user: Optional[:class:`int`]
             The id of the User giving the votes.
 
         with_deleted: Optional[:class:`str`]
-            The param has no effect as api calls do not currently receive group permissions
+            This param has no effect as api calls do not currently receive group permissions
 
-        **Returns**
-
-        :class:`dict`
-            {
-            cursor: :class:`dict`,
-
-            discussions: Sequence[:class:`BeatmapsetDiscussion`],
-
-            users: Sequence[:class:`UserCompact`],
+        cursor: Optional[Dict[:class:`str`, :class:`int`]]
+            A cursor object received from a previous call to get_beatmapset_discussion_votes
+            (:class:`BeatmapsetDiscussionVotesResult`.cursor)
 
-            votes: Sequence[:class:`BeatmapsetDiscussionVote`]
-            }
-        """
-        # TODO: Change is supposed to occur on the response given back from the server,
-        #  make sure to change it when that happens.
-        resp = self.http.make_request(Path.beatmapset_discussion_votes(),
-                                      beatmapset_discussion_id=beatmapset_discussion_id,
-                                      limit=limit, receiver=receiver, score=score, page=page,
-                                      sort=sort, user=user, with_deleted=with_deleted)
-        return {
-            'cursor': resp['cursor'],
-            'discussions': list(map(BeatmapsetDiscussion, resp['discussions'])),
-            'users': list(map(UserCompact, resp['users'])),
-            'votes': list(map(BeatmapsetDiscussionVote, resp['votes']))
-        }
+        **Returns**
 
-    def get_beatmapset_discussions(self, beatmap_id: Optional[int] = None, beatmapset_id: Optional[int] = None,
-                                   beatmapset_status: Optional[str] = None, limit: Optional[int] = None,
-                                   message_types: Optional[Sequence[str]] = None,
-                                   only_unresolved: Optional[bool] = None, page: Optional[int] = None,
-                                   sort: Optional[str] = None, user: Optional[int] = None,
-                                   with_deleted: Optional[str] = None) -> dict:
+        :class:`BeatmapsetDiscussionVotesResult`
+        """
+        if cursor is None:
+            cursor = {}
+        if "page" in cursor:
+            page = cursor["page"]
+        if "limit" in cursor:
+            limit = cursor["limit"]
+        resp = self.http.make_request(
+            Path.beatmapset_discussion_votes(),
+            beatmapset_discussion_id=beatmapset_discussion_id,
+            limit=limit,
+            receiver=receiver,
+            score=score,
+            page=page,
+            sort=sort,
+            user=user,
+            with_deleted=with_deleted,
+        )
+        return BeatmapsetDiscussionVotesResult(
+            list(map(BeatmapsetDiscussion, resp["discussions"])),
+            list(map(BeatmapsetDiscussionVote, resp["votes"])),
+            list(map(UserCompact, resp["users"])),
+            resp["cursor"],
+        )
+
+    def get_beatmapset_discussions(
+        self,
+        beatmap_id: Optional[int] = None,
+        beatmapset_id: Optional[int] = None,
+        beatmapset_status: Optional[str] = None,
+        limit: Optional[int] = None,
+        message_types: Optional[Sequence[Union[str, MessageType]]] = None,
+        only_unresolved: Optional[bool] = None,
+        page: Optional[int] = None,
+        sort: Optional[str] = None,
+        user: Optional[int] = None,
+        with_deleted: Optional[str] = None,
+        cursor: Optional[Dict[str, int]] = None,
+    ) -> BeatmapsetDiscussionsResult:
         """
         Returns a list of beatmapset discussions
 
         Requires OAuth and scope public
 
         **Parameters**
 
         beatmap_id: Optional[:class:`int`]
-            id of the Beatmap
+            id of the beatmap
 
         beatmapset_id: Optional[:class:`int`]
-            id of the Beatmapset
+            id of the beatmapset
 
         beatmapset_status: Optional[:class:`str`]
-            One of all, ranked, qualified, disqualified, never_qualified. Defaults to all.
+            One of `all`, `ranked`, `qualified`, `disqualified`, `never_qualified`. Defaults to `all`.
 
         limit: Optional[:class:`int`]
             Maximum number of results.
 
-        message_types: Optional[Sequence[:class:`str`]]
-            suggestion, problem, mapper_note, praise, hype, review. Blank defaults to all types.
+        message_types: Optional[Sequence[Union[:class:`str`, :class:`MessageType`]]]
+            None defaults to all types.
 
         only_unresolved: Optional[:class:`bool`]
             true to show only unresolved issues; false, otherwise. Defaults to false.
 
         page: Optional[:class:`int`]
             Search result page.
 
         sort: Optional[:class:`str`]
-            id_desc for newest first; id_asc for oldest first. Defaults to id_desc.
+            `id_desc` for newest first; `id_asc` for oldest first. Defaults to `id_desc`.
 
         user: Optional[:class:`int`]
             The id of the User.
 
         with_deleted: Optional[:class:`str`]
             This param has no effect as api calls do not currently receive group permissions.
 
-        **Returns**
-
-        :class:`dict`
-            {
-
-            beatmaps: Sequence[:class:`Beatmap`],
-                List of beatmaps associated with the discussions returned.
-
-            cursor: :class:`dict`,
+        cursor: Optional[Dict[:class:`str`, :class:`int`]]
+            A cursor object received from a previous call to get_beatmapset_discussions
+            (:class:`BeatmapsetDiscussionsResult`.cursor)
 
-            discussions: Sequence[:class:`BeatmapsetDiscussion`],
-                List of discussions according to sort order.
-
-            included_discussions: Sequence[:class:`BeatmapsetDiscussion`],
-                Additional discussions related to discussions.
-
-            reviews_config.max_blocks: :class:`int`,
-                Maximum number of blocks allowed in a review.
-
-            users: Sequence[:class:`UserCompact`]
-                List of users associated with the discussions returned.
+        **Returns**
 
-            }
-        """
-        # TODO: Change is supposed to occur on the response given back from the server,
-        #  make sure to change it when that happens.
-        message_types = {"message_types[]": message_types}
-        resp = self.http.make_request(Path.beatmapset_discussions(), beatmap_id=beatmap_id,
-                                      beatmapset_id=beatmapset_id, beatmapset_status=beatmapset_status,
-                                      limit=limit, only_unresolved=only_unresolved, page=page, sort=sort,
-                                      user=user, with_deleted=with_deleted, **message_types)
-        return {
-            'beatmaps': list(map(Beatmap, resp['beatmaps'])),
-            'cursor': resp['cursor'],
-            'discussions': list(map(BeatmapsetDiscussion, resp['discussions'])),
-            'included_discussions': list(map(BeatmapsetDiscussion, resp['included_discussions'])),
-            'reviews_config.max_blocks': resp['reviews_config'],
-            'users': list(map(UserCompact, resp['users']))
-        }
+        :class:`BeatmapsetDiscussionsResult`
+        """
+        if cursor is None:
+            cursor = {}
+        if "page" in cursor:
+            page = cursor["page"]
+        if "limit" in cursor:
+            limit = cursor["limit"]
+        params = {}
+        if message_types is not None:
+            message_types = list(map(lambda t: t.value if isinstance(t, MessageType) else t, message_types))
+            params = {"message_types[]": message_types}
+        resp = self.http.make_request(
+            Path.beatmapset_discussions(),
+            beatmap_id=beatmap_id,
+            beatmapset_id=beatmapset_id,
+            beatmapset_status=beatmapset_status,
+            limit=limit,
+            only_unresolved=only_unresolved,
+            page=page,
+            sort=sort,
+            user=user,
+            with_deleted=with_deleted,
+            **params,
+        )
+        return BeatmapsetDiscussionsResult(
+            list(map(Beatmap, resp["beatmaps"])),
+            list(map(BeatmapsetDiscussion, resp["discussions"])),
+            list(map(BeatmapsetDiscussion, resp["included_discussions"])),
+            list(map(UserCompact, resp["users"])),
+            ReviewsConfig(resp["reviews_config"]),
+            resp["cursor"],
+        )
 
     def get_changelog_build(self, stream: str, build: str) -> Build:
         """
         Returns details of the specified build.
 
         **Parameters**
 
@@ -560,127 +686,126 @@
             Update stream name.
 
         build: :class:`str`
             Build version.
 
         **Returns**
 
-        A :class:`Build` with changelog_entries, changelog_entries.github_user, and versions included.
+        A :class:`Build` with `changelog_entries`, `changelog_entries.github_user`, and `versions` included.
         """
         return Build(self.http.make_request(Path.get_changelog_build(stream, build)))
 
-    def get_changelog_listing(self, from_version: Optional[str] = None, max_id: Optional[int] = None,
-                              stream: Optional[str] = None, to: Optional[str] = None,
-                              message_formats: Optional[Sequence[str]] = None) -> \
-            Dict[str, Union[Sequence[Build], Sequence[UpdateStream], Dict[str, Union[str, int, None]]]]:
+    def get_changelog_listing(
+        self,
+        start: Optional[str] = None,
+        max_id: Optional[int] = None,
+        stream: Optional[str] = None,
+        end: Optional[str] = None,
+        message_formats: Optional[Sequence[str]] = None,
+    ) -> ChangelogListingResult:
         """
         Returns a listing of update streams, builds, and changelog entries.
 
         **Parameters**
 
-        from_version: Optional[:class:`str`]
+        start: Optional[:class:`str`]
             Minimum build version.
 
         max_id: Optional[:class:`int`]
             Maximum build ID.
 
         stream: Optional[:class:`str`]
             Stream name to return builds from.
 
-        to: Optional[:class:`str`]
+        end: Optional[:class:`str`]
             Maximum build version.
 
         message_formats: Optional[Sequence[:class:`str`]]
-            html, markdown. Default to both.
+            `html`, `markdown`. Default to both.
 
         **Returns**
 
-        {
-
-        "build": Sequence[:class:`Build`]
-
-        "search": {
-
-            "from": :class:`str`
-                from_version input.
-
-            "limit": :class:`int`
-                Always 21.
-
-            "max_id": :class:`int`
-                max_id input.
-
-            "stream": :class:`str`
-                stream input.
-
-            "to": :class:`str`
-                to input.
-
-        }
-
-        "streams": Sequence[:class:`UpdateStream`]
-
-        }
+        :class:`ChangelogListingResult`
         """
-        response = self.http.make_request(Path.get_changelog_listing(), max_id=max_id,
-                                          stream=stream, to=to, message_formats=message_formats,
-                                          **{"from": from_version})
-        return {
-            "build": list(map(Build, response['builds'])),
-            "search": response['search'],
-            "streams": list(map(UpdateStream, response['streams'])),
-        }
-
-    def lookup_changelog_build(self, changelog: str, key: Optional[str] = None,
-                               message_formats: Optional[Sequence[str]] = None) -> Build:
+        response = self.http.make_request(
+            Path.get_changelog_listing(),
+            max_id=max_id,
+            stream=stream,
+            to=end,
+            **{"from": start, "message_formats[]": message_formats},
+        )
+        return ChangelogListingResult(
+            list(map(Build, response["builds"])),
+            list(map(UpdateStream, response["streams"])),
+            ChangelogListingSearch(
+                response["search"]["from"],
+                response["search"]["to"],
+                response["search"]["limit"],
+                response["search"]["max_id"],
+                response["search"]["stream"],
+            ),
+        )
+
+    def lookup_changelog_build(
+        self,
+        changelog: str,
+        key: Optional[str] = None,
+        message_formats: Optional[Sequence[str]] = None,
+    ) -> Build:
         """
         Returns details of the specified build.
 
         **Parameters**
 
         changelog: :class:`str`
             Build version, update stream name, or build ID.
 
         key: Optional[:class:`str`]
-            Unset to query by build version or stream name, or id to query by build ID.
+            Leave blank to query by build version or stream name, or `id` to query by build ID.
 
         message_formats: Optional[Sequence[:class:`str`]]
-            html, markdown. Default to both.
+            `html`, `markdown`. Default to both.
 
         **Returns**
 
         A :class:`Build` with changelog_entries, changelog_entries.github_user, and versions included.
         """
-        return Build(self.http.make_request(Path.lookup_changelog_build(changelog),
-                                            key=key, message_formats=message_formats))
-
-    def chat_acknowledge(self, history_since: Optional[int] = None, since: Optional[int] = None) -> \
-            Sequence[UserSilence]:
+        return Build(
+            self.http.make_request(
+                Path.lookup_changelog_build(changelog), key=key, **{"message_formats[]": message_formats}
+            )
+        )
+
+    def chat_acknowledge(
+        self, history_since: Optional[int] = None, since: Optional[int] = None
+    ) -> Sequence[UserSilence]:
         """
         Send a chat ack.
 
         Requires OAuth, scope lazer, and a user (authorization code grant, delegate scope, or password auth)
 
         **Parameters**
 
-        history_since: Optional[:class:`int]
-            :class:`UserSilence`s after the specified id to return.
+        history_since: Optional[:class:`int`]
+            :class:`UserSilence` s after the specified id to return.
             This field is preferred and takes precedence over since.
 
         since: Optional[:class:`int`]
-            :class:`UserSilence`s after the specified :class:`ChatMessage`.message_id to return.
+            :class:`UserSilence` s after the specified :class:`ChatMessage`.message_id to return.
 
         **Returns**
 
-        Sequence[:class:`UserSilence`]
+        List[:class:`UserSilence`]
         """
         resp = self.http.make_request(Path.chat_ack(), history_since=history_since, since=since)
         return list(map(UserSilence, resp["silences"]))
 
-    def create_new_pm(self, target_id: int, message: str, is_action: bool, uuid: Optional[str] = None) -> dict:
+    def create_new_pm(
+        self, target_id: int, message: str, is_action: bool, uuid: Optional[str] = None
+    ) -> CreateNewPmResult:
         """
         This endpoint allows you to create a new PM channel.
 
         Requires OAuth, scope chat.write, and a user (authorization code grant, delegate scope, or password auth)
 
         **Parameters**
 
@@ -694,82 +819,78 @@
             whether the message is an action
 
         uuid: Optional[:class:`str`]
             client-side message identifier which will be sent back in response and websocket json.
 
         **Returns**
 
-        :class:`dict`
-            {
-
-            channel: :class:`ChatChannel`
-                channel the message was sent in
-
-            message: :class:`ChatMessage`
-                the sent message
-
-            new_channel_id: :class:`int`
-                channel_id of newly created channel
-
-            }
+        :class:`CreateNewPmResult`
         """
-        data = {'target_id': target_id, 'message': message, 'is_action': is_action}
+        data = {"target_id": target_id, "message": message, "is_action": is_action}
         if uuid is not None:
-            data['uuid'] = uuid
+            data["uuid"] = uuid
         resp = self.http.make_request(Path.create_new_pm(), files=create_multipart_formdata(data))
-        return {
-            'channel': ChatChannel(resp['channel']),
-            'message': ChatMessage(resp['message']),
-            'new_channel_id': resp['new_channel_id'],
-        }
-
-    def get_updates(self, since: int, includes: Optional[Sequence[str]] = None,
-                    history_since: Optional[int] = None) -> dict:
+        return CreateNewPmResult(
+            ChatChannel(resp["channel"]),
+            ChatMessage(resp["message"]),
+            resp["new_channel_id"],
+        )
+
+    def get_updates(
+        self,
+        since: int = 0,
+        includes: Optional[Sequence[str]] = None,
+        history_since: Optional[int] = None,
+    ) -> GetUpdatesResult:
         """
         This endpoint returns new messages since the given message_id along with updated channel 'presence' data.
 
         Requires OAuth, scope lazer, a user (authorization code grant, delegate scope, or password auth)
 
         **Parameters**
 
         since: :class:`int`
-            Messages after the specified message_id to return.
+            Defaults to 0. :class:`UserSilence`s after the specified `ChatMessage.message_id` to return.
 
         includes: Optional[Sequence[:class:`str`]]
-            List of fields from presence, silences to include in the response. Returns presence if not specified.
-            Specifying silences may cause the api to return blank content for both presence and silences.
+            List of fields from `presence`, `silences` to include in the response. Uses `presences` if not specified.
 
         history_since: Optional[:class:`int`]
             :class:`UserSilence`s after the specified id to return.
+            This field is preferred and takes precedence over `since`.
 
         **Returns**
 
-        :class:`dict`
-            {
-            presence: List[:class:`ChatChannel`],
-
-            silences: List[:class:`UserSilence`]
-
-            }
+        :class:`GetUpdatesResult`
         """
         if includes is None:
             includes = ["presence"]
-        resp = self.http.make_request(Path.get_updates(), since=since, history_since=history_since,
-                                      **{"includes[]": ",".join(includes)})
+        resp = self.http.make_request(
+            Path.get_updates(),
+            since=since,
+            history_since=history_since,
+            **{"includes[]": includes},
+        )
         if resp is None:
             resp = {}
-        return {
-            'presence': list(map(ChatChannel, resp['presence'])) if 'presence' in resp else None,
-            'silences': list(map(UserSilence, resp['silences'])) if 'silences' in resp else None
-        }
-
-    def get_channel_messages(self, channel_id: int, limit: Optional[int] = None, since: Optional[int] = None,
-                             until: Optional[int] = None) -> Sequence[ChatMessage]:
+        return GetUpdatesResult(
+            get_optional_list(resp, "presence", ChatChannel),
+            get_optional_list(resp, "silences", UserSilence),
+        )
+
+    def get_channel_messages(
+        self,
+        channel_id: int,
+        limit: Optional[int] = None,
+        since: Optional[int] = None,
+        until: Optional[int] = None,
+    ) -> List[ChatMessage]:
         """
         This endpoint returns the chat messages for a specific channel.
+        You may need to first join the channel with :func:`osu.Client.join_channel`.
 
         Requires OAuth, scope lazer, and a user (authorization code grant, delegate scope, or password auth)
 
         **Parameter**
 
         channel_id: :class:`int`
             The ID of the channel to retrieve messages for
@@ -781,22 +902,29 @@
             messages after the specified message id will be returned
 
         until: Optional[:class:`int`]
             messages up to but not including the specified message id will be returned
 
         **Returns**
 
-        Sequence[:class:`ChatMessage`]
-            list containing :class:`ChatMessage` objects
+        List[:class:`ChatMessage`]
         """
-        return list(map(ChatMessage, self.http.make_request(Path.get_channel_messages(channel_id),
-                                                            limit=limit, since=since, until=until)))
+        return list(
+            map(
+                ChatMessage,
+                self.http.make_request(
+                    Path.get_channel_messages(channel_id),
+                    limit=limit,
+                    since=since,
+                    until=until,
+                ),
+            )
+        )
 
-    def send_message_to_channel(self, channel_id: int, message: str, is_action: bool,
-                                uuid: Optional[str] = None) -> ChatMessage:
+    def send_message_to_channel(self, channel_id: int, message: str, is_action: bool) -> ChatMessage:
         """
         This endpoint sends a message to the specified channel.
 
         Requires OAuth, scope lazer, and a user (authorization code grant, delegate scope, or password auth)
 
         **Parameters**
 
@@ -805,63 +933,59 @@
 
         message: :class:`str`
             message to send
 
         is_action: :class:`bool`
             whether the message is an action
 
-        uuid: Optional[:class:`str`]
-
         **Returns**
 
         :class:`ChatMessage`
         """
-        data = {'is_action': str(is_action).lower(), 'message': message}
-        if uuid is not None:
-            data["uuid"] = uuid
+        data = {"is_action": str(is_action).lower(), "message": message}
         data = create_multipart_formdata(data)
         return ChatMessage(self.http.make_request(Path.send_message_to_channel(channel_id), files=data))
 
-    def join_channel(self, channel: str, user: str) -> ChatChannel:
+    def join_channel(self, channel: int, user: int) -> ChatChannel:
         """
-        This endpoint allows you to join a public channel.
+        This endpoint allows you (or someone else) to join a public channel.
 
         Requires OAuth, scope lazer, and a user (authorization code grant, delegate scope, or password auth)
 
         **Parameters**
 
-        channel: :class:`str`
+        channel: :class:`int`
             channel id of channel to join
 
-        user: :class:`str`
-            user joining (you)
+        user: :class:`int`
+            user id of user joining
 
         **Returns**
 
         :class:`ChatChannel`
         """
         return ChatChannel(self.http.make_request(Path.join_channel(channel, user)))
 
-    def leave_channel(self, channel: str, user: str):
+    def leave_channel(self, channel: int, user: int) -> None:
         """
-        This endpoint allows you to leave a public channel.
+        This endpoint allows you (or someone else) to leave a public channel.
 
         Requires OAuth, scope lazer, and a user (authorization code grant, delegate scope, or password auth)
 
         **Parameters**
 
-        channel: :class:`str`
+        channel: :class:`int`
             channel id of channel to leave
 
-        user: :class:`str`
-            user leaving (you)
+        user: :class:`int`
+            user id of user leaving
         """
         self.http.make_request(Path.leave_channel(channel, user))
 
-    def mark_channel_as_read(self, channel_id: int, message_id: int):
+    def mark_channel_as_read(self, channel_id: int, message_id: int) -> None:
         """
         This endpoint marks the channel as having being read up to the given message_id.
 
         Requires OAuth, scope lazer, and a user (authorization code grant, delegate scope, or password auth)
 
         **Parameters**
 
@@ -869,47 +993,52 @@
             The channel_id of the channel to mark as read
 
         message_id: :class:`int`
             The message_id of the message to mark as read up to
         """
         self.http.make_request(Path.mark_channel_as_read(channel_id, message_id))
 
-    def get_channel_list(self) -> Sequence[ChatChannel]:
+    def get_channel_list(self) -> List[ChatChannel]:
         """
         This endpoint returns a list of all joinable public channels.
 
         Requires OAuth, scope lazer, and a user (authorization code grant, delegate scope, or password auth)
 
         **Returns**
 
         Sequence[:class:`ChatChannel`]
         """
         return list(map(ChatChannel, self.http.make_request(Path.get_channel_list())))
 
-    def create_channel(self, channel_type: Union[ChatChannelType, str], target_id: Optional[int] = None,
-                       target_ids: Optional[Sequence[int]] = None, message: Optional[str] = None,
-                       channel: Optional[Dict[str, str]] = None) -> ChatChannel:
+    def create_channel(
+        self,
+        channel_type: Union[ChatChannelType, str],
+        target_id: Optional[int] = None,
+        target_ids: Optional[Sequence[int]] = None,
+        message: Optional[str] = None,
+        channel: Optional[Dict[str, str]] = None,
+    ) -> ChatChannel:
         """
         [This description may be outdated]
 
         This endpoint creates a new channel if doesn't exist and joins it.
         Currently only for rejoining existing PM channels which the user has left.
 
         Requires OAuth, scope lazer, and a user (authorization code grant, delegate scope, or password auth)
 
         **Parameter**
 
         channel_type: Union[:class:`ChatChannelType`, :class:`str`]
-            channel type (currently only supports "PM" and "ANNOUNCE")
+            channel type (currently only supports `PM` and `ANNOUNCE`)
 
         target_id: Optional[:class:`int`]
             target user id; required if type is PM; ignored, otherwise.
 
         target_ids: Optional[Sequence[:class:`int`]]
-            target user ids; required if type is PM; ignored, otherwise.
+            target user ids; required if type is ANNOUNCE; ignored, otherwise.
 
         message: Optional[:class:`str`]
             message to send with the announcement; required if type is ANNOUNCE.
 
         channel: Optional[Dict[str, str]]
             channel details; required if type is ANNOUNCE.
 
@@ -918,66 +1047,57 @@
 
             description: :class:`str`
                 the channel description
 
         **Returns**
 
         :class:`ChatChannel`
-             contains recent_messages attribute. Note that if there's no existing PM channel,
-             most of the fields will be blank. In that case, send a message (create_new_pm)
-             instead to create the channel.
+             contains recent_messages attribute (which is deprecated).
         """
         channel_type = parse_enum_args(channel_type)
         if channel_type == "PM":
-            if target_id is None and target_ids is None:
-                raise ValueError("target_id and target_ids cannot both be null if the channel type is PM")
-            data = {"type": channel_type,
-                    **({"target_ids": target_ids} if target_ids is not None else {"target_id": target_id})}
+            data = {"type": "PM", "target_id": target_id}
         elif channel_type == "ANNOUNCE":
-            if message is None:
-                raise ValueError("message cannot be null when the channel type is ANNOUNCE")
-            elif channel is None or channel["name"] is None or channel["description"] is None:
-                raise ValueError("channel and it's items cannot be null when the channel type is ANNOUNCEMENT")
-            data = {"type": channel_type, "message": message, "channel": channel}
+            data = {
+                "type": channel_type,
+                "message": message,
+                "channel": json.dumps(channel),
+                "target_ids": json.dumps(target_ids),
+            }
         else:
-            raise ValueError(f"{channel_type} is not a valid channel type that can be created. "
-                             f"Check for casing (uppercase) if the type is correct.")
-        return ChatChannel(self.http.make_request(Path.create_channel(), data=data))
+            raise ValueError(
+                f"{channel_type} is not a valid channel type that can be created. " f"Check for casing (uppercase)."
+            )
+        return ChatChannel(self.http.make_request(Path.create_channel(), files=create_multipart_formdata(data)))
 
-    def get_channel(self, channel_id: int) -> dict:
+    def get_channel(self, channel_id: int) -> GetChannelResult:
         """
         Gets details of a chat channel.
 
         Requires OAuth, scope lazer, and a user (authorization code grant, delegate scope, or password auth)
 
         **Parameter**
 
         channel_id: :class:`int`
 
         **Returns**
 
-        :class:`dict`
-            {
-            channel: :class:`ChatChannel`,
-
-            users: :class:`UserCompact`
-                Only visible for PM channels
-
-            }
+        :class:`GetChannelResult`
         """
         resp = self.http.make_request(Path.get_channel(channel_id))
-        return {
-            'channel': ChatChannel(resp['channel']),
-            'users': list(map(UserCompact, resp['users'])),
-        }
+        return GetChannelResult(ChatChannel(resp["channel"]), list(map(UserCompact, resp["users"])))
 
-    def get_comments(self, commentable_type: Optional[Union[ObjectType, str]] = None,
-                     commentable_id: Optional[int] = None, cursor: Optional[dict] = None,
-                     parent_id: Optional[int] = None,
-                     sort: Optional[Union[str, CommentSort]] = None) -> CommentBundle:
+    def get_comments(
+        self,
+        commentable_type: Optional[Union[ObjectType, str]] = None,
+        commentable_id: Optional[int] = None,
+        cursor: Optional[dict] = None,
+        parent_id: Optional[int] = None,
+        sort: Optional[Union[str, CommentSort]] = None,
+    ) -> CommentBundle:
         """
         Returns a list comments and their replies up to 2 levels deep.
 
         Does not require OAuth
 
         **Parameter**
 
@@ -1001,23 +1121,38 @@
 
         **Returns**
 
         :class:`CommentBundle`
             pinned_comments is only included when commentable_type and commentable_id are specified.
         """
         commentable_type, sort = parse_enum_args(commentable_type, sort)
-        if commentable_type is not None and commentable_type not in ("beatmapset", "build", "news_post"):
+        if commentable_type is not None and commentable_type not in (
+            "beatmapset",
+            "build",
+            "news_post",
+        ):
             raise ValueError("commentable_type, if not null, must be of the following: beatmapset, build, new_post")
-        return CommentBundle(self.http.make_request(Path.get_comments(), commentable_type=commentable_type,
-                                                    commentable_id=commentable_id, **(cursor if cursor else {}),
-                                                    parent_id=parent_id, sort=sort))
-
-    def post_comment(self, commentable_type: Optional[Union[ObjectType, str]] = None,
-                     commentable_id: Optional[int] = None, message: Optional[str] = None,
-                     parent_id: Optional[int] = None) -> CommentBundle:
+        return CommentBundle(
+            self.http.make_request(
+                Path.get_comments(),
+                commentable_type=commentable_type,
+                commentable_id=commentable_id,
+                parent_id=parent_id,
+                sort=sort,
+                **(cursor if cursor else {}),
+            )
+        )
+
+    def post_comment(
+        self,
+        commentable_type: Optional[Union[ObjectType, str]] = None,
+        commentable_id: Optional[int] = None,
+        message: Optional[str] = None,
+        parent_id: Optional[int] = None,
+    ) -> CommentBundle:
         """
         Posts a new comment to a comment thread.
 
         Requires OAuth, scope lazer, and a user (authorization code grant, delegate scope, or password auth)
 
         **Parameter**
 
@@ -1034,21 +1169,21 @@
         parent_id: Optional[:class:`int`]
             The id of the comment to reply to, null if not a reply
 
         **Returns**
 
         :class:`CommentBundle`
         """
-        params = {
+        data = {
             "comment[commentable_type]": parse_enum_args(commentable_type),
             "comment[commentable_id]": commentable_id,
             "comment[message]": message,
-            "comment[parent_id]": parent_id
+            "comment[parent_id]": parent_id,
         }
-        return CommentBundle(self.http.make_request(Path.post_new_comment(), **params))
+        return CommentBundle(self.http.make_request(Path.post_new_comment(), files=create_multipart_formdata(data)))
 
     def get_comment(self, comment: int) -> CommentBundle:
         """
         Gets a comment and its replies up to 2 levels deep.
 
         Does not require OAuth
 
@@ -1077,16 +1212,19 @@
         message: Optional[:class:`str`]
             New text of the comment
 
         **Returns**
 
         :class:`CommentBundle`
         """
-        return CommentBundle(self.http.make_request(Path.edit_comment(comment),
-                                                    **{"comment[message]": message}))
+        return CommentBundle(
+            self.http.make_request(
+                Path.edit_comment(comment), files=create_multipart_formdata({"comment[message]": message})
+            )
+        )
 
     def delete_comment(self, comment: int) -> CommentBundle:
         """
         Deletes the specified comment.
 
         Requires OAuth, scope lazer, and a user (authorization code grant, delegate scope, or password auth)
 
@@ -1150,21 +1288,30 @@
             Content of the reply post.
 
         **Returns**
 
         :class:`ForumPost`
             body attributes included
         """
-        data = {'body': body}
-        return ForumPost(self.http.make_request(Path.reply_topic(topic), data=data))
+        data = {"body": body}
+        return ForumPost(self.http.make_request(Path.reply_topic(topic), files=create_multipart_formdata(data)))
 
-    def create_topic(self, body: str, forum_id: int, title: str, with_poll: Optional[bool] = None,
-                     hide_results: Optional[bool] = None, length_days: Optional[int] = None,
-                     max_options: Optional[int] = None, poll_options: Optional[str] = None,
-                     poll_title: Optional[str] = None, vote_change: Optional[bool] = None) -> dict:
+    def create_topic(
+        self,
+        body: str,
+        forum_id: int,
+        title: str,
+        with_poll: Optional[bool] = None,
+        hide_results: Optional[bool] = None,
+        length_days: Optional[int] = None,
+        max_options: Optional[int] = None,
+        poll_options: Optional[str] = None,
+        poll_title: Optional[str] = None,
+        vote_change: Optional[bool] = None,
+    ) -> CreateTopicResult:
         """
         Create a new topic.
 
         Requires OAuth, scope forum.write, and a user (authorization code grant, delegate scope, or password auth)
 
         **Parameters**
 
@@ -1197,90 +1344,92 @@
             Title of the poll.
 
         vote_change: Optional[:class:`bool`]
             Enable this to allow user to change their votes (default: false).
 
         **Returns**
 
-        :class:`dict`
-            {
-            topic: :class:`ForumTopic`
-
-            post: :class:`ForumPost`
-                includes body
-
-            }
+        :class:`CreateTopicResult`
         """
-        data = {'body': body, 'forum_id': forum_id, 'title': title, 'with_poll': with_poll}
+        data = {
+            "body": body,
+            "forum_id": forum_id,
+            "title": title,
+            "with_poll": with_poll,
+        }
         if with_poll:
             if poll_options is None or poll_title is None:
                 raise TypeError("poll_options and poll_title are required since the topic has a poll.")
-            data.update({'forum_topic_poll': {
-                'hide_results': hide_results, 'length_days': length_days,
-                'max_options': max_options, 'poll_options': poll_options,
-                'poll_title': poll_title, 'vote_change': vote_change
-            }})
-        resp = self.http.make_request(Path.create_topic(), data=json.dumps(data))
-        return {
-            'topic': ForumTopic(resp['topic']),
-            'post': ForumPost(resp['post'])
-        }
-
-    def get_topic_and_posts(self, topic: int, cursor: Optional[dict] = None, sort: Optional[str] = None,
-                            limit: Optional[int] = None, start: Optional[int] = None,
-                            end: Optional[int] = None) -> dict:
+            data.update(
+                {
+                    "forum_topic_poll[hide_results]": hide_results,
+                    "forum_topic_poll[length_days]": length_days,
+                    "forum_topic_poll[max_options]": max_options,
+                    "forum_topic_poll[poll_options]": poll_options,
+                    "forum_topic_poll[poll_title]": poll_title,
+                    "forum_topic_poll[vote_change]": vote_change,
+                }
+            )
+        resp = self.http.make_request(Path.create_topic(), files=create_multipart_formdata(data))
+        return CreateTopicResult(ForumTopic(resp["topic"]), ForumPost(resp["post"]))
+
+    def get_topic_and_posts(
+        self,
+        topic: int,
+        cursor: Optional[str] = None,
+        sort: Optional[str] = None,
+        limit: Optional[int] = None,
+        start: Optional[int] = None,
+        end: Optional[int] = None,
+    ) -> GetTopicAndPostsResult:
         """
         Get topic and its posts.
 
         Requires OAuth and scope public
 
         **Parameters**
 
         topic: :class:`int`
             Id of the topic.
 
-        cursor: Optional[:class:`dict`]
-            To be used to fetch the next page of results
+        cursor: Optional[:class:`str`]
+            Parameter for pagination.
 
         sort: Optional[:class:`str`]
             Post sorting option. Valid values are id_asc (default) and id_desc.
 
         limit: Optional[:class:`int`]
             Maximum number of posts to be returned (20 default, 50 at most).
 
         start: Optional[:class:`int`]
             First post id to be returned with sort set to id_asc.
-            This parameter is ignored if cursor is specified.
+            This parameter is ignored if cursor_string is specified.
 
         end: Optional[:class:`int`]
             First post id to be returned with sort set to id_desc.
-            This parameter is ignored if cursor is specified.
+            This parameter is ignored if cursor_string is specified.
 
         **Returns**
 
-        :class:`dict`
-            {
-            cursor: :class:`dict`,
-
-            search: :class:`dict`,
-
-            posts: Sequence[:class:`ForumPost`],
-
-            topic: :class:`ForumTopic`
-
-            }
+        :class:`GetTopicAndPostsResult`
         """
-        resp = self.http.make_request(Path.get_topic_and_posts(topic), **(cursor if cursor else {}),
-                                      sort=sort, limit=limit, start=start, end=end)
-        return {
-            'cursor': resp['cursor'],
-            'search': resp['search'],
-            'posts': list(map(ForumPost, resp['posts'])),
-            'topic': ForumTopic(resp['topic'])
-        }
+        resp = self.http.make_request(
+            Path.get_topic_and_posts(topic),
+            **(cursor if cursor else {}),
+            sort=sort,
+            limit=limit,
+            start=start,
+            end=end,
+        )
+        return GetTopicAndPostsResult(
+            resp["cursor_string"],
+            resp["search"],
+            ForumTopic(resp["topic"]),
+            list(map(ForumPost, resp["posts"])),
+        )
 
     def edit_topic(self, topic: int, topic_title: str) -> ForumTopic:
         """
         Edit topic. Only title can be edited through this endpoint.
 
         Requires OAuth and scope forum.write
 
@@ -1292,16 +1441,16 @@
         topic_title: :class:`str`
             New topic title.
 
         **Returns**
 
         :class:`ForumTopic`
         """
-        data = {'forum_topic': {'topic_title': topic_title}}
-        return ForumTopic(self.http.make_request(Path.edit_topic(topic), data=json.dumps(data)))
+        data = {"forum_topic[topic_title]": topic_title}
+        return ForumTopic(self.http.make_request(Path.edit_topic(topic), files=create_multipart_formdata(data)))
 
     def edit_post(self, post: int, body: str) -> ForumPost:
         """
         Edit specified forum post.
 
         Requires OAuth and scope forum.write
 
@@ -1311,19 +1460,23 @@
         body: :class:`str`
             New post content in BBCode format.
 
         **Returns**
 
         :class:`ForumPost`
         """
-        data = {'body': body}
-        return ForumPost(self.http.make_request(Path.edit_post(post), data=data))
+        data = {"body": body}
+        return ForumPost(self.http.make_request(Path.edit_post(post), files=create_multipart_formdata(data)))
 
-    def search(self, mode: Optional[Union[str, WikiSearchMode]] = None, query: Optional[str] = None,
-               page: Optional[int] = None) -> Dict[str, SearchResults]:
+    def search(
+        self,
+        mode: Optional[Union[str, WikiSearchMode]] = None,
+        query: Optional[str] = None,
+        page: Optional[int] = None,
+    ) -> SearchResult:
         """
         Searches users and wiki pages.
 
         Requires OAuth and scope public
 
         **Parameters**
 
@@ -1334,29 +1487,22 @@
             Search keyword.
 
         page: Optional[:class:`int`]
             Search result page. Ignored for mode all.
 
         **Returns**
 
-        Dict[:class:`str`, :class:`SearchResults`]
-            {
-
-            "user": Union[:class:`SearchResults`, :class:`None`]
-
-            "wiki_page": Union[:class:`SearchResults`, :class:`None`]
-
-            }
+        :class:`SearchResult`
         """
         mode = parse_enum_args(mode)
         resp = self.http.make_request(Path.search(), mode=mode, query=query, page=page)
-        return {
-            'user': SearchResults(resp["user"], UserCompact) if 'user' in resp else None,
-            'wiki_page': SearchResults(resp["wiki_page"], WikiPage) if 'wiki_page' in resp else None,
-        }
+        return SearchResult(
+            get_optional_list(resp.get("user", {}), "data", UserCompact),
+            get_optional_list(resp.get("wiki_page", {}), "data", WikiPage),
+        )
 
     def get_user_highscore(self, room: int, playlist: int, user: int) -> MultiplayerScore:
         """
         Requires OAuth, scope lazer, and a user (authorization code grant, delegate scope, or password auth)
 
         **Parameters**
 
@@ -1371,17 +1517,22 @@
 
         **Returns**
 
         :class:`MultiplayerScores`
         """
         return MultiplayerScore(self.http.make_request(Path.get_user_high_score(room, playlist, user)))
 
-    def get_scores(self, room: int, playlist: int, limit: Optional[int] = None,
-                   sort: Optional[Union[str, MultiplayerScoresSort]] = None,
-                   cursor: Optional[dict] = None) -> MultiplayerScores:
+    def get_scores(
+        self,
+        room: int,
+        playlist: int,
+        limit: Optional[int] = None,
+        sort: Optional[Union[str, MultiplayerScoresSort]] = None,
+        cursor: Optional[str] = None,
+    ) -> MultiplayerScores:
         """
         Requires OAuth, scope public, and a user (authorization code grant, delegate scope, or password auth)
 
         **Parameters**
 
         room: :class:`int`
             Id of the room.
@@ -1390,24 +1541,30 @@
             Id of the playlist item.
 
         limit: Optional[:class:`int`]
             Number of scores to be returned.
 
         sort: Optional[Union[:class:`str`, :class:`MultiplayerScoresSort`]]
 
-
-        cursor: Optional[:class:`dict`]
+        cursor: Optional[:class:`str`]
+            :class:`MultiplayerScores`.cursor value from a previous call to get next page.
 
         **Returns**
 
         :class:`MultiplayerScores`
         """
         sort = parse_enum_args(sort)
-        return MultiplayerScores(self.http.make_request(Path.get_scores(room, playlist),
-                                                        limit=limit, sort=sort, **(cursor if cursor else {})))
+        return MultiplayerScores(
+            self.http.make_request(
+                Path.get_scores(room, playlist),
+                limit=limit,
+                sort=sort,
+                cursor_string=cursor,
+            )
+        )
 
     def get_score(self, room: int, playlist: int, score: int) -> MultiplayerScore:
         """
         Requires OAuth, scope lazer, and a user (authorization code grant, delegate scope, or password auth)
 
         **Parameters**
 
@@ -1422,206 +1579,187 @@
 
         **Returns**
 
         :class:`MultiplayerScore`
         """
         return MultiplayerScore(self.http.make_request(Path.get_score(room, playlist, score)))
 
-    def get_news_listing(self, limit: Optional[int] = None, year: Optional[int] = None,
-                         cursor: Optional[dict] = None) -> dict:
+    def get_news_listing(
+        self,
+        limit: Optional[int] = None,
+        year: Optional[int] = None,
+        cursor: Optional[dict] = None,
+    ) -> GetNewsListingResult:
         """
         Returns a list of news posts and related metadata.
 
         **Parameters**
 
         limit: Optional[:class:`int`]
             Maximum number of posts (12 default, 1 minimum, 21 maximum).
 
         year: Optional[:class:`int`]
             Year to return posts from.
 
-        cursor: Optional[:class:`dict`]
+        cursor: Optional[:class:`str`]
             Cursor for pagination.
 
         **Returns**
 
-        {
-
-        cursor: :class:`dict`
-
-        news_posts: Sequence[:class:`NewsPost`]
-            Includes preview.
-
-        news_sidebar: {
-
-            current_year: :class:`int`
-                Year of the first post's publish time, or current year if no posts returned.
-
-            years: :class:`int`
-                All years during which posts have been published.
-
-            news_posts: Sequence[:class:`NewsPost`]
-                All posts published during current_year.
-
-        }
-
-        search: {
-
-            limit: :class:`int`
-                Clamped limit input.
-
-            sort: :class:`str`
-                Always published_desc.
-
-            }
-
-        }
+        :class:`GetNewsListingResult`
         """
-        response = self.http.make_request(Path.get_news_listing(), limit=limit, year=year, cursor=cursor)
-        return {
-            "cursor": response['cursor'],
-            "news_posts": list(map(NewsPost, response["news_posts"])),
-            "news_sidebar": {
-                "current_year": response['news_sidebar']['current_year'],
-                "years": response['news_sidebar']['years'],
-                "news_posts": list(map(NewsPost, response['news_sidebar']['news_posts'])),
-            },
-            "search": response['search']
-        }
+        resp = self.http.make_request(Path.get_news_listing(), limit=limit, year=year, cursor=cursor)
+        return GetNewsListingResult(
+            resp["cursor_string"],
+            list(map(NewsPost, resp["news_posts"])),
+            NewsSidebar(
+                resp["news_sidebar"]["current_year"],
+                list(map(NewsPost, resp["news_sidebar"]["news_posts"])),
+                resp["news_sidebar"]["years"],
+            ),
+            SearchInfo(resp["search"]["sort"], resp["search"]["limit"], None, None),
+        )
 
     def get_news_post(self, news: str, key: Optional[str] = None) -> NewsPost:
         """
         Returns details of the specified news post.
 
         **Parameters**
 
         news: class:`str`
             News post slug or ID.
 
         key: Optional[:class:`str`]
-            Unset to query by slug, or id to query by ID.
+            Unset to query by slug, or `id` to query by ID.
 
         **Returns**
 
         Returns a :class:`NewsPost` with content and navigation included.
         """
         return NewsPost(self.http.make_request(Path.get_news_post(news), key=key))
 
-    def get_notifications(self, max_id: Optional[int] = None) -> dict:
+    def get_notifications(self, max_id: Optional[int] = None) -> GetNotificationsResult:
         """
         This endpoint returns a list of the user's unread notifications. Sorted descending by id with limit of 50.
 
         Requires OAuth, scope lazer, a user (authorization code grant, delegate scope, or password auth)
 
         **Parameters**
 
         max_id: Optional[:class:`int`]
             Maximum id fetched. Can be used to load earlier notifications.
             Defaults to no limit (fetch latest notifications)
 
         **Returns**
 
-        :class:`dict`
-            {
-
-            has_more: :class:`bool`,
-                whether or not there are more notifications
-
-            notifications: Sequence[:class:`Notification`],
-
-            unread_count: :class:`bool`
-                total unread notifications
-
-            notification_endpoint: :class:`str`
-                url to connect to websocket server
-
-            }
+        :class:`GetNotificationsResult`
         """
         resp = self.http.make_request(Path.get_notifications(), max_id=max_id)
-        return {
-            "notifications": list(map(Notification, resp['notifications'])),
-            "stacks": resp["stacks"],
-            "timestamp": resp["timestamp"],
-            "types": resp["types"],
-            "notification_endpoint": resp['notification_endpoint'],
-        }
-
-    def mark_notifications_read(self, identities: Optional[Sequence[Union[
-        IdentitiesUtil, Dict[str, Union[str, int]]]]] = None,
-        notifications: Optional[Sequence[Union[
-            NotificationsUtil, Dict[str, str]]]] = None):
+        return GetNotificationsResult(
+            list(map(Notification, resp["notifications"])),
+            [
+                NotificationStackResult(
+                    NotificationType(category)
+                    if (category := stack["category"]).upper() in NotificationType.__members__
+                    else ObjectType(category),
+                    stack["cursor"],
+                    ObjectType(stack["object_type"]),
+                    stack["object_id"],
+                    stack["total"],
+                )
+                for stack in resp["stacks"]
+            ],
+            parser.parse(resp["timestamp"]),
+            [
+                NotificationTypeResult(t["cursor"], get_optional(t, "name", ObjectType), t["total"])
+                for t in resp["types"]
+            ],
+            resp.get("unread_count"),
+            resp["notification_endpoint"],
+        )
+
+    def mark_notifications_read(
+        self,
+        identities: Optional[Sequence[Union[IdentitiesUtil, Dict[str, Union[str, int]]]]] = None,
+        notifications: Optional[Sequence[Union[NotificationsUtil, Dict[str, str]]]] = None,
+    ) -> None:
         """
         This endpoint allows you to mark notifications read. Should only supply one of the arguments.
 
         Requires OAuth, scope lazer, a user (authorization code grant, delegate scope, or password auth)
 
         **Parameters**
 
-        identities: Sequence[Union[:class:`ReadNotifIdentitiesUtil`,
-        Dict[:class:`str`, Union[:class:`str`, :class:`int`]]]]
+        identities: Optional[Sequence[Union[:class:`IdentitiesUtil`, Dict[:class:`str`, :class:`str`]]]]
 
-        notifications: Sequence[Union[:class:`ReadNotifNotificationsUtil`, Dict[:class:`str`, :class:`str`]]]
+        notifications: Optional[Sequence[Union[:class:`NotificationsUtil`, Dict[:class:`str`, :class:`str`]]]]
         """
-        if identities is not None and notifications is not None:
-            raise ValueError("Should only supply one argument, either identities or notifications.")
-        elif identities is None and notifications is None:
-            raise ValueError("Must supply at least one argument, either identities or notifications.")
-        try:
-            name = "identities" if notifications is None else "notifications"
-            params = JsonUtil.list_to_labeled_dict(locals()[name], name)
-        except Exception as exc:
-            raise ValueError("An error occurred while parsing the argument you provided.") from exc
+        name = "identities" if notifications is None else "notifications"
+        params = JsonUtil.list_to_labeled_dict(locals()[name], name)
         self.http.make_request(Path.mark_notifications_as_read(), **params)
 
-    def revoke_current_token(self):
+    def revoke_current_token(self) -> None:
         """
         Revokes currently authenticated token.
 
         Requires OAuth
         """
         self.http.make_request(Path.revoke_current_token())
 
-    def get_ranking(self, mode: Union[str, GameModeStr], type: Union[str, RankingType],
-                    country: Optional[str] = None, cursor: Optional[dict] = None,
-                    filter: Optional[str] = None, spotlight: Optional[int] = None,
-                    variant: Optional[str] = None) -> Rankings:
+    def get_ranking(
+        self,
+        mode: Union[str, GameModeStr],
+        type: Union[str, RankingType],
+        country: Optional[str] = None,
+        cursor: Optional[dict] = None,
+        filter: Optional[str] = None,
+        spotlight: Optional[int] = None,
+        variant: Optional[str] = None,
+    ) -> Rankings:
         """
         Gets the current ranking for the specified type and game mode.
 
         Requires OAuth and scope public
 
         mode: Union[:class:`str`, :class:`GameModeStr`]
 
         type: Union[:class:`str`, :class:`RankingType`]
             :class:`RankingType`
 
         country: Optional[:class:`str`]
-            Filter ranking by country code. Only available for type of performance.
+            Filter ranking by country code. Only available for `type` of `performance`.
 
         cursor: Optional[:class:`dict`]
 
         filter: Optional[:class:`str`]
-            Either all (default) or friends.
+            Either `all` (default) or `friends`.
 
         spotlight: Optional[:class:`int`]
-            The id of the spotlight if type is charts.
+            The id of the spotlight if `type` is `charts`.
             Ranking for latest spotlight will be returned if not specified.
 
         variant: Optional[:class:`str`]
             Filter ranking to specified mode variant.
-            For mode of mania, it's either 4k or 7k. Only available for type of performance.
+            For `mode` of `mania`, it's either `4k` or `7k`. Only available for `type` of `performance`.
 
         **Returns**
 
         :class:`Rankings`
         """
         mode, type = parse_enum_args(mode, type)
-        return Rankings(self.http.make_request(Path.get_ranking(mode, type), country=country,
-                                               **(cursor if cursor else {}), filter=filter,
-                                               spotlight=spotlight, variant=variant))
+        return Rankings(
+            self.http.make_request(
+                Path.get_ranking(mode, type),
+                country=country,
+                **(cursor if cursor else {}),
+                filter=filter,
+                spotlight=spotlight,
+                variant=variant,
+            )
+        )
 
     def get_spotlights(self) -> Spotlights:
         """
         Gets the list of spotlights.
 
         Requires OAuth and scope public
 
@@ -1666,90 +1804,116 @@
         offset: Optional[:class:`int`]
             Result offset for pagination.
 
         **Returns**
 
         Sequence[:class:`KudosuHistory`]
         """
-        return list(map(KudosuHistory, self.http.make_request(Path.get_user_kudosu(user),
-                                                              limit=limit, offset=offset)))
-
-    def get_user_scores(self, user: int, type: Union[UserScoreType, str], include_fails: Optional[int] = None,
-                        mode: Optional[Union[str, GameModeStr]] = None, limit: Optional[int] = None,
-                        offset: Optional[int] = None) -> Sequence[LegacyScore]:
+        return list(
+            map(
+                KudosuHistory,
+                self.http.make_request(Path.get_user_kudosu(user), limit=limit, offset=offset),
+            )
+        )
+
+    def get_user_scores(
+        self,
+        user: int,
+        type: Union[UserScoreType, str],
+        include_fails: Optional[bool] = False,
+        mode: Optional[Union[str, GameModeStr]] = None,
+        limit: Optional[int] = None,
+        offset: Optional[int] = None,
+    ) -> List[Union[LegacyScore, SoloScore]]:
         """
         This endpoint returns the scores of specified user.
 
         Requires OAuth and scope public
 
         **Parameters**
 
         user: :class:`int`
             Id of the user.
 
-        type: union[:class:`UserScoreType` :class:`str`]
-            Score type. Must be one of these: best, firsts, recent
+        type: Union[:class:`UserScoreType` :class:`str`]
+            Score type. Must be one of `best`, `firsts`, `recent`
 
-        include_fails: Optional[:class:`int`]
-            Only for recent scores, include scores of failed plays. Set to 1 to include them. Defaults to 0.
+        include_fails: Optional[:class:`bool`]
+            Only for recent scores, include scores of failed plays. Defaults to False.
 
         mode: Optional[Union[:class:`GameModeStr`, :class:`str`]]
             game mode of the scores to be returned. Defaults to the specified user's mode.
 
         limit: Optional[:class:`int`]
             Maximum number of results.
 
         offset: Optional[:class:`int`]
             Result offset for pagination.
 
         **Returns**
 
-        Sequence[:class:`LegacyScore`]
-            Includes attributes beatmap, beatmapset, weight: Only for type best, user
+        Sequence[Union[:class:`LegacyScore`, :class:`SoloScore`]]
+            Includes attributes `beatmap`, `beatmapset`. Additionally includes `weight` if `type` is `best`.
         """
         mode, type = parse_enum_args(mode, type)
-        return [LegacyScore(score) for score in self.http.make_request(Path.get_user_scores(user, type),
-                                                                       include_fails=include_fails, mode=mode,
-                                                                       limit=limit, offset=offset)]
-
-    def get_user_beatmaps(self, user: int, type: Union[str, UserBeatmapType], limit: Optional[int] = None,
-                          offset: Optional[int] = None) -> Sequence[Union[BeatmapPlaycount, Beatmapset]]:
+        return list(
+            map(
+                get_score_object,
+                self.http.make_request(
+                    Path.get_user_scores(user, type),
+                    include_fails=int(include_fails),
+                    mode=mode,
+                    limit=limit,
+                    offset=offset,
+                ),
+            )
+        )
+
+    def get_user_beatmaps(
+        self,
+        user: int,
+        type: Union[str, UserBeatmapType],
+        limit: Optional[int] = None,
+        offset: Optional[int] = None,
+    ) -> List[Union[BeatmapPlaycount, Beatmapset]]:
         """
         Returns the beatmaps of specified user.
 
         Requires OAuth and scope public
 
         **Parameters**
 
         user: :class:`int`
             Id of the user.
 
         type: Union[:class:`str`, :class:`UserBeatmapType`]
-            Beatmap type. Can be one of the following - favourite, graveyard, loved, most_played, pending, ranked.
+            Beatmap type. Can be one of `favourite`, `graveyard`, `loved`, `most_played`, `pending`, `ranked`.
 
         limit: Optional[:class:`int`]
             Maximum number of results.
 
         offset: Optional[:class:`int`]
             Result offset for pagination.
 
         **Returns**
 
-        Sequence[Union[:class:`BeatmapPlaycount`, :class:`Beatmapset`]]
-            :class:`BeatmapPlaycount` for type most_played or :class:`Beatmapset` for any other type.
+        List[Union[:class:`BeatmapPlaycount`, :class:`Beatmapset`]]
+            :class:`BeatmapPlaycount` for `type` `most_played` and :class:`Beatmapset` for any other type.
         """
-        object_type = Beatmapset
         type = parse_enum_args(type)
-        if type == 'most_played':
-            object_type = BeatmapPlaycount
-        return list(map(object_type, self.http.make_request(Path.get_user_beatmaps(user, type),
-                                                            limit=limit, offset=offset)))
-
-    def get_user_recent_activity(self, user: int, limit: Optional[int] = None,
-                                 offset: Optional[int] = None) -> Sequence[Event]:
+        return list(
+            map(
+                BeatmapPlaycount if type == "most_played" else Beatmapset,
+                self.http.make_request(Path.get_user_beatmaps(user, type), limit=limit, offset=offset),
+            )
+        )
+
+    def get_user_recent_activity(
+        self, user: int, limit: Optional[int] = None, offset: Optional[int] = None
+    ) -> List[EVENT_TYPE]:
         """
         Returns recent activity.
 
         Requires OAuth and scope public
 
         **Parameters**
 
@@ -1760,56 +1924,69 @@
             Maximum number of results.
 
         offset: Optional[:class:`int`]
             Result offset for pagination.
 
         **Returns**
 
-        Sequence[:class:`Event`]
+        List[:class:`Event`]
             list of :class:`Event` objects
         """
-        return list(map(Event, self.http.make_request(Path.get_user_recent_activity(user),
-                                                      limit=limit, offset=offset)))
-
-    def get_user(self, user: int, mode: Optional[Union[str, GameModeStr]] = '', key: Optional[str] = None) -> User:
+        return list(
+            map(
+                get_event_object,
+                self.http.make_request(Path.get_user_recent_activity(user), limit=limit, offset=offset),
+            )
+        )
+
+    def get_user(
+        self,
+        user: int,
+        mode: Optional[Union[str, GameModeStr]] = "",
+        key: Optional[str] = None,
+    ) -> User:
         """
         This endpoint returns the detail of specified user.
 
+        NOTE: It's highly recommended to pass key parameter
+        to avoid getting unexpected result (mainly when
+        looking up user with numeric username or nonexistent user id).
+
         Requires OAuth and scope public
 
         **Parameters**
 
         user: Union[:class:`int`, :class:`str`]
             Id or username of the user. Id lookup is prioritised unless key parameter is specified.
             Previous usernames are also checked in some cases.
 
         mode: Optional[Union[:class:`str`, :class:`GameModeStr`]
             User default mode will be used if not specified.
 
         key: Optional[:class:`str`]
-            Type of user passed in url parameter. Can be either id or username
+            Type of user passed in url parameter. Can be either `id` or `username`
             to limit lookup by their respective type. Passing empty or invalid
             value will result in id lookup followed by username lookup if not found.
 
         **Returns**
 
         :class:`User`
-            Includes following attributes: account_history, active_tournament_banner,
-            badges, beatmap_playcounts_count, favourite_beatmapset_count, follower_count,
-            graveyard_beatmapset_count, groups, loved_beatmapset_count,
-            mapping_follower_count, monthly_playcounts, page, pending_beatmapset_count,
-            previous_usernames, rank_history, ranked_beatmapset_count, replays_watched_counts,
-            scores_best_count, scores_first_count, scores_recent_count, statistics,
-            statistics.country_rank, statistics.rank, statistics.variants, support_level,
-            user_achievements.
+            Includes attributes `account_history`, `active_tournament_banner`, `badges`,
+            `beatmap_playcounts_count`, `favourite_beatmapset_count`, `follower_count`,
+            `graveyard_beatmapset_count`, `groups`, `loved_beatmapset_count`, `mapping_follower_count`,
+            `monthly_playcounts`, `page`, `pending_beatmapset_count`, `previous_usernames`,
+            `rank_highest`, `rank_history`, `ranked_beatmapset_count`, `replays_watched_counts`,
+            `scores_best_count`, `scores_first_count`, `scores_recent_count`, `statistics`,
+            `statistics.country_rank`, `statistics.rank`, `statistics.variants`, `support_level`,
+            `user_achievements`.
         """
         mode = parse_enum_args(mode)
         return User(self.http.make_request(Path.get_user(user, mode), key=key))
 
-    def get_users(self, ids: Sequence[int]) -> Sequence[UserCompact]:
+    def get_users(self, ids: Sequence[int]) -> List[UserCompact]:
         """
         Returns list of users.
 
         Requires OAuth and scope public
 
         **Parameters**
 
@@ -1841,20 +2018,23 @@
 
         **Returns**
 
         :class:`WikiPage`
         """
         return WikiPage(self.http.make_request(Path.get_wiki_page(locale, path)))
 
-    def get_beatmapset_events(self, page: Optional[int] = None, limit: Optional[int] = None,
-                              sort: Optional[Union[str, BeatmapsetEventSort]] = None,
-                              type: Optional[Union[str, BeatmapsetEventType]] = None,
-                              min_date: Optional[Union[str, datetime]] = None,
-                              max_date: Optional[Union[str, datetime]] = None) -> \
-            Dict[str, Union[Sequence[BeatmapsetEvent], Dict, Sequence[UserCompact]]]:
+    def get_beatmapset_events(
+        self,
+        page: Optional[int] = None,
+        limit: Optional[int] = None,
+        sort: Optional[Union[str, BeatmapsetEventSort]] = None,
+        type: Optional[Union[str, BeatmapsetEventType]] = None,
+        min_date: Optional[Union[str, datetime]] = None,
+        max_date: Optional[Union[str, datetime]] = None,
+    ) -> GetBeatmapsetEventsResult:
         """
         Returns a list of beatmapset events.
 
         Requires OAuth and scope public.
 
         **Parameters**
 
@@ -1866,65 +2046,59 @@
             Specified a sort order.
 
         type: Optional[Union[:class:`str`, :class:`BeatmapsetEventType`]]
             Specifies for only a certain type of event to be returned.
 
         **Returns**
 
-        Dict[str, Union[Sequence[BeatmapsetEvent], Dict, Sequence[UserCompact]]]
-
-        {
-
-            'events': Sequence[BeatmapsetEvent],
-
-            'reviews_config': Dict,
-
-            'users': Sequence[UserCompact]
-
-        }
+        :class:`GetBeatmapsetEventsResult`
         """
         sort, type = parse_enum_args(sort, type)
         if isinstance(min_date, datetime):
             min_date = min_date.isoformat()
         if isinstance(max_date, datetime):
             max_date = max_date.isoformat()
-        resp = self.http.make_request(Path.get_beatmapset_events(), page=page, limit=limit, sort=sort,
-                                      type=type, min_date=min_date, max_date=max_date)
-        return {
-            "events": [BeatmapsetEvent(event) for event in resp['events']],
-            "reviews_config": resp['reviewsConfig'],
-            "users": [UserCompact(user) for user in resp['users']],
-        }
-
-    def get_matches(self, limit: Optional[int] = None, sort: Optional[Union[str, MatchSort]] = None) \
-            -> Dict[str, Union[Sequence[Match], Dict]]:
+        resp = self.http.make_request(
+            Path.get_beatmapset_events(),
+            page=page,
+            limit=limit,
+            sort=sort,
+            type=type,
+            min_date=min_date,
+            max_date=max_date,
+        )
+        return GetBeatmapsetEventsResult(
+            list(map(BeatmapsetEvent, resp["events"])),
+            Review(resp["reviewsConfig"]),
+            list(map(UserCompact, resp["users"])),
+        )
+
+    def get_matches(
+        self, limit: Optional[int] = None, sort: Optional[Union[str, MatchSort]] = None
+    ) -> GetMatchesResult:
         """
         Returns a list of matches.
 
         Requires OAuth and scope public.
 
         **Parameters**
 
         limit: Optional[:class:`int`]
 
         sort: Optional[Union[:class:`str`, :class:`MatchSort`]]
 
         **Returns**
 
-        Dict[:class:`str`, Union[Dict, Sequence[:class:`Match`]]]
+        :class:`GetMatchesResult`
         """
         sort = parse_enum_args(sort)
         resp = self.http.make_request(Path.get_matches(), limit=limit, sort=sort)
-        return {
-            "matches": list(map(Match, resp['matches'])),
-            "cursor": resp['cursor'],
-            "params": resp['params'],
-        }
+        return GetMatchesResult(list(map(Match, resp["matches"])), resp["params"], resp["cursor"])
 
-    def get_match(self, match_id: int) -> Match:
+    def get_match(self, match_id: int) -> MatchExtended:
         """
         Returns a match by id.
 
         Requires OAuth and scope public.
 
         **Parameters**
 
@@ -1933,19 +2107,23 @@
 
         **Returns**
 
         :class:`Match`
         """
         return MatchExtended(self.http.make_request(Path.get_match(match_id)))
 
-    def get_rooms(self, mode: Union[str, GameModeStr] = '', sort: Optional[Union[str, RoomSort]] = None,
-                  limit: Optional[int] = None,
-                  room_type: Optional[Union[RoomType, str]] = None,
-                  category: Optional[Union[RoomCategory, str]] = None,
-                  filter_mode: Optional[Union[RoomFilterMode, str]] = None) -> Sequence[Room]:
+    def get_rooms(
+        self,
+        mode: Union[str, GameModeStr] = "",
+        sort: Optional[Union[str, RoomSort]] = None,
+        limit: Optional[int] = None,
+        room_type: Optional[Union[RoomType, str]] = None,
+        category: Optional[Union[RoomCategory, str]] = None,
+        filter_mode: Optional[Union[RoomFilterMode, str]] = None,
+    ) -> List[Room]:
         """
         Returns a list of rooms.
 
         Requires OAuth, scope public, and a user (authorization code grant, delegate scope, or password auth).
 
         **Parameters**
 
@@ -1962,18 +2140,28 @@
             type of room to look for
 
         category: Optional[Union[:class:`RoomCategory`, :class:`str`]]
             type of category of room to look for
 
         filter_mode: Optional[Union[:class:`RoomFilterMode`, :class:`str`]]
         """
-        mode, sort, room_type, category, filter_mode = parse_enum_args(
-            mode, sort, room_type, category, filter_mode)
-        return list(map(Room, self.http.make_request(Path.get_rooms(mode), sort=sort, limit=limit,
-                                                     type_group=room_type, category=category, mode=filter_mode)))
+        mode, sort, room_type, category, filter_mode = parse_enum_args(mode, sort, room_type, category, filter_mode)
+        return list(
+            map(
+                Room,
+                self.http.make_request(
+                    Path.get_rooms(mode),
+                    sort=sort,
+                    limit=limit,
+                    type_group=room_type,
+                    category=category,
+                    mode=filter_mode,
+                ),
+            )
+        )
 
     def get_seasonal_backgrounds(self) -> SeasonalBackgrounds:
         """
         Get the season backgrounds.
 
         Doesn't require OAuth
 
@@ -1996,108 +2184,83 @@
 
         **Returns**
 
         :class:`Room`
         """
         return Room(self.http.make_request(Path.get_room(room_id)))
 
-    def get_score_by_id(self, mode, score_id) -> LegacyScore:
+    def get_score_by_id(self, mode, score_id) -> Union[LegacyScore, SoloScore]:
         """
         Returns a score by id.
 
         Requires OAuth and scope public.
 
         **Parameters**
 
         mode: Union[:class:`str`, :class:`GameModeStr`]
 
         score_id: :class:`int`
 
         **Returns**
 
-        :class:`LegacyScore`
+        Union[:class:`SoloScore`, :class:`LegacyScore`]
         """
         mode = parse_enum_args(mode)
-        return LegacyScore(self.http.make_request(Path.get_score_by_id(mode, score_id)))
+        return get_score_object(self.http.make_request(Path.get_score_by_id(mode, score_id)))
 
-    def search_beatmapsets(self, filters=None, page=None) -> dict:
+    def search_beatmapsets(self, filters=None, page=None) -> BeatmapsetSearchResult:
         """
         Search for beatmapsets.
 
         Requires OAuth and scope public.
 
         **Attributes**
 
         filters: Optional[:class:`BeatmapsetSearchFilter`]
 
         page: Optional[:class:`int`]
 
         **Returns**
 
-        {
-
-        "beatmapsets": Sequence[:class:`Beatmapset`]
-
-        "cursor": :class:`dict`,
-
-        "search": :class:`dict`,
-
-        "recommended_difficulty": Union[:class:`float`, :class:`None`]
-
-        "error": Union[:class:`str`, :class:`None`]
-
-        "total": :class:`int`
-
-        }
+        :class:`BeatmapsetSearchResult`
         """
         if filters is None:
             filters = {}
         if isinstance(filters, BeatmapsetSearchFilter):
             filters = filters.filters
         resp = self.http.make_request(Path.beatmapset_search(), page=page, **filters)
-        return {
-            'beatmapsets': [Beatmapset(beatmapset) for beatmapset in resp['beatmapsets']],
-            'cursor': resp['cursor'],
-            'search': resp['search'],
-            'recommended_difficulty': resp['recommended_difficulty'],
-            'error': resp['error'],
-            'total': resp['total'],
-        }
+        return BeatmapsetSearchResult(
+            list(map(Beatmapset, resp["beatmapsets"])),
+            resp["cursor"],
+            resp["search"],
+            resp["recommended_difficulty"],
+            resp["error"],
+            resp["total"],
+        )
 
-    def get_room_leaderboard(self, room_id: int) -> \
-            Dict[str, Union[Sequence[UserScoreAggregate], Union[UserScoreAggregate, None]]]:
+    def get_room_leaderboard(self, room_id: int) -> GetRoomLeaderboardResult:
         """
         Return a room's leaderboard. The :class:`UserScoreAggregate` objects returned under the "leaderboard"
         key contain the "user" attribute. The :class:`UserScoreAggregate` object under the "user_score" key
         contains the "user" and "position" attributes.
 
         Requires OAuth, scope public, and a user (authorization code grant, delegate scope, or password auth).
 
         **Parameters**
 
         room_id: :class:`int`
 
         **Returns**
 
-        Dict[:class:`str`, Union[Sequence[:class:`UserScoreAggregate`],
-        Union[:class:`UserScoreAggregate`, :class:`NoneType`]]]
-
-        {
-
-            'leaderboard': Sequence[:class:`UserScoreAggregate`],
-
-            'user_score': Union[:class:`UserScoreAggregate`, :class:`NoneType`]
-
-        }
+        :class:`GetRoomLeaderboard`
         """
         resp = self.http.make_request(Path.get_room_leaderboard(room_id))
-        return {
-            'leaderboard': list(map(UserScoreAggregate, resp['leaderboard'])),
-            'user_score': UserScoreAggregate(resp['user_score']) if resp['user_score'] is not None else None,
-        }
+        return GetRoomLeaderboardResult(
+            list(map(UserScoreAggregate, resp["leaderboard"])), get_optional(resp, "user_score", UserScoreAggregate)
+        )
 
     def get_replay_data(self, mode, score_id):
         """
         Returns replay data for a score.
 
         Requires OAuth, scope public, and a user (authorization code grant, delegate scope, or password auth).
 
@@ -2118,82 +2281,18 @@
         """
         Returns a list of friends.
 
         Requires OAuth, scope friends.read, and a user (authorization code grant, delegate scope, or password auth).
 
         **Returns**
 
-        Sequence[:class:`User`]
+        List[:class:`User`]
         """
         return list(map(UserCompact, self.http.make_request(Path.get_friends())))
 
-    def get_new_score_token(self, beatmap_id: int, version_hash: str, beatmap_hash: str,
-                            ruleset: Union[GameModeInt, GameModeStr, int]) -> dict:
-        """
-        Creates a score token with which can be used to submit a score.
-
-        Requires OAuth, lazer scope, and a user (authorization code grant, delegate scope, or password auth).
-
-        **Parameters**
-
-        beatmap_id: :class:`int`
-            id of the beatmap
-
-        version_hash: :class:`str`
-            version hash is the md5 checksum of f"{game_version}{os_enum}"
-            os_enum is Windows = 1, Linux = 2, macOS = 3, iOS = 4, Android = 5
-
-        beatmap_hash: :class:`str`
-            md5 hash of the beatmap
-
-        ruleset: Union[:class:`GameModeStr`, :class:`GameModeInt`, :class:`int`]
-
-        **Returns**
-
-        :class:`dict`
-
-        {
-
-        "beatmap_id": :class:`int`,
-
-        "created_at": :class:`datetime.datetime`
-
-        "id": :class:`int`
-
-        "user_id": :class:`int`
-
-        }
-        """
-        if isinstance(ruleset, GameModeStr):
-            ruleset = GameModeStr.get_int_equivalent(ruleset)
-        ruleset = parse_enum_args(ruleset)
-        data = {"version_hash": version_hash, "beatmap_hash": beatmap_hash, "ruleset_id": ruleset}
-        resp = self.http.make_request(Path.get_new_score_id(beatmap_id), files=create_multipart_formdata(data))
-        resp["created_at"] = parser.parse(resp["created_at"])
-        return resp
-
-    def submit_score(self, beatmap_id, token, score_data) -> SoloScore:
-        """
-        Submits a score
-
-        Requires OAuth, lazer scope, and a user (authorization code grant, delegate scope, or password auth).
-
-        **Parameters**
-
-        beatmap_id: :class:`int`
-            id of the beatmap
-
-        token: :class:`str`
-            score token which can be obtained from Client.get_new_score_token
-
-        score_data: :class:`dict`
-            data of the score which is being submitted
-        """
-        return SoloScore(self.http.make_request(Path.submit_score(beatmap_id, token), data=score_data))
-
     def favourite_beatmapset(self, beatmapset_id: int, favourite: bool) -> int:
         """
         Add or remove a favourite beatmapset
 
         Requires OAuth, lazer scope, and a user (authorization code grant, delegate scope, or password auth).
 
         **Parameters**
@@ -2204,61 +2303,69 @@
             whether to favourite (true) or unfavourite (false)
 
         **Returns**
 
         :class:`int`
             The number of favourites on the beatmapsets
         """
-        resp = self.http.make_request(Path.favourite_beatmapset(beatmapset_id),
-                                      data={"action": "favourite" if favourite else "unfavourite"})
+        resp = self.http.make_request(
+            Path.favourite_beatmapset(beatmapset_id),
+            data={"action": "favourite" if favourite else "unfavourite"},
+        )
         return resp["favourite_count"]
 
     def get_open_chat_channels(self):
         """
         Get a list of chat channels that you have open. Includes recent DMs and public chat channels.
 
         Requires OAuth, lazer scope, and a user (authorization code grant, delegate scope, or password auth).
 
         **Returns**
 
-        Sequence[:class:`ChatChannel`]
+        List[:class:`ChatChannel`]
         """
         return list(map(ChatChannel, self.http.make_request(Path.get_chat_presence())))
 
-    def join_user_to_room(self, room: int, user: int, password: Optional[str] = None):
+    def join_user_to_room(self, room: int, user: int, password: Optional[str] = None) -> None:
         """
-        Invite a user to a room.
+        Join a user to a room.
 
         Requires OAuth, lazer scope, and a user (authorization code grant, delegate scope, or password auth).
 
         **Parameters**
 
         room: :class:`int`
 
         user: :class:`int`
 
         password: Optional[:class:`str`]
         """
-        return self.http.make_request(Path.join_to_room(room, user), password=password)
+        self.http.make_request(Path.join_to_room(room, user), password=password)
 
-    def kick_user_from_room(self, room: int, user: int):
+    def kick_user_from_room(self, room: int, user: int) -> None:
         """
-        Kick a user from a room (or leave by kicking yourself).
+        Kick a user from a room.
 
         Requires OAuth, lazer scope, and a user (authorization code grant, delegate scope, or password auth).
 
         **Parameters**
 
         room: :class:`int`
 
         user: :class:`int`
         """
-        return self.http.make_request(Path.kick_from_room(room, user))
+        self.http.make_request(Path.kick_from_room(room, user))
 
-    def report(self, comments: str, reason: str, reportable_id: int, reportable_type: Union[ObjectType, str]):
+    def report(
+        self,
+        comments: str,
+        reason: str,
+        reportable_id: int,
+        reportable_type: Union[ObjectType, str],
+    ) -> None:
         """
         Send a report.
 
         Requires OAuth, lazer scope, and a user (authorization code grant, delegate scope, or password auth).
 
         **Parameters**
 
@@ -2267,25 +2374,31 @@
         reason: :class:`str`
 
         reportable_id: :class:`id`
 
         reportable_type: Union[:class:`str`, :class:`ObjectType`]
         """
         params = {
-            "comments": comments, "reason": reason, "reportable_id": reportable_id,
-            "reportable_type": parse_enum_args(reportable_type)
+            "comments": comments,
+            "reason": reason,
+            "reportable_id": reportable_id,
+            "reportable_type": parse_enum_args(reportable_type),
         }
         self.http.make_request(Path.send_report(), **params)
 
-    def create_multiplayer_room(self, name: str, starting_map: Union[PlaylistItemUtil, dict],
-                                password: Optional[str] = None,
-                                queue_mode: Optional[Union[RealTimeQueueMode, str]] = RealTimeQueueMode.HOST_ONLY,
-                                auto_start_duration: Optional[int] = 0,
-                                room_type: Optional[Union[RealTimeType, str]] = RealTimeType.HEAD_TO_HEAD,
-                                auto_skip: Optional[bool] = False) -> Room:
+    def create_multiplayer_room(
+        self,
+        name: str,
+        starting_map: Union[PlaylistItemUtil, dict],
+        password: Optional[str] = None,
+        queue_mode: Optional[Union[RealTimeQueueMode, str]] = RealTimeQueueMode.HOST_ONLY,
+        auto_start_duration: Optional[int] = 0,
+        room_type: Optional[Union[RoomType, str]] = RoomType.HEAD_TO_HEAD,
+        auto_skip: Optional[bool] = False,
+    ) -> Room:
         """
         Create a multiplayer (realtime) room.
 
         Requires OAuth, lazer scope, and a user (authorization code grant, delegate scope, or password auth).
 
         **Parameters**
 
@@ -2298,38 +2411,48 @@
             Password to enter the room which is optional.
 
         queue_mode: Optional[Union[:class:`RealTimeQueueMode`, :class:`str`]]
             The mode for queuing maps.
 
         auto_start_duration: Optional[:class:`int`]
 
-        room_type: Optional[Union[:class:`RealTimeType`, :class:`str`]]
+        room_type: Optional[Union[:class:`RoomType`, :class:`str`]]
 
         auto_skip: Optional[:class:`bool`]
             Whether to automatically skip intro or not.
 
         **Returns**
 
         :class:`Room`
         """
         if isinstance(starting_map, PlaylistItemUtil):
             starting_map = starting_map.json
         queue_mode, room_type = parse_enum_args(queue_mode, room_type)
         data = {
-            "name": name, "password": password, "playlist": [starting_map],
-            "queue_mode": queue_mode, "auto_start_duration": auto_start_duration,
-            "category": "realtime", "type": room_type, "auto_skip": auto_skip,
+            "name": name,
+            "password": password,
+            "playlist": [starting_map],
+            "queue_mode": queue_mode,
+            "auto_start_duration": auto_start_duration,
+            "category": "realtime",
+            "type": room_type,
+            "auto_skip": auto_skip,
         }
         return Room(self.http.make_request(Path.create_room(), data=json.dumps(data)))
 
-    def create_playlist(self, name: str, playlist_items: Sequence[Union[PlaylistItemUtil, dict]],
-                        duration: Optional[int] = None, ends_at: Optional[Union[str, datetime]] = None,
-                        max_attempts: Optional[int] = None,
-                        queue_mode: Optional[Union[PlaylistQueueMode, str]] = PlaylistQueueMode.HOST_ONLY,
-                        auto_start_duration: Optional[int] = 0):
+    def create_playlist(
+        self,
+        name: str,
+        playlist_items: Sequence[Union[PlaylistItemUtil, dict]],
+        duration: Optional[int] = None,
+        ends_at: Optional[Union[str, datetime]] = None,
+        max_attempts: Optional[int] = None,
+        queue_mode: Optional[Union[PlaylistQueueMode, str]] = PlaylistQueueMode.HOST_ONLY,
+        auto_start_duration: Optional[int] = 0,
+    ) -> Room:
         """
         Create a playlist
 
         Requires OAuth, lazer scope, and a user (authorization code grant, delegate scope, or password auth).
 
         **Parameters**
 
@@ -2351,34 +2474,41 @@
         max_attempts: Optional[:class:`int`]
             Null means infinite attempts.
 
         queue_mode: Optional[Union[:class:`PlaylistQueueMode`, :class:`str`]]
             PlaylistQueueMode.HOST_ONLY is the only option
 
         auto_start_duration: Optional[:class:`int`]
+
+        **Returns**
+
+        :class:`Room`
         """
         if duration is None and ends_at is None:
             raise ValueError("Either duration or ends_at must be not null.")
         if ends_at is not None and isinstance(ends_at, datetime):
             ends_at = ends_at.isoformat()
         playlist_items = [item.json if isinstance(item, PlaylistItemUtil) else item for item in playlist_items]
         data = {
-            "name": name, "max_attempts": max_attempts, "duration": duration,
-            "ends_at": ends_at, "queue_mode": parse_enum_args(queue_mode),
-            "auto_start_duration": auto_start_duration, "category": "playlists",
+            "name": name,
+            "max_attempts": max_attempts,
+            "duration": duration,
+            "ends_at": ends_at,
+            "queue_mode": parse_enum_args(queue_mode),
+            "auto_start_duration": auto_start_duration,
+            "category": "playlists",
             "playlist": playlist_items,
         }
         return Room(self.http.make_request(Path.create_room(), data=json.dumps(data)))
 
-    def check_download_quota(self):
+    def check_download_quota(self) -> int:
         """
         Get the amount of quota you've used.
 
         Requires OAuth, lazer scope, and a user (authorization code grant, delegate scope, or password auth).
 
-        Requires
-
         **Returns**
 
         :class:`int`
         """
-        return self.http.make_request(Path.download_quota_check())["quota_used"]
+        resp = self.http.make_request(Path.download_quota_check())
+        return resp["quota_used"]
```

### Comparing `osu.py-0.6.0/osu/constants.py` & `osu.py-1.0.0/osu/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,9 +19,9 @@
     "Nightcore": ["HalfTime"],
     "Flashlight": [],
     "SpunOut": ["AutoPilot"],
     "AutoPilot": ["NoFail", "SuddenDeath", "Perfect", "Relax", "SpunOut"],
     "Perfect": ["NoFail", "SuddenDeath", "Relax"],
     "FadeIn": ["Hidden", "Flashlight"],
     "Mirror": ["HardRock"],
-    **{f"Key{k}": [f"Key{k2}" for k2 in range(4, 10) if k2 != k] for k in range(4, 10)}
+    **{f"Key{k}": [f"Key{k2}" for k2 in range(4, 10) if k2 != k] for k in range(4, 10)},
 }
```

### Comparing `osu.py-0.6.0/osu/http.py` & `osu.py-1.0.0/osu/http.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,23 +7,27 @@
 
 class HTTPHandler:
     def __init__(self, client, request_wait_time, limit_per_minute, use_lazer=False):
         self.client = client
         self.rate_limit = RateLimitHandler(request_wait_time, limit_per_minute)
         self.use_lazer = use_lazer
 
-    def get_headers(self, requires_auth=True, is_files=False, **kwargs):
+    def get_headers(self, path, is_files=False, **kwargs):
         headers = {
-            'charset': 'utf-8',
-            **{str(key): str(value) for key, value in kwargs.items() if value is not None}
+            "charset": "utf-8",
+            "x-api-version": "20220705",
+            "Accept": path.accept,
         }
-        if not is_files and "Content-Type" not in headers:
-            headers["Content-Type"] = "application/json"
-        if requires_auth and "Authorization" not in headers:
-            headers['Authorization'] = f"Bearer {self.client.auth.token}"
+        if not is_files:  # otherwise let requests library handle it
+            headers["Content-Type"] = path.content_type
+        if path.requires_auth and "Authorization" not in headers:
+            headers["Authorization"] = f"Bearer {self.client.auth.token}"
+        for key, value in kwargs.items():
+            if value is not None:
+                headers[str(key)] = str(value)
         return headers
 
     def make_request(self, path, data=None, headers=None, is_download=False, files=None, **kwargs):
         if headers is None:
             headers = {}
         if data is None:
             data = {}
@@ -31,33 +35,40 @@
         if path.requires_auth and self.client.auth is None:
             raise ScopeException("You need to be authenticated to make this request.")
 
         if path.requires_auth and path.scope not in self.client.auth.scope:
             raise ScopeException(f"You don't have the {path.scope} scope, which is required to make this request.")
 
         if path.requires_user and not self.client.auth.has_user:
-            raise ScopeException("This request requires a user. You need either a delegate scope or "
-                                 "to register OAuth with Authorization Code Grant.")
+            raise ScopeException(
+                "This request requires a user. You need either a delegate scope or "
+                "to register OAuth with Authorization Code Grant."
+            )
 
         if not self.rate_limit.can_request:
             self.rate_limit.wait()
 
-        headers = self.get_headers(path.requires_auth, files is not None, **headers)
+        headers = self.get_headers(path, files is not None, **headers)
         params = {str(key): value for key, value in kwargs.items() if value is not None}
-        response = getattr(requests, path.method)((lazer_base_url if self.use_lazer else base_url) + path.path,
-                                                  headers=headers, data=data, params=params, files=files)
+        response = getattr(requests, path.method)(
+            (lazer_base_url if self.use_lazer else base_url) + path.path,
+            headers=headers,
+            data=data,
+            params=params,
+            files=files,
+        )
         self.rate_limit.request_used()
         try:
             response.raise_for_status()
         except Exception as e:
             try:
-                err = response.json()['error']
+                err = response.json()["error"]
             except:
                 err = None
-            raise type(e)(str(e)+": "+err) if err is not None else e
+            raise type(e)(str(e) + ": " + err) if err is not None else e from None
         if response.content == b"":
             return
         return response.json() if not is_download else response.content
 
 
 class RateLimitHandler:
     def __init__(self, request_wait_limit, limit_per_minute):
@@ -67,23 +78,25 @@
         self.requests = []
 
     def request_used(self):
         self.requests.append(time.perf_counter())
         self.last_request = time.perf_counter()
 
     def wait(self):
-        next_available_request = self.wait_limit-(time.perf_counter()-self.last_request)
+        next_available_request = self.wait_limit - (time.perf_counter() - self.last_request)
         if len(self.requests) >= self.limit:
-            next_available_request = max(next_available_request, self.requests[0]+60-time.perf_counter())
+            next_available_request = max(next_available_request, self.requests[0] + 60 - time.perf_counter())
+        if next_available_request <= 0:
+            return
         time.sleep(next_available_request)
 
     def reset(self):
         while len(self.requests) > 0:
             if self.requests[0] + 60 < time.perf_counter():
                 self.requests.pop(0)
             else:
                 break
 
     @property
     def can_request(self):
         self.reset()
-        return time.perf_counter()-self.last_request >= self.wait_limit and len(self.requests) < self.limit
+        return time.perf_counter() - self.last_request >= self.wait_limit and len(self.requests) < self.limit
```

### Comparing `osu.py-0.6.0/osu/notification.py` & `osu.py-1.0.0/osu/notification.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 from .objects import Notification, ChatChannel, UserCompact, ChatMessage
 
 
 class NotificationWebsocket:
     """
     This class allows you to receive notifications without constantly polling the server.
     To utilize it you should do either of:
-        - Make a class inheriting this one and redefine the event functions (on_logout, on_new, ...).
-        - Use the event function as a decorator, read more on its use under its docs.
+    - Make a class inheriting this one and redefine the event functions (on_logout, on_new, ...).
+    - Use the event function as a decorator, read more on its use under its docs.
 
     **Event types**
 
     on_ready
         Fired when the websocket establishes connection.
 
     on_logout
@@ -73,17 +73,24 @@
         users: Sequence[:class:`UserCompact`]
             The related uesrs who sent the messages.
 
     on_unplanned_disconnect
         Event fired by NotificationWebsocket object when there's a disconnection
         without having been sent a logout event.
     """
+
     valid_events = [
-        'ready', 'logout', 'new', 'read', 'unplanned_disconnect', 'chat_channel_join',
-        'chat_channel_part', 'chat_message_new',
+        "ready",
+        "logout",
+        "new",
+        "read",
+        "unplanned_disconnect",
+        "chat_channel_join",
+        "chat_channel_part",
+        "chat_message_new",
     ]
     valid_event_functions = ["on_" + event for event in valid_events]
 
     def __init__(self, notification_uri, auth, loop=None):
         """
         **Arguments**
 
@@ -97,37 +104,37 @@
         self.auth = auth
         self.uri = notification_uri
         self.loop = asyncio.get_event_loop() if loop is None else loop
         self.ws = None
         self.connected = False
 
     async def _run(self):
-        headers = {
-            "Authorization": f"Bearer {self.auth.token}"
-        }
+        headers = {"Authorization": f"Bearer {self.auth.token}"}
         async with websockets.connect(self.uri, extra_headers=headers) as ws:
             self.ws = ws
             await self._on_ready()
             while self.connected:
                 try:
                     event = await self.ws.recv()
                 except websockets.exceptions.ConnectionClosed:
                     self.ws = None
                     self.connected = False
                     await self._on_unplanned_disconnect()
                     return
 
                 event = json.loads(event)
-                if 'error' in event:
+                if "error" in event:
                     print(f"Notification websocket received error: {event['error']}")
                     continue
-                event_type = event['event'].replace(".", "_")
-                del event['event']
+                event_type = event["event"].replace(".", "_")
+                del event["event"]
+
+                # TODO: run event funcs using run_coroutine_threadsafe
 
-                func = getattr(self, "_on_"+event_type)
+                func = getattr(self, "_on_" + event_type)
                 if func is None:
                     return print(f"Received {event_type} event but cannot parse it.")
                 try:
                     await func(event)
                 except:
                     traceback.print_exc()
 
@@ -147,38 +154,39 @@
             notification_websocket = NotificationWebsocket(notif_uri, auth)
 
             @notification_websocket.event()
             def new(notification):
                 print(notification.name)
         """
         if func.__name__ not in self.valid_event_functions:
-            raise ValueError(f"This is not a valid event name. Valid events consist of "
-                             f"{', '.join(self.valid_event_functions)}")
+            raise ValueError(
+                f"This is not a valid event name. Valid events consist of " f"{', '.join(self.valid_event_functions)}"
+            )
         setattr(self, func.__name__, func)
 
     # Default events
 
     # Fired by NotificationSocket when websocket establishes connection.
     async def _on_ready(self):
         self.connected = True
         if hasattr(self, "on_ready"):
             await self.on_ready()
 
     async def _on_logout(self, event):
         self.connected = False
-        if hasattr(self, 'on_logout'):
+        if hasattr(self, "on_logout"):
             await self.on_logout()
 
     async def _on_new(self, event):
-        if hasattr(self, 'on_new'):
+        if hasattr(self, "on_new"):
             data = Notification(event["data"])
             await self.on_new(data)
 
     async def _on_read(self, event):
-        if hasattr(self, 'on_read'):
+        if hasattr(self, "on_read"):
             data = event["data"]
             notifications = list(map(lambda notification: notification["id"], data["notifications"]))
             timestamp = parser.parse(data["timestamp"])
             await self.on_read(notifications, timestamp)
 
     async def _on_chat_channel_join(self, event):
         if hasattr(self, "on_chat_channel_join"):
@@ -193,15 +201,15 @@
             data = event["data"]
             messages = list(map(ChatMessage, data["messages"]))
             users = list(map(UserCompact, data["users"]))
             await self.on_chat_message_new(messages, users)
 
     # Event fired by NotificationWebsocket object when connection without having been sent a logout event.
     async def _on_unplanned_disconnect(self):
-        if hasattr(self, 'on_unplanned_disconnect'):
+        if hasattr(self, "on_unplanned_disconnect"):
             await self.on_unplanned_disconnect()
 
     # Commands
 
     async def send_json(self, event):
         await self.ws.send(json.dumps({"event": event}))
```

### Comparing `osu.py-0.6.0/osu/objects/beatmap.py` & `osu.py-1.0.0/osu/objects/beatmap.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,243 +1,276 @@
-from ..enums import RankStatus, GameModeStr, GameModeInt
-from .user import UserCompact, CurrentUserAttributes
 from dateutil import parser
+from typing import Dict, Optional, List, Union, TYPE_CHECKING
+
+from ..enums import RankStatus, GameModeStr, GameModeInt
+from ..util import prettify, get_optional, get_optional_list
+from .user import UserCompact
+from .current_user_attributes import BeatmapsetPermissions
 
-from ..util import prettify
+
+if TYPE_CHECKING:
+    from datetime import datetime
 
 
 class BeatmapsetCompact:
     """
     Represents a beatmapset.
 
     **Attributes**
 
     artist: :class:`str`
 
     artist_unicode: :class:`str`
 
+    background_url: :class:`str`
+        Not given by api but created locally based on beatmapset id.
+
     covers: :class:`Covers`
 
     creator: :class:`str`
 
     favourite_count: :class:`int`
 
+    hype: Optional[:class:`BeatmapsetRequirement`]
+
     id: :class:`int`
 
     nsfw: :class:`bool`
 
+    offset: :class:`int`
+
     play_count: :class:`int`
 
     preview_url: :class:`str`
 
     source: :class:`str`
 
+    spotlight: :class:`bool`
+
     status: :class:`RankStatus`
 
     title: :class:`str`
 
     title_unicode: :class:`str`
 
-    user_id: :class:`int`
-
-    video: :class:`str`
-
-    **Possible Attributes**
-
-    (Information about these attributes is lacking on the documentation)
-
-    beatmaps: :class:`list`
-        list containing objects of type :class:`Beatmap`
-
-    converts
-
-    current_user_attributes: :class:`CurrentUserAttributes`
-
-    description
-
-    discussions
-
-    events
-
-    genre
-
-    has_favourited: :class:`bool`
-
-    language
-
-    nominations: :class:`dict`
-        Contains items current: :class:`int` and required: :class:`int`
-
-    ratings
-
-    recent_favourites
-
-    related_users
-
-    user: :class:`UserCompact`
-    """
-    __slots__ = (
-        "artist", "artist_unicode", "covers", "creator", "favourite_count", "id", "nsfw",
-        "play_count", "preview_url", "source", "status", "title", "title_unicode", "user_id",
-        "video", "beatmaps", "current_user_attributes", "user", "converts", "description", "discussions",
-        "events", "genre", "has_favourited", "language", "nominations", "ratings", "recent_favourites",
-        "related_users"
-    )
-
-    def __init__(self, data):
-        self.artist = data['artist']
-        self.artist_unicode = data['artist_unicode']
-        self.covers = Covers(data['covers'])
-        self.creator = data['creator']
-        self.favourite_count = data['favourite_count']
-        self.id = data['id']
-        self.nsfw = data['nsfw']
-        self.play_count = data['play_count']
-        self.preview_url = data['preview_url']
-        self.source = data['source']
-        self.status = RankStatus[data['status'].upper()]
-        self.title = data['title']
-        self.title_unicode = data['title_unicode']
-        self.user_id = data['user_id']
-        self.video = data['video']
-
-        # Documentation lacks information on all the possible attributes :/
-        self.beatmaps = list(map(Beatmap, data['beatmaps'])) if 'beatmaps' in data else None
-        self.current_user_attributes = CurrentUserAttributes(data['current_user_attributes'],
-                                                             'BeatmapsetDiscussionPermissions') \
-            if 'current_user_attributes' in data else None
-        self.user = UserCompact(data['user']) if 'user' in data else None
-        self.converts = data.get('converts')
-        self.description = data.get('description')
-        self.discussions = data.get('discussions')
-        self.events = data.get('events')
-        self.genre = data.get('genre')
-        self.has_favourited = data.get('has_favourited')
-        self.language = data.get('language')
-        self.nominations = data.get('nominations')
-        self.ratings = data.get('ratings')
-        self.recent_favourites = data.get('recent_favourites')
-        self.related_users = data.get('related_users')
-
-    def __repr__(self):
-        return prettify(self, 'artist', 'title', 'creator')
+    track_id: Optional[:class:`int`]
 
+    user_id: :class:`int`
 
-class Covers:
-    """
-    **Attributes**
-
-    cover: :class:`str`
-
-    cover_2x: :class:`str`
-
-    card: :class:`str`
-
-    card_2x: :class:`str`
-
-    list: :class:`str`
+    video: :class:`bool`
 
-    list_2x: :class:`str`
+    availability: Optional[:class:`BeatmapsetAvailability`]
 
-    slimcover: :class:`str`
+    beatmaps: Optional[List[:class:`BeatmapCompact`]]
+        Beatmaps contained in the beatmapset
 
-    slimcover_2x: :class:`str`
-    """
-    __slots__ = (
-        "cover", "cover_2x", "card", "card_2x", "list", "list_2x", "slimcover", "slimcover_2x"
-    )
+    converts: Optional[List[:class:`Beatmap`]]
 
-    def __init__(self, data):
-        self.cover = data['cover']
-        self.cover_2x = data['cover@2x']
-        self.card = data['card']
-        self.card_2x = data['card@2x']
-        self.list = data['list']
-        self.list_2x = data['list@2x']
-        self.slimcover = data['slimcover']
-        self.slimcover_2x = data['slimcover@2x']
+    current_nominations: Optional[List[Union[:class:`LegacyNominations`, :class:`Nominations`]]]
+
+    current_user_attributes: Optional[:class:`BeatmapsetDiscussionPermissions`]
+
+    description: Optional[:class:`str`]
+
+    description_bbcode: Optional[:class:`str`]
+
+    discussions: Optional[:class:`BeatmapsetDiscussion`]
+
+    events: Optional[List[:class:`BeatmapsetEvent`]]
+
+    genre: Optional[:class:`MetadataAttribute`]
+
+    has_favourited: Optional[:class:`bool`]
+
+    language: Optional[:class:`MetadataAttribute`]
+
+    nominations: Optional[Union[:class:`LegacyNominations`, :class:`Nominations`]]
+
+    ratings: Optional[List[:class:`int`]]
+
+    recent_favourites: Optional[List[:class:`UserCompact`]]
+
+    related_users: Optional[List[:class:`UserCompact`]]
+
+    user: Optional[:class:`UserCompact`]
+    """
+
+    __slots__ = (
+        "artist",
+        "artist_unicode",
+        "covers",
+        "creator",
+        "favourite_count",
+        "hype",
+        "id",
+        "nsfw",
+        "offset",
+        "play_count",
+        "preview_url",
+        "source",
+        "spotlight",
+        "status",
+        "title",
+        "title_unicode",
+        "track_id",
+        "user_id",
+        "video",
+        "background_url",
+        "availability",
+        "beatmaps",
+        "converts",
+        "current_nominations",
+        "current_user_attributes",
+        "description",
+        "description_bbcode",
+        "discussions",
+        "events",
+        "genre",
+        "has_favourited",
+        "language",
+        "nominations",
+        "ratings",
+        "recent_favourites",
+        "related_users",
+        "user",
+    )
+
+    def __init__(self, data):
+        from .discussion import BeatmapsetDiscussion
+        from .beatmapset_event import BeatmapsetEvent
+
+        self.artist: str = data["artist"]
+        self.artist_unicode: str = data["artist_unicode"]
+        self.covers: Covers = Covers(data["covers"])
+        self.creator: str = data["creator"]
+        self.favourite_count: int = data["favourite_count"]
+        self.hype: Optional[BeatmapsetRequirement] = get_optional(data, "hype", BeatmapsetRequirement)
+        self.id: int = data["id"]
+        self.nsfw: bool = data["nsfw"]
+        self.offset: int = data["offset"]
+        self.play_count: int = data["play_count"]
+        self.preview_url: str = data["preview_url"]
+        self.source: str = data["source"]
+        self.spotlight: bool = data["spotlight"]
+        self.status: RankStatus = RankStatus[data["status"].upper()]
+        self.title: str = data["title"]
+        self.title_unicode: str = data["title_unicode"]
+        self.track_id: Optional[int] = data["track_id"]
+        self.user_id: int = data["user_id"]
+        self.video: bool = data["video"]
+
+        self.background_url: str = f"https://assets.ppy.sh/beatmaps/{self.id}/covers/raw.jpg"
+
+        self.availability: BeatmapsetAvailability = get_optional(data, "availability", BeatmapsetAvailability)
+        self.beatmaps: Optional[List[BeatmapCompact]] = get_optional_list(data, "beatmaps", BeatmapCompact)
+        self.converts: Optional[List[Beatmap]] = get_optional_list(data, "converts", Beatmap)
+        self.current_nominations: Optional[List[_NOMINATIONS_TYPE]] = get_optional_list(
+            data, "current_nominations", get_beatmapset_nominations
+        )
+        self.current_user_attributes: Optional[BeatmapsetPermissions] = get_optional(
+            data, "current_user_attributes", BeatmapsetPermissions
+        )
+        self.description: Optional[str] = get_optional(data, "description", lambda value: value["description"])
+        self.description_bbcode: Optional[str] = get_optional(data, "description", lambda value: value.get("bbcode"))
+        self.discussions: Optional[List[BeatmapsetDiscussion]] = get_optional_list(
+            data, "discussions", BeatmapsetDiscussion
+        )
+        self.events: Optional[List[BeatmapsetEvent]] = get_optional_list(data, "events", BeatmapsetEvent)
+        self.genre: Optional[MetadataAttribute] = get_optional(data, "genre", MetadataAttribute)
+        self.has_favourited: Optional[bool] = data.get("has_favourited")
+        self.language: Optional[MetadataAttribute] = get_optional(data, "language", MetadataAttribute)
+        self.nominations: Optional[_NOMINATIONS_TYPE] = get_optional(data, "nominations", get_beatmapset_nominations)
+        self.ratings: Optional[List[int]] = data.get("ratings")
+        self.recent_favourites: Optional[List[UserCompact]] = get_optional_list(data, "recent_favourites", UserCompact)
+        self.related_users: Optional[List[UserCompact]] = get_optional_list(data, "related_users", UserCompact)
+        self.user: Optional[UserCompact] = get_optional(data, "user", UserCompact)
 
     def __repr__(self):
-        return prettify(self, 'cover')
+        return prettify(self, "artist", "title", "creator")
 
 
 class Beatmapset(BeatmapsetCompact):
     """
     Represents a beatmapset. This extends :class:`BeatmapsetCompact` with additional attributes.
+    Also overrides the type of `beatmaps` attribute.
 
     **Attributes**
 
-    availability: :class:`dict`
-        Contains two items, download_disabled: :class:`bool` and more_information: :class:`str`
+    availability: :class:`BeatmapsetAvailability`
+
+    beatmaps: Optional[List[:class:`Beatmap`]]
+        null when this :class:`Beatmapset` object comes from a :class:`Beatmap` object
 
     bpm: :class:`float`
 
     can_be_hyped: :class:`bool`
 
-    creator: :class:`str`
-        Username of the mapper at the time of beatmapset creation.
+    deleted_at: :class:`datetime.datetime`
 
     discussion_enabled: :class:`bool`
         Deprecated. Is always true.
 
     discussion_locked: :class:`bool`
 
-    hype: :class:`dict`
-        Contains items current: :class:`int` and required: :class:`int`
-
     is_scoreable: :class:`bool`
 
-    last_updated: :class:`datetime.datetime`
+    last_updated: Optional[:class:`datetime.datetime`]
 
     legacy_thread_url: :class:`str`
 
-    nominations: :class:`dict`
-        Contains items current: :class:`int` and required: :class:`int`
+    nominations_summary: :class:`NominationsSummary`
 
     ranked: :class:`RankStatus`
 
-    ranked_date: :class:`datetime.datetime`
-
-    source: :class:`str`
+    ranked_date: Optional[:class:`datetime.datetime`]
 
     storyboard: :class:`bool`
 
-    submitted_date: :class:`datetime.datetime`
+    submitted_date: Optional[:class:`datetime.datetime`]
 
     tags: :class:`str`
     """
+
     __slots__ = (
-        "availability", "bpm", "can_be_hyped", "creator", "discussion_enabled", "discussion_locked",
-        "hype", "is_scoreable", "last_updated", "legacy_thread_url", "ranked", "ranked_date", "storyboard",
-        "submitted_date", "tags", "has_favourited", "nominations"
+        "availability",
+        "bpm",
+        "can_be_hyped",
+        "deleted_at",
+        "discussion_enabled",
+        "discussion_locked",
+        "is_scoreable",
+        "last_updated",
+        "legacy_thread_url",
+        "nominations_summary",
+        "ranked",
+        "ranked_date",
+        "storyboard",
+        "submitted_date",
+        "tags",
     )
 
     def __init__(self, data):
         super().__init__(data)
-        self.availability = data['availability']
-        self.bpm = data['bpm']
-        self.can_be_hyped = data['can_be_hyped']
-        self.creator = data['creator']
-        self.discussion_enabled = True  # Deprecated, all beatmapset discussions are enabled
-        self.discussion_locked = data['discussion_locked']
-        self.hype = data['hype']
-        self.is_scoreable = data['is_scoreable']
-        self.last_updated = parser.parse(data['last_updated']) if data.get('last_updated') is not None else None
-        self.legacy_thread_url = data['legacy_thread_url']
-        self.ranked_date = parser.parse(data['ranked_date']) if data.get('ranked_date') is not None else None
-        self.source = data['source']
-        self.storyboard = data['storyboard']
-        self.tags = data['tags']
-        self.submitted_date = parser.parse(data['submitted_date']) if data.get('submitted_date') is not None else None
-        self.has_favourited = data['has_favourited'] if 'has_favourited' in data else None
-        self.ranked = RankStatus(int(data['ranked']))
-        self.nominations = data['nominations'] if 'nominations' in data else None
 
-    def __repr__(self):
-        return super().__repr__()
+        self.availability: BeatmapsetAvailability = BeatmapsetAvailability(data["availability"])
+        self.beatmaps: Optional[List[Beatmap]] = get_optional_list(data, "beatmaps", Beatmap)
+        self.bpm: float = data["bpm"]
+        self.can_be_hyped: bool = data["can_be_hyped"]
+        self.deleted_at: Optional[datetime] = get_optional(data, "deleted_at", parser.parse)
+        self.discussion_enabled: bool = True  # Deprecated, all beatmapset discussions are enabled
+        self.discussion_locked: bool = data["discussion_locked"]
+        self.is_scoreable: bool = data["is_scoreable"]
+        self.last_updated: Optional[datetime] = get_optional(data, "last_updated", parser.parse)
+        self.legacy_thread_url: Optional[str] = data["legacy_thread_url"]
+        self.nominations_summary: BeatmapsetRequirement = BeatmapsetRequirement(data["nominations_summary"])
+        self.ranked: RankStatus = RankStatus(data["ranked"])
+        self.ranked_date: Optional[datetime] = get_optional(data, "ranked_date", parser.parse)
+        self.storyboard: bool = data["storyboard"]
+        self.submitted_date: Optional[datetime] = get_optional(data, "submitted_date", parser.parse)
+        self.tags: str = data["tags"]
 
 
 class BeatmapCompact:
     """
     Represents a beatmap.
 
     **Attributes**
@@ -254,133 +287,172 @@
 
     total_length: :class:`int`
 
     user_id: :class:`int`
 
     version: :class:`str`
 
-    **Possible Attributes**
+    beatmapset: Optional[:class:`BeatmapsetCompact`]
 
-    beatmapset: :class:`Beatmapset` | :class:`BeatmapsetCompact` | :class:`NoneType`
-        Beatmapset for Beatmap object, BeatmapsetCompact for BeatmapCompact object.
-        null if the beatmap doesn't have associated beatmapset (e.g. deleted).
+    checksum: Optional[:class:`str`]
 
-    checksum: :class:`str` or :class:`NoneType`
+    failtimes: Optional[:class:`Failtimes`]
 
-    failtimes: :class:`Failtimes`
+    max_combo: Optional[:class:`int`]
 
-    max_combo: :class:`int`
+    user: Optional[:class:`UserCompact`]
     """
+
     __slots__ = (
-        "difficulty_rating", "id", "mode", "status", "total_length", "user_id", "version",
-        "checksum", "max_combo", "failtimes", "beatmapset"
+        "beatmapset_id",
+        "difficulty_rating",
+        "id",
+        "mode",
+        "status",
+        "total_length",
+        "user_id",
+        "version",
+        "beatmapset",
+        "checksum",
+        "failtimes",
+        "max_combo",
+        "user",
     )
 
     def __init__(self, data):
-        self.difficulty_rating = data['difficulty_rating']
-        self.id = data['id']
-        self.mode = GameModeStr(data['mode'])
-        self.status = RankStatus[data['status'].upper()]
-        self.total_length = data['total_length']
-        self.user_id = data['user_id']
-        self.version = data['version']
-        self.checksum = data.get("checksum", None)
-        self.max_combo = data.get("max_combo", None)
-        self.failtimes = Failtimes(data['failtimes']) if "failtimes" in data else None
-
-        if 'beatmapset' in data and data['beatmapset'] is not None:
-            if type(self).__name__ == 'Beatmap':
-                self.beatmapset = Beatmapset(data['beatmapset'])
-            else:
-                self.beatmapset = BeatmapsetCompact(data['beatmapset'])
-        else:
-            self.beatmapset = None
+        self.beatmapset_id: int = data["beatmapset_id"]
+        self.difficulty_rating: float = data["difficulty_rating"]
+        self.id: int = data["id"]
+        self.mode: GameModeStr = GameModeStr(data["mode"])
+        self.status: RankStatus = RankStatus[data["status"].upper()]
+        self.total_length: int = data["total_length"]
+        self.user_id: int = data["user_id"]
+        self.version: str = data["version"]
+
+        self.beatmapset: Optional[BeatmapsetCompact] = get_optional(data, "beatmapset", BeatmapsetCompact)
+        self.checksum: Optional[str] = data.get("checksum")
+        self.failtimes: Optional[Failtimes] = get_optional(data, "failtimes", Failtimes)
+        self.max_combo: Optional[int] = data.get("max_combo")
+        self.user: Optional[UserCompact] = get_optional(data, "user", UserCompact)
 
     def __repr__(self):
-        return prettify(self, 'version', 'beatmapset')
+        return prettify(
+            self,
+            "beatmapset_id" if self.beatmapset is None else "beatmapset",
+            "version",
+        )
 
 
-class BeatmapDifficultyAttributes:
+class Beatmap(BeatmapCompact):
     """
-    Represent beatmap difficulty attributes. Following fields are always present and
-    then there are additional fields for different rulesets.
+    Represent a beatmap. This extends :class:`BeatmapCompact` with additional attributes.
+    Also overrides the type of `beatmapset`
 
     **Attributes**
 
-    The parameters depend on the ruleset, but the following two attributes are present in all rulesets.
+    accuracy: :class:`float`
 
-    max_combo: :class:`int`
+    ar: :class:`float`
 
-    star_rating: :class:`float`
+    beatmapset: Optional[:class:`Beatmapset`]
 
-    mode_attributes: Union[:class:`OsuBeatmapDifficultyAttributes`, :class:`TaikoBeatmapDifficultyAttributes`,
-    :class:`FruitsBeatmapDifficultyAttributes`, :class:`ManiaBeatmapDifficultyAttributes`, :class:`None`]
-        Can be none for some beatmaps that are bugged and have no difficulty attributes.
+    bpm: :class:`float`
+
+    convert: Optional[:class:`bool`]
 
-    osu
-        aim_difficulty: :class:`float`
+    count_circles: :class:`int`
 
-        approach_rate: :class:`float`
+    count_sliders: :class:`int`
 
-        flashlight_difficulty: :class:`float`
+    count_spinners: :class:`int`
 
-        overall_difficulty: :class:`float`
+    cs: :class:`float`
 
-        slider_factor: :class:`float`
+    deleted_at: Optional[:class:`datetime.datetime`]
 
-        speed_difficulty: :class:`float`
+    drain: :class:`float`
 
-    taiko
-        stamina_difficulty: :class:`float`
+    hit_length: :class:`int`
 
-        rhythm_difficulty: :class:`float`
+    is_scoreable: :class:`bool`
 
-        colour_difficulty: :class:`float`
+    last_updated: :class:`datetime.datetime`
 
-        approach_rate: :class:`float`
+    mode_int: :class:`GameModeInt`
 
-        great_hit_window: :class:`float`
+    passcount: :class:`int`
 
-    fruits
-        approach_rate: :class:`float`
+    playcount: :class:`int`
 
-    mania
-        great_hit_window: :class:`float`
+    ranked: :class:`RankStatus`
 
-        score_multiplier: :class:`float`
+    url: :class:`str`
     """
+
     __slots__ = (
-        "max_combo", "star_rating", "type", "mode_attributes"
+        "accuracy",
+        "ar",
+        "bpm",
+        "convert",
+        "count_circles",
+        "count_sliders",
+        "count_spinners",
+        "cs",
+        "deleted_at",
+        "drain",
+        "hit_length",
+        "is_scoreable",
+        "last_updated",
+        "mode_int",
+        "passcount",
+        "playcount",
+        "ranked",
+        "url",
     )
 
     def __init__(self, data):
-        data = data['attributes']
-        self.max_combo = data['max_combo']
-        self.star_rating = data['star_rating']
-        if "aim_difficulty" in data:
-            self.type = "osu"
-            self.mode_attributes = OsuBeatmapDifficultyAttributes(data)
-        elif "stamina_difficulty" in data:
-            self.type = "taiko"
-            self.mode_attributes = TaikoBeatmapDifficultyAttributes(data)
-        elif "great_hit_window" in data:
-            self.type = "mania"
-            self.mode_attributes = ManiaBeatmapDifficultyAttributes(data)
-        elif "approach_rate" in data:
-            self.type = 'fruits'
-            self.mode_attributes = FruitsBeatmapDifficultyAttributes(data)
-        else:
-            self.type = None
-            self.mode_attributes = None
+        super().__init__(data)
 
-    def __getattr__(self, item):
-        return getattr(self.mode_attributes, item)
+        self.accuracy: float = data["accuracy"]
+        self.ar: float = data["ar"]
+        self.beatmapset: Optional[Beatmapset] = get_optional(data, "beatmapset", Beatmapset)
+        self.bpm: float = data["bpm"]
+        self.convert: Optional[bool] = data["convert"]
+        self.count_circles: int = data["count_circles"]
+        self.count_sliders: int = data["count_sliders"]
+        self.count_spinners: int = data["count_spinners"]
+        self.cs: float = data["cs"]
+        self.deleted_at: Optional[datetime] = get_optional(data, "deleted_at", parser.parse)
+        self.drain: float = data["drain"]
+        self.hit_length: int = data["hit_length"]
+        self.is_scoreable: bool = data["is_scoreable"]
+        self.last_updated: datetime = parser.parse(data["last_updated"])
+        self.mode_int: GameModeInt = GameModeInt(data["mode_int"])
+        self.passcount: int = data["passcount"]
+        self.playcount: int = data["playcount"]
+        self.ranked: RankStatus = RankStatus(data["ranked"])
+        self.url: str = data["url"]
 
-    def __repr__(self):
-        return prettify(self, 'star_rating', 'type', 'mode_attributes')
+
+class MetadataAttribute:
+    """
+    Genre of a beatmapset
+
+    **Attributes**
+
+    id: Optional[:class:`int`]
+
+    name: :class:`str`
+    """
+
+    __slots__ = ("id", "name")
+
+    def __init__(self, data):
+        self.id: Optional[int] = data["id"]
+        self.name: str = data["name"]
 
 
 class OsuBeatmapDifficultyAttributes:
     """
     osu!standard beatmap difficulty attributes.
     See :class:`BeatmapDifficultyAttributes` for more information.
 
@@ -396,31 +468,36 @@
 
     slider_factor: :class:`float`
 
     speed_difficulty: :class:`float`
 
     speed_note_count: :class:`float`
     """
+
     __slots__ = (
-        "aim_difficulty", "approach_rate", "flashlight_difficulty",
-        "overall_difficulty", "slider_factor", "speed_difficulty",
-        "speed_note_count"
+        "aim_difficulty",
+        "approach_rate",
+        "flashlight_difficulty",
+        "overall_difficulty",
+        "slider_factor",
+        "speed_difficulty",
+        "speed_note_count",
     )
 
     def __init__(self, data):
-        self.aim_difficulty = data['aim_difficulty']
-        self.approach_rate = data['approach_rate']
-        self.flashlight_difficulty = data['flashlight_difficulty']
-        self.overall_difficulty = data['overall_difficulty']
-        self.slider_factor = data['slider_factor']
-        self.speed_difficulty = data['speed_difficulty']
-        self.speed_note_count = data['speed_note_count']
+        self.aim_difficulty: float = data["aim_difficulty"]
+        self.approach_rate: float = data["approach_rate"]
+        self.flashlight_difficulty: float = data["flashlight_difficulty"]
+        self.overall_difficulty: float = data["overall_difficulty"]
+        self.slider_factor: float = data["slider_factor"]
+        self.speed_difficulty: float = data["speed_difficulty"]
+        self.speed_note_count: float = data["speed_note_count"]
 
     def __repr__(self):
-        return prettify(self, 'aim_difficulty', 'speed_difficulty')
+        return prettify(self, "aim_difficulty", "speed_difficulty")
 
 
 class TaikoBeatmapDifficultyAttributes:
     """
     osu!taiko beatmap difficulty attributes.
     See :class:`BeatmapDifficultyAttributes` for more information.
 
@@ -434,192 +511,360 @@
 
     great_hit_window: :class:`float`
 
     peak_difficulty: :class:`float`
     """
 
     __slots__ = (
-        "stamina_difficulty", "rhythm_difficulty", "colour_difficulty",
-        "great_hit_window", "peak_difficulty"
+        "stamina_difficulty",
+        "rhythm_difficulty",
+        "colour_difficulty",
+        "great_hit_window",
+        "peak_difficulty",
     )
 
     def __init__(self, data):
-        self.stamina_difficulty = data['stamina_difficulty']
-        self.rhythm_difficulty = data['rhythm_difficulty']
-        self.colour_difficulty = data['colour_difficulty']
-        self.great_hit_window = data['great_hit_window']
-        self.peak_difficulty = data['peak_difficulty']
+        self.stamina_difficulty: float = data["stamina_difficulty"]
+        self.rhythm_difficulty: float = data["rhythm_difficulty"]
+        self.colour_difficulty: float = data["colour_difficulty"]
+        self.great_hit_window: float = data["great_hit_window"]
+        self.peak_difficulty: float = data["peak_difficulty"]
 
     def __repr__(self):
-        return prettify(self, 'stamina_difficulty')
+        return prettify(self, "stamina_difficulty")
 
 
 class FruitsBeatmapDifficultyAttributes:
     """
     osu!catch beatmap difficulty attributes.
     See :class:`BeatmapDifficultyAttributes` for more information.
 
     **Attributes**
 
     approach_rate: :class:`float`
     """
 
-    __slots__ = (
-        "approach_rate"
-    )
+    __slots__ = "approach_rate"
 
     def __init__(self, data):
-        self.approach_rate = data['approach_rate']
+        self.approach_rate: float = data["approach_rate"]
 
     def __repr__(self):
-        return prettify(self, 'approach_rate')
+        return prettify(self, "approach_rate")
 
 
 class ManiaBeatmapDifficultyAttributes:
     """
     osu!mania beatmap difficulty attributes.
     See :class:`BeatmapDifficultyAttributes` for more information.
 
     **Attributes**
 
     great_hit_window: :class:`float`
+
+    score_multiplier: :class:`float`
     """
 
-    __slots__ = (
-        "great_hit_window"
-    )
+    __slots__ = ("great_hit_window", "score_multiplier")
 
     def __init__(self, data):
-        self.great_hit_window = data['great_hit_window']
+        self.great_hit_window: float = data["great_hit_window"]
+        self.score_multiplier: float = data["score_multiplier"]
 
     def __repr__(self):
-        return prettify(self, 'great_hit_window')
+        return prettify(self, "great_hit_window")
 
 
-class Failtimes:
+class BeatmapDifficultyAttributes:
     """
-    All attributes are optional but there's always at least one attribute present.
+    Represent beatmap difficulty attributes. Following fields are always present and
+    then there are additional fields for different rulesets.
 
     **Attributes**
 
-    exit: Sequence[:class:`int`]
-        Sequence of integers. List is length 100.
+    The parameters depend on the ruleset, but the following two attributes are present in all rulesets.
 
-    fail: Sequence[:class:`int`]
-        Sequence of integers. List is length 100.
-    """
-    def __init__(self, data):
-        if 'exit' in data:
-            self.exit = data['exit']
-        if 'fail' in data:
-            self.fail = data['fail']
+    max_combo: :class:`int`
 
-    def __repr__(self):
-        try:
-            return prettify(self, 'exit')
-        except AttributeError:
-            return prettify(self, 'fail')
+    star_rating: :class:`float`
 
+    mode_attributes: Optional[Union[:class:`OsuBeatmapDifficultyAttributes`, :class:`TaikoBeatmapDifficultyAttributes`,
+    :class:`FruitsBeatmapDifficultyAttributes`, :class:`ManiaBeatmapDifficultyAttributes`]]
+        Can be none for some beatmaps that are bugged and have no difficulty attributes.
 
-class Beatmap(BeatmapCompact):
+    type: Optional[:class:`GameModeStr`]
     """
-    Represent a beatmap. This extends :class:`BeatmapCompact` with additional attributes.
 
-    **Attributes**
+    __slots__ = ("max_combo", "star_rating", "type", "mode_attributes")
+    if TYPE_CHECKING:
+        type: Optional[GameModeStr]
+        mode_attributes: Optional[
+            Union[
+                OsuBeatmapDifficultyAttributes,
+                TaikoBeatmapDifficultyAttributes,
+                ManiaBeatmapDifficultyAttributes,
+                FruitsBeatmapDifficultyAttributes,
+            ]
+        ]
+
+    def __init__(self, data):
+        data = data["attributes"]
+        self.max_combo: int = data["max_combo"]
+        self.star_rating: float = data["star_rating"]
+        if "aim_difficulty" in data:
+            self.type = GameModeStr.STANDARD
+            self.mode_attributes = OsuBeatmapDifficultyAttributes(data)
+        elif "stamina_difficulty" in data:
+            self.type = GameModeStr.TAIKO
+            self.mode_attributes = TaikoBeatmapDifficultyAttributes(data)
+        elif "great_hit_window" in data:
+            self.type = GameModeStr.MANIA
+            self.mode_attributes = ManiaBeatmapDifficultyAttributes(data)
+        elif "approach_rate" in data:
+            self.type = GameModeStr.CATCH
+            self.mode_attributes = FruitsBeatmapDifficultyAttributes(data)
+        else:
+            self.type = None
+            self.mode_attributes = None
 
-    accuracy: :class:`float`
+    def __getattr__(self, item):
+        return getattr(self.mode_attributes, item)
 
-    ar: :class:`float`
+    def __repr__(self):
+        return prettify(self, "star_rating", "type", "mode_attributes")
 
-    beatmapset_id: :class:`int`
 
-    bpm: :class:`float` or :class:`NoneType`
+class Failtimes:
+    """
+    **Attributes**
 
-    convert: :class:`bool`
+    exit: Optional[List[:class:`int`]]
+        List of 100 integers.
 
-    count_circles: :class:`int`
+    fail: Optional[List[:class:`int`]]
+        List of 100 integers.
+    """
 
-    count_sliders: :class:`int`
+    __slots__ = ("exit", "fail")
 
-    count_spinners: :class:`int`
+    def __init__(self, data):
+        self.exit: Optional[List[int]] = data.get("exit")
+        self.fail: Optional[List[int]] = data.get("fail")
 
-    cs: :class:`float`
+    def __repr__(self):
+        return prettify(self, "exit" if self.exit is not None else "fail")
 
-    deleted_at: :class:`datetime.datetime` or :class:`NoneType`
 
-    drain: :class:`float`
+class Covers:
+    """
+    **Attributes**
 
-    hit_length: :class:`int`
+    cover: :class:`str`
 
-    is_scoreable: :class:`bool`
+    cover_2x: :class:`str`
 
-    last_updated: :class:`datetime.datetime`
+    card: :class:`str`
 
-    mode_int: :class:`GameModeInt`
+    card_2x: :class:`str`
 
-    passcount: :class:`int`
+    list: :class:`str`
 
-    playcount: :class:`int`
+    list_2x: :class:`str`
 
-    ranked: :class:`RankStatus`
+    slimcover: :class:`str`
 
-    url: :class:`str`
+    slimcover_2x: :class:`str`
     """
+
     __slots__ = (
-        "ranked", "url", "playcount", "passcount", "mode_int", "last_updated",
-        "is_scoreable", "hit_length", "drain", "deleted_at", "cs", "count_spinners",
-        "count_circles", "count_sliders", "convert", "bpm", "beatmapset_id", "ar",
-        "accuracy"
+        "cover",
+        "cover_2x",
+        "card",
+        "card_2x",
+        "list",
+        "list_2x",
+        "slimcover",
+        "slimcover_2x",
     )
 
     def __init__(self, data):
-        super().__init__(data)
-        self.ranked = RankStatus(int(data['ranked']))
-        self.url = data['url']
-        self.playcount = data['playcount']
-        self.passcount = data['passcount']
-        self.mode_int = GameModeInt(data['mode_int'])
-        self.last_updated = parser.parse(data['last_updated'])
-        self.is_scoreable = data['is_scoreable']
-        self.hit_length = data['hit_length']
-        self.drain = data['drain']
-        self.deleted_at = parser.parse(data['deleted_at']) if data['deleted_at'] is not None else None
-        self.cs = data['cs']
-        self.count_spinners = data['count_spinners']
-        self.count_sliders = data['count_sliders']
-        self.count_circles = data['count_circles']
-        self.convert = data['convert']
-        self.bpm = data['bpm']
-        self.beatmapset_id = data['beatmapset_id']
-        self.ar = data['ar']
-        self.accuracy = data['accuracy']
+        self.cover: str = data["cover"]
+        self.cover_2x: str = data["cover@2x"]
+        self.card: str = data["card"]
+        self.card_2x: str = data["card@2x"]
+        self.list: str = data["list"]
+        self.list_2x: str = data["list@2x"]
+        self.slimcover: str = data["slimcover"]
+        self.slimcover_2x: str = data["slimcover@2x"]
 
     def __repr__(self):
-        return super().__repr__()
+        return prettify(self, "cover")
 
 
 class BeatmapPlaycount:
     """
     Represent the playcount of a beatmap.
 
     **Attributes**
 
     beatmap_id: :class:`int`
 
-    beatmap: :class:`BeatmapCompact` or :class:`NoneType`
+    beatmap: Optional[:class:`BeatmapCompact`]
 
-    beatmapset: :class:`BeatmapsetCompact` or :class:`NoneType`
+    beatmapset: Optional[:class:`BeatmapsetCompact`]
 
     count: :class:`int`
     """
+
+    __slots__ = ("beatmap_id", "beatmap", "beatmapset", "count")
+
+    def __init__(self, data):
+        self.beatmap_id: int = data["beatmap_id"]
+        self.beatmap: Optional[BeatmapCompact] = get_optional(data, "beatmap", BeatmapCompact)
+        self.beatmapset: Optional[BeatmapsetCompact] = get_optional(data, "beatmapset", BeatmapsetCompact)
+        self.count: int = data["count"]
+
+    def __repr__(self):
+        return prettify(self, "beatmap_id", "count")
+
+
+class BeatmapsetRequirement:
+    """
+    Gives information on requirements for a beatmap
+
+    **Attributes**
+
+    current: :class:`int`
+
+    required: :class:`int`
+    """
+
+    __slots__ = ("current", "required")
+
+    def __init__(self, data):
+        self.current: int = data["current"]
+        self.required: int = data["required"]
+
+    def __repr__(self):
+        return prettify(self, "current", "required")
+
+
+class BeatmapsetAvailability:
+    """
+    Gives information on the availability of a beatmap for download.
+
+    **Attributes**
+
+    download_disabled: :class:`bool`
+
+    more_information: Optional[:class:`str`]
+    """
+
+    __slots__ = ("download_disabled", "more_information")
+
+    def __init__(self, data):
+        self.download_disabled: bool = data["download_disabled"]
+        self.more_information: Optional[str] = data.get("more_information")
+
+    def __repr__(self):
+        return prettify(self, "download_disabled", "more_information")
+
+
+class BaseNominations:
+    """
+    Base attributes for :class:`LegacyNominations` and :class:`Nominations`
+
+    **Attributes**
+
+    disqualification: Optional[:class:`BeatmapsetEvent`]
+
+    nominated: Optional[:class:`bool`]
+
+    nomination_reset: Optional[:class:`BeatmapsetEvent`]
+
+    ranking_eta: Optional[:class:`str`]
+
+    ranking_queue_position: Optional[:class:`int`]
+
+    required_hype: :class:`int`
+    """
+
     __slots__ = (
-        "beatmap_id", "beatmap", "beatmapset", "count"
+        "disqualification",
+        "nominated",
+        "nomination_reset",
+        "ranking_eta",
+        "ranking_queue_position",
+        "required_hype",
     )
 
     def __init__(self, data):
-        self.beatmap_id = data['beatmap_id']
-        self.beatmap = BeatmapCompact(data['beatmap']) if data['beatmap'] is not None else None
-        self.beatmapset = BeatmapsetCompact(data['beatmapset']) if data['beatmapset'] is not None else None
-        self.count = data['count']
+        from .beatmapset_event import BeatmapsetEvent
 
-    def __repr__(self):
-        return prettify(self, 'beatmap_id', 'count')
+        self.disqualification: Optional[BeatmapsetEvent] = get_optional(data, "disqualification", BeatmapsetEvent)
+        self.nominated: Optional[bool] = data["nominated"]
+        self.nomination_reset: Optional[BeatmapsetEvent] = get_optional(data, "nomination_reset", BeatmapsetEvent)
+        self.ranking_eta: Optional[str] = data["ranking_eta"]
+        self.ranking_queue_position: Optional[int] = data["ranking_queue_position"]
+        self.required_hype: int = data["required_hype"]
+
+
+class LegacyNominations(BaseNominations):
+    """
+    Shows info about nominations on a beatmapset, extending :class:`BaseNominations`
+
+    **Attributes**
+
+    is_legacy: :class:`bool`
+        True
+
+    current: :class:`int`
+
+    required: :class:`int`
+    """
+
+    __slots__ = ("current", "required")
+    is_legacy = True
+
+    def __init__(self, data):
+        super().__init__(data)
+        self.current: int = data["current"]
+        self.required: int = data["required"]
+
+
+class Nominations(BaseNominations):
+    """
+    Shows info about nominations on a beatmapset, extending :class:`BaseNominations`
+
+    **Attributes**
+
+    is_legacy: :class:`bool`
+        False
+
+    current: Union[:class:`int`, Dict[:class:`GameModeStr`, :class:`int`]]
+
+    required: :class:`int`
+    """
+
+    __slots__ = ("current", "required")
+    is_legacy = False
+
+    def __init__(self, data):
+        super().__init__(data)
+        self.current: Dict[GameModeStr, int] = dict(
+            zip(map(GameModeStr, (current := data["current"]).keys()), current.values())
+        )
+        self.required: Dict[GameModeStr, int] = dict(
+            zip(
+                map(GameModeStr, (required := data["required"]).keys()),
+                required.values(),
+            )
+        )
+
+
+_NOMINATIONS_TYPE = Union[LegacyNominations, Nominations]
+
+
+def get_beatmapset_nominations(data) -> _NOMINATIONS_TYPE:
+    if data.get("legacy_mode", False):
+        return LegacyNominations(data)
+    return Nominations(data)
```

### Comparing `osu.py-0.6.0/osu/objects/beatmapset_event.py` & `osu.py-1.0.0/osu/objects/beatmapset_event.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,320 +1,345 @@
+from dateutil import parser
+from typing import Optional, List, TYPE_CHECKING
+
 from ..enums import GameModeStr, BeatmapsetEventType
+from ..util import prettify
 from .discussion import BeatmapsetDiscussion
 from .beatmap import BeatmapsetCompact
-from dateutil import parser
 
-from ..util import prettify
 
+if TYPE_CHECKING:
+    from datetime import datetime
 
-class BeatmapsetEvent:
+
+class BeatmapsetEventComment:
     """
-    Represent a beatmapset event. This object is relevant for the :func:`osu.Client.get_beatmapset_events` endpoint.
+    This object holds some extra information of the event.
 
     **Attributes**
 
-    id: :class:`int`
+    beatmap_discussion_id: Optional[:class:`int`]
 
-    type: :class:`BeatmapsetEventType`
+    beatmap_discussion_post_id: Optional[:class:`int`]
 
-    comment: Union[:class:`BeatmapsetEventComment`, :class:`NoneType`]
-        Is :class:`NoneType` for the following types:
-        - :class:`BeatmapsetEventType.LOVE`
-        - :class:`BeatmapsetEventType.QUALIFY`
-        - :class:`BeatmapsetEventType.APPROVE`
-        - :class:`BeatmapsetEventType.RANK`
+    event_data: Union[:class:`BeatmapsetEventNominate`, :class:`BeatmapsetEventRemoveFromLoved`,
+    :class:`BeatmapsetEventDisqualify`, :class:`BeatmapsetEventKudosuGain`, :class:`BeatmapsetEventKudosuLost`,
+    :class:`BeatmapsetEventKudosuRecalculate`, :class:`BeatmapsetEventDiscussionLock`,
+    :class:`BeatmapsetEventNominationReset`, :class:`BeatmapsetEventNominationResetReceived`,
+    :class:`BeatmapsetEventGenreEdit`, :class:`BeatmapsetEventLanguageEdit`, :class:`BeatmapsetEventNsfwToggle`,
+    :class:`BeatmapsetEventOffsetEdit`, :class:`BeatmapsetEventBeatmapOwnerChange`]
+        The type of this attribute depends on the type of the BeatmapsetEvent object.
+    """
 
-    created_at: :class:`datetime.datetime`
+    __slots__ = ("beatmap_discussion_id", "beatmap_discussion_post_id", "event_data")
 
-    user_id: Union[:class:`int`, :class:`NoneType`]
+    def __init__(self, data, type: BeatmapsetEventType):
+        self.beatmap_discussion_id: Optional[int] = data.get("beatmap_discussion_id")
+        self.beatmap_discussion_post_id: Optional[int] = data.get("beatmap_discussion_post_id")
+        self.event_data = _get_event_data_object(data, type)
 
-    beatmapset: Union[:class:`BeatmapsetCompact`, :class:`NoneType`]
+    def __repr__(self):
+        return prettify(self, "beatmap_discussion_id", "beatmap_discussion_post_id")
 
-    discussion: Union[:class:`BeatmapsetDiscussion`, :class:`NoneType`]
+
+class BeatmapsetEvent:
     """
-    __slots__ = (
-        "id", "type", "comment", "created_at", "user_id", "beatmapset", "discussion"
-    )
+    Represent a beatmapset event. This object is relevant for the :func:`osu.Client.get_beatmapset_events` endpoint.
 
-    def __init__(self, data):
-        self.id = data['id']
-        self.type = BeatmapsetEventType(data['type'])
-        self.comment = data['comment']
-        if self.comment is not None:
-            self.comment = BeatmapsetEventComment(self.comment, self.type)
-        self.created_at = parser.parse(data['created_at'])
-        self.user_id = data.get('user_id')
-        self.beatmapset = BeatmapsetCompact(data['beatmapset']) if data.get("beatmapset") is not None else None
-        self.discussion = BeatmapsetDiscussion(data['discussion']) if data.get('discussion') is not None else None
+    **Attributes**
 
-    def __repr__(self):
-        return prettify(self, 'type', 'beatmapset')
+    id: :class:`int`
 
+    type: :class:`BeatmapsetEventType`
 
-class BeatmapsetEventComment:
-    """
-    This object holds some extra information of the event.
+    comment: Optional[:class:`BeatmapsetEventComment`]
+        Is None for the following types:
+        - :class:`BeatmapsetEventType`.LOVE
+        - :class:`BeatmapsetEventType`.QUALIFY
+        - :class:`BeatmapsetEventType`.APPROVE
+        - :class:`BeatmapsetEventType`.RANK
 
-    **Attributes**
+    created_at: :class:`datetime.datetime`
 
-    beatmap_discussion_id: Union[:class:`int`, :class:`NoneType`]
+    user_id: Optional[:class:`int`]
 
-    beatmap_discussion_post_id: Union[:class:`int`, :class:`NoneType`]
+    beatmapset: Optional[:class:`BeatmapsetCompact`]
 
-    event_data: Union[:class:`BeatmapsetEventNominate`, :class:`BeatmapsetEventRemoveFromLoved`,
-    :class:`BeatmapsetEventDisqualify`, :class:`BeatmapsetEventKudosuGain`, :class:`BeatmapsetEventKudosuLost`,
-    :class:`BeatmapsetEventKudosuRecalculate`, :class:`BeatmapsetEventDiscussionLock`,
-    :class:`BeatmapsetEventNominationReset`, :class:`BeatmapsetEventNominationResetReceived`,
-    :class:`BeatmapsetEventGenreEdit`, :class:`BeatmapsetEventLanguageEdit`, :class:`BeatmapsetEventNsfwToggle`,
-    :class:`BeatmapsetEventOffsetEdit`, :class:`BeatmapsetEventBeatmapOwnerChange`]
-        The type of this attribute depends on the type of the BeatmapsetEvent object.
+    discussion: Optional[:class:`BeatmapsetDiscussion`]
     """
 
     __slots__ = (
-        "beatmap_discussion_id", "beatmap_discussion_post_id", "event_data"
+        "id",
+        "type",
+        "comment",
+        "created_at",
+        "user_id",
+        "beatmapset",
+        "discussion",
     )
-    event_types = {
-        BeatmapsetEventType.NOMINATE: 'BeatmapsetEventNominate',
-        BeatmapsetEventType.REMOVE_FROM_LOVED: 'BeatmapsetEventRemoveFromLoved',
-        BeatmapsetEventType.DISQUALIFY: 'BeatmapsetEventDisqualify',
-        BeatmapsetEventType.KUDOSU_GAIN: 'BeatmapsetEventKudosuGain',
-        BeatmapsetEventType.KUDOSU_LOST: 'BeatmapsetEventKudosuLost',
-        BeatmapsetEventType.KUDOSU_RECALCULATE: 'BeatmapsetEventKudosuRecalculate',
-        BeatmapsetEventType.DISCUSSION_LOCK: 'BeatmapsetEventDiscussionLock',
-        BeatmapsetEventType.NOMINATION_RESET: 'BeatmapsetEventNominationReset',
-        BeatmapsetEventType.NOMINATION_RESET_RECEIVED: 'BeatmapsetEventNominationResetReceived',
-        BeatmapsetEventType.GENRE_EDIT: 'BeatmapsetEventGenreEdit',
-        BeatmapsetEventType.LANGUAGE_EDIT: 'BeatmapsetEventLanguageEdit',
-        BeatmapsetEventType.NSFW_TOGGLE: 'BeatmapsetEventNsfwToggle',
-        BeatmapsetEventType.OFFSET_EDIT: 'BeatmapsetEventOffsetEdit',
-        BeatmapsetEventType.BEATMAP_OWNER_CHANGE: 'BeatmapsetEventBeatmapOwnerChange',
-    }
-
-    def __init__(self, data, type):
-        self.beatmap_discussion_id = data.get('beatmap_discussion_id')
-        self.beatmap_discussion_post_id = data.get('beatmap_discussion_post_id')
-        self.event_data = globals()[self.event_types[type]](data) if type in self.event_types else None
+
+    def __init__(self, data):
+        self.id: int = data["id"]
+        self.type: BeatmapsetEventType = BeatmapsetEventType(data["type"])
+        self.comment: Optional[BeatmapsetEventComment] = data["comment"]
+        if self.comment is not None:
+            self.comment = BeatmapsetEventComment(self.comment, self.type)  # type: ignore
+        self.created_at: datetime = parser.parse(data["created_at"])
+        self.user_id: Optional[int] = data.get("user_id")
+        self.beatmapset: Optional[BeatmapsetCompact] = (
+            BeatmapsetCompact(data["beatmapset"]) if data.get("beatmapset") is not None else None
+        )
+        self.discussion: Optional[BeatmapsetDiscussion] = (
+            BeatmapsetDiscussion(data["discussion"]) if data.get("discussion") is not None else None
+        )
 
     def __repr__(self):
-        return prettify(self, 'beatmap_discussion_id', 'beatmap_discussion_post_id')
+        return prettify(self, "type", "beatmapset")
 
 
 class BeatmapsetEventNominate:
     """
     **Attributes**
 
-    modes: Sequence[:class:`GameModeStr`]
+    modes: List[:class:`GameModeStr`]
     """
+
     __slots__ = ("modes",)
 
     def __init__(self, data):
-        self.modes = [GameModeStr(mode) for mode in data['modes']]
+        self.modes: List[GameModeStr] = list(map(GameModeStr, data["modes"]))
 
     def __repr__(self):
-        return prettify(self, 'modes')
+        return prettify(self, "modes")
 
 
 class BeatmapsetEventRemoveFromLoved:
     """
     **Attributes**
 
     reason: :class:`str`
     """
+
     __slots__ = ("reason",)
 
     def __init__(self, data):
-        self.reason = data['reason']
+        self.reason: str = data["reason"]
 
     def __repr__(self):
-        return prettify(self, 'reason')
+        return prettify(self, "reason")
 
 
 class BeatmapsetEventDisqualify:
     """
     **Attributes**
 
-    nominator_ids: Sequence[:class:`int`]
+    nominator_ids: List[:class:`int`]
     """
+
     __slots__ = ("nominator_ids",)
 
     def __init__(self, data):
-        self.nominator_ids = data['nominator_ids']
+        self.nominator_ids: List[int] = data["nominator_ids"]
 
     def __repr__(self):
-        return prettify(self, 'nominator_ids')
+        return prettify(self, "nominator_ids")
 
 
 class BeatmapsetEventVote:
     """
     **Attributes**
 
     user_id: :class:`int`
 
     score: :class:`int`
     """
+
     __slots__ = ("user_id", "score")
 
     def __init__(self, data):
-        self.user_id = data['user_id']
-        self.score = data['score']
+        self.user_id: int = data["user_id"]
+        self.score: int = data["score"]
 
     def __repr__(self):
-        return prettify(self, 'user_id', 'score')
+        return prettify(self, "user_id", "score")
 
 
 class BeatmapsetEventKudosuChange:
     """
     **Attributes**
 
-    new_votes: Union[:class:`BeatmapsetEventVote`, :class:`NoneType`]
+    new_votes: Optional[:class:`BeatmapsetEventVote`]
 
-    votes: Union[Sequence[:class:`BeatmapsetEventVote`], :class:`NoneType`]
+    votes: Optional[List[:class:`BeatmapsetEventVote`]]
     """
+
     __slots__ = ("new_votes", "votes")
 
     def __init__(self, data):
-        self.new_votes = BeatmapsetEventVote(data['new_votes']) if data.get('new_votes') is not None else None
-        self.votes = list(map(BeatmapsetEventVote, data['votes'])) if data.get('votes') is not None else None
+        self.new_votes: Optional[BeatmapsetEventVote] = (
+            BeatmapsetEventVote(data["new_votes"]) if data.get("new_votes") is not None else None
+        )
+        self.votes: Optional[List[BeatmapsetEventVote]] = (
+            list(map(BeatmapsetEventVote, data["votes"])) if data.get("votes") is not None else None
+        )
 
     def __repr__(self):
-        return prettify(self, 'new_votes', 'votes')
+        return prettify(self, "new_votes", "votes")
 
 
 class BeatmapsetEventKudosuGain(BeatmapsetEventKudosuChange):
     __doc__ = BeatmapsetEventKudosuChange.__doc__
 
 
 class BeatmapsetEventKudosuLost(BeatmapsetEventKudosuChange):
     __doc__ = BeatmapsetEventKudosuChange.__doc__
 
 
 class BeatmapsetEventKudosuRecalculate:
     """
     **Attributes**
 
-    new_votes: Union[:class:`BeatmapsetEventVote`, :class:`NoneType`]
+    new_votes: Optional[:class:`BeatmapsetEventVote`]
     """
+
     __slots__ = ("new_votes",)
 
     def __init__(self, data):
-        self.new_votes = BeatmapsetEventVote(data['new_votes']) if data.get('new_votes') is not None else None
+        self.new_votes: Optional[BeatmapsetEventVote] = (
+            BeatmapsetEventVote(data["new_votes"]) if data.get("new_votes") is not None else None
+        )
 
     def __repr__(self):
-        return prettify(self, 'new_votes')
+        return prettify(self, "new_votes")
 
 
 class BeatmapsetEventDiscussionLock:
     """
     **Attributes**
 
     reason: :class:`str`
     """
+
     __slots__ = ("reason",)
 
     def __init__(self, data):
-        self.reason = data['reason']
+        self.reason: str = data["reason"]
 
     def __repr__(self):
-        return prettify(self, 'reason')
+        return prettify(self, "reason")
 
 
 class BeatmapsetEventNominationReset:
     """
     **Attributes**
 
-    nominator_ids: Sequence[:class:`int`]
+    nominator_ids: List[:class:`int`]
     """
+
     __slots__ = ("nominator_ids",)
 
     def __init__(self, data):
-        self.nominator_ids = data['nominator_ids']
+        self.nominator_ids: List[int] = data["nominator_ids"]
 
     def __repr__(self):
-        return prettify(self, 'nominator_ids')
+        return prettify(self, "nominator_ids")
 
 
 class BeatmapsetEventNominationResetReceived:
     """
     **Attributes**
 
     source_user_id: :class:`int`
 
     source_user_name: :class:`str`
     """
+
     __slots__ = ("source_user_id", "source_user_username")
 
     def __init__(self, data):
-        self.source_user_id = data['source_user_id']
-        self.source_user_username = data['source_user_username']
+        self.source_user_id: int = data["source_user_id"]
+        self.source_user_username: str = data["source_user_username"]
 
     def __repr__(self):
-        return prettify(self, 'source_user_id', 'source_user_username')
+        return prettify(self, "source_user_id", "source_user_username")
 
 
 class BeatmapsetEventEdit:
     """
     **Attributes**
 
     old: :class:`str`
 
     new: :class:`str`
     """
+
     __slots__ = ("old", "new")
 
     def __init__(self, data):
-        self.old = data['old']
-        self.new = data['new']
+        self.old: str = data["old"]
+        self.new: str = data["new"]
 
     def __repr__(self):
-        return prettify(self, 'old', 'new')
+        return prettify(self, "old", "new")
 
 
 class BeatmapsetEventGenreEdit(BeatmapsetEventEdit):
     __doc__ = BeatmapsetEventEdit.__doc__
 
 
 class BeatmapsetEventLanguageEdit(BeatmapsetEventEdit):
     __doc__ = BeatmapsetEventEdit.__doc__
 
 
 class BeatmapsetEventNsfwToggle(BeatmapsetEventEdit):
-    """
-    **Attributes**
-
-    old: :class:`bool`
-
-    new: :class:`bool`
-    """
+    __doc__ = BeatmapsetEventEdit.__doc__
 
 
 class BeatmapsetEventOffsetEdit(BeatmapsetEventEdit):
-    """
-    **Attributes**
-
-    old: :class:`int`
-
-    new: :class:`int`
-    """
+    __doc__ = BeatmapsetEventEdit.__doc__
 
 
 class BeatmapsetEventBeatmapOwnerChange:
     """
     **Attributes**
 
     beatmap_id: :class:`int`
 
     beatmap_version: :class:`str`
 
     new_user_id: :class:`int`
 
     new_user_username: :class:`str`
     """
+
     __slots__ = ("beatmap_id", "beatmap_version", "new_user_id", "new_user_username")
 
     def __init__(self, data):
-        self.beatmap_id = data['beatmap_id']
-        self.beatmap_version = data['beatmap_version']
-        self.new_user_id = data['new_user_id']
-        self.new_user_username = data['new_user_username']
+        self.beatmap_id: int = data["beatmap_id"]
+        self.beatmap_version: str = data["beatmap_version"]
+        self.new_user_id: int = data["new_user_id"]
+        self.new_user_username: str = data["new_user_username"]
+
+    def __repr__(self):
+        return prettify(self, "beatmap_id", "new_user_username")
+
+
+_EVENT_TYPES = {
+    BeatmapsetEventType.NOMINATE: BeatmapsetEventNominate,
+    BeatmapsetEventType.REMOVE_FROM_LOVED: BeatmapsetEventRemoveFromLoved,
+    BeatmapsetEventType.DISQUALIFY: BeatmapsetEventDisqualify,
+    BeatmapsetEventType.KUDOSU_GAIN: BeatmapsetEventKudosuGain,
+    BeatmapsetEventType.KUDOSU_LOST: BeatmapsetEventKudosuLost,
+    BeatmapsetEventType.KUDOSU_RECALCULATE: BeatmapsetEventKudosuRecalculate,
+    BeatmapsetEventType.DISCUSSION_LOCK: BeatmapsetEventDiscussionLock,
+    BeatmapsetEventType.NOMINATION_RESET: BeatmapsetEventNominationReset,
+    BeatmapsetEventType.NOMINATION_RESET_RECEIVED: BeatmapsetEventNominationResetReceived,
+    BeatmapsetEventType.GENRE_EDIT: BeatmapsetEventGenreEdit,
+    BeatmapsetEventType.LANGUAGE_EDIT: BeatmapsetEventLanguageEdit,
+    BeatmapsetEventType.NSFW_TOGGLE: BeatmapsetEventNsfwToggle,
+    BeatmapsetEventType.OFFSET_EDIT: BeatmapsetEventOffsetEdit,
+    BeatmapsetEventType.BEATMAP_OWNER_CHANGE: BeatmapsetEventBeatmapOwnerChange,
+}
 
-    def __repr__(self):
-        return prettify(self, 'beatmap_id', 'new_user_username')
+
+def _get_event_data_object(data, type):
+    return _EVENT_TYPES[type](data) if type in _EVENT_TYPES else None
```

### Comparing `osu.py-0.6.0/osu/objects/discussion.py` & `osu.py-1.0.0/osu/objects/current_user_attributes.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,173 +1,185 @@
-from .user import CurrentUserAttributes
-from .beatmap import BeatmapCompact, BeatmapsetCompact
-from dateutil import parser
+from typing import Optional, Dict
 
-from ..util import prettify
+from ..util import prettify, get_optional
+from ..enums import ObjectType, GameModeStr
 
 
-class BeatmapsetDiscussion:
+class BeatmapsetDiscussionPermissions:
     """
-    Represents a Beatmapset modding discussion
+    A user's permissions in a beatmapset discussion
 
     **Attributes**
 
-    beatmap: :class:`BeatmapCompact` or :class:`NoneType`
+    can_destroy: :class:`bool`
 
-    beatmap_id: :class:`int` or :class:`NoneType`
+    can_reopen: :class:`bool`
 
-    beatmapset: :class:`BeatmapsetCompact` or :class:`NoneType`
+    can_moderate_kudosu: :class:`bool`
 
-    beatmapset_id: :class:`int`
+    can_resolve: :class:`bool`
 
-    can_be_resolved: :class:`bool`
+    vote_score: :class:`int`
+    """
 
-    can_grant_kudosu: :class:`bool`
+    __slots__ = (
+        "can_destroy",
+        "can_reopen",
+        "can_moderate_kudosu",
+        "can_resolve",
+        "vote_score",
+    )
+
+    def __init__(self, data):
+        self.can_destroy: bool = data["can_destroy"]
+        self.can_reopen: bool = data["can_reopen"]
+        self.can_moderate_kudosu: bool = data["can_moderate_kudosu"]
+        self.can_resolve: bool = data["can_resolve"]
+        self.vote_score: int = data["vote_score"]
 
-    created_at: :class:`datetime.datetime`
+    def __repr__(self):
+        return prettify(self, "vote_score")
+
+
+class BeatmapsetPermissions:
+    """
+    User permissions on a beatmapset
 
-    current_user_attributes: :class:`CurrentUserAttributes`
+    **Attributes**
 
-    deleted_at: :class:`datetime.datetime` or :class:`NoneType`
+    can_beatmap_update_owner: :class:`bool`
 
-    deleted_by_id: :class:`int`
+    can_delete: :class:`bool`
 
-    id: :class:`int`
+    can_edit_metadata: :class:`bool`
 
-    kudosu_denied: :class:`bool`
+    can_edit_offset: :class:`bool`
 
-    last_post_at: :class:`datetime.datetime`
+    can_edit_tags: :class:`bool`
 
-    message_type: :class:`str`
-        can be any of the following: hype, mapper_note, praise, problem, review, suggestion
+    can_hype: :class:`bool`
 
-    parent_id: :class:`int` or :class:`NoneType`
+    can_hype_reason: :class:`str`
 
-    posts: :class:`list`
-        list contains objects of type :class:`BeatmapsetDiscussionPost`
+    can_love: :class:`bool`
 
-    resolved: :class:`bool`
+    can_remove_from_loved: :class:`bool`
 
-    starting_post: :class:`BeatmapsetDiscussionPost`
+    is_watching: :class:`bool`
 
-    timestamp: :class:`int` or :class:`NoneType`
+    new_hype_time: Optional[:class:`str`]
 
-    updated_at: :class:`datetime.datetime`
+    nomination_modes: Dict[:class:`GameModeStr`, :class:`str`]
+        Values are either "full" or "limited".
 
-    user_id: :class:`int`
+    remaining_hype: :class:`int`
     """
+
     __slots__ = (
-        "beatmap", "beatmap_id", "beatmapset", "beatmapset_id", "can_be_resolved", "can_grant_kudosu",
-        "created_at", "current_user_attributes", "deleted_at", "deleted_by_id", "id", "kudosu_denied",
-        "last_post_at", "message_type", "parent_id", "posts", "resolved", "starting_post", "timestamp",
-        "updated_at", "user_id", "votes"
+        "can_beatmap_update_owner",
+        "can_delete",
+        "can_edit_metadata",
+        "can_edit_offset",
+        "can_edit_tags",
+        "can_hype",
+        "can_hype_reason",
+        "can_love",
+        "can_remove_from_loved",
+        "is_watching",
+        "new_hype_time",
+        "nomination_modes",
+        "remaining_hype",
     )
 
     def __init__(self, data):
-        self.beatmap = BeatmapCompact(data['beatmap']) if data.get('beatmap') is not None else None
-        self.beatmap_id = data['beatmap_id']
-        self.beatmapset = BeatmapsetCompact(data['beatmapset']) if data.get('beatmapset') is not None else None
-        self.beatmapset_id = data['beatmapset_id']
-        self.can_be_resolved = data['can_be_resolved']
-        self.can_grant_kudosu = data['can_grant_kudosu']
-        self.created_at = parser.parse(data['created_at'])
-        self.current_user_attributes = CurrentUserAttributes(data['current_user_attributes'],
-                                                             'BeatmapsetDiscussionPermissions') \
-            if 'current_user_attributes' in data else None
-        self.deleted_at = parser.parse(data['deleted_at']) if data['deleted_at'] is not None else None
-        self.deleted_by_id = data['deleted_by_id'] if 'deleted_by_id' in data else None
-        self.id = data['id']
-        self.kudosu_denied = data['kudosu_denied']
-        self.last_post_at = parser.parse(data['last_post_at'])
-        self.message_type = data['message_type']
-        self.parent_id = data['parent_id'] if 'parent_id' in data else None
-        self.posts = list(map(BeatmapsetDiscussionPost, data['posts'])) if 'posts' in data else None
-        self.resolved = data['resolved']
-        self.starting_post = BeatmapsetDiscussionPost(data['starting_post']) if 'starting_post' in data else None
-        self.timestamp = data['timestamp'] if 'timestamp' in data else None
-        self.updated_at = parser.parse(data['updated_at'])
-        self.user_id = data['user_id']
+        self.can_beatmap_update_owner: bool = data["can_beatmap_update_owner"]
+        self.can_delete: bool = data["can_delete"]
+        self.can_edit_metadata: bool = data["can_edit_metadata"]
+        self.can_edit_offset: bool = data["can_edit_offset"]
+        self.can_edit_tags: bool = data["can_edit_tags"]
+        self.can_hype: bool = data["can_hype"]
+        self.can_hype_reason: str = data["can_hype_reason"]
+        self.can_love: bool = data["can_love"]
+        self.can_remove_from_loved: bool = data["can_remove_from_loved"]
+        self.is_watching: bool = data["is_watching"]
+        self.new_hype_time: Optional[str] = data["new_hype_time"]
+        self.nomination_modes: Dict[GameModeStr, str] = get_optional(
+            data,
+            "nomination_modes",
+            lambda value: dict(map(lambda item: (GameModeStr(item[0]), item[1]), value.items())),
+        )
+        self.remaining_hype: int = data["remaining_hype"]
 
-    def __repr__(self):
-        return prettify(self, 'beatmapset', 'starting_post')
 
-
-class BeatmapsetDiscussionPost:
+class ChatChannelUserAttributes:
     """
-    Represents a post in a :class:`BeatmapsetDiscussion`.
+    Data about a user related to a chat channel.
 
     **Attributes**
 
-    beatmapset_discussion_id: :class:`int`
+    can_message: :class:`bool`
 
-    created_at: :class:`datetime.datetime`
+    can_message_error: Optional[:class:`str`]
 
-    deleted_at: :class:`datetime.datetime` or :class:`NoneType`
+    last_read_id: Optional[:class:`int`]
+    """
 
-    deleted_by_id: :class:`int` or :class:`NoneType`
+    __slots__ = ("can_message", "can_message_error", "last_read_id")
 
-    id: :class:`int`
+    def __init__(self, data):
+        self.can_message: bool = data["can_message"]
+        self.can_message_error: Optional[str] = data["can_message_error"]
+        self.last_read_id: Optional[int] = data["last_read_id"]
 
-    last_editor_id: :class:`int` or :class:`NoneType`
+    def __repr__(self):
+        return prettify(self, "can_message", "last_read_id")
 
-    message: :class:`str`
 
-    system: :class:`bool`
+class ScoreUserAttributes:
+    """
+    Gives info about a score related to the current user
 
-    updated_at: :class:`datetime.datetime`
+    **Attributes**
 
-    user_id: :class:`int`
+    Optional[:class:`CurrentUserPin`]
     """
-    __slots__ = (
-        "beatmapset_discussion_id", "created_at", "deleted_at", "deleted_by_id", "id",
-        "last_editor_id", "message", "system", "updated_at", "user_id"
-    )
 
-    def __init__(self, data):
-        self.beatmapset_discussion_id = data['beatmapset_discussion_id']
-        self.created_at = parser.parse(data['created_at'])
-        self.deleted_at = parser.parse(data['deleted_at']) if data['deleted_at'] is not None else None
-        self.deleted_by_id = data['deleted_by_id']
-        self.id = data['id']
-        self.last_editor_id = data['last_editor_id']
-        self.message = data['message']
-        self.system = data['system']
-        self.updated_at = parser.parse(data['updated_at'])
-        self.user_id = data['user_id']
+    __slots__ = ("pin",)
 
-    def __repr__(self):
-        return prettify(self, 'user_id', 'message', 'beatmapset_discussion_id')
+    def __init__(self, data):
+        self.pin: Optional[CurrentUserPin] = get_optional(data, "pin", CurrentUserPin)
 
 
-class BeatmapsetDiscussionVote:
+class CurrentUserPin:
     """
-    Represents a vote on a :class:`BeatmapsetDiscussion`.
+    Gives info about a score related to if it's pinned or not
 
     **Attributes**
 
-    beatmapset_discussion_id: :class:`int`
+    is_pinned: :class:`bool`
 
-    created_at: :class:`datetime.datetime`
+    score_id: :class:`int`
 
-    id: :class:`int`
+    score_type: :class:`ObjectType`
+    """
+
+    __slots__ = ("is_pinned", "score_id", "score_type")
 
-    score: :class:`int`
+    def __init__(self, data):
+        self.is_pinned: bool = data["is_pinned"]
+        self.score_id: int = data["score_id"]
+        self.score_type: ObjectType = ObjectType(data["score_type"])
 
-    updated_at: :class:`datetime.datetime`
 
-    user_id: :class:`int`
+class CommentableMetaAttributes:
     """
-    __slots__ = (
-        "beatmapset_discussion_id", "created_at", "id", "score",
-        "updated_at", "user_id"
-    )
+    User attributes for a :class:`CommentableMeta` object
 
-    def __init__(self, data):
-        self.beatmapset_discussion_id = data['beatmapset_discussion_id']
-        self.created_at = parser.parse(data['created_at'])
-        self.id = data['id']
-        self.score = data['score']
-        self.updated_at = parser.parse(data['updated_at'])
-        self.user_id = data['user_id']
+    **Attributes**
 
-    def __repr__(self):
-        return prettify(self, 'beatmapset_discussion_id', 'score', 'user_id')
+    can_new_comment_reason: Optional[:class:`str`]
+    """
+
+    __slots__ = ("can_new_comment_reason",)
+
+    def __init__(self, data):
+        self.can_new_comment_reason = data["can_new_comment_reason"]
```

### Comparing `osu.py-0.6.0/osu/objects/group.py` & `osu.py-1.0.0/osu/objects/kudosu.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,91 +1,86 @@
-from ..util import prettify
+from dateutil import parser
+from typing import Optional, TYPE_CHECKING
 
+from ..util import prettify, get_optional
+from ..enums import KudosuAction, ObjectType
 
-class Group:
-    """
-    This object isn't returned by any endpoints yet, it is here purely as a reference for :class:`UserGroup`
-
-    **Attributes**
 
-    id: :class:`int`
+if TYPE_CHECKING:
+    from datetime import datetime
 
-    identifier: :class:`str`
-        Unique string to identify the group.
 
-    is_probationary: :class:`str`
-        Whether members of this group are considered probationary.
+class KudosuHistory:
+    """
+    **Attributes**
 
-    has_playmodes: :class:`bool`
-        If this group associates GameModes with a user's membership, e.g. BN/NAT members
+    id: :class:`int`
 
-    has_listing: :class:`bool`
-        Whether this group displays a listing at /groups/{id}
+    action: :class:`KudosuAction`
 
-    name: :class:`str`
+    amount: :class:`int`
 
-    short_name: :class:`str`
-        Short name of the group for display.
+    model: :class:`ObjectType`
+        Object type which the exchange happened on (forum_post, etc).
 
-    colour: :class:`str` or :class:`NoneType`
+    created_at: :class:`datetime.datetime`
 
-    **Optional Attributes**
+    giver: Optional[:class:`KudosuGiver`]
+        Simple detail of the user who started the exchange.
 
-    description: :class:`Description` or :class:`NoneType`
-        A dictionary with keys html and markdown.
+    post: :class:`KudosuPost`
+        Simple detail of the object for display.
     """
-    __slots__ = (
-        "id", "identifier", "is_probationary", "has_playmodes", "has_listing",
-        "name", "short_name", "colour", "description"
-    )
+
+    __slots__ = ("id", "action", "amount", "model", "created_at", "giver", "post")
 
     def __init__(self, data):
-        self.id = data['id']
-        self.identifier = data['identifier']
-        self.is_probationary = data['is_probationary']
-        self.has_playmodes = data['has_playmodes']
-        self.name = data['name']
-        self.short_name = data['short_name']
-        self.colour = data['colour']
-        self.description = Description(data['description']) if data.get('description') is not None else None
+        self.id: int = data["id"]
+        self.action: KudosuAction = KudosuAction(data["action"])
+        self.amount: int = data["amount"]
+        self.model: ObjectType = ObjectType(data["model"])
+        self.created_at: datetime = parser.parse(data["created_at"])
+        self.giver: Optional[KudosuGiver] = get_optional(data, "giver", KudosuGiver)
+        self.post: KudosuPost = KudosuPost(data["post"])
 
     def __repr__(self):
-        return prettify(self, 'name')
+        return prettify(self, "action", "amount", "giver")
 
 
-class Description:
+class KudosuPost:
     """
     **Attributes**
 
-    html: :class:`str`
+    url: Optional[:class:`str`]
+        Url of the object.
 
-    markdown: :class:`str`
+    title: :class:`str`
+        Title of the object. It'll be "[deleted beatmap]" for deleted beatmaps.
     """
 
+    __slots__ = ("url", "title")
+
     def __init__(self, data):
-        self.html = data['html']
-        self.markdown = data['markdown']
+        self.url: Optional[str] = data["url"]
+        self.title: str = data["title"]
 
     def __repr__(self):
-        return prettify(self)
+        return prettify(self, "title")
 
 
-class UserGroup(Group):
+class KudosuGiver:
     """
-    Describes the :class:`Group` membership of a :class:`User`.
-    It contains all of the attributes of the :class:`Group`, in addition to what is listed here.
-
     **Attributes**
 
-    playmodes: Sequence[:class:`str`]
-        GameModes associated with this membership (null if has_playmodes is unset).
+    url: :class:`str`
+
+    username: :class:`str`
     """
-    __slots__ = (
-        "playmodes",
-    )
+
+    __slots__ = ("url", "username")
 
     def __init__(self, data):
-        super().__init__(data)
-        self.playmodes = data['playmodes']
+        self.url: str = data["url"]
+        self.username: str = data["username"]
 
     def __repr__(self):
-        return super().__repr__()
+        return prettify(self, "username")
```

### Comparing `osu.py-0.6.0/osu/objects/kudosu.py` & `osu.py-1.0.0/osu/objects/wiki.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,84 +1,85 @@
-from dateutil import parser
+from typing import List, Optional, Union, TYPE_CHECKING
 
 from ..util import prettify
 
 
-class KudosuHistory:
-    """
-    **Attributes**
+if TYPE_CHECKING:
+    from .user import UserCompact
 
-    id: :class:`int`
 
-    action: :class:`str`
-        One of give, vote.give, reset, vote.reset, revoke, or vote.revoke.
+class WikiPage:
+    """
+    Represents a wiki article
 
-    amount: :class:`int`
+    **Attributes**
 
-    model: :class:`str`
-        Object type which the exchange happened on (forum_post, etc).
+    available_locales: List[:class:`str`]
+        All available locales for the article.
 
-    created_at: :class:`datetime.datetime`
+    layout: :class:`str`
+        The layout type for the page.
 
-    giver: :class:`Giver` or :class:`NoneType`
-        Simple detail of the user who started the exchange.
+    locale: :class:`str`
+        All lowercase BCP 47 language tag.
 
-    post: :class:`Post`
-        Simple detail of the object for display.
-    """
-    __slots__ = (
-        "id", "action", "amount", "model", "created_at", "giver", "post"
-    )
+    markdown: :class:`str`
+        Markdown content.
 
-    def __init__(self, data):
-        self.id = data['id']
-        self.action = data['action']
-        self.amount = data['amount']
-        self.model = data['model']
-        self.created_at = parser.parse(data['created_at'])
-        self.giver = Giver(data['giver']) if data.get('giver') else None
-        self.post = Post(data['post'])
+    path: :class:`str`
+        Path of the article.
 
-    def __repr__(self):
-        return prettify(self, 'action', 'amount', 'giver')
+    subtitle: Optional[:class:`str`]
+        The article's subtitle.
 
-
-class Post:
-    """
-    **Attributes**
-
-    url: :class:`str` or :class:`NoneType`
-        Url of the object.
+    tags: List[:class:`str`]
+        Associated tags for the article.
 
     title: :class:`str`
-        Title of the object. It'll be "[deleted beatmap]" for deleted beatmaps.
+        The article's title.
     """
+
     __slots__ = (
-        "url", "title"
+        "available_locales",
+        "layout",
+        "locale",
+        "markdown",
+        "path",
+        "subtitle",
+        "tags",
+        "title",
     )
 
     def __init__(self, data):
-        self.url = data['url']
-        self.title = data['title']
+        self.available_locales: List[str] = data["available_locales"]
+        self.layout: str = data["layout"]
+        self.locale: str = data["locale"]
+        self.markdown: str = data["markdown"]
+        self.path: str = data["path"]
+        self.subtitle: Optional[str] = data["subtitle"]
+        self.tags: List[str] = data["tags"]
+        self.title: str = data["title"]
 
     def __repr__(self):
-        return prettify(self, 'title')
+        return prettify(self, "title")
 
 
-class Giver:
+class SearchResults:
     """
+    Represents the results of a search.
+
     **Attributes**
 
-    url: :class:`str`
+    results: List[Union[:class:`UserCompact`, :class:`WikiPage`]]
+        type depends on search type
 
-    username: :class:`str`
+    total: :class:`int`
     """
-    __slots__ = (
-        "url", "username"
-    )
 
-    def __init__(self, data):
-        self.url = data['url']
-        self.username = data['username']
+    __slots__ = ("results", "total")
+
+    def __init__(self, data, data_type):
+        self.results: List[Union[UserCompact, WikiPage]] = list(map(data_type, data["data"]))
+        self.total: int = data["total"]
 
     def __repr__(self):
-        return prettify(self, 'username')
+        return prettify(self, "results", "total")
```

### Comparing `osu.py-0.6.0/osu/objects/match.py` & `osu.py-1.0.0/osu/objects/ranking.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,78 +1,111 @@
 from dateutil import parser
-from .user import UserCompact
-from ..enums import MatchEventType
-from ..util import prettify
+from typing import Dict, Optional, List, TYPE_CHECKING
 
+from .beatmap import Beatmapset
+from .user import UserStatistics
+from ..util import prettify, get_optional, get_optional_list
 
-class Match:
-    __slots__ = ("id", "start_time", "end_time", "name")
 
-    def __init__(self, data):
-        self.id = data['id']
-        self.name = data['name']
-        self.start_time = parser.parse(data['start_time']) if data['start_time'] is not None else None
-        self.end_time = parser.parse(data['end_time']) if data['end_time'] is not None else None
-
-    def __repr__(self):
-        return prettify(self, 'name', 'start_time')
+if TYPE_CHECKING:
+    from datetime import datetime
 
 
-class MatchExtended(Match):
+class Rankings:
     """
-    Extended version of :class:`Match` that is relevant at the :func:`osu.Client.get_match` endpoint.
-
     **Attributes**
 
-    events: Sequence[:class:`MatchEvent`]
-        List of events that occurred in the match.
+    beatmapsets: Optional[List[:class:`Beatmapset`]]
+        The list of beatmaps in the requested spotlight for the given mode;
+        only available if type is charts
 
-    users: Sequence[:class:`UserCompact`]
+    cursor: Dict
+        To be used to query the next page
 
-    first_event_id: :class:`int`
+    ranking: List[:class:`UserStatistics`]
+        Score details ordered by rank in descending order.
 
-    latest_event_id: :class:`int`
+    spotlight: Optional[:class:`Spotlight`]
+        Spotlight details; only available if type is charts
 
-    current_game_id: :class:`int`
+    total: :class:`int`
+        An approximate count of ranks available
     """
-    __slots__ = Match.__slots__ + (
-        "events", "users", "first_event_id", "latest_event_id", "current_game_id"
-    )
+
+    __slots__ = ("beatmapsets", "cursor", "ranking", "spotlight", "total")
 
     def __init__(self, data):
-        super().__init__(data["match"])
-        self.events = list(map(MatchEvent, data['events']))
-        self.users = list(map(UserCompact, data['users']))
-        self.first_event_id = data['first_event_id']
-        self.latest_event_id = data['latest_event_id']
-        self.current_game_id = data['current_game_id']
+        self.cursor: Dict = data["cursor"]
+        self.ranking: List[UserStatistics] = list(map(UserStatistics, data["ranking"]))
+        self.total: int = data["total"]
+        self.spotlight: Optional[Spotlight] = get_optional(data, "spotlight", Spotlight)
+        self.beatmapsets: Optional[List[Beatmapset]] = get_optional_list(data, "beatmapsets", Beatmapset)
+
+    def __repr__(self):
+        return prettify(self, "ranking")
 
 
-class MatchEvent:
+class Spotlight:
     """
-    An event that occurred in a match.
+    The details of a spotlight.
 
     **Attributes**
 
+    end_date: :class:`datetime.datetime`
+        In DateTime format. The end date of the spotlight.
+
     id: :class:`int`
+        The ID of this spotlight.
 
-    timestamp: :class:`datetime.datetime`
+    mode_specific: :class:`bool`
+        If the spotlight has different modes specific to each game mode.
 
-    user_id: :class:`int`
+    participant_count: Optional[:class:`int`]
+        The number of users participating in this spotlight. This is only shown when viewing a single spotlight.
 
-    type: :class:`MatchEventType`
+    name: :class:`str`
+        The name of the spotlight.
 
-    text: Union[:class:`str`, :class:`NoneType`]
-        None unless the event type is :class:`MatchEventType`.OTHER
+    start_date: :class:`datetime.datetime`
+        In DatTime format. The starting date of the spotlight.
+
+    type: :class:`str`
+        The type of spotlight.
     """
-    __slots__ = ("id", "timestamp", "user_id", "type", "text")
+
+    __slots__ = (
+        "end_date",
+        "id",
+        "mode_specific",
+        "name",
+        "start_date",
+        "type",
+        "participant_count",
+    )
+
+    def __init__(self, data):
+        self.end_date: datetime = parser.parse(data["end_date"])
+        self.id: int = data["id"]
+        self.mode_specific: bool = data["mode_specific"]
+        self.participant_count: Optional[int] = data.get("participant_count")
+        self.name: str = data["name"]
+        self.start_date: datetime = parser.parse(data["start_date"])
+        self.type: str = data["type"]
+
+    def __repr__(self):
+        return prettify(self, "name")
+
+
+class Spotlights:
+    """
+    **Attributes**
+
+    spotlights: List[:class:`Spotlight`]
+    """
+
+    __slots__ = ("spotlights",)
 
     def __init__(self, data):
-        self.id = data['id']
-        self.timestamp = parser.parse(data['timestamp'])
-        self.user_id = data['user_id']
-        self.type = MatchEventType(data['detail']['type'])
-        self.text = data['detail']['text'] if 'text' in data['detail'] else None
+        self.spotlights: List[Spotlight] = list(map(Spotlight, data["spotlights"]))
 
     def __repr__(self):
-        attributes = ('type',) if self.type != MatchEventType.OTHER else ('type', 'text')
-        return prettify(self, *attributes)
+        return prettify(self, "spotlights")
```

### Comparing `osu.py-0.6.0/osu/objects/multiplayer.py` & `osu.py-1.0.0/osu/objects/score.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,346 +1,462 @@
-from .user import UserCompact
-from .beatmap import BeatmapCompact
-from .score import ScoreDataStatistics, LazerMod
-from ..enums import RoomCategory, RoomType, RealTimeQueueMode, PlaylistQueueMode, GameModeInt, RealTimeType
-from ..util import prettify
 from dateutil import parser
+from typing import Optional, List, TYPE_CHECKING, Union, Dict
+
+from .beatmap import BeatmapCompact, BeatmapsetCompact
+from .user import UserCompact
+from .current_user_attributes import ScoreUserAttributes
+from ..enums import GameModeStr, GameModeInt, Mods, Mod, ObjectType, ScoreRank
+from ..util import prettify, get_optional_list, get_optional
 
 
-class MultiplayerScore:
+if TYPE_CHECKING:
+    from datetime import datetime
+
+
+class BeatmapScores:
     """
-    Score data.
+    Contains a list of scores as well as, possibly, a :class:`BeatmapUserScore` object.
 
     **Attributes**
 
-    id: :class:`int`
+    scores: List[Union[:class:`LegacyScore`, :class:`SoloScore`]]
+        The list of top scores for the beatmap in descending order.
 
-    user_id: :class:`int`
+    user_score: Optional[:class:`BeatmapUserScore`]
+        The score of the current user. This is not returned if the current user does not have a score.
+    """
 
-    room_id: :class:`int`
+    __slots__ = ("scores", "user_score")
 
-    playlist_item_id: :class:`int`
+    def __init__(self, data):
+        self.scores: List[Union[LegacyScore, SoloScore]] = list(map(get_score_object, data["scores"]))
+        var_name = "userScore" if "userScore" in data else "user_score"
+        self.user_score: Optional[BeatmapUserScore] = get_optional(data, var_name, BeatmapUserScore)
 
-    beatmap_id: :class:`int`
+    def __repr__(self):
+        return prettify(self, "user_score", "scores")
 
-    rank: :class:`str`
-        Can be one of the following: charts (Spotlight), country (Country), performance (Performance), score (Score)
 
-    total_score: :class:`int`
+class LegacyScore:
+    """
+    Contains information about a score
 
-    accuracy: :class:`int`
+    **Attributes**
 
-    max_combo: :class:`int`
+    id: :class:`int`
 
-    mods: Sequence[:class:`LazerMod`]
+    best_id: :class:`int`
 
-    statistics: :class:`ScoreDataStatistics`
+    user_id: :class:`int`
 
-    passed: :class:`bool`
+    accuracy: :class:`float`
 
-    position: :class:`int` or :class:`NoneType`
+    mods: :class:`Mods`
 
-    scores_around: :class:`MultiplayerScoresAround` or :class:`NoneType`
-        Scores around the specified score.
+    score: :class:`int`
 
-    user: :class:`User`
-    """
-    __slots__ = (
-        "id", "user_id", "room_id", "playlist_item_id", "beatmap_id", "rank",
-        "total_score", "accuracy", "max_combo", "mods", "statistics", "passed",
-        "position", "scores_around", "user"
-    )
+    max_combo: :class:`int`
 
-    def __init__(self, data):
-        self.id = data['id']
-        self.user_id = data['user_id']
-        self.room_id = data['room_id']
-        self.playlist_item_id = data['playlist_item_id']
-        self.beatmap_id = data['beatmap_id']
-        self.rank = data['rank']
-        self.total_score = data['total_score']
-        self.accuracy = data['accuracy']
-        self.max_combo = data['max_combo']
-        self.mods = list(map(LazerMod, data['mods'])) if data["mods"] is not None else []
-        self.statistics = ScoreDataStatistics(data['statistics'])
-        self.passed = data['passed']
-        self.position = data.get('position')
-        self.scores_around = MultiplayerScoresAround(data['scores_around']) \
-            if data.get('scores_around') is not None else None
-        self.user = UserCompact(data['user']) if data.get('user') is not None else None
+    perfect: :class:`bool`
 
-    def __repr__(self):
-        return prettify(self, 'user', 'position')
+    statistics: :class:`ScoreStatistics`
 
+    passed :class:`bool`
 
-class MultiplayerScores:
-    """
-    An object which contains scores and related data for fetching next page of the result.
-    To fetch the next page, make request to scores index (Client.get_scores) with relevant
-    room and playlist, use the data in attribute params and cursor to fill in the 3 other optional queries.
+    pp: :class:`float`
 
-    **Attributes**
+    rank: :class:`ScoreRank`
 
-    cursor: :class:`dict`
-        To be used to fetch the next page.
+    created_at: :class:`datetime.datetime`
 
-    params: :class:`dict`
-        To be used to fetch the next page.
+    mode: :class:`GameModeStr`
 
-    scores: Union[Sequence[:class:`MultiplayerScore`], :class:`None`]
+    mode_int: :class:`GameModeInt`
 
-    total: Union[:class:`int`, :class:`None`]
-        Index only. Total scores of the specified playlist item.
+    replay: :class:`bool`
+        is the replay is available
 
-    user_score: Union[:class:`MultiplayerScore`, :class:`None`]
-        Index only. Score of the accessing user if exists.
-    """
-    __slots__ = (
-        "cursor", "params", "scores", "total", "user_score"
-    )
+    beatmap: Optional[:class:`BeatmapCompact`]
 
-    def __init__(self, data):
-        self.cursor = data['cursor']
-        self.params = data['params']
-        self.scores = list(map(MultiplayerScore, data['scores'])) if data.get('scores') is not None else None
-        self.total = data.get('total')
-        self.user_score = MultiplayerScore(data['user_score']) if data.get('user_score') is not None else None
+    beatmapset: Optional[:class:`BeatmapsetCompact`]
 
-    def __repr__(self):
-        return prettify(self, 'total', 'scores')
+    rank_country: Optional[:class:`int`]
 
+    rank_global: Optional[:class:`int`]
 
-class MultiplayerScoresAround:
-    """
-    **Attributes**
+    weight: Optional[:class:`PpWeight`]
 
-    higher: :class:`MultiplayerScores`
+    user: Optional[:class:`UserCompact`]
 
-    lower: :class:`MultiplayerScores`
+    match: Optional[:class:`MatchGameScoreInfo`]
+
+    current_user_attributes: Optional[:class:`ScoreUserAttributes`]
     """
+
     __slots__ = (
-        "higher", "lower"
+        "id",
+        "best_id",
+        "user_id",
+        "accuracy",
+        "mods",
+        "score",
+        "max_combo",
+        "perfect",
+        "statistics",
+        "passed",
+        "pp",
+        "rank",
+        "created_at",
+        "mode",
+        "mode_int",
+        "replay",
+        "beatmap",
+        "beatmapset",
+        "rank_country",
+        "rank_global",
+        "weight",
+        "user",
+        "match",
+        "type",
+        "current_user_attributes",
     )
 
     def __init__(self, data):
-        self.higher = MultiplayerScores(data['higher'])
-        self.lower = MultiplayerScores(data['lower'])
+        self.id: int = data["id"]
+        self.best_id: int = data["best_id"]
+        self.user_id: int = data["user_id"]
+        self.accuracy: float = data["accuracy"]
+        self.mods: Mods = Mods.parse_any_list(data["mods"])
+        self.score: int = data["score"]
+        self.max_combo: int = data["max_combo"]
+        self.perfect: bool = data["perfect"]
+        self.statistics: ScoreStatistics = ScoreStatistics(data["statistics"])
+        self.passed: bool = data["passed"]
+        self.pp: float = data["pp"]
+        self.rank: ScoreRank = ScoreRank(data["rank"])
+        self.created_at: datetime = parser.parse(data["created_at"])
+        self.mode: GameModeStr = GameModeStr(data["mode"])
+        self.mode_int: GameModeInt = GameModeInt(data["mode_int"])
+        self.replay: bool = data["replay"]
+        self.type: ObjectType = ObjectType(data["type"])
+
+        from .match import MatchGameScoreInfo
+
+        self.beatmap: Optional[BeatmapCompact] = get_optional(data, "beatmap", BeatmapCompact)
+        self.beatmapset: Optional[BeatmapsetCompact] = get_optional(data, "beatmapset", BeatmapsetCompact)
+        self.user: Optional[UserCompact] = get_optional(data, "user", UserCompact)
+        self.match: Optional[MatchGameScoreInfo] = get_optional(data, "match", MatchGameScoreInfo)
+        self.rank_country: Optional[int] = data.get("rank_country")
+        self.rank_global: Optional[int] = data.get("rank_global")
+        self.weight: Optional[PpWeight] = get_optional(data, "weight", PpWeight)
+        self.current_user_attributes: Optional[ScoreUserAttributes] = get_optional(
+            data, "current_user_attributes", ScoreUserAttributes
+        )
 
     def __repr__(self):
-        return prettify(self, 'higher', 'lower')
+        return prettify(self, "user_id", "accuracy")
 
 
-class Room:
+class SoloScore:
     """
-    :func:`osu.Client.get_rooms` and :func:`osu.Client.get_room` endpoints include host, playlist,
-    and recent_participants attributes. In addition, the :class:`PlaylistItem` objects in playlist
-    include the beatmap attribute and the beatmap attribute has the beatmapset, checksum, and
-    max_combo attributes.
+    Contains information about a lazer score.
 
     **Attributes**
 
-    id: :class:`int`
+    accuracy: :class:`float`
 
-    name: :class:`str`
+    beatmap_id: Optional[:class:`int`]
 
-    category: :class:`RoomCategory`
+    ended_at: :class:`datetime.datetime`
 
-    type: :class:`RoomType`
+    max_combo: :class:`int`
 
-    realtime_type: :class:`RealTimeType`
-        Only applicable when type is RoomType.REALTIME
+    maximum_statistics: :class:`ScoreDataStatistics`
 
-    user_id: :class:`int`
+    mods: List[:class:`LazerMod`]
 
-    start_at: Union[:class:`datetime.datetime`, :class:`NoneType`]
+    passed: :class:`bool`
 
-    ends_at: Union[:class:`datetime.datetime`, :class:`NoneType`]
+    rank: :class:`ScoreRank`
 
-    max_attempts: :class:`int`
+    ruleset_id: :class:`int`
 
-    participant_count: :class:`int`
+    statistics: :class:`ScoreDataStatistics`
 
-    channel_id: :class:`int`
+    total_score: :class:`int`
 
-    active: :class:`bool`
+    user_id: :class:`int`
 
-    has_password: :class:`bool`
+    best_id: Optional[:class:`int`]
 
-    queue_mode: Union[:class:`RealTimeQueueMode`, :class:`PlaylistQueueMode`]
-        type depends on the room type. :class:`RealTimeQueueMode` for type :class:`RoomType`.REALTIME and
-        :class:`PlaylistQueueMode` for type :class:`RoomType`.PLAYLIST.
+    id: :class:`int`
 
-    current_playlist_item: Union[:class:`PlaylistItem`, :class:`NoneType`]
+    legacy_perfect: Optional[:class:`bool`]
 
-    current_user_score: Union[:class:`UserScoreAggregate`, :class:`NoneType`]
+    pp: Optional[:class:`float`]
 
-    difficulty_range: Union[Dict[:class:`str`, :class:`int`], :class:`NoneType`]
-        When not none, is a dictionary containing keys "max" and "min."
+    replay: :class:`bool`
 
-    host: Union[:class:`UserCompact`, :class:`NoneType`]
+    type: :class:`ObjectType`
 
-    playlist: Union[Sequence[:class:`PlaylistItem`], :class:`NoneType`]
+    user: Optional[:class:`UserCompact`]
 
-    playlist_item_stats: Union[:class:`PlaylistItemStats`, :class:`NoneType`]
+    build_id: Optional[:class:`int`]
 
-    recent_participants: Union[Sequence[:class:`UserCompact`], :class:`NoneType`]
+    legacy_score_id: Optional[:class:`int`]
 
-    scores: Union[:class:`MultiplayerScore`, :class:`NoneType`]
+    legacy_total_score: Optional[:class:`int`]
+
+    started_at: Optional[:class:`datetime.datetime`]
+
+    current_user_attributes: Optional[:class:`ScoreUserAttributes`]
+
+    weight: Optional[:class:`PpWeight`]
     """
+
     __slots__ = (
-        "id", "name", "category", "type", "user_id", "start_at", "ends_at", "max_attempts",
-        "participant_count", "channel_id", "active", "has_password", "queue_mode",
-        "current_playlist_item", "current_user_score", "difficulty_range", "host",
-        "playlist", "playlist_item_stats", "recent_participants", "scores",
-        "realtime_type"
+        "accuracy",
+        "beatmap_id",
+        "build_id",
+        "ended_at",
+        "legacy_score_id",
+        "legacy_total_score",
+        "max_combo",
+        "maximum_statistics",
+        "mods",
+        "passed",
+        "rank",
+        "ruleset_id",
+        "started_at",
+        "statistics",
+        "total_score",
+        "user_id",
+        "best_id",
+        "id",
+        "legacy_perfect",
+        "pp",
+        "replay",
+        "type",
+        "user",
+        "current_user_attributes",
+        "weight",
     )
 
     def __init__(self, data):
-        self.id = data['id']
-        self.name = data['name']
-        self.category = RoomCategory(data['category'])
-        self.type = RoomType.PLAYLISTS if data["type"] == "playlists" else RoomType.REALTIME
-        self.realtime_type = RealTimeType(data["type"]) if self.type == RoomType.REALTIME else None
-        self.user_id = data['user_id']
-        self.start_at = parser.parse(data['start_at']) if data.get('start_at') is not None else None
-        self.ends_at = parser.parse(data['ends_at']) if data.get('ends_at') is not None else None
-        self.max_attempts = data['max_attempts']
-        self.participant_count = data['participant_count']
-        self.channel_id = data['channel_id']
-        self.active = data['active']
-        self.has_password = data['has_password']
-        self.queue_mode = (RealTimeQueueMode if self.type == RoomType.REALTIME
-                           else PlaylistQueueMode)(data['queue_mode'])
-
-        self.current_playlist_item = PlaylistItem(data['current_playlist_item']) \
-            if data.get('current_playlist_item') is not None else None
-        self.current_user_score = UserScoreAggregate(data['current_user_score']) \
-            if data.get('current_user_score') is not None else None
-        self.difficulty_range = data.get('difficulty_range')  # {min, max}
-        self.host = UserCompact(data['host']) if data.get('host') is not None else None
-        self.playlist = list(map(PlaylistItem, data['playlist'])) if data.get('playlist') is not None else None
-        self.playlist_item_stats = PlaylistItemStats(data['playlist_item_stats']) \
-            if data.get('playlist_item_stats') is not None else None
-        self.recent_participants = list(map(UserCompact, data['recent_participants'])) \
-            if data.get('recent_participants') is not None else None
-        self.scores = list(map(MultiplayerScore, data['scores'])) if data.get('scores') is not None else None
+        self.accuracy: float = data["accuracy"]
+        self.beatmap_id: int = data["beatmap_id"]
+        self.ended_at: datetime = parser.parse(data["ended_at"])
+        self.max_combo: int = data["max_combo"]
+        self.maximum_statistics: ScoreDataStatistics = ScoreDataStatistics(data["maximum_statistics"])
+        self.mods: List[LazerMod] = list(map(LazerMod, data["mods"]))
+        self.passed: bool = data["passed"]
+        self.rank: ScoreRank = ScoreRank(data["rank"])
+        self.ruleset_id: int = data["ruleset_id"]
+        self.statistics: ScoreDataStatistics = ScoreDataStatistics(data["statistics"])
+        self.total_score: int = data["total_score"]
+        self.user_id: int = data["user_id"]
+        self.best_id: Optional[int] = data["best_id"]
+        self.id: int = data["id"]
+        self.legacy_perfect: Optional[bool] = data["legacy_perfect"]
+        self.pp: Optional[float] = data["pp"]
+        self.replay: bool = data["replay"]
+        self.type: ObjectType = ObjectType(data["type"])
+
+        self.user: Optional[UserCompact] = get_optional(data, "user", UserCompact)
+        self.build_id: Optional[int] = data.get("build_id")
+        self.legacy_score_id: Optional[int] = data.get("legacy_score_id")
+        self.legacy_total_score: Optional[int] = data.get("legacy_total_score")
+        self.started_at: Optional[datetime] = get_optional(data, "started_at", parser.parse)
+        self.current_user_attributes: Optional[ScoreUserAttributes] = get_optional(
+            data, "current_user_attributes", ScoreUserAttributes
+        )
+        self.weight: Optional[PpWeight] = get_optional(data, "weight", PpWeight)
 
     def __repr__(self):
-        return prettify(self, 'name', 'type')
+        return prettify(self, "beatmap_id", "statistics")
 
 
-class UserScoreAggregate:
+class PpWeight:
     """
+    Weighted pp info
+
     **Attributes**
 
-    accuracy: :class:`float`
+    percentage: :class:`int`
+        number (0-100) that tells percentage weighed
 
-    attempts: :class:`int`
+    pp: :class:`float`
+        amount of pp after being weighted
+    """
 
-    completed: :class:`int`
+    __slots__ = ("percentage", "pp")
 
-    pp: :class:`float`
+    def __init__(self, data):
+        self.percentage: float = data["percentage"]
+        self.pp: float = data["pp"]
 
-    room_id: :class:`int`
 
-    total_score: :class:`int`
+def get_score_object(data) -> Union[SoloScore, LegacyScore]:
+    # EAFP cuz type attribute is not reliable
+    try:
+        return SoloScore(data)
+    except KeyError:
+        return LegacyScore(data)
 
-    user_id: :class:`int`
 
-    playlist_item_attempts: Union[Dict[:class:`str`, :class:`int`], :class:`NoneType`]
-        contains keys "attempts" and "id."
+class ScoreStatistics:
+    """
+    **Attributes**
+
+    count_50: :class:`int`
+
+    count_100: :class:`int`
+
+    count_300: :class:`int`
+
+    count_geki: :class:`int`
 
-    position: Union[:class:`int`, :class:`NoneType`]
-        user rank
+    count_katu: :class:`int`
 
-    user: Union[:class:`UserCompact`, :class:`NoneType`]
+    count_miss: :class:`int`
     """
+
     __slots__ = (
-        "accuracy", "attempts", "completed", "pp", "room_id", "total_score",
-        "user_id", "playlist_item_attempts", "position", "user"
+        "count_50",
+        "count_100",
+        "count_300",
+        "count_geki",
+        "count_katu",
+        "count_miss",
     )
 
     def __init__(self, data):
-        self.accuracy = data['accuracy']
-        self.attempts = data['attempts']
-        self.completed = data['completed']
-        self.pp = data['pp']
-        self.room_id = data['room_id']
-        self.total_score = data['total_score']
-        self.user_id = data['user_id']
-        self.playlist_item_attempts = data.get('playlist_item_attempts')  # {attempts, id}
-        self.position = data.get('position')
-        self.user = UserCompact(data['user']) if data.get('user') is not None else None
+        self.count_50: int = data["count_50"]
+        self.count_100: int = data["count_100"]
+        self.count_300: int = data["count_300"]
+        self.count_geki: int = data["count_geki"]
+        self.count_katu: int = data["count_katu"]
+        self.count_miss: int = data["count_miss"]
 
     def __repr__(self):
-        attributes = ('total_score', 'user' if self.user is not None else 'user_id')
-        return prettify(self, *attributes)
+        return prettify(self, "count_300", "count_miss")
 
 
-class PlaylistItemStats:
+class ScoreDataStatistics:
     """
     **Attributes**
 
-    count_active: :class:`int`
+    ok: Optional[:class:`int`]
+
+    meh: Optional[:class:`int`]
+
+    good: Optional[:class:`int`]
+
+    miss: Optional[:class:`int`]
+
+    none: Optional[:class:`int`]
 
-    count_total: :class:`int`
+    great: Optional[:class:`int`]
 
-    ruleset_ids: :class:`Sequence[:class:`GameModeInt`]
+    perfect: Optional[:class:`int`]
+
+    ignore_hit: Optional[:class:`int`]
+
+    ignore_miss: Optional[:class:`int`]
+
+    large_bonus: Optional[:class:`int`]
+
+    small_bonus: Optional[:class:`int`]
+
+    large_tick_hit: Optional[:class:`int`]
+
+    small_tick_hit: Optional[:class:`int`]
+
+    large_tick_miss: Optional[:class:`int`]
+
+    small_tick_miss: Optional[:class:`int`]
     """
-    __slots__ = ("count_active", "count_total", "ruleset_ids")
+
+    __slots__ = (
+        "ok",
+        "meh",
+        "good",
+        "miss",
+        "none",
+        "great",
+        "perfect",
+        "ignore_hit",
+        "ignore_miss",
+        "large_bonus",
+        "small_bonus",
+        "large_tick_hit",
+        "small_tick_hit",
+        "large_tick_miss",
+        "small_tick_miss",
+    )
 
     def __init__(self, data):
-        self.count_active = data['count_active']
-        self.count_total = data['count_total']
-        self.ruleset_ids = list(map(GameModeInt, data['ruleset_ids']))
+        self.ok: Optional[int] = data.get("ok")
+        self.meh: Optional[int] = data.get("meh")
+        self.good: Optional[int] = data.get("good")
+        self.miss: Optional[int] = data.get("miss")
+        self.none: Optional[int] = data.get("none")
+        self.great: Optional[int] = data.get("great")
+        self.perfect: Optional[int] = data.get("perfect")
+        self.ignore_hit: Optional[int] = data.get("ignore_hit")
+        self.ignore_miss: Optional[int] = data.get("ignore_miss")
+        self.large_bonus: Optional[int] = data.get("large_bonus")
+        self.small_bonus: Optional[int] = data.get("small_bonus")
+        self.large_tick_hit: Optional[int] = data.get("large_tick_hit")
+        self.small_tick_hit: Optional[int] = data.get("small_tick_hit")
+        self.large_tick_miss: Optional[int] = data.get("large_tick_miss")
+        self.small_tick_miss: Optional[int] = data.get("small_tick_miss")
 
     def __repr__(self):
-        return prettify(self, 'count_active', 'count_total')
+        attrs = tuple(filter(lambda attr: getattr(self, attr) is not None, self.__slots__))
+        return prettify(self, *attrs[:2])
 
 
-class PlaylistItem:
+class LazerMod:
     """
     **Attributes**
 
-    id: :class:`int`
-
-    room_id: :class:`int`
-
-    beatmap_id: :class:`int`
+    mod: Union[:class:`Mod`, :class:`str`]
+        :class:`str` if mod acronym doesn't exist in :class:`Mod` enum
 
-    ruleset_id: :class:`GameModeInt`
+    settings: Optional[Dict]
+    """
 
-    allowed_mods: Sequence[:class:`LazerMod`]
+    __slots__ = ("mod", "settings")
+    if TYPE_CHECKING:
+        mod: Union[Mod, str]
 
-    required_mods: Sequence[:class:`LazerMod`]
+    def __init__(self, data):
+        try:
+            self.mod = Mod(data["acronym"])
+        except ValueError:
+            self.mod = data["acronym"]
+        self.settings: Optional[Dict] = data.get("settings")
 
-    expired: :class:`bool`
+    def __repr__(self):
+        return prettify(self, "mod", "settings")
 
-    owner_id: :class:`int`
 
-    playlist_order: Union[:class:`int`, :class:`NoneType`]
+class BeatmapUserScore:
+    """
+    **Attributes**
 
-    played_at: Union[:class:`datetime.datetime`, :class:`NoneType`]
+    position: :class:`int`
+        The position of the score within the requested beatmap ranking.
 
-    beatmap: Union[:class:`BeatmapCompact`, :class:`NoneType`]
+    score: :class:`LegacyScore`
+        The details of the score.
     """
-    __slots__ = (
-        "id", "room_id", "beatmap_id", "ruleset_id", "allowed_mods", "required_mods",
-        "expired", "owner_id", "playlist_order", "played_at", "beatmap"
-    )
+
+    __slots__ = ("position", "score")
 
     def __init__(self, data):
-        self.id = data['id']
-        self.room_id = data['room_id']
-        self.beatmap_id = data['beatmap_id']
-        self.ruleset_id = GameModeInt(data['ruleset_id'])
-        self.allowed_mods = list(map(LazerMod, data['allowed_mods']))
-        self.required_mods = list(map(LazerMod, data['required_mods']))
-        self.expired = data['expired']
-        self.owner_id = data['owner_id']
-        self.playlist_order = data['playlist_order']
-        self.played_at = parser.parse(data['played_at']) if data['played_at'] is not None else None
-        self.beatmap = BeatmapCompact(data['beatmap']) if data.get('beatmap') is not None else None
+        self.position: int = data["position"]
+        self.score: Union[LegacyScore, SoloScore] = get_score_object(data["score"])
 
     def __repr__(self):
-        attributes = ('id', 'beatmap' if self.beatmap is not None else 'beatmap_id')
-        return prettify(self, *attributes)
+        return prettify(self, "position")
```

### Comparing `osu.py-0.6.0/osu/objects/news.py` & `osu.py-1.0.0/osu/objects/news.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,80 +1,92 @@
 from dateutil import parser
+from typing import Optional, TYPE_CHECKING
 
-from ..util import prettify
+from ..util import prettify, get_optional
+
+if TYPE_CHECKING:
+    from datetime import datetime
 
 
 class NewsPost:
     """
     **Attributes**
 
     author: :class:`str`
 
     edit_url: :class:`str`
         Link to the file view on GitHub.
 
-    first_image: :class:`str` or :class:`NoneType`
+    first_image: Optional[:class:`str`]
         Link to the first image in the document.
 
     id: :class:`int`
 
     published_at: :class:`datetime.datetime`
 
     slug: :class:`str`
         Filename without the extension, used in URLs.
 
     title: :class:`str`
 
     updated_at: :class:`datetime.datetime`
 
-    **Optional Attributes**
-
-    content: :class:`str`
+    content: Optional[:class:`str`]
         HTML post content.
 
-    navigation: :class:`Navigation`
+    navigation: Optional[:class:`Navigation`]
         Navigation metadata.
 
-    preview: :class:`str`
+    preview: Optional[:class:`str`]
         First paragraph of content with HTML markup stripped.
     """
+
     __slots__ = (
-        "author", "edit_url", "first_image", "id",
-        "published_at", "slug", "title", "updated_at",
-        "content", "navigation", "preview"
+        "author",
+        "edit_url",
+        "first_image",
+        "id",
+        "published_at",
+        "slug",
+        "title",
+        "updated_at",
+        "content",
+        "navigation",
+        "preview",
     )
 
     def __init__(self, data):
-        self.author = data['author']
-        self.edit_url = data['edit_url']
-        self.first_image = data['first_image']
-        self.id = data['id']
-        self.published_at = parser.parse(data['published_at'])
-        self.slug = data['slug']
-        self.title = data['title']
-        self.updated_at = parser.parse(data['updated_at'])
-        self.content = data.get("content", "")
-        self.navigation = Navigation(data) if "navigation" in data else None
-        self.preview = data.get("preview", "")
+        self.author: str = data["author"]
+        self.edit_url: str = data["edit_url"]
+        self.first_image: Optional[str] = data["first_image"]
+        self.id: int = data["id"]
+        self.published_at: datetime = parser.parse(data["published_at"])
+        self.slug: str = data["slug"]
+        self.title: str = data["title"]
+        self.updated_at: datetime = parser.parse(data["updated_at"])
+        self.content: Optional[str] = data.get("content")
+        self.navigation: Optional[Navigation] = get_optional(data, "navigation", Navigation)
+        self.preview: Optional[str] = data.get("preview")
 
     def __repr__(self):
-        return prettify(self, 'title')
+        return prettify(self, "title")
 
 
 class Navigation:
     """
     **Attributes**
 
-    newer: :class:`NewsPost` or :class:`NoneType`
+    newer: Optional[:class:`NewsPost`]
         null if the next post is not present.
 
-    older: :class:`NewsPost` or :class:`NoneType`
+    older: Optional[:class:`NewsPost`]
         null if the previous post is not present.
     """
+
     __slots__ = ("newer", "older")
 
     def __init__(self, data):
-        self.newer = NewsPost(data['newer']) if data.get("newer") is not None else None
-        self.older = NewsPost(data['older']) if data.get("older") is not None else None
+        self.newer: Optional[NewsPost] = get_optional(data, "newer", NewsPost)
+        self.older: Optional[NewsPost] = get_optional(data, "older", NewsPost)
 
     def __repr__(self):
-        return prettify(self, 'newer', 'older')
+        return prettify(self, "newer", "older")
```

### Comparing `osu.py-0.6.0/osu/objects/notification.py` & `osu.py-1.0.0/osu/objects/notification.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,22 @@
 from dateutil import parser
+from typing import Optional, TYPE_CHECKING, Union
 
-from ..util import prettify
-from ..enums import NotificationCategory, ObjectType, NotificationType, ChatChannelType, GameModeStr
+from ..util import prettify, get_optional
+from ..enums import (
+    NotificationCategory,
+    ObjectType,
+    NotificationType,
+    ChatChannelType,
+    GameModeStr,
+)
+
+
+if TYPE_CHECKING:
+    from datetime import datetime
 
 
 class Notification:
     """
     Represents a notification object.
     Go to :class:`Details` object to see details for each event
 
@@ -18,35 +29,32 @@
 
     created_at: :class:`datetime.datetime`
 
     object_type: :class:`ObjectType`
 
     object_id: :class:`int`
 
-    source_user_id: :class:`int`
+    source_user_id: Optional[:class:`int`]
 
     is_read: :class:`bool`
 
-    details: Optional[Union[
+    details: Union[
     :class:`BeatmapOwnerChangeDetails`, :class:`BeatmapsetDiscussionLockDetails`,
-    :class:`BeatmapsetDiscussionPostDetails`, :class:`BeatmapsetDiscussionQualifiedProblemDetails`,
+    :class:`BeatmapsetDiscussionPostNewDetails`, :class:`BeatmapsetDiscussionQualifiedProblemDetails`,
     :class:`BeatmapsetDiscussionReviewNewDetails`, :class:`BeatmapsetDiscussionUnlockDetails`,
     :class:`BeatmapsetDisqualifyDetails`, :class:`BeatmapsetLoveDetails`,
     :class:`BeatmapsetNominateDetails`, :class:`BeatmapsetQualifyDetails`,
     :class:`BeatmapsetRankDetails`, :class:`BeatmapsetRemoveFromLovedDetails`,
     :class:`BeatmapsetResetNominationsDetails`, :class:`ChannelAnnouncementDetails`,
     :class:`ChannelMessageDetails`, :class:`CommentNewDetails`,
     :class:`ForumTopicReplyDetails`, :class:`UserAchievementUnlockDetails`,
     :class:`UserBeatmapsetNewDetails`, :class:`UserBeatmapsetReviveDetails`
-    ]]
+    ]
         Details of the notification.
 
-    source_user_id: Optional[int]
-
-
     **Documented event names and their attribute meanings**
 
     beatmapset_discussion_lock
         object_id: Beatmapset id
         object_type: beatmapset
         source_user_id: User who locked discussion
 
@@ -96,72 +104,80 @@
         source_user_id: User who posted message
 
     forum_topic_reply
         object_id: Topic id
         object_type: forum_topic
         source_user_id: User who posted message
     """
+
     __slots__ = (
-        "id", "name", "created_at", "object_type", "object_id", "is_read",
-        "source_user_id", "details"
+        "id",
+        "name",
+        "created_at",
+        "object_type",
+        "object_id",
+        "is_read",
+        "source_user_id",
+        "details",
     )
 
     def __init__(self, data):
-        self.id = data['id']
-        self.name = NotificationType(data['name'])
-        self.created_at = parser.parse(data['created_at'])
-        self.object_type = ObjectType(data['object_type'])
-        self.object_id = data['object_id']
-        self.is_read = data['is_read']
-        self.details = Details(data['details'], self.name)
-
-        self.source_user_id = data.get('source_user_id', None)
+        self.id: int = data["id"]
+        self.name: NotificationType = NotificationType(data["name"])
+        self.created_at: datetime = parser.parse(data["created_at"])
+        self.object_type: ObjectType = ObjectType(data["object_type"])
+        self.object_id: int = data["object_id"]
+        self.source_user_id: Optional[int] = data.get("source_user_id")
+        self.is_read: bool = data["is_read"]
+        self.details: _DETAILS_TYPE = _get_details_object(data["details"], self.name)
 
     def __repr__(self):
-        return prettify(self, 'name', 'details')
+        return prettify(self, "name", "details")
 
 
 class ReadNotification:
     """
     Represents a read notification.
 
     **Attributes**
 
-    category: :class:`str`
+    category: :class:`NotificationCategory`
 
     id: :class:`int`
 
     object_id: :class:`int`
 
-    object_type: :class:`str`
+    object_type: :class:`ObjectType`
     """
+
     __slots__ = ("category", "id", "object_id", "object_type")
 
     def __init__(self, data):
-        self.category = NotificationCategory(data["category"])
-        self.id = data["id"]
-        self.object_id = data["object_id"]
-        self.object_type = ObjectType(data["object_type"])
+        self.category: NotificationCategory = NotificationCategory(data["category"])
+        self.id: int = data["id"]
+        self.object_id: int = data["object_id"]
+        self.object_type: ObjectType = ObjectType(data["object_type"])
 
     def __repr__(self):
-        return prettify(self, 'id')
+        return prettify(self, "id")
 
 
 class NotificationsDetailsBase:
     """
     Base class for all Detail objects.
 
     **Attributes**
 
     username: :class:`str`
     """
+
     __slots__ = ("username",)
 
     def __init__(self, data):
-        self.username = data["username"]
+        self.username: str = data["username"]
 
     def __repr__(self):
         # all the subclasses have a title attribute
         return prettify(self, "title", "username")
 
 
 class BeatmapOwnerChangeDetails(NotificationsDetailsBase):
@@ -178,23 +194,24 @@
 
     title: :class:`str`
 
     title_unicode: :class:`str`
 
     version: :class:`str`
     """
+
     __slots__ = ("beatmap_id", "cover_url", "title", "title_unicode", "version")
 
     def __init__(self, data):
         super().__init__(data)
-        self.beatmap_id = data["beatmap_id"]
-        self.cover_url = data["cover_url"]
-        self.title = data["title"]
-        self.title_unicode = data["title_unicode"]
-        self.version = data["version"]
+        self.beatmap_id: int = data["beatmap_id"]
+        self.cover_url: str = data["cover_url"]
+        self.title: str = data["title"]
+        self.title_unicode: str = data["title_unicode"]
+        self.version: str = data["version"]
 
 
 class BeatmapsetNotificationDetails(NotificationsDetailsBase):
     """
     Base class for several other detail objects.
 
     Extends :class:`NotificationsDetailsBase`
@@ -203,21 +220,22 @@
 
     title: :class:`str`
 
     title_unicode: :class:`str`
 
     cover_url: :class:`str`
     """
+
     __slots__ = ("title", "title_unicode", "cover_url")
 
     def __init__(self, data):
         super().__init__(data)
-        self.title = data["title"]
-        self.title_unicode = data["title_unicode"]
-        self.cover_url = data["cover_url"]
+        self.title: str = data["title"]
+        self.title_unicode: str = data["title_unicode"]
+        self.cover_url: str = data["cover_url"]
 
 
 class BeatmapsetDiscussionPostNotificationDetails(NotificationsDetailsBase):
     """
     Base class for a couple other detail objects.
 
     Extends :class:`NotificationsDetailsBase`
@@ -234,28 +252,53 @@
 
     discussion_id: :class:`int`
 
     beatmap_id: :class:`int`
 
     cover_url: :class:`str`
     """
+
     __slots__ = (
-        "content", "title", "title_unicode", "post_id", "discussion_id",
-        "beatmap_id", "cover_url"
+        "content",
+        "title",
+        "title_unicode",
+        "post_id",
+        "discussion_id",
+        "beatmap_id",
+        "cover_url",
     )
 
     def __init__(self, data):
         super().__init__(data)
-        self.content = data["content"]
-        self.title = data["title"]
-        self.title_unicode = data["title_unicode"]
-        self.post_id = data["post_id"]
-        self.discussion_id = data["discussion_id"]
-        self.beatmap_id = data["beatmap_id"]
-        self.cover_url = data["cover_url"]
+        self.content: str = data["content"]
+        self.title: str = data["title"]
+        self.title_unicode: str = data["title_unicode"]
+        self.post_id: int = data["post_id"]
+        self.discussion_id: int = data["discussion_id"]
+        self.beatmap_id: int = data["beatmap_id"]
+        self.cover_url: str = data["cover_url"]
+
+
+class ReviewStats:
+    """
+    **Attributes**
+
+    praises: :class:`int`
+
+    suggestions: :class:`int`
+
+    problems: :class:`int`
+    """
+
+    __slots__ = ("praises", "suggestions", "problems")
+
+    def __init__(self, data):
+        self.praises = data["praises"]
+        self.suggestions = data["suggestions"]
+        self.problems = data["problems"]
 
 
 class BeatmapsetDiscussionReviewNewDetails(NotificationsDetailsBase):
     """
     New beatmapset discussion review.
 
     Extends :class:`NotificationsDetailsBase`
@@ -270,31 +313,36 @@
 
     discussion_id: :class:`int`
 
     beatmap_id: :class:`int`
 
     cover_url: :class:`str`
 
-    embeds: :class:`dict`
-        contains keys 'suggestions', 'problems', and 'praises'
+    embeds: :class:`ReviewStats`
     """
+
     __slots__ = (
-        "title", "title_unicode", "post_id", "discussion_id",
-        "beatmap_id", "cover_url", "embeds"
+        "title",
+        "title_unicode",
+        "post_id",
+        "discussion_id",
+        "beatmap_id",
+        "cover_url",
+        "embeds",
     )
 
     def __init__(self, data):
         super().__init__(data)
-        self.title = data["title"]
-        self.title_unicode = data["title_unicode"]
-        self.post_id = data["post_id"]
-        self.discussion_id = data["discussion_id"]
-        self.beatmap_id = data["beatmap_id"]
-        self.cover_url = data["cover_url"]
-        self.embeds = data["embeds"]
+        self.title: str = data["title"]
+        self.title_unicode: str = data["title_unicode"]
+        self.post_id: int = data["post_id"]
+        self.discussion_id: int = data["discussion_id"]
+        self.beatmap_id: int = data["beatmap_id"]
+        self.cover_url: str = data["cover_url"]
+        self.embeds: ReviewStats = ReviewStats(data["embeds"])
 
 
 class ChannelAnnouncementDetails(NotificationsDetailsBase):
     """
     Chat channel announcement
 
     Extends :class:`NotificationsDetailsBase`
@@ -307,23 +355,24 @@
 
     title: :class:`str`
 
     type: :class:`ChatChannelType`
 
     cover_url: :class:`str`
     """
+
     __slots__ = ("channel_id", "name", "title", "type", "cover_url")
 
     def __init__(self, data):
         super().__init__(data)
-        self.channel_id = data["channel_id"]
-        self.name = data["name"]
-        self.title = data["title"]
-        self.type = ChatChannelType(data["type"].upper())
-        self.cover_url = data["cover_url"]
+        self.channel_id: int = data["channel_id"]
+        self.name: str = data["name"]
+        self.title: str = data["title"]
+        self.type: ChatChannelType = ChatChannelType(data["type"].upper())
+        self.cover_url: str = data["cover_url"]
 
 
 class ChannelMessageDetails(NotificationsDetailsBase):
     """
     Chat channel message
 
     Extends :class:`NotificationsDetailsBase`
@@ -332,21 +381,22 @@
 
     title: :class:`str`
 
     type: :class:`ChatChannelType`
 
     cover_url: :class:`str`
     """
+
     __slots__ = ("title", "type", "cover_url")
 
     def __init__(self, data):
         super().__init__(data)
-        self.title = data["title"]
-        self.type = ChatChannelType(data["type"].upper())
-        self.cover_url = data["cover_url"]
+        self.title: str = data["title"]
+        self.type: ChatChannelType = ChatChannelType(data["type"].upper())
+        self.cover_url: str = data["cover_url"]
 
 
 class CommentNewDetails(NotificationsDetailsBase):
     """
     New comment
 
     Extends :class:`NotificationsDetailsBase`
@@ -357,22 +407,23 @@
 
     title: :class:`str`
 
     content: :class:`str`
 
     cover_url: :class:`str`
     """
+
     __slots__ = ("comment_id", "title", "content", "cover_url")
 
     def __init__(self, data):
         super().__init__(data)
-        self.comment_id = data["comment_id"]
-        self.title = data["title"]
-        self.content = data["content"]
-        self.cover_url = data["cover_url"]
+        self.comment_id: int = data["comment_id"]
+        self.title: str = data["title"]
+        self.content: str = data["content"]
+        self.cover_url: str = data["cover_url"]
 
 
 class ForumTopicReplyDetails(NotificationsDetailsBase):
     """
     Forum topic reply
 
     Extends :class:`NotificationsDetailsBase`
@@ -381,21 +432,22 @@
 
     title: :class:`str`
 
     post_id: :class:`int`
 
     cover_url: :class:`str`
     """
+
     __slots__ = ("title", "post_id", "cover_url")
 
     def __init__(self, data):
         super().__init__(data)
-        self.title = data["title"]
-        self.post_id = data["post_id"]
-        self.cover_url = data["cover_url"]
+        self.title: str = data["title"]
+        self.post_id: int = data["post_id"]
+        self.cover_url: str = data["cover_url"]
 
 
 class UserAchievementUnlockDetails(NotificationsDetailsBase):
     """
     New achievement unlocked
 
     Extends :class:`NotificationsDetailsBase`
@@ -410,28 +462,32 @@
 
     slug: :class:`str`
 
     title: :class:`str`
 
     user_id: :class:`int`
     """
+
     __slots__ = (
-        "achievement_id", "achievement_mode", "cover_url",
-        "slug", "title", "user_id"
+        "achievement_id",
+        "achievement_mode",
+        "cover_url",
+        "slug",
+        "title",
+        "user_id",
     )
 
     def __init__(self, data):
         super().__init__(data)
-        self.achievement_id = data["achievement_id"]
-        self.achievement_mode = GameModeStr(data["achievement_mode"]) \
-            if data["achievement_mode"] is not None else None
-        self.cover_url = data["cover_url"]
-        self.slug = data["slug"]
-        self.title = data["title"]
-        self.user_id = data["user_id"]
+        self.achievement_id: int = data["achievement_id"]
+        self.achievement_mode: Optional[GameModeStr] = get_optional(data, "achievement_mode", GameModeStr)
+        self.cover_url: str = data["cover_url"]
+        self.slug: str = data["slug"]
+        self.title: str = data["title"]
+        self.user_id: int = data["user_id"]
 
 
 class UserBeatmapsetNewDetails(NotificationsDetailsBase):
     """
     New beatmapset
 
     Extends: :class:`NotificationsDetailsBase`
@@ -442,23 +498,23 @@
 
     title: :class:`str`
 
     title_unicode: :class:`str`
 
     cover_url: :class:`str`
     """
+
     __slots__ = ("beatmapset_id", "title", "title_unicode", "cover_url")
 
     def __init__(self, data):
         super().__init__(data)
-        self.beatmapset_id = data["beatmapset_id"]
-        self.title = data["title"]
-        self.title_unicode = data["title_unicode"]
-        self.cover_url = data["cover_url"]
-        self.username = data.get("username")
+        self.beatmapset_id: int = data["beatmapset_id"]
+        self.title: str = data["title"]
+        self.title_unicode: str = data["title_unicode"]
+        self.cover_url: str = data["cover_url"]
 
 
 class BeatmapsetDiscussionLockDetails(BeatmapsetNotificationDetails):
     """
     Beatmapset discussion locked
 
     Extends :class:`BeatmapsetNotificationDetails`
@@ -549,33 +605,55 @@
     """
     User beatmapset revived
 
     Extends :class:`UserBeatmapsetNewDetails`
     """
 
 
-class Details:
-    DETAIL_MAP = {
-        NotificationType.BEATMAP_OWNER_CHANGE: BeatmapOwnerChangeDetails,
-        NotificationType.BEATMAPSET_DISCUSSION_LOCK: BeatmapsetDiscussionLockDetails,
-        NotificationType.BEATMAPSET_DISCUSSION_POST_NEW: BeatmapsetDiscussionPostNewDetails,
-        NotificationType.BEATMAPSET_DISCUSSION_QUALIFIED_PROBLEM: BeatmapsetDiscussionQualifiedProblemDetails,
-        NotificationType.BEATMAPSET_DISCUSSION_REVIEW_NEW: BeatmapsetDiscussionReviewNewDetails,
-        NotificationType.BEATMAPSET_DISCUSSION_UNLOCK: BeatmapsetDiscussionUnlockDetails,
-        NotificationType.BEATMAPSET_DISQUALIFY: BeatmapsetDisqualifyDetails,
-        NotificationType.BEATMAPSET_LOVE: BeatmapsetLoveDetails,
-        NotificationType.BEATMAPSET_NOMINATE: BeatmapsetNominateDetails,
-        NotificationType.BEATMAPSET_QUALIFY: BeatmapsetQualifyDetails,
-        NotificationType.BEATMAPSET_RANK: BeatmapsetRankDetails,
-        NotificationType.BEATMAPSET_REMOVE_FROM_LOVED: BeatmapsetRemoveFromLovedDetails,
-        NotificationType.BEATMAPSET_RESET_NOMINATIONS: BeatmapsetResetNominationsDetails,
-        NotificationType.CHANNEL_ANNOUNCEMENT: ChannelAnnouncementDetails,
-        NotificationType.CHANNEL_MESSAGE: ChannelMessageDetails,
-        NotificationType.COMMENT_NEW: CommentNewDetails,
-        NotificationType.FORUM_TOPIC_REPLY: ForumTopicReplyDetails,
-        NotificationType.USER_ACHIEVEMENT_UNLOCK: UserAchievementUnlockDetails,
-        NotificationType.USER_BEATMAPSET_NEW: UserBeatmapsetNewDetails,
-        NotificationType.USER_BEATMAPSET_REVIVE: UserBeatmapsetReviveDetails,
-    }
+_DETAILS_TYPE = Union[
+    BeatmapOwnerChangeDetails,
+    BeatmapsetDiscussionLockDetails,
+    BeatmapsetDiscussionPostNewDetails,
+    BeatmapsetDiscussionQualifiedProblemDetails,
+    BeatmapsetDiscussionReviewNewDetails,
+    BeatmapsetDiscussionUnlockDetails,
+    BeatmapsetDisqualifyDetails,
+    BeatmapsetLoveDetails,
+    BeatmapsetNominateDetails,
+    BeatmapsetQualifyDetails,
+    BeatmapsetRankDetails,
+    BeatmapsetRemoveFromLovedDetails,
+    BeatmapsetResetNominationsDetails,
+    ChannelAnnouncementDetails,
+    ChannelMessageDetails,
+    CommentNewDetails,
+    ForumTopicReplyDetails,
+    UserAchievementUnlockDetails,
+    UserBeatmapsetNewDetails,
+    UserBeatmapsetReviveDetails,
+]
+_DETAIL_MAP = {
+    NotificationType.BEATMAP_OWNER_CHANGE: BeatmapOwnerChangeDetails,
+    NotificationType.BEATMAPSET_DISCUSSION_LOCK: BeatmapsetDiscussionLockDetails,
+    NotificationType.BEATMAPSET_DISCUSSION_POST_NEW: BeatmapsetDiscussionPostNewDetails,
+    NotificationType.BEATMAPSET_DISCUSSION_QUALIFIED_PROBLEM: BeatmapsetDiscussionQualifiedProblemDetails,
+    NotificationType.BEATMAPSET_DISCUSSION_REVIEW_NEW: BeatmapsetDiscussionReviewNewDetails,
+    NotificationType.BEATMAPSET_DISCUSSION_UNLOCK: BeatmapsetDiscussionUnlockDetails,
+    NotificationType.BEATMAPSET_DISQUALIFY: BeatmapsetDisqualifyDetails,
+    NotificationType.BEATMAPSET_LOVE: BeatmapsetLoveDetails,
+    NotificationType.BEATMAPSET_NOMINATE: BeatmapsetNominateDetails,
+    NotificationType.BEATMAPSET_QUALIFY: BeatmapsetQualifyDetails,
+    NotificationType.BEATMAPSET_RANK: BeatmapsetRankDetails,
+    NotificationType.BEATMAPSET_REMOVE_FROM_LOVED: BeatmapsetRemoveFromLovedDetails,
+    NotificationType.BEATMAPSET_RESET_NOMINATIONS: BeatmapsetResetNominationsDetails,
+    NotificationType.CHANNEL_ANNOUNCEMENT: ChannelAnnouncementDetails,
+    NotificationType.CHANNEL_MESSAGE: ChannelMessageDetails,
+    NotificationType.COMMENT_NEW: CommentNewDetails,
+    NotificationType.FORUM_TOPIC_REPLY: ForumTopicReplyDetails,
+    NotificationType.USER_ACHIEVEMENT_UNLOCK: UserAchievementUnlockDetails,
+    NotificationType.USER_BEATMAPSET_NEW: UserBeatmapsetNewDetails,
+    NotificationType.USER_BEATMAPSET_REVIVE: UserBeatmapsetReviveDetails,
+}
+
 
-    def __new__(cls, data, detail_type):
-        return cls.DETAIL_MAP[detail_type](data)
+def _get_details_object(data, detail_type) -> _DETAILS_TYPE:
+    return _DETAIL_MAP[detail_type](data)
```

### Comparing `osu.py-0.6.0/osu/objects/scope.py` & `osu.py-1.0.0/osu/objects/scope.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,38 +13,41 @@
     forum.write
         Allows creating and editing forum posts on a user's behalf.
     delegate
         Allows acting as the owner of a client; only available for Client Credentials Grant.
     chat.write
         Allows sending chat messages on a user's behalf.
     """
+
+    __slots__ = ("scopes", "scopes_list")
     valid_scopes = [
-        'chat.write',
-        'delegate',
-        'forum.write',
-        'friends.read',
-        'identify',
-        'public',
+        "chat.write",
+        "delegate",
+        "forum.write",
+        "friends.read",
+        "identify",
+        "public",
     ]
 
     def __init__(self, *scopes):
         for scope in scopes:
             if scope not in self.valid_scopes and scope != "*":
-                raise NameError(f"{scope} is not a valid scope. The valid scopes consist of "
-                                f"{','.join(self.valid_scopes)}")
-        self.scopes = ' '.join(scopes)
+                raise NameError(
+                    f"{scope} is not a valid scope. The valid scopes consist of " f"{','.join(self.valid_scopes)}"
+                )
+        self.scopes = " ".join(scopes)
         self.scopes_list = list(scopes)
 
     @classmethod
     def default(cls):
-        return cls('public')
+        return cls("public")
 
     @classmethod
     def identify(cls):
-        return cls('public', 'identify')
+        return cls("public", "identify")
 
     def __iter__(self):
         return iter(self.scopes_list)
 
     def __len__(self):
         return len(self.scopes_list)
```

### Comparing `osu.py-0.6.0/osu/objects/seasonal_background.py` & `osu.py-1.0.0/osu/objects/seasonal_background.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,48 +1,55 @@
-from .user import UserCompact
 from dateutil import parser
+from typing import TYPE_CHECKING, List
 
+from .user import UserCompact
 from ..util import prettify
 
 
+if TYPE_CHECKING:
+    from datetime import datetime
+
+
 class SeasonalBackgrounds:
     """
     Contains data on the seasonal backgrounds.
 
     **Attributes**
 
     ends_at: :class:`datetime.datetime`
         The date when the seasonal backgrounds will end.
 
-    backgrounds: Sequence[:class:`SeasonalBackground`]
+    backgrounds: List[:class:`SeasonalBackground`]
         A list of all the seasonal backgrounds.
     """
-    __slots__ = ('ends_at', 'backgrounds')
+
+    __slots__ = ("ends_at", "backgrounds")
 
     def __init__(self, data):
-        self.ends_at = parser.parse(data['ends_at'])
-        self.backgrounds = list(map(SeasonalBackground, data['backgrounds']))
+        self.ends_at: datetime = parser.parse(data["ends_at"])
+        self.backgrounds: List[SeasonalBackground] = list(map(SeasonalBackground, data["backgrounds"]))
 
     def __repr__(self):
-        return prettify(self, 'ends_at', 'backgrounds')
+        return prettify(self, "ends_at", "backgrounds")
 
 
 class SeasonalBackground:
     """
     Represents a seasonal background.
 
     **Attributes**
 
     url: :class:`str`
         The url of the background.
 
     user: :class:`UserCompact`
         The artist of the background.
     """
-    __slots__ = ('url', 'user')
+
+    __slots__ = ("url", "user")
 
     def __init__(self, data):
-        self.url = data['url']
-        self.user = UserCompact(data['user'])
+        self.url: str = data["url"]
+        self.user: UserCompact = UserCompact(data["user"])
 
     def __repr__(self):
-        return prettify(self, 'url', 'user')
+        return prettify(self, "url", "user")
```

### Comparing `osu.py-0.6.0/osu/path.py` & `osu.py-1.0.0/osu/path.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,320 +1,329 @@
 class Path:
-    __slots__ = ("method", "path", "scope", "requires_user")
+    __slots__ = ("method", "path", "scope", "requires_user", "content_type", "accept")
 
-    def __init__(self, method, path, scope, requires_user=False):
+    def __init__(
+        self, method, path, scope, requires_user=False, content_type="application/json", accept="application/json"
+    ):
         self.method = method
         self.path = path
         self.scope = scope
         self.requires_user = requires_user
+        self.content_type = content_type
+        self.accept = accept
 
     @property
     def requires_auth(self):
         return self.scope is not None
 
     @classmethod
     def beatmap_lookup(cls):
-        return cls('get', "beatmaps/lookup", 'public')
+        return cls("get", "beatmaps/lookup", "public")
 
     @classmethod
     def user_beatmap_score(cls, beatmap, user):
-        return cls('get', f"beatmaps/{beatmap}/scores/users/{user}", 'public')
+        return cls("get", f"beatmaps/{beatmap}/scores/users/{user}", "public")
 
     @classmethod
     def user_beatmap_scores(cls, beatmap, user):
-        return cls('get', f"beatmaps/{beatmap}/scores/users/{user}/all", 'public')
+        return cls("get", f"beatmaps/{beatmap}/scores/users/{user}/all", "public")
 
     @classmethod
     def beatmap_scores(cls, beatmap):
-        return cls('get', f"beatmaps/{beatmap}/scores", 'public')
+        return cls("get", f"beatmaps/{beatmap}/scores", "public")
 
     @classmethod
     def lazer_beatmap_scores(cls, beatmap):
-        return cls('get', f"beatmaps/{beatmap}/solo-scores", 'public')
+        return cls("get", f"beatmaps/{beatmap}/solo-scores", "public")
 
     @classmethod
     def beatmap(cls, beatmap):
-        return cls('get', f"beatmaps/{beatmap}", 'public')
+        return cls("get", f"beatmaps/{beatmap}", "public")
 
     @classmethod
     def beatmaps(cls):
-        return cls('get', "beatmaps", 'public')
+        return cls("get", "beatmaps", "public")
 
     @classmethod
     def get_beatmap_attributes(cls, beatmap):
-        return cls('post', f"beatmaps/{beatmap}/attributes", 'public')
+        return cls("post", f"beatmaps/{beatmap}/attributes", "public")
 
     @classmethod
     def get_beatmapset(cls, beatmapset):
-        return cls('get', f'beatmapsets/{beatmapset}', 'public')
+        return cls("get", f"beatmapsets/{beatmapset}", "public")
 
     @classmethod
     def beatmapset_discussion_posts(cls):
-        return cls('get', 'beatmapsets/discussions/posts', 'public')
+        return cls("get", "beatmapsets/discussions/posts", "public")
 
     @classmethod
     def beatmapset_discussion_votes(cls):
-        return cls('get', 'beatmapsets/discussions/votes', 'public')
+        return cls("get", "beatmapsets/discussions/votes", "public")
 
     @classmethod
     def beatmapset_discussions(cls):
-        return cls('get', 'beatmapsets/discussions', 'public')
+        return cls("get", "beatmapsets/discussions", "public")
 
     @classmethod
     def get_changelog_build(cls, stream, build):
-        return cls('get', f"changelog/{stream}/{build}", None)
+        return cls("get", f"changelog/{stream}/{build}", None)
 
     @classmethod
     def get_changelog_listing(cls):
-        return cls('get', 'changelog', None)
+        return cls("get", "changelog", None)
 
     @classmethod
     def lookup_changelog_build(cls, changelog):
-        return cls('get', f'changelog/{changelog}', None)
+        return cls("get", f"changelog/{changelog}", None)
 
     @classmethod
     def chat_ack(cls):
-        return cls('post', 'chat/ack', 'lazer', True)
+        return cls("post", "chat/ack", "lazer", True)
 
     @classmethod
     def create_new_pm(cls):
-        return cls('post', 'chat/new', 'chat.write', True)
+        return cls("post", "chat/new", "chat.write", True)
 
     @classmethod
     def get_updates(cls):
-        return cls('get', 'chat/updates', 'lazer', True)
+        return cls("get", "chat/updates", "lazer", True)
 
     @classmethod
     def get_channel_messages(cls, channel):
-        return cls('get', f'chat/channels/{channel}/messages', 'lazer', True)
+        return cls("get", f"chat/channels/{channel}/messages", "lazer", True)
 
     @classmethod
     def send_message_to_channel(cls, channel):
-        return cls('post', f'chat/channels/{channel}/messages', 'lazer', True)
+        return cls("post", f"chat/channels/{channel}/messages", "lazer", True)
 
     @classmethod
     def join_channel(cls, channel, user):
-        return cls('put', f'chat/channels/{channel}/users/{user}', 'lazer', True)
+        return cls("put", f"chat/channels/{channel}/users/{user}", "lazer", True)
 
     @classmethod
     def leave_channel(cls, channel, user):
-        return cls('delete', f'chat/channels/{channel}/users/{user}', 'lazer', True)
+        return cls("delete", f"chat/channels/{channel}/users/{user}", "lazer", True)
 
     @classmethod
     def mark_channel_as_read(cls, channel, message):
-        return cls('put', f'chat/channels/{channel}/mark-as-read/{message}', 'lazer', True)
+        return cls("put", f"chat/channels/{channel}/mark-as-read/{message}", "lazer", True)
 
     @classmethod
     def get_channel_list(cls):
-        return cls('get', 'chat/channels', 'lazer', True)
+        return cls("get", "chat/channels", "lazer", True)
 
     @classmethod
     def create_channel(cls):
-        return cls('post', 'chat/channels', 'lazer', True)
+        return cls("post", "chat/channels", "lazer", True)
 
     @classmethod
     def get_channel(cls, channel):
-        return cls('get', f'chat/channels/{channel}', 'lazer', True)
+        return cls("get", f"chat/channels/{channel}", "lazer", True)
 
     @classmethod
     def get_comments(cls):
-        return cls('get', 'comments', None)
+        return cls("get", "comments", None)
 
     @classmethod
     def post_new_comment(cls):
-        return cls('post', 'comments', 'lazer', True)
+        return cls("post", "comments", "lazer", True)
 
     @classmethod
     def get_comment(cls, comment):
-        return cls('get', f'comments/{comment}', None)
+        return cls("get", f"comments/{comment}", None)
 
     @classmethod
     def edit_comment(cls, comment):
-        return cls('patch', f'comments/{comment}', 'lazer', True)
+        return cls("patch", f"comments/{comment}", "lazer", True)
 
     @classmethod
     def delete_comment(cls, comment):
-        return cls('delete', f'comments/{comment}', 'lazer', True)
+        return cls("delete", f"comments/{comment}", "lazer", True)
 
     @classmethod
     def add_comment_vote(cls, comment):
-        return cls('post', f'comments/{comment}/vote', 'lazer', True)
+        return cls("post", f"comments/{comment}/vote", "lazer", True)
 
     @classmethod
     def remove_comment_vote(cls, comment):
-        return cls('delete', f'comments/{comment}/vote', 'lazer', True)
+        return cls("delete", f"comments/{comment}/vote", "lazer", True)
 
     @classmethod
     def reply_topic(cls, topic):
-        return cls('post', f'forums/topics/{topic}/reply', 'forum.write', True)
+        return cls("post", f"forums/topics/{topic}/reply", "forum.write", True)
 
     @classmethod
     def create_topic(cls):
-        return cls('post', 'forums/topics', 'forum.write', True)
+        return cls("post", "forums/topics", "forum.write", True)
 
     @classmethod
     def get_topic_and_posts(cls, topic):
-        return cls('get', f'forums/topics/{topic}', 'public')
+        return cls("get", f"forums/topics/{topic}", "public")
 
     @classmethod
     def edit_topic(cls, topic):
-        return cls('patch', f'forums/topics/{topic}', 'forum.write')
+        return cls("patch", f"forums/topics/{topic}", "forum.write")
 
     @classmethod
     def edit_post(cls, post):
-        return cls('patch', f'forums/posts/{post}', 'forum.write')
+        return cls("patch", f"forums/posts/{post}", "forum.write")
 
     @classmethod
     def search(cls):
-        return cls('get', 'search', 'public')
+        return cls("get", "search", "public")
 
     @classmethod
     def get_user_high_score(cls, room, playlist, user):
-        return cls('get', f'rooms/{room}/playlist/{playlist}/scores/users/{user}', 'lazer', True)
+        return cls(
+            "get",
+            f"rooms/{room}/playlist/{playlist}/scores/users/{user}",
+            "lazer",
+            True,
+        )
 
     @classmethod
     def get_scores(cls, room, playlist):
-        return cls('get', f'rooms/{room}/playlist/{playlist}/scores', 'public', True)
+        return cls("get", f"rooms/{room}/playlist/{playlist}/scores", "public", True)
 
     @classmethod
     def get_score(cls, room, playlist, score):
-        return cls('get', f'rooms/{room}/playlist/{playlist}/scores/{score}', 'lazer', True)
+        return cls("get", f"rooms/{room}/playlist/{playlist}/scores/{score}", "lazer", True)
 
     @classmethod
     def get_news_listing(cls):
-        return cls('get', 'news', None)
+        return cls("get", "news", None)
 
     @classmethod
     def get_news_post(cls, news):
-        return cls('get', f'news/{news}', None)
+        return cls("get", f"news/{news}", None)
 
     @classmethod
     def get_notifications(cls):
-        return cls('get', 'notifications', 'lazer', True)
+        return cls("get", "notifications", "lazer", True)
 
     @classmethod
     def mark_notifications_as_read(cls):
-        return cls('post', 'notifications/mark-read', 'lazer', True)
+        return cls("post", "notifications/mark-read", "lazer", True)
 
     @classmethod
     def revoke_current_token(cls):
-        return cls('delete', 'oauth/tokens/current', 'public')
+        return cls("delete", "oauth/tokens/current", "public")
 
     @classmethod
     def get_ranking(cls, mode, type):
-        return cls('get', f'rankings/{mode}/{type}', 'public')
+        return cls("get", f"rankings/{mode}/{type}", "public")
 
     @classmethod
     def get_spotlights(cls):
-        return cls('get', 'spotlights', 'public')
+        return cls("get", "spotlights", "public")
 
     @classmethod
-    def get_own_data(cls, mode=''):
-        return cls('get', f'me/{mode}', 'identify')
+    def get_own_data(cls, mode=""):
+        return cls("get", f"me/{mode}", "identify")
 
     @classmethod
     def get_user_kudosu(cls, user):
-        return cls('get', f'users/{user}/kudosu', 'public')
+        return cls("get", f"users/{user}/kudosu", "public")
 
     @classmethod
     def get_user_scores(cls, user, type):
-        return cls('get', f'users/{user}/scores/{type}', 'public')
+        return cls("get", f"users/{user}/scores/{type}", "public")
 
     @classmethod
     def get_user_beatmaps(cls, user, type):
-        return cls('get', f'users/{user}/beatmapsets/{type}', 'public')
+        return cls("get", f"users/{user}/beatmapsets/{type}", "public")
 
     @classmethod
     def get_user_recent_activity(cls, user):
-        return cls('get', f'users/{user}/recent_activity', 'public')
+        return cls("get", f"users/{user}/recent_activity", "public")
 
     @classmethod
-    def get_user(cls, user, mode=''):
-        return cls('get', f'users/{user}/{mode}', 'public')
+    def get_user(cls, user, mode=""):
+        return cls("get", f"users/{user}/{mode}", "public")
 
     @classmethod
     def get_users(cls):
-        return cls('get', 'users', 'public')
+        return cls("get", "users", "public")
 
     @classmethod
     def get_wiki_page(cls, locale, path):
-        return cls('get', f'wiki/{locale}/{path}', None)
+        return cls("get", f"wiki/{locale}/{path}", None)
 
     @classmethod
     def get_score_by_id(cls, mode, score):
-        return cls('get', f'scores/{mode}/{score}', 'public')
+        return cls("get", f"scores/{mode}/{score}", "public")
 
     @classmethod
     def get_beatmapset_events(cls):
-        return cls('get', 'beatmapsets/events', 'public')
+        return cls("get", "beatmapsets/events", "public")
 
     @classmethod
     def get_matches(cls):
-        return cls('get', 'matches', 'public')
+        return cls("get", "matches", "public")
 
     @classmethod
     def get_match(cls, match):
-        return cls('get', f'matches/{match}', 'public')
+        return cls("get", f"matches/{match}", "public")
 
     @classmethod
-    def get_rooms(cls, mode=''):
-        return cls('get', f'rooms/{mode}', 'public', True)
+    def get_rooms(cls, mode=""):
+        return cls("get", f"rooms/{mode}", "public", True)
 
     @classmethod
     def get_room(cls, room):
-        return cls('get', f'rooms/{room}', 'public')
+        return cls("get", f"rooms/{room}", "public")
 
     @classmethod
     def get_room_leaderboard(cls, room):
-        return cls('get', f'rooms/{room}/leaderboard', 'public', True)
+        return cls("get", f"rooms/{room}/leaderboard", "public", True)
 
     @classmethod
     def get_seasonal_backgrounds(cls):
-        return cls('get', 'seasonal-backgrounds', None)
+        return cls("get", "seasonal-backgrounds", None)
 
     @classmethod
     def get_replay_data(cls, mode, score):
-        return cls('get', f'scores/{mode}/{score}/download', 'public', True)
+        return cls("get", f"scores/{mode}/{score}/download", "public", True)
 
     @classmethod
     def get_friends(cls):
-        return cls('get', 'friends', 'friends.read', True)
+        return cls("get", "friends", "friends.read", True)
 
     @classmethod
     def get_new_score_id(cls, beatmap_id):
-        return cls('post', f'beatmaps/{beatmap_id}/solo/scores', 'lazer', True)
+        return cls("post", f"beatmaps/{beatmap_id}/solo/scores", "lazer", True)
 
     @classmethod
     def submit_score(cls, beatmap_id, token):
-        return cls('put', f'beatmaps/{beatmap_id}/solo/scores/{token}', 'lazer', True)
+        return cls("put", f"beatmaps/{beatmap_id}/solo/scores/{token}", "lazer", True)
 
     @classmethod
     def favourite_beatmapset(cls, beatmapset_id):
-        return cls('post', f'beatmapsets/{beatmapset_id}/favourites', 'lazer', True)
+        return cls("post", f"beatmapsets/{beatmapset_id}/favourites", "lazer", True)
 
     @classmethod
     def get_chat_presence(cls):
-        return cls('get', 'chat/presence', 'lazer', True)
+        return cls("get", "chat/presence", "lazer", True)
 
     @classmethod
     def join_to_room(cls, room, user):
-        return cls('put', f'rooms/{room}/users/{user}', 'lazer', True)
+        return cls("put", f"rooms/{room}/users/{user}", "lazer", True)
 
     @classmethod
     def kick_from_room(cls, room, user):
-        return cls('delete', f'rooms/{room}/users/{user}', 'lazer', True)
+        return cls("delete", f"rooms/{room}/users/{user}", "lazer", True)
 
     @classmethod
     def send_report(cls):
-        return cls('post', 'reports', 'lazer', True)
+        return cls("post", "reports", "lazer", True)
 
     @classmethod
     def create_room(cls):
-        return cls('post', 'rooms', 'lazer', True)
+        return cls("post", "rooms", "lazer", True)
 
     @classmethod
     def download_quota_check(cls):
-        return cls('get', 'me/download-quota-check', 'lazer', True)
+        return cls("get", "me/download-quota-check", "lazer", True)
 
     @classmethod
     def beatmapset_search(cls):
-        return cls('get', 'beatmapsets/search', 'public')
+        return cls("get", "beatmapsets/search", "public")
```

### Comparing `osu.py-0.6.0/osu/util.py` & `osu.py-1.0.0/osu/util.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,41 +1,55 @@
 from .enums import (
-    Mods, Enum, BeatmapsetSearchSort,
-    BeatmapsetSearchGeneral, BeatmapsetSearchPlayed,
-    BeatmapsetSearchStatus, BeatmapsetSearchExtra,
-    ScoreRank, GameModeInt, Mod, NotificationCategory,
-    ObjectType
+    Mods,
+    Enum,
+    BeatmapsetSearchSort,
+    BeatmapsetSearchGeneral,
+    BeatmapsetSearchPlayed,
+    BeatmapsetSearchStatus,
+    BeatmapsetSearchExtra,
+    BeatmapsetLanguage,
+    BeatmapsetGenre,
+    ScoreRank,
+    GameModeInt,
+    Mod,
+    NotificationCategory,
+    ObjectType,
 )
-from typing import Sequence, Union
+from typing import Any, Sequence, Union, Optional, TypeVar, List, Callable, Dict
+
+
+_T = TypeVar("_T")
+_V = TypeVar("_V")
 
 
 def check_scope(func):
     def check(self, other):
         if not isinstance(other, self.__class__) and type(other) != str:
             raise TypeError(f"Cannot compare type Scope with type {type(other).__name__}")
         if isinstance(other, self.__class__):
             other = other.scope
         if other not in self.valid_scopes:
             raise NameError(f"{other} is not a valid scope.")
         return func(self, other)
+
     return check
 
 
 def create_autoclass_for_sphinx():
-    with open('objects.py', 'r') as f:
+    with open("objects.py", "r") as f:
         info = f.readline()
         while info:
-            if info.startswith('class'):
+            if info.startswith("class"):
                 name = info.split()[1]
-                if '(' in name:
-                    name = name.split('(')[0]
+                if "(" in name:
+                    name = name.split("(")[0]
                 else:
                     name = name[:-1]
                 content = f"{name}\n{'^' * len(name)}\n.. autoclass:: osu.{name}\n   :members:\n\n"
-                with open('text.txt', 'a') as f2:
+                with open("text.txt", "a") as f2:
                     f2.write(content)
                     f2.close()
             info = f.readline()
         f.close()
 
 
 def parse_mods_arg(mods):
@@ -48,18 +62,18 @@
             return
         return Mods.parse_any_list(mods).value
     raise TypeError(f"mods argument must be of type Mods or Sequence, not {type(mods)}")
 
 
 def prettify(cls: object, *fields: str) -> str:
     d = {s: getattr(cls, s) for s in fields}
-    return cls.__class__.__qualname__ + '(' + ', '.join([f"{k}={d[k]!r}" for k in d]) + ')'
+    return cls.__class__.__qualname__ + "(" + ", ".join([f"{k}={d[k]!r}" for k in d]) + ")"
 
 
-def parse_enum_args(*args):
+def parse_enum_args(*args: Enum) -> Union[List[Any], Any]:
     args = [arg.value if isinstance(arg, Enum) else arg for arg in args]
     return args if len(args) != 1 else args[0]
 
 
 def create_multipart_formdata(data: dict):
     return {k: (None, v, "text/plain", {"charset": "utf-8"}) for k, v in data.items()}
 
@@ -82,14 +96,15 @@
     """
     Util class that helps for filtering in :func:`Client.search_beatmapsets`.
 
     Read about each filter under its corresponding function.
 
     All set functions return the instance of the class to allow for chaining.
     """
+
     def __init__(self):
         self._filters = {
             "query": None,
             "sort": None,
             "nsfw": None,
             "played": None,
             "r": None,
@@ -97,121 +112,133 @@
             "l": None,
             "g": None,
             "e": None,
             "c": None,
             "s": None,
         }
 
-    def set_query(self, query: str) -> 'BeatmapsetSearchFilter':
+    def set_query(self, query: str) -> "BeatmapsetSearchFilter":
         """
         Set the query to search for.
 
         query: :class:`str`
         """
         self._filters["query"] = query
         return self
 
-    def set_sort(self, sort: Union[BeatmapsetSearchSort, str]) -> 'BeatmapsetSearchFilter':
+    def set_sort(self, sort: Union[BeatmapsetSearchSort, str]) -> "BeatmapsetSearchFilter":
         """
         Set the sort order of the search.
 
         sort: Union[:class:`BeatmapsetSearchSort`, :class:`str`]
         """
         self._filters["sort"] = sort.value if isinstance(sort, BeatmapsetSearchSort) else sort
         return self
 
-    def set_nsfw(self, nsfw: bool) -> 'BeatmapsetSearchFilter':
+    def set_nsfw(self, nsfw: bool) -> "BeatmapsetSearchFilter":
         """
         Set whether to include NSFW in the search.
 
         nsfw: :class:`bool`
         """
         self._filters["nsfw"] = nsfw
         return self
 
-    def set_played(self, played: Union[BeatmapsetSearchPlayed, str]) -> 'BeatmapsetSearchFilter':
+    def set_played(self, played: Union[BeatmapsetSearchPlayed, str]) -> "BeatmapsetSearchFilter":
         """
         Set whether to include played and unplayed beatmapsets in the search.
 
         played: Union[:class:`BeatmapsetSearchPlayed`, :class:`str`]
         """
         self._filters["played"] = played.value if isinstance(played, BeatmapsetSearchPlayed) else played
         return self
 
-    def set_ranked(self, rank: Union[ScoreRank, str]) -> 'BeatmapsetSearchFilter':
+    def set_ranked(self, rank: Union[ScoreRank, str]) -> "BeatmapsetSearchFilter":
         """
         Filter by rank achieved.
 
         rank: Union[:class:`ScoreRank`, :class:`str`]
         """
         self._filters["r"] = rank.value if isinstance(rank, ScoreRank) else rank
         return self
 
-    def set_mode(self, mode: Union[GameModeInt, str]) -> 'BeatmapsetSearchFilter':
+    def set_mode(self, mode: Union[GameModeInt, int]) -> "BeatmapsetSearchFilter":
         """
         Set the game mode to filter by.
 
         mode: Union[:class:`GameModeStr`, :class:`str`]
         """
         self._filters["m"] = mode.value if isinstance(mode, GameModeInt) else mode
         return self
 
-    def set_language(self, language: str) -> 'BeatmapsetSearchFilter':
+    def set_language(self, language: Union[BeatmapsetLanguage, int]) -> "BeatmapsetSearchFilter":
         """
         Set the language to filter by.
 
         language: :class:`str`
         """
-        self._filters["l"] = language
+        self._filters["l"] = language.value if isinstance(language, BeatmapsetLanguage) else language
         return self
 
-    def set_genre(self, genre: str) -> 'BeatmapsetSearchFilter':
+    def set_genre(self, genre: Union[BeatmapsetGenre, int]) -> "BeatmapsetSearchFilter":
         """
         Set the genre to filter by.
 
         genre: :class:`str`
         """
-        self._filters["g"] = genre
+        self._filters["g"] = genre.value if isinstance(genre, BeatmapsetGenre) else genre
         return self
 
-    def set_extra(self, extras: Sequence[Union[BeatmapsetSearchExtra, str]]) -> 'BeatmapsetSearchFilter':
+    def set_extra(self, extras: Sequence[Union[BeatmapsetSearchExtra, str]]) -> "BeatmapsetSearchFilter":
         """
         Set the extras to filter by.
 
         extras: Sequence[Union[:class:`BeatmapsetSearchExtra`, :class:`str`]]
         """
-        self._filters["e"] = ".".join(list(map(
-            lambda x: x.value if isinstance(x, BeatmapsetSearchExtra) else x, extras)))
+        self._filters["e"] = ".".join(
+            list(
+                map(
+                    lambda x: x.value if isinstance(x, BeatmapsetSearchExtra) else x,
+                    extras,
+                )
+            )
+        )
         return self
 
-    def set_generals(self, generals: Sequence[Union[BeatmapsetSearchGeneral, str]]) -> 'BeatmapsetSearchFilter':
+    def set_generals(self, generals: Sequence[Union[BeatmapsetSearchGeneral, str]]) -> "BeatmapsetSearchFilter":
         """
         Set the generals to filter by.
 
         generals: Sequence[Union[:class:`BeatmapsetSearchGeneral`, :class:`str`]]
         """
-        self._filters["c"] = ".".join(list(map(
-            lambda x: x.value if isinstance(x, BeatmapsetSearchGeneral) else x, generals)))
+        self._filters["c"] = ".".join(
+            list(
+                map(
+                    lambda x: x.value if isinstance(x, BeatmapsetSearchGeneral) else x,
+                    generals,
+                )
+            )
+        )
         return self
 
-    def set_status(self, status: Union[BeatmapsetSearchStatus, str]) -> 'BeatmapsetSearchFilter':
+    def set_status(self, status: Union[BeatmapsetSearchStatus, str]) -> "BeatmapsetSearchFilter":
         """
         Set the status to filter by.
 
         status: Union[:class:`BeatmapsetSearchStatus`, :class:`str`]
         """
         self._filters["s"] = status.value if isinstance(status, BeatmapsetSearchStatus) else status
         return self
 
     @property
-    def filters(self):
+    def filters(self) -> dict:
         """
         Dictionary of all filters only including ones that have been set.
         """
-        return {k: v for k, v in self._filters.items() if v is not None}
+        return dict(filter(lambda item: item[1] is not None, self._filters.items()))
 
 
 class PlaylistItemUtil:
     """
     Util class for passing playlist items to endpoints that involve creating a room
     like create_multiplayer_room and create_playlist.
 
@@ -227,27 +254,34 @@
 
     **Properties**
 
     json: :class:`dict`
         Dictionary format of all the attributes which the client uses
         when sending a http request
     """
+
     __slots__ = ("beatmap_id", "ruleset_id", "allowed_mods", "required_mods")
 
-    def __init__(self, beatmap_id: int, ruleset_id: Union[GameModeInt, int],
-                 allowed_mods: Sequence[Mod] = None, required_mods: Sequence[Mod] = None):
+    def __init__(
+        self,
+        beatmap_id: int,
+        ruleset_id: Union[GameModeInt, int],
+        allowed_mods: Sequence[Mod] = None,
+        required_mods: Sequence[Mod] = None,
+    ):
         self.beatmap_id = beatmap_id
         self.ruleset_id = ruleset_id
         self.allowed_mods = allowed_mods
         self.required_mods = required_mods
 
     @property
     def json(self) -> dict:
         def mod_map(mod):
             return {"acronym": mod.value}
+
         return {
             "beatmap_id": self.beatmap_id,
             "ruleset_id": parse_enum_args(self.ruleset_id),
             "allowed_mods": list(map(mod_map, self.allowed_mods)) if self.allowed_mods is not None else None,
             "required_mods": list(map(mod_map, self.required_mods)) if self.required_mods is not None else None,
         }
 
@@ -273,57 +307,81 @@
 
     @staticmethod
     def parse_list(l):
         return list(map(lambda item: item.json if isinstance(item, JsonUtil) else item, l))
 
     @staticmethod
     def list_to_labeled_dict(l, name):
-        return dict(sum(map(
-            lambda i: list(map(
-                lambda i2: (f"{name}[{i[0]}][{i2[0]}]", f"{i2[1]}"),
-                filter(lambda i2: i2[1] is not None, i[1].items())
-            )),
-            enumerate(l)
-        ), []))
+        return dict(
+            sum(
+                map(
+                    lambda i: list(
+                        map(
+                            lambda i2: (f"{name}[{i[0]}][{i2[0]}]", f"{i2[1]}"),
+                            filter(lambda i2: i2[1] is not None, i[1].items()),
+                        )
+                    ),
+                    enumerate(l),
+                ),
+                [],
+            )
+        )
 
 
 class NotificationsUtil(JsonUtil):
-    __slots__ = ("category", "id", "object_id", "object_type")
+    """
+    **Init parameters**
 
-    def __init__(self, category: Union[NotificationCategory, str] = None, id: int = None,
-                 object_id: str = None, object_type: Union[ObjectType, str] = None):
-        """
-        **Arguments**
+    category: Optional[Union[:class:`str`, :class:`NotificationCategory`]]
+        Notification category.
 
-        category: Optional[:class:`str`]
-            Notification category.
+    id: Optional[:class:`id`]
+        Id of notification to be marked as read
 
-        id: Optional[:class:`id`]
-            Id of notification to be marked as read
+    object_id: Optional[:class:`str`]
+        Id of the object that triggered the notification
 
-        object_id: Optional[:class:`str`]
-            Id of the object that triggered the notification
+    object_type: Optional[Union[:class:`str`, :class:`ObjectType`]]
+        Type of the object that triggered the notification
+    """
+    __slots__ = ("category", "id", "object_id", "object_type")
 
-        object_type: Optional[:class:`str`]
-            Type of the object that triggered the notification
-        """
+    def __init__(
+        self,
+        category: Optional[Union[NotificationCategory, str]] = None,
+        id: Optional[int] = None,
+        object_id: Optional[str] = None,
+        object_type: Optional[Union[ObjectType, str]] = None,
+    ):
         super().__init__(*parse_enum_args(category, id, object_id, object_type))
 
 
 class IdentitiesUtil(JsonUtil):
-    __slots__ = ("category", "object_id", "object_type")
+    """
+    **Init parameters**
 
-    def __init__(self, category: Union[NotificationCategory, str] = None, object_id: str = None,
-                 object_type: Union[ObjectType, str] = None):
-        """
-        **Arguments**
+    category: Optional[Union[:class:`str`, :class:`NotificationCategory`]]
+        Notification category.
 
-        category: Optional[:class:`str`]
-            Notification category.
+    object_id: Optional[:class:`str`]
+        Id of the object that triggered the notification
 
-        object_id: Optional[:class:`str`]
-            Id of the object that triggered the notification
+    object_type: Optional[Union[:class:`str`, :class:`ObjectType`]]
+        Type of the object that triggered the notification
+    """
+    __slots__ = ("category", "object_id", "object_type")
 
-        object_type: Optional[:class:`str`]
-            Type of the object that triggered the notification
-        """
+    def __init__(
+        self,
+        category: Optional[Union[NotificationCategory, str]] = None,
+        object_id: Optional[str] = None,
+        object_type: Optional[Union[ObjectType, str]] = None,
+    ):
         super().__init__(*parse_enum_args(category, object_id, object_type))
+
+
+def get_optional(data: Dict[str, _V], key: str, call: Callable[[_V], _T]) -> Optional[_T]:
+    return call(value) if (value := data.get(key)) is not None else None
+
+
+def get_optional_list(data: Dict[str, _V], key: str, obj: Callable[[_V], _T]) -> Optional[List[_T]]:
+    return list(map(obj, value)) if (value := data.get(key)) is not None else None
```

### Comparing `osu.py-0.6.0/osu.py.egg-info/PKG-INFO` & `osu.py-1.0.0/osu.py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osu.py
-Version: 0.6.0
+Version: 1.0.0
 Summary: API Wrapper for osu!api v2 written in Python.
 Home-page: https://github.com/Sheepposu/osu.py
 Author: Sheepposu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Sheepposu/osu.py/issues
 Project-URL: osu.py documentation, https://osupy.readthedocs.io/
 Project-URL: osu!api v2 documentation, https://osu.ppy.sh/docs/index.html
```

### Comparing `osu.py-0.6.0/osu.py.egg-info/SOURCES.txt` & `osu.py-1.0.0/osu.py.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -7,29 +7,32 @@
 osu/client.py
 osu/constants.py
 osu/enums.py
 osu/exceptions.py
 osu/http.py
 osu/notification.py
 osu/path.py
+osu/results.py
 osu/util.py
 osu.py.egg-info/PKG-INFO
 osu.py.egg-info/SOURCES.txt
 osu.py.egg-info/dependency_links.txt
 osu.py.egg-info/requires.txt
 osu.py.egg-info/top_level.txt
 osu/asyncio/__init__.py
 osu/asyncio/client.py
 osu/asyncio/http.py
 osu/objects/__init__.py
+osu/objects/achievement.py
 osu/objects/beatmap.py
 osu/objects/beatmapset_event.py
 osu/objects/build.py
 osu/objects/chat.py
 osu/objects/comment.py
+osu/objects/current_user_attributes.py
 osu/objects/discussion.py
 osu/objects/event.py
 osu/objects/forum.py
 osu/objects/group.py
 osu/objects/kudosu.py
 osu/objects/match.py
 osu/objects/multiplayer.py
```

### Comparing `osu.py-0.6.0/setup.py` & `osu.py-1.0.0/setup.py`

 * *Files identical despite different names*

