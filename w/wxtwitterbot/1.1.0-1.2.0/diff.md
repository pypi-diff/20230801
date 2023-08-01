# Comparing `tmp/wxtwitterbot-1.1.0-py3-none-any.whl.zip` & `tmp/wxtwitterbot-1.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 12297 bytes, number of entries: 14
--rw-r--r--  2.0 unx        0 b- defN 22-Sep-30 15:32 wxtwitterbot/__init__.py
--rw-r--r--  2.0 unx      117 b- defN 22-Sep-30 15:32 wxtwitterbot/const.py
--rw-r--r--  2.0 unx      586 b- defN 22-Sep-30 15:32 wxtwitterbot/envvarname.py
--rw-r--r--  2.0 unx     1916 b- defN 22-Sep-30 15:32 wxtwitterbot/main.py
--rw-r--r--  2.0 unx     2403 b- defN 22-Sep-30 15:32 wxtwitterbot/twitter.py
--rw-r--r--  2.0 unx     3276 b- defN 22-Sep-30 15:32 wxtwitterbot/util.py
--rw-r--r--  2.0 unx        0 b- defN 22-Sep-30 15:32 wxtwitterbot/tasks/__init__.py
--rw-r--r--  2.0 unx    10090 b- defN 22-Sep-30 15:32 wxtwitterbot/tasks/lunartime.py
--rw-r--r--  2.0 unx     6789 b- defN 22-Sep-30 15:32 wxtwitterbot/tasks/solartime.py
--rw-r--r--  2.0 unx     1089 b- defN 22-Sep-30 15:32 wxtwitterbot-1.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     3308 b- defN 22-Sep-30 15:32 wxtwitterbot-1.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Sep-30 15:32 wxtwitterbot-1.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 22-Sep-30 15:32 wxtwitterbot-1.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1143 b- defN 22-Sep-30 15:32 wxtwitterbot-1.1.0.dist-info/RECORD
-14 files, 30822 bytes uncompressed, 10391 bytes compressed:  66.3%
+Zip file size: 12286 bytes, number of entries: 14
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-01 03:52 wxtwitterbot/__init__.py
+-rw-r--r--  2.0 unx      117 b- defN 23-Aug-01 03:52 wxtwitterbot/const.py
+-rw-r--r--  2.0 unx      586 b- defN 23-Aug-01 03:52 wxtwitterbot/envvarname.py
+-rw-r--r--  2.0 unx     1916 b- defN 23-Aug-01 03:52 wxtwitterbot/main.py
+-rw-r--r--  2.0 unx     2337 b- defN 23-Aug-01 03:52 wxtwitterbot/twitter.py
+-rw-r--r--  2.0 unx     3276 b- defN 23-Aug-01 03:52 wxtwitterbot/util.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-01 03:52 wxtwitterbot/tasks/__init__.py
+-rw-r--r--  2.0 unx    10090 b- defN 23-Aug-01 03:52 wxtwitterbot/tasks/lunartime.py
+-rw-r--r--  2.0 unx     6789 b- defN 23-Aug-01 03:52 wxtwitterbot/tasks/solartime.py
+-rw-r--r--  2.0 unx     1089 b- defN 23-Aug-01 03:53 wxtwitterbot-1.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3308 b- defN 23-Aug-01 03:53 wxtwitterbot-1.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-01 03:53 wxtwitterbot-1.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 23-Aug-01 03:53 wxtwitterbot-1.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1143 b- defN 23-Aug-01 03:53 wxtwitterbot-1.2.0.dist-info/RECORD
+14 files, 30756 bytes uncompressed, 10380 bytes compressed:  66.3%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: wxtwitterbot/tasks/lunartime.py
 Comment: 
 
 Filename: wxtwitterbot/tasks/solartime.py
 Comment: 
 
-Filename: wxtwitterbot-1.1.0.dist-info/LICENSE
+Filename: wxtwitterbot-1.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: wxtwitterbot-1.1.0.dist-info/METADATA
+Filename: wxtwitterbot-1.2.0.dist-info/METADATA
 Comment: 
 
-Filename: wxtwitterbot-1.1.0.dist-info/WHEEL
+Filename: wxtwitterbot-1.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: wxtwitterbot-1.1.0.dist-info/top_level.txt
+Filename: wxtwitterbot-1.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: wxtwitterbot-1.1.0.dist-info/RECORD
+Filename: wxtwitterbot-1.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## wxtwitterbot/twitter.py

```diff
@@ -1,11 +1,11 @@
 import logging
 
 from envvarname import EnvVarName
-from tweepy import API, OAuthHandler
+from tweepy import API, OAuth1UserHandler
 from util import getEnvVar, isEmpty
 
 
 class TwitterUtil(object):
 
     LOGGER = logging.getLogger()
 
@@ -47,19 +47,17 @@
 
         access_token_secret = getEnvVar(EnvVarName.TWITTER_ACCESS_TOKEN_SECRET)
         if (isEmpty(access_token_secret)):
             message = "Environment Variable " + EnvVarName.TWITTER_ACCESS_TOKEN_SECRET.name + " is not set"
             TwitterUtil.LOGGER.error(message)
             raise RuntimeError(message)
 
-        auth = OAuthHandler(consumer_key, consumer_secret)
-        auth.set_access_token(access_token, access_token_secret)
+        auth = OAuth1UserHandler(consumer_key, consumer_secret, access_token, access_token_secret)
         api = API(auth,
-            wait_on_rate_limit=True,
-            wait_on_rate_limit_notify=True)
+            wait_on_rate_limit=True)
 
         try:
             api.verify_credentials()
         except Exception as e:
             TwitterUtil.LOGGER.error("Error creating Twitter API", exc_info=True)
             raise e
```

## Comparing `wxtwitterbot-1.1.0.dist-info/LICENSE` & `wxtwitterbot-1.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `wxtwitterbot-1.1.0.dist-info/METADATA` & `wxtwitterbot-1.2.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wxtwitterbot
-Version: 1.1.0
+Version: 1.2.0
 Summary: Wx Twitter Bot
 Home-page: https://github.com/karjanme/wx-twitter-bot
 Author: Karl Jansen
 Author-email: jnsnkrl@live.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

## Comparing `wxtwitterbot-1.1.0.dist-info/RECORD` & `wxtwitterbot-1.2.0.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 wxtwitterbot/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 wxtwitterbot/const.py,sha256=xQgc0kCMvg2gTz_P-SKXeF7Um9GeXN8rV4UVV9KuDJ0,117
 wxtwitterbot/envvarname.py,sha256=34Rn_LwXgZypYy5hqTmxXUMcPj0-URserHDXDdRQZE4,586
 wxtwitterbot/main.py,sha256=7LcPJedzBpkxy9aMLFJP9QVEvP4kxPo6FlLzehIuYg4,1916
-wxtwitterbot/twitter.py,sha256=ofv6sokrbG9mUV-GcMdrrQlw-Mk-VPCNVbRffjw9aFQ,2403
+wxtwitterbot/twitter.py,sha256=2DTn4nzmKtyz8jAZfSyGyeCnW_t8ru3GucmFk-kmHPw,2337
 wxtwitterbot/util.py,sha256=_xAIbDV-FXzmwv6sNx1xYzuYDJROENmBNOa_OlFc9Zw,3276
 wxtwitterbot/tasks/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 wxtwitterbot/tasks/lunartime.py,sha256=tRWNxMZak3IhDvTTNj4XFDh-yCyQJxaqVTJEfzp0XS4,10090
 wxtwitterbot/tasks/solartime.py,sha256=bdrfHkCJYcUyAw14z0Nb3iGEU1O3X5D8WcIlX0kHK7A,6789
-wxtwitterbot-1.1.0.dist-info/LICENSE,sha256=bnsVbzmAoVOrNQX0IGjbGjm-57l0YA8-9pAJ5ItCeTc,1089
-wxtwitterbot-1.1.0.dist-info/METADATA,sha256=ka4uhc-n0v8PgCUmY6pYdoq-ZgDeC0C6f_GIEy7yFec,3308
-wxtwitterbot-1.1.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-wxtwitterbot-1.1.0.dist-info/top_level.txt,sha256=9-v__TX_uLgBTeYqONTcWzPKSq1AFpzUV_ZffxW6_NY,13
-wxtwitterbot-1.1.0.dist-info/RECORD,,
+wxtwitterbot-1.2.0.dist-info/LICENSE,sha256=bnsVbzmAoVOrNQX0IGjbGjm-57l0YA8-9pAJ5ItCeTc,1089
+wxtwitterbot-1.2.0.dist-info/METADATA,sha256=pKFFdyBGWhsk5wsKuYGJRr9T6pBwEZ3i2BX_l-HW7-4,3308
+wxtwitterbot-1.2.0.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+wxtwitterbot-1.2.0.dist-info/top_level.txt,sha256=9-v__TX_uLgBTeYqONTcWzPKSq1AFpzUV_ZffxW6_NY,13
+wxtwitterbot-1.2.0.dist-info/RECORD,,
```

