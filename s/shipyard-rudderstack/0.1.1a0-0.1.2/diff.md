# Comparing `tmp/shipyard_rudderstack-0.1.1a0.tar.gz` & `tmp/shipyard_rudderstack-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_rudderstack-0.1.1a0.tar", max compression
+gzip compressed data, was "shipyard_rudderstack-0.1.2.tar", max compression
```

## Comparing `shipyard_rudderstack-0.1.1a0.tar` & `shipyard_rudderstack-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      732 2023-06-26 14:41:35.509415 shipyard_rudderstack-0.1.1a0/README.md
--rw-r--r--   0        0        0      684 2023-07-28 00:30:07.883375 shipyard_rudderstack-0.1.1a0/pyproject.toml
--rw-r--r--   0        0        0       43 2023-06-26 16:14:24.727635 shipyard_rudderstack-0.1.1a0/shipyard_rudderstack/__init__.py
--rw-r--r--   0        0        0      279 2023-07-28 00:25:41.252773 shipyard_rudderstack-0.1.1a0/shipyard_rudderstack/cli/authtest.py
--rw-r--r--   0        0        0     2872 2023-07-28 00:27:21.204147 shipyard_rudderstack-0.1.1a0/shipyard_rudderstack/cli/trigger_sync_cli.py
--rw-r--r--   0        0        0     5677 2023-07-03 14:05:58.559154 shipyard_rudderstack-0.1.1a0/shipyard_rudderstack/rudderstack.py
--rw-r--r--   0        0        0     1316 1970-01-01 00:00:00.000000 shipyard_rudderstack-0.1.1a0/PKG-INFO
+-rw-r--r--   0        0        0      732 2023-06-26 14:41:35.509415 shipyard_rudderstack-0.1.2/README.md
+-rw-r--r--   0        0        0      682 2023-07-29 03:57:09.597324 shipyard_rudderstack-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       43 2023-06-26 16:14:24.727635 shipyard_rudderstack-0.1.2/shipyard_rudderstack/__init__.py
+-rw-r--r--   0        0        0      279 2023-07-28 00:25:41.252773 shipyard_rudderstack-0.1.2/shipyard_rudderstack/cli/authtest.py
+-rw-r--r--   0        0        0     2872 2023-07-29 03:56:44.241814 shipyard_rudderstack-0.1.2/shipyard_rudderstack/cli/trigger_sync_cli.py
+-rw-r--r--   0        0        0     5677 2023-07-03 14:05:58.559154 shipyard_rudderstack-0.1.2/shipyard_rudderstack/rudderstack.py
+-rw-r--r--   0        0        0     1314 1970-01-01 00:00:00.000000 shipyard_rudderstack-0.1.2/PKG-INFO
```

### Comparing `shipyard_rudderstack-0.1.1a0/README.md` & `shipyard_rudderstack-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `shipyard_rudderstack-0.1.1a0/pyproject.toml` & `shipyard_rudderstack-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shipyard-rudderstack"
-version = "0.1.1a0"
+version = "0.1.2"
 description = "A local client for connecting and working with Rudderstack"
 authors = ["JR <johnathan.rodriguez@shipyardapp.com>", "wrp801 <wespoulsen@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "shipyard_rudderstack" }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `shipyard_rudderstack-0.1.1a0/shipyard_rudderstack/cli/trigger_sync_cli.py` & `shipyard_rudderstack-0.1.2/shipyard_rudderstack/cli/trigger_sync_cli.py`

 * *Files identical despite different names*

### Comparing `shipyard_rudderstack-0.1.1a0/shipyard_rudderstack/rudderstack.py` & `shipyard_rudderstack-0.1.2/shipyard_rudderstack/rudderstack.py`

 * *Files identical despite different names*

### Comparing `shipyard_rudderstack-0.1.1a0/PKG-INFO` & `shipyard_rudderstack-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipyard-rudderstack
-Version: 0.1.1a0
+Version: 0.1.2
 Summary: A local client for connecting and working with Rudderstack
 Author: JR
 Author-email: johnathan.rodriguez@shipyardapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

