# Comparing `tmp/brewblox_service-3.1.1.tar.gz` & `tmp/brewblox_service-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brewblox_service-3.1.1.tar", max compression
+gzip compressed data, was "brewblox_service-3.1.2.tar", max compression
```

## Comparing `brewblox_service-3.1.1.tar` & `brewblox_service-3.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    35140 2023-08-01 12:46:02.667931 brewblox_service-3.1.1/LICENSE.md
--rw-r--r--   0        0        0     3759 2023-08-01 12:46:02.667931 brewblox_service-3.1.1/README.md
--rw-r--r--   0        0        0     1147 2023-08-01 12:46:02.667931 brewblox_service-3.1.1/brewblox_service/__init__.py
--rw-r--r--   0        0        0     1503 2023-08-01 12:46:02.667931 brewblox_service-3.1.1/brewblox_service/cors.py
--rw-r--r--   0        0        0     9701 2023-08-01 12:46:02.667931 brewblox_service-3.1.1/brewblox_service/features.py
--rw-r--r--   0        0        0     1153 2023-08-01 12:46:02.667931 brewblox_service-3.1.1/brewblox_service/http.py
--rw-r--r--   0        0        0      362 2023-08-01 12:46:02.667931 brewblox_service-3.1.1/brewblox_service/models.py
--rw-r--r--   0        0        0    15460 2023-08-01 12:46:02.667931 brewblox_service-3.1.1/brewblox_service/mqtt.py
--rw-r--r--   0        0        0     5382 2023-08-01 12:46:02.667931 brewblox_service-3.1.1/brewblox_service/repeater.py
--rw-r--r--   0        0        0     5687 2023-08-01 12:46:02.667931 brewblox_service-3.1.1/brewblox_service/scheduler.py
--rw-r--r--   0        0        0     7358 2023-08-01 12:46:02.667931 brewblox_service-3.1.1/brewblox_service/service.py
--rw-r--r--   0        0        0     2573 2023-08-01 12:46:02.667931 brewblox_service-3.1.1/brewblox_service/testing.py
--rw-r--r--   0        0        0      729 2023-08-01 12:46:02.671931 brewblox_service-3.1.1/pyproject.toml
--rw-r--r--   0        0        0     4457 1970-01-01 00:00:00.000000 brewblox_service-3.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35140 2023-08-01 13:32:06.625320 brewblox_service-3.1.2/LICENSE.md
+-rw-r--r--   0        0        0     3759 2023-08-01 13:32:06.625320 brewblox_service-3.1.2/README.md
+-rw-r--r--   0        0        0     1147 2023-08-01 13:32:06.625320 brewblox_service-3.1.2/brewblox_service/__init__.py
+-rw-r--r--   0        0        0     1503 2023-08-01 13:32:06.625320 brewblox_service-3.1.2/brewblox_service/cors.py
+-rw-r--r--   0        0        0     9701 2023-08-01 13:32:06.625320 brewblox_service-3.1.2/brewblox_service/features.py
+-rw-r--r--   0        0        0     1153 2023-08-01 13:32:06.625320 brewblox_service-3.1.2/brewblox_service/http.py
+-rw-r--r--   0        0        0      362 2023-08-01 13:32:06.625320 brewblox_service-3.1.2/brewblox_service/models.py
+-rw-r--r--   0        0        0    15460 2023-08-01 13:32:06.625320 brewblox_service-3.1.2/brewblox_service/mqtt.py
+-rw-r--r--   0        0        0     5382 2023-08-01 13:32:06.625320 brewblox_service-3.1.2/brewblox_service/repeater.py
+-rw-r--r--   0        0        0     5687 2023-08-01 13:32:06.625320 brewblox_service-3.1.2/brewblox_service/scheduler.py
+-rw-r--r--   0        0        0     7358 2023-08-01 13:32:06.625320 brewblox_service-3.1.2/brewblox_service/service.py
+-rw-r--r--   0        0        0     2573 2023-08-01 13:32:06.625320 brewblox_service-3.1.2/brewblox_service/testing.py
+-rw-r--r--   0        0        0      729 2023-08-01 13:32:06.625320 brewblox_service-3.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4457 1970-01-01 00:00:00.000000 brewblox_service-3.1.2/PKG-INFO
```

### Comparing `brewblox_service-3.1.1/LICENSE.md` & `brewblox_service-3.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `brewblox_service-3.1.1/README.md` & `brewblox_service-3.1.2/README.md`

 * *Files identical despite different names*

### Comparing `brewblox_service-3.1.1/brewblox_service/__init__.py` & `brewblox_service-3.1.2/brewblox_service/__init__.py`

 * *Files identical despite different names*

### Comparing `brewblox_service-3.1.1/brewblox_service/cors.py` & `brewblox_service-3.1.2/brewblox_service/cors.py`

 * *Files identical despite different names*

### Comparing `brewblox_service-3.1.1/brewblox_service/features.py` & `brewblox_service-3.1.2/brewblox_service/features.py`

 * *Files identical despite different names*

### Comparing `brewblox_service-3.1.1/brewblox_service/http.py` & `brewblox_service-3.1.2/brewblox_service/http.py`

 * *Files identical despite different names*

### Comparing `brewblox_service-3.1.1/brewblox_service/mqtt.py` & `brewblox_service-3.1.2/brewblox_service/mqtt.py`

 * *Files identical despite different names*

### Comparing `brewblox_service-3.1.1/brewblox_service/repeater.py` & `brewblox_service-3.1.2/brewblox_service/repeater.py`

 * *Files identical despite different names*

### Comparing `brewblox_service-3.1.1/brewblox_service/scheduler.py` & `brewblox_service-3.1.2/brewblox_service/scheduler.py`

 * *Files identical despite different names*

### Comparing `brewblox_service-3.1.1/brewblox_service/service.py` & `brewblox_service-3.1.2/brewblox_service/service.py`

 * *Files identical despite different names*

### Comparing `brewblox_service-3.1.1/brewblox_service/testing.py` & `brewblox_service-3.1.2/brewblox_service/testing.py`

 * *Files identical despite different names*

### Comparing `brewblox_service-3.1.1/pyproject.toml` & `brewblox_service-3.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "brewblox-service"
-version = "3.1.1"
+version = "3.1.2"
 description = "Scaffolding for Brewblox backend services"
 authors = ["BrewPi <development@brewpi.com>"]
 license = "GPL-3.0"
 readme = "README.md"
 
 [tool.pyright]
 include = ["brewblox_service"]
```

### Comparing `brewblox_service-3.1.1/PKG-INFO` & `brewblox_service-3.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brewblox-service
-Version: 3.1.1
+Version: 3.1.2
 Summary: Scaffolding for Brewblox backend services
 License: GPL-3.0
 Author: BrewPi
 Author-email: development@brewpi.com
 Requires-Python: >=3.9,<4
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

