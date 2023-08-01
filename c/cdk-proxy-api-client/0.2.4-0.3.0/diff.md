# Comparing `tmp/cdk_proxy_api_client-0.2.4.tar.gz` & `tmp/cdk_proxy_api_client-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk_proxy_api_client-0.2.4.tar", max compression
+gzip compressed data, was "cdk_proxy_api_client-0.3.0.tar", max compression
```

## Comparing `cdk_proxy_api_client-0.2.4.tar` & `cdk_proxy_api_client-0.3.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
--rw-r--r--   0        0        0    10280 2023-03-08 09:09:19.917488 cdk_proxy_api_client-0.2.4/LICENSE
--rw-r--r--   0        0        0     4404 2023-03-26 16:28:29.410881 cdk_proxy_api_client-0.2.4/README.md
--rw-r--r--   0        0        0      181 2023-04-25 09:35:50.180415 cdk_proxy_api_client-0.2.4/cdk_proxy_api_client/__init__.py
--rw-r--r--   0        0        0     1163 2023-03-26 16:47:51.442956 cdk_proxy_api_client-0.2.4/cdk_proxy_api_client/admin_auth/__init__.py
--rw-r--r--   0        0        0      133 2023-03-10 11:53:55.066691 cdk_proxy_api_client-0.2.4/cdk_proxy_api_client/admin_auth/exceptions.py
--rw-r--r--   0        0        0     6831 2023-04-25 09:19:47.673991 cdk_proxy_api_client-0.2.4/cdk_proxy_api_client/cli/__init__.py
--rw-r--r--   0        0        0     6619 2023-04-25 09:19:42.357928 cdk_proxy_api_client-0.2.4/cdk_proxy_api_client/cli/main_parser.py
--rw-r--r--   0        0        0     5728 2023-03-14 12:38:20.148498 cdk_proxy_api_client-0.2.4/cdk_proxy_api_client/client_wrapper.py
--rw-r--r--   0        0        0      601 2023-03-08 21:22:30.578973 cdk_proxy_api_client-0.2.4/cdk_proxy_api_client/common/__init__.py
--rw-r--r--   0        0        0     1174 2023-03-26 16:44:44.959697 cdk_proxy_api_client-0.2.4/cdk_proxy_api_client/common/logging.py
--rw-r--r--   0        0        0     2269 2023-04-24 16:24:30.445038 cdk_proxy_api_client-0.2.4/cdk_proxy_api_client/concentration/__init__.py
--rw-r--r--   0        0        0     3012 2023-03-10 11:34:33.523871 cdk_proxy_api_client-0.2.4/cdk_proxy_api_client/errors.py
--rw-r--r--   0        0        0       93 2023-03-08 21:22:30.582973 cdk_proxy_api_client-0.2.4/cdk_proxy_api_client/models/__init__.py
--rw-r--r--   0        0        0     1467 2023-03-08 10:34:32.551495 cdk_proxy_api_client-0.2.4/cdk_proxy_api_client/models/v1b1.py
--rw-r--r--   0        0        0     1400 2023-03-26 16:47:51.434956 cdk_proxy_api_client-0.2.4/cdk_proxy_api_client/proxy_api.py
--rw-r--r--   0        0        0        0 2023-03-14 12:46:32.223933 cdk_proxy_api_client-0.2.4/cdk_proxy_api_client/specs/__init__.py
--rw-r--r--   0        0        0     3825 2023-04-25 09:23:41.838770 cdk_proxy_api_client-0.2.4/cdk_proxy_api_client/specs/tenant_mappings-input.json
--rw-r--r--   0        0        0     2973 2023-04-24 16:24:30.445038 cdk_proxy_api_client-0.2.4/cdk_proxy_api_client/tenant_mappings/__init__.py
--rw-r--r--   0        0        0      414 2023-03-10 12:11:17.799028 cdk_proxy_api_client-0.2.4/cdk_proxy_api_client/tenant_mappings/exceptions.py
--rw-r--r--   0        0        0      800 2023-03-26 16:00:22.879474 cdk_proxy_api_client-0.2.4/cdk_proxy_api_client/tools/__init__.py
--rw-r--r--   0        0        0    10915 2023-04-19 10:54:30.871690 cdk_proxy_api_client-0.2.4/cdk_proxy_api_client/tools/import_tenants_mappings.py
--rw-r--r--   0        0        0     2430 2023-04-25 09:35:50.180415 cdk_proxy_api_client-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     5941 1970-01-01 00:00:00.000000 cdk_proxy_api_client-0.2.4/setup.py
--rw-r--r--   0        0        0     6035 1970-01-01 00:00:00.000000 cdk_proxy_api_client-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0    10280 2023-03-08 09:09:19.917488 cdk_proxy_api_client-0.3.0/LICENSE
+-rw-r--r--   0        0        0     4404 2023-03-26 16:28:29.410881 cdk_proxy_api_client-0.3.0/README.md
+-rw-r--r--   0        0        0      181 2023-08-01 15:08:54.886977 cdk_proxy_api_client-0.3.0/cdk_proxy_api_client/__init__.py
+-rw-r--r--   0        0        0     1163 2023-03-26 16:47:51.442956 cdk_proxy_api_client-0.3.0/cdk_proxy_api_client/admin_auth/__init__.py
+-rw-r--r--   0        0        0      133 2023-03-10 11:53:55.066691 cdk_proxy_api_client-0.3.0/cdk_proxy_api_client/admin_auth/exceptions.py
+-rw-r--r--   0        0        0     7399 2023-08-01 14:05:10.455088 cdk_proxy_api_client-0.3.0/cdk_proxy_api_client/cli/__init__.py
+-rw-r--r--   0        0        0     7005 2023-08-01 14:05:10.455088 cdk_proxy_api_client-0.3.0/cdk_proxy_api_client/cli/main_parser.py
+-rw-r--r--   0        0        0     5728 2023-03-14 12:38:20.148498 cdk_proxy_api_client-0.3.0/cdk_proxy_api_client/client_wrapper.py
+-rw-r--r--   0        0        0      601 2023-03-08 21:22:30.578973 cdk_proxy_api_client-0.3.0/cdk_proxy_api_client/common/__init__.py
+-rw-r--r--   0        0        0     1174 2023-03-26 16:44:44.959697 cdk_proxy_api_client-0.3.0/cdk_proxy_api_client/common/logging.py
+-rw-r--r--   0        0        0     2269 2023-04-24 16:24:30.445038 cdk_proxy_api_client-0.3.0/cdk_proxy_api_client/concentration/__init__.py
+-rw-r--r--   0        0        0     3012 2023-03-10 11:34:33.523871 cdk_proxy_api_client-0.3.0/cdk_proxy_api_client/errors.py
+-rw-r--r--   0        0        0       93 2023-03-08 21:22:30.582973 cdk_proxy_api_client-0.3.0/cdk_proxy_api_client/models/__init__.py
+-rw-r--r--   0        0        0     1467 2023-03-08 10:34:32.551495 cdk_proxy_api_client-0.3.0/cdk_proxy_api_client/models/v1b1.py
+-rw-r--r--   0        0        0     1400 2023-03-26 16:47:51.434956 cdk_proxy_api_client-0.3.0/cdk_proxy_api_client/proxy_api.py
+-rw-r--r--   0        0        0        0 2023-03-14 12:46:32.223933 cdk_proxy_api_client-0.3.0/cdk_proxy_api_client/specs/__init__.py
+-rw-r--r--   0        0        0     2268 2023-08-01 14:05:10.456088 cdk_proxy_api_client-0.3.0/cdk_proxy_api_client/specs/profiles_config.spec.json
+-rw-r--r--   0        0        0     3825 2023-08-01 13:58:16.127216 cdk_proxy_api_client-0.3.0/cdk_proxy_api_client/specs/tenant_mappings-input.json
+-rw-r--r--   0        0        0     2973 2023-04-24 16:24:30.445038 cdk_proxy_api_client-0.3.0/cdk_proxy_api_client/tenant_mappings/__init__.py
+-rw-r--r--   0        0        0      414 2023-03-10 12:11:17.799028 cdk_proxy_api_client-0.3.0/cdk_proxy_api_client/tenant_mappings/exceptions.py
+-rw-r--r--   0        0        0      800 2023-03-26 16:00:22.879474 cdk_proxy_api_client-0.3.0/cdk_proxy_api_client/tools/__init__.py
+-rw-r--r--   0        0        0     4333 2023-08-01 14:05:10.456088 cdk_proxy_api_client-0.3.0/cdk_proxy_api_client/tools/import_from_config.py
+-rw-r--r--   0        0        0    10915 2023-04-19 10:54:30.871690 cdk_proxy_api_client-0.3.0/cdk_proxy_api_client/tools/import_tenants_mappings.py
+-rw-r--r--   0        0        0     2446 2023-08-01 15:08:54.885977 cdk_proxy_api_client-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5871 1970-01-01 00:00:00.000000 cdk_proxy_api_client-0.3.0/PKG-INFO
```

### Comparing `cdk_proxy_api_client-0.2.4/LICENSE` & `cdk_proxy_api_client-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk_proxy_api_client-0.2.4/README.md` & `cdk_proxy_api_client-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `cdk_proxy_api_client-0.2.4/cdk_proxy_api_client/admin_auth/__init__.py` & `cdk_proxy_api_client-0.3.0/cdk_proxy_api_client/admin_auth/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk_proxy_api_client-0.2.4/cdk_proxy_api_client/cli/__init__.py` & `cdk_proxy_api_client-0.3.0/cdk_proxy_api_client/cli/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from cdk_proxy_api_client.admin_auth import AdminAuth
 from cdk_proxy_api_client.cli.main_parser import set_parser
 from cdk_proxy_api_client.common.logging import LOG
 from cdk_proxy_api_client.concentration import TenantContentrationMapping, TopicsTenants
 from cdk_proxy_api_client.proxy_api import ApiClient, Multitenancy, ProxyClient
 from cdk_proxy_api_client.tenant_mappings import TenantTopicMappings
 from cdk_proxy_api_client.tools import load_config_file
+from cdk_proxy_api_client.tools.import_from_config import import_clients
 from cdk_proxy_api_client.tools.import_tenants_mappings import import_tenants_mappings
 
 
 def format_return(function):
     """
     Decorator to evaluate the requests payload returned
     """
@@ -171,19 +172,31 @@
             LOG.setLevel(logging.getLevelName(_args.loglevel.upper()))
             LOG.handlers[0].setLevel(logging.getLevelName(_args.loglevel.upper()))
         else:
             print(
                 f"Log level value {_args.loglevel} is invalid. Must me one of {valid_levels}"
             )
     _vars = vars(_args)
-    _client = ApiClient(
-        username=_vars.pop("username"),
-        password=_vars.pop("password"),
-        url=_vars.pop("url"),
-    )
+    if _args.url:
+        if not _args.username or not _args.password:
+            raise Exception(
+                "If you specify URL, you must specify username and password too"
+            )
+        _client = ApiClient(
+            username=_vars.pop("username"),
+            password=_vars.pop("password"),
+            url=_vars.pop("url"),
+        )
+    elif _args.profile_name:
+        _clients = import_clients(_args.config_file)
+        _client = _clients[_args.profile_name]
+    else:
+        raise Exception(
+            "You must either set --profile-name (possibly -c) or define --url, --username and --password"
+        )
     _category = _vars.pop("category")
     _action = _vars.pop("action")
     _proxy = ProxyClient(_client)
 
     _categories_mappings: dict = {
         "tenants": tenants_actions,
         "tenant-topic-mappings": tenant_mappings_actions,
```

### Comparing `cdk_proxy_api_client-0.2.4/cdk_proxy_api_client/cli/main_parser.py` & `cdk_proxy_api_client-0.3.0/cdk_proxy_api_client/cli/main_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #   SPDX-License-Identifier: Apache-2.0
 #   Copyright 2023 John Mille <john@ews-network.net>
 
 from __future__ import annotations
 
 from argparse import ArgumentParser
+from os import environ
 
 TENANT_PARSER = ArgumentParser(add_help=False)
 TENANT_PARSER.add_argument(
     "--tenant-name", required=True, help="Name of the tenant to make operations for"
 )
 
 
@@ -158,17 +159,31 @@
         dest="output_format",
         help="output format",
         default="yaml",
     )
     main_parser.add_argument(
         "--log-level", dest="loglevel", type=str, help="Set loglevel", required=False
     )
-    main_parser.add_argument("--username", required=True)
-    main_parser.add_argument("--password", required=True)
-    main_parser.add_argument("--url", required=True)
+    main_parser.add_argument("--url", required=False)
+    main_parser.add_argument("--username", required=False)
+    main_parser.add_argument("--password", required=False)
+    main_parser.add_argument(
+        "-c",
+        "--config-file",
+        type=str,
+        help="Path to the profiles files",
+        default="{}/.cdk_gw.yaml".format(environ.get("HOME", ".")),
+    )
+    main_parser.add_argument(
+        "-p",
+        "--profile-name",
+        type=str,
+        help="Name of the profile to use to make API Calls",
+    )
+
     cmd_parser = main_parser.add_subparsers(dest="category", help="Resources to manage")
     auth_admin_parser = cmd_parser.add_parser(
         name="auth",
         help="Manages proxy tenant token",
     )
     set_admin_auth_parser(auth_admin_parser)
```

### Comparing `cdk_proxy_api_client-0.2.4/cdk_proxy_api_client/client_wrapper.py` & `cdk_proxy_api_client-0.3.0/cdk_proxy_api_client/client_wrapper.py`

 * *Files identical despite different names*

### Comparing `cdk_proxy_api_client-0.2.4/cdk_proxy_api_client/common/__init__.py` & `cdk_proxy_api_client-0.3.0/cdk_proxy_api_client/common/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk_proxy_api_client-0.2.4/cdk_proxy_api_client/common/logging.py` & `cdk_proxy_api_client-0.3.0/cdk_proxy_api_client/common/logging.py`

 * *Files identical despite different names*

### Comparing `cdk_proxy_api_client-0.2.4/cdk_proxy_api_client/concentration/__init__.py` & `cdk_proxy_api_client-0.3.0/cdk_proxy_api_client/concentration/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk_proxy_api_client-0.2.4/cdk_proxy_api_client/errors.py` & `cdk_proxy_api_client-0.3.0/cdk_proxy_api_client/errors.py`

 * *Files identical despite different names*

### Comparing `cdk_proxy_api_client-0.2.4/cdk_proxy_api_client/models/v1b1.py` & `cdk_proxy_api_client-0.3.0/cdk_proxy_api_client/models/v1b1.py`

 * *Files identical despite different names*

### Comparing `cdk_proxy_api_client-0.2.4/cdk_proxy_api_client/proxy_api.py` & `cdk_proxy_api_client-0.3.0/cdk_proxy_api_client/proxy_api.py`

 * *Files identical despite different names*

### Comparing `cdk_proxy_api_client-0.2.4/cdk_proxy_api_client/specs/tenant_mappings-input.json` & `cdk_proxy_api_client-0.3.0/cdk_proxy_api_client/specs/tenant_mappings-input.json`

 * *Files identical despite different names*

### Comparing `cdk_proxy_api_client-0.2.4/cdk_proxy_api_client/tenant_mappings/__init__.py` & `cdk_proxy_api_client-0.3.0/cdk_proxy_api_client/tenant_mappings/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk_proxy_api_client-0.2.4/cdk_proxy_api_client/tools/__init__.py` & `cdk_proxy_api_client-0.3.0/cdk_proxy_api_client/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk_proxy_api_client-0.2.4/cdk_proxy_api_client/tools/import_tenants_mappings.py` & `cdk_proxy_api_client-0.3.0/cdk_proxy_api_client/tools/import_tenants_mappings.py`

 * *Files identical despite different names*

### Comparing `cdk_proxy_api_client-0.2.4/pyproject.toml` & `cdk_proxy_api_client-0.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "cdk-proxy-api-client"
 description = "Conduktor Proxy API Client"
-version = "0.2.4"
+version = "0.3.0"
 authors = ["John \"Preston\" Mille <john@ews-network.net>"]
 readme = "README.md"
 license = "LICENSE"
 packages = [{include = "cdk_proxy_api_client"}]
 keywords = ["compose-x", "conduktor", "kafka", "proxy"]
 classifiers = [
   "Development Status :: 2 - Pre-Alpha",
@@ -32,14 +32,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "^2.28.2"
 jsonschema = {version = "^4.17.3", optional = true }
 compose-x-common = {version = "^1.2", optional = true }
 importlib-resources = {version = "^5.12.0", optional = true }
+pyyaml = "^6.0"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.1.1"
 black = "^23.1.0"
 isort = "^5.12.0"
 openapi-python-client = "^0.13.1"
 datamodel-code-generator = "^0.17.1"
@@ -55,15 +56,15 @@
 cdk-cli = "cdk_proxy_api_client.cli:main"
 
 
 [tool.tbump]
 github_url = "https://codeberg.org/JohnPreston/cdk-proxy-api-client"
 
 [tool.tbump.version]
-current = "0.2.4"
+current = "0.3.0"
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
   (?:(?P<rc>[\S]+))?
```

### Comparing `cdk_proxy_api_client-0.2.4/setup.py` & `cdk_proxy_api_client-0.3.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,51 +1,208 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: cdk-proxy-api-client
+Version: 0.3.0
+Summary: Conduktor Proxy API Client
+License: LICENSE
+Keywords: compose-x,conduktor,kafka,proxy
+Author: John "Preston" Mille
+Author-email: john@ews-network.net
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: System Administrators
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: License :: Other/Proprietary License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: cli
+Provides-Extra: tools
+Requires-Dist: compose-x-common (>=1.2,<2.0) ; extra == "tools" or extra == "cli"
+Requires-Dist: importlib-resources (>=5.12.0,<6.0.0) ; extra == "tools" or extra == "cli"
+Requires-Dist: jsonschema (>=4.17.3,<5.0.0) ; extra == "tools" or extra == "cli"
+Requires-Dist: pyyaml (>=6.0,<7.0)
+Requires-Dist: requests (>=2.28.2,<3.0.0)
+Project-URL: Bug Tracker, https://github.com/JohnPreston/cdk-proxy-api-client/issues
+Project-URL: Source (GitHub), https://github.com/JohnPreston/cdk-proxy-api-client
+Project-URL: Source (CodeBerg), https://codeberg.org/JohnPreston/cdk-proxy-api-client
+Description-Content-Type: text/markdown
+
+# cdk-proxy-api-client
+
+API Client library to interact with Conduktor Proxy
+
+Current version: v1beta1
+
+
+## Getting started
+
+First, create a Proxy Client
+
+```python
+from cdk_proxy_api_client.proxy_api import ApiClient, ProxyClient
+
+api = ApiClient("localhost", port=8888, username="superUser", password="superUser")
+proxy_client = ProxyClient(api)
+```
+
+### Features
+
+Note: we assume you are re-using the ``proxy_client`` as shown above.
+
+* Create new Token for a tenant
+
+```python
+from cdk_proxy_api_client.admin_auth import AdminAuth
+
+admin = AdminAuth(proxy_client)
+admin.create_tenant_credentials("a_tenant_name")
+```
+
+* List all topic mappings for a tenant
+
+```python
+from cdk_proxy_api_client.proxy_api import Multitenancy
+
+tenants_mgmt = Multitenancy(proxy_client)
+tenants = tenants_mgmt.list_tenants(as_list=True)
+```
+
+* Create a new mapping for a tenant
+* Delete a tenant - topic mapping
+* Delete all topic mappings for a tenant
+
+```python
+from cdk_proxy_api_client.tenant_mappings import TenantTopicMappings
+
+tenant_mappings_mgmt = TenantTopicMappings(proxy_client)
+tenant_mappings_mgmt.create_tenant_topic_mapping(
+    "tenant_name", "logical_name", "real_name"
+)
+tenant_mappings_mgmt.delete_tenant_topic_mapping("tenant_name", "logical_name")
+```
+
+## Testing
+The testing is for now very manual. See ``e2e_testing.py``
+
+Pytest will be added later on
+
+
+## Tools & CLI
+
+To simplify the usage of the client, you can use some CLI commands
+
+```shell
+usage: CDK Proxy CLI [-h] [--format OUTPUT_FORMAT] --username USERNAME --password PASSWORD --url URL {auth,tenant-topic-mappings,tenants} ...
+
+positional arguments:
+  {auth,tenant-topic-mappings,tenants}
+                        Resources to manage
+    auth                Manages proxy tenant token
+    tenant-topic-mappings
+                        Manages tenant mappings
+    tenants             Manage tenants
+
+optional arguments:
+  -h, --help            show this help message and exit
+  --format OUTPUT_FORMAT, --output-format OUTPUT_FORMAT
+                        output format
+  --username USERNAME
+  --password PASSWORD
+  --url URL
+
+```
+
+### cdk-cli tenant-topic-mappings
+
+```shell
+usage: CDK Proxy CLI tenant-topic-mappings [-h] {list,create,import-from-tenants-config,import-from-tenant,delete-all-mappings,delete-topic-mapping} ...
+
+positional arguments:
+  {list,create,import-from-tenants-config,import-from-tenant,delete-all-mappings,delete-topic-mapping}
+                        Mappings management
+    list                List tenant mappings
+    create              Create a new tenant mapping
+    import-from-tenants-config
+                        Create topic mappings from existing tenants
+    import-from-tenant  Import all topics from a existing tenant
+    delete-all-mappings
+                        Delete all topics mappings for a given tenant
+    delete-topic-mapping
+                        Delete a topic mapping for a given tenant
+
+optional arguments:
+  -h, --help            show this help message and exit
+```
+
+#### import-from-tenants-config
+
+This command uses a configuration file that will be used to propagate mappings from one/multiple existing tenants to another.
+
+example file:
+
+```yaml
+---
+# example.config.yaml
+
+tenant_name: application-01
+ignore_duplicates_conflict: true
+mappings:
+  - logicalTopicName: data.stock
+    physicalTopicName: data.stock
+    readOnly: true
+```
+
+```shell
+cdk-cli --username ${PROXY_USERNAME} \
+        --password ${PROXY_PASSWORD} \
+        --url ${PROXY_URL} \
+        tenant-topic-mappings import-from-tenants-config -f example.config.yaml
+```
+
+### cdk-cli auth
+
+```shell
+cdk-cli auth --help
+usage: CDK Proxy CLI auth [-h] {create} ...
+
+positional arguments:
+  {create}    Token actions to execute
+    create    Create a new tenant proxy JWT Token
+
+optional arguments:
+  -h, --help  show this help message and exit
+```
+
+#### cdk-cli-create-tenant-token
+
+Create a new user tenant token
+
+```shell
+cdk-cli \
+        --username ${PROXY_USERNAME} \
+        --password ${PROXY_PASSWORD} \
+        --url ${PROXY_URL} \
+        auth create \
+        --lifetime-in-seconds 3600  \
+        --tenant-name js-fin-panther-stg
+```
+
+### cdk-cli tenants
+
+Manage tenants
+
+```shell
+cdk-cli tenants --help
+usage: CDK Proxy CLI tenants [-h] {list} ...
+
+positional arguments:
+  {list}      Manage tenants
+    list      List tenants
+
+optional arguments:
+  -h, --help  show this help message and exit
+```
 
-packages = \
-['cdk_proxy_api_client',
- 'cdk_proxy_api_client.admin_auth',
- 'cdk_proxy_api_client.cli',
- 'cdk_proxy_api_client.common',
- 'cdk_proxy_api_client.concentration',
- 'cdk_proxy_api_client.models',
- 'cdk_proxy_api_client.specs',
- 'cdk_proxy_api_client.tenant_mappings',
- 'cdk_proxy_api_client.tools']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['requests>=2.28.2,<3.0.0']
-
-extras_require = \
-{'cli': ['jsonschema>=4.17.3,<5.0.0',
-         'compose-x-common>=1.2,<2.0',
-         'importlib-resources>=5.12.0,<6.0.0'],
- 'tools': ['jsonschema>=4.17.3,<5.0.0',
-           'compose-x-common>=1.2,<2.0',
-           'importlib-resources>=5.12.0,<6.0.0']}
-
-entry_points = \
-{'console_scripts': ['cdk-cli = cdk_proxy_api_client.cli:main']}
-
-setup_kwargs = {
-    'name': 'cdk-proxy-api-client',
-    'version': '0.2.4',
-    'description': 'Conduktor Proxy API Client',
-    'long_description': '# cdk-proxy-api-client\n\nAPI Client library to interact with Conduktor Proxy\n\nCurrent version: v1beta1\n\n\n## Getting started\n\nFirst, create a Proxy Client\n\n```python\nfrom cdk_proxy_api_client.proxy_api import ApiClient, ProxyClient\n\napi = ApiClient("localhost", port=8888, username="superUser", password="superUser")\nproxy_client = ProxyClient(api)\n```\n\n### Features\n\nNote: we assume you are re-using the ``proxy_client`` as shown above.\n\n* Create new Token for a tenant\n\n```python\nfrom cdk_proxy_api_client.admin_auth import AdminAuth\n\nadmin = AdminAuth(proxy_client)\nadmin.create_tenant_credentials("a_tenant_name")\n```\n\n* List all topic mappings for a tenant\n\n```python\nfrom cdk_proxy_api_client.proxy_api import Multitenancy\n\ntenants_mgmt = Multitenancy(proxy_client)\ntenants = tenants_mgmt.list_tenants(as_list=True)\n```\n\n* Create a new mapping for a tenant\n* Delete a tenant - topic mapping\n* Delete all topic mappings for a tenant\n\n```python\nfrom cdk_proxy_api_client.tenant_mappings import TenantTopicMappings\n\ntenant_mappings_mgmt = TenantTopicMappings(proxy_client)\ntenant_mappings_mgmt.create_tenant_topic_mapping(\n    "tenant_name", "logical_name", "real_name"\n)\ntenant_mappings_mgmt.delete_tenant_topic_mapping("tenant_name", "logical_name")\n```\n\n## Testing\nThe testing is for now very manual. See ``e2e_testing.py``\n\nPytest will be added later on\n\n\n## Tools & CLI\n\nTo simplify the usage of the client, you can use some CLI commands\n\n```shell\nusage: CDK Proxy CLI [-h] [--format OUTPUT_FORMAT] --username USERNAME --password PASSWORD --url URL {auth,tenant-topic-mappings,tenants} ...\n\npositional arguments:\n  {auth,tenant-topic-mappings,tenants}\n                        Resources to manage\n    auth                Manages proxy tenant token\n    tenant-topic-mappings\n                        Manages tenant mappings\n    tenants             Manage tenants\n\noptional arguments:\n  -h, --help            show this help message and exit\n  --format OUTPUT_FORMAT, --output-format OUTPUT_FORMAT\n                        output format\n  --username USERNAME\n  --password PASSWORD\n  --url URL\n\n```\n\n### cdk-cli tenant-topic-mappings\n\n```shell\nusage: CDK Proxy CLI tenant-topic-mappings [-h] {list,create,import-from-tenants-config,import-from-tenant,delete-all-mappings,delete-topic-mapping} ...\n\npositional arguments:\n  {list,create,import-from-tenants-config,import-from-tenant,delete-all-mappings,delete-topic-mapping}\n                        Mappings management\n    list                List tenant mappings\n    create              Create a new tenant mapping\n    import-from-tenants-config\n                        Create topic mappings from existing tenants\n    import-from-tenant  Import all topics from a existing tenant\n    delete-all-mappings\n                        Delete all topics mappings for a given tenant\n    delete-topic-mapping\n                        Delete a topic mapping for a given tenant\n\noptional arguments:\n  -h, --help            show this help message and exit\n```\n\n#### import-from-tenants-config\n\nThis command uses a configuration file that will be used to propagate mappings from one/multiple existing tenants to another.\n\nexample file:\n\n```yaml\n---\n# example.config.yaml\n\ntenant_name: application-01\nignore_duplicates_conflict: true\nmappings:\n  - logicalTopicName: data.stock\n    physicalTopicName: data.stock\n    readOnly: true\n```\n\n```shell\ncdk-cli --username ${PROXY_USERNAME} \\\n        --password ${PROXY_PASSWORD} \\\n        --url ${PROXY_URL} \\\n        tenant-topic-mappings import-from-tenants-config -f example.config.yaml\n```\n\n### cdk-cli auth\n\n```shell\ncdk-cli auth --help\nusage: CDK Proxy CLI auth [-h] {create} ...\n\npositional arguments:\n  {create}    Token actions to execute\n    create    Create a new tenant proxy JWT Token\n\noptional arguments:\n  -h, --help  show this help message and exit\n```\n\n#### cdk-cli-create-tenant-token\n\nCreate a new user tenant token\n\n```shell\ncdk-cli \\\n        --username ${PROXY_USERNAME} \\\n        --password ${PROXY_PASSWORD} \\\n        --url ${PROXY_URL} \\\n        auth create \\\n        --lifetime-in-seconds 3600  \\\n        --tenant-name js-fin-panther-stg\n```\n\n### cdk-cli tenants\n\nManage tenants\n\n```shell\ncdk-cli tenants --help\nusage: CDK Proxy CLI tenants [-h] {list} ...\n\npositional arguments:\n  {list}      Manage tenants\n    list      List tenants\n\noptional arguments:\n  -h, --help  show this help message and exit\n```\n',
-    'author': 'John "Preston" Mille',
-    'author_email': 'john@ews-network.net',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

