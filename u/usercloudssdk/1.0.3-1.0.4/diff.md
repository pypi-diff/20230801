# Comparing `tmp/usercloudssdk-1.0.3.tar.gz` & `tmp/usercloudssdk-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usercloudssdk-1.0.3.tar", last modified: Thu Jul 27 19:01:05 2023, max compression
+gzip compressed data, was "usercloudssdk-1.0.4.tar", last modified: Tue Aug  1 19:31:41 2023, max compression
```

## Comparing `usercloudssdk-1.0.3.tar` & `usercloudssdk-1.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 jwang      (501) staff       (20)        0 2023-07-27 19:01:05.584837 usercloudssdk-1.0.3/
--rw-r--r--   0 jwang      (501) staff       (20)     1103 2023-07-27 17:28:09.000000 usercloudssdk-1.0.3/LICENSE
--rw-r--r--   0 jwang      (501) staff       (20)     1507 2023-07-27 19:01:05.584720 usercloudssdk-1.0.3/PKG-INFO
--rw-r--r--   0 jwang      (501) staff       (20)       12 2023-07-27 00:40:23.000000 usercloudssdk-1.0.3/README.md
--rw-r--r--   0 jwang      (501) staff       (20)      634 2023-07-27 19:00:20.000000 usercloudssdk-1.0.3/pyproject.toml
--rw-r--r--   0 jwang      (501) staff       (20)       38 2023-07-27 19:01:05.584873 usercloudssdk-1.0.3/setup.cfg
-drwxr-xr-x   0 jwang      (501) staff       (20)        0 2023-07-27 19:01:05.581624 usercloudssdk-1.0.3/src/
-drwxr-xr-x   0 jwang      (501) staff       (20)        0 2023-07-27 19:01:05.583876 usercloudssdk-1.0.3/src/usercloudssdk/
--rw-r--r--   0 jwang      (501) staff       (20)        0 2023-07-27 13:43:32.000000 usercloudssdk-1.0.3/src/usercloudssdk/__init__.py
--rw-r--r--   0 jwang      (501) staff       (20)    17780 2023-07-27 17:19:10.000000 usercloudssdk-1.0.3/src/usercloudssdk/client.py
--rw-r--r--   0 jwang      (501) staff       (20)      636 2023-07-27 13:43:32.000000 usercloudssdk-1.0.3/src/usercloudssdk/constants.py
--rw-r--r--   0 jwang      (501) staff       (20)    14342 2023-07-27 17:19:10.000000 usercloudssdk-1.0.3/src/usercloudssdk/models.py
--rw-r--r--   0 jwang      (501) staff       (20)      790 2023-07-27 17:19:10.000000 usercloudssdk-1.0.3/src/usercloudssdk/policies.py
--rw-r--r--   0 jwang      (501) staff       (20)     6377 2023-07-27 17:19:10.000000 usercloudssdk-1.0.3/src/usercloudssdk/tokenizer_sample.py
--rw-r--r--   0 jwang      (501) staff       (20)      405 2023-07-27 13:43:32.000000 usercloudssdk-1.0.3/src/usercloudssdk/ucjson.py
--rw-r--r--   0 jwang      (501) staff       (20)    11159 2023-07-27 17:19:10.000000 usercloudssdk-1.0.3/src/usercloudssdk/userstore_sample.py
-drwxr-xr-x   0 jwang      (501) staff       (20)        0 2023-07-27 19:01:05.584581 usercloudssdk-1.0.3/src/usercloudssdk.egg-info/
--rw-r--r--   0 jwang      (501) staff       (20)     1507 2023-07-27 19:01:05.000000 usercloudssdk-1.0.3/src/usercloudssdk.egg-info/PKG-INFO
--rw-r--r--   0 jwang      (501) staff       (20)      487 2023-07-27 19:01:05.000000 usercloudssdk-1.0.3/src/usercloudssdk.egg-info/SOURCES.txt
--rw-r--r--   0 jwang      (501) staff       (20)        1 2023-07-27 19:01:05.000000 usercloudssdk-1.0.3/src/usercloudssdk.egg-info/dependency_links.txt
--rw-r--r--   0 jwang      (501) staff       (20)      166 2023-07-27 19:01:05.000000 usercloudssdk-1.0.3/src/usercloudssdk.egg-info/requires.txt
--rw-r--r--   0 jwang      (501) staff       (20)       14 2023-07-27 19:01:05.000000 usercloudssdk-1.0.3/src/usercloudssdk.egg-info/top_level.txt
+drwxr-xr-x   0 jwang      (501) staff       (20)        0 2023-08-01 19:31:41.316470 usercloudssdk-1.0.4/
+-rw-r--r--   0 jwang      (501) staff       (20)     1103 2023-08-01 19:28:49.000000 usercloudssdk-1.0.4/LICENSE
+-rw-r--r--   0 jwang      (501) staff       (20)     1507 2023-08-01 19:31:41.316332 usercloudssdk-1.0.4/PKG-INFO
+-rw-r--r--   0 jwang      (501) staff       (20)       12 2023-07-27 00:40:23.000000 usercloudssdk-1.0.4/README.md
+-rw-r--r--   0 jwang      (501) staff       (20)      634 2023-08-01 19:29:24.000000 usercloudssdk-1.0.4/pyproject.toml
+-rw-r--r--   0 jwang      (501) staff       (20)       38 2023-08-01 19:31:41.316511 usercloudssdk-1.0.4/setup.cfg
+drwxr-xr-x   0 jwang      (501) staff       (20)        0 2023-08-01 19:31:41.312994 usercloudssdk-1.0.4/src/
+drwxr-xr-x   0 jwang      (501) staff       (20)        0 2023-08-01 19:31:41.315316 usercloudssdk-1.0.4/src/usercloudssdk/
+-rw-r--r--   0 jwang      (501) staff       (20)        0 2023-08-01 19:21:03.000000 usercloudssdk-1.0.4/src/usercloudssdk/__init__.py
+-rw-r--r--   0 jwang      (501) staff       (20)    17774 2023-08-01 19:21:03.000000 usercloudssdk-1.0.4/src/usercloudssdk/client.py
+-rw-r--r--   0 jwang      (501) staff       (20)      636 2023-08-01 19:21:03.000000 usercloudssdk-1.0.4/src/usercloudssdk/constants.py
+-rw-r--r--   0 jwang      (501) staff       (20)    14342 2023-08-01 19:21:03.000000 usercloudssdk-1.0.4/src/usercloudssdk/models.py
+-rw-r--r--   0 jwang      (501) staff       (20)      790 2023-08-01 19:21:03.000000 usercloudssdk-1.0.4/src/usercloudssdk/policies.py
+-rw-r--r--   0 jwang      (501) staff       (20)     6402 2023-08-01 19:21:03.000000 usercloudssdk-1.0.4/src/usercloudssdk/tokenizer_sample.py
+-rw-r--r--   0 jwang      (501) staff       (20)      405 2023-08-01 19:21:03.000000 usercloudssdk-1.0.4/src/usercloudssdk/ucjson.py
+-rw-r--r--   0 jwang      (501) staff       (20)    11139 2023-08-01 19:26:24.000000 usercloudssdk-1.0.4/src/usercloudssdk/userstore_sample.py
+drwxr-xr-x   0 jwang      (501) staff       (20)        0 2023-08-01 19:31:41.316166 usercloudssdk-1.0.4/src/usercloudssdk.egg-info/
+-rw-r--r--   0 jwang      (501) staff       (20)     1507 2023-08-01 19:31:41.000000 usercloudssdk-1.0.4/src/usercloudssdk.egg-info/PKG-INFO
+-rw-r--r--   0 jwang      (501) staff       (20)      487 2023-08-01 19:31:41.000000 usercloudssdk-1.0.4/src/usercloudssdk.egg-info/SOURCES.txt
+-rw-r--r--   0 jwang      (501) staff       (20)        1 2023-08-01 19:31:41.000000 usercloudssdk-1.0.4/src/usercloudssdk.egg-info/dependency_links.txt
+-rw-r--r--   0 jwang      (501) staff       (20)      166 2023-08-01 19:31:41.000000 usercloudssdk-1.0.4/src/usercloudssdk.egg-info/requires.txt
+-rw-r--r--   0 jwang      (501) staff       (20)       14 2023-08-01 19:31:41.000000 usercloudssdk-1.0.4/src/usercloudssdk.egg-info/top_level.txt
```

### Comparing `usercloudssdk-1.0.3/LICENSE` & `usercloudssdk-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `usercloudssdk-1.0.3/PKG-INFO` & `usercloudssdk-1.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usercloudssdk
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python SDK for UserClouds
 Author-email: Real Python <info@realpython.com>
 License: The MIT License
         
         Copyright (c) 2021- UserClouds, Inc. (https://userclouds.com)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `usercloudssdk-1.0.3/pyproject.toml` & `usercloudssdk-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "usercloudssdk"
-version = "1.0.3"
+version = "1.0.4"
 description = "Python SDK for UserClouds"
 authors = [{ name = "Real Python", email = "info@realpython.com" }]
 license = { file = "LICENSE" }
 dependencies = [
   "certifi >= 2023.7.2",
   "cffi >= 1.15.1",
   "charset-normalizer >= 2.1.1",
```

### Comparing `usercloudssdk-1.0.3/src/usercloudssdk/client.py` & `usercloudssdk-1.0.4/src/usercloudssdk/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -224,18 +224,17 @@
         j = self._put(
             f"/tokenizer/policies/accesstemplate/{access_policy_template.id}",
             data=ucjson.dumps(body),
         )
         return AccessPolicyTemplate.from_json(j)
 
     def DeleteAccessPolicyTemplate(self, id: uuid.UUID, version: int):
-        body = {"version": version}
-
         return self._delete(
-            f"/tokenizer/policies/accesstemplate/{str(id)}", data=ucjson.dumps(body)
+            f"/tokenizer/policies/accesstemplate/{str(id)}",
+            params={"template_version": str(version)},
         )
 
     # Access Policies
 
     def CreateAccessPolicy(
         self, access_policy: AccessPolicy, if_not_exists=False
     ) -> AccessPolicy | Error:
@@ -275,18 +274,17 @@
         j = self._put(
             f"/tokenizer/policies/access/{access_policy.id}",
             data=ucjson.dumps(body),
         )
         return AccessPolicy.from_json(j)
 
     def DeleteAccessPolicy(self, id: uuid.UUID, version: int):
-        body = {"version": version}
-
         return self._delete(
-            f"/tokenizer/policies/access/{str(id)}", data=ucjson.dumps(body)
+            f"/tokenizer/policies/access/{str(id)}",
+            params={"policy_version": str(version)},
         )
 
     ### Transformers
 
     def CreateTransformer(self, transformer: Transformer, if_not_exists=False):
         body = {"transformer": transformer.__dict__}
 
@@ -303,15 +301,15 @@
                     return transformer
             raise e
 
     def ListTransformers(self):
         j = self._get("/tokenizer/policies/transformation")
 
         policies = []
-        for p in j:
+        for p in j["data"]:
             policies.append(Transformer.from_json(p))
 
         return policies
 
     # Note: Transformers are immutable, so no Update method is provided.
 
     def DeleteTransformer(self, id: uuid.UUID):
```

### Comparing `usercloudssdk-1.0.3/src/usercloudssdk/constants.py` & `usercloudssdk-1.0.4/src/usercloudssdk/constants.py`

 * *Files identical despite different names*

### Comparing `usercloudssdk-1.0.3/src/usercloudssdk/models.py` & `usercloudssdk-1.0.4/src/usercloudssdk/models.py`

 * *Files identical despite different names*

### Comparing `usercloudssdk-1.0.3/src/usercloudssdk/policies.py` & `usercloudssdk-1.0.4/src/usercloudssdk/policies.py`

 * *Files identical despite different names*

### Comparing `usercloudssdk-1.0.3/src/usercloudssdk/tokenizer_sample.py` & `usercloudssdk-1.0.4/src/usercloudssdk/tokenizer_sample.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import functools
 import sys
-import uuid
 
 from usercloudssdk.client import Client, Error
 from usercloudssdk.models import (
     AccessPolicy,
     Transformer,
     AccessPolicyComponent,
     AccessPolicyTemplate,
@@ -184,15 +183,16 @@
     except Error as e:
         print("failed to delete token: ", e)
 
 
 def test_error_handling(c):
     try:
         d = c.ResolveTokens(["not a token"], {}, [])
-        print("expected error but got data: ", d)
+        if d[0]["data"] != "":
+            print("expected nothing but got data: ", d)
     except Error as e:
         if e.code != 404:
             print("got unexpected error code (wanted 404): ", e.code)
 
 
 if __name__ == "__main__":
     c = Client(url, client_id, client_secret)
```

### Comparing `usercloudssdk-1.0.3/src/usercloudssdk/userstore_sample.py` & `usercloudssdk-1.0.4/src/usercloudssdk/userstore_sample.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-import uuid
-
-from usercloudssdk.client import Client, Error
+from usercloudssdk.client import Client
 from usercloudssdk.models import (
     AccessPolicy,
     AccessPolicyTemplate,
     AccessPolicyComponent,
     Column,
     ColumnInputConfig,
     ColumnOutputConfig,
```

### Comparing `usercloudssdk-1.0.3/src/usercloudssdk.egg-info/PKG-INFO` & `usercloudssdk-1.0.4/src/usercloudssdk.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usercloudssdk
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python SDK for UserClouds
 Author-email: Real Python <info@realpython.com>
 License: The MIT License
         
         Copyright (c) 2021- UserClouds, Inc. (https://userclouds.com)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

