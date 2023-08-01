# Comparing `tmp/Sift-5.3.0.tar.gz` & `tmp/Sift-5.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Sift-5.3.0.tar", last modified: Fri Feb  3 11:36:08 2023, max compression
+gzip compressed data, was "Sift-5.4.0.tar", last modified: Tue Aug  1 16:30:05 2023, max compression
```

## Comparing `Sift-5.3.0.tar` & `Sift-5.4.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 11:36:08.231741 Sift-5.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-02-03 11:36:07.000000 Sift-5.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-03 11:36:07.000000 Sift-5.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9056 2023-02-03 11:36:08.231741 Sift-5.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-02-03 11:36:07.000000 Sift-5.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 11:36:08.227741 Sift-5.3.0/Sift.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9056 2023-02-03 11:36:08.000000 Sift-5.3.0/Sift.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-02-03 11:36:08.000000 Sift-5.3.0/Sift.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-03 11:36:08.000000 Sift-5.3.0/Sift.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-02-03 11:36:08.000000 Sift-5.3.0/Sift.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-03 11:36:08.000000 Sift-5.3.0/Sift.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-03 11:36:08.231741 Sift-5.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-02-03 11:36:07.000000 Sift-5.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 11:36:08.231741 Sift-5.3.0/sift/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-02-03 11:36:07.000000 Sift-5.3.0/sift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37210 2023-02-03 11:36:07.000000 Sift-5.3.0/sift/client.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-03 11:36:07.000000 Sift-5.3.0/sift/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:30:05.482966 Sift-5.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-08-01 16:30:05.000000 Sift-5.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-01 16:30:05.000000 Sift-5.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-08-01 16:30:05.482966 Sift-5.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6451 2023-08-01 16:30:05.000000 Sift-5.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:30:05.482966 Sift-5.4.0/Sift.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-08-01 16:30:05.000000 Sift-5.4.0/Sift.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-08-01 16:30:05.000000 Sift-5.4.0/Sift.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 16:30:05.000000 Sift-5.4.0/Sift.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-01 16:30:05.000000 Sift-5.4.0/Sift.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-01 16:30:05.000000 Sift-5.4.0/Sift.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 16:30:05.482966 Sift-5.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-08-01 16:30:05.000000 Sift-5.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:30:05.482966 Sift-5.4.0/sift/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-01 16:30:05.000000 Sift-5.4.0/sift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45891 2023-08-01 16:30:05.000000 Sift-5.4.0/sift/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 16:30:05.000000 Sift-5.4.0/sift/version.py
```

### Comparing `Sift-5.3.0/LICENSE` & `Sift-5.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Sift-5.3.0/PKG-INFO` & `Sift-5.4.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Sift
-Version: 5.3.0
+Version: 5.4.0
 Summary: Python bindings for Sift Science's API
 Home-page: https://siftscience.com
 Author: Sift Science
 Author-email: support@siftscience.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
@@ -109,14 +109,41 @@
     response = client.track("$transaction", properties)
     if response.is_ok():
         print "Successfully tracked event"
 except sift.client.ApiException:
     # request failed
     pass
 
+# Track a transaсtion event and receive a score with percentiles in response (sync flow).
+# Note: `return_score` or `return_workflow_status` must be set `True`.
+properties = {
+    "$user_id": user_id,
+    "$user_email": "buyer@gmail.com",
+    "$seller_user_id": "2371",
+    "seller_user_email": "seller@gmail.com",
+    "$transaction_id": "573050",
+    "$payment_method": {
+        "$payment_type": "$credit_card",
+        "$payment_gateway": "$braintree",
+        "$card_bin": "542486",
+        "$card_last4": "4444"
+    },
+    "$currency_code": "USD",
+    "$amount": 15230000,
+}
+
+try:
+    response = client.track("$transaction", properties, return_score=True, include_score_percentiles=True, abuse_types=["promotion_abuse", "content_abuse", "payment_abuse"])
+    if response.is_ok():
+        score_response = response.body["score_response"]
+        print(score_response)
+except sift.client.ApiException:
+    # request failed
+    pass
+
 # Request a score for the user with user_id 23056
 try:
     response = client.score(user_id)
     s = json.dumps(response.body)
     print s
 
 except sift.client.ApiException:
@@ -173,26 +200,79 @@
 
 # Get the latest decisions for a piece of content
 try:
     response = client.get_content_decisions('example_user', 'example_content')
 except sift.client.ApiException:
     # request failed
     pass
-```
 
+# The send call triggers the generation of a OTP code that is stored by Sift and email/sms the code to the user.
+send_properties = {
+	"$user_id": "billy_jones_301",
+	"$send_to": "billy_jones_301@gmail.com",
+	"$verification_type": "$email",
+	"$brand_name": "MyTopBrand",
+	"$language": "en",
+	"$site_country": "IN",
+	"$event": {
+		"$session_id": "SOME_SESSION_ID",
+		"$verified_event": "$login",
+		"$verified_entity_id": "SOME_SESSION_ID",
+		"$reason": "$automated_rule",
+		"$ip": "192.168.1.1",
+		"$browser": {
+			"$user_agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_12_3) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/56.0.2924.87 Safari/537.36"
+		}
+	}
+}
+try:
+    response = client.verification_send(send_properties)
+except sift.client.ApiException:
+    # request failed
+    pass
+
+# The resend call generates a new OTP and sends it to the original recipient with the same settings.
+resend_properties = {
+	"$user_id": "billy_jones_301",
+	"$verified_event": "$login",
+	"$verified_entity_id": "SOME_SESSION_ID"
+}
+try:
+    response = client.verification_resend(resend_properties)
+except sift.client.ApiException:
+    # request failed
+    pass
+
+# The check call is used for verifying the OTP provided by the end user to Sift.
+check_properties = {
+	"$user_id": "billy_jones_301",
+    "$code": 123456,
+	"$verified_event": "$login",
+	"$verified_entity_id": "SOME_SESSION_ID"
+}
+try:
+    response = client.verification_check(check_properties)
+except sift.client.ApiException:
+    # request failed
+    pass
+
+```
 
 ## Testing
 
 Before submitting a change, make sure the following commands run without
 errors from the root dir of the repository:
 
     python -m unittest discover
     python3 -m unittest discover
 
 
+5.4.0 2023-07-26
+- Support for Verification API
+
 5.3.0 2023-02-03
 - Added support for score_percentiles
 
 5.2.0 2022-11-07
 - Update  PSP Merchant Management API
 
 5.1.0 2022-06-22
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `Sift-5.3.0/Sift.egg-info/PKG-INFO` & `Sift-5.4.0/Sift.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Sift
-Version: 5.3.0
+Version: 5.4.0
 Summary: Python bindings for Sift Science's API
 Home-page: https://siftscience.com
 Author: Sift Science
 Author-email: support@siftscience.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
@@ -109,14 +109,41 @@
     response = client.track("$transaction", properties)
     if response.is_ok():
         print "Successfully tracked event"
 except sift.client.ApiException:
     # request failed
     pass
 
+# Track a transaсtion event and receive a score with percentiles in response (sync flow).
+# Note: `return_score` or `return_workflow_status` must be set `True`.
+properties = {
+    "$user_id": user_id,
+    "$user_email": "buyer@gmail.com",
+    "$seller_user_id": "2371",
+    "seller_user_email": "seller@gmail.com",
+    "$transaction_id": "573050",
+    "$payment_method": {
+        "$payment_type": "$credit_card",
+        "$payment_gateway": "$braintree",
+        "$card_bin": "542486",
+        "$card_last4": "4444"
+    },
+    "$currency_code": "USD",
+    "$amount": 15230000,
+}
+
+try:
+    response = client.track("$transaction", properties, return_score=True, include_score_percentiles=True, abuse_types=["promotion_abuse", "content_abuse", "payment_abuse"])
+    if response.is_ok():
+        score_response = response.body["score_response"]
+        print(score_response)
+except sift.client.ApiException:
+    # request failed
+    pass
+
 # Request a score for the user with user_id 23056
 try:
     response = client.score(user_id)
     s = json.dumps(response.body)
     print s
 
 except sift.client.ApiException:
@@ -173,26 +200,79 @@
 
 # Get the latest decisions for a piece of content
 try:
     response = client.get_content_decisions('example_user', 'example_content')
 except sift.client.ApiException:
     # request failed
     pass
-```
 
+# The send call triggers the generation of a OTP code that is stored by Sift and email/sms the code to the user.
+send_properties = {
+	"$user_id": "billy_jones_301",
+	"$send_to": "billy_jones_301@gmail.com",
+	"$verification_type": "$email",
+	"$brand_name": "MyTopBrand",
+	"$language": "en",
+	"$site_country": "IN",
+	"$event": {
+		"$session_id": "SOME_SESSION_ID",
+		"$verified_event": "$login",
+		"$verified_entity_id": "SOME_SESSION_ID",
+		"$reason": "$automated_rule",
+		"$ip": "192.168.1.1",
+		"$browser": {
+			"$user_agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_12_3) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/56.0.2924.87 Safari/537.36"
+		}
+	}
+}
+try:
+    response = client.verification_send(send_properties)
+except sift.client.ApiException:
+    # request failed
+    pass
+
+# The resend call generates a new OTP and sends it to the original recipient with the same settings.
+resend_properties = {
+	"$user_id": "billy_jones_301",
+	"$verified_event": "$login",
+	"$verified_entity_id": "SOME_SESSION_ID"
+}
+try:
+    response = client.verification_resend(resend_properties)
+except sift.client.ApiException:
+    # request failed
+    pass
+
+# The check call is used for verifying the OTP provided by the end user to Sift.
+check_properties = {
+	"$user_id": "billy_jones_301",
+    "$code": 123456,
+	"$verified_event": "$login",
+	"$verified_entity_id": "SOME_SESSION_ID"
+}
+try:
+    response = client.verification_check(check_properties)
+except sift.client.ApiException:
+    # request failed
+    pass
+
+```
 
 ## Testing
 
 Before submitting a change, make sure the following commands run without
 errors from the root dir of the repository:
 
     python -m unittest discover
     python3 -m unittest discover
 
 
+5.4.0 2023-07-26
+- Support for Verification API
+
 5.3.0 2023-02-03
 - Added support for score_percentiles
 
 5.2.0 2022-11-07
 - Update  PSP Merchant Management API
 
 5.1.0 2022-06-22
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `Sift-5.3.0/setup.py` & `Sift-5.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `Sift-5.3.0/sift/client.py` & `Sift-5.4.0/sift/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,14 +18,16 @@
     _UNICODE_STRING = str
 
 import sift
 import sift.version
 
 API_URL = 'https://api.siftscience.com'
 API3_URL = 'https://api3.siftscience.com'
+API_URL_VERIFICATION = 'https://api.sift.com/v1/verification/'
+
 DECISION_SOURCES = ['MANUAL_REVIEW', 'AUTOMATED_RULE', 'CHARGEBACK']
 
 
 def _quote_path(s):
     # by default, urllib.quote doesn't escape forward slash; pass the
     # optional arg to override this
     return urllib.parse.quote(s, '')
@@ -176,15 +178,14 @@
 
         if force_workflow_run:
             params['force_workflow_run'] = 'true'
 
         if include_score_percentiles:
             field_types = ['SCORE_PERCENTILES']
             params['fields'] = ','.join(field_types)
-
         try:
             response = self.session.post(
                 path,
                 data=json.dumps(properties, cls=DecimalEncoder),
                 headers=headers,
                 timeout=timeout,
                 params=params)
@@ -481,15 +482,14 @@
         """
 
         if timeout is None:
             timeout = self.timeout
 
         self._validate_apply_decision_request(properties, user_id)
         url = self._user_decisions_url(self.account_id, user_id)
-
         try:
             return Response(self.session.post(
                 url,
                 data=json.dumps(properties),
                 auth=requests.auth.HTTPBasicAuth(self.api_key, ''),
                 headers={'Content-type': 'application/json',
                          'Accept': '*/*',
@@ -520,15 +520,14 @@
 
         _assert_non_empty_unicode(user_id, 'user_id')
         _assert_non_empty_unicode(order_id, 'order_id')
 
         self._validate_apply_decision_request(properties, user_id)
 
         url = self._order_apply_decisions_url(self.account_id, user_id, order_id)
-
         try:
             return Response(self.session.post(
                 url,
                 data=json.dumps(properties),
                 auth=requests.auth.HTTPBasicAuth(self.api_key, ''),
                 headers={'Content-type': 'application/json',
                          'Accept': '*/*',
@@ -784,15 +783,14 @@
             A sift.client.Response object if the call succeeded, else raises an ApiException
         """
 
         if timeout is None:
             timeout = self.timeout
 
         url = self._psp_merchant_id_url(self.account_id, merchant_id)
-
         try:
             return Response(self.session.put(
                 url,
                 data=json.dumps(properties),
                 auth=requests.auth.HTTPBasicAuth(self.api_key, ''),
                 headers={'Content-type': 'application/json',
                          'Accept': '*/*',
@@ -850,14 +848,204 @@
                 url,
                 auth=requests.auth.HTTPBasicAuth(self.api_key, ''),
                 headers={'User-Agent': self._user_agent()},
                 timeout=timeout))
         except requests.exceptions.RequestException as e:
             raise ApiException(str(e), url)
 
+    def verification_send(self, properties, timeout=None,  version=None):
+        """The send call triggers the generation of a OTP code that is stored by Sift and email/sms the code to the user.
+        This call is blocking. Check out https://sift.com/developers/docs/python/verification-api/send
+        for more information on our send response structure.
+
+        Args:
+
+            properties: 
+
+                $user_id: User ID of user being verified, e.g. johndoe123.
+                $send_to: The phone / email to send the OTP to.
+                $verification_type: The channel used for verification. Should be either $email or $sms.
+                $brand_name(optional): Name of the brand of product or service the user interacts with.
+                $language(optional): Language of the content of the web site.
+                $site_country(optional): Country of the content of the site.
+                $event: 
+                    $session_id:  The session being verified. See $verification in the Sift Events API documentation.
+                    $verified_event: The type of the reserved event being verified.
+                    $reason(optional): The trigger for the verification. See $verification in the Sift Events API documentation.
+                    $ip(optional): The user's IP address.
+                    $browser:
+                        $user_agent: The user agent of the browser that is verifying. Represented by the $browser object.
+                                     Use this field if the client is a browser.
+
+
+            timeout(optional): Use a custom timeout (in seconds) for this call.
+
+            version(optional): Use a different version of the Sift Science API for this call.
+
+        Returns:
+            A sift.client.Response object if the send call succeeded, or raises an ApiException.
+        """
+
+        if timeout is None:
+            timeout = self.timeout
+
+        self._validate_send_request(properties)
+
+        url = self._verification_send_url()
+
+        try:
+            return Response(self.session.post(
+                url,
+                data=json.dumps(properties),
+                auth=requests.auth.HTTPBasicAuth(self.api_key, ''),
+                headers={'Content-type': 'application/json',
+                         'Accept': '*/*',
+                         'User-Agent': self._user_agent()},
+                timeout=timeout))
+
+        except requests.exceptions.RequestException as e:
+            raise ApiException(str(e), url)  
+
+    def _validate_send_request(self, properties):
+        """ This method is used to validate arguments passed to the send method. """
+
+        if not isinstance(properties, dict):
+            raise TypeError("properties must be a dict")
+        elif not properties:
+            raise ValueError("properties dictionary may not be empty")
+
+        user_id = properties.get('$user_id')
+        _assert_non_empty_unicode(user_id, 'user_id', error_cls=ValueError)
+
+        send_to = properties.get('$send_to')
+        _assert_non_empty_unicode(send_to, 'send_to', error_cls=ValueError)
+
+        verification_type = properties.get('$verification_type')
+        _assert_non_empty_unicode(
+            verification_type, 'verification_type', error_cls=ValueError)
+
+        event = properties.get('$event')
+        if not isinstance(event, dict):
+            raise TypeError("$event must be a dict")
+        elif not event:
+            raise ValueError("$event dictionary may not be empty")
+
+        session_id = event.get('$session_id')
+        _assert_non_empty_unicode(
+            session_id, 'session_id', error_cls=ValueError)
+    
+    def verification_resend(self, properties, timeout=None,  version=None):
+        """A user can ask for a new OTP (one-time password) if they haven't received the previous one,
+        or in case the previous OTP expired.
+        This call is blocking. Check out https://sift.com/developers/docs/python/verification-api/resend
+        for more information on our send response structure.
+
+        Args:
+
+            properties: 
+
+                $user_id: User ID of user being verified, e.g. johndoe123.
+                $verified_event(optional): This will be the event type that triggered the verification.
+                $verified_entity_id(optional): The ID of the entity impacted by the event being verified.
+
+            timeout(optional): Use a custom timeout (in seconds) for this call.
+
+            version(optional): Use a different version of the Sift Science API for this call.
+
+        Returns:
+            A sift.client.Response object if the send call succeeded, or raises an ApiException.
+        """
+
+        if timeout is None:
+            timeout = self.timeout
+
+        self._validate_resend_request(properties)
+
+        url = self._verification_resend_url()
+
+        try:
+            return Response(self.session.post(
+                url,
+                data=json.dumps(properties),
+                auth=requests.auth.HTTPBasicAuth(self.api_key, ''),
+                headers={'Content-type': 'application/json',
+                         'Accept': '*/*',
+                         'User-Agent': self._user_agent()},
+                timeout=timeout))
+
+        except requests.exceptions.RequestException as e:
+            raise ApiException(str(e), url)  
+
+    def _validate_resend_request(self, properties):
+        """ This method is used to validate arguments passed to the send method. """
+
+        if not isinstance(properties, dict):
+            raise TypeError("properties must be a dict")
+        elif not properties:
+            raise ValueError("properties dictionary may not be empty")
+
+        user_id = properties.get('$user_id')
+        _assert_non_empty_unicode(user_id, 'user_id', error_cls=ValueError)
+    
+    def verification_check(self, properties, timeout=None,  version=None):
+            """The verification_check call is used for checking the OTP provided by the end user to Sift. 
+            Sift then compares the OTP, checks rate limits and responds with a decision whether the user should be able to proceed or not.
+            This call is blocking. Check out https://sift.com/developers/docs/python/verification-api/check
+            for more information on our check response structure.
+
+            Args:
+
+                properties:
+                    $user_id: User ID of user being verified, e.g. johndoe123.
+                    $code: The code the user sent to the customer for validation..
+                    $verified_event(optional): This will be the event type that triggered the verification. 
+                    $verified_entity_id(optional): The ID of the entity impacted by the event being verified.
+
+                timeout(optional): Use a custom timeout (in seconds) for this call.
+                version(optional): Use a different version of the Sift Science API for this call.
+
+            Returns:
+                A sift.client.Response object if the check call succeeded, or raises
+                an ApiException.
+            """
+            if timeout is None:
+                timeout = self.timeout
+
+            self._validate_check_request(properties)
+
+            url = self._verification_check_url()
+
+            try:
+                return Response(self.session.post(
+                    url,
+                    data=json.dumps(properties),
+                    auth=requests.auth.HTTPBasicAuth(self.api_key, ''),
+                    headers={'Content-type': 'application/json',
+                            'Accept': '*/*',
+                            'User-Agent': self._user_agent()},
+                    timeout=timeout))
+
+            except requests.exceptions.RequestException as e:
+                raise ApiException(str(e), url)
+
+    def _validate_check_request(self, properties):
+        """ This method is used to validate arguments passed to the check method. """
+
+        if not isinstance(properties, dict):
+            raise TypeError("properties must be a dict")
+        elif not properties:
+            raise ValueError("properties dictionary may not be empty")
+
+        user_id = properties.get('$user_id')
+        _assert_non_empty_unicode(user_id, 'user_id', error_cls=ValueError)
+
+        otp_code = properties.get('$code')
+        if otp_code is None:
+            raise ValueError("code is required")
+  
     def _user_agent(self):
         return 'SiftScience/v%s sift-python/%s' % (sift.version.API_VERSION, sift.version.VERSION)
 
     def _event_url(self, version):
         return self.url + '/v%s/events' % version
 
     def _score_url(self, user_id, version):
@@ -908,14 +1096,22 @@
         return (self.url + '/v3/accounts/%s/psp_management/merchants' %
                 (_quote_path(account_id)))
 
     def _psp_merchant_id_url(self, account_id, merchant_id):
         return (self.url + '/v3/accounts/%s/psp_management/merchants/%s' %
                 (_quote_path(account_id), _quote_path(merchant_id)))
 
+    def _verification_send_url(self):
+        return (API_URL_VERIFICATION + 'send')
+    
+    def _verification_resend_url(self):
+        return (API_URL_VERIFICATION + 'resend')
+    
+    def _verification_check_url(self):
+        return (API_URL_VERIFICATION + 'check')
 
 class Response(object):
     HTTP_CODES_WITHOUT_BODY = [204, 304]
 
     def __init__(self, http_response):
         """
         Raises ApiException on invalid JSON in Response body or non-2XX HTTP
```

