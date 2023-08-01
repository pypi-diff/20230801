# Comparing `tmp/screenshotone-0.0.5.tar.gz` & `tmp/screenshotone-0.0.6.tar.gz`

## Comparing `screenshotone-0.0.5.tar` & `screenshotone-0.0.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 screenshotone-0.0.5/.github/workflows/pypi-release.yml
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 screenshotone-0.0.5/src/screenshotone/__init__.py
--rw-r--r--   0        0        0     8396 2020-02-02 00:00:00.000000 screenshotone-0.0.5/src/screenshotone/sdk.py
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 screenshotone-0.0.5/LICENSE
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 screenshotone-0.0.5/README.md
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 screenshotone-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 screenshotone-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 screenshotone-0.0.6/.github/workflows/pypi-release.yml
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 screenshotone-0.0.6/src/screenshotone/__init__.py
+-rw-r--r--   0        0        0     8408 2020-02-02 00:00:00.000000 screenshotone-0.0.6/src/screenshotone/sdk.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 screenshotone-0.0.6/LICENSE
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 screenshotone-0.0.6/README.md
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 screenshotone-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 screenshotone-0.0.6/PKG-INFO
```

### Comparing `screenshotone-0.0.5/.github/workflows/pypi-release.yml` & `screenshotone-0.0.6/.github/workflows/pypi-release.yml`

 * *Files identical despite different names*

### Comparing `screenshotone-0.0.5/src/screenshotone/sdk.py` & `screenshotone-0.0.6/src/screenshotone/sdk.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from collections import OrderedDict
 from typing import List
 import urllib.parse
 import hmac
 import hashlib
 import requests
+import json
 
 API_BASE_URL = 'https://api.screenshotone.com'
 API_TAKE_PATH = '/take'
 
 class InvalidRequestException(Exception):
     pass
 class APIErrorException(Exception):
```

### Comparing `screenshotone-0.0.5/LICENSE` & `screenshotone-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `screenshotone-0.0.5/README.md` & `screenshotone-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `screenshotone-0.0.5/pyproject.toml` & `screenshotone-0.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "screenshotone"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Dmytro Krasun", email="support@screenshotone.com" },
 ]
 dependencies = [
     "requests >= 2.28.1"
 ]
 description = "A Python SDK for ScreenshotOne.com API to take screenshots of URLs, render HTML as images and PDF"
```

### Comparing `screenshotone-0.0.5/PKG-INFO` & `screenshotone-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: screenshotone
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Python SDK for ScreenshotOne.com API to take screenshots of URLs, render HTML as images and PDF
 Project-URL: Homepage, https://screenshotone.com/
 Project-URL: Docs, https://screenshotone.com/docs/getting-started/
 Author-email: Dmytro Krasun <support@screenshotone.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

