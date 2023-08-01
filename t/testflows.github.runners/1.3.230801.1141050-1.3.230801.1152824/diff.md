# Comparing `tmp/testflows.github.runners-1.3.230801.1141050.tar.gz` & `tmp/testflows.github.runners-1.3.230801.1152824.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testflows.github.runners-1.3.230801.1141050.tar", last modified: Tue Aug  1 14:10:51 2023, max compression
+gzip compressed data, was "testflows.github.runners-1.3.230801.1152824.tar", last modified: Tue Aug  1 15:28:25 2023, max compression
```

## Comparing `testflows.github.runners-1.3.230801.1141050.tar` & `testflows.github.runners-1.3.230801.1152824.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 14:10:51.023690 testflows.github.runners-1.3.230801.1141050/
--rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1141050/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)    57192 2023-08-01 14:10:51.023690 testflows.github.runners-1.3.230801.1141050/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    56600 2023-07-31 22:43:07.000000 testflows.github.runners-1.3.230801.1141050/README.rst
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-08-01 14:10:51.023690 testflows.github.runners-1.3.230801.1141050/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     2043 2023-08-01 14:10:50.000000 testflows.github.runners-1.3.230801.1141050/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 14:10:51.019690 testflows.github.runners-1.3.230801.1141050/testflows/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 14:10:51.019690 testflows.github.runners-1.3.230801.1141050/testflows/github/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 14:10:51.019690 testflows.github.runners-1.3.230801.1141050/testflows/github/runners/
--rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-08-01 14:10:50.000000 testflows.github.runners-1.3.230801.1141050/testflows/github/runners/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1615 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1141050/testflows/github/runners/actions.py
--rw-rw-r--   0 user      (1000) user      (1000)     1951 2023-08-01 03:44:03.000000 testflows.github.runners-1.3.230801.1141050/testflows/github/runners/api_watch.py
--rw-rw-r--   0 user      (1000) user      (1000)     2599 2023-07-31 15:05:55.000000 testflows.github.runners-1.3.230801.1141050/testflows/github/runners/args.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 14:10:51.019690 testflows.github.runners-1.3.230801.1141050/testflows/github/runners/bin/
--rwxrwxr-x   0 user      (1000) user      (1000)    24893 2023-08-01 14:07:13.000000 testflows.github.runners-1.3.230801.1141050/testflows/github/runners/bin/github-runners
--rw-rw-r--   0 user      (1000) user      (1000)    13607 2023-07-29 23:57:40.000000 testflows.github.runners-1.3.230801.1141050/testflows/github/runners/cloud.py
--rw-rw-r--   0 user      (1000) user      (1000)     4164 2023-08-01 01:08:42.000000 testflows.github.runners-1.3.230801.1141050/testflows/github/runners/config.py
--rw-rw-r--   0 user      (1000) user      (1000)     2473 2023-07-29 23:43:11.000000 testflows.github.runners-1.3.230801.1141050/testflows/github/runners/delete.py
--rw-rw-r--   0 user      (1000) user      (1000)      726 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1141050/testflows/github/runners/logger.py
--rw-rw-r--   0 user      (1000) user      (1000)     1926 2023-07-29 23:39:43.000000 testflows.github.runners-1.3.230801.1141050/testflows/github/runners/request.py
--rw-rw-r--   0 user      (1000) user      (1000)    11279 2023-08-01 03:43:12.000000 testflows.github.runners-1.3.230801.1141050/testflows/github/runners/scale_down.py
--rw-rw-r--   0 user      (1000) user      (1000)    17362 2023-08-01 03:14:02.000000 testflows.github.runners-1.3.230801.1141050/testflows/github/runners/scale_up.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 14:10:51.019690 testflows.github.runners-1.3.230801.1141050/testflows/github/runners/scripts/
--rw-rw-r--   0 user      (1000) user      (1000)     1061 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1141050/testflows/github/runners/scripts/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 14:10:51.019690 testflows.github.runners-1.3.230801.1141050/testflows/github/runners/scripts/deploy/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1141050/testflows/github/runners/scripts/deploy/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      519 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1141050/testflows/github/runners/scripts/deploy/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      260 2023-07-31 12:43:19.000000 testflows.github.runners-1.3.230801.1141050/testflows/github/runners/scripts/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)     1148 2023-07-31 12:59:30.000000 testflows.github.runners-1.3.230801.1141050/testflows/github/runners/scripts/setup_docker.sh
--rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1141050/testflows/github/runners/scripts/startup_arm64.sh
--rw-rw-r--   0 user      (1000) user      (1000)      715 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1141050/testflows/github/runners/scripts/startup_x64.sh
--rw-rw-r--   0 user      (1000) user      (1000)     2522 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1141050/testflows/github/runners/server.py
--rw-rw-r--   0 user      (1000) user      (1000)     5158 2023-07-31 17:30:38.000000 testflows.github.runners-1.3.230801.1141050/testflows/github/runners/service.py
--rw-rw-r--   0 user      (1000) user      (1000)     1483 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1141050/testflows/github/runners/shell.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 14:10:51.019690 testflows.github.runners-1.3.230801.1141050/testflows.github.runners.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    57192 2023-08-01 14:10:50.000000 testflows.github.runners-1.3.230801.1141050/testflows.github.runners.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1192 2023-08-01 14:10:50.000000 testflows.github.runners-1.3.230801.1141050/testflows.github.runners.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-08-01 14:10:50.000000 testflows.github.runners-1.3.230801.1141050/testflows.github.runners.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-29 01:22:42.000000 testflows.github.runners-1.3.230801.1141050/testflows.github.runners.egg-info/not-zip-safe
--rw-rw-r--   0 user      (1000) user      (1000)       61 2023-08-01 14:10:50.000000 testflows.github.runners-1.3.230801.1141050/testflows.github.runners.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       10 2023-08-01 14:10:50.000000 testflows.github.runners-1.3.230801.1141050/testflows.github.runners.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 15:28:25.103008 testflows.github.runners-1.3.230801.1152824/
+-rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1152824/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)    57192 2023-08-01 15:28:25.103008 testflows.github.runners-1.3.230801.1152824/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    56600 2023-07-31 22:43:07.000000 testflows.github.runners-1.3.230801.1152824/README.rst
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-08-01 15:28:25.103008 testflows.github.runners-1.3.230801.1152824/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     2043 2023-08-01 15:28:24.000000 testflows.github.runners-1.3.230801.1152824/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 15:28:25.103008 testflows.github.runners-1.3.230801.1152824/testflows/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 15:28:25.103008 testflows.github.runners-1.3.230801.1152824/testflows/github/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 15:28:25.103008 testflows.github.runners-1.3.230801.1152824/testflows/github/runners/
+-rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-08-01 15:28:24.000000 testflows.github.runners-1.3.230801.1152824/testflows/github/runners/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1615 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1152824/testflows/github/runners/actions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1951 2023-08-01 03:44:03.000000 testflows.github.runners-1.3.230801.1152824/testflows/github/runners/api_watch.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2599 2023-07-31 15:05:55.000000 testflows.github.runners-1.3.230801.1152824/testflows/github/runners/args.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 15:28:25.103008 testflows.github.runners-1.3.230801.1152824/testflows/github/runners/bin/
+-rwxrwxr-x   0 user      (1000) user      (1000)    24953 2023-08-01 15:27:48.000000 testflows.github.runners-1.3.230801.1152824/testflows/github/runners/bin/github-runners
+-rw-rw-r--   0 user      (1000) user      (1000)    13607 2023-07-29 23:57:40.000000 testflows.github.runners-1.3.230801.1152824/testflows/github/runners/cloud.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4164 2023-08-01 01:08:42.000000 testflows.github.runners-1.3.230801.1152824/testflows/github/runners/config.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2473 2023-07-29 23:43:11.000000 testflows.github.runners-1.3.230801.1152824/testflows/github/runners/delete.py
+-rw-rw-r--   0 user      (1000) user      (1000)      726 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1152824/testflows/github/runners/logger.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1926 2023-07-29 23:39:43.000000 testflows.github.runners-1.3.230801.1152824/testflows/github/runners/request.py
+-rw-rw-r--   0 user      (1000) user      (1000)    11279 2023-08-01 03:43:12.000000 testflows.github.runners-1.3.230801.1152824/testflows/github/runners/scale_down.py
+-rw-rw-r--   0 user      (1000) user      (1000)    17362 2023-08-01 03:14:02.000000 testflows.github.runners-1.3.230801.1152824/testflows/github/runners/scale_up.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 15:28:25.103008 testflows.github.runners-1.3.230801.1152824/testflows/github/runners/scripts/
+-rw-rw-r--   0 user      (1000) user      (1000)     1061 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1152824/testflows/github/runners/scripts/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 15:28:25.103008 testflows.github.runners-1.3.230801.1152824/testflows/github/runners/scripts/deploy/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1152824/testflows/github/runners/scripts/deploy/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      519 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1152824/testflows/github/runners/scripts/deploy/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      260 2023-07-31 12:43:19.000000 testflows.github.runners-1.3.230801.1152824/testflows/github/runners/scripts/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)     1148 2023-07-31 12:59:30.000000 testflows.github.runners-1.3.230801.1152824/testflows/github/runners/scripts/setup_docker.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1152824/testflows/github/runners/scripts/startup_arm64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      715 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1152824/testflows/github/runners/scripts/startup_x64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)     2522 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1152824/testflows/github/runners/server.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5158 2023-07-31 17:30:38.000000 testflows.github.runners-1.3.230801.1152824/testflows/github/runners/service.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1483 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1152824/testflows/github/runners/shell.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 15:28:25.103008 testflows.github.runners-1.3.230801.1152824/testflows.github.runners.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    57192 2023-08-01 15:28:25.000000 testflows.github.runners-1.3.230801.1152824/testflows.github.runners.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1192 2023-08-01 15:28:25.000000 testflows.github.runners-1.3.230801.1152824/testflows.github.runners.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-08-01 15:28:25.000000 testflows.github.runners-1.3.230801.1152824/testflows.github.runners.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-29 01:22:42.000000 testflows.github.runners-1.3.230801.1152824/testflows.github.runners.egg-info/not-zip-safe
+-rw-rw-r--   0 user      (1000) user      (1000)       61 2023-08-01 15:28:25.000000 testflows.github.runners-1.3.230801.1152824/testflows.github.runners.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       10 2023-08-01 15:28:25.000000 testflows.github.runners-1.3.230801.1152824/testflows.github.runners.egg-info/top_level.txt
```

### Comparing `testflows.github.runners-1.3.230801.1141050/LICENSE` & `testflows.github.runners-1.3.230801.1152824/LICENSE`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1141050/PKG-INFO` & `testflows.github.runners-1.3.230801.1152824/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.3.230801.1141050
+Version: 1.3.230801.1152824
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `testflows.github.runners-1.3.230801.1141050/README.rst` & `testflows.github.runners-1.3.230801.1152824/README.rst`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1141050/setup.py` & `testflows.github.runners-1.3.230801.1152824/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 with open("README.rst", "r", encoding="utf-8") as fd:
     long_description = fd.read()
 
 
 setup(
     name="testflows.github.runners",
-    version="1.3.230801.1141050",
+    version="1.3.230801.1152824",
     description="Autoscaling GitHub Actions Runners Using Hetzner Cloud ",
     author="Vitaliy Zakaznikov",
     author_email="vzakaznikov@testflows.com",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/testflows/github-runners",
     classifiers=[
```

### Comparing `testflows.github.runners-1.3.230801.1141050/testflows/github/runners/__init__.py` & `testflows.github.runners-1.3.230801.1152824/testflows/github/runners/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 __author__ = "Vitaliy Zakaznikov"
-__version__ = "1.3.230801.1141050"
+__version__ = "1.3.230801.1152824"
 __license__ = f"""
 Copyright 2023 Katteli Inc.
 TestFlows.com Open-Source Software Testing Framework (http://testflows.com)
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `testflows.github.runners-1.3.230801.1141050/testflows/github/runners/actions.py` & `testflows.github.runners-1.3.230801.1152824/testflows/github/runners/actions.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1141050/testflows/github/runners/api_watch.py` & `testflows.github.runners-1.3.230801.1152824/testflows/github/runners/api_watch.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1141050/testflows/github/runners/args.py` & `testflows.github.runners-1.3.230801.1152824/testflows/github/runners/args.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1141050/testflows/github/runners/bin/github-runners` & `testflows.github.runners-1.3.230801.1152824/testflows/github/runners/bin/github-runners`

 * *Files 0% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 
 import testflows.github.runners.args as args
 import testflows.github.runners.cloud as cloud
 import testflows.github.runners.service as service
 import testflows.github.runners.delete as delete
 
 from requests_cache import DO_NOT_CACHE, EXPIRE_IMMEDIATELY, install_cache
+from requests_cache.backends.filesystem import FileCache
 
 description = """Auto-scaling GitHub Actions runners service using Hetzner Cloud.
 
     Service that starts and monitors queued up GitHub Actions workflows.
     When a new job is queued up, it creates new Hetzner Cloud server instance
     that provides an ephemeral GitHub Actions runner. Server is automatically
     powered off when job completes and then powered off servers are
@@ -583,15 +584,15 @@
         name = os.path.join(tempdir, "http_cache")
 
         with Action(f"Enabling HTTP cache at {name}"):
             pass
 
         install_cache(
             name=name,
-            backend="filesystem",
+            backend=FileCache(name),
             cache_control=True,
             urls_expire_after={
                 "*.github.com": EXPIRE_IMMEDIATELY,
                 "*": DO_NOT_CACHE,
             },
         )
```

### Comparing `testflows.github.runners-1.3.230801.1141050/testflows/github/runners/cloud.py` & `testflows.github.runners-1.3.230801.1152824/testflows/github/runners/cloud.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1141050/testflows/github/runners/config.py` & `testflows.github.runners-1.3.230801.1152824/testflows/github/runners/config.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1141050/testflows/github/runners/delete.py` & `testflows.github.runners-1.3.230801.1152824/testflows/github/runners/delete.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1141050/testflows/github/runners/logger.py` & `testflows.github.runners-1.3.230801.1152824/testflows/github/runners/logger.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1141050/testflows/github/runners/request.py` & `testflows.github.runners-1.3.230801.1152824/testflows/github/runners/request.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1141050/testflows/github/runners/scale_down.py` & `testflows.github.runners-1.3.230801.1152824/testflows/github/runners/scale_down.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1141050/testflows/github/runners/scale_up.py` & `testflows.github.runners-1.3.230801.1152824/testflows/github/runners/scale_up.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1141050/testflows/github/runners/scripts/__init__.py` & `testflows.github.runners-1.3.230801.1152824/testflows/github/runners/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1141050/testflows/github/runners/scripts/deploy/__init__.py` & `testflows.github.runners-1.3.230801.1152824/testflows/github/runners/scripts/deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1141050/testflows/github/runners/scripts/deploy/setup.sh` & `testflows.github.runners-1.3.230801.1152824/testflows/github/runners/scripts/deploy/setup.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1141050/testflows/github/runners/scripts/setup_docker.sh` & `testflows.github.runners-1.3.230801.1152824/testflows/github/runners/scripts/setup_docker.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1141050/testflows/github/runners/scripts/startup_arm64.sh` & `testflows.github.runners-1.3.230801.1152824/testflows/github/runners/scripts/startup_arm64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1141050/testflows/github/runners/scripts/startup_x64.sh` & `testflows.github.runners-1.3.230801.1152824/testflows/github/runners/scripts/startup_x64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1141050/testflows/github/runners/server.py` & `testflows.github.runners-1.3.230801.1152824/testflows/github/runners/server.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1141050/testflows/github/runners/service.py` & `testflows.github.runners-1.3.230801.1152824/testflows/github/runners/service.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1141050/testflows/github/runners/shell.py` & `testflows.github.runners-1.3.230801.1152824/testflows/github/runners/shell.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1141050/testflows.github.runners.egg-info/PKG-INFO` & `testflows.github.runners-1.3.230801.1152824/testflows.github.runners.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.3.230801.1141050
+Version: 1.3.230801.1152824
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `testflows.github.runners-1.3.230801.1141050/testflows.github.runners.egg-info/SOURCES.txt` & `testflows.github.runners-1.3.230801.1152824/testflows.github.runners.egg-info/SOURCES.txt`

 * *Files identical despite different names*

