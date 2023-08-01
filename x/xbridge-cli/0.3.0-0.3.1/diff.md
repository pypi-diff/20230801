# Comparing `tmp/xbridge_cli-0.3.0.tar.gz` & `tmp/xbridge_cli-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xbridge_cli-0.3.0.tar", max compression
+gzip compressed data, was "xbridge_cli-0.3.1.tar", max compression
```

## Comparing `xbridge_cli-0.3.0.tar` & `xbridge_cli-0.3.1.tar`

### file list

```diff
@@ -1,45 +1,46 @@
--rw-r--r--   0        0        0     1076 2022-06-02 18:55:19.569628 xbridge_cli-0.3.0/LICENSE
--rw-r--r--   0        0        0      941 2023-04-12 21:26:10.799452 xbridge_cli-0.3.0/README.md
--rw-r--r--   0        0        0     1350 2023-04-17 21:02:02.743330 xbridge_cli-0.3.0/pyproject.toml
--rw-r--r--   0        0        0       51 2023-04-12 21:26:10.827320 xbridge_cli-0.3.0/xbridge_cli/__init__.py
--rw-r--r--   0        0        0      642 2023-04-12 21:26:10.829434 xbridge_cli-0.3.0/xbridge_cli/bridge/__init__.py
--rw-r--r--   0        0        0    18431 2023-04-17 20:46:34.649920 xbridge_cli-0.3.0/xbridge_cli/bridge/build.py
--rw-r--r--   0        0        0     6260 2023-04-17 20:43:50.122911 xbridge_cli-0.3.0/xbridge_cli/bridge/create_account.py
--rw-r--r--   0        0        0     6477 2023-04-12 21:26:10.832975 xbridge_cli-0.3.0/xbridge_cli/bridge/register.py
--rw-r--r--   0        0        0     8049 2023-04-17 20:43:50.124018 xbridge_cli-0.3.0/xbridge_cli/bridge/transfer.py
--rw-r--r--   0        0        0      500 2023-04-12 21:26:10.834687 xbridge_cli-0.3.0/xbridge_cli/exceptions.py
--rw-r--r--   0        0        0      680 2023-04-17 20:41:09.822418 xbridge_cli-0.3.0/xbridge_cli/main.py
--rw-r--r--   0        0        0       20 2023-04-12 21:26:10.837291 xbridge_cli-0.3.0/xbridge_cli/misc/__init__.py
--rw-r--r--   0        0        0     6174 2023-04-12 21:26:10.838312 xbridge_cli-0.3.0/xbridge_cli/misc/explorer.html
--rw-r--r--   0        0        0      406 2023-04-12 21:26:10.839082 xbridge_cli-0.3.0/xbridge_cli/misc/explorer.py
--rw-r--r--   0        0        0     2094 2023-04-17 20:41:09.824441 xbridge_cli-0.3.0/xbridge_cli/misc/fund.py
--rw-r--r--   0        0        0     1700 2023-04-12 21:26:10.841233 xbridge_cli-0.3.0/xbridge_cli/misc/trust.py
--rw-r--r--   0        0        0     1109 2023-04-12 21:26:10.841776 xbridge_cli-0.3.0/xbridge_cli/server/__init__.py
--rw-r--r--   0        0        0      614 2023-04-12 21:26:10.842765 xbridge_cli-0.3.0/xbridge_cli/server/config/__init__.py
--rw-r--r--   0        0        0    18276 2023-04-17 20:43:50.125098 xbridge_cli-0.3.0/xbridge_cli/server/config/config.py
--rw-r--r--   0        0        0     2253 2023-04-12 21:26:10.845523 xbridge_cli-0.3.0/xbridge_cli/server/config/ports.py
--rw-r--r--   0        0        0     1360 2023-04-12 21:26:10.847508 xbridge_cli-0.3.0/xbridge_cli/server/config/templates/bootstrap.jinja
--rw-r--r--   0        0        0     1806 2023-04-12 21:26:10.848692 xbridge_cli-0.3.0/xbridge_cli/server/config/templates/rippled.jinja
--rw-r--r--   0        0        0     1518 2023-04-12 21:26:10.849839 xbridge_cli-0.3.0/xbridge_cli/server/config/templates/witness.jinja
--rw-r--r--   0        0        0     1403 2023-04-12 21:26:10.851113 xbridge_cli-0.3.0/xbridge_cli/server/list.py
--rw-r--r--   0        0        0      721 2023-04-12 21:26:10.851992 xbridge_cli-0.3.0/xbridge_cli/server/print.py
--rw-r--r--   0        0        0     2338 2023-04-12 21:26:10.852613 xbridge_cli-0.3.0/xbridge_cli/server/request.py
--rw-r--r--   0        0        0     2156 2023-04-12 21:26:10.853921 xbridge_cli-0.3.0/xbridge_cli/server/restart.py
--rw-r--r--   0        0        0    12440 2023-04-17 20:46:34.651131 xbridge_cli-0.3.0/xbridge_cli/server/start.py
--rw-r--r--   0        0        0     2834 2023-04-12 21:26:10.855973 xbridge_cli-0.3.0/xbridge_cli/server/stop.py
--rw-r--r--   0        0        0     1341 2023-04-12 21:26:10.856994 xbridge_cli-0.3.0/xbridge_cli/utils/__init__.py
--rw-r--r--   0        0        0     4741 2023-04-12 21:26:10.857889 xbridge_cli-0.3.0/xbridge_cli/utils/attestations.py
--rw-r--r--   0        0        0      539 2023-04-12 21:26:10.858776 xbridge_cli-0.3.0/xbridge_cli/utils/config_file/__init__.py
--rw-r--r--   0        0        0     2399 2023-04-12 21:26:10.859431 xbridge_cli-0.3.0/xbridge_cli/utils/config_file/bridge_config.py
--rw-r--r--   0        0        0     1189 2023-04-12 21:26:10.860319 xbridge_cli-0.3.0/xbridge_cli/utils/config_file/chain_config.py
--rw-r--r--   0        0        0     5813 2023-04-12 21:26:10.861145 xbridge_cli-0.3.0/xbridge_cli/utils/config_file/config_file.py
--rw-r--r--   0        0        0      543 2023-04-12 21:26:10.862021 xbridge_cli-0.3.0/xbridge_cli/utils/config_file/config_item.py
--rw-r--r--   0        0        0      702 2023-04-12 21:26:10.862611 xbridge_cli-0.3.0/xbridge_cli/utils/config_file/server_config.py
--rw-r--r--   0        0        0      840 2023-04-12 21:26:10.864534 xbridge_cli-0.3.0/xbridge_cli/utils/config_file/witness_config.py
--rw-r--r--   0        0        0     6603 2023-04-12 21:26:10.865568 xbridge_cli-0.3.0/xbridge_cli/utils/config_utils.py
--rw-r--r--   0        0        0      665 2023-04-12 21:26:10.867038 xbridge_cli-0.3.0/xbridge_cli/utils/misc.py
--rw-r--r--   0        0        0     5073 2023-04-12 21:26:10.868191 xbridge_cli-0.3.0/xbridge_cli/utils/rippled_config.py
--rw-r--r--   0        0        0     2596 2023-04-12 21:26:10.869342 xbridge_cli-0.3.0/xbridge_cli/utils/transaction.py
--rw-r--r--   0        0        0     1075 2023-04-12 21:26:10.871219 xbridge_cli-0.3.0/xbridge_cli/utils/types.py
--rw-r--r--   0        0        0     2189 1970-01-01 00:00:00.000000 xbridge_cli-0.3.0/setup.py
--rw-r--r--   0        0        0     2007 1970-01-01 00:00:00.000000 xbridge_cli-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2022-06-02 18:55:19.569628 xbridge_cli-0.3.1/LICENSE
+-rw-r--r--   0        0        0      941 2023-04-12 21:26:10.799452 xbridge_cli-0.3.1/README.md
+-rw-r--r--   0        0        0     1350 2023-08-01 02:12:29.337845 xbridge_cli-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0       51 2023-04-12 21:26:10.827320 xbridge_cli-0.3.1/xbridge_cli/__init__.py
+-rw-r--r--   0        0        0      642 2023-04-12 21:26:10.829434 xbridge_cli-0.3.1/xbridge_cli/bridge/__init__.py
+-rw-r--r--   0        0        0    18955 2023-08-01 02:12:29.341217 xbridge_cli-0.3.1/xbridge_cli/bridge/build.py
+-rw-r--r--   0        0        0     6260 2023-08-01 02:12:29.342437 xbridge_cli-0.3.1/xbridge_cli/bridge/create_account.py
+-rw-r--r--   0        0        0     6477 2023-04-12 21:26:10.832975 xbridge_cli-0.3.1/xbridge_cli/bridge/register.py
+-rw-r--r--   0        0        0     8049 2023-08-01 02:12:29.343442 xbridge_cli-0.3.1/xbridge_cli/bridge/transfer.py
+-rw-r--r--   0        0        0      500 2023-04-12 21:26:10.834687 xbridge_cli-0.3.1/xbridge_cli/exceptions.py
+-rw-r--r--   0        0        0      680 2023-04-17 20:41:09.822418 xbridge_cli-0.3.1/xbridge_cli/main.py
+-rw-r--r--   0        0        0       20 2023-04-12 21:26:10.837291 xbridge_cli-0.3.1/xbridge_cli/misc/__init__.py
+-rw-r--r--   0        0        0     6174 2023-04-12 21:26:10.838312 xbridge_cli-0.3.1/xbridge_cli/misc/explorer.html
+-rw-r--r--   0        0        0      406 2023-04-12 21:26:10.839082 xbridge_cli-0.3.1/xbridge_cli/misc/explorer.py
+-rw-r--r--   0        0        0     2094 2023-08-01 02:12:29.344324 xbridge_cli-0.3.1/xbridge_cli/misc/fund.py
+-rw-r--r--   0        0        0     1700 2023-08-01 02:12:29.345090 xbridge_cli-0.3.1/xbridge_cli/misc/trust.py
+-rw-r--r--   0        0        0     1109 2023-04-12 21:26:10.841776 xbridge_cli-0.3.1/xbridge_cli/server/__init__.py
+-rw-r--r--   0        0        0      614 2023-04-12 21:26:10.842765 xbridge_cli-0.3.1/xbridge_cli/server/config/__init__.py
+-rw-r--r--   0        0        0    18276 2023-08-01 02:12:29.345999 xbridge_cli-0.3.1/xbridge_cli/server/config/config.py
+-rw-r--r--   0        0        0     2253 2023-04-12 21:26:10.845523 xbridge_cli-0.3.1/xbridge_cli/server/config/ports.py
+-rw-r--r--   0        0        0     1360 2023-04-12 21:26:10.847508 xbridge_cli-0.3.1/xbridge_cli/server/config/templates/bootstrap.jinja
+-rw-r--r--   0        0        0     1806 2023-04-12 21:26:10.848692 xbridge_cli-0.3.1/xbridge_cli/server/config/templates/rippled.jinja
+-rw-r--r--   0        0        0     1518 2023-04-12 21:26:10.849839 xbridge_cli-0.3.1/xbridge_cli/server/config/templates/witness.jinja
+-rw-r--r--   0        0        0     2322 2023-08-01 02:12:15.179860 xbridge_cli-0.3.1/xbridge_cli/server/docker-compose.yml
+-rw-r--r--   0        0        0     1403 2023-04-12 21:26:10.851113 xbridge_cli-0.3.1/xbridge_cli/server/list.py
+-rw-r--r--   0        0        0      721 2023-04-12 21:26:10.851992 xbridge_cli-0.3.1/xbridge_cli/server/print.py
+-rw-r--r--   0        0        0     2338 2023-04-12 21:26:10.852613 xbridge_cli-0.3.1/xbridge_cli/server/request.py
+-rw-r--r--   0        0        0     2156 2023-04-12 21:26:10.853921 xbridge_cli-0.3.1/xbridge_cli/server/restart.py
+-rw-r--r--   0        0        0    12388 2023-08-01 02:12:15.181035 xbridge_cli-0.3.1/xbridge_cli/server/start.py
+-rw-r--r--   0        0        0     2834 2023-04-12 21:26:10.855973 xbridge_cli-0.3.1/xbridge_cli/server/stop.py
+-rw-r--r--   0        0        0     1341 2023-04-12 21:26:10.856994 xbridge_cli-0.3.1/xbridge_cli/utils/__init__.py
+-rw-r--r--   0        0        0     4741 2023-04-12 21:26:10.857889 xbridge_cli-0.3.1/xbridge_cli/utils/attestations.py
+-rw-r--r--   0        0        0      539 2023-04-12 21:26:10.858776 xbridge_cli-0.3.1/xbridge_cli/utils/config_file/__init__.py
+-rw-r--r--   0        0        0     2399 2023-04-12 21:26:10.859431 xbridge_cli-0.3.1/xbridge_cli/utils/config_file/bridge_config.py
+-rw-r--r--   0        0        0     1189 2023-04-12 21:26:10.860319 xbridge_cli-0.3.1/xbridge_cli/utils/config_file/chain_config.py
+-rw-r--r--   0        0        0     5813 2023-04-12 21:26:10.861145 xbridge_cli-0.3.1/xbridge_cli/utils/config_file/config_file.py
+-rw-r--r--   0        0        0      543 2023-04-12 21:26:10.862021 xbridge_cli-0.3.1/xbridge_cli/utils/config_file/config_item.py
+-rw-r--r--   0        0        0      702 2023-04-12 21:26:10.862611 xbridge_cli-0.3.1/xbridge_cli/utils/config_file/server_config.py
+-rw-r--r--   0        0        0      840 2023-04-12 21:26:10.864534 xbridge_cli-0.3.1/xbridge_cli/utils/config_file/witness_config.py
+-rw-r--r--   0        0        0     6603 2023-04-12 21:26:10.865568 xbridge_cli-0.3.1/xbridge_cli/utils/config_utils.py
+-rw-r--r--   0        0        0      665 2023-04-12 21:26:10.867038 xbridge_cli-0.3.1/xbridge_cli/utils/misc.py
+-rw-r--r--   0        0        0     5073 2023-04-12 21:26:10.868191 xbridge_cli-0.3.1/xbridge_cli/utils/rippled_config.py
+-rw-r--r--   0        0        0     2596 2023-08-01 02:12:29.347183 xbridge_cli-0.3.1/xbridge_cli/utils/transaction.py
+-rw-r--r--   0        0        0     1075 2023-04-12 21:26:10.871219 xbridge_cli-0.3.1/xbridge_cli/utils/types.py
+-rw-r--r--   0        0        0     2189 1970-01-01 00:00:00.000000 xbridge_cli-0.3.1/setup.py
+-rw-r--r--   0        0        0     2007 1970-01-01 00:00:00.000000 xbridge_cli-0.3.1/PKG-INFO
```

### Comparing `xbridge_cli-0.3.0/LICENSE` & `xbridge_cli-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xbridge_cli-0.3.0/README.md` & `xbridge_cli-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `xbridge_cli-0.3.0/pyproject.toml` & `xbridge_cli-0.3.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xbridge-cli"
-version = "0.3.0"
+version = "0.3.1"
 description = "A CLI that helps you set up an XRPL-XRPL bridge."
 readme = "README.md"
 repository = "https://github.com/xpring-eng/xbridge-cli"
 authors = ["Mayukha Vadari <mvadari@ripple.com>"]
 keywords = [
   "xrp",
   "xrpl",
```

### Comparing `xbridge_cli-0.3.0/xbridge_cli/bridge/__init__.py` & `xbridge_cli-0.3.1/xbridge_cli/bridge/__init__.py`

 * *Files identical despite different names*

### Comparing `xbridge_cli-0.3.0/xbridge_cli/bridge/build.py` & `xbridge_cli-0.3.1/xbridge_cli/bridge/build.py`

 * *Files 8% similar despite different names*

```diff
@@ -317,17 +317,23 @@
                 )
             )
 
     # create the bridge
 
     # check if the bridge already exists
     locking_bridge_exists = False
-    locking_door_objs = locking_client.request(
+    locking_objs_result = locking_client.request(
         AccountObjects(account=locking_door, type=AccountObjectType.BRIDGE)
-    ).result["account_objects"]
+    ).result
+    if "account_objects" not in locking_objs_result:
+        obj_error = locking_objs_result.get("error_message") or json.dumps(
+            locking_objs_result
+        )
+        raise XBridgeCLIException(obj_error)
+    locking_door_objs = locking_objs_result["account_objects"]
     if len(locking_door_objs) > 0:
         assert (
             len(locking_door_objs) == 1
         ), "Cannot have multiple bridges on one account"
         if XChainBridge.from_xrpl(locking_door_objs[0]["XChainBridge"]) == bridge_obj:
             locking_bridge_exists = True
         else:
@@ -433,17 +439,23 @@
 
     issuing_txs: List[Transaction] = []
 
     # create the bridge
 
     # check if the bridge already exists
     issuing_bridge_exists = False
-    issuing_door_objs = issuing_client.request(
+    issuing_objs_result = issuing_client.request(
         AccountObjects(account=issuing_door, type=AccountObjectType.BRIDGE)
-    ).result["account_objects"]
+    ).result
+    if "account_objects" not in issuing_objs_result:
+        obj_error = issuing_objs_result.get("error_message") or json.dumps(
+            issuing_objs_result
+        )
+        raise XBridgeCLIException(obj_error)
+    issuing_door_objs = issuing_objs_result["account_objects"]
     if len(issuing_door_objs) > 0:
         assert (
             len(issuing_door_objs) == 1
         ), "Cannot have multiple bridges on one account"
         if XChainBridge.from_xrpl(issuing_door_objs[0]["XChainBridge"]) == bridge_obj:
             issuing_bridge_exists = True
         else:
```

### Comparing `xbridge_cli-0.3.0/xbridge_cli/bridge/create_account.py` & `xbridge_cli-0.3.1/xbridge_cli/bridge/create_account.py`

 * *Files identical despite different names*

### Comparing `xbridge_cli-0.3.0/xbridge_cli/bridge/register.py` & `xbridge_cli-0.3.1/xbridge_cli/bridge/register.py`

 * *Files identical despite different names*

### Comparing `xbridge_cli-0.3.0/xbridge_cli/bridge/transfer.py` & `xbridge_cli-0.3.1/xbridge_cli/bridge/transfer.py`

 * *Files identical despite different names*

### Comparing `xbridge_cli-0.3.0/xbridge_cli/main.py` & `xbridge_cli-0.3.1/xbridge_cli/main.py`

 * *Files identical despite different names*

### Comparing `xbridge_cli-0.3.0/xbridge_cli/misc/explorer.html` & `xbridge_cli-0.3.1/xbridge_cli/misc/explorer.html`

 * *Files identical despite different names*

### Comparing `xbridge_cli-0.3.0/xbridge_cli/misc/fund.py` & `xbridge_cli-0.3.1/xbridge_cli/misc/fund.py`

 * *Files identical despite different names*

### Comparing `xbridge_cli-0.3.0/xbridge_cli/misc/trust.py` & `xbridge_cli-0.3.1/xbridge_cli/misc/trust.py`

 * *Files identical despite different names*

### Comparing `xbridge_cli-0.3.0/xbridge_cli/server/__init__.py` & `xbridge_cli-0.3.1/xbridge_cli/server/__init__.py`

 * *Files identical despite different names*

### Comparing `xbridge_cli-0.3.0/xbridge_cli/server/config/__init__.py` & `xbridge_cli-0.3.1/xbridge_cli/server/config/__init__.py`

 * *Files identical despite different names*

### Comparing `xbridge_cli-0.3.0/xbridge_cli/server/config/config.py` & `xbridge_cli-0.3.1/xbridge_cli/server/config/config.py`

 * *Files identical despite different names*

### Comparing `xbridge_cli-0.3.0/xbridge_cli/server/config/ports.py` & `xbridge_cli-0.3.1/xbridge_cli/server/config/ports.py`

 * *Files identical despite different names*

### Comparing `xbridge_cli-0.3.0/xbridge_cli/server/config/templates/bootstrap.jinja` & `xbridge_cli-0.3.1/xbridge_cli/server/config/templates/bootstrap.jinja`

 * *Files identical despite different names*

### Comparing `xbridge_cli-0.3.0/xbridge_cli/server/config/templates/rippled.jinja` & `xbridge_cli-0.3.1/xbridge_cli/server/config/templates/rippled.jinja`

 * *Files identical despite different names*

### Comparing `xbridge_cli-0.3.0/xbridge_cli/server/config/templates/witness.jinja` & `xbridge_cli-0.3.1/xbridge_cli/server/config/templates/witness.jinja`

 * *Files identical despite different names*

### Comparing `xbridge_cli-0.3.0/xbridge_cli/server/list.py` & `xbridge_cli-0.3.1/xbridge_cli/server/list.py`

 * *Files identical despite different names*

### Comparing `xbridge_cli-0.3.0/xbridge_cli/server/print.py` & `xbridge_cli-0.3.1/xbridge_cli/server/print.py`

 * *Files identical despite different names*

### Comparing `xbridge_cli-0.3.0/xbridge_cli/server/request.py` & `xbridge_cli-0.3.1/xbridge_cli/server/request.py`

 * *Files identical despite different names*

### Comparing `xbridge_cli-0.3.0/xbridge_cli/server/restart.py` & `xbridge_cli-0.3.1/xbridge_cli/server/restart.py`

 * *Files identical despite different names*

### Comparing `xbridge_cli-0.3.0/xbridge_cli/server/start.py` & `xbridge_cli-0.3.1/xbridge_cli/server/start.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,17 +24,14 @@
     get_config_folder,
 )
 
 _DOCKER_COMPOSE_FILE = os.path.abspath(
     os.path.join(
         os.path.realpath(__file__),
         "..",
-        "..",
-        "..",
-        "docker-setup",
         "docker-compose.yml",
     )
 )
 
 _DOCKER_COMPOSE = ["docker", "compose", "-f", _DOCKER_COMPOSE_FILE]
 
 _START_UP_TIME = 30  # seconds
```

### Comparing `xbridge_cli-0.3.0/xbridge_cli/server/stop.py` & `xbridge_cli-0.3.1/xbridge_cli/server/stop.py`

 * *Files identical despite different names*

### Comparing `xbridge_cli-0.3.0/xbridge_cli/utils/__init__.py` & `xbridge_cli-0.3.1/xbridge_cli/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `xbridge_cli-0.3.0/xbridge_cli/utils/attestations.py` & `xbridge_cli-0.3.1/xbridge_cli/utils/attestations.py`

 * *Files identical despite different names*

### Comparing `xbridge_cli-0.3.0/xbridge_cli/utils/config_file/__init__.py` & `xbridge_cli-0.3.1/xbridge_cli/utils/config_file/__init__.py`

 * *Files identical despite different names*

### Comparing `xbridge_cli-0.3.0/xbridge_cli/utils/config_file/bridge_config.py` & `xbridge_cli-0.3.1/xbridge_cli/utils/config_file/bridge_config.py`

 * *Files identical despite different names*

### Comparing `xbridge_cli-0.3.0/xbridge_cli/utils/config_file/chain_config.py` & `xbridge_cli-0.3.1/xbridge_cli/utils/config_file/chain_config.py`

 * *Files identical despite different names*

### Comparing `xbridge_cli-0.3.0/xbridge_cli/utils/config_file/config_file.py` & `xbridge_cli-0.3.1/xbridge_cli/utils/config_file/config_file.py`

 * *Files identical despite different names*

### Comparing `xbridge_cli-0.3.0/xbridge_cli/utils/config_file/config_item.py` & `xbridge_cli-0.3.1/xbridge_cli/utils/config_file/config_item.py`

 * *Files identical despite different names*

### Comparing `xbridge_cli-0.3.0/xbridge_cli/utils/config_file/server_config.py` & `xbridge_cli-0.3.1/xbridge_cli/utils/config_file/server_config.py`

 * *Files identical despite different names*

### Comparing `xbridge_cli-0.3.0/xbridge_cli/utils/config_file/witness_config.py` & `xbridge_cli-0.3.1/xbridge_cli/utils/config_file/witness_config.py`

 * *Files identical despite different names*

### Comparing `xbridge_cli-0.3.0/xbridge_cli/utils/config_utils.py` & `xbridge_cli-0.3.1/xbridge_cli/utils/config_utils.py`

 * *Files identical despite different names*

### Comparing `xbridge_cli-0.3.0/xbridge_cli/utils/misc.py` & `xbridge_cli-0.3.1/xbridge_cli/utils/misc.py`

 * *Files identical despite different names*

### Comparing `xbridge_cli-0.3.0/xbridge_cli/utils/rippled_config.py` & `xbridge_cli-0.3.1/xbridge_cli/utils/rippled_config.py`

 * *Files identical despite different names*

### Comparing `xbridge_cli-0.3.0/xbridge_cli/utils/transaction.py` & `xbridge_cli-0.3.1/xbridge_cli/utils/transaction.py`

 * *Files identical despite different names*

### Comparing `xbridge_cli-0.3.0/xbridge_cli/utils/types.py` & `xbridge_cli-0.3.1/xbridge_cli/utils/types.py`

 * *Files identical despite different names*

### Comparing `xbridge_cli-0.3.0/setup.py` & `xbridge_cli-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
  'xrpl-py==1.9.0b1']
 
 entry_points = \
 {'console_scripts': ['xbridge-cli = xbridge_cli.main:main']}
 
 setup_kwargs = {
     'name': 'xbridge-cli',
-    'version': '0.3.0',
+    'version': '0.3.1',
     'description': 'A CLI that helps you set up an XRPL-XRPL bridge.',
     'long_description': "# xbridge-cli\n\n## Install\n\n```bash\npip install xbridge-cli\n```\n\nNOTE: if you're looking at the repo before it's published, this won't work. Instead, you'll do this:\n\n```bash\ngit clone https://github.com/xpring-eng/xbridge-cli.git\ncd xbridge-cli\n# install poetry\ncurl -sSL https://raw.githubusercontent.com/python-poetry/poetry/master/get-poetry.py | python -\npoetry install\npoetry shell\n```\n\nInstall rippled and the xbridge witness.\n\nrippled: https://xrpl.org/install-rippled.html\n\nwitness: https://github.com/seelabs/xbridge_witness\n\n## Get started\n\n```bash\nexport XCHAIN_CONFIG_DIR={filepath where you want your config files stored}\nexport RIPPLED_EXE={rippled exe filepath}\nexport WITNESSD_EXE={witnessd exe filepath}\n./scripts/tutorial.sh\n```\n\nTo stop the servers:\n\n```bash\nxbridge-cli server stop --all\n```\n\n## Use Commands\n\n```bash\nxbridge-cli --help\n```\n\nEach subcommand also has a `--help` flag, to tell you what fields you'll need.\n",
     'author': 'Mayukha Vadari',
     'author_email': 'mvadari@ripple.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/xpring-eng/xbridge-cli',
```

### Comparing `xbridge_cli-0.3.0/PKG-INFO` & `xbridge_cli-0.3.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xbridge-cli
-Version: 0.3.0
+Version: 0.3.1
 Summary: A CLI that helps you set up an XRPL-XRPL bridge.
 Home-page: https://github.com/xpring-eng/xbridge-cli
 License: MIT
 Keywords: xrp,xrpl,cryptocurrency
 Author: Mayukha Vadari
 Author-email: mvadari@ripple.com
 Requires-Python: >=3.7.1,<4.0.0
```

