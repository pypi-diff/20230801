# Comparing `tmp/pydata-google-auth-1.8.1.tar.gz` & `tmp/pydata-google-auth-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydata-google-auth-1.8.1.tar", last modified: Mon Jul 10 15:11:24 2023, max compression
+gzip compressed data, was "pydata-google-auth-1.8.2.tar", last modified: Tue Aug  1 17:02:17 2023, max compression
```

## Comparing `pydata-google-auth-1.8.1.tar` & `pydata-google-auth-1.8.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 swast    (212416) primarygroup (89939)        0 2023-07-10 15:11:24.264217 pydata-google-auth-1.8.1/
--rw-r--r--   0 swast    (212416) primarygroup (89939)     2283 2021-12-02 22:18:28.000000 pydata-google-auth-1.8.1/AUTHORS.md
--rw-r--r--   0 swast    (212416) primarygroup (89939)     1582 2021-12-02 22:18:28.000000 pydata-google-auth-1.8.1/LICENSE.txt
--rw-r--r--   0 swast    (212416) primarygroup (89939)      331 2021-12-02 22:18:28.000000 pydata-google-auth-1.8.1/MANIFEST.in
--rw-r--r--   0 swast    (212416) primarygroup (89939)     2906 2023-07-10 15:11:24.264391 pydata-google-auth-1.8.1/PKG-INFO
--rw-r--r--   0 swast    (212416) primarygroup (89939)     1795 2021-12-02 22:18:28.000000 pydata-google-auth-1.8.1/README.rst
-drwxr-xr-x   0 swast    (212416) primarygroup (89939)        0 2023-07-10 15:11:24.265661 pydata-google-auth-1.8.1/pydata_google_auth/
--rw-r--r--   0 swast    (212416) primarygroup (89939)      662 2021-12-02 22:18:28.000000 pydata-google-auth-1.8.1/pydata_google_auth/__init__.py
--rw-r--r--   0 swast    (212416) primarygroup (89939)     3706 2022-03-10 20:53:17.000000 pydata-google-auth-1.8.1/pydata_google_auth/__main__.py
--rw-r--r--   0 swast    (212416) primarygroup (89939)      497 2023-07-10 15:11:24.265795 pydata-google-auth-1.8.1/pydata_google_auth/_version.py
--rw-r--r--   0 swast    (212416) primarygroup (89939)     2319 2021-12-02 22:18:28.000000 pydata-google-auth-1.8.1/pydata_google_auth/_webserver.py
--rw-r--r--   0 swast    (212416) primarygroup (89939)    20022 2023-07-10 15:01:28.000000 pydata-google-auth-1.8.1/pydata_google_auth/auth.py
--rw-r--r--   0 swast    (212416) primarygroup (89939)     8789 2021-12-02 22:18:28.000000 pydata-google-auth-1.8.1/pydata_google_auth/cache.py
--rw-r--r--   0 swast    (212416) primarygroup (89939)      262 2021-12-02 22:18:28.000000 pydata-google-auth-1.8.1/pydata_google_auth/exceptions.py
-drwxr-xr-x   0 swast    (212416) primarygroup (89939)        0 2023-07-10 15:11:24.263839 pydata-google-auth-1.8.1/pydata_google_auth.egg-info/
--rw-r--r--   0 swast    (212416) primarygroup (89939)     2906 2023-07-10 15:11:24.000000 pydata-google-auth-1.8.1/pydata_google_auth.egg-info/PKG-INFO
--rw-r--r--   0 swast    (212416) primarygroup (89939)      501 2023-07-10 15:11:24.000000 pydata-google-auth-1.8.1/pydata_google_auth.egg-info/SOURCES.txt
--rw-r--r--   0 swast    (212416) primarygroup (89939)        1 2023-07-10 15:11:24.000000 pydata-google-auth-1.8.1/pydata_google_auth.egg-info/dependency_links.txt
--rw-r--r--   0 swast    (212416) primarygroup (89939)      188 2023-07-10 15:11:24.000000 pydata-google-auth-1.8.1/pydata_google_auth.egg-info/requires.txt
--rw-r--r--   0 swast    (212416) primarygroup (89939)       19 2023-07-10 15:11:24.000000 pydata-google-auth-1.8.1/pydata_google_auth.egg-info/top_level.txt
--rw-r--r--   0 swast    (212416) primarygroup (89939)      356 2023-07-10 15:11:24.265066 pydata-google-auth-1.8.1/setup.cfg
--rw-r--r--   0 swast    (212416) primarygroup (89939)     1859 2021-12-03 19:00:07.000000 pydata-google-auth-1.8.1/setup.py
--rw-r--r--   0 swast    (212416) primarygroup (89939)    68752 2021-12-02 22:18:28.000000 pydata-google-auth-1.8.1/versioneer.py
+drwxr-xr-x   0 swast    (212416) primarygroup (89939)        0 2023-08-01 17:02:17.692107 pydata-google-auth-1.8.2/
+-rw-r--r--   0 swast    (212416) primarygroup (89939)     2283 2021-12-02 22:18:28.000000 pydata-google-auth-1.8.2/AUTHORS.md
+-rw-r--r--   0 swast    (212416) primarygroup (89939)     1582 2021-12-02 22:18:28.000000 pydata-google-auth-1.8.2/LICENSE.txt
+-rw-r--r--   0 swast    (212416) primarygroup (89939)      331 2021-12-02 22:18:28.000000 pydata-google-auth-1.8.2/MANIFEST.in
+-rw-r--r--   0 swast    (212416) primarygroup (89939)     2906 2023-08-01 17:02:17.692313 pydata-google-auth-1.8.2/PKG-INFO
+-rw-r--r--   0 swast    (212416) primarygroup (89939)     1795 2021-12-02 22:18:28.000000 pydata-google-auth-1.8.2/README.rst
+drwxr-xr-x   0 swast    (212416) primarygroup (89939)        0 2023-08-01 17:02:17.694082 pydata-google-auth-1.8.2/pydata_google_auth/
+-rw-r--r--   0 swast    (212416) primarygroup (89939)      662 2021-12-02 22:18:28.000000 pydata-google-auth-1.8.2/pydata_google_auth/__init__.py
+-rw-r--r--   0 swast    (212416) primarygroup (89939)     3706 2022-03-10 20:53:17.000000 pydata-google-auth-1.8.2/pydata_google_auth/__main__.py
+-rw-r--r--   0 swast    (212416) primarygroup (89939)      497 2023-08-01 17:02:17.694250 pydata-google-auth-1.8.2/pydata_google_auth/_version.py
+-rw-r--r--   0 swast    (212416) primarygroup (89939)     2339 2023-08-01 15:58:38.000000 pydata-google-auth-1.8.2/pydata_google_auth/_webserver.py
+-rw-r--r--   0 swast    (212416) primarygroup (89939)    20376 2023-08-01 16:04:45.000000 pydata-google-auth-1.8.2/pydata_google_auth/auth.py
+-rw-r--r--   0 swast    (212416) primarygroup (89939)     8789 2021-12-02 22:18:28.000000 pydata-google-auth-1.8.2/pydata_google_auth/cache.py
+-rw-r--r--   0 swast    (212416) primarygroup (89939)      262 2021-12-02 22:18:28.000000 pydata-google-auth-1.8.2/pydata_google_auth/exceptions.py
+drwxr-xr-x   0 swast    (212416) primarygroup (89939)        0 2023-08-01 17:02:17.691568 pydata-google-auth-1.8.2/pydata_google_auth.egg-info/
+-rw-r--r--   0 swast    (212416) primarygroup (89939)     2906 2023-08-01 17:02:17.000000 pydata-google-auth-1.8.2/pydata_google_auth.egg-info/PKG-INFO
+-rw-r--r--   0 swast    (212416) primarygroup (89939)      501 2023-08-01 17:02:17.000000 pydata-google-auth-1.8.2/pydata_google_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 swast    (212416) primarygroup (89939)        1 2023-08-01 17:02:17.000000 pydata-google-auth-1.8.2/pydata_google_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 swast    (212416) primarygroup (89939)      188 2023-08-01 17:02:17.000000 pydata-google-auth-1.8.2/pydata_google_auth.egg-info/requires.txt
+-rw-r--r--   0 swast    (212416) primarygroup (89939)       19 2023-08-01 17:02:17.000000 pydata-google-auth-1.8.2/pydata_google_auth.egg-info/top_level.txt
+-rw-r--r--   0 swast    (212416) primarygroup (89939)      356 2023-08-01 17:02:17.693312 pydata-google-auth-1.8.2/setup.cfg
+-rw-r--r--   0 swast    (212416) primarygroup (89939)     1859 2021-12-03 19:00:07.000000 pydata-google-auth-1.8.2/setup.py
+-rw-r--r--   0 swast    (212416) primarygroup (89939)    68752 2021-12-02 22:18:28.000000 pydata-google-auth-1.8.2/versioneer.py
```

### Comparing `pydata-google-auth-1.8.1/AUTHORS.md` & `pydata-google-auth-1.8.2/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `pydata-google-auth-1.8.1/LICENSE.txt` & `pydata-google-auth-1.8.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pydata-google-auth-1.8.1/PKG-INFO` & `pydata-google-auth-1.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydata-google-auth
-Version: 1.8.1
+Version: 1.8.2
 Summary: PyData helpers for authenticating to Google APIs
 Home-page: https://github.com/pydata/pydata-google-auth
 Author: The PyData Development Team
 Author-email: pydata@googlegroups.com
 License: BSD License
 Keywords: data
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pydata-google-auth-1.8.1/README.rst` & `pydata-google-auth-1.8.2/README.rst`

 * *Files identical despite different names*

### Comparing `pydata-google-auth-1.8.1/pydata_google_auth/__init__.py` & `pydata-google-auth-1.8.2/pydata_google_auth/__init__.py`

 * *Files identical despite different names*

### Comparing `pydata-google-auth-1.8.1/pydata_google_auth/__main__.py` & `pydata-google-auth-1.8.2/pydata_google_auth/__main__.py`

 * *Files identical despite different names*

### Comparing `pydata-google-auth-1.8.1/pydata_google_auth/_webserver.py` & `pydata-google-auth-1.8.2/pydata_google_auth/_webserver.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         if is_port_open(port):
             return port
 
     # No open ports found.
     return None
 
 
-def run_local_server(app_flow):
+def run_local_server(app_flow, **kwargs):
     """Run local webserver installed app flow on some open port.
 
     Parameters
     ----------
     app_flow : google_auth_oauthlib.flow.InstalledAppFlow
         Installed application flow to fetch user credentials.
 
@@ -82,8 +82,8 @@
     pydata_google_auth.exceptions.PyDataConnectionError
         If no open port can be found in the range from 8080 to 8089,
         inclusive.
     """
     port = find_open_port()
     if not port:
         raise exceptions.PyDataConnectionError("Could not find open port.")
-    return app_flow.run_local_server(host=LOCALHOST, port=port)
+    return app_flow.run_local_server(host=LOCALHOST, port=port, **kwargs)
```

### Comparing `pydata-google-auth-1.8.1/pydata_google_auth/auth.py` & `pydata-google-auth-1.8.2/pydata_google_auth/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,21 @@
     "262006177488-ka1m0ue4fptfmt9siejdd5lom7p39upa.apps.googleusercontent.com"
 )
 WEBAPP_CLIENT_SECRET = "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"
 
 GOOGLE_AUTH_URI = "https://accounts.google.com/o/oauth2/auth"
 GOOGLE_TOKEN_URI = "https://oauth2.googleapis.com/token"
 
+AUTH_URI_KWARGS = {
+    # Ensure that we get a refresh token by telling Google we want to assume
+    # this is first time we're authorizing this app. See:
+    # https://github.com/googleapis/google-api-python-client/issues/213#issuecomment-205886341
+    "prompt": "consent",
+}
+
 
 def _run_webapp(flow, redirect_uri=None, **kwargs):
 
     if redirect_uri:
         flow.redirect_uri = redirect_uri
     else:
         flow.redirect_uri = flow._OOB_REDIRECT_URI
@@ -348,17 +355,19 @@
     if credentials is None:
         app_flow = flow.InstalledAppFlow.from_client_config(
             client_config, scopes=scopes
         )
 
         try:
             if use_local_webserver:
-                credentials = _webserver.run_local_server(app_flow)
+                credentials = _webserver.run_local_server(app_flow, **AUTH_URI_KWARGS)
             else:
-                credentials = _run_webapp(app_flow, redirect_uri=redirect_uri)
+                credentials = _run_webapp(
+                    app_flow, redirect_uri=redirect_uri, **AUTH_URI_KWARGS
+                )
 
         except oauthlib.oauth2.rfc6749.errors.OAuth2Error as exc:
             raise exceptions.PyDataCredentialsError(
                 "Unable to get valid credentials: {}".format(exc)
             )
 
         credentials_cache.save(credentials)
```

### Comparing `pydata-google-auth-1.8.1/pydata_google_auth/cache.py` & `pydata-google-auth-1.8.2/pydata_google_auth/cache.py`

 * *Files identical despite different names*

### Comparing `pydata-google-auth-1.8.1/pydata_google_auth.egg-info/PKG-INFO` & `pydata-google-auth-1.8.2/pydata_google_auth.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydata-google-auth
-Version: 1.8.1
+Version: 1.8.2
 Summary: PyData helpers for authenticating to Google APIs
 Home-page: https://github.com/pydata/pydata-google-auth
 Author: The PyData Development Team
 Author-email: pydata@googlegroups.com
 License: BSD License
 Keywords: data
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pydata-google-auth-1.8.1/setup.py` & `pydata-google-auth-1.8.2/setup.py`

 * *Files identical despite different names*

### Comparing `pydata-google-auth-1.8.1/versioneer.py` & `pydata-google-auth-1.8.2/versioneer.py`

 * *Files identical despite different names*

