# Comparing `tmp/flask_shopify_utils-0.0.7.tar.gz` & `tmp/flask_shopify_utils-0.0.8.tar.gz`

## Comparing `flask_shopify_utils-0.0.7.tar` & `flask_shopify_utils-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    32368 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.7/src/flask_shopify_utils/__init__.py
--rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.7/src/flask_shopify_utils/model.py
--rw-r--r--   0        0        0     3634 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.7/src/flask_shopify_utils/utils.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.7/tests/conftest.py
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.7/tests/test_admin_routes.py
--rw-r--r--   0        0        0     4440 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.7/tests/test_default_routes.py
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.7/tests/test_gdpr_routes.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.7/tests/test_graphql_cli.py
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.7/tests/test_init.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.7/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.7/LICENSE
--rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.7/README.md
--rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     3639 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0    32330 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.8/src/flask_shopify_utils/__init__.py
+-rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.8/src/flask_shopify_utils/model.py
+-rw-r--r--   0        0        0     3634 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.8/src/flask_shopify_utils/utils.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.8/tests/conftest.py
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.8/tests/test_admin_routes.py
+-rw-r--r--   0        0        0     4440 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.8/tests/test_default_routes.py
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.8/tests/test_gdpr_routes.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.8/tests/test_graphql_cli.py
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.8/tests/test_init.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.8/LICENSE
+-rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.8/README.md
+-rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     3639 2020-02-02 00:00:00.000000 flask_shopify_utils-0.0.8/PKG-INFO
```

### Comparing `flask_shopify_utils-0.0.7/src/flask_shopify_utils/__init__.py` & `flask_shopify_utils-0.0.8/src/flask_shopify_utils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     make_response, url_for
 from jinja2 import TemplateNotFound
 from jwt import encode as jwt_encode, decode as jwt_decode, ExpiredSignatureError
 from cerberus.validator import Validator
 from pytz import timezone
 from flask_shopify_utils.utils import get_version, GraphQLClient
 
-__version__ = '0.0.7'
+__version__ = '0.0.8'
 
 JWT_DATA = TypeVar('JWT_DATA', dict, Response)
 current_time_func = None
 sqlalchemy_instance = None
 
 
 class ShopifyUtil:
@@ -543,39 +543,39 @@
 
     def enroll_default_route(self) -> None:
         """
         Register default Shopify routes
         """
         from flask_shopify_utils.model import Store
 
-        static_folder = path.join(path.dirname(self.config.get('ROOT_PATH')), 'dist', 'front')
+        static_folder = path.join(self.config.get('ROOT_PATH'), 'dist', 'docs')
         doc_routes = Blueprint(
             'docs_default',
             'docs_routes',
             url_prefix='/docs',
             static_folder=static_folder,
-            template_folder=static_folder
+            template_folder=static_folder,
         )
 
         @doc_routes.route('/', methods=['GET'])
         def index() -> Response:
             """
             Show the docs for default message
             """
             try:
                 return make_response(render_template('index.html'))
             except TemplateNotFound:
                 return make_response('Please contact "dev@pocketsquare.co.nz" for more information.')
 
-        static_folder = path.join(path.dirname(self.config.get('ROOT_PATH')), 'dist')
+        static_folder = path.join(self.config.get('ROOT_PATH'), 'dist', 'admin')
         default_routes = Blueprint(
             'shopify_default',
             'shopify_default_routes',
             static_folder=static_folder,
-            template_folder=static_folder
+            template_folder=static_folder,
         )
 
         # Register the `admin` route
         @default_routes.route('/', methods=['GET'], endpoint='index')
         @self.check_hmac
         def index() -> Response:
             """ Show Embedded App or Docs page """
@@ -592,15 +592,15 @@
                     resp = self.proxy_response(404, msg)
                     resp.status_code = 404
                     return resp
                 g.store_id = store.id
             # Render the Embedded App Index Page
             try:
                 code = render_template(
-                    path.join('admin', 'index.html'),
+                    'index.html',
                     apiKey=self.config.get('SHOPIFY_API_KEY'),
                     host=g.host,
                     jwtToken=self.create_admin_jwt_token()
                 )
             except TemplateNotFound:
                 return self.proxy_response(0, 'Oops... The `index.html` is gone!')
             return make_response(code)
```

### Comparing `flask_shopify_utils-0.0.7/src/flask_shopify_utils/model.py` & `flask_shopify_utils-0.0.8/src/flask_shopify_utils/model.py`

 * *Files identical despite different names*

### Comparing `flask_shopify_utils-0.0.7/src/flask_shopify_utils/utils.py` & `flask_shopify_utils-0.0.8/src/flask_shopify_utils/utils.py`

 * *Files identical despite different names*

### Comparing `flask_shopify_utils-0.0.7/tests/conftest.py` & `flask_shopify_utils-0.0.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `flask_shopify_utils-0.0.7/tests/test_admin_routes.py` & `flask_shopify_utils-0.0.8/tests/test_admin_routes.py`

 * *Files identical despite different names*

### Comparing `flask_shopify_utils-0.0.7/tests/test_default_routes.py` & `flask_shopify_utils-0.0.8/tests/test_default_routes.py`

 * *Files identical despite different names*

### Comparing `flask_shopify_utils-0.0.7/tests/test_gdpr_routes.py` & `flask_shopify_utils-0.0.8/tests/test_gdpr_routes.py`

 * *Files identical despite different names*

### Comparing `flask_shopify_utils-0.0.7/LICENSE` & `flask_shopify_utils-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_shopify_utils-0.0.7/README.md` & `flask_shopify_utils-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `flask_shopify_utils-0.0.7/pyproject.toml` & `flask_shopify_utils-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `flask_shopify_utils-0.0.7/PKG-INFO` & `flask_shopify_utils-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-shopify-utils
-Version: 0.0.7
+Version: 0.0.8
 Summary: A Flask extension for Shopify app development
 Project-URL: Homepage, https://github.com/leocxy/flask-shopify-utils
 Project-URL: Bug Tracker, https://github.com/leocxy/flask-shopify-utils/issues
 Author: Leo Chen
 Author-email: leo.cxy88@gmail.com
 Maintainer: Leo Chen
 Maintainer-email: leo.cxy88@gmail.com
```

