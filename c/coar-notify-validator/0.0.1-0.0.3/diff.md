# Comparing `tmp/coar_notify_validator-0.0.1.tar.gz` & `tmp/coar_notify_validator-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coar_notify_validator-0.0.1.tar", last modified: Tue Aug  1 09:31:24 2023, max compression
+gzip compressed data, was "coar_notify_validator-0.0.3.tar", last modified: Tue Aug  1 09:51:16 2023, max compression
```

## Comparing `coar_notify_validator-0.0.1.tar` & `coar_notify_validator-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:31:24.208495 coar_notify_validator-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-01 09:31:10.000000 coar_notify_validator-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-08-01 09:31:24.208495 coar_notify_validator-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-08-01 09:31:10.000000 coar_notify_validator-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:31:24.204494 coar_notify_validator-0.0.1/coar_notify_validator/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-01 09:31:10.000000 coar_notify_validator-0.0.1/coar_notify_validator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-01 09:31:10.000000 coar_notify_validator-0.0.1/coar_notify_validator/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-08-01 09:31:10.000000 coar_notify_validator-0.0.1/coar_notify_validator/results_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:31:24.208495 coar_notify_validator-0.0.1/coar_notify_validator/shape_files/
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-08-01 09:31:10.000000 coar_notify_validator-0.0.1/coar_notify_validator/shape_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-08-01 09:31:10.000000 coar_notify_validator-0.0.1/coar_notify_validator/shape_files/read_shape_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-08-01 09:31:10.000000 coar_notify_validator-0.0.1/coar_notify_validator/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:31:24.208495 coar_notify_validator-0.0.1/coar_notify_validator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-08-01 09:31:24.000000 coar_notify_validator-0.0.1/coar_notify_validator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-08-01 09:31:24.000000 coar_notify_validator-0.0.1/coar_notify_validator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 09:31:24.000000 coar_notify_validator-0.0.1/coar_notify_validator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-01 09:31:24.000000 coar_notify_validator-0.0.1/coar_notify_validator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-01 09:31:24.000000 coar_notify_validator-0.0.1/coar_notify_validator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 09:31:24.208495 coar_notify_validator-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-08-01 09:31:10.000000 coar_notify_validator-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:51:16.474932 coar_notify_validator-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-01 09:51:06.000000 coar_notify_validator-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-01 09:51:06.000000 coar_notify_validator-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-08-01 09:51:16.474932 coar_notify_validator-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-08-01 09:51:06.000000 coar_notify_validator-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:51:16.474932 coar_notify_validator-0.0.3/coar_notify_validator/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-01 09:51:06.000000 coar_notify_validator-0.0.3/coar_notify_validator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-01 09:51:06.000000 coar_notify_validator-0.0.3/coar_notify_validator/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-08-01 09:51:06.000000 coar_notify_validator-0.0.3/coar_notify_validator/results_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:51:16.474932 coar_notify_validator-0.0.3/coar_notify_validator/shape_files/
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-08-01 09:51:06.000000 coar_notify_validator-0.0.3/coar_notify_validator/shape_files/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:51:16.474932 coar_notify_validator-0.0.3/coar_notify_validator/shape_files/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-08-01 09:51:06.000000 coar_notify_validator-0.0.3/coar_notify_validator/shape_files/data/CoarActor.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-08-01 09:51:06.000000 coar_notify_validator-0.0.3/coar_notify_validator/shape_files/data/accept-review-shape.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-08-01 09:51:06.000000 coar_notify_validator-0.0.3/coar_notify_validator/shape_files/data/acknowledge-and-reject-shape.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-08-01 09:51:06.000000 coar_notify_validator-0.0.3/coar_notify_validator/shape_files/data/acknowledge-and-tentative-accept-shape.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-08-01 09:51:06.000000 coar_notify_validator-0.0.3/coar_notify_validator/shape_files/data/acknowledge-and-tentative-reject-shape.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-08-01 09:51:06.000000 coar_notify_validator-0.0.3/coar_notify_validator/shape_files/data/announce-endorse-shape.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-08-01 09:51:06.000000 coar_notify_validator-0.0.3/coar_notify_validator/shape_files/data/announce-ingest-shape.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-08-01 09:51:06.000000 coar_notify_validator-0.0.3/coar_notify_validator/shape_files/data/announce-relationship-shape.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-08-01 09:51:06.000000 coar_notify_validator-0.0.3/coar_notify_validator/shape_files/data/announce-review-shape.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-08-01 09:51:06.000000 coar_notify_validator-0.0.3/coar_notify_validator/shape_files/data/announce-shape.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-08-01 09:51:06.000000 coar_notify_validator-0.0.3/coar_notify_validator/shape_files/data/offer-endorse-shape.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-08-01 09:51:06.000000 coar_notify_validator-0.0.3/coar_notify_validator/shape_files/data/offer-ingest-shape.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-08-01 09:51:06.000000 coar_notify_validator-0.0.3/coar_notify_validator/shape_files/data/offer-review-shape.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-08-01 09:51:06.000000 coar_notify_validator-0.0.3/coar_notify_validator/shape_files/data/scen_2-1.shacl.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-08-01 09:51:06.000000 coar_notify_validator-0.0.3/coar_notify_validator/shape_files/data/scen_7-1.shacl.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-08-01 09:51:06.000000 coar_notify_validator-0.0.3/coar_notify_validator/shape_files/data/test-announce-endorse-shape.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-08-01 09:51:06.000000 coar_notify_validator-0.0.3/coar_notify_validator/shape_files/data/undo-shape.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-08-01 09:51:06.000000 coar_notify_validator-0.0.3/coar_notify_validator/shape_files/read_shape_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-08-01 09:51:06.000000 coar_notify_validator-0.0.3/coar_notify_validator/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:51:16.474932 coar_notify_validator-0.0.3/coar_notify_validator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-08-01 09:51:16.000000 coar_notify_validator-0.0.3/coar_notify_validator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-08-01 09:51:16.000000 coar_notify_validator-0.0.3/coar_notify_validator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 09:51:16.000000 coar_notify_validator-0.0.3/coar_notify_validator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-01 09:51:16.000000 coar_notify_validator-0.0.3/coar_notify_validator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-01 09:51:16.000000 coar_notify_validator-0.0.3/coar_notify_validator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 09:51:16.474932 coar_notify_validator-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-08-01 09:51:06.000000 coar_notify_validator-0.0.3/setup.py
```

### Comparing `coar_notify_validator-0.0.1/LICENSE` & `coar_notify_validator-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `coar_notify_validator-0.0.1/PKG-INFO` & `coar_notify_validator-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coar_notify_validator
-Version: 0.0.1
+Version: 0.0.3
 Summary: Utility for validating COAR Notify payloads.
 Home-page: https://github.com/seanwiseman/coar-notify-validator.git
 Maintainer: Sean Wiseman
 Maintainer-email: seanwiseman2012@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `coar_notify_validator-0.0.1/README.md` & `coar_notify_validator-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `coar_notify_validator-0.0.1/coar_notify_validator/results_parser.py` & `coar_notify_validator-0.0.3/coar_notify_validator/results_parser.py`

 * *Files identical despite different names*

### Comparing `coar_notify_validator-0.0.1/coar_notify_validator/shape_files/__init__.py` & `coar_notify_validator-0.0.3/coar_notify_validator/shape_files/__init__.py`

 * *Files identical despite different names*

### Comparing `coar_notify_validator-0.0.1/coar_notify_validator/validate.py` & `coar_notify_validator-0.0.3/coar_notify_validator/validate.py`

 * *Files identical despite different names*

### Comparing `coar_notify_validator-0.0.1/coar_notify_validator.egg-info/PKG-INFO` & `coar_notify_validator-0.0.3/coar_notify_validator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coar-notify-validator
-Version: 0.0.1
+Version: 0.0.3
 Summary: Utility for validating COAR Notify payloads.
 Home-page: https://github.com/seanwiseman/coar-notify-validator.git
 Maintainer: Sean Wiseman
 Maintainer-email: seanwiseman2012@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `coar_notify_validator-0.0.1/setup.py` & `coar_notify_validator-0.0.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,17 +9,14 @@
     long_description_content_type='text/markdown',
     long_description=open('README.md').read(),
     packages=[
         "coar_notify_validator",
         "coar_notify_validator.shape_files",
     ],
     include_package_data=True,
-    package_data={
-        "shape_files": ["coar_notify_validator/shape_files/data/*.ttl"],
-    },
     install_requires=[
         "kglab == 0.6.6",
         "rdflib == 6.3.2",
         "pyshacl == 0.23.0",
     ],
     license="MIT",
     url="https://github.com/seanwiseman/coar-notify-validator.git",
```

