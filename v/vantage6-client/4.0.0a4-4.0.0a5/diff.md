# Comparing `tmp/vantage6-client-4.0.0a4.tar.gz` & `tmp/vantage6-client-4.0.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vantage6-client-4.0.0a4.tar", last modified: Mon Jul 24 13:22:27 2023, max compression
+gzip compressed data, was "vantage6-client-4.0.0a5.tar", last modified: Tue Aug  1 14:00:28 2023, max compression
```

## Comparing `vantage6-client-4.0.0a4.tar` & `vantage6-client-4.0.0a5.tar`

### file list

```diff
@@ -1,34 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:27.060478 vantage6-client-4.0.0a4/
--rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-07-24 13:22:27.060478 vantage6-client-4.0.0a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 13:22:27.060478 vantage6-client-4.0.0a4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-07-24 13:22:06.000000 vantage6-client-4.0.0a4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:27.056478 vantage6-client-4.0.0a4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-24 13:22:06.000000 vantage6-client-4.0.0a4/tests/algorithm_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-07-24 13:22:06.000000 vantage6-client-4.0.0a4/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-24 13:22:06.000000 vantage6-client-4.0.0a4/tests/test_deserialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-07-24 13:22:06.000000 vantage6-client-4.0.0a4/tests/test_docker_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-24 13:22:06.000000 vantage6-client-4.0.0a4/tests/test_serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:27.056478 vantage6-client-4.0.0a4/vantage6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:27.056478 vantage6-client-4.0.0a4/vantage6/client/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 13:22:06.000000 vantage6-client-4.0.0a4/vantage6/client/__build__
--rw-r--r--   0 runner    (1001) docker     (123)    58214 2023-07-24 13:22:06.000000 vantage6-client-4.0.0a4/vantage6/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-24 13:22:06.000000 vantage6-client-4.0.0a4/vantage6/client/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    17789 2023-07-24 13:22:06.000000 vantage6-client-4.0.0a4/vantage6/client/algorithm_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-24 13:22:06.000000 vantage6-client-4.0.0a4/vantage6/client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-07-24 13:22:06.000000 vantage6-client-4.0.0a4/vantage6/client/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-24 13:22:06.000000 vantage6-client-4.0.0a4/vantage6/client/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:27.060478 vantage6-client-4.0.0a4/vantage6/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:06.000000 vantage6-client-4.0.0a4/vantage6/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-07-24 13:22:06.000000 vantage6-client-4.0.0a4/vantage6/tools/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-24 13:22:06.000000 vantage6-client-4.0.0a4/vantage6/tools/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    22159 2023-07-24 13:22:06.000000 vantage6-client-4.0.0a4/vantage6/tools/mock_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-24 13:22:06.000000 vantage6-client-4.0.0a4/vantage6/tools/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-24 13:22:06.000000 vantage6-client-4.0.0a4/vantage6/tools/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-07-24 13:22:06.000000 vantage6-client-4.0.0a4/vantage6/tools/wrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-07-24 13:22:06.000000 vantage6-client-4.0.0a4/vantage6/tools/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:27.060478 vantage6-client-4.0.0a4/vantage6_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-07-24 13:22:27.000000 vantage6-client-4.0.0a4/vantage6_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-24 13:22:27.000000 vantage6-client-4.0.0a4/vantage6_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 13:22:27.000000 vantage6-client-4.0.0a4/vantage6_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-24 13:22:27.000000 vantage6-client-4.0.0a4/vantage6_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-24 13:22:27.000000 vantage6-client-4.0.0a4/vantage6_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:00:28.699443 vantage6-client-4.0.0a5/
+-rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-08-01 14:00:28.699443 vantage6-client-4.0.0a5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 14:00:28.699443 vantage6-client-4.0.0a5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-08-01 14:00:14.000000 vantage6-client-4.0.0a5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:00:28.699443 vantage6-client-4.0.0a5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-08-01 14:00:14.000000 vantage6-client-4.0.0a5/tests/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:00:28.699443 vantage6-client-4.0.0a5/vantage6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:00:28.699443 vantage6-client-4.0.0a5/vantage6/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 14:00:14.000000 vantage6-client-4.0.0a5/vantage6/client/__build__
+-rw-r--r--   0 runner    (1001) docker     (123)    54889 2023-08-01 14:00:14.000000 vantage6-client-4.0.0a5/vantage6/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-08-01 14:00:14.000000 vantage6-client-4.0.0a5/vantage6/client/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-08-01 14:00:14.000000 vantage6-client-4.0.0a5/vantage6/client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8006 2023-08-01 14:00:14.000000 vantage6-client-4.0.0a5/vantage6/client/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-08-01 14:00:14.000000 vantage6-client-4.0.0a5/vantage6/client/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:00:28.699443 vantage6-client-4.0.0a5/vantage6_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-08-01 14:00:28.000000 vantage6-client-4.0.0a5/vantage6_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-08-01 14:00:28.000000 vantage6-client-4.0.0a5/vantage6_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 14:00:28.000000 vantage6-client-4.0.0a5/vantage6_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-01 14:00:28.000000 vantage6-client-4.0.0a5/vantage6_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-01 14:00:28.000000 vantage6-client-4.0.0a5/vantage6_client.egg-info/top_level.txt
```

### Comparing `vantage6-client-4.0.0a4/PKG-INFO` & `vantage6-client-4.0.0a5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: vantage6-client
-Version: 4.0.0a4
+Version: 4.0.0a5
 Summary: Vantage6 client
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
-Metadata-Version: 2.1 Name: vantage6-client Version: 4.0.0a4 Summary: Vantage6
-client Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.6
+Metadata-Version: 2.1 Name: vantage6-client Version: 4.0.0a5 Summary: Vantage6
+client Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.10
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

### Comparing `vantage6-client-4.0.0a4/setup.py` & `vantage6-client-4.0.0a5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,26 +28,20 @@
     name='vantage6-client',
     version=version_ns['__version__'],
     description='Vantage6 client',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/vantage6/vantage6',
     packages=find_namespace_packages(),
-    python_requires='>=3.6',
+    python_requires='>=3.10',
     install_requires=[
-        'pandas==1.5.3',
         'PyJWT==2.6.0',
         'pyfiglet==0.8.post1',
-        'SPARQLWrapper==2.0.0',
-        'qrcode==7.3.1',
         f'vantage6-common=={version_ns["__version__"]}',
     ],
     tests_require=["pytest"],
     package_data={
         'vantage6.client': [
             '__build__',
-        ],
-        'vantage6.tools': [
-            '__build__'
-        ],
+        ]
     }
 )
```

### Comparing `vantage6-client-4.0.0a4/tests/test_client.py` & `vantage6-client-4.0.0a5/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-4.0.0a4/vantage6/client/__init__.py` & `vantage6-client-4.0.0a5/vantage6/client/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,7 @@
-"""
-vantage6 clients
-
-This module is contains a base client. From this base client the container
-client (client used by master algorithms) and the user client are derived.
-"""
 from __future__ import annotations
 
 import logging
 import time
 import typing
 import jwt
 import pyfiglet
@@ -16,15 +10,15 @@
 import traceback
 
 from pathlib import Path
 
 from vantage6.common.globals import APPNAME
 from vantage6.common.encryption import RSACryptor
 from vantage6.common import WhoAmI
-from vantage6.tools import serialization
+from vantage6.common.serialization import serialize
 from vantage6.client.filter import post_filtering
 from vantage6.common.client.utils import print_qr_code
 from vantage6.client.utils import LogLevel
 from vantage6.common.task_status import TaskStatus
 from vantage6.common.client.client_base import ClientBase
 
 
@@ -404,16 +398,15 @@
     class Collaboration(ClientBase.SubClient):
         """Collection of collaboration requests"""
 
         @post_filtering()
         def list(self, scope: str = 'organization',
                  name: str = None, encrypted: bool = None,
                  organization: int = None, page: int = 1,
-                 per_page: int = 20, include_metadata: bool = True,
-                 ) -> dict:
+                 per_page: int = 20) -> dict:
             """View your collaborations
 
             Parameters
             ----------
             scope : str, optional
                 Scope of the list, accepted values are `organization` and
                 `global`. In case of `organization` you get the collaborations
@@ -425,35 +418,29 @@
                 Filter collaborations by organization id
             encrypted: bool, optional
                 Filter collaborations by whether or not they are encrypted
             page: int, optional
                 Pagination page, by default 1
             per_page: int, optional
                 Number of items on a single page, by default 20
-            include_metadata: bool, optional
-                Whenever to include the pagination metadata. If this is
-                set to False the output is no longer wrapped in a
-                dictonairy, by default True
 
             Returns
             -------
             list of dicts
                 Containing collabotation information
 
             Notes
             -----
             - Pagination does not work in combination with scope
               `organization` as pagination is missing at endpoint
               /organization/<id>/collaboration
             """
-            includes = ['metadata'] if include_metadata else []
             params = {
-                'page': page, 'per_page': per_page, 'include': includes,
-                'name': name, 'encrypted': encrypted,
-                'organization_id': organization,
+                'page': page, 'per_page': per_page, 'name': name,
+                'encrypted': encrypted, 'organization_id': organization,
             }
             if scope == 'organization':
                 self.parent.log.info('pagination for scope `organization` '
                                      'not available')
                 org_id = self.parent.whoami.organization_id
                 return self.parent.request(
                     f'organization/{org_id}/collaboration'
@@ -527,15 +514,14 @@
             return self.parent.request(f'node/{id_}')
 
         @post_filtering()
         def list(self, name: str = None, organization: int = None,
                  collaboration: int = None, is_online: bool = None,
                  ip: str = None, last_seen_from: str = None,
                  last_seen_till: str = None, page: int = 1, per_page: int = 20,
-                 include_metadata: bool = True,
                  ) -> list[dict]:
             """List nodes
 
             Parameters
             ----------
             name: str, optional
                 Filter by name (with LIKE operator)
@@ -551,28 +537,23 @@
                 Filter if node has been online since date (format: yyyy-mm-dd)
             last_seen_till: str, optional
                 Filter if node has been online until date (format: yyyy-mm-dd)
             page: int, optional
                 Pagination page, by default 1
             per_page: int, optional
                 Number of items on a single page, by default 20
-            include_metadata: bool, optional
-                Whenever to include the pagination metadata. If this is
-                set to False the output is no longer wrapped in a
-                dictonairy, by default True
 
             Returns
             -------
 
             list of dicts
                 Containing meta-data of the nodes
             """
-            includes = ['metadata'] if include_metadata else []
             params = {
-                'page': page, 'per_page': per_page, 'include': includes,
+                'page': page, 'per_page': per_page,
                 'name': name, 'organization_id': organization,
                 'collaboration_id': collaboration, 'ip': ip,
                 'last_seen_from': last_seen_from,
                 'last_seen_till': last_seen_till
             }
             if is_online is not None:
                 params['status'] = 'online' if is_online else 'offline'
@@ -673,15 +654,14 @@
     class Organization(ClientBase.SubClient):
         """Collection of organization requests"""
 
         @post_filtering()
         def list(
             self, name: str = None, country: int = None,
             collaboration: int = None, page: int = None, per_page: int = None,
-            include_metadata: bool = True
         ) -> list[dict]:
             """List organizations
 
             Parameters
             ----------
             name: str, optional
                 Filter by name (with LIKE operator)
@@ -689,29 +669,23 @@
                 Filter by country
             collaboration: int, optional
                 Filter by collaboration id
             page: int, optional
                 Pagination page, by default 1
             per_page: int, optional
                 Number of items on a single page, by default 20
-            include_metadata: bool, optional
-                Whenever to include the pagination metadata. If this is
-                set to False the output is no longer wrapped in a
-                dictonairy, by default True
 
             Returns
             -------
             list[dict]
                 Containing meta-data information of the organizations
             """
-            includes = ['metadata'] if include_metadata else []
             params = {
-                'page': page, 'per_page': per_page, 'include': includes,
-                'name': name, 'country': country,
-                'collaboration_id': collaboration
+                'page': page, 'per_page': per_page, 'name': name,
+                'country': country, 'collaboration_id': collaboration
             }
             return self.parent.request('organization', params=params)
 
         @post_filtering(iterable=False)
         def get(self, id_: int = None) -> dict:
             """View specific organization
 
@@ -828,16 +802,15 @@
     class User(ClientBase.SubClient):
 
         @post_filtering()
         def list(self, username: str = None, organization: int = None,
                  firstname: str = None, lastname: str = None,
                  email: str = None, role: int = None, rule: int = None,
                  last_seen_from: str = None, last_seen_till: str = None,
-                 page: int = 1, per_page: int = 20,
-                 include_metadata: bool = True) -> list:
+                 page: int = 1, per_page: int = 20) -> list:
             """List users
 
             Parameters
             ----------
             username: str, optional
                 Filter by username (with LIKE operator)
             organization: int, optional
@@ -856,27 +829,22 @@
                 Filter users that have logged on since (format yyyy-mm-dd)
             last_seen_till: str, optional
                 Filter users that have logged on until (format yyyy-mm-dd)
             page: int, optional
                 Pagination page, by default 1
             per_page: int, optional
                 Number of items on a single page, by default 20
-            include_metadata: bool, optional
-                Whenever to include the pagination metadata. If this is
-                set to False the output is no longer wrapped in a
-                dictonairy, by default True
 
             Returns
             -------
             list of dicts
                 Containing the meta-data of the users
             """
-            includes = ['metadata'] if include_metadata else []
             params = {
-                'page': page, 'per_page': per_page, 'include': includes,
+                'page': page, 'per_page': per_page,
                 'username': username, 'organization_id': organization,
                 'firstname': firstname, 'lastname': lastname, 'email': email,
                 'role_id': role, 'rule_id': rule,
                 'last_seen_from': last_seen_from,
                 'last_seen_till': last_seen_till,
             }
             return self.parent.request('user', params=params)
@@ -1000,15 +968,15 @@
 
     class Role(ClientBase.SubClient):
 
         @post_filtering()
         def list(self, name: str = None, description: str = None,
                  organization: int = None, rule: int = None, user: int = None,
                  include_root: bool = None, page: int = 1, per_page: int = 20,
-                 include_metadata: bool = True) -> list[dict]:
+                 ) -> list[dict]:
             """List of roles
 
             Parameters
             ----------
             name: str, optional
                 Filter by name (with LIKE operator)
             description: str, optional
@@ -1022,27 +990,22 @@
             include_root: bool, optional
                 Include roles that are not assigned to any particular
                 organization
             page: int, optional
                 Pagination page, by default 1
             per_page: int, optional
                 Number of items on a single page, by default 20
-            include_metadata: bool, optional
-                Whenever to include the pagination metadata. If this is
-                set to False the output is no longer wrapped in a
-                dictonairy, by default True
 
             Returns
             -------
             list[dict]
                 Containing roles meta-data
             """
-            includes = ['metadata'] if include_metadata else []
             params = {
-                'page': page, 'per_page': per_page, 'include': includes,
+                'page': page, 'per_page': per_page,
                 'name': name, 'description': description,
                 'organization_id': organization, 'rule_id': rule,
                 'include_root': include_root, 'user_id': user,
             }
             return self.parent.request('role', params=params)
 
         @post_filtering(iterable=True)
@@ -1164,15 +1127,15 @@
         @post_filtering()
         def list(
             self, initiating_org: int = None, initiating_user: int = None,
             collaboration: int = None, image: str = None, parent: int = None,
             job: int = None, name: str = None, include_results: bool = False,
             description: str = None, database: str = None, run: int = None,
             status: str = None, user_created: bool = None, page: int = 1,
-            per_page: int = 20, include_metadata: bool = True
+            per_page: int = 20
         ) -> dict:
             """List tasks
 
             Parameters
             ----------
             name: str, optional
                 Filter by the name of the task. It will match with a
@@ -1205,48 +1168,35 @@
             user_created: bool, optional
                 If True, show only top-level tasks created by users. If False,
                 show only subtasks created by algorithm containers.
             page: int, optional
                 Pagination page, by default 1
             per_page: int, optional
                 Number of items on a single page, by default 20
-            include_metadata: bool, optional
-                Whenever to include the pagination metadata. If this is
-                set to False the output is no longer wrapped in a
-                dictonairy, by default True
 
             Returns
             -------
             dict
                 dictonairy containing the key 'data' which contains the
                 tasks and a key 'links' containing the pagination
                 metadata
-
-            OR
-
-            list
-                when 'include_metadata' is set to false, it removes the
-                metadata wrapper. I.e. directly returning the 'data'
-                key.
             """
             # if the param is None, it will not be passed on to the
             # request
             params = {
                 'init_org_id': initiating_org, 'init_user_id': initiating_user,
                 'collaboration_id': collaboration,
                 'image': image, 'parent_id': parent, 'job_id': job,
                 'name': name, 'page': page, 'per_page': per_page,
                 'description': description, 'database': database,
                 'run_id': run, 'status': status,
             }
             includes = []
             if include_results:
                 includes.append('results')
-            if include_metadata:
-                includes.append('metadata')
             params['include'] = includes
             if user_created is not None:
                 params['is_user_created'] = 1 if user_created else 0
 
             return self.parent.request('task', params=params)
 
         @post_filtering(iterable=False)
@@ -1287,15 +1237,15 @@
                 databases = ['default']
             elif isinstance(databases, str):
                 # it is not unlikely that users specify a single database as a
                 # str, in that case we convert it to a list
                 databases = [databases]
 
             # Data will be serialized in JSON.
-            serialized_input = serialization.serialize(input_)
+            serialized_input = serialize(input_)
 
             # Encrypt the input per organization using that organization's
             # public key.
             organization_json_list = []
             for org_id in organizations:
                 pub_key = self.parent.request(f"organization/{org_id}")\
                     .get("public_key")
@@ -1385,15 +1335,15 @@
         @post_filtering()
         def list(self, task: int = None, organization: int = None,
                  state: str = None, node: int = None,
                  include_task: bool = False, started: tuple[str, str] = None,
                  assigned: tuple[str, str] = None,
                  finished: tuple[str, str] = None, port: int = None,
                  page: int = None, per_page: int = None,
-                 include_metadata: bool = True) -> dict | list[dict]:
+                 ) -> dict | list[dict]:
             """List runs
 
             Parameters
             ----------
             task: int, optional
                 Filter by task id
             organization: int, optional
@@ -1412,31 +1362,22 @@
                 Filter on a range of finished times (format: yyyy-mm-dd)
             port: int, optional
                 Port on which run was computed
             page: int, optional
                 Pagination page number, defaults to 1
             per_page: int, optional
                 Number of items per page, defaults to 20
-            include_metedata: bool, optional
-                Whenevet to include pagination metadata, defaults to
-                True
 
             Returns
             -------
             dict | list[dict]
-                If include_metadata is True, a dictionary is returned
-                containing the key 'data' which contains a list of
-                runs, and a key 'links' which contains the pagination
-                metadata.
-                When include_metadata is False, the metadata wrapper
-                is stripped and only a list of runs is returned
+                A dictionary containing the key 'data' which contains a list of
+                runs, and a key 'links' which contains the pagination metadata.
             """
             includes = []
-            if include_metadata:
-                includes.append('metadata')
             if include_task:
                 includes.append('task')
 
             s_from, s_till = started if started else (None, None)
             a_from, a_till = assigned if assigned else (None, None)
             f_from, f_till = finished if finished else (None, None)
 
@@ -1586,15 +1527,15 @@
                 Containing the information about this rule
             """
             return self.parent.request(f'rule/{id_}')
 
         @post_filtering()
         def list(self, name: str = None, operation: str = None,
                  scope: str = None, role: int = None, page: int = 1,
-                 per_page: int = 20, include_metadata: bool = True) -> list:
+                 per_page: int = 20) -> list:
             """List of all available rules
 
             Parameters
             ----------
             name: str, optional
                 Filter by rule name
             operation: str, optional
@@ -1603,24 +1544,18 @@
                 Filter by scope
             role: int, optional
                 Only show rules that belong to this role id
             page: int, optional
                 Pagination page, by default 1
             per_page: int, optional
                 Number of items on a single page, by default 20
-            include_metadata: bool, optional
-                Whenever to include the pagination metadata. If this is
-                set to False the output is no longer wrapped in a
-                dictonairy, by default True
 
             Returns
             -------
             list of dicts
                 Containing all the rules from the vantage6 server
             """
-            includes = ['metadata'] if include_metadata else []
             params = {
-                'page': page, 'per_page': per_page, 'include': includes,
-                'name': name, 'operation': operation, 'scope': scope,
-                'role_id': role
+                'page': page, 'per_page': per_page, 'name': name,
+                'operation': operation, 'scope': scope, 'role_id': role
             }
             return self.parent.request('rule', params=params)
```

### Comparing `vantage6-client-4.0.0a4/vantage6/client/_version.py` & `vantage6-client-4.0.0a5/vantage6/client/_version.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-4.0.0a4/vantage6/client/filter.py` & `vantage6-client-4.0.0a5/vantage6/client/filter.py`

 * *Files 10% similar despite different names*

```diff
@@ -130,18 +130,18 @@
             A list of keys to filter the dictionary on, by default None
 
         Returns
         -------
         list[dict]
             The filtered list of dicts.
         """
-        dicts = func(*args, **kwargs)
+        dict_ = func(*args, **kwargs)
         if field:
-            return filter_dicts_keys(dicts, [field])
-        return filter_dicts_keys(dicts, fields)
+            return filter_dicts_keys(dict_, [field])
+        return filter_dicts_keys(dict_, fields)
     return wrapper_filter
 
 
 def post_filtering(iterable: bool = True) -> callable:
     """Decorator to add filtering of dictornaries from the result.
 
     Depending on whether this is a list of or a single dictionairy, the
@@ -227,34 +227,37 @@
         The filtered list of dicts.
     """
     if filters:
         return filter_dicts_on_values(dicts, filters)
     return dicts
 
 
-def filter_dicts_keys(dicts: list[dict], keys: list[str]) -> list[dict]:
+def filter_dicts_keys(dict_: dict, keys: list[str]) -> list[dict]:
     """
     Filter a list of dicts on the specified keys. If no keys are given, the
     original list of dicts is returned.
 
     Parameters
     ----------
     dicts : list[dict]
-        The list of dicts to filter.
+        The dict to filter. This is a dict with a 'data' key that contains the
+        list of data dictionaries that will be filtered.
     keys : list[str]
         A list of keys to keep in the dictionaries
 
     Returns
     -------
     list[dict]
         The filtered list of dicts.
     """
+    # note: we look only in the 'data' key of the dict, which contains the list
+    # of data. The only other key is 'links' which contains pagination links
     if keys:
-        return [filter_dict_keys(adict, keys) for adict in dicts]
-    return dicts
+        return [filter_dict_keys(adict, keys) for adict in dict_['data']]
+    return dict_
 
 
 def filter_dict_keys(dict_: dict, keys: list[str]) -> dict:
     """
     Filter a dict on the specified keys. If no keys are given, the original
     dict is returned.
```

### Comparing `vantage6-client-4.0.0a4/vantage6_client.egg-info/PKG-INFO` & `vantage6-client-4.0.0a5/vantage6_client.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: vantage6-client
-Version: 4.0.0a4
+Version: 4.0.0a5
 Summary: Vantage6 client
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
-Metadata-Version: 2.1 Name: vantage6-client Version: 4.0.0a4 Summary: Vantage6
-client Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.6
+Metadata-Version: 2.1 Name: vantage6-client Version: 4.0.0a5 Summary: Vantage6
+client Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.10
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

