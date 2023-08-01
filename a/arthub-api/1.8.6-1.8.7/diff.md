# Comparing `tmp/arthub_api-1.8.6.tar.gz` & `tmp/arthub_api-1.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arthub_api-1.8.6.tar", last modified: Mon Jul 31 12:07:44 2023, max compression
+gzip compressed data, was "arthub_api-1.8.7.tar", last modified: Tue Aug  1 12:18:31 2023, max compression
```

## Comparing `arthub_api-1.8.6.tar` & `arthub_api-1.8.7.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 12:07:44.198725 arthub_api-1.8.6/
--rw-rw-rw-   0        0        0     1077 2022-09-05 10:15:53.000000 arthub_api-1.8.6/LICENSE
--rw-rw-rw-   0        0        0      107 2022-09-05 10:15:53.000000 arthub_api-1.8.6/MANIFEST.in
--rw-rw-rw-   0        0        0     1412 2023-07-31 12:07:44.197728 arthub_api-1.8.6/PKG-INFO
--rw-rw-rw-   0        0        0      864 2023-05-19 06:20:15.000000 arthub_api-1.8.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-31 12:07:44.177758 arthub_api-1.8.6/arthub_api/
--rw-rw-rw-   0        0        0      675 2023-07-25 13:45:45.000000 arthub_api-1.8.6/arthub_api/__init__.py
--rw-rw-rw-   0        0        0     3049 2023-07-31 12:06:21.000000 arthub_api-1.8.6/arthub_api/__main__.py
--rw-rw-rw-   0        0        0      241 2023-07-31 12:07:37.000000 arthub_api-1.8.6/arthub_api/__version__.py
--rw-rw-rw-   0        0        0    13661 2023-05-11 11:13:51.000000 arthub_api-1.8.6/arthub_api/_internal_utils.py
--rw-rw-rw-   0        0        0      104 2023-07-25 13:45:45.000000 arthub_api-1.8.6/arthub_api/arthub_api_config.py
--rw-rw-rw-   0        0        0      501 2023-07-25 13:45:45.000000 arthub_api-1.8.6/arthub_api/asset_matrix.py
--rw-rw-rw-   0        0        0    43536 2023-07-25 13:45:45.000000 arthub_api-1.8.6/arthub_api/blade_api.py
--rw-rw-rw-   0        0        0     2072 2023-07-25 13:45:45.000000 arthub_api-1.8.6/arthub_api/blade_api_instance.py
--rw-rw-rw-   0        0        0    28990 2023-07-25 13:45:45.000000 arthub_api-1.8.6/arthub_api/blade_storage.py
--rw-rw-rw-   0        0        0       22 2023-02-08 16:32:42.000000 arthub_api-1.8.6/arthub_api/cli.py
--rw-rw-rw-   0        0        0     1443 2023-07-25 13:45:45.000000 arthub_api-1.8.6/arthub_api/config.py
--rw-rw-rw-   0        0        0      523 2023-02-08 16:32:42.000000 arthub_api-1.8.6/arthub_api/exception.py
--rw-rw-rw-   0        0        0     1258 2023-03-14 10:50:34.000000 arthub_api-1.8.6/arthub_api/models.py
--rw-rw-rw-   0        0        0    44649 2023-07-28 07:48:53.000000 arthub_api-1.8.6/arthub_api/open_api.py
--rw-rw-rw-   0        0        0    41836 2023-07-25 13:45:45.000000 arthub_api-1.8.6/arthub_api/storage.py
--rw-rw-rw-   0        0        0     9102 2023-07-25 13:45:45.000000 arthub_api-1.8.6/arthub_api/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-31 12:07:44.188729 arthub_api-1.8.6/arthub_api.egg-info/
--rw-rw-rw-   0        0        0     1412 2023-07-31 12:07:44.000000 arthub_api-1.8.6/arthub_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      790 2023-07-31 12:07:44.000000 arthub_api-1.8.6/arthub_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 12:07:44.000000 arthub_api-1.8.6/arthub_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-07-31 12:07:44.000000 arthub_api-1.8.6/arthub_api.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-02-09 14:04:12.000000 arthub_api-1.8.6/arthub_api.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      164 2023-07-31 12:07:44.000000 arthub_api-1.8.6/arthub_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-31 12:07:44.000000 arthub_api-1.8.6/arthub_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       63 2022-09-26 03:28:18.000000 arthub_api-1.8.6/requirements-dev.txt
--rw-rw-rw-   0        0        0       42 2023-07-31 12:07:44.198725 arthub_api-1.8.6/setup.cfg
--rw-rw-rw-   0        0        0     3129 2023-07-31 11:59:40.000000 arthub_api-1.8.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-31 12:07:44.195783 arthub_api-1.8.6/tests/
--rw-rw-rw-   0        0        0      176 2023-07-25 13:45:45.000000 arthub_api-1.8.6/tests/__init__.py
--rw-rw-rw-   0        0        0      108 2023-05-19 06:20:15.000000 arthub_api-1.8.6/tests/_utils.py
--rw-rw-rw-   0        0        0      735 2023-07-25 13:45:45.000000 arthub_api-1.8.6/tests/conftest.py
--rw-rw-rw-   0        0        0     6646 2023-07-25 13:45:45.000000 arthub_api-1.8.6/tests/test_open_api.py
--rw-rw-rw-   0        0        0     2979 2023-07-25 13:45:45.000000 arthub_api-1.8.6/tests/test_storage.py
+drwxrwxrwx   0        0        0        0 2023-08-01 12:18:31.435008 arthub_api-1.8.7/
+-rw-rw-rw-   0        0        0     1077 2022-09-05 10:15:53.000000 arthub_api-1.8.7/LICENSE
+-rw-rw-rw-   0        0        0      107 2022-09-05 10:15:53.000000 arthub_api-1.8.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     1412 2023-08-01 12:18:31.434252 arthub_api-1.8.7/PKG-INFO
+-rw-rw-rw-   0        0        0      864 2023-05-19 06:20:15.000000 arthub_api-1.8.7/README.md
+drwxrwxrwx   0        0        0        0 2023-08-01 12:18:31.411812 arthub_api-1.8.7/arthub_api/
+-rw-rw-rw-   0        0        0      675 2023-07-25 13:45:45.000000 arthub_api-1.8.7/arthub_api/__init__.py
+-rw-rw-rw-   0        0        0     3049 2023-07-31 12:06:21.000000 arthub_api-1.8.7/arthub_api/__main__.py
+-rw-rw-rw-   0        0        0      241 2023-08-01 12:15:58.000000 arthub_api-1.8.7/arthub_api/__version__.py
+-rw-rw-rw-   0        0        0    13661 2023-05-11 11:13:51.000000 arthub_api-1.8.7/arthub_api/_internal_utils.py
+-rw-rw-rw-   0        0        0      104 2023-07-25 13:45:45.000000 arthub_api-1.8.7/arthub_api/arthub_api_config.py
+-rw-rw-rw-   0        0        0      501 2023-07-25 13:45:45.000000 arthub_api-1.8.7/arthub_api/asset_matrix.py
+-rw-rw-rw-   0        0        0    43536 2023-07-25 13:45:45.000000 arthub_api-1.8.7/arthub_api/blade_api.py
+-rw-rw-rw-   0        0        0     2072 2023-07-25 13:45:45.000000 arthub_api-1.8.7/arthub_api/blade_api_instance.py
+-rw-rw-rw-   0        0        0    28990 2023-07-25 13:45:45.000000 arthub_api-1.8.7/arthub_api/blade_storage.py
+-rw-rw-rw-   0        0        0       22 2023-02-08 16:32:42.000000 arthub_api-1.8.7/arthub_api/cli.py
+-rw-rw-rw-   0        0        0     1443 2023-07-25 13:45:45.000000 arthub_api-1.8.7/arthub_api/config.py
+-rw-rw-rw-   0        0        0      523 2023-02-08 16:32:42.000000 arthub_api-1.8.7/arthub_api/exception.py
+-rw-rw-rw-   0        0        0     1258 2023-03-14 10:50:34.000000 arthub_api-1.8.7/arthub_api/models.py
+-rw-rw-rw-   0        0        0    44784 2023-08-01 12:07:16.000000 arthub_api-1.8.7/arthub_api/open_api.py
+-rw-rw-rw-   0        0        0    41836 2023-07-25 13:45:45.000000 arthub_api-1.8.7/arthub_api/storage.py
+-rw-rw-rw-   0        0        0     9102 2023-07-25 13:45:45.000000 arthub_api-1.8.7/arthub_api/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-01 12:18:31.424777 arthub_api-1.8.7/arthub_api.egg-info/
+-rw-rw-rw-   0        0        0     1412 2023-08-01 12:18:30.000000 arthub_api-1.8.7/arthub_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      790 2023-08-01 12:18:30.000000 arthub_api-1.8.7/arthub_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 12:18:30.000000 arthub_api-1.8.7/arthub_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-08-01 12:18:30.000000 arthub_api-1.8.7/arthub_api.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-02-09 14:04:12.000000 arthub_api-1.8.7/arthub_api.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      164 2023-08-01 12:18:30.000000 arthub_api-1.8.7/arthub_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-08-01 12:18:30.000000 arthub_api-1.8.7/arthub_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       63 2022-09-26 03:28:18.000000 arthub_api-1.8.7/requirements-dev.txt
+-rw-rw-rw-   0        0        0       42 2023-08-01 12:18:31.435008 arthub_api-1.8.7/setup.cfg
+-rw-rw-rw-   0        0        0     3129 2023-07-31 11:59:40.000000 arthub_api-1.8.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 12:18:31.431809 arthub_api-1.8.7/tests/
+-rw-rw-rw-   0        0        0      176 2023-07-25 13:45:45.000000 arthub_api-1.8.7/tests/__init__.py
+-rw-rw-rw-   0        0        0      108 2023-05-19 06:20:15.000000 arthub_api-1.8.7/tests/_utils.py
+-rw-rw-rw-   0        0        0      735 2023-07-25 13:45:45.000000 arthub_api-1.8.7/tests/conftest.py
+-rw-rw-rw-   0        0        0     6646 2023-07-25 13:45:45.000000 arthub_api-1.8.7/tests/test_open_api.py
+-rw-rw-rw-   0        0        0     2979 2023-07-25 13:45:45.000000 arthub_api-1.8.7/tests/test_storage.py
```

### Comparing `arthub_api-1.8.6/LICENSE` & `arthub_api-1.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `arthub_api-1.8.6/PKG-INFO` & `arthub_api-1.8.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arthub_api
-Version: 1.8.6
+Version: 1.8.7
 Summary: ArHhub Python SDK
 Home-page: UNKNOWN
 Author: Joey Ding
 Author-email: joeyding@tencent.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `arthub_api-1.8.6/README.md` & `arthub_api-1.8.7/README.md`

 * *Files identical despite different names*

### Comparing `arthub_api-1.8.6/arthub_api/__init__.py` & `arthub_api-1.8.7/arthub_api/__init__.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.8.6/arthub_api/__main__.py` & `arthub_api-1.8.7/arthub_api/__main__.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.8.6/arthub_api/_internal_utils.py` & `arthub_api-1.8.7/arthub_api/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.8.6/arthub_api/blade_api.py` & `arthub_api-1.8.7/arthub_api/blade_api.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.8.6/arthub_api/blade_api_instance.py` & `arthub_api-1.8.7/arthub_api/blade_api_instance.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.8.6/arthub_api/blade_storage.py` & `arthub_api-1.8.7/arthub_api/blade_storage.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.8.6/arthub_api/config.py` & `arthub_api-1.8.7/arthub_api/config.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.8.6/arthub_api/exception.py` & `arthub_api-1.8.7/arthub_api/exception.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.8.6/arthub_api/models.py` & `arthub_api-1.8.7/arthub_api/models.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.8.6/arthub_api/open_api.py` & `arthub_api-1.8.7/arthub_api/open_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -348,23 +348,28 @@
             permission_group.append("pass")
         return permission_group
 
     def clear_token(self):
         self._token = ""
         self._public_token = ""
 
+    def clear_cookies(self):
+        self._cookies = None
+
     def clear_token_cache(self):
         name = self.api_host
         if name == "":
             return
         utils.remove_token_cache_file(name)
 
     def logout(self):
         self.clear_token()
         self.clear_token_cache()
+        self.clear_cookies()
+        self._current_account_info = None
 
     def get_token_from_cache(self):
         name = self.api_host
         if name == "":
             return
         token = utils.get_token_from_cache(name)
         if token:
```

### Comparing `arthub_api-1.8.6/arthub_api/storage.py` & `arthub_api-1.8.7/arthub_api/storage.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.8.6/arthub_api/utils.py` & `arthub_api-1.8.7/arthub_api/utils.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.8.6/arthub_api.egg-info/PKG-INFO` & `arthub_api-1.8.7/arthub_api.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arthub-api
-Version: 1.8.6
+Version: 1.8.7
 Summary: ArHhub Python SDK
 Home-page: UNKNOWN
 Author: Joey Ding
 Author-email: joeyding@tencent.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `arthub_api-1.8.6/arthub_api.egg-info/SOURCES.txt` & `arthub_api-1.8.7/arthub_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arthub_api-1.8.6/setup.py` & `arthub_api-1.8.7/setup.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.8.6/tests/conftest.py` & `arthub_api-1.8.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.8.6/tests/test_open_api.py` & `arthub_api-1.8.7/tests/test_open_api.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.8.6/tests/test_storage.py` & `arthub_api-1.8.7/tests/test_storage.py`

 * *Files identical despite different names*

