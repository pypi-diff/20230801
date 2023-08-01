# Comparing `tmp/trex-apis-1.0.4.tar.gz` & `tmp/trex-apis-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trex-apis-1.0.4.tar", last modified: Mon May 15 06:06:52 2023, max compression
+gzip compressed data, was "trex-apis-1.0.6.tar", last modified: Tue Aug  1 02:33:34 2023, max compression
```

## Comparing `trex-apis-1.0.4.tar` & `trex-apis-1.0.6.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-15 06:06:52.119286 trex-apis-1.0.4/
--rw-r--r--   0 jacklok    (501) staff       (20)      447 2023-05-15 06:06:52.119410 trex-apis-1.0.4/PKG-INFO
--rw-r--r--   0 jacklok    (501) staff       (20)       25 2021-06-30 02:28:26.000000 trex-apis-1.0.4/README.md
--rw-r--r--   0 jacklok    (501) staff       (20)       75 2023-05-15 06:06:52.119850 trex-apis-1.0.4/setup.cfg
--rw-r--r--   0 jacklok    (501) staff       (20)      713 2023-05-15 06:06:46.000000 trex-apis-1.0.4/setup.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-15 06:06:52.096436 trex-apis-1.0.4/trex_apis.egg-info/
--rw-r--r--   0 jacklok    (501) staff       (20)      447 2023-05-15 06:06:51.000000 trex-apis-1.0.4/trex_apis.egg-info/PKG-INFO
--rw-r--r--   0 jacklok    (501) staff       (20)     1328 2023-05-15 06:06:51.000000 trex-apis-1.0.4/trex_apis.egg-info/SOURCES.txt
--rw-r--r--   0 jacklok    (501) staff       (20)        1 2023-05-15 06:06:51.000000 trex-apis-1.0.4/trex_apis.egg-info/dependency_links.txt
--rw-r--r--   0 jacklok    (501) staff       (20)       23 2023-05-15 06:06:51.000000 trex-apis-1.0.4/trex_apis.egg-info/requires.txt
--rw-r--r--   0 jacklok    (501) staff       (20)        8 2023-05-15 06:06:51.000000 trex-apis-1.0.4/trex_apis.egg-info/top_level.txt
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-15 06:06:52.096992 trex-apis-1.0.4/trexapi/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-06-30 02:30:07.000000 trex-apis-1.0.4/trexapi/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)      837 2023-04-19 06:13:09.000000 trex-apis-1.0.4/trexapi/conf.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-15 06:06:52.111374 trex-apis-1.0.4/trexapi/controllers/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-06-30 02:45:28.000000 trex-apis-1.0.4/trexapi/controllers/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)    14569 2023-05-15 02:45:00.000000 trex-apis-1.0.4/trexapi/controllers/api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     2259 2022-11-14 14:26:16.000000 trex-apis-1.0.4/trexapi/controllers/app_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    35947 2023-05-05 09:27:49.000000 trex-apis-1.0.4/trexapi/controllers/customer_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     6945 2023-04-13 05:36:42.000000 trex-apis-1.0.4/trexapi/controllers/customer_membership_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     4750 2023-01-30 07:03:11.000000 trex-apis-1.0.4/trexapi/controllers/customer_reward_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    13204 2023-05-15 02:06:38.000000 trex-apis-1.0.4/trexapi/controllers/loyalty_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1214 2023-05-07 13:49:51.000000 trex-apis-1.0.4/trexapi/controllers/lucky_draw_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    11170 2023-05-05 09:32:39.000000 trex-apis-1.0.4/trexapi/controllers/outlet_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1430 2022-09-26 04:18:01.000000 trex-apis-1.0.4/trexapi/controllers/payment_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    22728 2023-01-13 04:39:15.000000 trex-apis-1.0.4/trexapi/controllers/pos_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    27329 2023-04-18 07:01:48.000000 trex-apis-1.0.4/trexapi/controllers/reward_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     7315 2023-04-20 09:46:08.000000 trex-apis-1.0.4/trexapi/controllers/sales_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)      998 2023-04-18 06:08:18.000000 trex-apis-1.0.4/trexapi/controllers/transaction_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    43378 2023-05-12 14:04:03.000000 trex-apis-1.0.4/trexapi/controllers/user_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     2980 2023-01-30 02:56:35.000000 trex-apis-1.0.4/trexapi/controllers/user_reward_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    15185 2023-04-07 15:27:24.000000 trex-apis-1.0.4/trexapi/controllers/voucher_api_routes.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-15 06:06:52.112479 trex-apis-1.0.4/trexapi/decorators/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-01 08:42:13.000000 trex-apis-1.0.4/trexapi/decorators/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     4734 2023-05-05 09:06:37.000000 trex-apis-1.0.4/trexapi/decorators/api_decorators.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-15 06:06:52.115279 trex-apis-1.0.4/trexapi/forms/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-12 06:42:53.000000 trex-apis-1.0.4/trexapi/forms/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     7419 2023-02-08 10:14:32.000000 trex-apis-1.0.4/trexapi/forms/customer_api_forms.py
--rw-r--r--   0 jacklok    (501) staff       (20)     7285 2023-04-18 02:42:03.000000 trex-apis-1.0.4/trexapi/forms/reward_api_forms.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1547 2023-04-18 02:41:54.000000 trex-apis-1.0.4/trexapi/forms/sales_api_forms.py
--rw-r--r--   0 jacklok    (501) staff       (20)     2505 2023-05-09 02:01:04.000000 trex-apis-1.0.4/trexapi/forms/user_api_forms.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-15 06:06:52.116165 trex-apis-1.0.4/trexapi/libs/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-05 10:17:19.000000 trex-apis-1.0.4/trexapi/libs/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1143 2021-07-05 10:57:23.000000 trex-apis-1.0.4/trexapi/libs/flask_auth_wrapper.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-15 06:06:52.117740 trex-apis-1.0.4/trexapi/utils/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-08 10:01:06.000000 trex-apis-1.0.4/trexapi/utils/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1347 2022-12-20 01:23:01.000000 trex-apis-1.0.4/trexapi/utils/api_helpers.py
--rw-r--r--   0 jacklok    (501) staff       (20)    76256 2023-04-24 10:05:07.000000 trex-apis-1.0.4/trexapi/utils/reward_transaction_helper.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-01 02:33:34.858237 trex-apis-1.0.6/
+-rw-r--r--   0 jacklok    (501) staff       (20)      447 2023-08-01 02:33:34.858375 trex-apis-1.0.6/PKG-INFO
+-rw-r--r--   0 jacklok    (501) staff       (20)       25 2021-06-30 02:28:26.000000 trex-apis-1.0.6/README.md
+-rw-r--r--   0 jacklok    (501) staff       (20)       75 2023-08-01 02:33:34.858830 trex-apis-1.0.6/setup.cfg
+-rw-r--r--   0 jacklok    (501) staff       (20)      713 2023-08-01 02:30:49.000000 trex-apis-1.0.6/setup.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-01 02:33:34.819427 trex-apis-1.0.6/trex_apis.egg-info/
+-rw-r--r--   0 jacklok    (501) staff       (20)      447 2023-08-01 02:33:34.000000 trex-apis-1.0.6/trex_apis.egg-info/PKG-INFO
+-rw-r--r--   0 jacklok    (501) staff       (20)     1371 2023-08-01 02:33:34.000000 trex-apis-1.0.6/trex_apis.egg-info/SOURCES.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)        1 2023-08-01 02:33:34.000000 trex-apis-1.0.6/trex_apis.egg-info/dependency_links.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)       23 2023-08-01 02:33:34.000000 trex-apis-1.0.6/trex_apis.egg-info/requires.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)        8 2023-08-01 02:33:34.000000 trex-apis-1.0.6/trex_apis.egg-info/top_level.txt
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-01 02:33:34.819954 trex-apis-1.0.6/trexapi/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-06-30 02:30:07.000000 trex-apis-1.0.6/trexapi/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      937 2023-07-20 09:41:39.000000 trex-apis-1.0.6/trexapi/conf.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-01 02:33:34.845328 trex-apis-1.0.6/trexapi/controllers/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-06-30 02:45:28.000000 trex-apis-1.0.6/trexapi/controllers/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     4523 2023-05-23 05:00:09.000000 trex-apis-1.0.6/trexapi/controllers/api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     3850 2023-05-25 08:10:20.000000 trex-apis-1.0.6/trexapi/controllers/app_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    35947 2023-05-18 03:00:00.000000 trex-apis-1.0.6/trexapi/controllers/customer_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     6945 2023-04-13 05:36:42.000000 trex-apis-1.0.6/trexapi/controllers/customer_membership_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     4750 2023-01-30 07:03:11.000000 trex-apis-1.0.6/trexapi/controllers/customer_reward_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    13204 2023-05-15 02:06:38.000000 trex-apis-1.0.6/trexapi/controllers/loyalty_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    13485 2023-07-12 07:15:15.000000 trex-apis-1.0.6/trexapi/controllers/lucky_draw_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    15269 2023-07-10 09:47:14.000000 trex-apis-1.0.6/trexapi/controllers/merchant_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    11170 2023-05-16 03:00:59.000000 trex-apis-1.0.6/trexapi/controllers/outlet_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1430 2022-09-26 04:18:01.000000 trex-apis-1.0.6/trexapi/controllers/payment_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    24944 2023-05-23 09:32:47.000000 trex-apis-1.0.6/trexapi/controllers/pos_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    27329 2023-04-18 07:01:48.000000 trex-apis-1.0.6/trexapi/controllers/reward_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    12777 2023-07-25 03:49:49.000000 trex-apis-1.0.6/trexapi/controllers/sales_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      998 2023-04-18 06:08:18.000000 trex-apis-1.0.6/trexapi/controllers/transaction_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    51442 2023-07-31 15:36:43.000000 trex-apis-1.0.6/trexapi/controllers/user_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     2980 2023-01-30 02:56:35.000000 trex-apis-1.0.6/trexapi/controllers/user_reward_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    16314 2023-07-05 09:44:39.000000 trex-apis-1.0.6/trexapi/controllers/voucher_api_routes.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-01 02:33:34.847640 trex-apis-1.0.6/trexapi/decorators/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-01 08:42:13.000000 trex-apis-1.0.6/trexapi/decorators/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     5778 2023-06-30 15:57:30.000000 trex-apis-1.0.6/trexapi/decorators/api_decorators.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-01 02:33:34.852726 trex-apis-1.0.6/trexapi/forms/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-12 06:42:53.000000 trex-apis-1.0.6/trexapi/forms/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     7419 2023-02-08 10:14:32.000000 trex-apis-1.0.6/trexapi/forms/customer_api_forms.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     7285 2023-04-18 02:42:03.000000 trex-apis-1.0.6/trexapi/forms/reward_api_forms.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1547 2023-04-18 02:41:54.000000 trex-apis-1.0.6/trexapi/forms/sales_api_forms.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     3922 2023-05-29 03:02:06.000000 trex-apis-1.0.6/trexapi/forms/user_api_forms.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-01 02:33:34.854114 trex-apis-1.0.6/trexapi/libs/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-05 10:17:19.000000 trex-apis-1.0.6/trexapi/libs/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1143 2021-07-05 10:57:23.000000 trex-apis-1.0.6/trexapi/libs/flask_auth_wrapper.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-01 02:33:34.856203 trex-apis-1.0.6/trexapi/utils/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-08 10:01:06.000000 trex-apis-1.0.6/trexapi/utils/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1347 2022-12-20 01:23:01.000000 trex-apis-1.0.6/trexapi/utils/api_helpers.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    78420 2023-06-30 14:45:12.000000 trex-apis-1.0.6/trexapi/utils/reward_transaction_helper.py
```

### Comparing `trex-apis-1.0.4/setup.py` & `trex-apis-1.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setuptools.setup(
      name='trex-apis',  
-     version='1.0.4',
+     version='1.0.6',
      author="Jack Lok",
      author_email="sglok77@gmail.com",
      description="TRex APIs package",
      long_description=long_description,
      long_description_content_type="text/markdown",
      url="https://bitbucket.org/lokjac/trex-apis",
      packages=setuptools.find_packages(),
```

### Comparing `trex-apis-1.0.4/trex_apis.egg-info/SOURCES.txt` & `trex-apis-1.0.6/trex_apis.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 trexapi/controllers/api_routes.py
 trexapi/controllers/app_api_routes.py
 trexapi/controllers/customer_api_routes.py
 trexapi/controllers/customer_membership_api_routes.py
 trexapi/controllers/customer_reward_api_routes.py
 trexapi/controllers/loyalty_api_routes.py
 trexapi/controllers/lucky_draw_api_routes.py
+trexapi/controllers/merchant_api_routes.py
 trexapi/controllers/outlet_api_routes.py
 trexapi/controllers/payment_api_routes.py
 trexapi/controllers/pos_api_routes.py
 trexapi/controllers/reward_api_routes.py
 trexapi/controllers/sales_api_routes.py
 trexapi/controllers/transaction_api_routes.py
 trexapi/controllers/user_api_routes.py
```

### Comparing `trex-apis-1.0.4/trexapi/conf.py` & `trex-apis-1.0.6/trexapi/conf.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,7 +11,9 @@
 UPDATED_DATE                                                    = '5 July 2021'
 
 API_TOKEN_EXPIRY_LENGTH_IN_MINUTE                               = os.environ.get('API_TOKEN_EXPIRY_LENGTH_IN_MINUTE') 
 
 API_ERR_CODE_INVALID_ACTIVATION_CODE                            = 'invalid.activation.code';
 
 EARN_INSTANT_REWARD_URL                                         = os.environ.get('EARN_INSTANT_REWARD_URL')
+
+LUCKY_DRAW_URL                                                  = os.environ.get('LUCKY_DRAW_URL')
```

### Comparing `trex-apis-1.0.4/trexapi/controllers/api_routes.py` & `trex-apis-1.0.6/trexapi/controllers/merchant_api_routes.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,158 +12,153 @@
 from trexapi import conf
 from flask_restful import Api
 from trexmodel.utils.model.model_util import create_db_client
 from trexmodel.models.datastore.merchant_models import MerchantUser,\
     MerchantAcct
 import hashlib
 from random import random
-from trexlib.utils.string_util import random_string, is_not_empty
+from trexlib.utils.string_util import is_not_empty
 from flask.json import jsonify
-from datetime import datetime, timedelta
 from trexapi import conf as api_conf
-from trexlib.utils.crypto_util import encrypt_json
 from trexapi.decorators.api_decorators import auth_token_required
-from trexapi.libs.flask_auth_wrapper import HTTPBasicAuthWrapper
 from trexmodel.models.datastore.loyalty_models import LoyaltyDeviceSetting
 from trexmodel.models.datastore.pos_models import POSSetting
+from trexapi.controllers.api_routes import APIBaseResource
+from trexmodel.models import merchant_helpers
+from trexadmin.libs.http import create_rest_message, StatusCode
+from trexmodel.models.datastore.customer_models import Customer
 
 #logger = logging.getLogger('api')
 logger = logging.getLogger('debug')
 
 auth = HTTPBasicAuth()
 #auth = HTTPBasicAuthWrapper()
 
 
-api_bp = Blueprint('api_base_bp', __name__,
-                                 template_folder='templates',
-                                 static_folder='static',
-                                 url_prefix='/api/v1')
-
 merchant_api_bp = Blueprint('merchant_api_bp', __name__,
                                  template_folder='templates',
                                  static_folder='static',
                                  url_prefix='/api/v1/merchant')
 
-api = Api(api_bp)
-
 merchant_api = Api(merchant_api_bp)
 
 
 
+@merchant_api_bp.route('/ping', methods=['GET'])
+def ping():
+    return 'Pong', 200
+
 @auth.verify_password
 def verify_user_auth(username, password):
     if not (username and password):
         return False
     
     db_client   = create_db_client(caller_info="verify_user_auth")
     valid_auth  = False
     
+    logger.debug('username=%s', username)
+    logger.debug('password=%s', password)
+    
     with db_client.context():
         merchant_user = MerchantUser.get_by_username(username)
         
+        logger.debug('merchant_user=%s', merchant_user)
+        
         if merchant_user:
             
             md5_hashed_password = hashlib.md5(password.encode('utf-8')).hexdigest()
             
-            logger.debug('verify_user_auth: username=%s', username)
-            logger.debug('verify_user_auth: password=%s', password)
             logger.debug('verify_user_auth: md5_hashed_password=%s', md5_hashed_password)
             
             if merchant_user.is_valid_password(md5_hashed_password):
                 valid_auth = True
             else:
                 logger.warn('Invalid merchant password')
         else:
             logger.warn('Invalid merchant username=%s', username)    
         
     return valid_auth
 
-def __generate_random():
-    return hashlib.md5(str(random_string(6)).encode('utf-8')).hexdigest()
-
-def default_generate_nonce():
-    session["auth_nonce"] = __generate_random()
-    return session["auth_nonce"]
- 
-def default_verify_nonce(nonce):
-    return nonce == session.get("auth_nonce")
-
-def default_generate_opaque():
-    session["auth_opaque"] = __generate_random()
-    return session["auth_opaque"]
-
-def default_verify_opaque(opaque):
-    return opaque == session.get("auth_opaque")
-    
-class APIBaseResource(Resource):
-    @property
-    def realm(self):
-        return 'base'
-    
-    def generate_ha1(self, username, password):
-        a1 = username + ":" + self.realm + ":" + password
-        a1 = a1.encode('utf-8')
-        return hashlib.md5(a1).hexdigest()
-    
-    def generate_token(self, acct_id, username):
-        expiry_datetime = datetime.now() + timedelta(minutes = int(api_conf.API_TOKEN_EXPIRY_LENGTH_IN_MINUTE))
-        
-        logger.debug('expiry_datetime=%s', expiry_datetime)
-        
-        token_content =  {
-                            'acct_id'           : acct_id,
-                            'username'          : username,
-                            'expiry_datetime'   : expiry_datetime.strftime('%d-%m-%Y %H:%M:%S'),
-                            }
-        
-        logger.debug('token_content=%s', token_content)
-        
-        return (expiry_datetime, encrypt_json(token_content))
-    
-    
-class APIVersionResource(APIBaseResource):
-    
-    @auth.login_required
-    def get(self):
-        output_json =  {
-                        'version'   :   conf.VERSION,
-                        'username'  :   auth.current_user()
-                        }
-        
-        return output_json
+@merchant_api_bp.route('/<merchant_acct_code>/details', methods=['GET'])
+def read_merchant_acct(merchant_acct_code):
     
-class APIResource(APIBaseResource):
+    merchant_acct           = None
+    if is_not_empty(merchant_acct_code):
+        db_client = create_db_client(caller_info="read_merchant_acct")
+        with db_client.context():
+            merchant_acct = MerchantAcct.get_by_account_code(merchant_acct_code)
+            logger.debug('website=%s', merchant_acct.website)
+            merchant_info = merchant_helpers.construct_merchant_acct_info(merchant_acct) 
+            
+        return create_rest_message(status_code=StatusCode.OK,
+                                               **merchant_info
+                                               )
+    else:
+        return create_rest_message("Missing merchant account key", status_code=StatusCode.BAD_REQUEST)
+
+@merchant_api_bp.route('/<merchant_key>/customer-details/reference-code/<reference_code>', methods=['GET'])
+def read_merchant_customer_details(merchant_key, reference_code):
+    
+    merchant_acct           = None
+    customer_details_dict   = {} 
+    
+    if is_not_empty(merchant_key) and is_not_empty(reference_code):
+        db_client = create_db_client(caller_info="read_merchant_customer_details")
+        with db_client.context():
+            merchant_acct = MerchantAcct.fetch(merchant_key)
+            customer = Customer.get_by_reference_code(reference_code, merchant_acct) 
+        
+            if customer:
+            
+                user_details = customer.registered_user_acct
+                customer_details_dict = customer.to_dict(date_format="%d-%m-%Y", datetime_format="%d-%m-%Y %H:%M:%S")
+                customer_details_dict['customer_key']               = customer.key_in_str
+                customer_details_dict['is_email_verified']          = user_details.is_email_verified
+                customer_details_dict['is_mobile_phone_verified']   = user_details.is_mobile_phone_verified
+                '''
+                if 'entitled_voucher_summary' in customer_details_dict:
+                    customer_details_dict['voucher_summary']            = customer.entitled_voucher_summary
+                    del customer_details_dict['entitled_voucher_summary']
+                '''
+        return jsonify(customer_details_dict)
+            
     
-    def get(self):
-        return conf.VERSION    
+    else:
+        return create_rest_message("Missing merchant account key or user reference code", status_code=StatusCode.BAD_REQUEST)
+
 
 class AccountActivatedAPIResource(APIBaseResource):  
     
     @auth.login_required
     def post(self):
         username    = auth.current_user()
         
         acct_id     = request.headers.get('x-acct-id')
         api_key     = request.headers.get('x-api-key')
         outlet_key  = request.headers.get('x-outlet-key')
         
+        logger.debug('username=%s', username)
         logger.debug('acct_id=%s', acct_id)    
         logger.debug('api_key=%s', api_key)
         logger.debug('outlet_key=%s', outlet_key)
         
         is_valid            = False
         is_authorized       = False
         output_json = {}
         
         if is_not_empty(acct_id) and is_not_empty(api_key):
             db_client = create_db_client(caller_info="AccountActivatedAPIResource.post")
             with db_client.context():
                 merchant_acct = MerchantAcct.fetch(acct_id)
-            
+                
+                #logger.debug('merchant_acct=%s', merchant_acct)
+                
                 if merchant_acct:
+                    logger.debug('merchant_acct api key=%s', merchant_acct.api_key)
+                    
                     if api_key == merchant_acct.api_key:
                         merchant_user               = MerchantUser.get_by_username(username)
                         
                         is_authorized = self.is_outlet_authorized(merchant_user, outlet_key)
                         if is_authorized:
                             (expiry_datetime, token)    = self.generate_token(acct_id, username)
                             logger.debug('outlet is_authorized=%s', is_authorized)
@@ -260,16 +255,18 @@
         abort(400, msg=["Failed to authenticate"])
         
     
     def is_outlet_authorized(self, merchant_user, outlet_key):
         return True    
 
 class ProgramDeviceAuthenticate(AccountActivatedAPIResource):
+    
     def is_outlet_authorized(self, merchant_user, outlet_key):
         if merchant_user.is_admin:
+            logger.debug('it is merchant admin user, thus it is authorized for all outlet')
             return True
         else:
             data_in_json        = request.get_json()
             activation_code     = data_in_json.get('activation_code')
             device_setting      = LoyaltyDeviceSetting.get_by_activation_code(activation_code)
             assigned_outlet_key = device_setting.assigned_outlet_key
             
@@ -328,19 +325,15 @@
 class CheckAuthTokenResource(SecureAPIResource):
     
     @auth_token_required
     def get(self):
         return 'Ping'             
     
      
-api.add_resource(APIResource,                   '/')
-api.add_resource(APIVersionResource,            '/version')
-api.add_resource(CheckAuthTokenResource,        '/auth-check')
-
 merchant_api.add_resource(AuthenticateAPIResource,       '/auth')
-merchant_api.add_resource(ProgramDeviceAuthenticate,       '/program-auth')
-merchant_api.add_resource(POSDeviceAuthenticate,       '/pos-auth')      
+merchant_api.add_resource(ProgramDeviceAuthenticate,     '/program-auth')
+merchant_api.add_resource(POSDeviceAuthenticate,         '/pos-auth')
```

### Comparing `trex-apis-1.0.4/trexapi/controllers/customer_api_routes.py` & `trex-apis-1.0.6/trexapi/controllers/customer_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.4/trexapi/controllers/customer_membership_api_routes.py` & `trex-apis-1.0.6/trexapi/controllers/customer_membership_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.4/trexapi/controllers/customer_reward_api_routes.py` & `trex-apis-1.0.6/trexapi/controllers/customer_reward_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.4/trexapi/controllers/loyalty_api_routes.py` & `trex-apis-1.0.6/trexapi/controllers/loyalty_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.4/trexapi/controllers/outlet_api_routes.py` & `trex-apis-1.0.6/trexapi/controllers/outlet_api_routes.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 outlet_api_bp = Blueprint('outlet_api_bp', __name__,
                                  template_folder='templates',
                                  static_folder='static',
                                  url_prefix='/api/v1/outlets')
 
 logger = logging.getLogger('debug')
 
-@outlet_api_bp.route('/details/<outlet_key>', methods=['GET'])
+@outlet_api_bp.route('/<outlet_key>/details', methods=['GET'])
 def read_outlet(outlet_key):
     
     outlet_details          = None
     merchant_acct           = None
     catalogue_details       = None
     outlet_setting_in_json  = {}   
     output_json             = {
```

### Comparing `trex-apis-1.0.4/trexapi/controllers/payment_api_routes.py` & `trex-apis-1.0.6/trexapi/controllers/payment_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.4/trexapi/controllers/pos_api_routes.py` & `trex-apis-1.0.6/trexapi/controllers/pos_api_routes.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,30 +46,67 @@
             else:
                 return create_rest_message('The code have been used to activate before', status_code=StatusCode.BAD_REQUEST)
         else:
             return create_rest_message('Invalid activate code', status_code=StatusCode.BAD_REQUEST)
     else:
         return create_rest_message('Activation code is required', status_code=StatusCode.BAD_REQUEST)
 
+@pos_api_bp.route('/read-settings/activation-code/<activation_code>', methods=['POST'])
+def read_device_setting(activation_code):
+    
+    logger.info('activation_code=%s', activation_code)
+    device_id       = request.args.get('device_id') or request.form.get('device_id') or request.json.get('device_id')
+    
+    if is_not_empty(activation_code):
+        db_client = create_db_client(caller_info="read_device_setting")
+        with db_client.context():
+            device_setting = POSSetting.get_by_activation_code(activation_code)
+        
+        if device_setting:
+            logger.info('Found device setting');
+            if device_setting.activated==False:
+            #if True:
+                logger.info('device activation code is valid');
+                device_setting_details = None
+                with db_client.context():
+                    device_setting_details                              = merchant_helpers.construct_setting_by_outlet(device_setting.assigned_outlet_entity, device_setting=device_setting) 
+                    device_setting_details['logo_image_url']            = url_for('system_bp.merchant_logo_image_url', merchant_act_key=device_setting_details.get('account_id'))
+                    device_setting_details['device_id']                 = device_id
+                    
+                logger.debug('device_setting_details=%s', device_setting_details)
+                
+                return create_rest_message(status_code=StatusCode.OK,
+                                               **device_setting_details
+                                               )
+            else:
+                return create_rest_message('The code have been used in other device', status_code=StatusCode.BAD_REQUEST)
+            
+        else:
+            logger.info('Device setting record is not found');
+            return create_rest_message('Invalid activate code', status_code=StatusCode.BAD_REQUEST, error_code=API_ERR_CODE_INVALID_ACTIVATION_CODE)
+    else:
+        logger.info('activation_code is empty');
+        return create_rest_message('Activation code is required', status_code=StatusCode.BAD_REQUEST)
+
 def getPOSAccountSetting(activation_code):
     if is_not_empty(activation_code):
         db_client = create_db_client(caller_info="getPOSAccountSetting")
         with db_client.context():
             pos_setting = POSSetting.get_by_activation_code(activation_code)
         
         if pos_setting:
             logger.info('Found POS setting');
             #if pos_setting.activated==False:
             if True:
                 logger.info('POS activation code is valid');
                 pos_setting_details = None
                 with db_client.context():
-                    #is_activated = POSSetting.activate(activation_code)
-                    #if is_activated:
-                    #merchant_acct                                       = pos_setting.merchant_acct_entity
+                    if pos_setting.is_test_setting==False:
+                        pos_setting.activate(activation_code)
+                    
                     outlet                                              = pos_setting.assigned_outlet_entity
                     pos_setting_details                                 = merchant_helpers.construct_setting_by_outlet(outlet, device_setting=pos_setting) 
                     
                     pos_setting_details['logo_image_url']               = url_for('system_bp.merchant_logo_image_url', merchant_act_key=pos_setting_details.get('account_id'))
                 
                 #if is_activated:
                 if True:
@@ -102,21 +139,24 @@
             logger.info('POS activation code is valid');
             
             is_valid = False
             pos_setting_details = None
             
             with db_client.context():
                 pos_setting = POSSetting.get_by_activation_code(activation_code)
-                if pos_setting.activated:
-                    if pos_setting.device_id == device_id:
+                if pos_setting.is_test_setting==False:
+                    if pos_setting.activated:
+                        if pos_setting.device_id == device_id:
+                            is_valid = True
+                    else:
                         is_valid = True
+                        pos_setting.activate(device_id)
                 else:
                     is_valid = True
-                    pos_setting.activate(device_id)
-            
+                    
                 if is_valid:    
                     pos_setting_details                                 = merchant_helpers.construct_setting_by_outlet(pos_setting.assigned_outlet_entity, device_setting=pos_setting)
                     #pos_setting_details['logo_image_url']               = url_for('system_bp.merchant_logo_image_url', merchant_act_key=pos_setting_details.get('account_id'))
             
             if is_valid:
                 
                 logger.debug('pos_setting_details=%s', pos_setting_details);
```

### Comparing `trex-apis-1.0.4/trexapi/controllers/reward_api_routes.py` & `trex-apis-1.0.6/trexapi/controllers/reward_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.4/trexapi/controllers/transaction_api_routes.py` & `trex-apis-1.0.6/trexapi/controllers/transaction_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.4/trexapi/controllers/user_api_routes.py` & `trex-apis-1.0.6/trexapi/controllers/user_api_routes.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,40 +4,89 @@
 @author: jacklok
 '''
 
 from flask import Blueprint, request
 import logging
 from trexlib.utils.log_util import get_tracelog
 from trexmodel.utils.model.model_util import create_db_client
-from datetime import datetime
-from trexlib.utils.string_util import is_not_empty
+from datetime import datetime, timedelta
+from trexlib.utils.string_util import is_not_empty, random_number
 from trexmodel.models.datastore.user_models import User
 from trexadmin.libs.http import create_rest_message
 from trexadmin.libs.http import StatusCode
 from werkzeug.datastructures import ImmutableMultiDict
-from trexapi.forms.user_api_forms import UserRegistrationForm, UserUpdateForm
+from trexapi.forms.user_api_forms import UserRegistrationForm, UserUpdateForm,\
+    OutletReviewsForm
 from trexapi.conf import APPLICATION_NAME, APPLICATION_BASE_URL
 from trexmail.email_helper import trigger_send_email
 from trexmodel.models.datastore.merchant_models import MerchantAcct, Outlet
 from trexmodel.models.datastore.customer_models import Customer
 from trexmodel.models.datastore.reward_models import CustomerEntitledVoucher,\
     CustomerPointReward, CustomerEntitledTierRewardSummary
 from trexapi.utils.api_helpers import generate_user_auth_token
 from trexapi.decorators.api_decorators import user_auth_token_required
 from trexadmin.libs.decorators import elapsed_time_trace
 from flask.json import jsonify
+from trexlib.conf import PRODUCTION_MODE, DEPLOYMENT_MODE
+from flask_babel import gettext
 
 user_api_bp = Blueprint('user_api_bp', __name__,
                                  template_folder='templates',
                                  static_folder='static',
                                  url_prefix='/api/v1/users')
 
 logger = logging.getLogger('debug')
 
 
+@user_api_bp.route('/guest-register', methods=['POST'])
+def guest_register():
+    logger.debug('---guest_register---')
+    
+    try:
+        user_data_in_json   = request.get_json()
+        logger.debug('guest_register: user_data_in_json=%s', user_data_in_json)
+        
+        register_user_form  = UserRegistrationForm(ImmutableMultiDict(user_data_in_json))
+        if register_user_form.validate():
+            logger.debug('guest_register:  registration input is valid')
+            db_client = create_db_client(caller_info="guest_register")
+            
+            registered_user_acct    = None
+            
+            with db_client.context():
+                name            = register_user_form.name.data
+                
+                logger.debug('name=%s', name)
+                
+                registered_user_acct = User.create(name=name)
+                        
+                
+                                
+            if registered_user_acct is not None:
+                
+                (expiry_datetime, token)    = generate_user_auth_token(registered_user_acct.user_id, registered_user_acct.reference_code)
+                
+                return create_rest_message(status_code=StatusCode.OK, 
+                                           auth_token                           = token,
+                                           reference_code                       = registered_user_acct.reference_code,
+                                           )
+            else:
+                return create_rest_message(status_code=StatusCode.BAD_REQUEST)
+            
+        else:
+            logger.warn('user_register: user registration input is invalid')
+            error_message = register_user_form.create_rest_return_error_message()
+            
+            return create_rest_message(error_message, status_code=StatusCode.BAD_REQUEST)
+            
+    except:
+        logger.error('user_register: Fail to register user due to %s', get_tracelog())
+        
+        return create_rest_message(status_code=StatusCode.BAD_REQUEST)
+    
 @user_api_bp.route('/register', methods=['POST'])
 def user_register():
     logger.debug('user_register: ---user_register---')
     
     try:
         user_data_in_json   = request.get_json()
         logger.debug('user_register: user_data_in_json=%s', user_data_in_json)
@@ -73,61 +122,60 @@
                         if checking_registered_user_acct is None:
                             registered_user_acct = User.create(name=name, 
                                                                email=email, 
                                                                mobile_phone=mobile_phone, 
                                                                birth_date=birth_date,
                                                                gender=gender,
                                                                password=password, 
-                                                               create_email_vc=True, 
-                                                               create_mobile_phone_vc=True
+                                                               is_email_verified=True, 
+                                                               is_mobile_phone_verified=True
                                                                )
                             logger.debug('new registered_user_acct=%s', registered_user_acct)
                         else:
                             if checking_registered_user_acct.is_mobile_phone_verified==True:
                                 return create_rest_message('Mobile Phone have been taken', status_code=StatusCode.BAD_REQUEST)
                     else:
                         registered_user_acct = User.create(name=name, 
                                                                email=email, 
                                                                birth_date=birth_date,
                                                                gender=gender,
                                                                password=password, 
-                                                               create_email_vc=True, 
-                                                               create_mobile_phone_vc=True
+                                                               is_email_verified=True,
                                                                )
                         
                         logger.debug('new registered_user_acct=%s', registered_user_acct)
                         
                 else:
                     return create_rest_message('Email have been taken', status_code=StatusCode.BAD_REQUEST)
                 
                                 
             if registered_user_acct is not None:
                 
-                send_email_verification_code_email(registered_user_acct)
+                #send_email_verification_code_email(registered_user_acct)
                 (expiry_datetime, token)    = generate_user_auth_token(registered_user_acct.user_id, registered_user_acct.reference_code)
                 
                 return create_rest_message(status_code=StatusCode.OK, 
                                            auth_token                           = token,
                                            reference_code                       = registered_user_acct.reference_code,
-                                           email_vc_expiry_datetime             = str(registered_user_acct.email_vc_expiry_datetime),
-                                           mobile_phone_vc_expiry_datetime      = str(registered_user_acct.mobile_phone_vc_expiry_datetime),
+                                           email_vc_expiry_datetime             = registered_user_acct.email_vc_expiry_datetime.strftime('%d-%m-%Y %H:%M:%S'),
+                                           mobile_phone_vc_expiry_datetime      = registered_user_acct.mobile_phone_vc_expiry_datetime.strftime('%d-%m-%Y %H:%M:%S'),
                                            )
             else:
                 return create_rest_message(status_code=StatusCode.BAD_REQUEST)
             
         else:
             logger.warn('user_register: user registration input is invalid')
             error_message = register_user_form.create_rest_return_error_message()
             
             return create_rest_message(error_message, status_code=StatusCode.BAD_REQUEST)
             
     except:
         logger.error('user_register: Fail to register user due to %s', get_tracelog())
         
-        return create_rest_message(status_code=StatusCode.BAD_REQUEST)
+        return create_rest_message(status_code=StatusCode.BAD_REQUEST)    
 
 @user_api_bp.route('/update', methods=['POST'])
 def user_update():
     logger.debug('user_update: ---user_register---')
     
     try:
         user_data_in_json   = request.get_json()
@@ -236,22 +284,23 @@
 @user_api_bp.route('/verify-email', methods=['POST'])
 def verify_email_account():
     
     user_data_in_json   = request.get_json()
     email               = user_data_in_json.get('email')
     verification_code   = user_data_in_json.get('verification_code')
     
+    
     if is_not_empty(email) and is_not_empty(verification_code):
         db_client = create_db_client(caller_info="verify_email_account")
         user_acct = None
         
         logger.debug('verify_email_account: going to find user account by email=%s', email)
         
         with db_client.context():
-            user_acct = User.get_by_email(email)
+            user_acct   = User.get_by_email(email)
         
         if user_acct:
             logger.debug('verify_email_account: found user account by email=%s', email)    
             if user_acct.email_vc==verification_code:
                 is_within_seconds = (user_acct.email_vc_expiry_datetime - datetime.now()).seconds
                 if is_within_seconds>0:
                     with db_client.context():
@@ -267,44 +316,50 @@
         else:
             return create_rest_message(status_code=StatusCode.BAD_REQUEST)
             
     else:
         logger.warn('verify_email_account: user verify input is invalid')
         return create_rest_message(status_code=StatusCode.BAD_REQUEST)    
     
-@user_api_bp.route('/verify-email', methods=['POST'])
+@user_api_bp.route('/verify-mobile-phone', methods=['POST'])
 def verify_mobile_phone_account():
     
     user_data_in_json   = request.get_json()
     mobile_phone        = user_data_in_json.get('mobile_phone')
     verification_code   = user_data_in_json.get('verification_code')
+    reference_code      = request.headers.get('x-reference-code')
     
     if is_not_empty(mobile_phone) and is_not_empty(verification_code):
         db_client = create_db_client(caller_info="verify_mobile_phone_account")
         user_acct = None
         with db_client.context():
-            user_acct = User.get_by_mobile_phone(mobile_phone)
+            user_acct_by_mobile_phone   = User.get_by_mobile_phone(mobile_phone)
+            user_acct                   = User.get_by_reference_code(reference_code)
         
-        if user_acct:
-            logger.debug('verify_mobile_phone_account: found user account by mobile_phone=%s', mobile_phone)    
-            if user_acct.mobile_phone_vc==verification_code:
-                is_within_seconds = (user_acct.mobile_phone_vc_expiry_datetime - datetime.now()).seconds
-                if is_within_seconds>0:
-                    with db_client.context():
-                        user_acct.mark_email_verified()
-                    return create_rest_message(status_code=StatusCode.OK)
+        if user_acct_by_mobile_phone is None or user_acct_by_mobile_phone.reference_code == reference_code:
+            if user_acct:
+                logger.debug('verify_mobile_phone_account: found user account by mobile_phone=%s', mobile_phone)    
+                if user_acct.mobile_phone_vc==verification_code:
+                    is_within_seconds = (user_acct.mobile_phone_vc_expiry_datetime - datetime.now()).seconds
+                    if is_within_seconds>0:
+                        with db_client.context():
+                            user_acct.mark_email_verified()
+                        return create_rest_message(status_code=StatusCode.OK)
+                    else:
+                        return create_rest_message("Verification Code is expired already", status_code=StatusCode.BAD_REQUEST)
+                
                 else:
-                    return create_rest_message("Verification Code is expired already", status_code=StatusCode.BAD_REQUEST)
-            
+                    logger.warn('verify_mobile_phone_account: verification code is invalid')
+                    return create_rest_message("Invalid verification code", status_code=StatusCode.BAD_REQUEST)
+                
             else:
-                logger.warn('verify_mobile_phone_account: verification code is invalid')
-                return create_rest_message("Invalid verification code", status_code=StatusCode.BAD_REQUEST)
-            
+                
+                return create_rest_message(gettext('Invalid user account'), status_code=StatusCode.BAD_REQUEST)
         else:
-            return create_rest_message(status_code=StatusCode.BAD_REQUEST)
+            return create_rest_message(gettext('Mobile phone have been taken'), status_code=StatusCode.BAD_REQUEST)
             
     else:
         logger.warn('verify_mobile_phone_account: user verify input is invalid')
         return create_rest_message(status_code=StatusCode.BAD_REQUEST)        
 
 @user_api_bp.route('/register-as-customer', methods=['POST'])
 #@user_auth_token_required
@@ -551,24 +606,32 @@
             if customer_tier_reward_summary:
                 for v in customer_tier_reward_summary:
                     tier_rewards.append(v.to_dict())
     
     
     
     result = {
-            'reference_code'    : reference_code,
+            'reference_code'                        : reference_code,
             #'vouchers'          : vouchers_list,
-            'tier_rewards'      : tier_rewards,
-            'reward_summary'    : customer.reward_summary,
-            'prepaid_summary'   : customer.prepaid_summary,
-            'voucher_summary'   : customer.entitled_voucher_summary,
+            'tier_rewards'                          : tier_rewards,
+            'reward_summary'                        : customer.reward_summary,
+            'prepaid_summary'                       : customer.prepaid_summary,
+            'entitled_voucher_summary'              : customer.entitled_voucher_summary,
+            'entitled_lucky_draw_ticket_summary'    : customer.entitled_lucky_draw_ticket_summary,
             }
     
     return jsonify(result)
     
+@user_api_bp.route('/check-auth-token', methods=['POST'])
+@user_auth_token_required
+def check_auth_token():
+    return create_rest_message(status_code=StatusCode.OK,)
+
+
+    
 @user_api_bp.route('/<reference_code>', methods=['GET'])
 @user_auth_token_required
 def read_user_acct(reference_code):
     
     if is_not_empty(reference_code):
         db_client = create_db_client(caller_info="read_user_acct")
         user_acct = None
@@ -604,17 +667,19 @@
             logger.debug('user account is not found')
             return create_rest_message(status_code=StatusCode.BAD_REQUEST)
             
     else:
         logger.warn('verify_user: user verify input is invalid')
         return create_rest_message(status_code=StatusCode.BAD_REQUEST)    
 
-@user_api_bp.route('/<reference_code>/joined-brands-list', methods=['GET'])
-#@user_auth_token_required
-def list_joined_brands(reference_code):
+@user_api_bp.route('/joined-brands-list', methods=['GET'])
+@user_auth_token_required
+def list_joined_brands():
+    reference_code = request.headers.get('x-reference-code')
+    
     limit           = request.args.get('limit')
     start_cursor    = request.args.get('start_cursor')
     
     logger.debug('limit=%s', limit)
     logger.debug('start_cursor=%s', start_cursor)
     
     if is_not_empty(reference_code):
@@ -637,50 +702,20 @@
             with db_client.context():
                 (customer_accts_list, next_cursor) = Customer.list_paginated_by_user_account(user_acct, start_cursor=start_cursor, limit=limit)
                 
                 for customer_acct in customer_accts_list:
                     merchant_acct = customer_acct.registered_merchant_acct
                     brands_list.append({
                                         'key'       : merchant_acct.key_in_str,
+                                        'account_id': merchant_acct.account_code,
                                         'name'      : merchant_acct.brand_name,
                                         'logo_url'  : merchant_acct.logo_public_url,
                                         
                                         })
-                    '''
-                    brands_list.append({
-                                        'key'       : merchant_acct.key_in_str,
-                                        'name'      : merchant_acct.brand_name,
-                                        'logo_url'  : merchant_acct.logo_public_url,
-                                        
-                                        })
-                    brands_list.append({
-                                        'key'       : merchant_acct.key_in_str,
-                                        'name'      : merchant_acct.brand_name,
-                                        'logo_url'  : merchant_acct.logo_public_url,
-                                        
-                                        })
-                    brands_list.append({
-                                        'key'       : merchant_acct.key_in_str,
-                                        'name'      : merchant_acct.brand_name,
-                                        'logo_url'  : merchant_acct.logo_public_url,
-                                        
-                                        })
-                    brands_list.append({
-                                        'key'       : merchant_acct.key_in_str,
-                                        'name'      : merchant_acct.brand_name,
-                                        'logo_url'  : merchant_acct.logo_public_url,
-                                        
-                                        })
-                    brands_list.append({
-                                        'key'       : merchant_acct.key_in_str,
-                                        'name'      : merchant_acct.brand_name,
-                                        'logo_url'  : merchant_acct.logo_public_url,
-                                        
-                                        })
-                     '''                    
+                                       
                 result_data= {
                                 'result'        : brands_list,
                                 'count'         : len(brands_list),
                                 }
                   
                 if is_not_empty(next_cursor):
                     result_data['next_cursor'] = next_cursor  
@@ -704,71 +739,147 @@
         user_acct = None
         
         
         
         with db_client.context():
             user_acct = User.get_by_email(email)
         
-        if user_acct:
+        if user_acct is None:
+            '''
             logger.debug('reset_email_verification_code: found user account by email=%s', email)    
             is_email_verified           = user_acct.is_email_verified
             
             logger.debug('reset_email_verification_code: is_email_verified=%s', is_email_verified)
             
             email_vc_expiry_datetime = None
             
             with db_client.context():
                 user_acct.reset_email_vc()
+            
             email_vc_expiry_datetime = user_acct.email_vc_expiry_datetime
-                
-                #send_email_verification_code_email(user_acct)
+            '''
+            
+            
+            email_vc_expiry_datetime    = datetime.utcnow() + timedelta(minutes=2)
+            email_vc                    = random_number(6)
+            
+            send_email_verification_code_email(email, email_vc)
             
             logger.debug('reset_email_verification_code: email_vc_expiry_datetime=%s', email_vc_expiry_datetime)
-            logger.debug('reset_email_verification_code: verification code=%s', user_acct.email_vc)
+            logger.debug('reset_email_verification_code: verification code=%s', email_vc)
                 
             return create_rest_message(status_code=StatusCode.OK, 
-                                       email_vc_expiry_datetime          = str(email_vc_expiry_datetime),
-                                       
+                                       #email_vc_expiry_datetime          = str(email_vc_expiry_datetime),
+                                       expiry_datetime     = email_vc_expiry_datetime.strftime('%d-%m-%Y %H:%M:%S'),
+                                       code                = email_vc,
                                        )
         else:
-            return create_rest_message('Cannot find user by email %s' % email, status_code=StatusCode.BAD_REQUEST)
+            return create_rest_message('The email have been taken %s' % email, status_code=StatusCode.BAD_REQUEST)
             
     else:
         logger.warn('reset_email_verification_code: reference code is invalid')
         return create_rest_message(status_code=StatusCode.BAD_REQUEST) 
     
 @user_api_bp.route('/reset-mobile-phone-vc', methods=['PUT'])
+@user_auth_token_required
 def reset_mobile_phone_verification_code():
     mobile_phone = request.args.get('mobile_phone') or request.form.get('mobile_phone') or request.json.get('mobile_phone')
+
+    reference_code = request.headers.get('x-reference-code')    
+    logger.debug('mobile_phone=%s', mobile_phone)
+    logger.debug('reference_code=%s', reference_code)
+    
     if is_not_empty(mobile_phone):
-        db_client = create_db_client(caller_info="reset_verification_code")
+        db_client                           = create_db_client(caller_info="reset_verification_code")
+        user_acct                           = None
+        mobile_phone_vc_expiry_datetime     = None
+        
+        with db_client.context():
+            user_by_mobile_phone    = User.get_by_mobile_phone(mobile_phone)
+        
+        if user_by_mobile_phone is not None:
+            if reference_code==user_by_mobile_phone.reference_code:
+                #logger.debug('reset_mobile_phone_verification_code: found user account by mobile_phone=%s', mobile_phone)    
+                #is_mobile_phone_verified           = user_acct.is_mobile_phone_verified
+                
+                
+                with db_client.context():
+                    user_by_mobile_phone.reset_mobile_phone_vc()
+                    
+                logger.debug('reset_mobile_phone_verification_code: mobile_phone_vc_expiry_datetime=%s', mobile_phone_vc_expiry_datetime)
+                logger.debug('reset_mobile_phone_verification_code: verification code=%s', user_acct.mobile_phone_vc)   
+                
+                return create_rest_message(status_code=StatusCode.OK, 
+                                           expiry_datetime     = mobile_phone_vc_expiry_datetime.strftime('%d-%m-%Y %H:%M:%S'),
+                                           code                = user_acct.mobile_phone_vc,
+                                           )
+            else:
+                return create_rest_message(gettext('Mobile phone have been taken'), status_code=StatusCode.BAD_REQUEST)
+        else:
+            with db_client.context():
+                user_acct    = User.get_by_reference_code(reference_code)
+            
+            if user_acct is not None:
+                with db_client.context():
+                    user_acct.reset_mobile_phone_vc()
+                    
+                    mobile_phone_vc_expiry_datetime = user_acct.mobile_phone_vc_expiry_datetime
+            
+                logger.debug('reset_mobile_phone_verification_code: mobile_phone_vc_expiry_datetime=%s', mobile_phone_vc_expiry_datetime)
+                logger.debug('reset_mobile_phone_verification_code: verification code=%s', user_acct.mobile_phone_vc)    
+            
+                return create_rest_message(status_code=StatusCode.OK, 
+                                           expiry_datetime     = mobile_phone_vc_expiry_datetime.strftime('%d-%m-%Y %H:%M:%S'),
+                                           code                = user_acct.mobile_phone_vc,
+                                           
+                                           )
+            else:
+                return create_rest_message(gettext('Invalid input'), status_code=StatusCode.BAD_REQUEST)
+                
+                
+    else:
+        logger.warn('reset_mobile_phone_verification_code: mobile phone is invalid')
+        return create_rest_message(gettext('Missing mobile phone'), status_code=StatusCode.BAD_REQUEST)  
+    
+@user_api_bp.route('/change-password', methods=['PUT'])
+@user_auth_token_required
+def change_password():
+    
+    reference_code = request.headers.get('x-reference-code')
+    
+    existing_password   = request.args.get('existing_password') or request.form.get('existing_password') or request.json.get('existing_password')
+    new_password        = request.args.get('new_password') or request.form.get('new_password') or request.json.get('new_password')
+    
+    if is_not_empty(existing_password) and is_not_empty(new_password):
+        db_client = create_db_client(caller_info="change_password")
         user_acct = None
+        is_existing_password_valid = False
         with db_client.context():
-            user_acct = User.get_by_mobile_phone(mobile_phone)
+            user_acct = User.get_by_reference_code(reference_code)
         
         if user_acct:
-            logger.debug('reset_mobile_phone_verification_code: found user account by mobile_phone=%s', mobile_phone)    
-            is_mobile_phone_verified           = user_acct.is_mobile_phone_verified
-            mobile_phone_vc_expiry_datetime = None
+            logger.debug('change_password: found user account by reference_code=%s', reference_code)    
+            logger.debug('change_password: existing_password=%s', existing_password)
+            logger.debug('change_password: new_password=%s', new_password)
             
             with db_client.context():
-                user_acct.reset_mobile_phone_vc()
-                
-            logger.debug('reset_mobile_phone_verification_code: mobile_phone_vc_expiry_datetime=%s', mobile_phone_vc_expiry_datetime)
-            logger.debug('reset_mobile_phone_verification_code: verification code=%s', user_acct.mobile_phone_vc)   
-            return create_rest_message(status_code=StatusCode.OK, 
-                                       mobile_phone_vc_expiry_datetime   = str(mobile_phone_vc_expiry_datetime),
+                if user_acct.is_valid_password(existing_password):
+                    is_existing_password_valid = True
+                    user_acct.change_password(new_password)
+                
+        if is_existing_password_valid:    
+            return create_rest_message(
+                                    status_code=StatusCode.OK
                                        
                                        )
         else:
-            return create_rest_message(status_code=StatusCode.BAD_REQUEST)
+            return create_rest_message('existing password is not valid', status_code=StatusCode.BAD_REQUEST)
             
     else:
-        logger.warn('reset_mobile_phone_verification_code: mobile phone is invalid')
-        return create_rest_message(status_code=StatusCode.BAD_REQUEST)  
+        return create_rest_message('Missing password input', status_code=StatusCode.BAD_REQUEST)      
     
 @user_api_bp.route('/request-reset-password', methods=['POST'])
 def request_reset_password_post():
     email = request.args.get('email') or request.form.get('email') or request.json.get('email')
     
     logger.debug('reset_password_request_post: going to reset email verification code by email=%s', email)
     
@@ -800,17 +911,72 @@
             return create_rest_message('Cannot find user by email %s' % email, status_code=StatusCode.BAD_REQUEST)
             
     else:
         logger.warn('reset_password_post: email is invalid')
         return create_rest_message(status_code=StatusCode.BAD_REQUEST)                 
 
 
-def send_email_verification_code_email(user_acct):
+@user_api_bp.route('/outlet-reviews', methods=['POST'])
+@user_auth_token_required
+def outlet_reviews():
+    logger.debug('---outlet_reviews---')
+    
+    try:
+        reviews_data_in_json   = request.get_json()
+        logger.debug('outlet_reviews: reviews_data_in_json=%s', reviews_data_in_json)
+        
+        reviews_data_form  = OutletReviewsForm(ImmutableMultiDict(reviews_data_in_json))
+        
+        if reviews_data_form.validate():
+            food_score              = reviews_data_form.food_score.data
+            service_score           = reviews_data_form.service_score.data
+            ambience_score          = reviews_data_form.ambience_score.data
+            value_for_money_score   = reviews_data_form.value_for_money_score.data
+            
+            logger.debug('outlet_reviews: food_score=%s', food_score)
+            logger.debug('outlet_reviews: service_score=%s', service_score)
+            logger.debug('outlet_reviews: ambience_score=%s', ambience_score)
+            logger.debug('outlet_reviews: value_for_money_score=%s', value_for_money_score)
+            
+            return create_rest_message(status_code=StatusCode.OK)
+        
+        else:
+            logger.warn('outlet_reviews: outlet reviews input is invalid')
+            error_message = reviews_data_form.create_rest_return_error_message()
+            
+            return create_rest_message(error_message, status_code=StatusCode.BAD_REQUEST)
+    except:
+        return create_rest_message('Failed to process outlet reviews', status_code=StatusCode.BAD_REQUEST)   
+        
+@user_api_bp.route('/voucher/<redeem_code>/remove', methods=['DELETE'])
+@user_auth_token_required
+def remove_user_voucher(redeem_code):
+    if is_not_empty(redeem_code):
+        reference_code = request.headers.get('x-reference-code')
+        logger.debug('reference_code=%s', reference_code)
+        db_client = create_db_client(caller_info="remove_user_voucher")
+        with db_client.context():
+            customer_voucher    = CustomerEntitledVoucher.get_by_redeem_code(redeem_code)
+            
+            if customer_voucher: 
+                
+                customer_voucher.remove()  
+                customer = customer_voucher.entitled_customer_acct
+                customer.update_after_removed_voucher(customer_voucher)
+                
+        if customer_voucher:        
+            return create_rest_message(status_code=StatusCode.OK)
+        else:
+            return create_rest_message('Invalid voucher redeem code', status_code=StatusCode.BAD_REQUEST)
+    else:
+        return create_rest_message('Missing voucher redeem code', status_code=StatusCode.BAD_REQUEST)
+
+def send_email_verification_code_email(email, verification_code):
     message = '''
-                Hi {name},
+                Dear,
                 
                 
                 Thanks for signing up with {application_name}!
                 Your account has been created, you can login with email {email} in future. 
                 
                 Just one more step to get started! Please enter below code to activate your account .
                 
@@ -822,32 +988,37 @@
                 
                 Cheers,
                 {application_name} Team
                 
                 
                 ***Please do not reply to this email. This is an auto-generated email.***
     
-            '''.format(name=user_acct.name, email=user_acct.email, verification_code=user_acct.email_vc, application_name=APPLICATION_NAME)
+            '''.format(email=email, verification_code=verification_code, application_name=APPLICATION_NAME)
     
     subject      = 'Email Verification from {application_name}'.format(application_name=APPLICATION_NAME)
     
-    trigger_send_email(recipient_address = user_acct.email, subject=subject, message=message)
+    if DEPLOYMENT_MODE==PRODUCTION_MODE:
+        trigger_send_email(recipient_address = email, subject=subject, message=message)
+    else:
+        logger.debug('not send email for development or local mode')
+        logger.debug(message)
+        
     '''
     send_email(sender           = DEFAULT_SENDER, 
                    to_address   = [user_acct.email], 
                    subject      = subject, 
                    body         = message,
                    app          = current_app
                    )
     '''
 def send_reset_password_request_email(user_acct):
-    reset_password_link = '{base_url}/user/reset-password-request/{request_reset_password_token}'.format(base_url=APPLICATION_BASE_URL, request_reset_password_token=user_acct.request_reset_password_token)
+    reset_password_link = '{base_url}user/reset-password-request/{request_reset_password_token}'.format(base_url=APPLICATION_BASE_URL, request_reset_password_token=user_acct.request_reset_password_token)
     
     message = '''
-                Hi {name},
+                Dear {name},
                 
                 
                 Forgot your password? No worries.
                 We received your request to reset the password for your account. 
                 
                 Just one more step to reset the password, please click the below link:
```

### Comparing `trex-apis-1.0.4/trexapi/controllers/user_reward_api_routes.py` & `trex-apis-1.0.6/trexapi/controllers/user_reward_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.4/trexapi/controllers/voucher_api_routes.py` & `trex-apis-1.0.6/trexapi/controllers/voucher_api_routes.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 '''
 
 from flask import Blueprint, request, session 
 import logging
 from trexlib.utils.log_util import get_tracelog
 from trexmodel.utils.model.model_util import create_db_client
 from datetime import datetime, timedelta
-from trexapi.decorators.api_decorators import auth_token_required
+from trexapi.decorators.api_decorators import auth_token_required,\
+    user_auth_token_required
 from trexlib.utils.string_util import is_not_empty, is_empty
 from trexmodel.models.datastore.customer_models import Customer
 from trexadmin.libs.http import create_rest_message
 from trexadmin.libs.http import StatusCode
 from trexmodel.models.datastore.merchant_models import Outlet,\
     MerchantUser, MerchantAcct
 from trexapi.forms.reward_api_forms import VoucherRedeemForm, VoucherRemoveForm
@@ -42,15 +43,15 @@
 logger = logging.getLogger('api')
 
 @voucher_api_bp.route('/ping', methods=['GET'])
 def ping():
     return create_rest_message('Pong', status_code=StatusCode.OK)
 
 @voucher_api_bp.route('/voucher/<redeem_code>/details', methods=['GET'])
-#@auth_token_required
+@auth_token_required
 def read_voucher(redeem_code):
     if is_not_empty(redeem_code):
         voucher_details = None
         db_client = create_db_client(caller_info="read_voucher")
         with db_client.context():
             customer_voucher    = CustomerEntitledVoucher.get_by_redeem_code(redeem_code)
             if customer_voucher:
@@ -209,15 +210,15 @@
     
     remove_voucher_form = VoucherRemoveForm(ImmutableMultiDict(remove_voucher_data_in_json))
     if remove_voucher_form.validate():
     
         #redeem_code         = remove_voucher_data_in_json.get('redeem_code')
         remarks             = remove_voucher_form.remarks.data
         remove_datetime     = remove_voucher_form.remove_datetime.data
-        merchant_acct       = None
+        #merchant_acct       = None
         
         logger.debug('redeem_code=%s', redeem_code)
         logger.debug('remove_datetime=%s', remove_datetime)
         
         
         if redeem_code:
             #redeem_code_list = redeem_code_list.split(',')
@@ -296,8 +297,29 @@
         return {
                 'vouchers': voucher_list,
             }
             
     else:
         logger.warn('reset_password_post: email is invalid')
         return create_rest_message(status_code=StatusCode.BAD_REQUEST)       
-    
+    
+@voucher_api_bp.route('/voucher/<redeem_code>/remove-by-user', methods=['DELETE'])
+@user_auth_token_required
+def remove_user_voucher(redeem_code):
+    if is_not_empty(redeem_code):
+        reference_code = request.headers.get('x-reference-code')
+        logger.debug('reference_code=%s', reference_code)
+        db_client = create_db_client(caller_info="remove_user_voucher")
+        with db_client.context():
+            customer_voucher    = CustomerEntitledVoucher.get_by_redeem_code(redeem_code)
+            '''
+            if customer_voucher: 
+                customer_voucher.remove()  
+                customer = customer_voucher.entitled_customer_acct
+                customer.update_after_removed_voucher(customer_voucher)
+            '''    
+        if customer_voucher:        
+            return create_rest_message(status_code=StatusCode.BAD_REQUEST)
+        else:
+            return create_rest_message('Invalid voucher redeem code', status_code=StatusCode.BAD_REQUEST)
+    else:
+        return create_rest_message('Missing voucher redeem code', status_code=StatusCode.BAD_REQUEST)
```

### Comparing `trex-apis-1.0.4/trexapi/decorators/api_decorators.py` & `trex-apis-1.0.6/trexapi/decorators/api_decorators.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 '''
 from functools import wraps
 from flask import request, session, abort
 from trexlib.utils.string_util import is_not_empty
 from trexlib.utils.crypto_util import decrypt_json
 import logging
 from datetime import datetime
+from trexlib.utils.log_util import get_tracelog
+from trexadmin.libs.http import create_rest_message, StatusCode
 
 logger = logging.getLogger('decorator')
 #logger = logging.getLogger('debug')
 
 def test_session_expired(f):
     @wraps(f)
     def decorated_function(*args, **kwargs):
@@ -69,22 +71,24 @@
     def decorated_function(*args, **kwargs):
         user_auth_token     = request.headers.get('x-auth-token')
         user_reference_code = request.headers.get('x-reference-code')
             
         logger.debug('user_auth_token=%s', user_auth_token)
         
         if is_not_empty(user_auth_token):
+            logger.debug('user_auth_token is not empty, going to decrypt it')
             try:
                 auth_details_json = decrypt_json(user_auth_token)
+                logger.debug('auth_details_json=%s', auth_details_json)
+                
             except:
+                logger.error('Failed due to %s', get_tracelog())
                 return ("Authenticated token is not valid", 401)
             
-             
             
-            logger.debug('auth_details_json=%s', auth_details_json)
             
             if auth_details_json:
                 expiry_datetime                 = auth_details_json.get('expiry_datetime')
                 user_reference_code_from_token  = auth_details_json.get('reference_code')
                 
                 if is_not_empty(expiry_datetime) and is_not_empty(user_reference_code_from_token) and user_reference_code_from_token == user_reference_code:
                     expiry_datetime = datetime.strptime(expiry_datetime, '%d-%m-%Y %H:%M:%S')
@@ -93,19 +97,22 @@
                     now             = datetime.now()
                     if now < expiry_datetime: 
                         logger.debug('auth token is still valid')
                         return f(*args, **kwargs)
                     else:
                         logger.debug('auth token is not logger valid')
                         
-                        return ("Authenticated token is expired", 401)
+                        #return ("Authenticated token is expired", 401)
+                        return create_rest_message('Authenticated token is expired', status_code=StatusCode.UNAUTHORIZED,)
             else:
-                return ("Authenticated token is invalid", 401)    
+                #return ("Authenticated token is invalid", 401)    
+                return create_rest_message('Authenticated token is invalid', status_code=StatusCode.UNAUTHORIZED,)
         
-        return ("Authenticated token is required", 401)
+        #return ("Authenticated token is required", 401)
+        return create_rest_message('Authenticated token is required', status_code=StatusCode.UNAUTHORIZED,)
 
     return decorated_function
 
 def outlet_key_required(f):
     @wraps(f)
     def decorated_function(*args, **kwargs):
         outlet_key = request.headers.get('x-outlet-key')
@@ -116,7 +123,23 @@
             logger.debug('Going to execute')
             return f(*args, **kwargs)
             
         
         return ("Outlet Key is required", 401)
 
     return decorated_function
+
+def merchant_key_required(f):
+    @wraps(f)
+    def decorated_function(*args, **kwargs):
+        acct_id = request.headers.get('x-acct-id')
+            
+        logger.debug('acct_id=%s', acct_id)
+        
+        if is_not_empty(acct_id):
+            logger.debug('Going to execute')
+            return f(*args, **kwargs)
+            
+        
+        return ("Merchant account id is required", 401)
+
+    return decorated_function
```

### Comparing `trex-apis-1.0.4/trexapi/forms/customer_api_forms.py` & `trex-apis-1.0.6/trexapi/forms/customer_api_forms.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.4/trexapi/forms/reward_api_forms.py` & `trex-apis-1.0.6/trexapi/forms/reward_api_forms.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.4/trexapi/forms/sales_api_forms.py` & `trex-apis-1.0.6/trexapi/forms/sales_api_forms.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.4/trexapi/forms/user_api_forms.py` & `trex-apis-1.0.6/trexapi/forms/user_api_forms.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from wtforms import StringField, PasswordField, validators, DateField
 from trexadmin.forms.base_forms import ValidationBaseForm
 from trexadmin.libs.wtforms import validators as custom_validator
 from flask_babel import gettext
 from datetime import date
+from wtforms.fields.core import FloatField
 
 class UserMinForm(ValidationBaseForm):
     name                = StringField(gettext('Name'), validators=[
                                         validators.InputRequired(gettext('Name is required')),
                                         validators.Length(min=3, max=300, message='Name length must be within 3 and 300 characters'),
                                         
                                         ]
@@ -43,8 +44,32 @@
     
 class UserUpdateForm(UserMinForm):
     reference_code      = StringField('User Reference Code', validators=[
                                         validators.InputRequired(gettext('User Reference Code is required')),
                                         ]
                                         )      
     
-  
+class OutletReviewsForm(ValidationBaseForm):
+    outlet_key               = StringField('Outlet Key', validators=[
+                                        validators.InputRequired(gettext('Outlet key is required')),
+                                        ]
+                                        )
+    
+    food_score               = FloatField('Food Score', validators=[
+                                        validators.InputRequired(gettext('Food score is required')),
+                                        ]
+                                        )
+    
+    service_score               = FloatField('Service Score', validators=[
+                                        validators.InputRequired(gettext('Service score is required')),
+                                        ]
+                                        )
+    
+    ambience_score          = FloatField('Ambience Score', validators=[
+                                        validators.InputRequired(gettext('Ambience score is required')),
+                                        ]
+                                        )
+    
+    value_for_money_score   = FloatField('Value for money Score', validators=[
+                                        validators.InputRequired(gettext('Value for money score is required')),
+                                        ]
+                                        )
```

### Comparing `trex-apis-1.0.4/trexapi/libs/flask_auth_wrapper.py` & `trex-apis-1.0.6/trexapi/libs/flask_auth_wrapper.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.4/trexapi/utils/api_helpers.py` & `trex-apis-1.0.6/trexapi/utils/api_helpers.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.4/trexapi/utils/reward_transaction_helper.py` & `trex-apis-1.0.6/trexapi/utils/reward_transaction_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 from trexmodel.models.datastore.prepaid_models import CustomerPrepaidReward
 from trexadmin.libs.app.reward_program.reward_program_base import EntitledVoucherSummary
 from trexmodel.models.datastore.customer_models import Customer,\
     CustomerMembership, CustomerTierMembership
 from trexmodel.models.datastore.redeem_models import CustomerRedemption
 from trexlib.utils.string_util import is_not_empty
 from trexlib.utils.log_util import get_tracelog
+from trexmodel.models.datastore.lucky_draw_models import LuckyDrawTicket
 
 logger = logging.getLogger('debug')
 #logger = logging.getLogger('debug')
 
 
 def create_sales_transaction(transact_outlet=None, sales_amount=.0, tax_amount=.0, invoice_id=None, remarks=None, 
                             transact_by=None, transact_datetime=None, invoice_details=None):
@@ -107,14 +108,38 @@
         if trigger_check_reward_success:
             create_merchant_customer_transaction_upstream_for_merchant(customer_transaction, streamed_datetime=transact_datetime)
         
         return customer_transaction
         
     return __start_transaction_for_customer_transaction()
 
+def give_reward_from_sales_transaction(customer, sales_transaction):
+    
+    logger.debug('---give_reward_from_sales_transaction---')
+    
+    @model_transactional(desc='give_reward_from_sales_transaction')
+    def __start_transaction(customer, sales_transaction):
+        customer_transaction = CustomerTransaction.create_from_sales_transaction(customer, sales_transaction)
+        
+        trigger_check_reward_success = trigger_spending_reward_for_transaction(customer_transaction)
+        
+        logger.debug('trigger_check_reward_success=%s', trigger_check_reward_success)
+        
+        if trigger_check_reward_success:
+            create_merchant_customer_transaction_upstream_for_merchant(customer_transaction, streamed_datetime=sales_transaction.transact_datetime)
+        
+        return customer_transaction
+    
+    customer_transaction = CustomerTransaction.get_by_transaction_id(sales_transaction.transaction_id)
+    if customer_transaction is None:
+        customer_transaction = __start_transaction(customer, sales_transaction)
+    
+    return customer_transaction
+    
+
 def create_non_sales_system_transaction(customer, transact_datetime=None, remarks=None, system_remarks=None):
     
     logger.debug('---create_non_sales_system_transaction---')
     
     #@model_transactional(desc='create_non_sales_system_transaction')
     def __start_transaction_for_customer_transaction():
         customer_transaction = CustomerTransaction.create_system_transaction(
@@ -510,17 +535,33 @@
     
     
     if give_reward_status:
         #check if the giveaway reward format match tier reward program setting
         check_tier_reward_for_transaction(customer_acct, transaction_details)
         update_customer_kpi_summary_and_transact_summary(customer_acct, transaction_details)
         check_for_tier_membership_upgrade_downgrade(customer_acct, merchant_acct, transaction_details)
+        check_entitled_lucky_draw_ticket_for_transaction(customer_acct, merchant_acct, transaction_details)
         
     return give_reward_status
+
+def check_entitled_lucky_draw_ticket_for_transaction(customer_acct, merchant_acct, transaction_details):
     
+    if merchant_acct.lucky_draw_program_count>0:
+        entries_list = LuckyDrawTicket.create_for_customer_from_sales_amount(customer_acct, sales_amount=transaction_details.transact_amount, merchant_acct=merchant_acct, transact_outlet=transaction_details.transact_outlet_entity)
+        ticket_configurations_list = []
+        logger.debug('entries_list count=%d', len(entries_list))
+        
+        for e in entries_list:
+            ticket_configurations_list.append(e.to_configuration())
+        
+        if ticket_configurations_list:
+            Customer.add_new_tickets_list_into_lucky_draw_ticket_summary(customer_acct, ticket_configurations_list)
+            transaction_details.update_entitled_lucky_draw_ticket_summary(ticket_configurations_list)
+            
+            
 def check_giveaway_reward_for_transaction(customer_acct, transaction_details, program_configuration_list=None, reward_set=1):
     merchant_acct                   = transaction_details.transact_merchant_acct
     program_configuration_list      = merchant_acct.program_configuration_list if program_configuration_list is None else program_configuration_list
     currency_code                   = merchant_acct.currency_code
     
     currency_config                 = get_currency_config(currency_code)
```

