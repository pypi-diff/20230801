# Comparing `tmp/OpenGeodeWeb-Back-0.0.2.tar.gz` & `tmp/OpenGeodeWeb-Back-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OpenGeodeWeb-Back-0.0.2.tar", last modified: Mon Jul 31 10:09:32 2023, max compression
+gzip compressed data, was "OpenGeodeWeb-Back-0.0.3.tar", last modified: Tue Aug  1 08:06:09 2023, max compression
```

## Comparing `OpenGeodeWeb-Back-0.0.2.tar` & `OpenGeodeWeb-Back-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:09:32.232092 OpenGeodeWeb-Back-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-31 10:09:22.000000 OpenGeodeWeb-Back-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-31 10:09:32.232092 OpenGeodeWeb-Back-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-07-31 10:09:22.000000 OpenGeodeWeb-Back-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-31 10:09:22.000000 OpenGeodeWeb-Back-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 10:09:32.232092 OpenGeodeWeb-Back-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:09:32.228092 OpenGeodeWeb-Back-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:09:32.228092 OpenGeodeWeb-Back-0.0.2/src/OpenGeodeWeb-Back/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 10:09:22.000000 OpenGeodeWeb-Back-0.0.2/src/OpenGeodeWeb-Back/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7295 2023-07-31 10:09:22.000000 OpenGeodeWeb-Back-0.0.2/src/OpenGeodeWeb-Back/geode_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    14018 2023-07-31 10:09:22.000000 OpenGeodeWeb-Back-0.0.2/src/OpenGeodeWeb-Back/geode_objects.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:09:32.232092 OpenGeodeWeb-Back-0.0.2/src/OpenGeodeWeb_Back.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-31 10:09:32.000000 OpenGeodeWeb-Back-0.0.2/src/OpenGeodeWeb_Back.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-31 10:09:32.000000 OpenGeodeWeb-Back-0.0.2/src/OpenGeodeWeb_Back.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 10:09:32.000000 OpenGeodeWeb-Back-0.0.2/src/OpenGeodeWeb_Back.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-31 10:09:32.000000 OpenGeodeWeb-Back-0.0.2/src/OpenGeodeWeb_Back.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:06:09.466091 OpenGeodeWeb-Back-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-01 08:06:00.000000 OpenGeodeWeb-Back-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-08-01 08:06:09.466091 OpenGeodeWeb-Back-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-08-01 08:06:00.000000 OpenGeodeWeb-Back-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-08-01 08:06:00.000000 OpenGeodeWeb-Back-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 08:06:09.466091 OpenGeodeWeb-Back-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:06:09.462090 OpenGeodeWeb-Back-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:06:09.462090 OpenGeodeWeb-Back-0.0.3/src/OpenGeodeWeb_Back.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-08-01 08:06:09.000000 OpenGeodeWeb-Back-0.0.3/src/OpenGeodeWeb_Back.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-08-01 08:06:09.000000 OpenGeodeWeb-Back-0.0.3/src/OpenGeodeWeb_Back.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 08:06:09.000000 OpenGeodeWeb-Back-0.0.3/src/OpenGeodeWeb_Back.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-01 08:06:09.000000 OpenGeodeWeb-Back-0.0.3/src/OpenGeodeWeb_Back.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:06:09.466091 OpenGeodeWeb-Back-0.0.3/src/opengeodeweb_back/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 08:06:00.000000 OpenGeodeWeb-Back-0.0.3/src/opengeodeweb_back/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7295 2023-08-01 08:06:00.000000 OpenGeodeWeb-Back-0.0.3/src/opengeodeweb_back/geode_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14018 2023-08-01 08:06:00.000000 OpenGeodeWeb-Back-0.0.3/src/opengeodeweb_back/geode_objects.py
```

### Comparing `OpenGeodeWeb-Back-0.0.2/LICENSE` & `OpenGeodeWeb-Back-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `OpenGeodeWeb-Back-0.0.2/PKG-INFO` & `OpenGeodeWeb-Back-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenGeodeWeb-Back
-Version: 0.0.2
+Version: 0.0.3
 Summary: OpenGeodeWeb-Back is an open source framework that proposes handy python functions and wrappers for the OpenGeode ecosystem
 Author-email: Geode-solutions <contact@geode-solutions.com>
 Project-URL: Homepage, https://github.com/Geode-solutions/OpenGeodeWeb-Back
 Project-URL: Bug Tracker, https://github.com/Geode-solutions/OpenGeodeWeb-Back/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `OpenGeodeWeb-Back-0.0.2/README.md` & `OpenGeodeWeb-Back-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `OpenGeodeWeb-Back-0.0.2/pyproject.toml` & `OpenGeodeWeb-Back-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "OpenGeodeWeb-Back"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Geode-solutions", email="contact@geode-solutions.com" },
 ]
 description = "OpenGeodeWeb-Back is an open source framework that proposes handy python functions and wrappers for the OpenGeode ecosystem"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `OpenGeodeWeb-Back-0.0.2/src/OpenGeodeWeb-Back/geode_functions.py` & `OpenGeodeWeb-Back-0.0.3/src/opengeodeweb_back/geode_functions.py`

 * *Files identical despite different names*

### Comparing `OpenGeodeWeb-Back-0.0.2/src/OpenGeodeWeb-Back/geode_objects.py` & `OpenGeodeWeb-Back-0.0.3/src/opengeodeweb_back/geode_objects.py`

 * *Files identical despite different names*

### Comparing `OpenGeodeWeb-Back-0.0.2/src/OpenGeodeWeb_Back.egg-info/PKG-INFO` & `OpenGeodeWeb-Back-0.0.3/src/OpenGeodeWeb_Back.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenGeodeWeb-Back
-Version: 0.0.2
+Version: 0.0.3
 Summary: OpenGeodeWeb-Back is an open source framework that proposes handy python functions and wrappers for the OpenGeode ecosystem
 Author-email: Geode-solutions <contact@geode-solutions.com>
 Project-URL: Homepage, https://github.com/Geode-solutions/OpenGeodeWeb-Back
 Project-URL: Bug Tracker, https://github.com/Geode-solutions/OpenGeodeWeb-Back/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

