# Comparing `tmp/dagster-docker-0.20.2.tar.gz` & `tmp/dagster-docker-0.20.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-docker-0.20.2.tar", last modified: Fri Jul 21 22:35:41 2023, max compression
+gzip compressed data, was "dagster-docker-0.20.3.tar", last modified: Mon Jul 31 23:06:13 2023, max compression
```

## Comparing `dagster-docker-0.20.2.tar` & `dagster-docker-0.20.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:35:41.201742 dagster-docker-0.20.2/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-07-21 22:28:10.000000 dagster-docker-0.20.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       48 2023-07-21 22:28:10.000000 dagster-docker-0.20.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      606 2023-07-21 22:35:41.201742 dagster-docker-0.20.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      128 2023-07-21 22:28:10.000000 dagster-docker-0.20.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:35:41.197742 dagster-docker-0.20.2/dagster_docker/
--rw-r--r--   0 root         (0) root         (0)      420 2023-07-21 22:28:10.000000 dagster-docker-0.20.2/dagster_docker/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6470 2023-07-21 22:28:10.000000 dagster-docker-0.20.2/dagster_docker/container_context.py
--rw-r--r--   0 root         (0) root         (0)    11733 2023-07-21 22:28:10.000000 dagster-docker-0.20.2/dagster_docker/docker_executor.py
--rw-r--r--   0 root         (0) root         (0)     7426 2023-07-21 22:28:10.000000 dagster-docker-0.20.2/dagster_docker/docker_run_launcher.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:35:41.201742 dagster-docker-0.20.2/dagster_docker/ops/
--rw-r--r--   0 root         (0) root         (0)      143 2023-07-21 22:28:10.000000 dagster-docker-0.20.2/dagster_docker/ops/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6365 2023-07-21 22:28:10.000000 dagster-docker-0.20.2/dagster_docker/ops/docker_container_op.py
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-21 22:28:10.000000 dagster-docker-0.20.2/dagster_docker/py.typed
--rw-r--r--   0 root         (0) root         (0)     1892 2023-07-21 22:28:10.000000 dagster-docker-0.20.2/dagster_docker/utils.py
--rw-r--r--   0 root         (0) root         (0)       23 2023-07-21 22:28:10.000000 dagster-docker-0.20.2/dagster_docker/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:35:41.197742 dagster-docker-0.20.2/dagster_docker.egg-info/
--rw-r--r--   0 root         (0) root         (0)      606 2023-07-21 22:35:41.000000 dagster-docker-0.20.2/dagster_docker.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      556 2023-07-21 22:35:41.000000 dagster-docker-0.20.2/dagster_docker.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 22:35:41.000000 dagster-docker-0.20.2/dagster_docker.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 22:35:41.000000 dagster-docker-0.20.2/dagster_docker.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       48 2023-07-21 22:35:41.000000 dagster-docker-0.20.2/dagster_docker.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-07-21 22:35:41.000000 dagster-docker-0.20.2/dagster_docker.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      125 2023-07-21 22:35:41.201742 dagster-docker-0.20.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1342 2023-07-21 22:28:10.000000 dagster-docker-0.20.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:06:13.157213 dagster-docker-0.20.3/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-07-31 22:58:19.000000 dagster-docker-0.20.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       48 2023-07-31 22:58:19.000000 dagster-docker-0.20.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      606 2023-07-31 23:06:13.157213 dagster-docker-0.20.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      128 2023-07-31 22:58:19.000000 dagster-docker-0.20.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:06:13.153213 dagster-docker-0.20.3/dagster_docker/
+-rw-r--r--   0 root         (0) root         (0)      420 2023-07-31 22:58:19.000000 dagster-docker-0.20.3/dagster_docker/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6470 2023-07-31 22:58:19.000000 dagster-docker-0.20.3/dagster_docker/container_context.py
+-rw-r--r--   0 root         (0) root         (0)    11733 2023-07-31 22:58:19.000000 dagster-docker-0.20.3/dagster_docker/docker_executor.py
+-rw-r--r--   0 root         (0) root         (0)     7426 2023-07-31 22:58:19.000000 dagster-docker-0.20.3/dagster_docker/docker_run_launcher.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:06:13.157213 dagster-docker-0.20.3/dagster_docker/ops/
+-rw-r--r--   0 root         (0) root         (0)      143 2023-07-31 22:58:19.000000 dagster-docker-0.20.3/dagster_docker/ops/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6365 2023-07-31 22:58:19.000000 dagster-docker-0.20.3/dagster_docker/ops/docker_container_op.py
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-31 22:58:19.000000 dagster-docker-0.20.3/dagster_docker/py.typed
+-rw-r--r--   0 root         (0) root         (0)     1892 2023-07-31 22:58:19.000000 dagster-docker-0.20.3/dagster_docker/utils.py
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-31 22:58:19.000000 dagster-docker-0.20.3/dagster_docker/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:06:13.153213 dagster-docker-0.20.3/dagster_docker.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      606 2023-07-31 23:06:13.000000 dagster-docker-0.20.3/dagster_docker.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      556 2023-07-31 23:06:13.000000 dagster-docker-0.20.3/dagster_docker.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 23:06:13.000000 dagster-docker-0.20.3/dagster_docker.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 23:06:13.000000 dagster-docker-0.20.3/dagster_docker.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       48 2023-07-31 23:06:13.000000 dagster-docker-0.20.3/dagster_docker.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-31 23:06:13.000000 dagster-docker-0.20.3/dagster_docker.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      125 2023-07-31 23:06:13.157213 dagster-docker-0.20.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1342 2023-07-31 22:58:19.000000 dagster-docker-0.20.3/setup.py
```

### Comparing `dagster-docker-0.20.2/LICENSE` & `dagster-docker-0.20.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-docker-0.20.2/PKG-INFO` & `dagster-docker-0.20.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-docker
-Version: 0.20.2
+Version: 0.20.3
 Summary: A Dagster integration for docker
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-docker
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-docker-0.20.2/dagster_docker/container_context.py` & `dagster-docker-0.20.3/dagster_docker/container_context.py`

 * *Files identical despite different names*

### Comparing `dagster-docker-0.20.2/dagster_docker/docker_executor.py` & `dagster-docker-0.20.3/dagster_docker/docker_executor.py`

 * *Files identical despite different names*

### Comparing `dagster-docker-0.20.2/dagster_docker/docker_run_launcher.py` & `dagster-docker-0.20.3/dagster_docker/docker_run_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-docker-0.20.2/dagster_docker/ops/docker_container_op.py` & `dagster-docker-0.20.3/dagster_docker/ops/docker_container_op.py`

 * *Files identical despite different names*

### Comparing `dagster-docker-0.20.2/dagster_docker/utils.py` & `dagster-docker-0.20.3/dagster_docker/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-docker-0.20.2/dagster_docker.egg-info/PKG-INFO` & `dagster-docker-0.20.3/dagster_docker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-docker
-Version: 0.20.2
+Version: 0.20.3
 Summary: A Dagster integration for docker
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-docker
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-docker-0.20.2/dagster_docker.egg-info/SOURCES.txt` & `dagster-docker-0.20.3/dagster_docker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-docker-0.20.2/setup.py` & `dagster-docker-0.20.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,10 +30,10 @@
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_docker_tests*"]),
     # urllib3<2 pin needed until docker-py is updated
     # see: https://github.com/docker/docker-py/issues/3113
-    install_requires=["dagster==1.4.2", "docker", "docker-image-py", "urllib3<2"],
+    install_requires=["dagster==1.4.3", "docker", "docker-image-py", "urllib3<2"],
     zip_safe=False,
 )
```

