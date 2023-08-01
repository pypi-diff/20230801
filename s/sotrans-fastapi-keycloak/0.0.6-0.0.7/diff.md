# Comparing `tmp/sotrans_fastapi_keycloak-0.0.6.tar.gz` & `tmp/sotrans_fastapi_keycloak-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sotrans_fastapi_keycloak-0.0.6.tar", last modified: Tue Aug  1 11:28:14 2023, max compression
+gzip compressed data, was "sotrans_fastapi_keycloak-0.0.7.tar", last modified: Tue Aug  1 12:29:19 2023, max compression
```

## Comparing `sotrans_fastapi_keycloak-0.0.6.tar` & `sotrans_fastapi_keycloak-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 11:28:14.715340 sotrans_fastapi_keycloak-0.0.6/
--rw-rw-rw-   0        0        0    11564 2023-07-28 12:35:22.000000 sotrans_fastapi_keycloak-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     1122 2023-08-01 11:28:14.715340 sotrans_fastapi_keycloak-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      192 2023-07-28 12:39:31.000000 sotrans_fastapi_keycloak-0.0.6/README.md
--rw-rw-rw-   0        0        0     1314 2023-08-01 11:28:09.000000 sotrans_fastapi_keycloak-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-01 11:28:14.715340 sotrans_fastapi_keycloak-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      218 2023-07-28 13:49:01.000000 sotrans_fastapi_keycloak-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-01 11:28:14.699625 sotrans_fastapi_keycloak-0.0.6/sotrans_fastapi_keycloak/
--rw-rw-rw-   0        0        0      949 2023-07-28 12:39:31.000000 sotrans_fastapi_keycloak-0.0.6/sotrans_fastapi_keycloak/__init__.py
--rw-rw-rw-   0        0        0    47740 2023-08-01 11:14:20.000000 sotrans_fastapi_keycloak-0.0.6/sotrans_fastapi_keycloak/api.py
--rw-rw-rw-   0        0        0     2732 2023-07-25 23:29:41.000000 sotrans_fastapi_keycloak-0.0.6/sotrans_fastapi_keycloak/exceptions.py
--rw-rw-rw-   0        0        0     9124 2023-07-28 13:53:54.000000 sotrans_fastapi_keycloak-0.0.6/sotrans_fastapi_keycloak/model.py
--rw-rw-rw-   0        0        0     2096 2023-08-01 11:28:09.000000 sotrans_fastapi_keycloak-0.0.6/sotrans_fastapi_keycloak/sotrans_model.py
-drwxrwxrwx   0        0        0        0 2023-08-01 11:28:14.715340 sotrans_fastapi_keycloak-0.0.6/sotrans_fastapi_keycloak.egg-info/
--rw-rw-rw-   0        0        0     1122 2023-08-01 11:28:14.000000 sotrans_fastapi_keycloak-0.0.6/sotrans_fastapi_keycloak.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      464 2023-08-01 11:28:14.000000 sotrans_fastapi_keycloak-0.0.6/sotrans_fastapi_keycloak.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 11:28:14.000000 sotrans_fastapi_keycloak-0.0.6/sotrans_fastapi_keycloak.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      218 2023-08-01 11:28:14.000000 sotrans_fastapi_keycloak-0.0.6/sotrans_fastapi_keycloak.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-08-01 11:28:14.000000 sotrans_fastapi_keycloak-0.0.6/sotrans_fastapi_keycloak.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 12:29:19.517334 sotrans_fastapi_keycloak-0.0.7/
+-rw-rw-rw-   0        0        0    11564 2023-07-28 12:35:22.000000 sotrans_fastapi_keycloak-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     1122 2023-08-01 12:29:19.517334 sotrans_fastapi_keycloak-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2023-07-28 12:39:31.000000 sotrans_fastapi_keycloak-0.0.7/README.md
+-rw-rw-rw-   0        0        0     1314 2023-08-01 12:29:11.000000 sotrans_fastapi_keycloak-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-01 12:29:19.517334 sotrans_fastapi_keycloak-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      218 2023-07-28 13:49:01.000000 sotrans_fastapi_keycloak-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 12:29:19.498000 sotrans_fastapi_keycloak-0.0.7/sotrans_fastapi_keycloak/
+-rw-rw-rw-   0        0        0      949 2023-07-28 12:39:31.000000 sotrans_fastapi_keycloak-0.0.7/sotrans_fastapi_keycloak/__init__.py
+-rw-rw-rw-   0        0        0    47787 2023-08-01 12:28:40.000000 sotrans_fastapi_keycloak-0.0.7/sotrans_fastapi_keycloak/api.py
+-rw-rw-rw-   0        0        0     2732 2023-07-25 23:29:41.000000 sotrans_fastapi_keycloak-0.0.7/sotrans_fastapi_keycloak/exceptions.py
+-rw-rw-rw-   0        0        0     9124 2023-07-28 13:53:54.000000 sotrans_fastapi_keycloak-0.0.7/sotrans_fastapi_keycloak/model.py
+-rw-rw-rw-   0        0        0     2096 2023-08-01 12:28:40.000000 sotrans_fastapi_keycloak-0.0.7/sotrans_fastapi_keycloak/sotrans_model.py
+drwxrwxrwx   0        0        0        0 2023-08-01 12:29:19.516025 sotrans_fastapi_keycloak-0.0.7/sotrans_fastapi_keycloak.egg-info/
+-rw-rw-rw-   0        0        0     1122 2023-08-01 12:29:19.000000 sotrans_fastapi_keycloak-0.0.7/sotrans_fastapi_keycloak.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      464 2023-08-01 12:29:19.000000 sotrans_fastapi_keycloak-0.0.7/sotrans_fastapi_keycloak.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 12:29:19.000000 sotrans_fastapi_keycloak-0.0.7/sotrans_fastapi_keycloak.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      218 2023-08-01 12:29:19.000000 sotrans_fastapi_keycloak-0.0.7/sotrans_fastapi_keycloak.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-08-01 12:29:19.000000 sotrans_fastapi_keycloak-0.0.7/sotrans_fastapi_keycloak.egg-info/top_level.txt
```

### Comparing `sotrans_fastapi_keycloak-0.0.6/LICENSE` & `sotrans_fastapi_keycloak-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sotrans_fastapi_keycloak-0.0.6/PKG-INFO` & `sotrans_fastapi_keycloak-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sotrans_fastapi_keycloak
-Version: 0.0.6
+Version: 0.0.7
 Author-email: Jonas Scholl <jonas@code-specialist.com>, Yannic Schröer <yannic@code-specialist.com>
 Maintainer-email: Jonas Scholl <jonas@code-specialist.com>, Yannic Schröer <yannic@code-specialist.com>
 Keywords: Keycloak,FastAPI,Authentication,Authorization
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP :: Session
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
```

### Comparing `sotrans_fastapi_keycloak-0.0.6/pyproject.toml` & `sotrans_fastapi_keycloak-0.0.7/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -32,8 +32,8 @@
     "pydantic_core==2.4.0",
     "requests==2.31.0",
     "sniffio==1.3.0",
     "starlette==0.27.0",
     "typing_extensions==4.7.1",
     "urllib3==2.0.4"
 ]
-version = "0.0.6"
+version = "0.0.7"
```

### Comparing `sotrans_fastapi_keycloak-0.0.6/sotrans_fastapi_keycloak/__init__.py` & `sotrans_fastapi_keycloak-0.0.7/sotrans_fastapi_keycloak/__init__.py`

 * *Files identical despite different names*

### Comparing `sotrans_fastapi_keycloak-0.0.6/sotrans_fastapi_keycloak/api.py` & `sotrans_fastapi_keycloak-0.0.7/sotrans_fastapi_keycloak/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -814,15 +814,15 @@
             data.update(get_keycloak_user_model(model))
 
             response = self._admin_request(
                 url = self.users_uri, data = data, method = HTTPMethod.POST
             )
             if response.status_code != 201:
                 return response
-            user = self.get_user(query = f"username={model.username}")
+            user = self.get_user(query = f"username={model.username if hasattr(model, 'username') else model.email}")
             if send_email_verification:
                 self.send_email_verification(user.id)
             if initial_roles:
                 self.add_user_roles(initial_roles, user.id)
                 user = self.get_user(user_id = user.id)
             return user
```

### Comparing `sotrans_fastapi_keycloak-0.0.6/sotrans_fastapi_keycloak/exceptions.py` & `sotrans_fastapi_keycloak-0.0.7/sotrans_fastapi_keycloak/exceptions.py`

 * *Files identical despite different names*

### Comparing `sotrans_fastapi_keycloak-0.0.6/sotrans_fastapi_keycloak/model.py` & `sotrans_fastapi_keycloak-0.0.7/sotrans_fastapi_keycloak/model.py`

 * *Files identical despite different names*

### Comparing `sotrans_fastapi_keycloak-0.0.6/sotrans_fastapi_keycloak/sotrans_model.py` & `sotrans_fastapi_keycloak-0.0.7/sotrans_fastapi_keycloak/sotrans_model.py`

 * *Files identical despite different names*

### Comparing `sotrans_fastapi_keycloak-0.0.6/sotrans_fastapi_keycloak.egg-info/PKG-INFO` & `sotrans_fastapi_keycloak-0.0.7/sotrans_fastapi_keycloak.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sotrans-fastapi-keycloak
-Version: 0.0.6
+Version: 0.0.7
 Author-email: Jonas Scholl <jonas@code-specialist.com>, Yannic Schröer <yannic@code-specialist.com>
 Maintainer-email: Jonas Scholl <jonas@code-specialist.com>, Yannic Schröer <yannic@code-specialist.com>
 Keywords: Keycloak,FastAPI,Authentication,Authorization
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP :: Session
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
```

