# Comparing `tmp/screenshotone-0.0.4.tar.gz` & `tmp/screenshotone-0.0.5.tar.gz`

## Comparing `screenshotone-0.0.4.tar` & `screenshotone-0.0.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 screenshotone-0.0.4/.github/workflows/pypi-release.yml
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 screenshotone-0.0.4/src/screenshotone/__init__.py
--rw-r--r--   0        0        0     7591 2020-02-02 00:00:00.000000 screenshotone-0.0.4/src/screenshotone/sdk.py
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 screenshotone-0.0.4/LICENSE
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 screenshotone-0.0.4/README.md
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 screenshotone-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 screenshotone-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 screenshotone-0.0.5/.github/workflows/pypi-release.yml
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 screenshotone-0.0.5/src/screenshotone/__init__.py
+-rw-r--r--   0        0        0     8396 2020-02-02 00:00:00.000000 screenshotone-0.0.5/src/screenshotone/sdk.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 screenshotone-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 screenshotone-0.0.5/README.md
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 screenshotone-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 screenshotone-0.0.5/PKG-INFO
```

### Comparing `screenshotone-0.0.4/.github/workflows/pypi-release.yml` & `screenshotone-0.0.5/.github/workflows/pypi-release.yml`

 * *Files identical despite different names*

### Comparing `screenshotone-0.0.4/src/screenshotone/sdk.py` & `screenshotone-0.0.5/src/screenshotone/sdk.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,19 @@
 import hmac
 import hashlib
 import requests
 
 API_BASE_URL = 'https://api.screenshotone.com'
 API_TAKE_PATH = '/take'
 
+class InvalidRequestException(Exception):
+    pass
+class APIErrorException(Exception):
+    pass
+
 class TakeOptions: 
     options = OrderedDict()    
 
     def __init__(self, defaults):
         for key, value in defaults.items(): 
             self.options[key] = value    
 
@@ -328,9 +333,21 @@
         query['access_key'] = self.access_key
 
         url = '%s%s' % (API_BASE_URL, API_TAKE_PATH)
         r = requests.post(url, json=query, stream=True)
         
         if r.status_code == 200: 
             return r.raw
+        elif r.status_code == 400:
+            error_response = json.loads(r.text)
+            if not error_response.get('is_successful'):
+                error_messages = [detail['message'] for detail in error_response.get('error_details', [])]
+                error_message = f"Error: {error_response.get('error_message', 'Unknown error')}\n"
+                error_message += "\n".join(error_messages)
+
+                raise InvalidRequestException(error_message)
+        else:
+            # Handle other error status codes with a generic message
+            error_message = f"An error occurred while processing the request. Status code: {r.status_code}"
+            raise APIErrorException(error_message)
 
         return None
```

### Comparing `screenshotone-0.0.4/LICENSE` & `screenshotone-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `screenshotone-0.0.4/README.md` & `screenshotone-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `screenshotone-0.0.4/pyproject.toml` & `screenshotone-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "screenshotone"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Dmytro Krasun", email="support@screenshotone.com" },
 ]
 dependencies = [
     "requests >= 2.28.1"
 ]
 description = "A Python SDK for ScreenshotOne.com API to take screenshots of URLs, render HTML as images and PDF"
```

### Comparing `screenshotone-0.0.4/PKG-INFO` & `screenshotone-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: screenshotone
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Python SDK for ScreenshotOne.com API to take screenshots of URLs, render HTML as images and PDF
 Project-URL: Homepage, https://screenshotone.com/
 Project-URL: Docs, https://screenshotone.com/docs/getting-started/
 Author-email: Dmytro Krasun <support@screenshotone.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

