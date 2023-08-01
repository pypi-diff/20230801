# Comparing `tmp/fastapi-oauth2-1.0.0a0.tar.gz` & `tmp/fastapi-oauth2-1.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-oauth2-1.0.0a0.tar", last modified: Thu Jul 13 10:33:36 2023, max compression
+gzip compressed data, was "fastapi-oauth2-1.0.0a1.tar", last modified: Tue Aug  1 13:01:30 2023, max compression
```

## Comparing `fastapi-oauth2-1.0.0a0.tar` & `fastapi-oauth2-1.0.0a1.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:33:36.258821 fastapi-oauth2-1.0.0a0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-13 10:33:25.000000 fastapi-oauth2-1.0.0a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-07-13 10:33:36.258821 fastapi-oauth2-1.0.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-07-13 10:33:25.000000 fastapi-oauth2-1.0.0a0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-13 10:33:25.000000 fastapi-oauth2-1.0.0a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-13 10:33:36.258821 fastapi-oauth2-1.0.0a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-13 10:33:25.000000 fastapi-oauth2-1.0.0a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:33:36.258821 fastapi-oauth2-1.0.0a0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:33:36.258821 fastapi-oauth2-1.0.0a0/src/fastapi_oauth2/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-13 10:33:25.000000 fastapi-oauth2-1.0.0a0/src/fastapi_oauth2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-13 10:33:25.000000 fastapi-oauth2-1.0.0a0/src/fastapi_oauth2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-13 10:33:25.000000 fastapi-oauth2-1.0.0a0/src/fastapi_oauth2/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-07-13 10:33:25.000000 fastapi-oauth2-1.0.0a0/src/fastapi_oauth2/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-07-13 10:33:25.000000 fastapi-oauth2-1.0.0a0/src/fastapi_oauth2/middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-07-13 10:33:25.000000 fastapi-oauth2-1.0.0a0/src/fastapi_oauth2/router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:33:36.258821 fastapi-oauth2-1.0.0a0/src/fastapi_oauth2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-07-13 10:33:36.000000 fastapi-oauth2-1.0.0a0/src/fastapi_oauth2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-13 10:33:36.000000 fastapi-oauth2-1.0.0a0/src/fastapi_oauth2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 10:33:36.000000 fastapi-oauth2-1.0.0a0/src/fastapi_oauth2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 10:33:36.000000 fastapi-oauth2-1.0.0a0/src/fastapi_oauth2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-13 10:33:36.000000 fastapi-oauth2-1.0.0a0/src/fastapi_oauth2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-13 10:33:36.000000 fastapi-oauth2-1.0.0a0/src/fastapi_oauth2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:01:30.301951 fastapi-oauth2-1.0.0a1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-01 13:01:21.000000 fastapi-oauth2-1.0.0a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-08-01 13:01:30.301951 fastapi-oauth2-1.0.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-08-01 13:01:21.000000 fastapi-oauth2-1.0.0a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-08-01 13:01:21.000000 fastapi-oauth2-1.0.0a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-08-01 13:01:30.301951 fastapi-oauth2-1.0.0a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-01 13:01:21.000000 fastapi-oauth2-1.0.0a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:01:30.301951 fastapi-oauth2-1.0.0a1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:01:30.301951 fastapi-oauth2-1.0.0a1/src/fastapi_oauth2/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-01 13:01:21.000000 fastapi-oauth2-1.0.0a1/src/fastapi_oauth2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-08-01 13:01:21.000000 fastapi-oauth2-1.0.0a1/src/fastapi_oauth2/claims.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-08-01 13:01:21.000000 fastapi-oauth2-1.0.0a1/src/fastapi_oauth2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-08-01 13:01:21.000000 fastapi-oauth2-1.0.0a1/src/fastapi_oauth2/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-08-01 13:01:21.000000 fastapi-oauth2-1.0.0a1/src/fastapi_oauth2/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5924 2023-08-01 13:01:21.000000 fastapi-oauth2-1.0.0a1/src/fastapi_oauth2/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-08-01 13:01:21.000000 fastapi-oauth2-1.0.0a1/src/fastapi_oauth2/router.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-08-01 13:01:21.000000 fastapi-oauth2-1.0.0a1/src/fastapi_oauth2/security.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:01:30.301951 fastapi-oauth2-1.0.0a1/src/fastapi_oauth2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-08-01 13:01:30.000000 fastapi-oauth2-1.0.0a1/src/fastapi_oauth2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-08-01 13:01:30.000000 fastapi-oauth2-1.0.0a1/src/fastapi_oauth2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 13:01:30.000000 fastapi-oauth2-1.0.0a1/src/fastapi_oauth2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 13:01:30.000000 fastapi-oauth2-1.0.0a1/src/fastapi_oauth2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-01 13:01:30.000000 fastapi-oauth2-1.0.0a1/src/fastapi_oauth2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-01 13:01:30.000000 fastapi-oauth2-1.0.0a1/src/fastapi_oauth2.egg-info/top_level.txt
```

### Comparing `fastapi-oauth2-1.0.0a0/LICENSE` & `fastapi-oauth2-1.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi-oauth2-1.0.0a0/PKG-INFO` & `fastapi-oauth2-1.0.0a1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-oauth2
-Version: 1.0.0a0
+Version: 1.0.0a1
 Summary: Easy to setup OAuth2 authentication with support for several auth providers.
 Author: Artyom Vancyan
 Author-email: artyom@pysnippet.org
 License: MIT
 Project-URL: Documentation, https://github.com/pysnippet/fastapi-oauth2/
 Project-URL: Source Code, https://github.com/pysnippet/fastapi-oauth2/
 Keywords: python,sso,auth,login,oauth,oauth2,social,fastapi,allauth,security,middleware,authentication
@@ -13,21 +13,21 @@
 Platform: osx
 Platform: win32
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: FastAPI
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # fastapi-oauth2 <img src="https://github.com/pysnippet.png" align="right" height="64" />
 
 [![PyPI](https://img.shields.io/pypi/v/fastapi-oauth2.svg)](https://pypi.org/project/fastapi-oauth2/)
 [![Python](https://img.shields.io/pypi/pyversions/fastapi-oauth2.svg?logoColor=white)](https://pypi.org/project/fastapi-oauth2/)
@@ -38,18 +38,15 @@
 FastAPI OAuth2 is a middleware-based social authentication mechanism supporting several auth providers. It depends on
 the [social-core](https://github.com/python-social-auth/social-core) authentication backends.
 
 ## Features to be implemented
 
 - Use multiple OAuth2 providers at the same time
     * There need to be provided a way to configure the OAuth2 for multiple providers
-- Provide `fastapi.security.*` implementations that use cookies
-- Token -> user data, user data -> token easy conversion
 - Customizable OAuth2 routes
-- Registration support
 
 ## Installation
 
 ```shell
 python -m pip install fastapi-oauth2
 ```
 
@@ -69,20 +66,22 @@
 ### OAuth2Client
 
 - `backend` - The [social-core](https://github.com/python-social-auth/social-core) authentication backend classname.
 - `client_id` - The OAuth2 client ID for the particular provider.
 - `client_secret` - The OAuth2 client secret for the particular provider.
 - `redirect_uri` - The OAuth2 redirect URI to redirect to after success. Defaults to the base URL.
 - `scope` - The OAuth2 scope for the particular provider. Defaults to `[]`.
+- `claims` - Claims mapping for the certain provider.
 
 It is also important to mention that for the configured clients of the auth providers, the authorization URLs are
 accessible by the `/oauth2/{provider}/auth` path where the `provider` variable represents the exact value of the auth
 provider backend `name` attribute.
 
 ```python
+from fastapi_oauth2.claims import Claims
 from fastapi_oauth2.client import OAuth2Client
 from fastapi_oauth2.config import OAuth2Config
 from social_core.backends.github import GithubOAuth2
 
 oauth2_config = OAuth2Config(
     allow_http=False,
     jwt_secret=os.getenv("JWT_SECRET"),
@@ -91,14 +90,18 @@
     clients=[
         OAuth2Client(
             backend=GithubOAuth2,
             client_id=os.getenv("OAUTH2_CLIENT_ID"),
             client_secret=os.getenv("OAUTH2_CLIENT_SECRET"),
             redirect_uri="https://pysnippet.org/",
             scope=["user:email"],
+            claims=Claims(
+                picture="avatar_url",
+                identity=lambda user: "%s:%s" % (user.get("provider"), user.get("id")),
+            ),
         ),
     ]
 )
 ```
 
 ## Integration
```

### Comparing `fastapi-oauth2-1.0.0a0/README.md` & `fastapi-oauth2-1.0.0a1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -63,215 +63,222 @@
 000003e0: 204f 4175 7468 3220 7072 6f76 6964 6572   OAuth2 provider
 000003f0: 7320 6174 2074 6865 2073 616d 6520 7469  s at the same ti
 00000400: 6d65 0a20 2020 202a 2054 6865 7265 206e  me.    * There n
 00000410: 6565 6420 746f 2062 6520 7072 6f76 6964  eed to be provid
 00000420: 6564 2061 2077 6179 2074 6f20 636f 6e66  ed a way to conf
 00000430: 6967 7572 6520 7468 6520 4f41 7574 6832  igure the OAuth2
 00000440: 2066 6f72 206d 756c 7469 706c 6520 7072   for multiple pr
-00000450: 6f76 6964 6572 730a 2d20 5072 6f76 6964  oviders.- Provid
-00000460: 6520 6066 6173 7461 7069 2e73 6563 7572  e `fastapi.secur
-00000470: 6974 792e 2a60 2069 6d70 6c65 6d65 6e74  ity.*` implement
-00000480: 6174 696f 6e73 2074 6861 7420 7573 6520  ations that use 
-00000490: 636f 6f6b 6965 730a 2d20 546f 6b65 6e20  cookies.- Token 
-000004a0: 2d3e 2075 7365 7220 6461 7461 2c20 7573  -> user data, us
-000004b0: 6572 2064 6174 6120 2d3e 2074 6f6b 656e  er data -> token
-000004c0: 2065 6173 7920 636f 6e76 6572 7369 6f6e   easy conversion
-000004d0: 0a2d 2043 7573 746f 6d69 7a61 626c 6520  .- Customizable 
-000004e0: 4f41 7574 6832 2072 6f75 7465 730a 2d20  OAuth2 routes.- 
-000004f0: 5265 6769 7374 7261 7469 6f6e 2073 7570  Registration sup
-00000500: 706f 7274 0a0a 2323 2049 6e73 7461 6c6c  port..## Install
-00000510: 6174 696f 6e0a 0a60 6060 7368 656c 6c0a  ation..```shell.
-00000520: 7079 7468 6f6e 202d 6d20 7069 7020 696e  python -m pip in
-00000530: 7374 616c 6c20 6661 7374 6170 692d 6f61  stall fastapi-oa
-00000540: 7574 6832 0a60 6060 0a0a 2323 2043 6f6e  uth2.```..## Con
-00000550: 6669 6775 7261 7469 6f6e 0a0a 436f 6e66  figuration..Conf
-00000560: 6967 7572 6174 696f 6e20 7265 7175 6972  iguration requir
-00000570: 6573 2079 6f75 2074 6f20 7072 6f76 6964  es you to provid
-00000580: 6520 7468 6520 4a57 5420 7265 7175 6973  e the JWT requis
-00000590: 6974 6573 2061 6e64 2064 6566 696e 6520  ites and define 
-000005a0: 7468 6520 636c 6965 6e74 7320 6f66 2074  the clients of t
-000005b0: 6865 2070 6172 7469 6375 6c61 7220 7072  he particular pr
-000005c0: 6f76 6964 6572 732e 2054 6865 0a6d 6964  oviders. The.mid
-000005d0: 646c 6577 6172 6520 636f 6e66 6967 7572  dleware configur
-000005e0: 6174 696f 6e20 6973 2064 6563 6c61 7265  ation is declare
-000005f0: 6420 7769 7468 2074 6865 2060 4f41 7574  d with the `OAut
-00000600: 6832 436f 6e66 6967 6020 616e 6420 604f  h2Config` and `O
-00000610: 4175 7468 3243 6c69 656e 7460 2063 6c61  Auth2Client` cla
-00000620: 7373 6573 2e0a 0a23 2323 204f 4175 7468  sses...### OAuth
-00000630: 3243 6f6e 6669 670a 0a2d 2060 616c 6c6f  2Config..- `allo
-00000640: 775f 6874 7470 6020 2d20 416c 6c6f 7720  w_http` - Allow 
-00000650: 696e 7365 6375 7265 2048 5454 5020 7265  insecure HTTP re
-00000660: 7175 6573 7473 2e20 4465 6661 756c 7473  quests. Defaults
-00000670: 2074 6f20 6046 616c 7365 602e 0a2d 2060   to `False`..- `
-00000680: 6a77 745f 7365 6372 6574 6020 2d20 5468  jwt_secret` - Th
-00000690: 6520 7365 6372 6574 206b 6579 2075 7365  e secret key use
-000006a0: 6420 746f 2073 6967 6e20 7468 6520 4a57  d to sign the JW
-000006b0: 542e 2044 6566 6175 6c74 7320 746f 2060  T. Defaults to `
-000006c0: 4e6f 6e65 602e 0a2d 2060 6a77 745f 6578  None`..- `jwt_ex
-000006d0: 7069 7265 7360 202d 2054 6865 2065 7870  pires` - The exp
-000006e0: 6972 6174 696f 6e20 7469 6d65 206f 6620  iration time of 
-000006f0: 7468 6520 4a57 5420 696e 2073 6563 6f6e  the JWT in secon
-00000700: 6473 2e20 4465 6661 756c 7473 2074 6f20  ds. Defaults to 
-00000710: 6039 3030 602e 0a2d 2060 6a77 745f 616c  `900`..- `jwt_al
-00000720: 676f 7269 7468 6d60 202d 2054 6865 2061  gorithm` - The a
-00000730: 6c67 6f72 6974 686d 2075 7365 6420 746f  lgorithm used to
-00000740: 2073 6967 6e20 7468 6520 4a57 542e 2044   sign the JWT. D
-00000750: 6566 6175 6c74 7320 746f 2060 4853 3235  efaults to `HS25
-00000760: 3660 2e0a 2d20 6063 6c69 656e 7473 6020  6`..- `clients` 
-00000770: 2d20 5468 6520 6c69 7374 206f 6620 7468  - The list of th
-00000780: 6520 4f41 7574 6832 2063 6c69 656e 7473  e OAuth2 clients
-00000790: 2e20 4465 6661 756c 7473 2074 6f20 605b  . Defaults to `[
-000007a0: 5d60 2e0a 0a23 2323 204f 4175 7468 3243  ]`...### OAuth2C
-000007b0: 6c69 656e 740a 0a2d 2060 6261 636b 656e  lient..- `backen
-000007c0: 6460 202d 2054 6865 205b 736f 6369 616c  d` - The [social
-000007d0: 2d63 6f72 655d 2868 7474 7073 3a2f 2f67  -core](https://g
-000007e0: 6974 6875 622e 636f 6d2f 7079 7468 6f6e  ithub.com/python
-000007f0: 2d73 6f63 6961 6c2d 6175 7468 2f73 6f63  -social-auth/soc
-00000800: 6961 6c2d 636f 7265 2920 6175 7468 656e  ial-core) authen
-00000810: 7469 6361 7469 6f6e 2062 6163 6b65 6e64  tication backend
-00000820: 2063 6c61 7373 6e61 6d65 2e0a 2d20 6063   classname..- `c
-00000830: 6c69 656e 745f 6964 6020 2d20 5468 6520  lient_id` - The 
-00000840: 4f41 7574 6832 2063 6c69 656e 7420 4944  OAuth2 client ID
-00000850: 2066 6f72 2074 6865 2070 6172 7469 6375   for the particu
-00000860: 6c61 7220 7072 6f76 6964 6572 2e0a 2d20  lar provider..- 
-00000870: 6063 6c69 656e 745f 7365 6372 6574 6020  `client_secret` 
-00000880: 2d20 5468 6520 4f41 7574 6832 2063 6c69  - The OAuth2 cli
-00000890: 656e 7420 7365 6372 6574 2066 6f72 2074  ent secret for t
-000008a0: 6865 2070 6172 7469 6375 6c61 7220 7072  he particular pr
-000008b0: 6f76 6964 6572 2e0a 2d20 6072 6564 6972  ovider..- `redir
-000008c0: 6563 745f 7572 6960 202d 2054 6865 204f  ect_uri` - The O
-000008d0: 4175 7468 3220 7265 6469 7265 6374 2055  Auth2 redirect U
-000008e0: 5249 2074 6f20 7265 6469 7265 6374 2074  RI to redirect t
-000008f0: 6f20 6166 7465 7220 7375 6363 6573 732e  o after success.
-00000900: 2044 6566 6175 6c74 7320 746f 2074 6865   Defaults to the
-00000910: 2062 6173 6520 5552 4c2e 0a2d 2060 7363   base URL..- `sc
-00000920: 6f70 6560 202d 2054 6865 204f 4175 7468  ope` - The OAuth
-00000930: 3220 7363 6f70 6520 666f 7220 7468 6520  2 scope for the 
-00000940: 7061 7274 6963 756c 6172 2070 726f 7669  particular provi
-00000950: 6465 722e 2044 6566 6175 6c74 7320 746f  der. Defaults to
-00000960: 2060 5b5d 602e 0a0a 4974 2069 7320 616c   `[]`...It is al
-00000970: 736f 2069 6d70 6f72 7461 6e74 2074 6f20  so important to 
-00000980: 6d65 6e74 696f 6e20 7468 6174 2066 6f72  mention that for
-00000990: 2074 6865 2063 6f6e 6669 6775 7265 6420   the configured 
-000009a0: 636c 6965 6e74 7320 6f66 2074 6865 2061  clients of the a
-000009b0: 7574 6820 7072 6f76 6964 6572 732c 2074  uth providers, t
-000009c0: 6865 2061 7574 686f 7269 7a61 7469 6f6e  he authorization
-000009d0: 2055 524c 7320 6172 650a 6163 6365 7373   URLs are.access
-000009e0: 6962 6c65 2062 7920 7468 6520 602f 6f61  ible by the `/oa
-000009f0: 7574 6832 2f7b 7072 6f76 6964 6572 7d2f  uth2/{provider}/
-00000a00: 6175 7468 6020 7061 7468 2077 6865 7265  auth` path where
-00000a10: 2074 6865 2060 7072 6f76 6964 6572 6020   the `provider` 
-00000a20: 7661 7269 6162 6c65 2072 6570 7265 7365  variable represe
-00000a30: 6e74 7320 7468 6520 6578 6163 7420 7661  nts the exact va
-00000a40: 6c75 6520 6f66 2074 6865 2061 7574 680a  lue of the auth.
-00000a50: 7072 6f76 6964 6572 2062 6163 6b65 6e64  provider backend
-00000a60: 2060 6e61 6d65 6020 6174 7472 6962 7574   `name` attribut
-00000a70: 652e 0a0a 6060 6070 7974 686f 6e0a 6672  e...```python.fr
-00000a80: 6f6d 2066 6173 7461 7069 5f6f 6175 7468  om fastapi_oauth
-00000a90: 322e 636c 6965 6e74 2069 6d70 6f72 7420  2.client import 
-00000aa0: 4f41 7574 6832 436c 6965 6e74 0a66 726f  OAuth2Client.fro
-00000ab0: 6d20 6661 7374 6170 695f 6f61 7574 6832  m fastapi_oauth2
-00000ac0: 2e63 6f6e 6669 6720 696d 706f 7274 204f  .config import O
-00000ad0: 4175 7468 3243 6f6e 6669 670a 6672 6f6d  Auth2Config.from
-00000ae0: 2073 6f63 6961 6c5f 636f 7265 2e62 6163   social_core.bac
-00000af0: 6b65 6e64 732e 6769 7468 7562 2069 6d70  kends.github imp
-00000b00: 6f72 7420 4769 7468 7562 4f41 7574 6832  ort GithubOAuth2
-00000b10: 0a0a 6f61 7574 6832 5f63 6f6e 6669 6720  ..oauth2_config 
-00000b20: 3d20 4f41 7574 6832 436f 6e66 6967 280a  = OAuth2Config(.
-00000b30: 2020 2020 616c 6c6f 775f 6874 7470 3d46      allow_http=F
-00000b40: 616c 7365 2c0a 2020 2020 6a77 745f 7365  alse,.    jwt_se
-00000b50: 6372 6574 3d6f 732e 6765 7465 6e76 2822  cret=os.getenv("
-00000b60: 4a57 545f 5345 4352 4554 2229 2c0a 2020  JWT_SECRET"),.  
-00000b70: 2020 6a77 745f 6578 7069 7265 733d 6f73    jwt_expires=os
-00000b80: 2e67 6574 656e 7628 224a 5754 5f45 5850  .getenv("JWT_EXP
-00000b90: 4952 4553 2229 2c0a 2020 2020 6a77 745f  IRES"),.    jwt_
-00000ba0: 616c 676f 7269 7468 6d3d 6f73 2e67 6574  algorithm=os.get
-00000bb0: 656e 7628 224a 5754 5f41 4c47 4f52 4954  env("JWT_ALGORIT
-00000bc0: 484d 2229 2c0a 2020 2020 636c 6965 6e74  HM"),.    client
-00000bd0: 733d 5b0a 2020 2020 2020 2020 4f41 7574  s=[.        OAut
-00000be0: 6832 436c 6965 6e74 280a 2020 2020 2020  h2Client(.      
-00000bf0: 2020 2020 2020 6261 636b 656e 643d 4769        backend=Gi
-00000c00: 7468 7562 4f41 7574 6832 2c0a 2020 2020  thubOAuth2,.    
-00000c10: 2020 2020 2020 2020 636c 6965 6e74 5f69          client_i
-00000c20: 643d 6f73 2e67 6574 656e 7628 224f 4155  d=os.getenv("OAU
-00000c30: 5448 325f 434c 4945 4e54 5f49 4422 292c  TH2_CLIENT_ID"),
-00000c40: 0a20 2020 2020 2020 2020 2020 2063 6c69  .            cli
-00000c50: 656e 745f 7365 6372 6574 3d6f 732e 6765  ent_secret=os.ge
-00000c60: 7465 6e76 2822 4f41 5554 4832 5f43 4c49  tenv("OAUTH2_CLI
-00000c70: 454e 545f 5345 4352 4554 2229 2c0a 2020  ENT_SECRET"),.  
-00000c80: 2020 2020 2020 2020 2020 7265 6469 7265            redire
-00000c90: 6374 5f75 7269 3d22 6874 7470 733a 2f2f  ct_uri="https://
-00000ca0: 7079 736e 6970 7065 742e 6f72 672f 222c  pysnippet.org/",
-00000cb0: 0a20 2020 2020 2020 2020 2020 2073 636f  .            sco
-00000cc0: 7065 3d5b 2275 7365 723a 656d 6169 6c22  pe=["user:email"
-00000cd0: 5d2c 0a20 2020 2020 2020 2029 2c0a 2020  ],.        ),.  
-00000ce0: 2020 5d0a 290a 6060 600a 0a23 2320 496e    ].).```..## In
-00000cf0: 7465 6772 6174 696f 6e0a 0a54 6f20 696e  tegration..To in
-00000d00: 7465 6772 6174 6520 7468 6520 7061 636b  tegrate the pack
-00000d10: 6167 6520 696e 746f 2079 6f75 7220 4661  age into your Fa
-00000d20: 7374 4150 4920 6170 706c 6963 6174 696f  stAPI applicatio
-00000d30: 6e2c 2079 6f75 206e 6565 6420 746f 2061  n, you need to a
-00000d40: 6464 2074 6865 2060 4f41 7574 6832 4d69  dd the `OAuth2Mi
-00000d50: 6464 6c65 7761 7265 6020 7769 7468 2070  ddleware` with p
-00000d60: 6172 7469 6375 6c61 7220 636f 6e66 6967  articular config
-00000d70: 730a 696e 2074 6865 2061 626f 7665 2d72  s.in the above-r
-00000d80: 6570 7265 7365 6e74 6564 2066 6f72 6d61  epresented forma
-00000d90: 7420 616e 6420 696e 636c 7564 6520 7468  t and include th
-00000da0: 6520 726f 7574 6572 2074 6f20 7468 6520  e router to the 
-00000db0: 6d61 696e 2072 6f75 7465 7220 6f66 2074  main router of t
-00000dc0: 6865 2061 7070 6c69 6361 7469 6f6e 2e0a  he application..
-00000dd0: 0a60 6060 7079 7468 6f6e 0a66 726f 6d20  .```python.from 
-00000de0: 6661 7374 6170 6920 696d 706f 7274 2046  fastapi import F
-00000df0: 6173 7441 5049 0a66 726f 6d20 6661 7374  astAPI.from fast
-00000e00: 6170 695f 6f61 7574 6832 2e6d 6964 646c  api_oauth2.middl
-00000e10: 6577 6172 6520 696d 706f 7274 204f 4175  eware import OAu
-00000e20: 7468 324d 6964 646c 6577 6172 650a 6672  th2Middleware.fr
-00000e30: 6f6d 2066 6173 7461 7069 5f6f 6175 7468  om fastapi_oauth
-00000e40: 322e 726f 7574 6572 2069 6d70 6f72 7420  2.router import 
-00000e50: 726f 7574 6572 2061 7320 6f61 7574 6832  router as oauth2
-00000e60: 5f72 6f75 7465 720a 0a61 7070 203d 2046  _router..app = F
-00000e70: 6173 7441 5049 2829 0a61 7070 2e69 6e63  astAPI().app.inc
-00000e80: 6c75 6465 5f72 6f75 7465 7228 6f61 7574  lude_router(oaut
-00000e90: 6832 5f72 6f75 7465 7229 0a61 7070 2e61  h2_router).app.a
-00000ea0: 6464 5f6d 6964 646c 6577 6172 6528 4f41  dd_middleware(OA
-00000eb0: 7574 6832 4d69 6464 6c65 7761 7265 2c20  uth2Middleware, 
-00000ec0: 636f 6e66 6967 3d6f 6175 7468 325f 636f  config=oauth2_co
-00000ed0: 6e66 6967 290a 6060 600a 0a41 6674 6572  nfig).```..After
-00000ee0: 2061 6464 696e 6720 7468 6520 6d69 6464   adding the midd
-00000ef0: 6c65 7761 7265 2c20 7468 6520 6075 7365  leware, the `use
-00000f00: 7260 2061 7474 7269 6275 7465 2077 696c  r` attribute wil
-00000f10: 6c20 6265 2061 7661 696c 6162 6c65 2069  l be available i
-00000f20: 6e20 7468 6520 7265 7175 6573 7420 636f  n the request co
-00000f30: 6e74 6578 742e 2049 7420 7769 6c6c 2063  ntext. It will c
-00000f40: 6f6e 7461 696e 2074 6865 2075 7365 720a  ontain the user.
-00000f50: 6461 7461 2070 726f 7669 6465 6420 6279  data provided by
-00000f60: 2074 6865 204f 4175 7468 3220 7072 6f76   the OAuth2 prov
-00000f70: 6964 6572 2e0a 0a60 6060 6a69 6e6a 6132  ider...```jinja2
-00000f80: 0a7b 2520 6966 2072 6571 7565 7374 2e75  .{% if request.u
-00000f90: 7365 722e 6973 5f61 7574 6865 6e74 6963  ser.is_authentic
-00000fa0: 6174 6564 2025 7d0a 2020 2020 3c61 2068  ated %}.    <a h
-00000fb0: 7265 663d 222f 6f61 7574 6832 2f6c 6f67  ref="/oauth2/log
-00000fc0: 6f75 7422 3e53 6967 6e20 6f75 743c 2f61  out">Sign out</a
-00000fd0: 3e0a 7b25 2065 6c73 6520 257d 0a20 2020  >.{% else %}.   
-00000fe0: 203c 6120 6872 6566 3d22 2f6f 6175 7468   <a href="/oauth
-00000ff0: 322f 6769 7468 7562 2f61 7574 6822 3e53  2/github/auth">S
-00001000: 6967 6e20 696e 3c2f 613e 0a7b 2520 656e  ign in</a>.{% en
-00001010: 6469 6620 257d 0a60 6060 0a0a 2323 2043  dif %}.```..## C
-00001020: 6f6e 7472 6962 7574 650a 0a41 6e79 2063  ontribute..Any c
-00001030: 6f6e 7472 6962 7574 696f 6e20 6973 2077  ontribution is w
-00001040: 656c 636f 6d65 2e20 4966 2079 6f75 2068  elcome. If you h
-00001050: 6176 6520 616e 7920 6964 6561 7320 6f72  ave any ideas or
-00001060: 2073 7567 6765 7374 696f 6e73 2c20 6665   suggestions, fe
-00001070: 656c 2066 7265 6520 746f 206f 7065 6e20  el free to open 
-00001080: 616e 2069 7373 7565 206f 7220 6120 7075  an issue or a pu
-00001090: 6c6c 2072 6571 7565 7374 2e20 416e 640a  ll request. And.
-000010a0: 646f 6e27 7420 666f 7267 6574 2074 6f20  don't forget to 
-000010b0: 6164 6420 7465 7374 7320 666f 7220 796f  add tests for yo
-000010c0: 7572 2063 6861 6e67 6573 2e0a 0a23 2320  ur changes...## 
-000010d0: 4c69 6365 6e73 650a 0a43 6f70 7972 6967  License..Copyrig
-000010e0: 6874 2028 4329 2032 3032 3320 4172 7479  ht (C) 2023 Arty
-000010f0: 6f6d 2056 616e 6379 616e 2e20 5b4d 4954  om Vancyan. [MIT
-00001100: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00001110: 2e63 6f6d 2f70 7973 6e69 7070 6574 2f66  .com/pysnippet/f
-00001120: 6173 7461 7069 2d6f 6175 7468 322f 626c  astapi-oauth2/bl
-00001130: 6f62 2f6d 6173 7465 722f 4c49 4345 4e53  ob/master/LICENS
-00001140: 4529 0a                                  E).
+00000450: 6f76 6964 6572 730a 2d20 4375 7374 6f6d  oviders.- Custom
+00000460: 697a 6162 6c65 204f 4175 7468 3220 726f  izable OAuth2 ro
+00000470: 7574 6573 0a0a 2323 2049 6e73 7461 6c6c  utes..## Install
+00000480: 6174 696f 6e0a 0a60 6060 7368 656c 6c0a  ation..```shell.
+00000490: 7079 7468 6f6e 202d 6d20 7069 7020 696e  python -m pip in
+000004a0: 7374 616c 6c20 6661 7374 6170 692d 6f61  stall fastapi-oa
+000004b0: 7574 6832 0a60 6060 0a0a 2323 2043 6f6e  uth2.```..## Con
+000004c0: 6669 6775 7261 7469 6f6e 0a0a 436f 6e66  figuration..Conf
+000004d0: 6967 7572 6174 696f 6e20 7265 7175 6972  iguration requir
+000004e0: 6573 2079 6f75 2074 6f20 7072 6f76 6964  es you to provid
+000004f0: 6520 7468 6520 4a57 5420 7265 7175 6973  e the JWT requis
+00000500: 6974 6573 2061 6e64 2064 6566 696e 6520  ites and define 
+00000510: 7468 6520 636c 6965 6e74 7320 6f66 2074  the clients of t
+00000520: 6865 2070 6172 7469 6375 6c61 7220 7072  he particular pr
+00000530: 6f76 6964 6572 732e 2054 6865 0a6d 6964  oviders. The.mid
+00000540: 646c 6577 6172 6520 636f 6e66 6967 7572  dleware configur
+00000550: 6174 696f 6e20 6973 2064 6563 6c61 7265  ation is declare
+00000560: 6420 7769 7468 2074 6865 2060 4f41 7574  d with the `OAut
+00000570: 6832 436f 6e66 6967 6020 616e 6420 604f  h2Config` and `O
+00000580: 4175 7468 3243 6c69 656e 7460 2063 6c61  Auth2Client` cla
+00000590: 7373 6573 2e0a 0a23 2323 204f 4175 7468  sses...### OAuth
+000005a0: 3243 6f6e 6669 670a 0a2d 2060 616c 6c6f  2Config..- `allo
+000005b0: 775f 6874 7470 6020 2d20 416c 6c6f 7720  w_http` - Allow 
+000005c0: 696e 7365 6375 7265 2048 5454 5020 7265  insecure HTTP re
+000005d0: 7175 6573 7473 2e20 4465 6661 756c 7473  quests. Defaults
+000005e0: 2074 6f20 6046 616c 7365 602e 0a2d 2060   to `False`..- `
+000005f0: 6a77 745f 7365 6372 6574 6020 2d20 5468  jwt_secret` - Th
+00000600: 6520 7365 6372 6574 206b 6579 2075 7365  e secret key use
+00000610: 6420 746f 2073 6967 6e20 7468 6520 4a57  d to sign the JW
+00000620: 542e 2044 6566 6175 6c74 7320 746f 2060  T. Defaults to `
+00000630: 4e6f 6e65 602e 0a2d 2060 6a77 745f 6578  None`..- `jwt_ex
+00000640: 7069 7265 7360 202d 2054 6865 2065 7870  pires` - The exp
+00000650: 6972 6174 696f 6e20 7469 6d65 206f 6620  iration time of 
+00000660: 7468 6520 4a57 5420 696e 2073 6563 6f6e  the JWT in secon
+00000670: 6473 2e20 4465 6661 756c 7473 2074 6f20  ds. Defaults to 
+00000680: 6039 3030 602e 0a2d 2060 6a77 745f 616c  `900`..- `jwt_al
+00000690: 676f 7269 7468 6d60 202d 2054 6865 2061  gorithm` - The a
+000006a0: 6c67 6f72 6974 686d 2075 7365 6420 746f  lgorithm used to
+000006b0: 2073 6967 6e20 7468 6520 4a57 542e 2044   sign the JWT. D
+000006c0: 6566 6175 6c74 7320 746f 2060 4853 3235  efaults to `HS25
+000006d0: 3660 2e0a 2d20 6063 6c69 656e 7473 6020  6`..- `clients` 
+000006e0: 2d20 5468 6520 6c69 7374 206f 6620 7468  - The list of th
+000006f0: 6520 4f41 7574 6832 2063 6c69 656e 7473  e OAuth2 clients
+00000700: 2e20 4465 6661 756c 7473 2074 6f20 605b  . Defaults to `[
+00000710: 5d60 2e0a 0a23 2323 204f 4175 7468 3243  ]`...### OAuth2C
+00000720: 6c69 656e 740a 0a2d 2060 6261 636b 656e  lient..- `backen
+00000730: 6460 202d 2054 6865 205b 736f 6369 616c  d` - The [social
+00000740: 2d63 6f72 655d 2868 7474 7073 3a2f 2f67  -core](https://g
+00000750: 6974 6875 622e 636f 6d2f 7079 7468 6f6e  ithub.com/python
+00000760: 2d73 6f63 6961 6c2d 6175 7468 2f73 6f63  -social-auth/soc
+00000770: 6961 6c2d 636f 7265 2920 6175 7468 656e  ial-core) authen
+00000780: 7469 6361 7469 6f6e 2062 6163 6b65 6e64  tication backend
+00000790: 2063 6c61 7373 6e61 6d65 2e0a 2d20 6063   classname..- `c
+000007a0: 6c69 656e 745f 6964 6020 2d20 5468 6520  lient_id` - The 
+000007b0: 4f41 7574 6832 2063 6c69 656e 7420 4944  OAuth2 client ID
+000007c0: 2066 6f72 2074 6865 2070 6172 7469 6375   for the particu
+000007d0: 6c61 7220 7072 6f76 6964 6572 2e0a 2d20  lar provider..- 
+000007e0: 6063 6c69 656e 745f 7365 6372 6574 6020  `client_secret` 
+000007f0: 2d20 5468 6520 4f41 7574 6832 2063 6c69  - The OAuth2 cli
+00000800: 656e 7420 7365 6372 6574 2066 6f72 2074  ent secret for t
+00000810: 6865 2070 6172 7469 6375 6c61 7220 7072  he particular pr
+00000820: 6f76 6964 6572 2e0a 2d20 6072 6564 6972  ovider..- `redir
+00000830: 6563 745f 7572 6960 202d 2054 6865 204f  ect_uri` - The O
+00000840: 4175 7468 3220 7265 6469 7265 6374 2055  Auth2 redirect U
+00000850: 5249 2074 6f20 7265 6469 7265 6374 2074  RI to redirect t
+00000860: 6f20 6166 7465 7220 7375 6363 6573 732e  o after success.
+00000870: 2044 6566 6175 6c74 7320 746f 2074 6865   Defaults to the
+00000880: 2062 6173 6520 5552 4c2e 0a2d 2060 7363   base URL..- `sc
+00000890: 6f70 6560 202d 2054 6865 204f 4175 7468  ope` - The OAuth
+000008a0: 3220 7363 6f70 6520 666f 7220 7468 6520  2 scope for the 
+000008b0: 7061 7274 6963 756c 6172 2070 726f 7669  particular provi
+000008c0: 6465 722e 2044 6566 6175 6c74 7320 746f  der. Defaults to
+000008d0: 2060 5b5d 602e 0a2d 2060 636c 6169 6d73   `[]`..- `claims
+000008e0: 6020 2d20 436c 6169 6d73 206d 6170 7069  ` - Claims mappi
+000008f0: 6e67 2066 6f72 2074 6865 2063 6572 7461  ng for the certa
+00000900: 696e 2070 726f 7669 6465 722e 0a0a 4974  in provider...It
+00000910: 2069 7320 616c 736f 2069 6d70 6f72 7461   is also importa
+00000920: 6e74 2074 6f20 6d65 6e74 696f 6e20 7468  nt to mention th
+00000930: 6174 2066 6f72 2074 6865 2063 6f6e 6669  at for the confi
+00000940: 6775 7265 6420 636c 6965 6e74 7320 6f66  gured clients of
+00000950: 2074 6865 2061 7574 6820 7072 6f76 6964   the auth provid
+00000960: 6572 732c 2074 6865 2061 7574 686f 7269  ers, the authori
+00000970: 7a61 7469 6f6e 2055 524c 7320 6172 650a  zation URLs are.
+00000980: 6163 6365 7373 6962 6c65 2062 7920 7468  accessible by th
+00000990: 6520 602f 6f61 7574 6832 2f7b 7072 6f76  e `/oauth2/{prov
+000009a0: 6964 6572 7d2f 6175 7468 6020 7061 7468  ider}/auth` path
+000009b0: 2077 6865 7265 2074 6865 2060 7072 6f76   where the `prov
+000009c0: 6964 6572 6020 7661 7269 6162 6c65 2072  ider` variable r
+000009d0: 6570 7265 7365 6e74 7320 7468 6520 6578  epresents the ex
+000009e0: 6163 7420 7661 6c75 6520 6f66 2074 6865  act value of the
+000009f0: 2061 7574 680a 7072 6f76 6964 6572 2062   auth.provider b
+00000a00: 6163 6b65 6e64 2060 6e61 6d65 6020 6174  ackend `name` at
+00000a10: 7472 6962 7574 652e 0a0a 6060 6070 7974  tribute...```pyt
+00000a20: 686f 6e0a 6672 6f6d 2066 6173 7461 7069  hon.from fastapi
+00000a30: 5f6f 6175 7468 322e 636c 6169 6d73 2069  _oauth2.claims i
+00000a40: 6d70 6f72 7420 436c 6169 6d73 0a66 726f  mport Claims.fro
+00000a50: 6d20 6661 7374 6170 695f 6f61 7574 6832  m fastapi_oauth2
+00000a60: 2e63 6c69 656e 7420 696d 706f 7274 204f  .client import O
+00000a70: 4175 7468 3243 6c69 656e 740a 6672 6f6d  Auth2Client.from
+00000a80: 2066 6173 7461 7069 5f6f 6175 7468 322e   fastapi_oauth2.
+00000a90: 636f 6e66 6967 2069 6d70 6f72 7420 4f41  config import OA
+00000aa0: 7574 6832 436f 6e66 6967 0a66 726f 6d20  uth2Config.from 
+00000ab0: 736f 6369 616c 5f63 6f72 652e 6261 636b  social_core.back
+00000ac0: 656e 6473 2e67 6974 6875 6220 696d 706f  ends.github impo
+00000ad0: 7274 2047 6974 6875 624f 4175 7468 320a  rt GithubOAuth2.
+00000ae0: 0a6f 6175 7468 325f 636f 6e66 6967 203d  .oauth2_config =
+00000af0: 204f 4175 7468 3243 6f6e 6669 6728 0a20   OAuth2Config(. 
+00000b00: 2020 2061 6c6c 6f77 5f68 7474 703d 4661     allow_http=Fa
+00000b10: 6c73 652c 0a20 2020 206a 7774 5f73 6563  lse,.    jwt_sec
+00000b20: 7265 743d 6f73 2e67 6574 656e 7628 224a  ret=os.getenv("J
+00000b30: 5754 5f53 4543 5245 5422 292c 0a20 2020  WT_SECRET"),.   
+00000b40: 206a 7774 5f65 7870 6972 6573 3d6f 732e   jwt_expires=os.
+00000b50: 6765 7465 6e76 2822 4a57 545f 4558 5049  getenv("JWT_EXPI
+00000b60: 5245 5322 292c 0a20 2020 206a 7774 5f61  RES"),.    jwt_a
+00000b70: 6c67 6f72 6974 686d 3d6f 732e 6765 7465  lgorithm=os.gete
+00000b80: 6e76 2822 4a57 545f 414c 474f 5249 5448  nv("JWT_ALGORITH
+00000b90: 4d22 292c 0a20 2020 2063 6c69 656e 7473  M"),.    clients
+00000ba0: 3d5b 0a20 2020 2020 2020 204f 4175 7468  =[.        OAuth
+00000bb0: 3243 6c69 656e 7428 0a20 2020 2020 2020  2Client(.       
+00000bc0: 2020 2020 2062 6163 6b65 6e64 3d47 6974       backend=Git
+00000bd0: 6875 624f 4175 7468 322c 0a20 2020 2020  hubOAuth2,.     
+00000be0: 2020 2020 2020 2063 6c69 656e 745f 6964         client_id
+00000bf0: 3d6f 732e 6765 7465 6e76 2822 4f41 5554  =os.getenv("OAUT
+00000c00: 4832 5f43 4c49 454e 545f 4944 2229 2c0a  H2_CLIENT_ID"),.
+00000c10: 2020 2020 2020 2020 2020 2020 636c 6965              clie
+00000c20: 6e74 5f73 6563 7265 743d 6f73 2e67 6574  nt_secret=os.get
+00000c30: 656e 7628 224f 4155 5448 325f 434c 4945  env("OAUTH2_CLIE
+00000c40: 4e54 5f53 4543 5245 5422 292c 0a20 2020  NT_SECRET"),.   
+00000c50: 2020 2020 2020 2020 2072 6564 6972 6563           redirec
+00000c60: 745f 7572 693d 2268 7474 7073 3a2f 2f70  t_uri="https://p
+00000c70: 7973 6e69 7070 6574 2e6f 7267 2f22 2c0a  ysnippet.org/",.
+00000c80: 2020 2020 2020 2020 2020 2020 7363 6f70              scop
+00000c90: 653d 5b22 7573 6572 3a65 6d61 696c 225d  e=["user:email"]
+00000ca0: 2c0a 2020 2020 2020 2020 2020 2020 636c  ,.            cl
+00000cb0: 6169 6d73 3d43 6c61 696d 7328 0a20 2020  aims=Claims(.   
+00000cc0: 2020 2020 2020 2020 2020 2020 2070 6963               pic
+00000cd0: 7475 7265 3d22 6176 6174 6172 5f75 726c  ture="avatar_url
+00000ce0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00000cf0: 2020 2069 6465 6e74 6974 793d 6c61 6d62     identity=lamb
+00000d00: 6461 2075 7365 723a 2022 2573 3a25 7322  da user: "%s:%s"
+00000d10: 2025 2028 7573 6572 2e67 6574 2822 7072   % (user.get("pr
+00000d20: 6f76 6964 6572 2229 2c20 7573 6572 2e67  ovider"), user.g
+00000d30: 6574 2822 6964 2229 292c 0a20 2020 2020  et("id")),.     
+00000d40: 2020 2020 2020 2029 2c0a 2020 2020 2020         ),.      
+00000d50: 2020 292c 0a20 2020 205d 0a29 0a60 6060    ),.    ].).```
+00000d60: 0a0a 2323 2049 6e74 6567 7261 7469 6f6e  ..## Integration
+00000d70: 0a0a 546f 2069 6e74 6567 7261 7465 2074  ..To integrate t
+00000d80: 6865 2070 6163 6b61 6765 2069 6e74 6f20  he package into 
+00000d90: 796f 7572 2046 6173 7441 5049 2061 7070  your FastAPI app
+00000da0: 6c69 6361 7469 6f6e 2c20 796f 7520 6e65  lication, you ne
+00000db0: 6564 2074 6f20 6164 6420 7468 6520 604f  ed to add the `O
+00000dc0: 4175 7468 324d 6964 646c 6577 6172 6560  Auth2Middleware`
+00000dd0: 2077 6974 6820 7061 7274 6963 756c 6172   with particular
+00000de0: 2063 6f6e 6669 6773 0a69 6e20 7468 6520   configs.in the 
+00000df0: 6162 6f76 652d 7265 7072 6573 656e 7465  above-represente
+00000e00: 6420 666f 726d 6174 2061 6e64 2069 6e63  d format and inc
+00000e10: 6c75 6465 2074 6865 2072 6f75 7465 7220  lude the router 
+00000e20: 746f 2074 6865 206d 6169 6e20 726f 7574  to the main rout
+00000e30: 6572 206f 6620 7468 6520 6170 706c 6963  er of the applic
+00000e40: 6174 696f 6e2e 0a0a 6060 6070 7974 686f  ation...```pytho
+00000e50: 6e0a 6672 6f6d 2066 6173 7461 7069 2069  n.from fastapi i
+00000e60: 6d70 6f72 7420 4661 7374 4150 490a 6672  mport FastAPI.fr
+00000e70: 6f6d 2066 6173 7461 7069 5f6f 6175 7468  om fastapi_oauth
+00000e80: 322e 6d69 6464 6c65 7761 7265 2069 6d70  2.middleware imp
+00000e90: 6f72 7420 4f41 7574 6832 4d69 6464 6c65  ort OAuth2Middle
+00000ea0: 7761 7265 0a66 726f 6d20 6661 7374 6170  ware.from fastap
+00000eb0: 695f 6f61 7574 6832 2e72 6f75 7465 7220  i_oauth2.router 
+00000ec0: 696d 706f 7274 2072 6f75 7465 7220 6173  import router as
+00000ed0: 206f 6175 7468 325f 726f 7574 6572 0a0a   oauth2_router..
+00000ee0: 6170 7020 3d20 4661 7374 4150 4928 290a  app = FastAPI().
+00000ef0: 6170 702e 696e 636c 7564 655f 726f 7574  app.include_rout
+00000f00: 6572 286f 6175 7468 325f 726f 7574 6572  er(oauth2_router
+00000f10: 290a 6170 702e 6164 645f 6d69 6464 6c65  ).app.add_middle
+00000f20: 7761 7265 284f 4175 7468 324d 6964 646c  ware(OAuth2Middl
+00000f30: 6577 6172 652c 2063 6f6e 6669 673d 6f61  eware, config=oa
+00000f40: 7574 6832 5f63 6f6e 6669 6729 0a60 6060  uth2_config).```
+00000f50: 0a0a 4166 7465 7220 6164 6469 6e67 2074  ..After adding t
+00000f60: 6865 206d 6964 646c 6577 6172 652c 2074  he middleware, t
+00000f70: 6865 2060 7573 6572 6020 6174 7472 6962  he `user` attrib
+00000f80: 7574 6520 7769 6c6c 2062 6520 6176 6169  ute will be avai
+00000f90: 6c61 626c 6520 696e 2074 6865 2072 6571  lable in the req
+00000fa0: 7565 7374 2063 6f6e 7465 7874 2e20 4974  uest context. It
+00000fb0: 2077 696c 6c20 636f 6e74 6169 6e20 7468   will contain th
+00000fc0: 6520 7573 6572 0a64 6174 6120 7072 6f76  e user.data prov
+00000fd0: 6964 6564 2062 7920 7468 6520 4f41 7574  ided by the OAut
+00000fe0: 6832 2070 726f 7669 6465 722e 0a0a 6060  h2 provider...``
+00000ff0: 606a 696e 6a61 320a 7b25 2069 6620 7265  `jinja2.{% if re
+00001000: 7175 6573 742e 7573 6572 2e69 735f 6175  quest.user.is_au
+00001010: 7468 656e 7469 6361 7465 6420 257d 0a20  thenticated %}. 
+00001020: 2020 203c 6120 6872 6566 3d22 2f6f 6175     <a href="/oau
+00001030: 7468 322f 6c6f 676f 7574 223e 5369 676e  th2/logout">Sign
+00001040: 206f 7574 3c2f 613e 0a7b 2520 656c 7365   out</a>.{% else
+00001050: 2025 7d0a 2020 2020 3c61 2068 7265 663d   %}.    <a href=
+00001060: 222f 6f61 7574 6832 2f67 6974 6875 622f  "/oauth2/github/
+00001070: 6175 7468 223e 5369 676e 2069 6e3c 2f61  auth">Sign in</a
+00001080: 3e0a 7b25 2065 6e64 6966 2025 7d0a 6060  >.{% endif %}.``
+00001090: 600a 0a23 2320 436f 6e74 7269 6275 7465  `..## Contribute
+000010a0: 0a0a 416e 7920 636f 6e74 7269 6275 7469  ..Any contributi
+000010b0: 6f6e 2069 7320 7765 6c63 6f6d 652e 2049  on is welcome. I
+000010c0: 6620 796f 7520 6861 7665 2061 6e79 2069  f you have any i
+000010d0: 6465 6173 206f 7220 7375 6767 6573 7469  deas or suggesti
+000010e0: 6f6e 732c 2066 6565 6c20 6672 6565 2074  ons, feel free t
+000010f0: 6f20 6f70 656e 2061 6e20 6973 7375 6520  o open an issue 
+00001100: 6f72 2061 2070 756c 6c20 7265 7175 6573  or a pull reques
+00001110: 742e 2041 6e64 0a64 6f6e 2774 2066 6f72  t. And.don't for
+00001120: 6765 7420 746f 2061 6464 2074 6573 7473  get to add tests
+00001130: 2066 6f72 2079 6f75 7220 6368 616e 6765   for your change
+00001140: 732e 0a0a 2323 204c 6963 656e 7365 0a0a  s...## License..
+00001150: 436f 7079 7269 6768 7420 2843 2920 3230  Copyright (C) 20
+00001160: 3233 2041 7274 796f 6d20 5661 6e63 7961  23 Artyom Vancya
+00001170: 6e2e 205b 4d49 545d 2868 7474 7073 3a2f  n. [MIT](https:/
+00001180: 2f67 6974 6875 622e 636f 6d2f 7079 736e  /github.com/pysn
+00001190: 6970 7065 742f 6661 7374 6170 692d 6f61  ippet/fastapi-oa
+000011a0: 7574 6832 2f62 6c6f 622f 6d61 7374 6572  uth2/blob/master
+000011b0: 2f4c 4943 454e 5345 290a                 /LICENSE).
```

### Comparing `fastapi-oauth2-1.0.0a0/setup.cfg` & `fastapi-oauth2-1.0.0a1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -27,33 +27,33 @@
 platforms = unix, linux, osx, win32
 classifiers = 
 	Operating System :: OS Independent
 	Development Status :: 2 - Pre-Alpha
 	Framework :: FastAPI
 	Programming Language :: Python
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	License :: OSI Approved :: MIT License
 
 [options]
 packages = 
 	fastapi_oauth2
 install_requires = 
 	fastapi>=0.68.1
-	httpx>=0.22.0
+	httpx>=0.23.0
 	oauthlib>=3.2.2
 	python-jose>=3.3.0
 	social-auth-core>=4.4.2
 	starlette>=0.19.1
 include_package_data = yes
-python_requires = >=3.6
+python_requires = >=3.7
 package_dir = 
 	=src
 zip_safe = no
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `fastapi-oauth2-1.0.0a0/src/fastapi_oauth2/client.py` & `fastapi-oauth2-1.0.0a1/src/fastapi_oauth2/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,36 @@
 from typing import Optional
 from typing import Sequence
 from typing import Type
+from typing import Union
 
 from social_core.backends.oauth import BaseOAuth2
 
+from .claims import Claims
+
 
 class OAuth2Client:
+    """OAuth2 client configuration for a single provider."""
+
     backend: Type[BaseOAuth2]
     client_id: str
     client_secret: str
     redirect_uri: Optional[str]
     scope: Optional[Sequence[str]]
+    claims: Optional[Union[Claims, dict]]
 
     def __init__(
             self,
             *,
             backend: Type[BaseOAuth2],
             client_id: str,
             client_secret: str,
             redirect_uri: Optional[str] = None,
             scope: Optional[Sequence[str]] = None,
-    ):
+            claims: Optional[Union[Claims, dict]] = None,
+    ) -> None:
         self.backend = backend
         self.client_id = client_id
         self.client_secret = client_secret
         self.redirect_uri = redirect_uri
         self.scope = scope or []
+        self.claims = Claims(claims)
```

### Comparing `fastapi-oauth2-1.0.0a0/src/fastapi_oauth2/config.py` & `fastapi-oauth2-1.0.0a1/src/fastapi_oauth2/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,29 +2,31 @@
 from typing import List
 from typing import Union
 
 from .client import OAuth2Client
 
 
 class OAuth2Config:
+    """Configuration class of the authentication middleware."""
+
     allow_http: bool
     jwt_secret: str
     jwt_expires: int
     jwt_algorithm: str
     clients: List[OAuth2Client]
 
     def __init__(
             self,
             *,
             allow_http: bool = False,
             jwt_secret: str = "",
             jwt_expires: Union[int, str] = 900,
             jwt_algorithm: str = "HS256",
             clients: List[OAuth2Client] = None,
-    ):
+    ) -> None:
         if allow_http:
             os.environ["OAUTHLIB_INSECURE_TRANSPORT"] = "1"
         self.allow_http = allow_http
         self.jwt_secret = jwt_secret
         self.jwt_expires = int(jwt_expires)
         self.jwt_algorithm = jwt_algorithm
         self.clients = clients or []
```

### Comparing `fastapi-oauth2-1.0.0a0/src/fastapi_oauth2/core.py` & `fastapi-oauth2-1.0.0a1/src/fastapi_oauth2/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,80 +12,81 @@
 from oauthlib.oauth2 import WebApplicationClient
 from social_core.backends.oauth import BaseOAuth2
 from social_core.strategy import BaseStrategy
 from starlette.exceptions import HTTPException
 from starlette.requests import Request
 from starlette.responses import RedirectResponse
 
+from .claims import Claims
 from .client import OAuth2Client
 
 
 class OAuth2LoginError(HTTPException):
-    """Raised when any login-related error occurs
-    (such as when user is not verified or if there was an attempt for fake login)
-    """
+    """Raised when any login-related error occurs."""
 
 
 class OAuth2Strategy(BaseStrategy):
-    def request_data(self, merge=True):
+    """Dummy strategy for using the `BaseOAuth2.user_data` method."""
+
+    def request_data(self, merge=True) -> Dict[str, Any]:
         return {}
 
-    def absolute_uri(self, path=None):
+    def absolute_uri(self, path=None) -> str:
         return path
 
-    def get_setting(self, name):
-        return None
+    def get_setting(self, name) -> Any:
+        """Mocked setting method."""
 
     @staticmethod
-    def get_json(url, method='GET', *args, **kwargs):
+    def get_json(url, method='GET', *args, **kwargs) -> httpx.Response:
         return httpx.request(method, url, *args, **kwargs)
 
 
 class OAuth2Core:
-    """Base class (mixin) for all SSO providers"""
+    """OAuth2 flow handler of a certain provider."""
 
     client_id: str = None
     client_secret: str = None
     callback_url: Optional[str] = None
     scope: Optional[List[str]] = None
+    claims: Optional[Claims] = None
     backend: BaseOAuth2 = None
     _oauth_client: Optional[WebApplicationClient] = None
 
     authorization_endpoint: str = None
     token_endpoint: str = None
 
     def __init__(self, client: OAuth2Client) -> None:
         self.client_id = client.client_id
         self.client_secret = client.client_secret
-        self.scope = client.scope or self.scope
+        self.scope = client.scope
+        self.claims = client.claims
         self.provider = client.backend.name
+        self.redirect_uri = client.redirect_uri
         self.backend = client.backend(OAuth2Strategy())
         self.authorization_endpoint = client.backend.AUTHORIZATION_URL
         self.token_endpoint = client.backend.ACCESS_TOKEN_URL
 
     @property
     def oauth_client(self) -> WebApplicationClient:
         if self._oauth_client is None:
             self._oauth_client = WebApplicationClient(self.client_id)
         return self._oauth_client
 
     def get_redirect_uri(self, request: Request) -> str:
         return urljoin(str(request.base_url), "/oauth2/%s/token" % self.provider)
 
-    async def get_login_url(self, request: Request) -> Any:
+    async def login_redirect(self, request: Request) -> RedirectResponse:
         redirect_uri = self.get_redirect_uri(request)
         state = "".join([random.choice(string.ascii_letters) for _ in range(32)])
-        return self.oauth_client.prepare_request_uri(
+        return RedirectResponse(str(self.oauth_client.prepare_request_uri(
             self.authorization_endpoint, redirect_uri=redirect_uri, state=state, scope=self.scope
-        )
-
-    async def login_redirect(self, request: Request) -> RedirectResponse:
-        return RedirectResponse(await self.get_login_url(request), 303)
+        )), 303)
 
-    async def get_token_data(self, request: Request) -> Optional[Dict[str, Any]]:
+    async def token_redirect(self, request: Request) -> RedirectResponse:
         if not request.query_params.get("code"):
             raise OAuth2LoginError(400, "'code' parameter was not found in callback request")
         if not request.query_params.get("state"):
             raise OAuth2LoginError(400, "'state' parameter was not found in callback request")
 
         url = request.url
         scheme = "http" if request.auth.http else "https"
@@ -104,23 +105,24 @@
             "Accept": "application/json",
             "Content-Type": "application/x-www-form-urlencoded",
         })
         auth = httpx.BasicAuth(self.client_id, self.client_secret)
         async with httpx.AsyncClient() as session:
             response = await session.post(token_url, headers=headers, content=content, auth=auth)
             token = self.oauth_client.parse_request_body_response(json.dumps(response.json()))
-            data = self.backend.user_data(token.get("access_token"))
-
-        return {**data, "scope": self.scope}
+            token_data = self.standardize(self.backend.user_data(token.get("access_token")))
+            access_token = request.auth.jwt_create(token_data)
 
-    async def token_redirect(self, request: Request) -> RedirectResponse:
-        token_data = await self.get_token_data(request)
-        access_token = request.auth.jwt_create(token_data)
-        response = RedirectResponse(request.base_url)
+        response = RedirectResponse(self.redirect_uri or request.base_url)
         response.set_cookie(
             "Authorization",
             value=f"Bearer {access_token}",
             max_age=request.auth.expires,
             expires=request.auth.expires,
             httponly=request.auth.http,
         )
         return response
+
+    def standardize(self, data: Dict[str, Any]) -> Dict[str, Any]:
+        data["provider"] = self.provider
+        data["scope"] = self.scope
+        return data
```

### Comparing `fastapi-oauth2-1.0.0a0/src/fastapi_oauth2/router.py` & `fastapi-oauth2-1.0.0a1/src/fastapi_oauth2/router.py`

 * *Files identical despite different names*

### Comparing `fastapi-oauth2-1.0.0a0/src/fastapi_oauth2.egg-info/PKG-INFO` & `fastapi-oauth2-1.0.0a1/src/fastapi_oauth2.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-oauth2
-Version: 1.0.0a0
+Version: 1.0.0a1
 Summary: Easy to setup OAuth2 authentication with support for several auth providers.
 Author: Artyom Vancyan
 Author-email: artyom@pysnippet.org
 License: MIT
 Project-URL: Documentation, https://github.com/pysnippet/fastapi-oauth2/
 Project-URL: Source Code, https://github.com/pysnippet/fastapi-oauth2/
 Keywords: python,sso,auth,login,oauth,oauth2,social,fastapi,allauth,security,middleware,authentication
@@ -13,21 +13,21 @@
 Platform: osx
 Platform: win32
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: FastAPI
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # fastapi-oauth2 <img src="https://github.com/pysnippet.png" align="right" height="64" />
 
 [![PyPI](https://img.shields.io/pypi/v/fastapi-oauth2.svg)](https://pypi.org/project/fastapi-oauth2/)
 [![Python](https://img.shields.io/pypi/pyversions/fastapi-oauth2.svg?logoColor=white)](https://pypi.org/project/fastapi-oauth2/)
@@ -38,18 +38,15 @@
 FastAPI OAuth2 is a middleware-based social authentication mechanism supporting several auth providers. It depends on
 the [social-core](https://github.com/python-social-auth/social-core) authentication backends.
 
 ## Features to be implemented
 
 - Use multiple OAuth2 providers at the same time
     * There need to be provided a way to configure the OAuth2 for multiple providers
-- Provide `fastapi.security.*` implementations that use cookies
-- Token -> user data, user data -> token easy conversion
 - Customizable OAuth2 routes
-- Registration support
 
 ## Installation
 
 ```shell
 python -m pip install fastapi-oauth2
 ```
 
@@ -69,20 +66,22 @@
 ### OAuth2Client
 
 - `backend` - The [social-core](https://github.com/python-social-auth/social-core) authentication backend classname.
 - `client_id` - The OAuth2 client ID for the particular provider.
 - `client_secret` - The OAuth2 client secret for the particular provider.
 - `redirect_uri` - The OAuth2 redirect URI to redirect to after success. Defaults to the base URL.
 - `scope` - The OAuth2 scope for the particular provider. Defaults to `[]`.
+- `claims` - Claims mapping for the certain provider.
 
 It is also important to mention that for the configured clients of the auth providers, the authorization URLs are
 accessible by the `/oauth2/{provider}/auth` path where the `provider` variable represents the exact value of the auth
 provider backend `name` attribute.
 
 ```python
+from fastapi_oauth2.claims import Claims
 from fastapi_oauth2.client import OAuth2Client
 from fastapi_oauth2.config import OAuth2Config
 from social_core.backends.github import GithubOAuth2
 
 oauth2_config = OAuth2Config(
     allow_http=False,
     jwt_secret=os.getenv("JWT_SECRET"),
@@ -91,14 +90,18 @@
     clients=[
         OAuth2Client(
             backend=GithubOAuth2,
             client_id=os.getenv("OAUTH2_CLIENT_ID"),
             client_secret=os.getenv("OAUTH2_CLIENT_SECRET"),
             redirect_uri="https://pysnippet.org/",
             scope=["user:email"],
+            claims=Claims(
+                picture="avatar_url",
+                identity=lambda user: "%s:%s" % (user.get("provider"), user.get("id")),
+            ),
         ),
     ]
 )
 ```
 
 ## Integration
```

