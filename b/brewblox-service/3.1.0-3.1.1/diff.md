# Comparing `tmp/brewblox_service-3.1.0.tar.gz` & `tmp/brewblox_service-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brewblox_service-3.1.0.tar", max compression
+gzip compressed data, was "brewblox_service-3.1.1.tar", max compression
```

## Comparing `brewblox_service-3.1.0.tar` & `brewblox_service-3.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    35140 2023-08-01 10:50:26.727620 brewblox_service-3.1.0/LICENSE.md
--rw-r--r--   0        0        0     3759 2023-08-01 10:50:26.727620 brewblox_service-3.1.0/README.md
--rw-r--r--   0        0        0     1147 2023-08-01 10:50:26.727620 brewblox_service-3.1.0/brewblox_service/__init__.py
--rw-r--r--   0        0        0     1503 2023-08-01 10:50:26.727620 brewblox_service-3.1.0/brewblox_service/cors.py
--rw-r--r--   0        0        0     9701 2023-08-01 10:50:26.727620 brewblox_service-3.1.0/brewblox_service/features.py
--rw-r--r--   0        0        0     1153 2023-08-01 10:50:26.727620 brewblox_service-3.1.0/brewblox_service/http.py
--rw-r--r--   0        0        0      362 2023-08-01 10:50:26.727620 brewblox_service-3.1.0/brewblox_service/models.py
--rw-r--r--   0        0        0    15460 2023-08-01 10:50:26.727620 brewblox_service-3.1.0/brewblox_service/mqtt.py
--rw-r--r--   0        0        0     5382 2023-08-01 10:50:26.727620 brewblox_service-3.1.0/brewblox_service/repeater.py
--rw-r--r--   0        0        0     5687 2023-08-01 10:50:26.727620 brewblox_service-3.1.0/brewblox_service/scheduler.py
--rw-r--r--   0        0        0     7358 2023-08-01 10:50:26.727620 brewblox_service-3.1.0/brewblox_service/service.py
--rw-r--r--   0        0        0     2573 2023-08-01 10:50:26.727620 brewblox_service-3.1.0/brewblox_service/testing.py
--rw-r--r--   0        0        0      681 2023-08-01 10:50:26.727620 brewblox_service-3.1.0/pyproject.toml
--rw-r--r--   0        0        0     4418 1970-01-01 00:00:00.000000 brewblox_service-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35140 2023-08-01 12:46:02.667931 brewblox_service-3.1.1/LICENSE.md
+-rw-r--r--   0        0        0     3759 2023-08-01 12:46:02.667931 brewblox_service-3.1.1/README.md
+-rw-r--r--   0        0        0     1147 2023-08-01 12:46:02.667931 brewblox_service-3.1.1/brewblox_service/__init__.py
+-rw-r--r--   0        0        0     1503 2023-08-01 12:46:02.667931 brewblox_service-3.1.1/brewblox_service/cors.py
+-rw-r--r--   0        0        0     9701 2023-08-01 12:46:02.667931 brewblox_service-3.1.1/brewblox_service/features.py
+-rw-r--r--   0        0        0     1153 2023-08-01 12:46:02.667931 brewblox_service-3.1.1/brewblox_service/http.py
+-rw-r--r--   0        0        0      362 2023-08-01 12:46:02.667931 brewblox_service-3.1.1/brewblox_service/models.py
+-rw-r--r--   0        0        0    15460 2023-08-01 12:46:02.667931 brewblox_service-3.1.1/brewblox_service/mqtt.py
+-rw-r--r--   0        0        0     5382 2023-08-01 12:46:02.667931 brewblox_service-3.1.1/brewblox_service/repeater.py
+-rw-r--r--   0        0        0     5687 2023-08-01 12:46:02.667931 brewblox_service-3.1.1/brewblox_service/scheduler.py
+-rw-r--r--   0        0        0     7358 2023-08-01 12:46:02.667931 brewblox_service-3.1.1/brewblox_service/service.py
+-rw-r--r--   0        0        0     2573 2023-08-01 12:46:02.667931 brewblox_service-3.1.1/brewblox_service/testing.py
+-rw-r--r--   0        0        0      729 2023-08-01 12:46:02.671931 brewblox_service-3.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4457 1970-01-01 00:00:00.000000 brewblox_service-3.1.1/PKG-INFO
```

### Comparing `brewblox_service-3.1.0/LICENSE.md` & `brewblox_service-3.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `brewblox_service-3.1.0/README.md` & `brewblox_service-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `brewblox_service-3.1.0/brewblox_service/__init__.py` & `brewblox_service-3.1.1/brewblox_service/__init__.py`

 * *Files identical despite different names*

### Comparing `brewblox_service-3.1.0/brewblox_service/cors.py` & `brewblox_service-3.1.1/brewblox_service/cors.py`

 * *Files identical despite different names*

### Comparing `brewblox_service-3.1.0/brewblox_service/features.py` & `brewblox_service-3.1.1/brewblox_service/features.py`

 * *Files identical despite different names*

### Comparing `brewblox_service-3.1.0/brewblox_service/http.py` & `brewblox_service-3.1.1/brewblox_service/http.py`

 * *Files identical despite different names*

### Comparing `brewblox_service-3.1.0/brewblox_service/mqtt.py` & `brewblox_service-3.1.1/brewblox_service/mqtt.py`

 * *Files identical despite different names*

### Comparing `brewblox_service-3.1.0/brewblox_service/repeater.py` & `brewblox_service-3.1.1/brewblox_service/repeater.py`

 * *Files identical despite different names*

### Comparing `brewblox_service-3.1.0/brewblox_service/scheduler.py` & `brewblox_service-3.1.1/brewblox_service/scheduler.py`

 * *Files identical despite different names*

### Comparing `brewblox_service-3.1.0/brewblox_service/service.py` & `brewblox_service-3.1.1/brewblox_service/service.py`

 * *Files identical despite different names*

### Comparing `brewblox_service-3.1.0/brewblox_service/testing.py` & `brewblox_service-3.1.1/brewblox_service/testing.py`

 * *Files identical despite different names*

### Comparing `brewblox_service-3.1.0/PKG-INFO` & `brewblox_service-3.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: brewblox-service
-Version: 3.1.0
+Version: 3.1.1
 Summary: Scaffolding for Brewblox backend services
 License: GPL-3.0
 Author: BrewPi
 Author-email: development@brewpi.com
 Requires-Python: >=3.9,<4
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (==3.*)
 Requires-Dist: aiohttp-pydantic (==1.*)
 Requires-Dist: aiomqtt (==1.*)
+Requires-Dist: cryptography (==40.0.1)
 Requires-Dist: pydantic (==1.*)
 Description-Content-Type: text/markdown
 
 # Scaffolding for Brewblox service applications
 
 In order to reduce code duplication between services, generic functionality is implemented here.
```

