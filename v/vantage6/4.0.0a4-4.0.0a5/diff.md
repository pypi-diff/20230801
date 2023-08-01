# Comparing `tmp/vantage6-4.0.0a4.tar.gz` & `tmp/vantage6-4.0.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vantage6-4.0.0a4.tar", last modified: Mon Jul 24 13:22:27 2023, max compression
+gzip compressed data, was "vantage6-4.0.0a5.tar", last modified: Tue Aug  1 14:00:29 2023, max compression
```

## Comparing `vantage6-4.0.0a4.tar` & `vantage6-4.0.0a5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:27.612513 vantage6-4.0.0a4/
--rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-07-24 13:22:27.612513 vantage6-4.0.0a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 13:22:27.612513 vantage6-4.0.0a4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-24 13:22:06.000000 vantage6-4.0.0a4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:27.608513 vantage6-4.0.0a4/tests_cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:06.000000 vantage6-4.0.0a4/tests_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-24 13:22:06.000000 vantage6-4.0.0a4/tests_cli/test_example.py
--rw-r--r--   0 runner    (1001) docker     (123)    14574 2023-07-24 13:22:06.000000 vantage6-4.0.0a4/tests_cli/test_node_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-07-24 13:22:06.000000 vantage6-4.0.0a4/tests_cli/test_server_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-07-24 13:22:06.000000 vantage6-4.0.0a4/tests_cli/test_wizard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:27.608513 vantage6-4.0.0a4/vantage6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:27.612513 vantage6-4.0.0a4/vantage6/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 13:22:06.000000 vantage6-4.0.0a4/vantage6/cli/__build__
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-24 13:22:06.000000 vantage6-4.0.0a4/vantage6/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-24 13:22:06.000000 vantage6-4.0.0a4/vantage6/cli/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-07-24 13:22:06.000000 vantage6-4.0.0a4/vantage6/cli/configuration_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    11327 2023-07-24 13:22:06.000000 vantage6-4.0.0a4/vantage6/cli/configuration_wizard.py
--rw-r--r--   0 runner    (1001) docker     (123)    13262 2023-07-24 13:22:06.000000 vantage6-4.0.0a4/vantage6/cli/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-24 13:22:06.000000 vantage6-4.0.0a4/vantage6/cli/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)    33998 2023-07-24 13:22:06.000000 vantage6-4.0.0a4/vantage6/cli/node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:27.612513 vantage6-4.0.0a4/vantage6/cli/rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-24 13:22:06.000000 vantage6-4.0.0a4/vantage6/cli/rabbitmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-24 13:22:06.000000 vantage6-4.0.0a4/vantage6/cli/rabbitmq/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-07-24 13:22:06.000000 vantage6-4.0.0a4/vantage6/cli/rabbitmq/queue_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-24 13:22:06.000000 vantage6-4.0.0a4/vantage6/cli/rabbitmq/rabbitmq.config
--rw-r--r--   0 runner    (1001) docker     (123)    28331 2023-07-24 13:22:06.000000 vantage6-4.0.0a4/vantage6/cli/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-24 13:22:06.000000 vantage6-4.0.0a4/vantage6/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:27.608513 vantage6-4.0.0a4/vantage6.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-07-24 13:22:27.000000 vantage6-4.0.0a4/vantage6.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-24 13:22:27.000000 vantage6-4.0.0a4/vantage6.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 13:22:27.000000 vantage6-4.0.0a4/vantage6.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-24 13:22:27.000000 vantage6-4.0.0a4/vantage6.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-24 13:22:27.000000 vantage6-4.0.0a4/vantage6.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-24 13:22:27.000000 vantage6-4.0.0a4/vantage6.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:00:29.591456 vantage6-4.0.0a5/
+-rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-08-01 14:00:29.591456 vantage6-4.0.0a5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 14:00:29.591456 vantage6-4.0.0a5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-08-01 14:00:14.000000 vantage6-4.0.0a5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:00:29.587456 vantage6-4.0.0a5/tests_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 14:00:14.000000 vantage6-4.0.0a5/tests_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-08-01 14:00:14.000000 vantage6-4.0.0a5/tests_cli/test_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14574 2023-08-01 14:00:14.000000 vantage6-4.0.0a5/tests_cli/test_node_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-08-01 14:00:14.000000 vantage6-4.0.0a5/tests_cli/test_server_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-08-01 14:00:14.000000 vantage6-4.0.0a5/tests_cli/test_wizard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:00:29.587456 vantage6-4.0.0a5/vantage6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:00:29.587456 vantage6-4.0.0a5/vantage6/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 14:00:14.000000 vantage6-4.0.0a5/vantage6/cli/__build__
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-01 14:00:14.000000 vantage6-4.0.0a5/vantage6/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-08-01 14:00:14.000000 vantage6-4.0.0a5/vantage6/cli/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-08-01 14:00:14.000000 vantage6-4.0.0a5/vantage6/cli/configuration_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11327 2023-08-01 14:00:14.000000 vantage6-4.0.0a5/vantage6/cli/configuration_wizard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13183 2023-08-01 14:00:14.000000 vantage6-4.0.0a5/vantage6/cli/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-08-01 14:00:14.000000 vantage6-4.0.0a5/vantage6/cli/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33981 2023-08-01 14:00:14.000000 vantage6-4.0.0a5/vantage6/cli/node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:00:29.587456 vantage6-4.0.0a5/vantage6/cli/rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-08-01 14:00:14.000000 vantage6-4.0.0a5/vantage6/cli/rabbitmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-08-01 14:00:14.000000 vantage6-4.0.0a5/vantage6/cli/rabbitmq/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-08-01 14:00:14.000000 vantage6-4.0.0a5/vantage6/cli/rabbitmq/queue_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-01 14:00:14.000000 vantage6-4.0.0a5/vantage6/cli/rabbitmq/rabbitmq.config
+-rw-r--r--   0 runner    (1001) docker     (123)    28331 2023-08-01 14:00:14.000000 vantage6-4.0.0a5/vantage6/cli/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-08-01 14:00:14.000000 vantage6-4.0.0a5/vantage6/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:00:29.587456 vantage6-4.0.0a5/vantage6.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-08-01 14:00:29.000000 vantage6-4.0.0a5/vantage6.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-08-01 14:00:29.000000 vantage6-4.0.0a5/vantage6.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 14:00:29.000000 vantage6-4.0.0a5/vantage6.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-01 14:00:29.000000 vantage6-4.0.0a5/vantage6.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-08-01 14:00:29.000000 vantage6-4.0.0a5/vantage6.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-01 14:00:29.000000 vantage6-4.0.0a5/vantage6.egg-info/top_level.txt
```

### Comparing `vantage6-4.0.0a4/PKG-INFO` & `vantage6-4.0.0a5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: vantage6
-Version: 4.0.0a4
+Version: 4.0.0a5
 Summary: vantage6 command line interface
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
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: vantage6 Version: 4.0.0a4 Summary: vantage6 command
+Metadata-Version: 2.1 Name: vantage6 Version: 4.0.0a5 Summary: vantage6 command
 line interface Home-page: https://github.com/vantage6/vantage6 Requires-Python:
->=3.6 Description-Content-Type: text/markdown Provides-Extra: dev
+>=3.10 Description-Content-Type: text/markdown Provides-Extra: dev
                                     ******
                                [vantage6] ******
           **** A privacy preserving federated learning solution ****
    ****  [![Release](https://github.com/vantage6/vantage6/actions/workflows/
 release.yml/badge.svg)](https://github.com/vantage6/vantage6/actions/workflows/
 release.yml) [![PyPI vantage6](https://badge.fury.io/py/vantage6.svg)](https://
 badge.fury.io/py/vantage6) [![Unittests](https://github.com/vantage6/vantage6/
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

### Comparing `vantage6-4.0.0a4/setup.py` & `vantage6-4.0.0a5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     name='vantage6',
     version=version_ns['__version__'],
     description='vantage6 command line interface',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/vantage6/vantage6',
     packages=find_namespace_packages(),
-    python_requires='>=3.6',
+    python_requires='>=3.10',
     install_requires=[
         'click==8.1.3',
         'colorama==0.4.6',
         'docker==6.1.2',
         'ipython==8.10.0',
         'questionary==1.10.0',
         'schema==0.7.5',
```

### Comparing `vantage6-4.0.0a4/tests_cli/test_node_cli.py` & `vantage6-4.0.0a5/tests_cli/test_node_cli.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.0.0a4/tests_cli/test_server_cli.py` & `vantage6-4.0.0a5/tests_cli/test_server_cli.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.0.0a4/tests_cli/test_wizard.py` & `vantage6-4.0.0a5/tests_cli/test_wizard.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.0.0a4/vantage6/cli/_version.py` & `vantage6-4.0.0a5/vantage6/cli/_version.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.0.0a4/vantage6/cli/configuration_manager.py` & `vantage6-4.0.0a5/vantage6/cli/configuration_manager.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.0.0a4/vantage6/cli/configuration_wizard.py` & `vantage6-4.0.0a5/vantage6/cli/configuration_wizard.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.0.0a4/vantage6/cli/context.py` & `vantage6-4.0.0a5/vantage6/cli/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     for production.
 
 *Node Context*
     In case the node is run in development mode, this context will also used by
     the node package. Normally the node uses the
     `vantage6.node.context.DockerNodeContext` which provides the same
     functionality but is tailored to the Docker environment.
--------------------------------------------------------------------------------
+
 """
 # TODO BvB 2023-01-10 we should have a look at all context classes and define
 # them in the same place. Now the DockerNodeContext is defined in the node, but
 # the server only has a TestServerContext there. This should be made consistent
 from __future__ import annotations
 
 import os.path
```

### Comparing `vantage6-4.0.0a4/vantage6/cli/globals.py` & `vantage6-4.0.0a5/vantage6/cli/globals.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.0.0a4/vantage6/cli/node.py` & `vantage6-4.0.0a5/vantage6/cli/node.py`

 * *Files 0% similar despite different names*

```diff
@@ -221,15 +221,15 @@
               help="Keep image after finishing")
 @click.option('--force-db-mount', is_flag=True,
               help="Skip the check of the existence of the DB (always try to "
                    "mount)")
 @click.option('--attach/--detach', default=False,
               help="Attach node logs to the console after start")
 @click.option('--mount-src', default='',
-              help="mount vantage6-master package source")
+              help="Mount the main vantage6 package source")
 def cli_node_start(name: str, config: str, system_folders: bool, image: str,
                    keep: bool, mount_src: str, attach: bool,
                    force_db_mount: bool) -> None:
     """
     Start the node instance inside a Docker container.
 
     Parameters
@@ -251,15 +251,14 @@
     attach : bool
         Attach node logs to the console after start.
     force_db_mount : bool
         Skip the check of the existence of the DB (always try to mount).
     """
     info("Starting node...")
     info("Finding Docker daemon")
-    print("alhoa")
     docker_client = docker.from_env()
     check_docker_running()
 
     NodeContext.LOGGING_ENABLED = False
     if config:
         name = Path(config).stem
         ctx = NodeContext(name, system_folders, config)
```

### Comparing `vantage6-4.0.0a4/vantage6/cli/rabbitmq/__init__.py` & `vantage6-4.0.0a5/vantage6/cli/rabbitmq/__init__.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.0.0a4/vantage6/cli/rabbitmq/definitions.py` & `vantage6-4.0.0a5/vantage6/cli/rabbitmq/definitions.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.0.0a4/vantage6/cli/rabbitmq/queue_manager.py` & `vantage6-4.0.0a5/vantage6/cli/rabbitmq/queue_manager.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.0.0a4/vantage6/cli/server.py` & `vantage6-4.0.0a5/vantage6/cli/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,15 +119,15 @@
 @click.option('-p', '--port', default=None, type=int, help='port to listen on')
 @click.option('-i', '--image', default=None, help="Server Docker image to use")
 @click.option('--rabbitmq-image', default=None,
               help="RabbitMQ docker image to use")
 @click.option('--keep/--auto-remove', default=False,
               help="Keep image after finishing")
 @click.option('--mount-src', default='',
-              help="mount vantage6-master package source")
+              help="Mount the main vantage6 package source")
 @click.option('--attach/--detach', default=False,
               help="Attach server logs to the console after start")
 @click_insert_context
 def cli_server_start(ctx: ServerContext, ip: str, port: int, image: str,
                      rabbitmq_image: str, keep: bool, mount_src: str,
                      attach: bool) -> None:
     """
@@ -422,32 +422,32 @@
 
 
 #
 #   import
 #
 # TODO this method has a lot of duplicated code from `start`
 @cli_server.command(name='import')
-@click.argument('file_', type=click.Path(exists=True))
+@click.argument('file', type=click.Path(exists=True))
 @click.option('--drop-all', is_flag=True, default=False)
 @click.option('-i', '--image', default=None, help="Node Docker image to use")
 @click.option('--mount-src', default='',
-              help="mount vantage6-master package source")
+              help="Mount the main vantage6 package source")
 @click.option('--keep/--auto-remove', default=False,
               help="Keep image after finishing")
 @click_insert_context
-def cli_server_import(ctx: ServerContext, file_: str, drop_all: bool,
+def cli_server_import(ctx: ServerContext, file: str, drop_all: bool,
                       image: str, mount_src: str, keep: bool) -> None:
     """
     Batch import organizations/collaborations/users and tasks.
 
     Parameters
     ----------
     ctx : ServerContext
         Server context object
-    file_ : str
+    file : str
         Yaml file containing the vantage6 formatted data to import
     drop_all : bool
         Wether to drop all data before importing
     image : str
         Node Docker image to use which contains the import script
     mount_src : str
         Vantage6 source location, this will overwrite the source code in the
@@ -482,15 +482,15 @@
 
     info("Creating mounts")
     mounts = [
         docker.types.Mount(
             "/mnt/config.yaml", str(ctx.config_file), type="bind"
         ),
         docker.types.Mount(
-            "/mnt/import.yaml", str(file_), type="bind"
+            "/mnt/import.yaml", str(file), type="bind"
         )
     ]
 
     # FIXME: code duplication with cli_server_start()
     # try to mount database
     uri = ctx.config['uri']
     url = make_url(uri)
```

### Comparing `vantage6-4.0.0a4/vantage6/cli/utils.py` & `vantage6-4.0.0a5/vantage6/cli/utils.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.0.0a4/vantage6.egg-info/PKG-INFO` & `vantage6-4.0.0a5/vantage6.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: vantage6
-Version: 4.0.0a4
+Version: 4.0.0a5
 Summary: vantage6 command line interface
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
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: vantage6 Version: 4.0.0a4 Summary: vantage6 command
+Metadata-Version: 2.1 Name: vantage6 Version: 4.0.0a5 Summary: vantage6 command
 line interface Home-page: https://github.com/vantage6/vantage6 Requires-Python:
->=3.6 Description-Content-Type: text/markdown Provides-Extra: dev
+>=3.10 Description-Content-Type: text/markdown Provides-Extra: dev
                                     ******
                                [vantage6] ******
           **** A privacy preserving federated learning solution ****
    ****  [![Release](https://github.com/vantage6/vantage6/actions/workflows/
 release.yml/badge.svg)](https://github.com/vantage6/vantage6/actions/workflows/
 release.yml) [![PyPI vantage6](https://badge.fury.io/py/vantage6.svg)](https://
 badge.fury.io/py/vantage6) [![Unittests](https://github.com/vantage6/vantage6/
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

### Comparing `vantage6-4.0.0a4/vantage6.egg-info/SOURCES.txt` & `vantage6-4.0.0a5/vantage6.egg-info/SOURCES.txt`

 * *Files identical despite different names*

