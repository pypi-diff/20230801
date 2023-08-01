# Comparing `tmp/drf_keycloak_auth-0.2.1.tar.gz` & `tmp/drf_keycloak_auth-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf_keycloak_auth-0.2.1.tar", last modified: Wed Jul 19 11:43:59 2023, max compression
+gzip compressed data, was "drf_keycloak_auth-0.2.2.tar", last modified: Tue Aug  1 03:27:53 2023, max compression
```

## Comparing `drf_keycloak_auth-0.2.1.tar` & `drf_keycloak_auth-0.2.2.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 11:43:59.018394 drf_keycloak_auth-0.2.1/
--rw-rw-rw-   0 root         (0) root         (0)     1077 2023-07-19 11:43:55.000000 drf_keycloak_auth-0.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5347 2023-07-19 11:43:59.017394 drf_keycloak_auth-0.2.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4729 2023-07-19 11:43:55.000000 drf_keycloak_auth-0.2.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 11:43:59.016394 drf_keycloak_auth-0.2.1/drf_keycloak_auth/
--rw-rw-rw-   0 root         (0) root         (0)      378 2023-07-19 11:43:55.000000 drf_keycloak_auth-0.2.1/drf_keycloak_auth/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-07-19 11:43:55.000000 drf_keycloak_auth-0.2.1/drf_keycloak_auth/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      110 2023-07-19 11:43:55.000000 drf_keycloak_auth-0.2.1/drf_keycloak_auth/apps.py
--rw-rw-rw-   0 root         (0) root         (0)    11993 2023-07-19 11:43:55.000000 drf_keycloak_auth-0.2.1/drf_keycloak_auth/authentication.py
--rw-rw-rw-   0 root         (0) root         (0)     2638 2023-07-19 11:43:55.000000 drf_keycloak_auth-0.2.1/drf_keycloak_auth/keycloak.py
--rw-rw-rw-   0 root         (0) root         (0)       81 2023-07-19 11:43:55.000000 drf_keycloak_auth-0.2.1/drf_keycloak_auth/models.py
--rw-rw-rw-   0 root         (0) root         (0)     3509 2023-07-19 11:43:55.000000 drf_keycloak_auth-0.2.1/drf_keycloak_auth/permissions.py
--rw-rw-rw-   0 root         (0) root         (0)     1878 2023-07-19 11:43:55.000000 drf_keycloak_auth-0.2.1/drf_keycloak_auth/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 11:43:59.017394 drf_keycloak_auth-0.2.1/drf_keycloak_auth.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5347 2023-07-19 11:43:58.000000 drf_keycloak_auth-0.2.1/drf_keycloak_auth.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      470 2023-07-19 11:43:58.000000 drf_keycloak_auth-0.2.1/drf_keycloak_auth.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 11:43:58.000000 drf_keycloak_auth-0.2.1/drf_keycloak_auth.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       86 2023-07-19 11:43:58.000000 drf_keycloak_auth-0.2.1/drf_keycloak_auth.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-19 11:43:58.000000 drf_keycloak_auth-0.2.1/drf_keycloak_auth.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-19 11:43:59.018394 drf_keycloak_auth-0.2.1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1142 2023-07-19 11:43:55.000000 drf_keycloak_auth-0.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 03:27:52.987605 drf_keycloak_auth-0.2.2/
+-rw-rw-rw-   0 root         (0) root         (0)     1077 2023-08-01 03:27:48.000000 drf_keycloak_auth-0.2.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5346 2023-08-01 03:27:52.987605 drf_keycloak_auth-0.2.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4728 2023-08-01 03:27:48.000000 drf_keycloak_auth-0.2.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 03:27:52.985605 drf_keycloak_auth-0.2.2/drf_keycloak_auth/
+-rw-rw-rw-   0 root         (0) root         (0)      378 2023-08-01 03:27:48.000000 drf_keycloak_auth-0.2.2/drf_keycloak_auth/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-08-01 03:27:48.000000 drf_keycloak_auth-0.2.2/drf_keycloak_auth/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      110 2023-08-01 03:27:48.000000 drf_keycloak_auth-0.2.2/drf_keycloak_auth/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)    11703 2023-08-01 03:27:48.000000 drf_keycloak_auth-0.2.2/drf_keycloak_auth/authentication.py
+-rw-rw-rw-   0 root         (0) root         (0)     4811 2023-08-01 03:27:48.000000 drf_keycloak_auth-0.2.2/drf_keycloak_auth/keycloak.py
+-rw-rw-rw-   0 root         (0) root         (0)       81 2023-08-01 03:27:48.000000 drf_keycloak_auth-0.2.2/drf_keycloak_auth/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     3509 2023-08-01 03:27:48.000000 drf_keycloak_auth-0.2.2/drf_keycloak_auth/permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1838 2023-08-01 03:27:48.000000 drf_keycloak_auth-0.2.2/drf_keycloak_auth/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)      938 2023-08-01 03:27:48.000000 drf_keycloak_auth-0.2.2/drf_keycloak_auth/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 03:27:52.986605 drf_keycloak_auth-0.2.2/drf_keycloak_auth.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5346 2023-08-01 03:27:52.000000 drf_keycloak_auth-0.2.2/drf_keycloak_auth.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      497 2023-08-01 03:27:52.000000 drf_keycloak_auth-0.2.2/drf_keycloak_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 03:27:52.000000 drf_keycloak_auth-0.2.2/drf_keycloak_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       97 2023-08-01 03:27:52.000000 drf_keycloak_auth-0.2.2/drf_keycloak_auth.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-08-01 03:27:52.000000 drf_keycloak_auth-0.2.2/drf_keycloak_auth.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-01 03:27:52.987605 drf_keycloak_auth-0.2.2/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1164 2023-08-01 03:27:48.000000 drf_keycloak_auth-0.2.2/setup.py
```

### Comparing `drf_keycloak_auth-0.2.1/LICENSE` & `drf_keycloak_auth-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `drf_keycloak_auth-0.2.1/PKG-INFO` & `drf_keycloak_auth-0.2.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf_keycloak_auth
-Version: 0.2.1
+Version: 0.2.2
 Summary: A convenience libary for authenticating users from Keycloak access tokens
 Home-page: https://gitlab.com/ecocommons-australia/lib/drf-keycloak-auth
 Author: EcoCommons Australia
 Author-email: ecocommons@griffith.edu.au
 License: MIT
 Keywords: drf,django,rest_framework,djangorestframework,authentication,python3,keycloak
 Classifier: Programming Language :: Python :: 3
@@ -129,15 +129,15 @@
 ```
 KEYCLOAK_DJANGO_USER_UUID_FIELD = 'uuid'
 ```
 
 Voila!
 
 
-## Multi tennancy support
+## Multi tenancy support
 
 An application can be configured for multiple tenancies by using different Keycloak Realms on the same or seperate Keycloak instances by using the environment var `KEYCLOAK_MULTI_OIDC_JSON`
 
 The client OIDC adaptor json file can be downloaded from Keycloak.
 
 ```
 KEYCLOAK_MULTI_OIDC_JSON=
```

### Comparing `drf_keycloak_auth-0.2.1/README.md` & `drf_keycloak_auth-0.2.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,15 @@
 ```
 KEYCLOAK_DJANGO_USER_UUID_FIELD = 'uuid'
 ```
 
 Voila!
 
 
-## Multi tennancy support
+## Multi tenancy support
 
 An application can be configured for multiple tenancies by using different Keycloak Realms on the same or seperate Keycloak instances by using the environment var `KEYCLOAK_MULTI_OIDC_JSON`
 
 The client OIDC adaptor json file can be downloaded from Keycloak.
 
 ```
 KEYCLOAK_MULTI_OIDC_JSON=
```

### Comparing `drf_keycloak_auth-0.2.1/drf_keycloak_auth/authentication.py` & `drf_keycloak_auth-0.2.2/drf_keycloak_auth/authentication.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,56 +9,67 @@
 from rest_framework import (
     authentication,
     exceptions,
 )
 from rest_framework.exceptions import AuthenticationFailed
 from keycloak import KeycloakOpenID
 from .keycloak import (
+    OIDCConfigException,
     get_keycloak_openid,
     get_resource_roles,
     add_roles_prefix
 )
 from .settings import api_settings
+from .utils import get_token_issuer
 from . import __title__
 
 
 log = logging.getLogger(__title__)
 User = get_user_model()
 
 
-class OIDCConfigException(Exception):
-    pass
-
-
 class KeycloakAuthentication(authentication.TokenAuthentication):
     keyword = api_settings.KEYCLOAK_AUTH_HEADER_PREFIX
 
     keycloak_openid = None
 
     def authenticate(self, request):
-        if self.keycloak_openid is None:
-            self.keycloak_openid = get_keycloak_openid()
-
         credentials = super().authenticate(request)
         if credentials:
             user, decoded_token = credentials
+
+            # Append realm_name
+            decoded_token.update(
+                {'realm_name': self.keycloak_openid.realm_name}
+            )
+
+            # Expose Keycloak roles
             request.roles = self._get_roles(user, decoded_token)
+
+            # Create local application groups?
             if api_settings.KEYCLOAK_MANAGE_LOCAL_GROUPS is True:
                 groups = self._get_or_create_groups(request.roles)
                 user.groups.set(groups)
+
+            # Set user is_staff based on Keycloak role mapping
             self._user_toggle_is_staff(request, user)
+
         return credentials
 
     def authenticate_credentials(
         self,
         key: str
     ) -> Tuple[AnonymousUser, Dict]:
         """ Attempt to verify JWT from Authorization header with Keycloak """
         log.debug('KeycloakAuthentication.authenticate_credentials')
         try:
+            # Create a default KeycloakOpenID configuration if not already available
+            if self.keycloak_openid is None:
+                self.keycloak_openid = get_keycloak_openid()
+
             user = None
             # Checks token is active
             decoded_token = self._get_decoded_token(key)
             self._verify_token_active(decoded_token)
             if api_settings.KEYCLOAK_MANAGE_LOCAL_USER is not True:
                 log.debug(
                     'KeycloakAuthentication.authenticate_credentials: '
@@ -92,21 +103,21 @@
         if not is_active:
             raise AuthenticationFailed(
                 'invalid or expired token'
             )
 
     def _add_realm_prefix(self, value: str) -> str:
         """ Add 'REALM_NAME:' prefix to a string value.
-            This only works if KEYCLOAK_REALM_PREFIX_DJANGO_USERNAME is True.
-            
+            This only works if using KEYCLOAK_MULTI_OIDC_JSON
+
             Checks to ensure the prefix is not already added.
             :param value: The string to prefix
             :returns: Prefixed string
         """
-        if not api_settings.KEYCLOAK_REALM_PREFIX_DJANGO_USERNAME:
+        if not api_settings.KEYCLOAK_MULTI_OIDC_JSON:
             return value
 
         if not self.keycloak_openid.realm_name:
             log.warning(f"Cannot add realm prefix. Realm missing!")
             return value
 
         prefix = str(self.keycloak_openid.realm_name)+':'
@@ -279,65 +290,48 @@
             log.warning(
                 'KeycloakAuthentication._user_toggle_is_staff | '
                 f'Exception: {e}'
             )
 
 
 class KeycloakMultiAuthentication(KeycloakAuthentication):
+    """ Keycloak authentication for multiple realms. Determined by KEYCLOAK_MULTI_OIDC_JSON"""
+
+    def authenticate_credentials(
+        self,
+        key: str
+    ) -> Tuple[AnonymousUser, Dict]:
+        """ 
+            Decode the unverified token to get the issuer and validate it against ALLOWED_HOSTS.
+            This determines the auth realm 
+        """
 
-    def authenticate(self, request):
         if api_settings.KEYCLOAK_MULTI_OIDC_JSON is None:
-            log.warning(
+            log.info(
                 'KeycloakMultiAuthentication.authenticate | '
                 'api_settings.KEYCLOAK_MULTI_OIDC_JSON is empty'
             )
-            return None
-
-        credentials = None
-
-        def get_host_oidc(hostname: str, oidc_dict: dict) -> KeycloakOpenID:
-            for key, oidc in oidc_dict.items():
-                if key in str(hostname):
-                    log.info(f"get_host_oidc: Found OIDC adapter for '{hostname}'")
-                    return get_keycloak_openid(oidc)
-            return None
-
-        # Resolve OIDC adapter by hostname
-        if not isinstance(api_settings.KEYCLOAK_MULTI_OIDC_JSON, dict):
-            raise OIDCConfigException(f"OIDC config not available")
 
         try:
-            self.keycloak_openid = get_host_oidc(
-                request.get_host(),
-                api_settings.KEYCLOAK_MULTI_OIDC_JSON)
-
-            if self.keycloak_openid is None:
-                raise OIDCConfigException(f"Could not determine OIDC adapter for "
-                                          f"'{str(request.get_host())}'. Trying all")
-
-            credentials = super().authenticate(request)
-            if credentials:
-                # Append realm_name
-                credentials[1].update(
-                    {'realm_name': self.keycloak_openid.realm_name}
-                )
-                return credentials
+            self.keycloak_openid = get_keycloak_openid(host=get_token_issuer(key))
+            return super().authenticate_credentials(key)
 
         except OIDCConfigException as e:
             log.warning(
                 'KeycloakMultiAuthentication.authenticate | '
                 f'OIDCConfigException: {e})'
             )
+            raise AuthenticationFailed() from e
 
         except AuthenticationFailed as e:
             log.info(
                 'KeycloakMultiAuthentication.authenticate | '
                 f'AuthenticationFailed: {e})'
             )
+            raise e
 
         except Exception as e:
             log.error(
                 'KeycloakMultiAuthentication.authenticate | '
                 f'Exception: {e})'
             )
-
-        return credentials
+            raise AuthenticationFailed() from e
```

### Comparing `drf_keycloak_auth-0.2.1/drf_keycloak_auth/permissions.py` & `drf_keycloak_auth-0.2.2/drf_keycloak_auth/permissions.py`

 * *Files identical despite different names*

### Comparing `drf_keycloak_auth-0.2.1/drf_keycloak_auth/settings.py` & `drf_keycloak_auth-0.2.2/drf_keycloak_auth/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 USER_SETTINGS = getattr(settings, 'DRF_KEYCLOAK_AUTH', None)
 
 # should be comma separated string
 KEYCLOAK_ROLES_TO_DJANGO_IS_STAFF = \
     os.getenv('KEYCLOAK_ROLES_TO_DJANGO_IS_STAFF')
 
 DEFAULTS = {
+    'ALLOWED_HOSTS': os.getenv('DJANGO_ALLOWED_HOSTS', '').split(' '),
+
     'KEYCLOAK_MULTI_OIDC_JSON': (
         json.loads(os.getenv('KEYCLOAK_MULTI_OIDC_JSON'))
         if os.getenv('KEYCLOAK_MULTI_OIDC_JSON')
         else None
     ),
     
     'KEYCLOAK_SERVER_URL': os.getenv('KEYCLOAK_SERVER_URL'),
@@ -42,17 +44,14 @@
 
     'KEYCLOAK_DJANGO_USER_UUID_FIELD':
         os.getenv('KEYCLOAK_DJANGO_USER_UUID_FIELD', 'pk'),
 
     'KEYCLOAK_FIELD_AS_DJANGO_USERNAME':
         os.getenv('KEYCLOAK_FIELD_AS_DJANGO_USERNAME', 'preferred_username'),
 
-    'KEYCLOAK_REALM_PREFIX_DJANGO_USERNAME':
-        os.getenv('KEYCLOAK_REALM_PREFIX_DJANGO_USERNAME', True),
-
     'KEYCLOAK_ROLES_TO_DJANGO_IS_STAFF': (
         [x.strip() for x in KEYCLOAK_ROLES_TO_DJANGO_IS_STAFF.split(',')]
         if KEYCLOAK_ROLES_TO_DJANGO_IS_STAFF
         else ['admin']  # can be list, tuple or set
     )
 }
```

### Comparing `drf_keycloak_auth-0.2.1/drf_keycloak_auth.egg-info/PKG-INFO` & `drf_keycloak_auth-0.2.2/drf_keycloak_auth.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-keycloak-auth
-Version: 0.2.1
+Version: 0.2.2
 Summary: A convenience libary for authenticating users from Keycloak access tokens
 Home-page: https://gitlab.com/ecocommons-australia/lib/drf-keycloak-auth
 Author: EcoCommons Australia
 Author-email: ecocommons@griffith.edu.au
 License: MIT
 Keywords: drf,django,rest_framework,djangorestframework,authentication,python3,keycloak
 Classifier: Programming Language :: Python :: 3
@@ -129,15 +129,15 @@
 ```
 KEYCLOAK_DJANGO_USER_UUID_FIELD = 'uuid'
 ```
 
 Voila!
 
 
-## Multi tennancy support
+## Multi tenancy support
 
 An application can be configured for multiple tenancies by using different Keycloak Realms on the same or seperate Keycloak instances by using the environment var `KEYCLOAK_MULTI_OIDC_JSON`
 
 The client OIDC adaptor json file can be downloaded from Keycloak.
 
 ```
 KEYCLOAK_MULTI_OIDC_JSON=
```

### Comparing `drf_keycloak_auth-0.2.1/setup.py` & `drf_keycloak_auth-0.2.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     ],
     python_requires='>=3',
     install_requires=[
         'djangorestframework>=3.9,<4',
         'python-keycloak>=3.3',
         'django>=3',
         'urllib3<1.27,>=1.21.1',
+        'pyjwt>=2.6',
         'pytz'
     ],
     keywords=[
         'drf',
         'django',
         'rest_framework',
         'djangorestframework',
```

