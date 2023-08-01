# Comparing `tmp/sotrans_fastapi_keycloak-0.0.5.tar.gz` & `tmp/sotrans_fastapi_keycloak-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sotrans_fastapi_keycloak-0.0.5.tar", last modified: Tue Aug  1 11:21:50 2023, max compression
+gzip compressed data, was "sotrans_fastapi_keycloak-0.0.6.tar", last modified: Tue Aug  1 11:28:14 2023, max compression
```

## Comparing `sotrans_fastapi_keycloak-0.0.5.tar` & `sotrans_fastapi_keycloak-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 11:21:50.610728 sotrans_fastapi_keycloak-0.0.5/
--rw-rw-rw-   0        0        0    11564 2023-07-28 12:35:22.000000 sotrans_fastapi_keycloak-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     1122 2023-08-01 11:21:50.610728 sotrans_fastapi_keycloak-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      192 2023-07-28 12:39:31.000000 sotrans_fastapi_keycloak-0.0.5/README.md
--rw-rw-rw-   0        0        0     1314 2023-08-01 11:21:45.000000 sotrans_fastapi_keycloak-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-01 11:21:50.610728 sotrans_fastapi_keycloak-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      218 2023-07-28 13:49:01.000000 sotrans_fastapi_keycloak-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-01 11:21:50.596383 sotrans_fastapi_keycloak-0.0.5/sotrans_fastapi_keycloak/
--rw-rw-rw-   0        0        0      949 2023-07-28 12:39:31.000000 sotrans_fastapi_keycloak-0.0.5/sotrans_fastapi_keycloak/__init__.py
--rw-rw-rw-   0        0        0    47740 2023-08-01 11:14:20.000000 sotrans_fastapi_keycloak-0.0.5/sotrans_fastapi_keycloak/api.py
--rw-rw-rw-   0        0        0     2732 2023-07-25 23:29:41.000000 sotrans_fastapi_keycloak-0.0.5/sotrans_fastapi_keycloak/exceptions.py
--rw-rw-rw-   0        0        0     9124 2023-07-28 13:53:54.000000 sotrans_fastapi_keycloak-0.0.5/sotrans_fastapi_keycloak/model.py
--rw-rw-rw-   0        0        0     1856 2023-08-01 11:21:21.000000 sotrans_fastapi_keycloak-0.0.5/sotrans_fastapi_keycloak/sotrans_model.py
-drwxrwxrwx   0        0        0        0 2023-08-01 11:21:50.610728 sotrans_fastapi_keycloak-0.0.5/sotrans_fastapi_keycloak.egg-info/
--rw-rw-rw-   0        0        0     1122 2023-08-01 11:21:50.000000 sotrans_fastapi_keycloak-0.0.5/sotrans_fastapi_keycloak.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      464 2023-08-01 11:21:50.000000 sotrans_fastapi_keycloak-0.0.5/sotrans_fastapi_keycloak.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 11:21:50.000000 sotrans_fastapi_keycloak-0.0.5/sotrans_fastapi_keycloak.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      218 2023-08-01 11:21:50.000000 sotrans_fastapi_keycloak-0.0.5/sotrans_fastapi_keycloak.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-08-01 11:21:50.000000 sotrans_fastapi_keycloak-0.0.5/sotrans_fastapi_keycloak.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 11:28:14.715340 sotrans_fastapi_keycloak-0.0.6/
+-rw-rw-rw-   0        0        0    11564 2023-07-28 12:35:22.000000 sotrans_fastapi_keycloak-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     1122 2023-08-01 11:28:14.715340 sotrans_fastapi_keycloak-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2023-07-28 12:39:31.000000 sotrans_fastapi_keycloak-0.0.6/README.md
+-rw-rw-rw-   0        0        0     1314 2023-08-01 11:28:09.000000 sotrans_fastapi_keycloak-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-01 11:28:14.715340 sotrans_fastapi_keycloak-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      218 2023-07-28 13:49:01.000000 sotrans_fastapi_keycloak-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 11:28:14.699625 sotrans_fastapi_keycloak-0.0.6/sotrans_fastapi_keycloak/
+-rw-rw-rw-   0        0        0      949 2023-07-28 12:39:31.000000 sotrans_fastapi_keycloak-0.0.6/sotrans_fastapi_keycloak/__init__.py
+-rw-rw-rw-   0        0        0    47740 2023-08-01 11:14:20.000000 sotrans_fastapi_keycloak-0.0.6/sotrans_fastapi_keycloak/api.py
+-rw-rw-rw-   0        0        0     2732 2023-07-25 23:29:41.000000 sotrans_fastapi_keycloak-0.0.6/sotrans_fastapi_keycloak/exceptions.py
+-rw-rw-rw-   0        0        0     9124 2023-07-28 13:53:54.000000 sotrans_fastapi_keycloak-0.0.6/sotrans_fastapi_keycloak/model.py
+-rw-rw-rw-   0        0        0     2096 2023-08-01 11:28:09.000000 sotrans_fastapi_keycloak-0.0.6/sotrans_fastapi_keycloak/sotrans_model.py
+drwxrwxrwx   0        0        0        0 2023-08-01 11:28:14.715340 sotrans_fastapi_keycloak-0.0.6/sotrans_fastapi_keycloak.egg-info/
+-rw-rw-rw-   0        0        0     1122 2023-08-01 11:28:14.000000 sotrans_fastapi_keycloak-0.0.6/sotrans_fastapi_keycloak.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      464 2023-08-01 11:28:14.000000 sotrans_fastapi_keycloak-0.0.6/sotrans_fastapi_keycloak.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 11:28:14.000000 sotrans_fastapi_keycloak-0.0.6/sotrans_fastapi_keycloak.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      218 2023-08-01 11:28:14.000000 sotrans_fastapi_keycloak-0.0.6/sotrans_fastapi_keycloak.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-08-01 11:28:14.000000 sotrans_fastapi_keycloak-0.0.6/sotrans_fastapi_keycloak.egg-info/top_level.txt
```

### Comparing `sotrans_fastapi_keycloak-0.0.5/LICENSE` & `sotrans_fastapi_keycloak-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sotrans_fastapi_keycloak-0.0.5/PKG-INFO` & `sotrans_fastapi_keycloak-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sotrans_fastapi_keycloak
-Version: 0.0.5
+Version: 0.0.6
 Author-email: Jonas Scholl <jonas@code-specialist.com>, Yannic Schröer <yannic@code-specialist.com>
 Maintainer-email: Jonas Scholl <jonas@code-specialist.com>, Yannic Schröer <yannic@code-specialist.com>
 Keywords: Keycloak,FastAPI,Authentication,Authorization
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP :: Session
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
```

### Comparing `sotrans_fastapi_keycloak-0.0.5/pyproject.toml` & `sotrans_fastapi_keycloak-0.0.6/pyproject.toml`

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
-version = "0.0.5"
+version = "0.0.6"
```

### Comparing `sotrans_fastapi_keycloak-0.0.5/sotrans_fastapi_keycloak/__init__.py` & `sotrans_fastapi_keycloak-0.0.6/sotrans_fastapi_keycloak/__init__.py`

 * *Files identical despite different names*

### Comparing `sotrans_fastapi_keycloak-0.0.5/sotrans_fastapi_keycloak/api.py` & `sotrans_fastapi_keycloak-0.0.6/sotrans_fastapi_keycloak/api.py`

 * *Files identical despite different names*

### Comparing `sotrans_fastapi_keycloak-0.0.5/sotrans_fastapi_keycloak/exceptions.py` & `sotrans_fastapi_keycloak-0.0.6/sotrans_fastapi_keycloak/exceptions.py`

 * *Files identical despite different names*

### Comparing `sotrans_fastapi_keycloak-0.0.5/sotrans_fastapi_keycloak/model.py` & `sotrans_fastapi_keycloak-0.0.6/sotrans_fastapi_keycloak/model.py`

 * *Files identical despite different names*

### Comparing `sotrans_fastapi_keycloak-0.0.5/sotrans_fastapi_keycloak/sotrans_model.py` & `sotrans_fastapi_keycloak-0.0.6/sotrans_fastapi_keycloak/sotrans_model.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Any, Annotated
 
 from pydantic import BaseModel, model_validator, model_serializer
 from sotrans_fastapi_keycloak.model import KeycloakUserBaseModel, OIDCUserBaseModel, user_model_attributes_validator, \
     user_model_attributes_serializer, KeycloakUserAttribute
 
-KeycloakUserStrAttribute = Annotated[str | None, KeycloakUserAttribute()]
+KeycloakUserOptionalStrAttribute = Annotated[str | None, KeycloakUserAttribute()]
+KeycloakUserStrAttribute = Annotated[str, KeycloakUserAttribute()]
 
 
 class SotransKeycloakUserBaseModel(BaseModel):
     @model_validator(mode = 'before')
     @classmethod
     def validate(cls: type[BaseModel], value: Any) -> Any:
         return user_model_attributes_validator(cls, value)
@@ -16,32 +17,32 @@
     def model_dump_keycloak(self):
         return user_model_attributes_serializer(self)
 
 
 class SotransKeycloakUserInfoModel(SotransKeycloakUserBaseModel):
     """Represents an update Keycloak user object in SOTRANS configuration"""
     email: str | None = None
-    name: KeycloakUserStrAttribute = None
-    surname: KeycloakUserStrAttribute = None
-    patronymic: KeycloakUserStrAttribute = None
-    phone: KeycloakUserStrAttribute = None
-    job_title: KeycloakUserStrAttribute = None
-    status: KeycloakUserStrAttribute = None
-    photo: KeycloakUserStrAttribute = None
-    subsidiary_id: KeycloakUserStrAttribute = None
-    organization_id: KeycloakUserStrAttribute = None
-    note: KeycloakUserStrAttribute = None
+    name: KeycloakUserOptionalStrAttribute = None
+    surname: KeycloakUserOptionalStrAttribute = None
+    patronymic: KeycloakUserOptionalStrAttribute = None
+    phone: KeycloakUserOptionalStrAttribute = None
+    job_title: KeycloakUserOptionalStrAttribute = None
+    status: KeycloakUserOptionalStrAttribute = None
+    photo: KeycloakUserOptionalStrAttribute = None
+    subsidiary_id: KeycloakUserOptionalStrAttribute = None
+    organization_id: KeycloakUserOptionalStrAttribute = None
+    note: KeycloakUserOptionalStrAttribute = None
 
 
 class SotransKeycloakUserCreateModel(SotransKeycloakUserBaseModel):
     """Represents a creation Keycloak user object in SOTRANS configuration"""
-    name: str
-    surname: str
-    patronymic: str
-    phone: str
+    name: KeycloakUserStrAttribute
+    surname: KeycloakUserStrAttribute
+    patronymic: KeycloakUserStrAttribute
+    phone: KeycloakUserStrAttribute
     email: str
     password: str
 
 
 class SotransKeycloakUserModel(KeycloakUserBaseModel, SotransKeycloakUserInfoModel):
     """Represents a full Keycloak user object in SOTRANS configuration"""
     pass
```

### Comparing `sotrans_fastapi_keycloak-0.0.5/sotrans_fastapi_keycloak.egg-info/PKG-INFO` & `sotrans_fastapi_keycloak-0.0.6/sotrans_fastapi_keycloak.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sotrans-fastapi-keycloak
-Version: 0.0.5
+Version: 0.0.6
 Author-email: Jonas Scholl <jonas@code-specialist.com>, Yannic Schröer <yannic@code-specialist.com>
 Maintainer-email: Jonas Scholl <jonas@code-specialist.com>, Yannic Schröer <yannic@code-specialist.com>
 Keywords: Keycloak,FastAPI,Authentication,Authorization
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP :: Session
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
```

