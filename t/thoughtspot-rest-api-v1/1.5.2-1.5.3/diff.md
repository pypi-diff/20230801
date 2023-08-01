# Comparing `tmp/thoughtspot_rest_api_v1-1.5.2.tar.gz` & `tmp/thoughtspot_rest_api_v1-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thoughtspot_rest_api_v1-1.5.2.tar", last modified: Mon Jun  5 14:38:39 2023, max compression
+gzip compressed data, was "thoughtspot_rest_api_v1-1.5.3.tar", last modified: Tue Aug  1 20:34:09 2023, max compression
```

## Comparing `thoughtspot_rest_api_v1-1.5.2.tar` & `thoughtspot_rest_api_v1-1.5.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 bryant.howell (535524999) 1339924365        0 2023-06-05 14:38:39.535963 thoughtspot_rest_api_v1-1.5.2/
--rw-r--r--   0 bryant.howell (535524999) 1339924365    14780 2022-04-06 21:26:49.000000 thoughtspot_rest_api_v1-1.5.2/LICENSE
--rw-r--r--   0 bryant.howell (535524999) 1339924365    29237 2023-06-05 14:38:39.536029 thoughtspot_rest_api_v1-1.5.2/PKG-INFO
--rw-r--r--   0 bryant.howell (535524999) 1339924365    28536 2023-03-17 18:28:57.000000 thoughtspot_rest_api_v1-1.5.2/README.md
--rw-r--r--   0 bryant.howell (535524999) 1339924365       85 2022-04-04 15:39:10.000000 thoughtspot_rest_api_v1-1.5.2/pyproject.toml
--rw-r--r--   0 bryant.howell (535524999) 1339924365      884 2023-06-05 14:38:39.536336 thoughtspot_rest_api_v1-1.5.2/setup.cfg
--rw-r--r--   0 bryant.howell (535524999) 1339924365      236 2022-04-04 15:39:10.000000 thoughtspot_rest_api_v1-1.5.2/setup.py
-drwxr-xr-x   0 bryant.howell (535524999) 1339924365        0 2023-06-05 14:38:39.532449 thoughtspot_rest_api_v1-1.5.2/src/
-drwxr-xr-x   0 bryant.howell (535524999) 1339924365        0 2023-06-05 14:38:39.534448 thoughtspot_rest_api_v1-1.5.2/src/thoughtspot_rest_api_v1/
--rw-r--r--   0 bryant.howell (535524999) 1339924365      318 2022-09-09 16:25:24.000000 thoughtspot_rest_api_v1-1.5.2/src/thoughtspot_rest_api_v1/__init__.py
--rw-r--r--   0 bryant.howell (535524999) 1339924365       22 2023-06-05 14:34:57.000000 thoughtspot_rest_api_v1-1.5.2/src/thoughtspot_rest_api_v1/_version.py
--rw-r--r--   0 bryant.howell (535524999) 1339924365     2328 2022-09-09 16:25:24.000000 thoughtspot_rest_api_v1-1.5.2/src/thoughtspot_rest_api_v1/details_objects.py
--rw-r--r--   0 bryant.howell (535524999) 1339924365    75805 2023-06-05 14:38:31.000000 thoughtspot_rest_api_v1-1.5.2/src/thoughtspot_rest_api_v1/tsrestapiv1.py
--rw-r--r--   0 bryant.howell (535524999) 1339924365    24853 2023-05-30 19:44:47.000000 thoughtspot_rest_api_v1-1.5.2/src/thoughtspot_rest_api_v1/tsrestapiv2.py
-drwxr-xr-x   0 bryant.howell (535524999) 1339924365        0 2023-06-05 14:38:39.535833 thoughtspot_rest_api_v1-1.5.2/src/thoughtspot_rest_api_v1.egg-info/
--rw-r--r--   0 bryant.howell (535524999) 1339924365    29237 2023-06-05 14:38:39.000000 thoughtspot_rest_api_v1-1.5.2/src/thoughtspot_rest_api_v1.egg-info/PKG-INFO
--rw-r--r--   0 bryant.howell (535524999) 1339924365      518 2023-06-05 14:38:39.000000 thoughtspot_rest_api_v1-1.5.2/src/thoughtspot_rest_api_v1.egg-info/SOURCES.txt
--rw-r--r--   0 bryant.howell (535524999) 1339924365        1 2023-06-05 14:38:39.000000 thoughtspot_rest_api_v1-1.5.2/src/thoughtspot_rest_api_v1.egg-info/dependency_links.txt
--rw-r--r--   0 bryant.howell (535524999) 1339924365       22 2023-06-05 14:38:39.000000 thoughtspot_rest_api_v1-1.5.2/src/thoughtspot_rest_api_v1.egg-info/requires.txt
--rw-r--r--   0 bryant.howell (535524999) 1339924365       24 2023-06-05 14:38:39.000000 thoughtspot_rest_api_v1-1.5.2/src/thoughtspot_rest_api_v1.egg-info/top_level.txt
+drwxr-xr-x   0 bryant.howell (535524999) 1339924365        0 2023-08-01 20:34:09.418260 thoughtspot_rest_api_v1-1.5.3/
+-rw-r--r--   0 bryant.howell (535524999) 1339924365    14780 2022-04-06 21:26:49.000000 thoughtspot_rest_api_v1-1.5.3/LICENSE
+-rw-r--r--   0 bryant.howell (535524999) 1339924365    28888 2023-08-01 20:34:09.418337 thoughtspot_rest_api_v1-1.5.3/PKG-INFO
+-rw-r--r--   0 bryant.howell (535524999) 1339924365    28187 2023-07-25 11:41:59.000000 thoughtspot_rest_api_v1-1.5.3/README.md
+-rw-r--r--   0 bryant.howell (535524999) 1339924365       85 2022-04-04 15:39:10.000000 thoughtspot_rest_api_v1-1.5.3/pyproject.toml
+-rw-r--r--   0 bryant.howell (535524999) 1339924365      884 2023-08-01 20:34:09.418656 thoughtspot_rest_api_v1-1.5.3/setup.cfg
+-rw-r--r--   0 bryant.howell (535524999) 1339924365      236 2022-04-04 15:39:10.000000 thoughtspot_rest_api_v1-1.5.3/setup.py
+drwxr-xr-x   0 bryant.howell (535524999) 1339924365        0 2023-08-01 20:34:09.414180 thoughtspot_rest_api_v1-1.5.3/src/
+drwxr-xr-x   0 bryant.howell (535524999) 1339924365        0 2023-08-01 20:34:09.417140 thoughtspot_rest_api_v1-1.5.3/src/thoughtspot_rest_api_v1/
+-rw-r--r--   0 bryant.howell (535524999) 1339924365      318 2022-09-09 16:25:24.000000 thoughtspot_rest_api_v1-1.5.3/src/thoughtspot_rest_api_v1/__init__.py
+-rw-r--r--   0 bryant.howell (535524999) 1339924365       22 2023-08-01 20:33:45.000000 thoughtspot_rest_api_v1-1.5.3/src/thoughtspot_rest_api_v1/_version.py
+-rw-r--r--   0 bryant.howell (535524999) 1339924365     2328 2022-09-09 16:25:24.000000 thoughtspot_rest_api_v1-1.5.3/src/thoughtspot_rest_api_v1/details_objects.py
+-rw-r--r--   0 bryant.howell (535524999) 1339924365    75805 2023-06-05 14:38:31.000000 thoughtspot_rest_api_v1-1.5.3/src/thoughtspot_rest_api_v1/tsrestapiv1.py
+-rw-r--r--   0 bryant.howell (535524999) 1339924365    25025 2023-08-01 20:32:16.000000 thoughtspot_rest_api_v1-1.5.3/src/thoughtspot_rest_api_v1/tsrestapiv2.py
+drwxr-xr-x   0 bryant.howell (535524999) 1339924365        0 2023-08-01 20:34:09.418136 thoughtspot_rest_api_v1-1.5.3/src/thoughtspot_rest_api_v1.egg-info/
+-rw-r--r--   0 bryant.howell (535524999) 1339924365    28888 2023-08-01 20:34:09.000000 thoughtspot_rest_api_v1-1.5.3/src/thoughtspot_rest_api_v1.egg-info/PKG-INFO
+-rw-r--r--   0 bryant.howell (535524999) 1339924365      518 2023-08-01 20:34:09.000000 thoughtspot_rest_api_v1-1.5.3/src/thoughtspot_rest_api_v1.egg-info/SOURCES.txt
+-rw-r--r--   0 bryant.howell (535524999) 1339924365        1 2023-08-01 20:34:09.000000 thoughtspot_rest_api_v1-1.5.3/src/thoughtspot_rest_api_v1.egg-info/dependency_links.txt
+-rw-r--r--   0 bryant.howell (535524999) 1339924365       22 2023-08-01 20:34:09.000000 thoughtspot_rest_api_v1-1.5.3/src/thoughtspot_rest_api_v1.egg-info/requires.txt
+-rw-r--r--   0 bryant.howell (535524999) 1339924365       24 2023-08-01 20:34:09.000000 thoughtspot_rest_api_v1-1.5.3/src/thoughtspot_rest_api_v1.egg-info/top_level.txt
```

### Comparing `thoughtspot_rest_api_v1-1.5.2/LICENSE` & `thoughtspot_rest_api_v1-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `thoughtspot_rest_api_v1-1.5.2/PKG-INFO` & `thoughtspot_rest_api_v1-1.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thoughtspot_rest_api_v1
-Version: 1.5.2
+Version: 1.5.3
 Summary: Library implementing the ThoughtSpot V1 REST API
 Home-page: https://github.com/thoughtspot/thoughtspot_rest_api_v1_python
 Author: Bryant Howell
 Author-email: bryant.howell@thoughtspot.com
 License: MIT
 Project-URL: Documentation, https://github.com/thoughtspot/thoughtspot_rest_api_v1_python#readme
 Project-URL: Bug Tracker, https://github.com/thoughtspot/thoughtspot_rest_api_v1_python/issues
@@ -421,16 +421,14 @@
 
     viz_data_response = ts.pinboarddata(pinboard_guid=lb_guid, vizids=[viz_on_lb_guid])
 
 
 ## Additional libraries
 `thoughtspot_tml` is a library for processing the ThoughtSpot Modeling Language (TML) files. You can use `thoughtspot_tml` to manipulate TML files from disk or exported via the REST API.
 
-`ts_rest_api_and_tml_tools` is a convenience library that imports both `thoughtspot_rest_api_v1` and `thoughtspot_tml` and wraps them in more convenient and obvious packaging. It also contains many example scripts to do common workflows. In particular, there are many examples of SDLC use cases that involve REST API commands and TML manipulation.
-
 `cs_tools` is a package of command-line tools built by the ThoughtSpot Professional Services team, aimed at ThoughtSpot administrators. 
 
 
 [jump-learning]: <#learning-from-the-source-code> "jump: Learning"
 [jump-getting-started]: <#getting-started> "jump: Getting Started"
 [jump-tutorial]: <#importing-the-library> "jump: Intro Tutorial"
 [jump-libraries]: <#additional-libraries> "jump: More Libraries"
```

### Comparing `thoughtspot_rest_api_v1-1.5.2/README.md` & `thoughtspot_rest_api_v1-1.5.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -404,16 +404,14 @@
 
     viz_data_response = ts.pinboarddata(pinboard_guid=lb_guid, vizids=[viz_on_lb_guid])
 
 
 ## Additional libraries
 `thoughtspot_tml` is a library for processing the ThoughtSpot Modeling Language (TML) files. You can use `thoughtspot_tml` to manipulate TML files from disk or exported via the REST API.
 
-`ts_rest_api_and_tml_tools` is a convenience library that imports both `thoughtspot_rest_api_v1` and `thoughtspot_tml` and wraps them in more convenient and obvious packaging. It also contains many example scripts to do common workflows. In particular, there are many examples of SDLC use cases that involve REST API commands and TML manipulation.
-
 `cs_tools` is a package of command-line tools built by the ThoughtSpot Professional Services team, aimed at ThoughtSpot administrators. 
 
 
 [jump-learning]: <#learning-from-the-source-code> "jump: Learning"
 [jump-getting-started]: <#getting-started> "jump: Getting Started"
 [jump-tutorial]: <#importing-the-library> "jump: Intro Tutorial"
 [jump-libraries]: <#additional-libraries> "jump: More Libraries"
```

### Comparing `thoughtspot_rest_api_v1-1.5.2/setup.cfg` & `thoughtspot_rest_api_v1-1.5.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = thoughtspot_rest_api_v1
-version = 1.5.2
+version = 1.5.3
 description = Library implementing the ThoughtSpot V1 REST API
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/thoughtspot/thoughtspot_rest_api_v1_python
 author = Bryant Howell
 author_email = bryant.howell@thoughtspot.com
 license = MIT
```

### Comparing `thoughtspot_rest_api_v1-1.5.2/src/thoughtspot_rest_api_v1/details_objects.py` & `thoughtspot_rest_api_v1-1.5.3/src/thoughtspot_rest_api_v1/details_objects.py`

 * *Files identical despite different names*

### Comparing `thoughtspot_rest_api_v1-1.5.2/src/thoughtspot_rest_api_v1/tsrestapiv1.py` & `thoughtspot_rest_api_v1-1.5.3/src/thoughtspot_rest_api_v1/tsrestapiv1.py`

 * *Files identical despite different names*

### Comparing `thoughtspot_rest_api_v1-1.5.2/src/thoughtspot_rest_api_v1/tsrestapiv2.py` & `thoughtspot_rest_api_v1-1.5.3/src/thoughtspot_rest_api_v1/tsrestapiv2.py`

 * *Files 0% similar despite different names*

```diff
@@ -523,22 +523,24 @@
     def metadata_answer_data(self, request: Dict):
         endpoint = 'metadata/answer/data'
         return self.post_request(endpoint=endpoint, request=request)
 
 #
 # /logs/ endpoints
 #
-    def logs_fetch(self, log_type: str, start_epoch_time_in_millis: int,
-                   end_epoch_time_in_millis: int):
+    def logs_fetch(self, log_type: str = 'SECURITY_AUDIT', start_epoch_time_in_millis: Optional[int] = None,
+                   end_epoch_time_in_millis: Optional[int] = None):
         endpoint = 'logs/fetch'
         request = {
-            'log_type': log_type,
-            'start_epoch_time_in_millis': start_epoch_time_in_millis,
-            'end_epoch_time_in_millis': end_epoch_time_in_millis
+            'log_type': log_type
         }
+        if start_epoch_time_in_millis is not None:
+            request['start_epoch_time_in_millis'] = start_epoch_time_in_millis
+        if end_epoch_time_in_millis is not None:
+            request['end_epoch_time_in_millis'] =  end_epoch_time_in_millis
         return self.post_request(endpoint=endpoint, request=request)
 
 #
 # Version Control /vcs/ endpoints
 #
     def vcs_git_config_search(self, request: Dict):
         endpoint = 'vcs/git/config/search'
```

### Comparing `thoughtspot_rest_api_v1-1.5.2/src/thoughtspot_rest_api_v1.egg-info/PKG-INFO` & `thoughtspot_rest_api_v1-1.5.3/src/thoughtspot_rest_api_v1.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thoughtspot-rest-api-v1
-Version: 1.5.2
+Version: 1.5.3
 Summary: Library implementing the ThoughtSpot V1 REST API
 Home-page: https://github.com/thoughtspot/thoughtspot_rest_api_v1_python
 Author: Bryant Howell
 Author-email: bryant.howell@thoughtspot.com
 License: MIT
 Project-URL: Documentation, https://github.com/thoughtspot/thoughtspot_rest_api_v1_python#readme
 Project-URL: Bug Tracker, https://github.com/thoughtspot/thoughtspot_rest_api_v1_python/issues
@@ -421,16 +421,14 @@
 
     viz_data_response = ts.pinboarddata(pinboard_guid=lb_guid, vizids=[viz_on_lb_guid])
 
 
 ## Additional libraries
 `thoughtspot_tml` is a library for processing the ThoughtSpot Modeling Language (TML) files. You can use `thoughtspot_tml` to manipulate TML files from disk or exported via the REST API.
 
-`ts_rest_api_and_tml_tools` is a convenience library that imports both `thoughtspot_rest_api_v1` and `thoughtspot_tml` and wraps them in more convenient and obvious packaging. It also contains many example scripts to do common workflows. In particular, there are many examples of SDLC use cases that involve REST API commands and TML manipulation.
-
 `cs_tools` is a package of command-line tools built by the ThoughtSpot Professional Services team, aimed at ThoughtSpot administrators. 
 
 
 [jump-learning]: <#learning-from-the-source-code> "jump: Learning"
 [jump-getting-started]: <#getting-started> "jump: Getting Started"
 [jump-tutorial]: <#importing-the-library> "jump: Intro Tutorial"
 [jump-libraries]: <#additional-libraries> "jump: More Libraries"
```

### Comparing `thoughtspot_rest_api_v1-1.5.2/src/thoughtspot_rest_api_v1.egg-info/SOURCES.txt` & `thoughtspot_rest_api_v1-1.5.3/src/thoughtspot_rest_api_v1.egg-info/SOURCES.txt`

 * *Files identical despite different names*

