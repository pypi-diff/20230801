# Comparing `tmp/osuExchange-0.0.2.tar.gz` & `tmp/osuExchange-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osuExchange-0.0.2.tar", last modified: Mon Jul 31 22:57:24 2023, max compression
+gzip compressed data, was "osuExchange-0.0.3.tar", last modified: Mon Jul 31 23:01:22 2023, max compression
```

## Comparing `osuExchange-0.0.2.tar` & `osuExchange-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 t_        (1000) t_        (1000)        0 2023-07-31 22:57:24.312741 osuExchange-0.0.2/
--rw-r--r--   0 t_        (1000) t_        (1000)      831 2023-07-31 22:57:24.312741 osuExchange-0.0.2/PKG-INFO
--rw-r--r--   0 t_        (1000) t_        (1000)      583 2023-07-23 17:42:53.000000 osuExchange-0.0.2/README.md
-drwxr-xr-x   0 t_        (1000) t_        (1000)        0 2023-07-31 22:57:24.312741 osuExchange-0.0.2/osuExchange/
--rw-r--r--   0 t_        (1000) t_        (1000)      166 2023-07-29 00:24:28.000000 osuExchange-0.0.2/osuExchange/__init__.py
--rw-r--r--   0 t_        (1000) t_        (1000)     1320 2023-07-29 01:23:40.000000 osuExchange-0.0.2/osuExchange/api.py
--rw-r--r--   0 t_        (1000) t_        (1000)     4353 2023-07-15 03:35:17.000000 osuExchange-0.0.2/osuExchange/auth.py
--rw-r--r--   0 t_        (1000) t_        (1000)     7836 2023-07-29 00:25:40.000000 osuExchange-0.0.2/osuExchange/beatmaps.py
--rw-r--r--   0 t_        (1000) t_        (1000)     2712 2023-07-29 01:32:24.000000 osuExchange-0.0.2/osuExchange/client.py
--rw-r--r--   0 t_        (1000) t_        (1000)     3399 2023-07-29 00:24:28.000000 osuExchange-0.0.2/osuExchange/scores.py
--rw-r--r--   0 t_        (1000) t_        (1000)      753 2023-07-29 01:14:28.000000 osuExchange-0.0.2/osuExchange/seasonalbg.py
--rw-r--r--   0 t_        (1000) t_        (1000)      221 2023-07-14 21:26:15.000000 osuExchange-0.0.2/osuExchange/typing.py
--rw-r--r--   0 t_        (1000) t_        (1000)     6833 2023-07-15 18:41:10.000000 osuExchange-0.0.2/osuExchange/users.py
--rw-r--r--   0 t_        (1000) t_        (1000)      671 2023-07-15 03:35:17.000000 osuExchange-0.0.2/osuExchange/util.py
-drwxr-xr-x   0 t_        (1000) t_        (1000)        0 2023-07-31 22:57:24.312741 osuExchange-0.0.2/osuExchange.egg-info/
--rw-r--r--   0 t_        (1000) t_        (1000)      831 2023-07-31 22:57:24.000000 osuExchange-0.0.2/osuExchange.egg-info/PKG-INFO
--rw-r--r--   0 t_        (1000) t_        (1000)      418 2023-07-31 22:57:24.000000 osuExchange-0.0.2/osuExchange.egg-info/SOURCES.txt
--rw-r--r--   0 t_        (1000) t_        (1000)        1 2023-07-31 22:57:24.000000 osuExchange-0.0.2/osuExchange.egg-info/dependency_links.txt
--rw-r--r--   0 t_        (1000) t_        (1000)        9 2023-07-31 22:57:24.000000 osuExchange-0.0.2/osuExchange.egg-info/requires.txt
--rw-r--r--   0 t_        (1000) t_        (1000)       12 2023-07-31 22:57:24.000000 osuExchange-0.0.2/osuExchange.egg-info/top_level.txt
--rw-r--r--   0 t_        (1000) t_        (1000)      293 2023-07-31 22:57:12.000000 osuExchange-0.0.2/pyproject.toml
--rw-r--r--   0 t_        (1000) t_        (1000)       38 2023-07-31 22:57:24.312741 osuExchange-0.0.2/setup.cfg
+drwxr-xr-x   0 t_        (1000) t_        (1000)        0 2023-07-31 23:01:22.149796 osuExchange-0.0.3/
+-rw-r--r--   0 t_        (1000) t_        (1000)      831 2023-07-31 23:01:22.149796 osuExchange-0.0.3/PKG-INFO
+-rw-r--r--   0 t_        (1000) t_        (1000)      583 2023-07-23 17:42:53.000000 osuExchange-0.0.3/README.md
+drwxr-xr-x   0 t_        (1000) t_        (1000)        0 2023-07-31 23:01:22.149796 osuExchange-0.0.3/osuExchange/
+-rw-r--r--   0 t_        (1000) t_        (1000)      166 2023-07-29 00:24:28.000000 osuExchange-0.0.3/osuExchange/__init__.py
+-rw-r--r--   0 t_        (1000) t_        (1000)     1320 2023-07-29 01:23:40.000000 osuExchange-0.0.3/osuExchange/api.py
+-rw-r--r--   0 t_        (1000) t_        (1000)     4353 2023-07-15 03:35:17.000000 osuExchange-0.0.3/osuExchange/auth.py
+-rw-r--r--   0 t_        (1000) t_        (1000)     7836 2023-07-29 00:25:40.000000 osuExchange-0.0.3/osuExchange/beatmaps.py
+-rw-r--r--   0 t_        (1000) t_        (1000)     2747 2023-07-31 23:00:29.000000 osuExchange-0.0.3/osuExchange/client.py
+-rw-r--r--   0 t_        (1000) t_        (1000)     3399 2023-07-29 00:24:28.000000 osuExchange-0.0.3/osuExchange/scores.py
+-rw-r--r--   0 t_        (1000) t_        (1000)      753 2023-07-29 01:14:28.000000 osuExchange-0.0.3/osuExchange/seasonalbg.py
+-rw-r--r--   0 t_        (1000) t_        (1000)      221 2023-07-14 21:26:15.000000 osuExchange-0.0.3/osuExchange/typing.py
+-rw-r--r--   0 t_        (1000) t_        (1000)     6833 2023-07-15 18:41:10.000000 osuExchange-0.0.3/osuExchange/users.py
+-rw-r--r--   0 t_        (1000) t_        (1000)      671 2023-07-15 03:35:17.000000 osuExchange-0.0.3/osuExchange/util.py
+drwxr-xr-x   0 t_        (1000) t_        (1000)        0 2023-07-31 23:01:22.149796 osuExchange-0.0.3/osuExchange.egg-info/
+-rw-r--r--   0 t_        (1000) t_        (1000)      831 2023-07-31 23:01:22.000000 osuExchange-0.0.3/osuExchange.egg-info/PKG-INFO
+-rw-r--r--   0 t_        (1000) t_        (1000)      418 2023-07-31 23:01:22.000000 osuExchange-0.0.3/osuExchange.egg-info/SOURCES.txt
+-rw-r--r--   0 t_        (1000) t_        (1000)        1 2023-07-31 23:01:22.000000 osuExchange-0.0.3/osuExchange.egg-info/dependency_links.txt
+-rw-r--r--   0 t_        (1000) t_        (1000)        9 2023-07-31 23:01:22.000000 osuExchange-0.0.3/osuExchange.egg-info/requires.txt
+-rw-r--r--   0 t_        (1000) t_        (1000)       12 2023-07-31 23:01:22.000000 osuExchange-0.0.3/osuExchange.egg-info/top_level.txt
+-rw-r--r--   0 t_        (1000) t_        (1000)      293 2023-07-31 23:00:53.000000 osuExchange-0.0.3/pyproject.toml
+-rw-r--r--   0 t_        (1000) t_        (1000)       38 2023-07-31 23:01:22.149796 osuExchange-0.0.3/setup.cfg
```

### Comparing `osuExchange-0.0.2/PKG-INFO` & `osuExchange-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osuExchange
-Version: 0.0.2
+Version: 0.0.3
 Summary: A simple osu!APIv2 wrapper for Python
 Author: trustytrojan, alittlerocket
 Project-URL: Homepage, https://github.com/alittlerocket/osuExchange
 Description-Content-Type: text/markdown
 
 # osuExchange
```

### Comparing `osuExchange-0.0.2/README.md` & `osuExchange-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `osuExchange-0.0.2/osuExchange/api.py` & `osuExchange-0.0.3/osuExchange/api.py`

 * *Files identical despite different names*

### Comparing `osuExchange-0.0.2/osuExchange/auth.py` & `osuExchange-0.0.3/osuExchange/auth.py`

 * *Files identical despite different names*

### Comparing `osuExchange-0.0.2/osuExchange/beatmaps.py` & `osuExchange-0.0.3/osuExchange/beatmaps.py`

 * *Files identical despite different names*

### Comparing `osuExchange-0.0.2/osuExchange/client.py` & `osuExchange-0.0.3/osuExchange/client.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,28 @@
 from osuExchange.users import get_user, get_users, User, UserCompact
 from osuExchange.beatmaps import get_beatmap, get_beatmaps, Beatmap
 from osuExchange.scores import get_beatmap_scores, get_score, get_user_beatmap_scores, BeatmapScores, Score, BeatmapUserScore
 from osuExchange.seasonalbg import get_seasonal_backgrounds, SeasonalBackgrounds
 from osuExchange.auth import get_access_token, get_client_credentials_token, ClientCredentialsToken, UserAccessToken, OAuth2Scope
 from osuExchange.typing import GameMode, Literal
 
-class OAuth2Client:
-	def __init__(self):
+class OsuApiClient:
+	def __init__(self, client_id: str, client_secret: str):
 		self.token_obj: ClientCredentialsToken | UserAccessToken | None = None
+		self.client_id = client_id
+		self.client_secret = client_secret
 
 	def get_user_access_token(self,
-		client_id: str, 
-		client_secret: str, 
 		redirect_uri: str,
 		scopes: list[OAuth2Scope]
 	) -> None:
-		self.token_obj = get_access_token(client_id, client_secret, redirect_uri, scopes)
+		self.token_obj = get_access_token(self.client_id, self.client_secret, redirect_uri, scopes)
 		
-	def get_client_credentials_token(
-		self,
-		client_id: str,
-		client_secret: str
-	) -> None:
-		self.token_obj = get_client_credentials_token(client_id, client_secret)
+	def get_client_credentials_token(self) -> None:
+		self.token_obj = get_client_credentials_token(self.client_id, self.client_secret)
 
 	def __raise_authenticate__(self):
 		return Exception('self.token_obj is None; please authenticate')
 
 	def get_user(self,
 		id: int,
 		mode: GameMode | None,
```

### Comparing `osuExchange-0.0.2/osuExchange/scores.py` & `osuExchange-0.0.3/osuExchange/scores.py`

 * *Files identical despite different names*

### Comparing `osuExchange-0.0.2/osuExchange/seasonalbg.py` & `osuExchange-0.0.3/osuExchange/seasonalbg.py`

 * *Files identical despite different names*

### Comparing `osuExchange-0.0.2/osuExchange/users.py` & `osuExchange-0.0.3/osuExchange/users.py`

 * *Files identical despite different names*

### Comparing `osuExchange-0.0.2/osuExchange/util.py` & `osuExchange-0.0.3/osuExchange/util.py`

 * *Files identical despite different names*

### Comparing `osuExchange-0.0.2/osuExchange.egg-info/PKG-INFO` & `osuExchange-0.0.3/osuExchange.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osuExchange
-Version: 0.0.2
+Version: 0.0.3
 Summary: A simple osu!APIv2 wrapper for Python
 Author: trustytrojan, alittlerocket
 Project-URL: Homepage, https://github.com/alittlerocket/osuExchange
 Description-Content-Type: text/markdown
 
 # osuExchange
```

