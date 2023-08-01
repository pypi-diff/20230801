# Comparing `tmp/flask_shopify_utils-0.0.6.tar.gz` & `tmp/flask_shopify_utils-0.0.7.tar.gz`

## Comparing `flask_shopify_utils-0.0.6.tar` & `flask_shopify_utils-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    32369 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.6/src/flask_shopify_utils/__init__.py
--rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.6/src/flask_shopify_utils/model.py
--rw-r--r--   0        0        0     3634 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.6/src/flask_shopify_utils/utils.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.6/tests/conftest.py
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.6/tests/test_admin_routes.py
--rw-r--r--   0        0        0     4440 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.6/tests/test_default_routes.py
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.6/tests/test_gdpr_routes.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.6/tests/test_graphql_cli.py
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.6/tests/test_init.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.6/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.6/LICENSE
--rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.6/README.md
--rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     3639 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0    32368 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.7/src/flask_shopify_utils/__init__.py
+-rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.7/src/flask_shopify_utils/model.py
+-rw-r--r--   0        0        0     3634 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.7/src/flask_shopify_utils/utils.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.7/tests/conftest.py
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.7/tests/test_admin_routes.py
+-rw-r--r--   0        0        0     4440 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.7/tests/test_default_routes.py
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.7/tests/test_gdpr_routes.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.7/tests/test_graphql_cli.py
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.7/tests/test_init.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.7/LICENSE
+-rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.7/README.md
+-rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     3639 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.7/PKG-INFO
```

### Comparing `flask_shopify_utils-0.0.6/src/flask_shopify_utils/__init__.py` & `flask_shopify_utils-0.0.7/src/flask_shopify_utils/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     make_response, url_for
 from jinja2 import TemplateNotFound
 from jwt import encode as jwt_encode, decode as jwt_decode, ExpiredSignatureError
 from cerberus.validator import Validator
 from pytz import timezone
 from flask_shopify_utils.utils import get_version, GraphQLClient
 
-__version__ = '0.0.6'
+__version__ = '0.0.7'
 
 JWT_DATA = TypeVar('JWT_DATA', dict, Response)
 current_time_func = None
 sqlalchemy_instance = None
 
 
 class ShopifyUtil:
@@ -225,15 +225,15 @@
         def decorator(*args, **kwargs):
             # check timestamp
             timestamp1 = int(request.args.get('timestamp', '0'))
             timestamp2 = int(time()) - 86400
             if timestamp1 < timestamp2:
                 return jsonify(dict(message='The request has expired', status=401))
             params = request.args
-            if len([x for x in params.keys() if x in ['shop', 'hmac', 'host', 'timestamp', 'session']]) >= 4:
+            if len([x for x in params.keys() if x in ['shop', 'hmac', 'host', 'timestamp', 'session']]) < 4:
                 # Redirect to the Docs page
                 return redirect(url_for('docs_default.index'))
             # Check Hmac
             if not compare_digest(
                     self.validate_hmac(params),
                     request.args.get('hmac', '')
             ):
```

### Comparing `flask_shopify_utils-0.0.6/src/flask_shopify_utils/model.py` & `flask_shopify_utils-0.0.7/src/flask_shopify_utils/model.py`

 * *Files identical despite different names*

### Comparing `flask_shopify_utils-0.0.6/src/flask_shopify_utils/utils.py` & `flask_shopify_utils-0.0.7/src/flask_shopify_utils/utils.py`

 * *Files identical despite different names*

### Comparing `flask_shopify_utils-0.0.6/tests/conftest.py` & `flask_shopify_utils-0.0.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `flask_shopify_utils-0.0.6/tests/test_admin_routes.py` & `flask_shopify_utils-0.0.7/tests/test_admin_routes.py`

 * *Files identical despite different names*

### Comparing `flask_shopify_utils-0.0.6/tests/test_default_routes.py` & `flask_shopify_utils-0.0.7/tests/test_default_routes.py`

 * *Files identical despite different names*

### Comparing `flask_shopify_utils-0.0.6/tests/test_gdpr_routes.py` & `flask_shopify_utils-0.0.7/tests/test_gdpr_routes.py`

 * *Files identical despite different names*

### Comparing `flask_shopify_utils-0.0.6/LICENSE` & `flask_shopify_utils-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_shopify_utils-0.0.6/README.md` & `flask_shopify_utils-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `flask_shopify_utils-0.0.6/pyproject.toml` & `flask_shopify_utils-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `flask_shopify_utils-0.0.6/PKG-INFO` & `flask_shopify_utils-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-shopify-utils
-Version: 0.0.6
+Version: 0.0.7
 Summary: A Flask extension for Shopify app development
 Project-URL: Homepage, https://github.com/leocxy/flask-shopify-utils
 Project-URL: Bug Tracker, https://github.com/leocxy/flask-shopify-utils/issues
 Author: Leo Chen
 Author-email: leo.cxy88@gmail.com
 Maintainer: Leo Chen
 Maintainer-email: leo.cxy88@gmail.com
```

