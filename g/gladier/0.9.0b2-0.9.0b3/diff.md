# Comparing `tmp/gladier-0.9.0b2.tar.gz` & `tmp/gladier-0.9.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gladier-0.9.0b2.tar", last modified: Thu Jul 20 17:38:20 2023, max compression
+gzip compressed data, was "gladier-0.9.0b3.tar", last modified: Tue Aug  1 21:55:44 2023, max compression
```

## Comparing `gladier-0.9.0b2.tar` & `gladier-0.9.0b3.tar`

### file list

```diff
@@ -1,43 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:38:20.448307 gladier-0.9.0b2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-20 17:38:09.000000 gladier-0.9.0b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-20 17:38:09.000000 gladier-0.9.0b2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-07-20 17:38:20.448307 gladier-0.9.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-07-20 17:38:09.000000 gladier-0.9.0b2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:38:20.444307 gladier-0.9.0b2/gladier/
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-20 17:38:09.000000 gladier-0.9.0b2/gladier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-07-20 17:38:09.000000 gladier-0.9.0b2/gladier/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    22625 2023-07-20 17:38:09.000000 gladier-0.9.0b2/gladier/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-07-20 17:38:09.000000 gladier-0.9.0b2/gladier/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-07-20 17:38:09.000000 gladier-0.9.0b2/gladier/exc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:38:20.448307 gladier-0.9.0b2/gladier/managers/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-20 17:38:09.000000 gladier-0.9.0b2/gladier/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-20 17:38:09.000000 gladier-0.9.0b2/gladier/managers/compute_login_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-07-20 17:38:09.000000 gladier-0.9.0b2/gladier/managers/compute_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    18884 2023-07-20 17:38:09.000000 gladier-0.9.0b2/gladier/managers/flows_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     8534 2023-07-20 17:38:09.000000 gladier-0.9.0b2/gladier/managers/login_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-07-20 17:38:09.000000 gladier-0.9.0b2/gladier/managers/service_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:38:20.448307 gladier-0.9.0b2/gladier/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 17:38:09.000000 gladier-0.9.0b2/gladier/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-20 17:38:09.000000 gladier-0.9.0b2/gladier/storage/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7037 2023-07-20 17:38:09.000000 gladier-0.9.0b2/gladier/storage/migrations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-20 17:38:09.000000 gladier-0.9.0b2/gladier/storage/tokens.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:38:20.448307 gladier-0.9.0b2/gladier/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 17:38:09.000000 gladier-0.9.0b2/gladier/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-07-20 17:38:09.000000 gladier-0.9.0b2/gladier/utils/automate.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-20 17:38:09.000000 gladier-0.9.0b2/gladier/utils/dynamic_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-07-20 17:38:09.000000 gladier-0.9.0b2/gladier/utils/flow_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-07-20 17:38:09.000000 gladier-0.9.0b2/gladier/utils/flow_modifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-20 17:38:09.000000 gladier-0.9.0b2/gladier/utils/flow_traversal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-20 17:38:09.000000 gladier-0.9.0b2/gladier/utils/name_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-20 17:38:09.000000 gladier-0.9.0b2/gladier/utils/tool_alias.py
--rw-r--r--   0 runner    (1001) docker     (123)     5072 2023-07-20 17:38:09.000000 gladier-0.9.0b2/gladier/utils/tool_chain.py
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-20 17:38:09.000000 gladier-0.9.0b2/gladier/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:38:20.448307 gladier-0.9.0b2/gladier.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-07-20 17:38:20.000000 gladier-0.9.0b2/gladier.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-20 17:38:20.000000 gladier-0.9.0b2/gladier.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 17:38:20.000000 gladier-0.9.0b2/gladier.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-20 17:38:20.000000 gladier-0.9.0b2/gladier.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-20 17:38:20.000000 gladier-0.9.0b2/gladier.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-20 17:38:09.000000 gladier-0.9.0b2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-20 17:38:20.448307 gladier-0.9.0b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-20 17:38:09.000000 gladier-0.9.0b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:55:44.669411 gladier-0.9.0b3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-01 21:55:33.000000 gladier-0.9.0b3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-08-01 21:55:33.000000 gladier-0.9.0b3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-08-01 21:55:44.669411 gladier-0.9.0b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-08-01 21:55:33.000000 gladier-0.9.0b3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:55:44.661411 gladier-0.9.0b3/gladier/
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-08-01 21:55:34.000000 gladier-0.9.0b3/gladier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-08-01 21:55:34.000000 gladier-0.9.0b3/gladier/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23331 2023-08-01 21:55:34.000000 gladier-0.9.0b3/gladier/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-08-01 21:55:34.000000 gladier-0.9.0b3/gladier/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-08-01 21:55:34.000000 gladier-0.9.0b3/gladier/exc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-08-01 21:55:34.000000 gladier-0.9.0b3/gladier/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:55:44.665411 gladier-0.9.0b3/gladier/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-08-01 21:55:34.000000 gladier-0.9.0b3/gladier/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-08-01 21:55:34.000000 gladier-0.9.0b3/gladier/managers/compute_login_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-08-01 21:55:34.000000 gladier-0.9.0b3/gladier/managers/compute_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18883 2023-08-01 21:55:34.000000 gladier-0.9.0b3/gladier/managers/flows_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8534 2023-08-01 21:55:34.000000 gladier-0.9.0b3/gladier/managers/login_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-08-01 21:55:34.000000 gladier-0.9.0b3/gladier/managers/service_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7901 2023-08-01 21:55:34.000000 gladier-0.9.0b3/gladier/state_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:55:44.665411 gladier-0.9.0b3/gladier/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 21:55:34.000000 gladier-0.9.0b3/gladier/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-08-01 21:55:34.000000 gladier-0.9.0b3/gladier/storage/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7037 2023-08-01 21:55:34.000000 gladier-0.9.0b3/gladier/storage/migrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-08-01 21:55:34.000000 gladier-0.9.0b3/gladier/storage/tokens.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:55:44.665411 gladier-0.9.0b3/gladier/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-08-01 21:55:34.000000 gladier-0.9.0b3/gladier/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:55:44.665411 gladier-0.9.0b3/gladier/tools/builtins/
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-08-01 21:55:34.000000 gladier-0.9.0b3/gladier/tools/builtins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-08-01 21:55:34.000000 gladier-0.9.0b3/gladier/tools/builtins/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-08-01 21:55:34.000000 gladier-0.9.0b3/gladier/tools/builtins/choice_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-08-01 21:55:34.000000 gladier-0.9.0b3/gladier/tools/builtins/expression_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-08-01 21:55:34.000000 gladier-0.9.0b3/gladier/tools/builtins/fail.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-08-01 21:55:34.000000 gladier-0.9.0b3/gladier/tools/builtins/pass_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-08-01 21:55:34.000000 gladier-0.9.0b3/gladier/tools/builtins/wait.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:55:44.665411 gladier-0.9.0b3/gladier/tools/globus/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-08-01 21:55:34.000000 gladier-0.9.0b3/gladier/tools/globus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-08-01 21:55:34.000000 gladier-0.9.0b3/gladier/tools/globus/compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-08-01 21:55:34.000000 gladier-0.9.0b3/gladier/tools/globus/transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-08-01 21:55:34.000000 gladier-0.9.0b3/gladier/tools/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:55:44.665411 gladier-0.9.0b3/gladier/tools/posix/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-08-01 21:55:34.000000 gladier-0.9.0b3/gladier/tools/posix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-08-01 21:55:34.000000 gladier-0.9.0b3/gladier/tools/posix/shell_cmd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:55:44.669411 gladier-0.9.0b3/gladier/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 21:55:34.000000 gladier-0.9.0b3/gladier/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-08-01 21:55:34.000000 gladier-0.9.0b3/gladier/utils/automate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-08-01 21:55:34.000000 gladier-0.9.0b3/gladier/utils/dynamic_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-08-01 21:55:34.000000 gladier-0.9.0b3/gladier/utils/flow_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5849 2023-08-01 21:55:34.000000 gladier-0.9.0b3/gladier/utils/flow_modifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-08-01 21:55:34.000000 gladier-0.9.0b3/gladier/utils/flow_traversal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-08-01 21:55:34.000000 gladier-0.9.0b3/gladier/utils/name_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-08-01 21:55:34.000000 gladier-0.9.0b3/gladier/utils/tool_alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5072 2023-08-01 21:55:34.000000 gladier-0.9.0b3/gladier/utils/tool_chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-01 21:55:34.000000 gladier-0.9.0b3/gladier/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:55:44.661411 gladier-0.9.0b3/gladier.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-08-01 21:55:44.000000 gladier-0.9.0b3/gladier.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-08-01 21:55:44.000000 gladier-0.9.0b3/gladier.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 21:55:44.000000 gladier-0.9.0b3/gladier.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-08-01 21:55:44.000000 gladier-0.9.0b3/gladier.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-01 21:55:44.000000 gladier-0.9.0b3/gladier.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-08-01 21:55:34.000000 gladier-0.9.0b3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-08-01 21:55:44.669411 gladier-0.9.0b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-08-01 21:55:34.000000 gladier-0.9.0b3/setup.py
```

### Comparing `gladier-0.9.0b2/LICENSE` & `gladier-0.9.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `gladier-0.9.0b2/PKG-INFO` & `gladier-0.9.0b3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gladier
-Version: 0.9.0b2
+Version: 0.9.0b3
 Summary: Tooling for rapid deployment of automation tooling.
 Home-page: https://github.com/globus-gladier/gladier
 Maintainer: 
 Maintainer-email: 
 License: Apache 2.0
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `gladier-0.9.0b2/README.rst` & `gladier-0.9.0b3/README.rst`

 * *Files identical despite different names*

### Comparing `gladier-0.9.0b2/gladier/base.py` & `gladier-0.9.0b3/gladier/base.py`

 * *Files identical despite different names*

### Comparing `gladier-0.9.0b2/gladier/client.py` & `gladier-0.9.0b3/gladier/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,34 @@
+from __future__ import annotations
+
+import typing as t
+
+import logging
 import os
 import pathlib
-import logging
 from collections.abc import Iterable
 
-from gladier.base import GladierBaseTool
-from gladier.managers.login_manager import (
-    BaseLoginManager,
-    AutoLoginManager,
-    ConfidentialClientLoginManager,
-)
-from globus_sdk import AccessTokenAuthorizer, RefreshTokenAuthorizer
-from gladier.managers import FlowsManager, ComputeManager
-
-from gladier.storage.tokens import GladierSecretsConfig
 import gladier
+import gladier.exc
+import gladier.managers.compute_login_manager
 import gladier.storage.config
-import gladier.utils.dynamic_imports
+import gladier.storage.migrations
 import gladier.utils.automate
+import gladier.utils.dynamic_imports
 import gladier.utils.name_generation
-import gladier.storage.migrations
 import gladier.utils.tool_alias
-import gladier.managers.compute_login_manager
-import gladier.exc
 import gladier.version
+from gladier.base import GladierBaseTool
+from gladier.managers import ComputeManager, FlowsManager
+from gladier.managers.login_manager import (
+    AutoLoginManager,
+    BaseLoginManager,
+    ConfidentialClientLoginManager,
+)
+from gladier.storage.tokens import GladierSecretsConfig
 
 log = logging.getLogger(__name__)
 
 
 class GladierBaseClient(object):
     """
     The Gladier Client ties together commonly used compute functions
@@ -96,26 +98,26 @@
                           will auto-login when additional scopes are needed.
     :param flows_manager: A flows manager class with customized behavior. Attrs like group
                           and login_manager will automatically be set if None
     :raises gladier.exc.AuthException: if authorizers given are insufficient
 
     """
 
-    secret_config_filename: str = None
-    app_name: str = "Gladier Client"
+    secret_config_filename: t.Optional[str] = None
+    app_name: t.Optional[str] = "Gladier Client"
     client_id: str = "f1631610-d9e4-4db2-81ba-7f93ad4414e3"
-    globus_group: str = None
-    subscription_id: str = None
+    globus_group: t.Optional[str] = None
+    subscription_id: t.Optional[str] = None
     alias_class = gladier.utils.tool_alias.StateSuffixVariablePrefix
 
     def __init__(
         self,
         auto_registration: bool = True,
-        login_manager: BaseLoginManager = None,
-        flows_manager: FlowsManager = None,
+        login_manager: t.Optional[BaseLoginManager] = None,
+        flows_manager: t.Optional[FlowsManager] = None,
     ):
         self._tools = None
         self.storage = self._determine_storage()
         self.login_manager = login_manager or self._determine_login_manager(
             self.storage
         )
 
@@ -199,15 +201,17 @@
             _, alias = gladier.utils.dynamic_imports.parse_alias(tool_ref)
             default_inst = default_cls(alias, alias_class)
             if issubclass(type(default_inst), gladier.base.GladierBaseTool):
                 return default_inst
             raise gladier.exc.ConfigException(
                 f"{default_inst} is not of type " f"{gladier.base.GladierBaseTool}"
             )
-        elif isinstance(tool_ref, gladier.base.GladierBaseTool):
+        elif isinstance(
+            tool_ref, (gladier.base.GladierBaseTool, gladier.GladierBaseState)
+        ):
             return tool_ref
         else:
             cls_inst = tool_ref()
             if isinstance(cls_inst, gladier.base.GladierBaseTool):
                 return cls_inst
             raise gladier.exc.ConfigException(
                 f'"{tool_ref}" must be a {gladier.base.GladierBaseTool} or a dotted import '
@@ -285,29 +289,32 @@
     def get_flow_definition(self):
         """
         Get the flow definition attached to this class. If the flow definition is an import string,
         it will automatically load the import string and return the full flow.
 
         :return: A dict of the Automate Flow definition
         """
-        if not getattr(self, "flow_definition", None):
+        try:
+            if isinstance(self.flow_definition, dict):
+                return self.flow_definition
+            elif isinstance(self.flow_definition, str):
+                return self.get_gladier_defaults_cls(
+                    self.flow_definition
+                ).flow_definition
+            else:
+                raise gladier.exc.ConfigException(
+                    '"flow_definition" must be a dict or an import string '
+                    "to a sub-class of type "
+                    '"gladier.GladierBaseTool"'
+                )
+        except AttributeError:
             raise gladier.exc.ConfigException(
-                f'"flow_definition" was not set on ' f"{self.__class__.__name__}"
+                '"flow_definition" was not set on ' f"{self.__class__.__name__}"
             )
 
-        if isinstance(self.flow_definition, dict):
-            return self.flow_definition
-        elif isinstance(self.flow_definition, str):
-            return self.get_gladier_defaults_cls(self.flow_definition).flow_definition
-        raise gladier.exc.ConfigException(
-            '"flow_definition" must be a dict or an import string '
-            "to a sub-class of type "
-            '"gladier.GladierBaseTool"'
-        )
-
     def get_flow_schema(self):
         """
         Get the flow schema attached to this class.
         """
         return getattr(self, "flow_schema", None)
 
     def sync_flow(self):
@@ -507,7 +514,23 @@
                           on the current tool being run.
         :param state_name: The state in the automate definition to fetch
         :returns: sub-dict of get_status() describing the :state_name:.
         """
         return gladier.utils.automate.get_details(
             self.get_status(action_id), state_name
         )
+
+
+class GladierClient(GladierBaseClient):
+    def __init__(
+        self,
+        flow_definition: t.Mapping[str, t.Any],
+        auto_registration: bool = True,
+        login_manager: t.Optional[BaseLoginManager] = None,
+        flows_manager: t.Optional[FlowsManager] = None,
+    ):
+        super().__init__(
+            auto_registration=auto_registration,
+            login_manager=login_manager,
+            flows_manager=flows_manager,
+        )
+        self.flow_definition = flow_definition
```

### Comparing `gladier-0.9.0b2/gladier/decorators.py` & `gladier-0.9.0b3/gladier/decorators.py`

 * *Files identical despite different names*

### Comparing `gladier-0.9.0b2/gladier/exc.py` & `gladier-0.9.0b3/gladier/exc.py`

 * *Files identical despite different names*

### Comparing `gladier-0.9.0b2/gladier/managers/compute_login_manager.py` & `gladier-0.9.0b3/gladier/managers/compute_login_manager.py`

 * *Files identical despite different names*

### Comparing `gladier-0.9.0b2/gladier/managers/compute_manager.py` & `gladier-0.9.0b3/gladier/managers/compute_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-import logging
 import hashlib
+import logging
 
+import gladier.managers.compute_login_manager
 from gladier.base import GladierBaseTool
 from gladier.managers.service_manager import ServiceManager
-from globus_compute_sdk import serialize, Client
-
-import gladier.managers.compute_login_manager
+from globus_compute_sdk import Client, serialize
 
 log = logging.getLogger(__name__)
 
 
 class ComputeManager(ServiceManager):
     def __init__(self, auto_registration: bool = True, **kwargs):
         super().__init__(**kwargs)
@@ -37,15 +36,15 @@
             login_manager=compute_login_manager
     )
         return self.__compute_client
 
     @staticmethod
     def get_compute_function_name(compute_function):
         """
-        Generate a function name given a compute function. These function namse are used to refer
+        Generate a function name given a compute function. These function names are used to refer
         to compute functions within the config. There is no guarantee of uniqueness for function
         names.
 
         :return: human readable string identifier for a function (intended for a gladier.cfg file)
         """
         return f"{compute_function.__name__}_function_id"
```

### Comparing `gladier-0.9.0b2/gladier/managers/flows_manager.py` & `gladier-0.9.0b3/gladier/managers/flows_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,34 +1,32 @@
-import logging
-import warnings
 import hashlib
 import json
+import logging
+import warnings
 from typing import Callable
 
-import globus_sdk
-import globus_automate_client
-
 import gladier
-from gladier.managers.service_manager import ServiceManager
+import gladier.exc
+import gladier.managers.compute_login_manager
 import gladier.storage.config
-import gladier.utils.dynamic_imports
+import gladier.storage.migrations
 import gladier.utils.automate
+import gladier.utils.dynamic_imports
 import gladier.utils.name_generation
-import gladier.storage.migrations
 import gladier.utils.tool_alias
-import gladier.managers.compute_login_manager
-import gladier.exc
 import gladier.version
-
+import globus_automate_client
+import globus_sdk
+from gladier.managers.service_manager import ServiceManager
 from globus_automate_client.flows_client import (
     MANAGE_FLOWS_SCOPE,
-    VIEW_FLOWS_SCOPE,
     RUN_FLOWS_SCOPE,
-    RUN_STATUS_SCOPE,
     RUN_MANAGE_SCOPE,
+    RUN_STATUS_SCOPE,
+    VIEW_FLOWS_SCOPE,
 )
 
 log = logging.getLogger(__name__)
 
 
 def ensure_flow_registered(
     flows_manager_instance, exc: gladier.exc.RegistrationException
@@ -267,15 +265,15 @@
             self.check_flow()
         except gladier.exc.RegistrationException:
             return True
         return False
 
     def check_flow(self):
         """
-        Check if the flow has changed by validating the current flow_definition agaist
+        Check if the flow has changed by validating the current flow_definition against
         the stored checksum. Raises an exception if the checksums do not match.
 
         :raises: gladier.exc.NoFlowRegistered if no flow has been registered
         :raises: gladier.exc.FlowObsolete if the stored flow checksums do not match
         """
         flow_id = self.get_flow_id()
         flow_checksum = self.storage.get_value("flow_checksum")
```

### Comparing `gladier-0.9.0b2/gladier/managers/login_manager.py` & `gladier-0.9.0b3/gladier/managers/login_manager.py`

 * *Files identical despite different names*

### Comparing `gladier-0.9.0b2/gladier/managers/service_manager.py` & `gladier-0.9.0b3/gladier/managers/service_manager.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 import logging
-from typing import List
+from typing import List, Optional
 import abc
 from gladier.managers.login_manager import BaseLoginManager
 from gladier.storage.config import GladierConfig
 
 
 log = logging.getLogger(__name__)
 
 
 class ServiceManager(abc.ABC):
-    def __init__(self, **kwargs):
-        self._storage = kwargs.get("storage")
+    def __init__(
+        self,
+        storage: Optional[GladierConfig] = None,
+        login_manager: Optional[BaseLoginManager] = None,
+        **kwargs,
+    ):
+        self._storage = storage
 
-        self.login_manager = kwargs.get("login_manager")
+        self.login_manager = login_manager
         self.register_scopes()
 
     @property
     def storage(self):
         if self._storage is None:
             raise AttributeError(f"Storage has not been set for {self}")
         return self._storage
```

### Comparing `gladier-0.9.0b2/gladier/storage/config.py` & `gladier-0.9.0b3/gladier/storage/config.py`

 * *Files identical despite different names*

### Comparing `gladier-0.9.0b2/gladier/storage/migrations.py` & `gladier-0.9.0b3/gladier/storage/migrations.py`

 * *Files identical despite different names*

### Comparing `gladier-0.9.0b2/gladier/storage/tokens.py` & `gladier-0.9.0b3/gladier/storage/tokens.py`

 * *Files identical despite different names*

### Comparing `gladier-0.9.0b2/gladier/utils/automate.py` & `gladier-0.9.0b3/gladier/utils/automate.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,25 @@
-import traceback
+from __future__ import annotations
+
 import logging
+
 from globus_compute_sdk import serialize
 
 log = logging.getLogger(__name__)
 
 automate_response_keys = {"action_id", "status", "state_name"}
 compute_response_keys = {"result", "status", "exception", "task_id"}
+import traceback
+
+from globus_compute_sdk.serialize import ComputeSerializer
+
+log = logging.getLogger(__name__)
+
+automate_response_keys = {"action_id", "status", "state_name"}
+funcx_response_keys = {"result", "status", "exception", "task_id"}
 
 
 def is_automate_response(state_output):
     return isinstance(state_output, dict) and set(state_output.keys()).intersection(
         automate_response_keys
     )
 
@@ -40,10 +50,10 @@
             exc = deserialize_exception(data["details"]["exception"])
             data["details"]["exception"] = exc
     return response
 
 
 def deserialize_exception(encoded_exc):
     try:
-        serialize.ComputeSerializer().deserialize(encoded_exc).reraise()
+        ComputeSerializer().deserialize(encoded_exc).reraise()
     except Exception:
         return traceback.format_exc()
```

### Comparing `gladier-0.9.0b2/gladier/utils/dynamic_imports.py` & `gladier-0.9.0b3/gladier/utils/dynamic_imports.py`

 * *Files identical despite different names*

### Comparing `gladier-0.9.0b2/gladier/utils/flow_generation.py` & `gladier-0.9.0b3/gladier/utils/flow_generation.py`

 * *Files identical despite different names*

### Comparing `gladier-0.9.0b2/gladier/utils/flow_modifiers.py` & `gladier-0.9.0b3/gladier/utils/flow_modifiers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+
 from gladier.exc import FlowModifierException
 from gladier.utils.name_generation import get_compute_flow_state_name
 
 log = logging.getLogger(__name__)
 compute_modifiers = {"endpoint", "payload", "tasks"}
 # All top level states can be modified.
 # https://globus-automate-client.readthedocs.io/en/latest/authoring_flows.html#action-state-type
@@ -26,15 +27,17 @@
     supported_modifiers = state_modifiers.union(compute_modifiers)
     compute_modifiers = compute_modifiers
     state_modifiers = state_modifiers
 
     def __init__(self, tools, modifiers, cls=None):
         self.cls = cls
         self.tools = tools
-        self.functions = [func for tool in tools for func in tool.compute_functions]
+        self.functions = [
+            func for tool in tools for func in getattr(tool, "compute_functions", [])
+        ]
         self.function_names = [f.__name__ for f in self.functions]
         self.state_names = [get_compute_flow_state_name(f) for f in self.functions]
         self.modifiers = modifiers
         self.check_modifiers()
 
     def get_function(self, function_identifier):
         if function_identifier in self.function_names:
```

### Comparing `gladier-0.9.0b2/gladier/utils/flow_traversal.py` & `gladier-0.9.0b3/gladier/utils/flow_traversal.py`

 * *Files identical despite different names*

### Comparing `gladier-0.9.0b2/gladier/utils/name_generation.py` & `gladier-0.9.0b3/gladier/utils/name_generation.py`

 * *Files identical despite different names*

### Comparing `gladier-0.9.0b2/gladier/utils/tool_alias.py` & `gladier-0.9.0b3/gladier/utils/tool_alias.py`

 * *Files identical despite different names*

### Comparing `gladier-0.9.0b2/gladier/utils/tool_chain.py` & `gladier-0.9.0b3/gladier/utils/tool_chain.py`

 * *Files identical despite different names*

### Comparing `gladier-0.9.0b2/gladier.egg-info/PKG-INFO` & `gladier-0.9.0b3/gladier.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gladier
-Version: 0.9.0b2
+Version: 0.9.0b3
 Summary: Tooling for rapid deployment of automation tooling.
 Home-page: https://github.com/globus-gladier/gladier
 Maintainer: 
 Maintainer-email: 
 License: Apache 2.0
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `gladier-0.9.0b2/setup.py` & `gladier-0.9.0b3/setup.py`

 * *Files identical despite different names*

