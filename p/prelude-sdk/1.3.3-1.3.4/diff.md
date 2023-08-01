# Comparing `tmp/prelude-sdk-1.3.3.tar.gz` & `tmp/prelude-sdk-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prelude-sdk-1.3.3.tar", last modified: Mon Jul 31 17:21:38 2023, max compression
+gzip compressed data, was "prelude-sdk-1.3.4.tar", last modified: Tue Aug  1 15:17:51 2023, max compression
```

## Comparing `prelude-sdk-1.3.3.tar` & `prelude-sdk-1.3.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-07-31 17:21:38.163368 prelude-sdk-1.3.3/
--rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude-sdk-1.3.3/LICENSE
--rw-r--r--   0 pack       (501) staff       (20)     1139 2023-07-31 17:21:38.163431 prelude-sdk-1.3.3/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      697 2023-04-11 22:16:02.000000 prelude-sdk-1.3.3/README.md
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-07-31 17:21:38.159266 prelude-sdk-1.3.3/prelude_sdk/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-1.3.3/prelude_sdk/__init__.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-07-31 17:21:38.161151 prelude-sdk-1.3.3/prelude_sdk/controllers/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-1.3.3/prelude_sdk/controllers/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     2484 2023-07-26 15:41:33.000000 prelude-sdk-1.3.3/prelude_sdk/controllers/build_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     5566 2023-07-26 15:41:33.000000 prelude-sdk-1.3.3/prelude_sdk/controllers/detect_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     3731 2023-07-26 15:41:33.000000 prelude-sdk-1.3.3/prelude_sdk/controllers/iam_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     2113 2023-07-31 17:07:15.000000 prelude-sdk-1.3.3/prelude_sdk/controllers/partner_controller.py
--rw-r--r--   0 pack       (501) staff       (20)      443 2023-05-03 13:30:52.000000 prelude-sdk-1.3.3/prelude_sdk/controllers/probe_controller.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-07-31 17:21:38.161721 prelude-sdk-1.3.3/prelude_sdk/models/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-1.3.3/prelude_sdk/models/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     2816 2023-07-11 13:50:29.000000 prelude-sdk-1.3.3/prelude_sdk/models/account.py
--rw-r--r--   0 pack       (501) staff       (20)     3508 2023-07-31 17:07:15.000000 prelude-sdk-1.3.3/prelude_sdk/models/codes.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-07-31 17:21:38.159876 prelude-sdk-1.3.3/prelude_sdk.egg-info/
--rw-r--r--   0 pack       (501) staff       (20)     1139 2023-07-31 17:21:38.000000 prelude-sdk-1.3.3/prelude_sdk.egg-info/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      773 2023-07-31 17:21:38.000000 prelude-sdk-1.3.3/prelude_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 pack       (501) staff       (20)        1 2023-07-31 17:21:38.000000 prelude-sdk-1.3.3/prelude_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 pack       (501) staff       (20)        9 2023-07-31 17:21:38.000000 prelude-sdk-1.3.3/prelude_sdk.egg-info/requires.txt
--rw-r--r--   0 pack       (501) staff       (20)       18 2023-07-31 17:21:38.000000 prelude-sdk-1.3.3/prelude_sdk.egg-info/top_level.txt
--rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude-sdk-1.3.3/pyproject.toml
--rw-r--r--   0 pack       (501) staff       (20)      532 2023-07-31 17:21:38.163663 prelude-sdk-1.3.3/setup.cfg
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-07-31 17:21:38.163082 prelude-sdk-1.3.3/tests/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-04-07 19:23:14.000000 prelude-sdk-1.3.3/tests/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     1097 2023-05-17 16:29:25.000000 prelude-sdk-1.3.3/tests/conftest.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-07-31 17:21:38.163283 prelude-sdk-1.3.3/tests/templates/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-04-07 19:23:14.000000 prelude-sdk-1.3.3/tests/templates/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     2075 2023-06-06 22:22:58.000000 prelude-sdk-1.3.3/tests/test_build_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     5045 2023-06-06 22:22:58.000000 prelude-sdk-1.3.3/tests/test_detect_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     3350 2023-06-07 19:10:37.000000 prelude-sdk-1.3.3/tests/test_iam_controller.py
--rw-r--r--   0 pack       (501) staff       (20)      682 2023-04-07 19:23:14.000000 prelude-sdk-1.3.3/tests/test_probe_controller.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-08-01 15:17:51.503397 prelude-sdk-1.3.4/
+-rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude-sdk-1.3.4/LICENSE
+-rw-r--r--   0 pack       (501) staff       (20)     1139 2023-08-01 15:17:51.503448 prelude-sdk-1.3.4/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      697 2023-04-11 22:16:02.000000 prelude-sdk-1.3.4/README.md
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-08-01 15:17:51.497575 prelude-sdk-1.3.4/prelude_sdk/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-1.3.4/prelude_sdk/__init__.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-08-01 15:17:51.500501 prelude-sdk-1.3.4/prelude_sdk/controllers/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-1.3.4/prelude_sdk/controllers/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     2484 2023-07-26 15:41:33.000000 prelude-sdk-1.3.4/prelude_sdk/controllers/build_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     5566 2023-07-26 15:41:33.000000 prelude-sdk-1.3.4/prelude_sdk/controllers/detect_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     3731 2023-07-26 15:41:33.000000 prelude-sdk-1.3.4/prelude_sdk/controllers/iam_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     2113 2023-07-31 17:07:15.000000 prelude-sdk-1.3.4/prelude_sdk/controllers/partner_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)      443 2023-05-03 13:30:52.000000 prelude-sdk-1.3.4/prelude_sdk/controllers/probe_controller.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-08-01 15:17:51.501308 prelude-sdk-1.3.4/prelude_sdk/models/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-1.3.4/prelude_sdk/models/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     2816 2023-07-11 13:50:29.000000 prelude-sdk-1.3.4/prelude_sdk/models/account.py
+-rw-r--r--   0 pack       (501) staff       (20)     3627 2023-08-01 15:12:48.000000 prelude-sdk-1.3.4/prelude_sdk/models/codes.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-08-01 15:17:51.498106 prelude-sdk-1.3.4/prelude_sdk.egg-info/
+-rw-r--r--   0 pack       (501) staff       (20)     1139 2023-08-01 15:17:51.000000 prelude-sdk-1.3.4/prelude_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      773 2023-08-01 15:17:51.000000 prelude-sdk-1.3.4/prelude_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 pack       (501) staff       (20)        1 2023-08-01 15:17:51.000000 prelude-sdk-1.3.4/prelude_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 pack       (501) staff       (20)        9 2023-08-01 15:17:51.000000 prelude-sdk-1.3.4/prelude_sdk.egg-info/requires.txt
+-rw-r--r--   0 pack       (501) staff       (20)       18 2023-08-01 15:17:51.000000 prelude-sdk-1.3.4/prelude_sdk.egg-info/top_level.txt
+-rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude-sdk-1.3.4/pyproject.toml
+-rw-r--r--   0 pack       (501) staff       (20)      532 2023-08-01 15:17:51.503663 prelude-sdk-1.3.4/setup.cfg
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-08-01 15:17:51.503075 prelude-sdk-1.3.4/tests/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-04-07 19:23:14.000000 prelude-sdk-1.3.4/tests/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     1097 2023-05-17 16:29:25.000000 prelude-sdk-1.3.4/tests/conftest.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-08-01 15:17:51.503295 prelude-sdk-1.3.4/tests/templates/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-04-07 19:23:14.000000 prelude-sdk-1.3.4/tests/templates/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     2075 2023-06-06 22:22:58.000000 prelude-sdk-1.3.4/tests/test_build_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     5045 2023-06-06 22:22:58.000000 prelude-sdk-1.3.4/tests/test_detect_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     3350 2023-06-07 19:10:37.000000 prelude-sdk-1.3.4/tests/test_iam_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)      682 2023-04-07 19:23:14.000000 prelude-sdk-1.3.4/tests/test_probe_controller.py
```

### Comparing `prelude-sdk-1.3.3/LICENSE` & `prelude-sdk-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.3.3/PKG-INFO` & `prelude-sdk-1.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prelude-sdk
-Version: 1.3.3
+Version: 1.3.4
 Summary: For interacting with the Prelude API
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `prelude-sdk-1.3.3/README.md` & `prelude-sdk-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.3.3/prelude_sdk/controllers/build_controller.py` & `prelude-sdk-1.3.4/prelude_sdk/controllers/build_controller.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.3.3/prelude_sdk/controllers/detect_controller.py` & `prelude-sdk-1.3.4/prelude_sdk/controllers/detect_controller.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.3.3/prelude_sdk/controllers/iam_controller.py` & `prelude-sdk-1.3.4/prelude_sdk/controllers/iam_controller.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.3.3/prelude_sdk/controllers/partner_controller.py` & `prelude-sdk-1.3.4/prelude_sdk/controllers/partner_controller.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.3.3/prelude_sdk/models/account.py` & `prelude-sdk-1.3.4/prelude_sdk/models/account.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.3.3/prelude_sdk/models/codes.py` & `prelude-sdk-1.3.4/prelude_sdk/models/codes.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import logging
+
 from enum import Enum
 
 
 class RunCode(Enum):
     INVALID = -1
     DEBUG = 0
     DAILY = 1
@@ -41,28 +43,28 @@
         return Permission.INVALID
 
 
 class ExitCode(Enum):
     MISSING = -1
     UNKNOWN_ERROR = 1
     MALFORMED_TEST = 2
-    BEHAVIOR_PREVENTED_1 = 9
-    BEHAVIOR_PREVENTED_2 = 15
-    CHECK_COMPLETED = 100
-    NOT_PREVENTED = 101
+    PROCESS_BLOCKED = 9
+    PROCESS_BLOCKED_GRACEFULLY = 15
+    PROTECTED = 100
+    UNPROTECTED = 101
     TIMED_OUT = 102
     FAILED_CLEANUP = 103
-    NOT_RELEVANT = 104
-    SIGNATURE_PREVENTED_1 = 105
+    TEST_NOT_RELEVANT = 104
+    DYNAMIC_QUARANTINE = 105
     BLOCKED_AT_PERIMETER = 106
-    BEHAVIOR_PREVENTED_3 = 107
-    TEST_UNAVAILABLE = 108
-    INCORRECTLY_BLOCKED = 110
-    BEHAVIOR_PREVENTED_4 = 126
-    SIGNATURE_PREVENTED_2 = 127
+    EXPLOIT_PREVENTED = 107
+    ENDPOINT_NOT_RELEVANT = 108
+    FALSE_POSITIVE = 110
+    TEST_DISALLOWED = 126
+    STATIC_QUARANTINE = 127
     OUT_OF_MEMORY = 137
     UNEXPECTED_ERROR = 256
 
     @classmethod
     def _missing_(cls, value):
         if value and not isinstance(value, int):
             return cls(int(value))
@@ -72,16 +74,16 @@
     def state(self):
         for k, v in State.mapping().items():
             if self in v:
                 return k
         return State.NONE
 
     def transform(self, test):
-        if test.unit == 'health' and self != ExitCode.CHECK_COMPLETED:
-            return ExitCode.INCORRECTLY_BLOCKED
+        if test.unit == 'health' and self != ExitCode.PROTECTED:
+            return ExitCode.FALSE_POSITIVE
         return self
 
 
 class State(Enum):
     NONE = 0
     PROTECTED = 1
     UNPROTECTED = 2
@@ -89,40 +91,40 @@
     NOT_RELEVANT = 4
 
     @classmethod
     def mapping(cls):
         return {
             State.NONE: [ExitCode.MISSING],
             State.PROTECTED: [
-                ExitCode.BEHAVIOR_PREVENTED_1,
-                ExitCode.BEHAVIOR_PREVENTED_2,
-                ExitCode.CHECK_COMPLETED,
-                ExitCode.NOT_RELEVANT,
-                ExitCode.SIGNATURE_PREVENTED_1,
+                ExitCode.PROCESS_BLOCKED,
+                ExitCode.PROCESS_BLOCKED_GRACEFULLY,
+                ExitCode.PROTECTED,
+                ExitCode.DYNAMIC_QUARANTINE,
                 ExitCode.BLOCKED_AT_PERIMETER,
-                ExitCode.BEHAVIOR_PREVENTED_3,
-                ExitCode.TEST_UNAVAILABLE,
-                ExitCode.BEHAVIOR_PREVENTED_4,
-                ExitCode.SIGNATURE_PREVENTED_2
+                ExitCode.EXPLOIT_PREVENTED,
+                ExitCode.TEST_DISALLOWED,
+                ExitCode.STATIC_QUARANTINE,
+                ExitCode.TEST_NOT_RELEVANT,
+                ExitCode.ENDPOINT_NOT_RELEVANT
             ],
             State.UNPROTECTED: [
-                ExitCode.NOT_PREVENTED,
+                ExitCode.UNPROTECTED,
+                ExitCode.FALSE_POSITIVE,
             ],
             State.ERROR: [
                 ExitCode.UNKNOWN_ERROR,
                 ExitCode.MALFORMED_TEST,
                 ExitCode.TIMED_OUT,
                 ExitCode.FAILED_CLEANUP,
-                ExitCode.INCORRECTLY_BLOCKED,
                 ExitCode.OUT_OF_MEMORY,
                 ExitCode.UNEXPECTED_ERROR
             ],
             State.NOT_RELEVANT: [
-                ExitCode.NOT_RELEVANT,
-                ExitCode.TEST_UNAVAILABLE
+                ExitCode.TEST_NOT_RELEVANT,
+                ExitCode.ENDPOINT_NOT_RELEVANT
             ]
         }
 
 
 class DOS(Enum):
     none = 'none'
     arm64 = 'arm64'
@@ -144,8 +146,13 @@
     INVALID = 0
     CROWDSTRIKE = 1
     DEFENDER = 2
     SPLUNK = 3
 
     @classmethod
     def _missing_(cls, value):
+        logging.error('Unknown control requested: %s', value)
         return Control.INVALID
+
+    @property
+    def is_siem(self):
+        return self == Control.SPLUNK
```

### Comparing `prelude-sdk-1.3.3/prelude_sdk.egg-info/PKG-INFO` & `prelude-sdk-1.3.4/prelude_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prelude-sdk
-Version: 1.3.3
+Version: 1.3.4
 Summary: For interacting with the Prelude API
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `prelude-sdk-1.3.3/prelude_sdk.egg-info/SOURCES.txt` & `prelude-sdk-1.3.4/prelude_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.3.3/setup.cfg` & `prelude-sdk-1.3.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = prelude-sdk
-version = 1.3.3
+version = 1.3.4
 author = Prelude Research
 author_email = support@preludesecurity.com
 description = For interacting with the Prelude API
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/preludeorg
 classifiers =
```

### Comparing `prelude-sdk-1.3.3/tests/conftest.py` & `prelude-sdk-1.3.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.3.3/tests/test_build_controller.py` & `prelude-sdk-1.3.4/tests/test_build_controller.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.3.3/tests/test_detect_controller.py` & `prelude-sdk-1.3.4/tests/test_detect_controller.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.3.3/tests/test_iam_controller.py` & `prelude-sdk-1.3.4/tests/test_iam_controller.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.3.3/tests/test_probe_controller.py` & `prelude-sdk-1.3.4/tests/test_probe_controller.py`

 * *Files identical despite different names*

