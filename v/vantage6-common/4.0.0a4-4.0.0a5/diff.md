# Comparing `tmp/vantage6-common-4.0.0a4.tar.gz` & `tmp/vantage6-common-4.0.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vantage6-common-4.0.0a4.tar", last modified: Mon Jul 24 13:22:26 2023, max compression
+gzip compressed data, was "vantage6-common-4.0.0a5.tar", last modified: Tue Aug  1 14:00:28 2023, max compression
```

## Comparing `vantage6-common-4.0.0a4.tar` & `vantage6-common-4.0.0a5.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:26.288429 vantage6-common-4.0.0a4/
--rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-07-24 13:22:26.288429 vantage6-common-4.0.0a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 13:22:26.288429 vantage6-common-4.0.0a4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-24 13:22:06.000000 vantage6-common-4.0.0a4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:26.280429 vantage6-common-4.0.0a4/vantage6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:26.284429 vantage6-common-4.0.0a4/vantage6/common/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 13:22:06.000000 vantage6-common-4.0.0a4/vantage6/common/__build__
--rw-r--r--   0 runner    (1001) docker     (123)     7291 2023-07-24 13:22:06.000000 vantage6-common-4.0.0a4/vantage6/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-24 13:22:06.000000 vantage6-common-4.0.0a4/vantage6/common/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:26.284429 vantage6-common-4.0.0a4/vantage6/common/client/
--rw-r--r--   0 runner    (1001) docker     (123)    14629 2023-07-24 13:22:06.000000 vantage6-common-4.0.0a4/vantage6/common/client/client_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-24 13:22:06.000000 vantage6-common-4.0.0a4/vantage6/common/client/deserialization.py
--rw-r--r--   0 runner    (1001) docker     (123)    12517 2023-07-24 13:22:06.000000 vantage6-common-4.0.0a4/vantage6/common/client/node_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-24 13:22:06.000000 vantage6-common-4.0.0a4/vantage6/common/client/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6906 2023-07-24 13:22:06.000000 vantage6-common-4.0.0a4/vantage6/common/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-07-24 13:22:06.000000 vantage6-common-4.0.0a4/vantage6/common/configuration_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    16764 2023-07-24 13:22:06.000000 vantage6-common-4.0.0a4/vantage6/common/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:26.288429 vantage6-common-4.0.0a4/vantage6/common/docker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:06.000000 vantage6-common-4.0.0a4/vantage6/common/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14583 2023-07-24 13:22:06.000000 vantage6-common-4.0.0a4/vantage6/common/docker/addons.py
--rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-07-24 13:22:06.000000 vantage6-common-4.0.0a4/vantage6/common/docker/network_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    11091 2023-07-24 13:22:06.000000 vantage6-common-4.0.0a4/vantage6/common/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-24 13:22:06.000000 vantage6-common-4.0.0a4/vantage6/common/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-24 13:22:06.000000 vantage6-common-4.0.0a4/vantage6/common/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-07-24 13:22:06.000000 vantage6-common-4.0.0a4/vantage6/common/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-24 13:22:06.000000 vantage6-common-4.0.0a4/vantage6/common/task_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4314 2023-07-24 13:22:06.000000 vantage6-common-4.0.0a4/vantage6/common/utest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:26.288429 vantage6-common-4.0.0a4/vantage6_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-07-24 13:22:26.000000 vantage6-common-4.0.0a4/vantage6_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-24 13:22:26.000000 vantage6-common-4.0.0a4/vantage6_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 13:22:26.000000 vantage6-common-4.0.0a4/vantage6_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-24 13:22:26.000000 vantage6-common-4.0.0a4/vantage6_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-24 13:22:26.000000 vantage6-common-4.0.0a4/vantage6_common.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:00:28.067435 vantage6-common-4.0.0a5/
+-rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-08-01 14:00:28.063435 vantage6-common-4.0.0a5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 14:00:28.067435 vantage6-common-4.0.0a5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-08-01 14:00:14.000000 vantage6-common-4.0.0a5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:00:28.063435 vantage6-common-4.0.0a5/vantage6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:00:28.063435 vantage6-common-4.0.0a5/vantage6/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 14:00:14.000000 vantage6-common-4.0.0a5/vantage6/common/__build__
+-rw-r--r--   0 runner    (1001) docker     (123)     6838 2023-08-01 14:00:14.000000 vantage6-common-4.0.0a5/vantage6/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-08-01 14:00:14.000000 vantage6-common-4.0.0a5/vantage6/common/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:00:28.063435 vantage6-common-4.0.0a5/vantage6/common/client/
+-rw-r--r--   0 runner    (1001) docker     (123)    14629 2023-08-01 14:00:14.000000 vantage6-common-4.0.0a5/vantage6/common/client/client_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-08-01 14:00:14.000000 vantage6-common-4.0.0a5/vantage6/common/client/deserialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12478 2023-08-01 14:00:14.000000 vantage6-common-4.0.0a5/vantage6/common/client/node_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-08-01 14:00:14.000000 vantage6-common-4.0.0a5/vantage6/common/client/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6906 2023-08-01 14:00:14.000000 vantage6-common-4.0.0a5/vantage6/common/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-08-01 14:00:14.000000 vantage6-common-4.0.0a5/vantage6/common/configuration_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16764 2023-08-01 14:00:14.000000 vantage6-common-4.0.0a5/vantage6/common/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:00:28.063435 vantage6-common-4.0.0a5/vantage6/common/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 14:00:14.000000 vantage6-common-4.0.0a5/vantage6/common/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14583 2023-08-01 14:00:14.000000 vantage6-common-4.0.0a5/vantage6/common/docker/addons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-08-01 14:00:14.000000 vantage6-common-4.0.0a5/vantage6/common/docker/network_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11091 2023-08-01 14:00:14.000000 vantage6-common-4.0.0a5/vantage6/common/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-08-01 14:00:14.000000 vantage6-common-4.0.0a5/vantage6/common/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-08-01 14:00:14.000000 vantage6-common-4.0.0a5/vantage6/common/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-08-01 14:00:14.000000 vantage6-common-4.0.0a5/vantage6/common/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-08-01 14:00:14.000000 vantage6-common-4.0.0a5/vantage6/common/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-08-01 14:00:14.000000 vantage6-common-4.0.0a5/vantage6/common/task_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4314 2023-08-01 14:00:14.000000 vantage6-common-4.0.0a5/vantage6/common/utest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:00:28.063435 vantage6-common-4.0.0a5/vantage6_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-08-01 14:00:28.000000 vantage6-common-4.0.0a5/vantage6_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-08-01 14:00:28.000000 vantage6-common-4.0.0a5/vantage6_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 14:00:28.000000 vantage6-common-4.0.0a5/vantage6_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-08-01 14:00:28.000000 vantage6-common-4.0.0a5/vantage6_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-01 14:00:28.000000 vantage6-common-4.0.0a5/vantage6_common.egg-info/top_level.txt
```

### Comparing `vantage6-common-4.0.0a4/PKG-INFO` & `vantage6-common-4.0.0a5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: vantage6-common
-Version: 4.0.0a4
+Version: 4.0.0a5
 Summary: Vantage6 common
 Home-page: https://github.com/vantage6/vantage6
-Requires-Python: >=3.6
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 <h1 align="center">
   <br>
   <a href="https://vantage6.ai"><img src="https://github.com/IKNL/guidelines/blob/master/resources/logos/vantage6.png?raw=true" alt="vantage6" width="350"></a>
 </h1>
 
@@ -31,20 +31,22 @@
 
 
 
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
-Metadata-Version: 2.1 Name: vantage6-common Version: 4.0.0a4 Summary: Vantage6
-common Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.6
+Metadata-Version: 2.1 Name: vantage6-common Version: 4.0.0a5 Summary: Vantage6
+common Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
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

### Comparing `vantage6-common-4.0.0a4/setup.py` & `vantage6-common-4.0.0a5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,25 +27,26 @@
     name='vantage6-common',
     version=version_ns['__version__'],
     description='Vantage6 common',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/vantage6/vantage6',
     packages=find_namespace_packages(),
-    python_requires='>=3.6',
+    python_requires='>=3.10',
     install_requires=[
         'appdirs==1.4.4',
         'click==8.1.3',
         'colorama==0.4.6',
         'cryptography==41.0.0',
         'docker==6.1.2',
         'pyfiglet==0.8.post1',
         'PyJWT==2.6.0',
         'PyYAML==6.0',
         'python-dateutil==2.8.2',
+        'qrcode==7.3.1',
         'requests==2.31.0',
         'schema==0.7.5',
     ],
     package_data={
         'vantage6.common': [
             '__build__',
         ],
```

### Comparing `vantage6-common-4.0.0a4/vantage6/common/__init__.py` & `vantage6-common-4.0.0a5/vantage6/common/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -309,33 +309,11 @@
     label: str
         Label of database configuration to retrieve
 
     Returns
     -------
     Dict | None
         Database configuration, or None if not found
-
-    Notes
-    -----
-    The ``databases`` configuration can be in two formats. The new format
-    allows for the specification of the database type. The structure of the
-    new format is as follows:
-
-    1. Old format:
-    {
-        "database_label": "database_uri",
-        ...
-    }
-
-    2. New format:
-    [
-        {
-            "label": "database_label",
-            "uri": "database_uri",
-            "db_type": "database_type"
-        }
-    ]
-
     """
     for database in databases:
         if database["label"] == label:
             return database
```

### Comparing `vantage6-common-4.0.0a4/vantage6/common/_version.py` & `vantage6-common-4.0.0a5/vantage6/common/_version.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-4.0.0a4/vantage6/common/client/client_base.py` & `vantage6-common-4.0.0a5/vantage6/common/client/client_base.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-4.0.0a4/vantage6/common/client/node_client.py` & `vantage6-common-4.0.0a5/vantage6/common/client/node_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,18 +83,19 @@
                         NODE_CLIENT_REFRESH_BEFORE_EXPIRES_SECONDS + 1)
                 )
 
     def request_token_for_container(self, task_id: int, image: str) -> dict:
         """ Request a container-token at the central server.
 
         This token is used by algorithm containers that run on this
-        node. These algorithms can then post tasks and retrieve
-        child-results (usually refered to as a master container).
+        node. These algorithms can then create subtasks and retrieve
+        subresults.
+
         The server performs a few checks (e.g. if the task you
-        request the key for is still open) before handing out this
+        request the key for is in progress) before handing out this
         token.
 
         Parameters
         ----------
         task_id : int
             id from the task, which is going to use this container token
         image : str
```

### Comparing `vantage6-common-4.0.0a4/vantage6/common/client/utils.py` & `vantage6-common-4.0.0a5/vantage6/common/client/utils.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-4.0.0a4/vantage6/common/colors.py` & `vantage6-common-4.0.0a5/vantage6/common/colors.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-4.0.0a4/vantage6/common/configuration_manager.py` & `vantage6-common-4.0.0a5/vantage6/common/configuration_manager.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-4.0.0a4/vantage6/common/context.py` & `vantage6-common-4.0.0a5/vantage6/common/context.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-4.0.0a4/vantage6/common/docker/addons.py` & `vantage6-common-4.0.0a5/vantage6/common/docker/addons.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-4.0.0a4/vantage6/common/docker/network_manager.py` & `vantage6-common-4.0.0a5/vantage6/common/docker/network_manager.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-4.0.0a4/vantage6/common/encryption.py` & `vantage6-common-4.0.0a5/vantage6/common/encryption.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-4.0.0a4/vantage6/common/globals.py` & `vantage6-common-4.0.0a5/vantage6/common/globals.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-4.0.0a4/vantage6/common/log.py` & `vantage6-common-4.0.0a5/vantage6/common/log.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-4.0.0a4/vantage6/common/task_status.py` & `vantage6-common-4.0.0a5/vantage6/common/task_status.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-4.0.0a4/vantage6/common/utest.py` & `vantage6-common-4.0.0a5/vantage6/common/utest.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-4.0.0a4/vantage6_common.egg-info/PKG-INFO` & `vantage6-common-4.0.0a5/vantage6_common.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: vantage6-common
-Version: 4.0.0a4
+Version: 4.0.0a5
 Summary: Vantage6 common
 Home-page: https://github.com/vantage6/vantage6
-Requires-Python: >=3.6
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 <h1 align="center">
   <br>
   <a href="https://vantage6.ai"><img src="https://github.com/IKNL/guidelines/blob/master/resources/logos/vantage6.png?raw=true" alt="vantage6" width="350"></a>
 </h1>
 
@@ -31,20 +31,22 @@
 
 
 
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
-Metadata-Version: 2.1 Name: vantage6-common Version: 4.0.0a4 Summary: Vantage6
-common Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.6
+Metadata-Version: 2.1 Name: vantage6-common Version: 4.0.0a5 Summary: Vantage6
+common Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
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

### Comparing `vantage6-common-4.0.0a4/vantage6_common.egg-info/SOURCES.txt` & `vantage6-common-4.0.0a5/vantage6_common.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 vantage6/common/colors.py
 vantage6/common/configuration_manager.py
 vantage6/common/context.py
 vantage6/common/encryption.py
 vantage6/common/exceptions.py
 vantage6/common/globals.py
 vantage6/common/log.py
+vantage6/common/serialization.py
 vantage6/common/task_status.py
 vantage6/common/utest.py
 vantage6/common/client/client_base.py
 vantage6/common/client/deserialization.py
 vantage6/common/client/node_client.py
 vantage6/common/client/utils.py
 vantage6/common/docker/__init__.py
```

