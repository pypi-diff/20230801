# Comparing `tmp/shaped_target_clickhouse-0.0.4.tar.gz` & `tmp/shaped_target_clickhouse-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shaped_target_clickhouse-0.0.4.tar", max compression
+gzip compressed data, was "shaped_target_clickhouse-0.0.5.tar", max compression
```

## Comparing `shaped_target_clickhouse-0.0.4.tar` & `shaped_target_clickhouse-0.0.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11337 2023-07-31 20:27:09.923095 shaped_target_clickhouse-0.0.4/LICENSE
--rw-r--r--   0        0        0     4397 2023-07-31 20:27:09.923095 shaped_target_clickhouse-0.0.4/README.md
--rw-r--r--   0        0        0     1413 2023-07-31 20:27:09.923095 shaped_target_clickhouse-0.0.4/pyproject.toml
--rw-r--r--   0        0        0       29 2023-07-31 20:27:09.923095 shaped_target_clickhouse-0.0.4/target_clickhouse/__init__.py
--rw-r--r--   0        0        0     5422 2023-07-31 20:27:09.923095 shaped_target_clickhouse-0.0.4/target_clickhouse/sinks.py
--rw-r--r--   0        0        0      775 2023-07-31 20:27:09.923095 shaped_target_clickhouse-0.0.4/target_clickhouse/target.py
--rw-r--r--   0        0        0     5192 1970-01-01 00:00:00.000000 shaped_target_clickhouse-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    11337 2023-08-01 17:47:34.294683 shaped_target_clickhouse-0.0.5/LICENSE
+-rw-r--r--   0        0        0     4397 2023-08-01 17:47:34.294683 shaped_target_clickhouse-0.0.5/README.md
+-rw-r--r--   0        0        0     1413 2023-08-01 17:47:34.298683 shaped_target_clickhouse-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0       29 2023-08-01 17:47:34.298683 shaped_target_clickhouse-0.0.5/target_clickhouse/__init__.py
+-rw-r--r--   0        0        0     5422 2023-08-01 17:47:34.298683 shaped_target_clickhouse-0.0.5/target_clickhouse/sinks.py
+-rw-r--r--   0        0        0      849 2023-08-01 17:47:34.298683 shaped_target_clickhouse-0.0.5/target_clickhouse/target.py
+-rw-r--r--   0        0        0     5192 1970-01-01 00:00:00.000000 shaped_target_clickhouse-0.0.5/PKG-INFO
```

### Comparing `shaped_target_clickhouse-0.0.4/LICENSE` & `shaped_target_clickhouse-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `shaped_target_clickhouse-0.0.4/README.md` & `shaped_target_clickhouse-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `shaped_target_clickhouse-0.0.4/pyproject.toml` & `shaped_target_clickhouse-0.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shaped-target-clickhouse"
-version = "0.0.4"
+version = "0.0.5"
 description = "`target-clickhouse` is a Singer target for clickhouse, built with the Meltano Singer SDK."
 readme = "README.md"
 authors = ["Ben Theunissen"]
 keywords = [
     "ELT",
     "clickhouse",
 ]
```

### Comparing `shaped_target_clickhouse-0.0.4/target_clickhouse/sinks.py` & `shaped_target_clickhouse-0.0.5/target_clickhouse/sinks.py`

 * *Files identical despite different names*

### Comparing `shaped_target_clickhouse-0.0.4/PKG-INFO` & `shaped_target_clickhouse-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shaped-target-clickhouse
-Version: 0.0.4
+Version: 0.0.5
 Summary: `target-clickhouse` is a Singer target for clickhouse, built with the Meltano Singer SDK.
 License: Apache-2.0
 Keywords: ELT,clickhouse
 Author: Ben Theunissen
 Requires-Python: >=3.7.1,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

