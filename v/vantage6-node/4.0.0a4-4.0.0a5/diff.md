# Comparing `tmp/vantage6-node-4.0.0a4.tar.gz` & `tmp/vantage6-node-4.0.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vantage6-node-4.0.0a4.tar", last modified: Mon Jul 24 13:22:28 2023, max compression
+gzip compressed data, was "vantage6-node-4.0.0a5.tar", last modified: Tue Aug  1 14:00:30 2023, max compression
```

## Comparing `vantage6-node-4.0.0a4.tar` & `vantage6-node-4.0.0a5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:28.184549 vantage6-node-4.0.0a4/
--rw-r--r--   0 runner    (1001) docker     (123)     5083 2023-07-24 13:22:28.184549 vantage6-node-4.0.0a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 13:22:28.184549 vantage6-node-4.0.0a4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-07-24 13:22:06.000000 vantage6-node-4.0.0a4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:28.180549 vantage6-node-4.0.0a4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:06.000000 vantage6-node-4.0.0a4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:06.000000 vantage6-node-4.0.0a4/tests/test_ssh_tunnel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:28.180549 vantage6-node-4.0.0a4/vantage6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:28.180549 vantage6-node-4.0.0a4/vantage6/node/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 13:22:06.000000 vantage6-node-4.0.0a4/vantage6/node/__build__
--rw-r--r--   0 runner    (1001) docker     (123)    41597 2023-07-24 13:22:06.000000 vantage6-node-4.0.0a4/vantage6/node/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-24 13:22:06.000000 vantage6-node-4.0.0a4/vantage6/node/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:28.180549 vantage6-node-4.0.0a4/vantage6/node/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:06.000000 vantage6-node-4.0.0a4/vantage6/node/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6884 2023-07-24 13:22:06.000000 vantage6-node-4.0.0a4/vantage6/node/cli/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-07-24 13:22:06.000000 vantage6-node-4.0.0a4/vantage6/node/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:28.180549 vantage6-node-4.0.0a4/vantage6/node/docker/
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-24 13:22:06.000000 vantage6-node-4.0.0a4/vantage6/node/docker/docker_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    23561 2023-07-24 13:22:06.000000 vantage6-node-4.0.0a4/vantage6/node/docker/docker_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-24 13:22:06.000000 vantage6-node-4.0.0a4/vantage6/node/docker/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9089 2023-07-24 13:22:06.000000 vantage6-node-4.0.0a4/vantage6/node/docker/squid.py
--rw-r--r--   0 runner    (1001) docker     (123)     9599 2023-07-24 13:22:06.000000 vantage6-node-4.0.0a4/vantage6/node/docker/ssh_tunnel.py
--rw-r--r--   0 runner    (1001) docker     (123)    19632 2023-07-24 13:22:06.000000 vantage6-node-4.0.0a4/vantage6/node/docker/task_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    23828 2023-07-24 13:22:06.000000 vantage6-node-4.0.0a4/vantage6/node/docker/vpn_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-24 13:22:06.000000 vantage6-node-4.0.0a4/vantage6/node/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11482 2023-07-24 13:22:06.000000 vantage6-node-4.0.0a4/vantage6/node/proxy_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-07-24 13:22:06.000000 vantage6-node-4.0.0a4/vantage6/node/socket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:28.180549 vantage6-node-4.0.0a4/vantage6/node/util/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-24 13:22:06.000000 vantage6-node-4.0.0a4/vantage6/node/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-07-24 13:22:06.000000 vantage6-node-4.0.0a4/vantage6/node/util/colorer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:28.184549 vantage6-node-4.0.0a4/vantage6_node.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5083 2023-07-24 13:22:28.000000 vantage6-node-4.0.0a4/vantage6_node.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-24 13:22:28.000000 vantage6-node-4.0.0a4/vantage6_node.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 13:22:28.000000 vantage6-node-4.0.0a4/vantage6_node.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-24 13:22:28.000000 vantage6-node-4.0.0a4/vantage6_node.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-24 13:22:28.000000 vantage6-node-4.0.0a4/vantage6_node.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-24 13:22:28.000000 vantage6-node-4.0.0a4/vantage6_node.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:00:30.063462 vantage6-node-4.0.0a5/
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-08-01 14:00:30.063462 vantage6-node-4.0.0a5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 14:00:30.063462 vantage6-node-4.0.0a5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-08-01 14:00:14.000000 vantage6-node-4.0.0a5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:00:30.059462 vantage6-node-4.0.0a5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 14:00:14.000000 vantage6-node-4.0.0a5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 14:00:14.000000 vantage6-node-4.0.0a5/tests/test_ssh_tunnel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:00:30.059462 vantage6-node-4.0.0a5/vantage6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:00:30.059462 vantage6-node-4.0.0a5/vantage6/node/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 14:00:14.000000 vantage6-node-4.0.0a5/vantage6/node/__build__
+-rw-r--r--   0 runner    (1001) docker     (123)    41634 2023-08-01 14:00:14.000000 vantage6-node-4.0.0a5/vantage6/node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-08-01 14:00:14.000000 vantage6-node-4.0.0a5/vantage6/node/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:00:30.059462 vantage6-node-4.0.0a5/vantage6/node/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 14:00:14.000000 vantage6-node-4.0.0a5/vantage6/node/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6884 2023-08-01 14:00:14.000000 vantage6-node-4.0.0a5/vantage6/node/cli/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-08-01 14:00:14.000000 vantage6-node-4.0.0a5/vantage6/node/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:00:30.059462 vantage6-node-4.0.0a5/vantage6/node/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-01 14:00:14.000000 vantage6-node-4.0.0a5/vantage6/node/docker/docker_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23561 2023-08-01 14:00:14.000000 vantage6-node-4.0.0a5/vantage6/node/docker/docker_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-08-01 14:00:14.000000 vantage6-node-4.0.0a5/vantage6/node/docker/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9089 2023-08-01 14:00:14.000000 vantage6-node-4.0.0a5/vantage6/node/docker/squid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9599 2023-08-01 14:00:14.000000 vantage6-node-4.0.0a5/vantage6/node/docker/ssh_tunnel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19632 2023-08-01 14:00:14.000000 vantage6-node-4.0.0a5/vantage6/node/docker/task_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23828 2023-08-01 14:00:14.000000 vantage6-node-4.0.0a5/vantage6/node/docker/vpn_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-08-01 14:00:14.000000 vantage6-node-4.0.0a5/vantage6/node/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11482 2023-08-01 14:00:14.000000 vantage6-node-4.0.0a5/vantage6/node/proxy_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-08-01 14:00:14.000000 vantage6-node-4.0.0a5/vantage6/node/socket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:00:30.063462 vantage6-node-4.0.0a5/vantage6/node/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-08-01 14:00:14.000000 vantage6-node-4.0.0a5/vantage6/node/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-08-01 14:00:14.000000 vantage6-node-4.0.0a5/vantage6/node/util/colorer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:00:30.063462 vantage6-node-4.0.0a5/vantage6_node.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-08-01 14:00:30.000000 vantage6-node-4.0.0a5/vantage6_node.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-08-01 14:00:30.000000 vantage6-node-4.0.0a5/vantage6_node.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 14:00:30.000000 vantage6-node-4.0.0a5/vantage6_node.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-08-01 14:00:30.000000 vantage6-node-4.0.0a5/vantage6_node.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-08-01 14:00:30.000000 vantage6-node-4.0.0a5/vantage6_node.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-01 14:00:30.000000 vantage6-node-4.0.0a5/vantage6_node.egg-info/top_level.txt
```

### Comparing `vantage6-node-4.0.0a4/PKG-INFO` & `vantage6-node-4.0.0a5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: vantage6-node
-Version: 4.0.0a4
+Version: 4.0.0a5
 Summary: vantage6 node
 Home-page: https://github.com/vantage6/vantage6
-Requires-Python: >=3.6
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
   <br>
   <a href="https://vantage6.ai"><img src="https://github.com/IKNL/guidelines/blob/master/resources/logos/vantage6.png?raw=true" alt="vantage6" width="350"></a>
 </h1>
@@ -32,20 +32,22 @@
 
 
 
 -----------------------------------------------------------------------------------------------------
 This repository is part of **vantage6**, our **privacy preserving federated learning infrastructure for secure insight exchange**, and contains all the **vantage6** infrastructure source/ code. Please visit our [website (vantage6.ai)](https://vantage6.ai) to learn more!
 
 ## :books: Documentation
-This repository is home to 4 PyPi packages:
+This repository is home to 6 PyPi packages:
 
 * [vantage6](https://pypi.org/project/vantage6) -> _CLI for managing node and server instances_
 * [vantage6-client](https://pypi.org/project/vantage6-client) -> _Python client for interacting with the vantage6-server_
+* [vantage6-algorithm-tools](https://pypi.org/project/vantage6-algorithm-tools) -> _Python tools to facilitate algorithm development_
 * [vantage6-node](https://pypi.org/project/vantage6-node) -> _Node application package_
 * [vantage6-server](https://pypi.org/project/vantage6-server) -> _Server application package_
+* [vantage6-common](https://pypi.org/project/vantage6-common) -> _Server application package_
 
 **Note that when using vantage6 you do not install the _server_ and _node_ packages. These are delivered to you in Docker images.**
 
 Two docker images are published which contain the Node and Server applications:
 
 * `harbor2.vantage6.ai/infrastructure/node:VERSION`
 * `harbor2.vantage6.ai/infrastructure/server:VERSION`
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: vantage6-node Version: 4.0.0a4 Summary: vantage6
-node Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.6
+Metadata-Version: 2.1 Name: vantage6-node Version: 4.0.0a5 Summary: vantage6
+node Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.10
 Description-Content-Type: text/markdown Provides-Extra: dev
                                     ******
                                [vantage6] ******
           **** A privacy preserving federated learning solution ****
    ****  [![Release](https://github.com/vantage6/vantage6/actions/workflows/
 release.yml/badge.svg)](https://github.com/vantage6/vantage6/actions/workflows/
 release.yml) [![PyPI vantage6](https://badge.fury.io/py/vantage6.svg)](https://
@@ -19,32 +19,35 @@
    10.5281/zenodo.7382602.svg)](https://doi.org/10.5281/zenodo.7382602) ****
                  Documentation â¢ Contributing â¢ References
 -------------------------------------------------------------------------------
 ---------------------- This repository is part of **vantage6**, our **privacy
 preserving federated learning infrastructure for secure insight exchange**, and
 contains all the **vantage6** infrastructure source/ code. Please visit our
 [website (vantage6.ai)](https://vantage6.ai) to learn more! ## :books:
-Documentation This repository is home to 4 PyPi packages: * [vantage6](https://
+Documentation This repository is home to 6 PyPi packages: * [vantage6](https://
 pypi.org/project/vantage6) -> _CLI for managing node and server instances_ *
 [vantage6-client](https://pypi.org/project/vantage6-client) -> _Python client
-for interacting with the vantage6-server_ * [vantage6-node](https://pypi.org/
-project/vantage6-node) -> _Node application package_ * [vantage6-server](https:
-//pypi.org/project/vantage6-server) -> _Server application package_ **Note that
-when using vantage6 you do not install the _server_ and _node_ packages. These
-are delivered to you in Docker images.** Two docker images are published which
-contain the Node and Server applications: * `harbor2.vantage6.ai/
-infrastructure/node:VERSION` * `harbor2.vantage6.ai/infrastructure/server:
-VERSION` These docker images are used by the _vantage6 CLI_ package, which can
-be installed by running: `pip install vantage6` This will install the CLI which
-enables you to use the commands: * `vnode CMD [OPTIONS]` * `vserver CMD
-[OPTIONS]` You can find more (user) documentation at [Gitbook
-(docs.vantage6.ai)](https://docs.vantage6.ai). If you have any questions,
-suggestions or just want to chat about federated learning: join our [Dircord
-(https://discord.gg/yAyFf6Y)](https://discord.gg/yAyFf6Y) channel. ## :
-gift_heart: Contributing We hope to continue developing, improving, and
+for interacting with the vantage6-server_ * [vantage6-algorithm-tools](https://
+pypi.org/project/vantage6-algorithm-tools) -> _Python tools to facilitate
+algorithm development_ * [vantage6-node](https://pypi.org/project/vantage6-
+node) -> _Node application package_ * [vantage6-server](https://pypi.org/
+project/vantage6-server) -> _Server application package_ * [vantage6-common]
+(https://pypi.org/project/vantage6-common) -> _Server application package_
+**Note that when using vantage6 you do not install the _server_ and _node_
+packages. These are delivered to you in Docker images.** Two docker images are
+published which contain the Node and Server applications: *
+`harbor2.vantage6.ai/infrastructure/node:VERSION` * `harbor2.vantage6.ai/
+infrastructure/server:VERSION` These docker images are used by the _vantage6
+CLI_ package, which can be installed by running: `pip install vantage6` This
+will install the CLI which enables you to use the commands: * `vnode CMD
+[OPTIONS]` * `vserver CMD [OPTIONS]` You can find more (user) documentation at
+[Gitbook (docs.vantage6.ai)](https://docs.vantage6.ai). If you have any
+questions, suggestions or just want to chat about federated learning: join our
+[Dircord (https://discord.gg/yAyFf6Y)](https://discord.gg/yAyFf6Y) channel. ##
+:gift_heart: Contributing We hope to continue developing, improving, and
 supporting **vantage6** with the help of the federated learning community. If
 you are interested in contributing, first of all, thank you! Second, please
 take a look at our [contributing guidelines](https://docs.vantage6.ai/en/main/
 devops/contribute.html) ## :black_nib: References If you are using
 **vantage6**, please cite this repository as well as the accompanying papers as
 follows: > * F. Martin, M. Sieswerda, H. Alradhi, et al. vantage6. Available at
 https://doi.org/10.5281/zenodo.7221216. Accessed on MONTH, 20XX. > * A.
```

### Comparing `vantage6-node-4.0.0a4/setup.py` & `vantage6-node-4.0.0a5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     name='vantage6-node',
     version=version_ns['__version__'],
     description='vantage6 node',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/vantage6/vantage6',
     packages=find_namespace_packages(),
-    python_requires='>=3.6',
+    python_requires='>=3.10',
     install_requires=[
         'click==8.1.3',
         'docker==6.1.2',
         'gevent==22.10.2',
         'python-socketio==5.7.2',
         'requests==2.31.0',
         f'vantage6 == {version_ns["__version__"]}',
```

### Comparing `vantage6-node-4.0.0a4/vantage6/node/__init__.py` & `vantage6-node-4.0.0a5/vantage6/node/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     new tasks to the task queue.
 *Speaking thread*
     Waits for tasks to finish. When they do, return the results to the central
     server.
 *Proxy server thread*
     Algorithm containers are isolated from the internet for security reasons.
     The local proxy server provides an interface to the central server for
-    *master* containers to create subtasks and retrieve their results.
+    algorithm containers to create subtasks and retrieve their results.
 
 The node connects to the server using a websocket connection. This connection
 is mainly used for sharing status updates. This avoids the need for polling to
 see if there are new tasks available.
 """
 import sys
 import os
@@ -643,26 +643,26 @@
     def setup_squid_proxy(self, isolated_network_mgr: NetworkManager) \
             -> Squid:
         """
         Initiates a Squid proxy if configured in the config.yml
 
         Expects the configuration in the following format:
 
-        ```yaml
-        whitelist:
-            domains:
-                - domain1
-                - domain2
-            ips:
-                - ip1
-                - ip2
-            ports:
-                - port1
-                - port2
-        ```
+        .. code:: yaml
+
+            whitelist:
+                domains:
+                    - domain1
+                    - domain2
+                ips:
+                    - ip1
+                    - ip2
+                ports:
+                    - port1
+                    - port2
 
         Parameters
         ----------
         isolated_network_mgr: NetworkManager
             Network manager for isolated network
 
         Returns
```

### Comparing `vantage6-node-4.0.0a4/vantage6/node/_version.py` & `vantage6-node-4.0.0a5/vantage6/node/_version.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-4.0.0a4/vantage6/node/cli/node.py` & `vantage6-node-4.0.0a5/vantage6/node/cli/node.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-4.0.0a4/vantage6/node/context.py` & `vantage6-node-4.0.0a5/vantage6/node/context.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-4.0.0a4/vantage6/node/docker/docker_base.py` & `vantage6-node-4.0.0a5/vantage6/node/docker/docker_base.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-4.0.0a4/vantage6/node/docker/docker_manager.py` & `vantage6-node-4.0.0a5/vantage6/node/docker/docker_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -345,15 +345,15 @@
         return run_ids_killed
 
     def cleanup(self) -> None:
         """
         Stop all active tasks and delete the isolated network
 
         Note: the temporary docker volumes are kept as they may still be used
-        by a master container
+        by a parent container
         """
         # note: the function `cleanup_tasks` returns a list of tasks that were
         # killed, but we don't register them as killed so they will be run
         # again when the node is restarted
         self.cleanup_tasks()
         for service in self.linked_services:
             self.isolated_network_mgr.disconnect(service)
```

### Comparing `vantage6-node-4.0.0a4/vantage6/node/docker/exceptions.py` & `vantage6-node-4.0.0a5/vantage6/node/docker/exceptions.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-4.0.0a4/vantage6/node/docker/squid.py` & `vantage6-node-4.0.0a5/vantage6/node/docker/squid.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-4.0.0a4/vantage6/node/docker/ssh_tunnel.py` & `vantage6-node-4.0.0a5/vantage6/node/docker/ssh_tunnel.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-4.0.0a4/vantage6/node/docker/task_manager.py` & `vantage6-node-4.0.0a5/vantage6/node/docker/task_manager.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-4.0.0a4/vantage6/node/docker/vpn_manager.py` & `vantage6-node-4.0.0a5/vantage6/node/docker/vpn_manager.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-4.0.0a4/vantage6/node/globals.py` & `vantage6-node-4.0.0a5/vantage6/node/globals.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-4.0.0a4/vantage6/node/proxy_server.py` & `vantage6-node-4.0.0a5/vantage6/node/proxy_server.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-4.0.0a4/vantage6/node/socket.py` & `vantage6-node-4.0.0a5/vantage6/node/socket.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,16 @@
         """
         if self.node_worker_ref:
             self.node_worker_ref.get_task_and_add_to_queue(task_id)
             self.log.info(f'New task has been added task_id={task_id}')
 
         else:
             self.log.critical(
-                'Task Master Node reference not set is socket namespace'
+                'Node reference is not set in socket namespace; cannot create '
+                'new task!'
             )
 
     def on_algorithm_status_change(self, data):
         """
         Actions to be taken when an algorithm container in the collaboration
         has changed its status.
```

### Comparing `vantage6-node-4.0.0a4/vantage6/node/util/colorer.py` & `vantage6-node-4.0.0a5/vantage6/node/util/colorer.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-4.0.0a4/vantage6_node.egg-info/PKG-INFO` & `vantage6-node-4.0.0a5/vantage6_node.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: vantage6-node
-Version: 4.0.0a4
+Version: 4.0.0a5
 Summary: vantage6 node
 Home-page: https://github.com/vantage6/vantage6
-Requires-Python: >=3.6
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
   <br>
   <a href="https://vantage6.ai"><img src="https://github.com/IKNL/guidelines/blob/master/resources/logos/vantage6.png?raw=true" alt="vantage6" width="350"></a>
 </h1>
@@ -32,20 +32,22 @@
 
 
 
 -----------------------------------------------------------------------------------------------------
 This repository is part of **vantage6**, our **privacy preserving federated learning infrastructure for secure insight exchange**, and contains all the **vantage6** infrastructure source/ code. Please visit our [website (vantage6.ai)](https://vantage6.ai) to learn more!
 
 ## :books: Documentation
-This repository is home to 4 PyPi packages:
+This repository is home to 6 PyPi packages:
 
 * [vantage6](https://pypi.org/project/vantage6) -> _CLI for managing node and server instances_
 * [vantage6-client](https://pypi.org/project/vantage6-client) -> _Python client for interacting with the vantage6-server_
+* [vantage6-algorithm-tools](https://pypi.org/project/vantage6-algorithm-tools) -> _Python tools to facilitate algorithm development_
 * [vantage6-node](https://pypi.org/project/vantage6-node) -> _Node application package_
 * [vantage6-server](https://pypi.org/project/vantage6-server) -> _Server application package_
+* [vantage6-common](https://pypi.org/project/vantage6-common) -> _Server application package_
 
 **Note that when using vantage6 you do not install the _server_ and _node_ packages. These are delivered to you in Docker images.**
 
 Two docker images are published which contain the Node and Server applications:
 
 * `harbor2.vantage6.ai/infrastructure/node:VERSION`
 * `harbor2.vantage6.ai/infrastructure/server:VERSION`
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: vantage6-node Version: 4.0.0a4 Summary: vantage6
-node Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.6
+Metadata-Version: 2.1 Name: vantage6-node Version: 4.0.0a5 Summary: vantage6
+node Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.10
 Description-Content-Type: text/markdown Provides-Extra: dev
                                     ******
                                [vantage6] ******
           **** A privacy preserving federated learning solution ****
    ****  [![Release](https://github.com/vantage6/vantage6/actions/workflows/
 release.yml/badge.svg)](https://github.com/vantage6/vantage6/actions/workflows/
 release.yml) [![PyPI vantage6](https://badge.fury.io/py/vantage6.svg)](https://
@@ -19,32 +19,35 @@
    10.5281/zenodo.7382602.svg)](https://doi.org/10.5281/zenodo.7382602) ****
                  Documentation â¢ Contributing â¢ References
 -------------------------------------------------------------------------------
 ---------------------- This repository is part of **vantage6**, our **privacy
 preserving federated learning infrastructure for secure insight exchange**, and
 contains all the **vantage6** infrastructure source/ code. Please visit our
 [website (vantage6.ai)](https://vantage6.ai) to learn more! ## :books:
-Documentation This repository is home to 4 PyPi packages: * [vantage6](https://
+Documentation This repository is home to 6 PyPi packages: * [vantage6](https://
 pypi.org/project/vantage6) -> _CLI for managing node and server instances_ *
 [vantage6-client](https://pypi.org/project/vantage6-client) -> _Python client
-for interacting with the vantage6-server_ * [vantage6-node](https://pypi.org/
-project/vantage6-node) -> _Node application package_ * [vantage6-server](https:
-//pypi.org/project/vantage6-server) -> _Server application package_ **Note that
-when using vantage6 you do not install the _server_ and _node_ packages. These
-are delivered to you in Docker images.** Two docker images are published which
-contain the Node and Server applications: * `harbor2.vantage6.ai/
-infrastructure/node:VERSION` * `harbor2.vantage6.ai/infrastructure/server:
-VERSION` These docker images are used by the _vantage6 CLI_ package, which can
-be installed by running: `pip install vantage6` This will install the CLI which
-enables you to use the commands: * `vnode CMD [OPTIONS]` * `vserver CMD
-[OPTIONS]` You can find more (user) documentation at [Gitbook
-(docs.vantage6.ai)](https://docs.vantage6.ai). If you have any questions,
-suggestions or just want to chat about federated learning: join our [Dircord
-(https://discord.gg/yAyFf6Y)](https://discord.gg/yAyFf6Y) channel. ## :
-gift_heart: Contributing We hope to continue developing, improving, and
+for interacting with the vantage6-server_ * [vantage6-algorithm-tools](https://
+pypi.org/project/vantage6-algorithm-tools) -> _Python tools to facilitate
+algorithm development_ * [vantage6-node](https://pypi.org/project/vantage6-
+node) -> _Node application package_ * [vantage6-server](https://pypi.org/
+project/vantage6-server) -> _Server application package_ * [vantage6-common]
+(https://pypi.org/project/vantage6-common) -> _Server application package_
+**Note that when using vantage6 you do not install the _server_ and _node_
+packages. These are delivered to you in Docker images.** Two docker images are
+published which contain the Node and Server applications: *
+`harbor2.vantage6.ai/infrastructure/node:VERSION` * `harbor2.vantage6.ai/
+infrastructure/server:VERSION` These docker images are used by the _vantage6
+CLI_ package, which can be installed by running: `pip install vantage6` This
+will install the CLI which enables you to use the commands: * `vnode CMD
+[OPTIONS]` * `vserver CMD [OPTIONS]` You can find more (user) documentation at
+[Gitbook (docs.vantage6.ai)](https://docs.vantage6.ai). If you have any
+questions, suggestions or just want to chat about federated learning: join our
+[Dircord (https://discord.gg/yAyFf6Y)](https://discord.gg/yAyFf6Y) channel. ##
+:gift_heart: Contributing We hope to continue developing, improving, and
 supporting **vantage6** with the help of the federated learning community. If
 you are interested in contributing, first of all, thank you! Second, please
 take a look at our [contributing guidelines](https://docs.vantage6.ai/en/main/
 devops/contribute.html) ## :black_nib: References If you are using
 **vantage6**, please cite this repository as well as the accompanying papers as
 follows: > * F. Martin, M. Sieswerda, H. Alradhi, et al. vantage6. Available at
 https://doi.org/10.5281/zenodo.7221216. Accessed on MONTH, 20XX. > * A.
```

### Comparing `vantage6-node-4.0.0a4/vantage6_node.egg-info/SOURCES.txt` & `vantage6-node-4.0.0a5/vantage6_node.egg-info/SOURCES.txt`

 * *Files identical despite different names*

