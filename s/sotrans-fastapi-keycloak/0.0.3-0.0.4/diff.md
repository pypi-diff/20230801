# Comparing `tmp/sotrans_fastapi_keycloak-0.0.3.tar.gz` & `tmp/sotrans_fastapi_keycloak-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sotrans_fastapi_keycloak-0.0.3.tar", last modified: Mon Jul 31 15:51:50 2023, max compression
+gzip compressed data, was "sotrans_fastapi_keycloak-0.0.4.tar", last modified: Tue Aug  1 11:15:18 2023, max compression
```

## Comparing `sotrans_fastapi_keycloak-0.0.3.tar` & `sotrans_fastapi_keycloak-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 15:51:50.643337 sotrans_fastapi_keycloak-0.0.3/
--rw-rw-rw-   0        0        0    11564 2023-07-28 12:35:22.000000 sotrans_fastapi_keycloak-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     1122 2023-07-31 15:51:50.642830 sotrans_fastapi_keycloak-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      192 2023-07-28 12:39:31.000000 sotrans_fastapi_keycloak-0.0.3/README.md
--rw-rw-rw-   0        0        0     1314 2023-07-31 15:51:42.000000 sotrans_fastapi_keycloak-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-31 15:51:50.643337 sotrans_fastapi_keycloak-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      218 2023-07-28 13:49:01.000000 sotrans_fastapi_keycloak-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-31 15:51:50.624916 sotrans_fastapi_keycloak-0.0.3/sotrans_fastapi_keycloak/
--rw-rw-rw-   0        0        0      949 2023-07-28 12:39:31.000000 sotrans_fastapi_keycloak-0.0.3/sotrans_fastapi_keycloak/__init__.py
--rw-rw-rw-   0        0        0    47534 2023-07-31 15:51:42.000000 sotrans_fastapi_keycloak-0.0.3/sotrans_fastapi_keycloak/api.py
--rw-rw-rw-   0        0        0     2732 2023-07-25 23:29:41.000000 sotrans_fastapi_keycloak-0.0.3/sotrans_fastapi_keycloak/exceptions.py
--rw-rw-rw-   0        0        0     9124 2023-07-28 13:53:54.000000 sotrans_fastapi_keycloak-0.0.3/sotrans_fastapi_keycloak/model.py
--rw-rw-rw-   0        0        0     1768 2023-07-28 12:39:31.000000 sotrans_fastapi_keycloak-0.0.3/sotrans_fastapi_keycloak/sotrans_model.py
-drwxrwxrwx   0        0        0        0 2023-07-31 15:51:50.640769 sotrans_fastapi_keycloak-0.0.3/sotrans_fastapi_keycloak.egg-info/
--rw-rw-rw-   0        0        0     1122 2023-07-31 15:51:50.000000 sotrans_fastapi_keycloak-0.0.3/sotrans_fastapi_keycloak.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      464 2023-07-31 15:51:50.000000 sotrans_fastapi_keycloak-0.0.3/sotrans_fastapi_keycloak.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 15:51:50.000000 sotrans_fastapi_keycloak-0.0.3/sotrans_fastapi_keycloak.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      218 2023-07-31 15:51:50.000000 sotrans_fastapi_keycloak-0.0.3/sotrans_fastapi_keycloak.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-07-31 15:51:50.000000 sotrans_fastapi_keycloak-0.0.3/sotrans_fastapi_keycloak.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 11:15:18.035283 sotrans_fastapi_keycloak-0.0.4/
+-rw-rw-rw-   0        0        0    11564 2023-07-28 12:35:22.000000 sotrans_fastapi_keycloak-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     1122 2023-08-01 11:15:18.032525 sotrans_fastapi_keycloak-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2023-07-28 12:39:31.000000 sotrans_fastapi_keycloak-0.0.4/README.md
+-rw-rw-rw-   0        0        0     1314 2023-08-01 11:15:16.000000 sotrans_fastapi_keycloak-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-01 11:15:18.035283 sotrans_fastapi_keycloak-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      218 2023-07-28 13:49:01.000000 sotrans_fastapi_keycloak-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 11:15:18.020078 sotrans_fastapi_keycloak-0.0.4/sotrans_fastapi_keycloak/
+-rw-rw-rw-   0        0        0      949 2023-07-28 12:39:31.000000 sotrans_fastapi_keycloak-0.0.4/sotrans_fastapi_keycloak/__init__.py
+-rw-rw-rw-   0        0        0    47740 2023-08-01 11:14:20.000000 sotrans_fastapi_keycloak-0.0.4/sotrans_fastapi_keycloak/api.py
+-rw-rw-rw-   0        0        0     2732 2023-07-25 23:29:41.000000 sotrans_fastapi_keycloak-0.0.4/sotrans_fastapi_keycloak/exceptions.py
+-rw-rw-rw-   0        0        0     9124 2023-07-28 13:53:54.000000 sotrans_fastapi_keycloak-0.0.4/sotrans_fastapi_keycloak/model.py
+-rw-rw-rw-   0        0        0     1768 2023-07-28 12:39:31.000000 sotrans_fastapi_keycloak-0.0.4/sotrans_fastapi_keycloak/sotrans_model.py
+drwxrwxrwx   0        0        0        0 2023-08-01 11:15:18.032525 sotrans_fastapi_keycloak-0.0.4/sotrans_fastapi_keycloak.egg-info/
+-rw-rw-rw-   0        0        0     1122 2023-08-01 11:15:17.000000 sotrans_fastapi_keycloak-0.0.4/sotrans_fastapi_keycloak.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      464 2023-08-01 11:15:17.000000 sotrans_fastapi_keycloak-0.0.4/sotrans_fastapi_keycloak.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 11:15:17.000000 sotrans_fastapi_keycloak-0.0.4/sotrans_fastapi_keycloak.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      218 2023-08-01 11:15:17.000000 sotrans_fastapi_keycloak-0.0.4/sotrans_fastapi_keycloak.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-08-01 11:15:17.000000 sotrans_fastapi_keycloak-0.0.4/sotrans_fastapi_keycloak.egg-info/top_level.txt
```

### Comparing `sotrans_fastapi_keycloak-0.0.3/LICENSE` & `sotrans_fastapi_keycloak-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sotrans_fastapi_keycloak-0.0.3/PKG-INFO` & `sotrans_fastapi_keycloak-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sotrans_fastapi_keycloak
-Version: 0.0.3
+Version: 0.0.4
 Author-email: Jonas Scholl <jonas@code-specialist.com>, Yannic Schröer <yannic@code-specialist.com>
 Maintainer-email: Jonas Scholl <jonas@code-specialist.com>, Yannic Schröer <yannic@code-specialist.com>
 Keywords: Keycloak,FastAPI,Authentication,Authorization
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP :: Session
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
```

### Comparing `sotrans_fastapi_keycloak-0.0.3/pyproject.toml` & `sotrans_fastapi_keycloak-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -32,8 +32,8 @@
     "pydantic_core==2.4.0",
     "requests==2.31.0",
     "sniffio==1.3.0",
     "starlette==0.27.0",
     "typing_extensions==4.7.1",
     "urllib3==2.0.4"
 ]
-version = "0.0.3"
+version = "0.0.4"
```

### Comparing `sotrans_fastapi_keycloak-0.0.3/sotrans_fastapi_keycloak/__init__.py` & `sotrans_fastapi_keycloak-0.0.4/sotrans_fastapi_keycloak/__init__.py`

 * *Files identical despite different names*

### Comparing `sotrans_fastapi_keycloak-0.0.3/sotrans_fastapi_keycloak/api.py` & `sotrans_fastapi_keycloak-0.0.4/sotrans_fastapi_keycloak/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,14 +115,27 @@
                 raise_from_response(result)
 
         return wrapper
 
     return inner
 
 
+def get_keycloak_user_model(model: BaseModel) -> dict[str, Any]:
+    """Dump pydantic user model to keycloak representation (i.e. move all custom fields to attributes)
+
+    Args:
+        model: model to dump
+
+    Returns: dict model representation
+    """
+    return model.model_dump_keycloak() if hasattr(model, 'model_dump_keycloak') else model.model_dump(
+        exclude_unset = True
+    )
+
+
 class FastAPIKeycloak:
     """Instance to wrap the Keycloak API with FastAPI
 
     Attributes: _admin_token (KeycloakToken): A KeycloakToken instance, containing the access token that is used for
     any admin related request
 
     Example:
@@ -793,15 +806,16 @@
                 "enabled": enabled,
                 "credentials": [
                     {"temporary": False, "type": "password", "value": model.password}
                 ],
                 "requiredActions": ["VERIFY_EMAIL" if send_email_verification else None],
                 "attributes": attributes,
             }
-            data.update(model.model_dump(exclude = {'password'}))
+            model.password = None
+            data.update(get_keycloak_user_model(model))
 
             response = self._admin_request(
                 url = self.users_uri, data = data, method = HTTPMethod.POST
             )
             if response.status_code != 201:
                 return response
             user = self.get_user(query = f"username={model.username}")
@@ -917,19 +931,14 @@
 
         Notes: - You may alter any aspect of the user object, also the requiredActions for instance. There is no
         explicit function for updating those as it is a user update in essence
         """
 
         @result_or_error(response_model = self._user_model)
         def impl():
-            def get_keycloak_user_model(model):
-                return model.model_dump_keycloak() if hasattr(model, 'model_dump_keycloak') else model.model_dump(
-                    exclude_unset = True
-                )
-
             def update(d, u):
                 for k, v in u.items():
                     if isinstance(v, collections.abc.Mapping):
                         d[k] = update(d.get(k, {}), v)
                     else:
                         d[k] = v
                 return d
```

### Comparing `sotrans_fastapi_keycloak-0.0.3/sotrans_fastapi_keycloak/exceptions.py` & `sotrans_fastapi_keycloak-0.0.4/sotrans_fastapi_keycloak/exceptions.py`

 * *Files identical despite different names*

### Comparing `sotrans_fastapi_keycloak-0.0.3/sotrans_fastapi_keycloak/model.py` & `sotrans_fastapi_keycloak-0.0.4/sotrans_fastapi_keycloak/model.py`

 * *Files identical despite different names*

### Comparing `sotrans_fastapi_keycloak-0.0.3/sotrans_fastapi_keycloak/sotrans_model.py` & `sotrans_fastapi_keycloak-0.0.4/sotrans_fastapi_keycloak/sotrans_model.py`

 * *Files identical despite different names*

### Comparing `sotrans_fastapi_keycloak-0.0.3/sotrans_fastapi_keycloak.egg-info/PKG-INFO` & `sotrans_fastapi_keycloak-0.0.4/sotrans_fastapi_keycloak.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sotrans-fastapi-keycloak
-Version: 0.0.3
+Version: 0.0.4
 Author-email: Jonas Scholl <jonas@code-specialist.com>, Yannic Schröer <yannic@code-specialist.com>
 Maintainer-email: Jonas Scholl <jonas@code-specialist.com>, Yannic Schröer <yannic@code-specialist.com>
 Keywords: Keycloak,FastAPI,Authentication,Authorization
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP :: Session
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
```

