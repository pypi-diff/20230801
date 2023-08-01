# Comparing `tmp/testflows.github.runners-1.3.230801.1123353.tar.gz` & `tmp/testflows.github.runners-1.3.230801.1141050.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testflows.github.runners-1.3.230801.1123353.tar", last modified: Tue Aug  1 12:33:53 2023, max compression
+gzip compressed data, was "testflows.github.runners-1.3.230801.1141050.tar", last modified: Tue Aug  1 14:10:51 2023, max compression
```

## Comparing `testflows.github.runners-1.3.230801.1123353.tar` & `testflows.github.runners-1.3.230801.1141050.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 12:33:53.362181 testflows.github.runners-1.3.230801.1123353/
--rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1123353/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)    57192 2023-08-01 12:33:53.362181 testflows.github.runners-1.3.230801.1123353/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    56600 2023-07-31 22:43:07.000000 testflows.github.runners-1.3.230801.1123353/README.rst
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-08-01 12:33:53.366182 testflows.github.runners-1.3.230801.1123353/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     2043 2023-08-01 12:33:53.000000 testflows.github.runners-1.3.230801.1123353/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 12:33:53.362181 testflows.github.runners-1.3.230801.1123353/testflows/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 12:33:53.362181 testflows.github.runners-1.3.230801.1123353/testflows/github/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 12:33:53.362181 testflows.github.runners-1.3.230801.1123353/testflows/github/runners/
--rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-08-01 12:33:53.000000 testflows.github.runners-1.3.230801.1123353/testflows/github/runners/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1615 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1123353/testflows/github/runners/actions.py
--rw-rw-r--   0 user      (1000) user      (1000)     1951 2023-08-01 03:44:03.000000 testflows.github.runners-1.3.230801.1123353/testflows/github/runners/api_watch.py
--rw-rw-r--   0 user      (1000) user      (1000)     2599 2023-07-31 15:05:55.000000 testflows.github.runners-1.3.230801.1123353/testflows/github/runners/args.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 12:33:53.362181 testflows.github.runners-1.3.230801.1123353/testflows/github/runners/bin/
--rwxrwxr-x   0 user      (1000) user      (1000)    24416 2023-08-01 12:32:31.000000 testflows.github.runners-1.3.230801.1123353/testflows/github/runners/bin/github-runners
--rw-rw-r--   0 user      (1000) user      (1000)    13607 2023-07-29 23:57:40.000000 testflows.github.runners-1.3.230801.1123353/testflows/github/runners/cloud.py
--rw-rw-r--   0 user      (1000) user      (1000)     4164 2023-08-01 01:08:42.000000 testflows.github.runners-1.3.230801.1123353/testflows/github/runners/config.py
--rw-rw-r--   0 user      (1000) user      (1000)     2473 2023-07-29 23:43:11.000000 testflows.github.runners-1.3.230801.1123353/testflows/github/runners/delete.py
--rw-rw-r--   0 user      (1000) user      (1000)      726 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1123353/testflows/github/runners/logger.py
--rw-rw-r--   0 user      (1000) user      (1000)     1926 2023-07-29 23:39:43.000000 testflows.github.runners-1.3.230801.1123353/testflows/github/runners/request.py
--rw-rw-r--   0 user      (1000) user      (1000)    11279 2023-08-01 03:43:12.000000 testflows.github.runners-1.3.230801.1123353/testflows/github/runners/scale_down.py
--rw-rw-r--   0 user      (1000) user      (1000)    17362 2023-08-01 03:14:02.000000 testflows.github.runners-1.3.230801.1123353/testflows/github/runners/scale_up.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 12:33:53.362181 testflows.github.runners-1.3.230801.1123353/testflows/github/runners/scripts/
--rw-rw-r--   0 user      (1000) user      (1000)     1061 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1123353/testflows/github/runners/scripts/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 12:33:53.362181 testflows.github.runners-1.3.230801.1123353/testflows/github/runners/scripts/deploy/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1123353/testflows/github/runners/scripts/deploy/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      519 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1123353/testflows/github/runners/scripts/deploy/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      260 2023-07-31 12:43:19.000000 testflows.github.runners-1.3.230801.1123353/testflows/github/runners/scripts/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)     1148 2023-07-31 12:59:30.000000 testflows.github.runners-1.3.230801.1123353/testflows/github/runners/scripts/setup_docker.sh
--rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1123353/testflows/github/runners/scripts/startup_arm64.sh
--rw-rw-r--   0 user      (1000) user      (1000)      715 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1123353/testflows/github/runners/scripts/startup_x64.sh
--rw-rw-r--   0 user      (1000) user      (1000)     2522 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1123353/testflows/github/runners/server.py
--rw-rw-r--   0 user      (1000) user      (1000)     5158 2023-07-31 17:30:38.000000 testflows.github.runners-1.3.230801.1123353/testflows/github/runners/service.py
--rw-rw-r--   0 user      (1000) user      (1000)     1483 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1123353/testflows/github/runners/shell.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 12:33:53.362181 testflows.github.runners-1.3.230801.1123353/testflows.github.runners.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    57192 2023-08-01 12:33:53.000000 testflows.github.runners-1.3.230801.1123353/testflows.github.runners.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1192 2023-08-01 12:33:53.000000 testflows.github.runners-1.3.230801.1123353/testflows.github.runners.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-08-01 12:33:53.000000 testflows.github.runners-1.3.230801.1123353/testflows.github.runners.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-29 01:22:42.000000 testflows.github.runners-1.3.230801.1123353/testflows.github.runners.egg-info/not-zip-safe
--rw-rw-r--   0 user      (1000) user      (1000)       61 2023-08-01 12:33:53.000000 testflows.github.runners-1.3.230801.1123353/testflows.github.runners.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       10 2023-08-01 12:33:53.000000 testflows.github.runners-1.3.230801.1123353/testflows.github.runners.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 14:10:51.023690 testflows.github.runners-1.3.230801.1141050/
+-rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1141050/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)    57192 2023-08-01 14:10:51.023690 testflows.github.runners-1.3.230801.1141050/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    56600 2023-07-31 22:43:07.000000 testflows.github.runners-1.3.230801.1141050/README.rst
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-08-01 14:10:51.023690 testflows.github.runners-1.3.230801.1141050/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     2043 2023-08-01 14:10:50.000000 testflows.github.runners-1.3.230801.1141050/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 14:10:51.019690 testflows.github.runners-1.3.230801.1141050/testflows/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 14:10:51.019690 testflows.github.runners-1.3.230801.1141050/testflows/github/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 14:10:51.019690 testflows.github.runners-1.3.230801.1141050/testflows/github/runners/
+-rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-08-01 14:10:50.000000 testflows.github.runners-1.3.230801.1141050/testflows/github/runners/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1615 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1141050/testflows/github/runners/actions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1951 2023-08-01 03:44:03.000000 testflows.github.runners-1.3.230801.1141050/testflows/github/runners/api_watch.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2599 2023-07-31 15:05:55.000000 testflows.github.runners-1.3.230801.1141050/testflows/github/runners/args.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 14:10:51.019690 testflows.github.runners-1.3.230801.1141050/testflows/github/runners/bin/
+-rwxrwxr-x   0 user      (1000) user      (1000)    24893 2023-08-01 14:07:13.000000 testflows.github.runners-1.3.230801.1141050/testflows/github/runners/bin/github-runners
+-rw-rw-r--   0 user      (1000) user      (1000)    13607 2023-07-29 23:57:40.000000 testflows.github.runners-1.3.230801.1141050/testflows/github/runners/cloud.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4164 2023-08-01 01:08:42.000000 testflows.github.runners-1.3.230801.1141050/testflows/github/runners/config.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2473 2023-07-29 23:43:11.000000 testflows.github.runners-1.3.230801.1141050/testflows/github/runners/delete.py
+-rw-rw-r--   0 user      (1000) user      (1000)      726 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1141050/testflows/github/runners/logger.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1926 2023-07-29 23:39:43.000000 testflows.github.runners-1.3.230801.1141050/testflows/github/runners/request.py
+-rw-rw-r--   0 user      (1000) user      (1000)    11279 2023-08-01 03:43:12.000000 testflows.github.runners-1.3.230801.1141050/testflows/github/runners/scale_down.py
+-rw-rw-r--   0 user      (1000) user      (1000)    17362 2023-08-01 03:14:02.000000 testflows.github.runners-1.3.230801.1141050/testflows/github/runners/scale_up.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 14:10:51.019690 testflows.github.runners-1.3.230801.1141050/testflows/github/runners/scripts/
+-rw-rw-r--   0 user      (1000) user      (1000)     1061 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1141050/testflows/github/runners/scripts/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 14:10:51.019690 testflows.github.runners-1.3.230801.1141050/testflows/github/runners/scripts/deploy/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1141050/testflows/github/runners/scripts/deploy/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      519 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1141050/testflows/github/runners/scripts/deploy/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      260 2023-07-31 12:43:19.000000 testflows.github.runners-1.3.230801.1141050/testflows/github/runners/scripts/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)     1148 2023-07-31 12:59:30.000000 testflows.github.runners-1.3.230801.1141050/testflows/github/runners/scripts/setup_docker.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1141050/testflows/github/runners/scripts/startup_arm64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      715 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1141050/testflows/github/runners/scripts/startup_x64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)     2522 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1141050/testflows/github/runners/server.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5158 2023-07-31 17:30:38.000000 testflows.github.runners-1.3.230801.1141050/testflows/github/runners/service.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1483 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1141050/testflows/github/runners/shell.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 14:10:51.019690 testflows.github.runners-1.3.230801.1141050/testflows.github.runners.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    57192 2023-08-01 14:10:50.000000 testflows.github.runners-1.3.230801.1141050/testflows.github.runners.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1192 2023-08-01 14:10:50.000000 testflows.github.runners-1.3.230801.1141050/testflows.github.runners.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-08-01 14:10:50.000000 testflows.github.runners-1.3.230801.1141050/testflows.github.runners.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-29 01:22:42.000000 testflows.github.runners-1.3.230801.1141050/testflows.github.runners.egg-info/not-zip-safe
+-rw-rw-r--   0 user      (1000) user      (1000)       61 2023-08-01 14:10:50.000000 testflows.github.runners-1.3.230801.1141050/testflows.github.runners.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       10 2023-08-01 14:10:50.000000 testflows.github.runners-1.3.230801.1141050/testflows.github.runners.egg-info/top_level.txt
```

### Comparing `testflows.github.runners-1.3.230801.1123353/LICENSE` & `testflows.github.runners-1.3.230801.1141050/LICENSE`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1123353/PKG-INFO` & `testflows.github.runners-1.3.230801.1141050/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.3.230801.1123353
+Version: 1.3.230801.1141050
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `testflows.github.runners-1.3.230801.1123353/README.rst` & `testflows.github.runners-1.3.230801.1141050/README.rst`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1123353/setup.py` & `testflows.github.runners-1.3.230801.1141050/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 with open("README.rst", "r", encoding="utf-8") as fd:
     long_description = fd.read()
 
 
 setup(
     name="testflows.github.runners",
-    version="1.3.230801.1123353",
+    version="1.3.230801.1141050",
     description="Autoscaling GitHub Actions Runners Using Hetzner Cloud ",
     author="Vitaliy Zakaznikov",
     author_email="vzakaznikov@testflows.com",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/testflows/github-runners",
     classifiers=[
```

### Comparing `testflows.github.runners-1.3.230801.1123353/testflows/github/runners/__init__.py` & `testflows.github.runners-1.3.230801.1141050/testflows/github/runners/__init__.py`

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
-__version__ = "1.3.230801.1123353"
+__version__ = "1.3.230801.1141050"
 __license__ = f"""
 Copyright 2023 Katteli Inc.
 TestFlows.com Open-Source Software Testing Framework (http://testflows.com)
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `testflows.github.runners-1.3.230801.1123353/testflows/github/runners/actions.py` & `testflows.github.runners-1.3.230801.1141050/testflows/github/runners/actions.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1123353/testflows/github/runners/api_watch.py` & `testflows.github.runners-1.3.230801.1141050/testflows/github/runners/api_watch.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1123353/testflows/github/runners/args.py` & `testflows.github.runners-1.3.230801.1141050/testflows/github/runners/args.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1123353/testflows/github/runners/bin/github-runners` & `testflows.github.runners-1.3.230801.1141050/testflows/github/runners/bin/github-runners`

 * *Files 2% similar despite different names*

```diff
@@ -9,21 +9,24 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+import os
 import sys
 import time
 import hashlib
+import tempfile
 import logging
 import threading
 import logging.config
 
+from contextlib import contextmanager
 from concurrent.futures import ThreadPoolExecutor, Future
 
 from hcloud import Client
 from hcloud.ssh_keys.domain import SSHKey
 
 from github import Github
 from github.Repository import Repository
@@ -42,23 +45,14 @@
 import testflows.github.runners.args as args
 import testflows.github.runners.cloud as cloud
 import testflows.github.runners.service as service
 import testflows.github.runners.delete as delete
 
 from requests_cache import DO_NOT_CACHE, EXPIRE_IMMEDIATELY, install_cache
 
-install_cache(
-    backend="filesystem",
-    cache_control=True,
-    urls_expire_after={
-        "*.github.com": EXPIRE_IMMEDIATELY,
-        "*": DO_NOT_CACHE,
-    },
-)
-
 description = """Auto-scaling GitHub Actions runners service using Hetzner Cloud.
 
     Service that starts and monitors queued up GitHub Actions workflows.
     When a new job is queued up, it creates new Hetzner Cloud server instance
     that provides an ephemeral GitHub Actions runner. Server is automatically
     powered off when job completes and then powered off servers are
     automatically deleted.
@@ -578,14 +572,36 @@
         help="follow the logs journal",
     )
     logs_service_parser.set_defaults(func=service.logs)
 
     return parser
 
 
+@contextmanager
+def http_cache():
+    """Enable caching of HTTP requests to GitHub api."""
+    with tempfile.TemporaryDirectory() as tempdir:
+        name = os.path.join(tempdir, "http_cache")
+
+        with Action(f"Enabling HTTP cache at {name}"):
+            pass
+
+        install_cache(
+            name=name,
+            backend="filesystem",
+            cache_control=True,
+            urls_expire_after={
+                "*.github.com": EXPIRE_IMMEDIATELY,
+                "*": DO_NOT_CACHE,
+            },
+        )
+
+        yield
+
+
 def main(
     config, scripts: Scripts, worker_pool: ThreadPoolExecutor, terminate_timeout=30
 ):
     """Auto-scale runners service."""
 
     terminate = threading.Event()
 
@@ -755,11 +771,12 @@
             if config.debug:
                 raise
             logger.fatal(f"❗ Error: {exc}")
 
     else:
         config.check()
 
-        with ThreadPoolExecutor(
-            max_workers=config.workers + 3, thread_name_prefix="worker"
-        ) as worker_pool:
-            main(config=config, scripts=scripts, worker_pool=worker_pool)
+        with http_cache():
+            with ThreadPoolExecutor(
+                max_workers=config.workers + 3, thread_name_prefix="worker"
+            ) as worker_pool:
+                main(config=config, scripts=scripts, worker_pool=worker_pool)
```

### Comparing `testflows.github.runners-1.3.230801.1123353/testflows/github/runners/cloud.py` & `testflows.github.runners-1.3.230801.1141050/testflows/github/runners/cloud.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1123353/testflows/github/runners/config.py` & `testflows.github.runners-1.3.230801.1141050/testflows/github/runners/config.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1123353/testflows/github/runners/delete.py` & `testflows.github.runners-1.3.230801.1141050/testflows/github/runners/delete.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1123353/testflows/github/runners/logger.py` & `testflows.github.runners-1.3.230801.1141050/testflows/github/runners/logger.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1123353/testflows/github/runners/request.py` & `testflows.github.runners-1.3.230801.1141050/testflows/github/runners/request.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1123353/testflows/github/runners/scale_down.py` & `testflows.github.runners-1.3.230801.1141050/testflows/github/runners/scale_down.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1123353/testflows/github/runners/scale_up.py` & `testflows.github.runners-1.3.230801.1141050/testflows/github/runners/scale_up.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1123353/testflows/github/runners/scripts/__init__.py` & `testflows.github.runners-1.3.230801.1141050/testflows/github/runners/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1123353/testflows/github/runners/scripts/deploy/__init__.py` & `testflows.github.runners-1.3.230801.1141050/testflows/github/runners/scripts/deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1123353/testflows/github/runners/scripts/deploy/setup.sh` & `testflows.github.runners-1.3.230801.1141050/testflows/github/runners/scripts/deploy/setup.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1123353/testflows/github/runners/scripts/setup_docker.sh` & `testflows.github.runners-1.3.230801.1141050/testflows/github/runners/scripts/setup_docker.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1123353/testflows/github/runners/scripts/startup_arm64.sh` & `testflows.github.runners-1.3.230801.1141050/testflows/github/runners/scripts/startup_arm64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1123353/testflows/github/runners/scripts/startup_x64.sh` & `testflows.github.runners-1.3.230801.1141050/testflows/github/runners/scripts/startup_x64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1123353/testflows/github/runners/server.py` & `testflows.github.runners-1.3.230801.1141050/testflows/github/runners/server.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1123353/testflows/github/runners/service.py` & `testflows.github.runners-1.3.230801.1141050/testflows/github/runners/service.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1123353/testflows/github/runners/shell.py` & `testflows.github.runners-1.3.230801.1141050/testflows/github/runners/shell.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1123353/testflows.github.runners.egg-info/PKG-INFO` & `testflows.github.runners-1.3.230801.1141050/testflows.github.runners.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.3.230801.1123353
+Version: 1.3.230801.1141050
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `testflows.github.runners-1.3.230801.1123353/testflows.github.runners.egg-info/SOURCES.txt` & `testflows.github.runners-1.3.230801.1141050/testflows.github.runners.egg-info/SOURCES.txt`

 * *Files identical despite different names*

