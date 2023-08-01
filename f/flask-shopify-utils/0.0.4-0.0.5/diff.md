# Comparing `tmp/flask_shopify_utils-0.0.4.tar.gz` & `tmp/flask_shopify_utils-0.0.5.tar.gz`

## Comparing `flask_shopify_utils-0.0.4.tar` & `flask_shopify_utils-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    32372 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.4/src/flask_shopify_utils/__init__.py
--rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.4/src/flask_shopify_utils/model.py
--rw-r--r--   0        0        0     3634 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.4/src/flask_shopify_utils/utils.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.4/tests/conftest.py
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.4/tests/test_admin_routes.py
--rw-r--r--   0        0        0     4440 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.4/tests/test_default_routes.py
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.4/tests/test_gdpr_routes.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.4/tests/test_graphql_cli.py
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.4/tests/test_init.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.4/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.4/LICENSE
--rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.4/README.md
--rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     3639 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    32366 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.5/src/flask_shopify_utils/__init__.py
+-rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.5/src/flask_shopify_utils/model.py
+-rw-r--r--   0        0        0     3634 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.5/src/flask_shopify_utils/utils.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.5/tests/conftest.py
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.5/tests/test_admin_routes.py
+-rw-r--r--   0        0        0     4440 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.5/tests/test_default_routes.py
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.5/tests/test_gdpr_routes.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.5/tests/test_graphql_cli.py
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.5/tests/test_init.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.5/LICENSE
+-rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.5/README.md
+-rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3639 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.5/PKG-INFO
```

### Comparing `flask_shopify_utils-0.0.4/src/flask_shopify_utils/__init__.py` & `flask_shopify_utils-0.0.5/src/flask_shopify_utils/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     make_response, url_for
 from jinja2 import TemplateNotFound
 from jwt import encode as jwt_encode, decode as jwt_decode, ExpiredSignatureError
 from cerberus.validator import Validator
 from pytz import timezone
 from flask_shopify_utils.utils import get_version, GraphQLClient
 
-__version__ = '0.0.4'
+__version__ = '0.0.5'
 
 JWT_DATA = TypeVar('JWT_DATA', dict, Response)
 current_time_func = None
 sqlalchemy_instance = None
 
 
 class ShopifyUtil:
@@ -620,30 +620,30 @@
                 resp.status_code = 500
                 return resp
             data = res.json()
             token = data.get('access_token', '')
             # Query the shop domain and save the data
             client = GraphQLClient(g.store_key, token)
             raw_query = '{ shop { name, url } appInstallation { accessScopes { handle }} }'
-            res = client.client(raw_query)
+            res = client.client(raw_query)['data']
             shop = res.get('shop', False)
             if not shop:
                 resp = self.proxy_response(500, 'Something went wrong while fetching shop data!')
                 resp.status_code = 500
                 return resp
             cond = dict(key=g.store_key)
             record = Store.create_or_update(cond, domain=shop['url'].split('/')[-1], token=token, **cond)
             scopes = res.get('appInstallation', None)
             if not scopes:
                 resp = self.proxy_response(500, 'Something went wrong while fetching installation data!')
                 resp.status_code = 500
                 return resp
             record.scopes = ','.join(list(map(lambda x: x['handle'], scopes['accessScopes'])))
             # Register GDPR mandatory webhook @todo
-            return redirect('https://{}.myshopify.com/admin/app/{}'.format(
+            return redirect('https://{}/admin/app/{}'.format(
                 g.store_key,
                 self.config.get('SHOPIFY_API_KEY'))
             )
 
         # Register the `install` route
         @default_routes.route('/install', methods=['GET'], endpoint='install')
         def install():
```

### Comparing `flask_shopify_utils-0.0.4/src/flask_shopify_utils/model.py` & `flask_shopify_utils-0.0.5/src/flask_shopify_utils/model.py`

 * *Files identical despite different names*

### Comparing `flask_shopify_utils-0.0.4/src/flask_shopify_utils/utils.py` & `flask_shopify_utils-0.0.5/src/flask_shopify_utils/utils.py`

 * *Files identical despite different names*

### Comparing `flask_shopify_utils-0.0.4/tests/conftest.py` & `flask_shopify_utils-0.0.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `flask_shopify_utils-0.0.4/tests/test_admin_routes.py` & `flask_shopify_utils-0.0.5/tests/test_admin_routes.py`

 * *Files identical despite different names*

### Comparing `flask_shopify_utils-0.0.4/tests/test_default_routes.py` & `flask_shopify_utils-0.0.5/tests/test_default_routes.py`

 * *Files identical despite different names*

### Comparing `flask_shopify_utils-0.0.4/tests/test_gdpr_routes.py` & `flask_shopify_utils-0.0.5/tests/test_gdpr_routes.py`

 * *Files identical despite different names*

### Comparing `flask_shopify_utils-0.0.4/LICENSE` & `flask_shopify_utils-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_shopify_utils-0.0.4/README.md` & `flask_shopify_utils-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `flask_shopify_utils-0.0.4/pyproject.toml` & `flask_shopify_utils-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `flask_shopify_utils-0.0.4/PKG-INFO` & `flask_shopify_utils-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-shopify-utils
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Flask extension for Shopify app development
 Project-URL: Homepage, https://github.com/leocxy/flask-shopify-utils
 Project-URL: Bug Tracker, https://github.com/leocxy/flask-shopify-utils/issues
 Author: Leo Chen
 Author-email: leo.cxy88@gmail.com
 Maintainer: Leo Chen
 Maintainer-email: leo.cxy88@gmail.com
```

