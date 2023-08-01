# Comparing `tmp/smplkit-0.0.2.tar.gz` & `tmp/smplkit-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smplkit-0.0.2.tar", last modified: Thu Jul 20 15:51:37 2023, max compression
+gzip compressed data, was "smplkit-0.0.3.tar", last modified: Tue Aug  1 06:55:06 2023, max compression
```

## Comparing `smplkit-0.0.2.tar` & `smplkit-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:51:37.447269 smplkit-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-20 15:51:25.000000 smplkit-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-07-20 15:51:37.447269 smplkit-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-07-20 15:51:25.000000 smplkit-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:51:37.447269 smplkit-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-07-20 15:51:25.000000 smplkit-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:51:37.447269 smplkit-0.0.2/smplkit/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-20 15:51:25.000000 smplkit-0.0.2/smplkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-20 15:51:26.000000 smplkit-0.0.2/smplkit/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29389 2023-07-20 15:51:25.000000 smplkit-0.0.2/smplkit/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13836 2023-07-20 15:51:25.000000 smplkit-0.0.2/smplkit/lbs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-07-20 15:51:25.000000 smplkit-0.0.2/smplkit/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    20282 2023-07-20 15:51:25.000000 smplkit-0.0.2/smplkit/params.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:51:37.447269 smplkit-0.0.2/smplkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-07-20 15:51:37.000000 smplkit-0.0.2/smplkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-20 15:51:37.000000 smplkit-0.0.2/smplkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:51:37.000000 smplkit-0.0.2/smplkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-20 15:51:37.000000 smplkit-0.0.2/smplkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-20 15:51:37.000000 smplkit-0.0.2/smplkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:51:37.447269 smplkit-0.0.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-20 15:51:25.000000 smplkit-0.0.2/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:55:06.892112 smplkit-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-01 06:54:56.000000 smplkit-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6409 2023-08-01 06:55:06.888112 smplkit-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-08-01 06:54:56.000000 smplkit-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 06:55:06.892112 smplkit-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-08-01 06:54:56.000000 smplkit-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:55:06.888112 smplkit-0.0.3/smplkit/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-08-01 06:54:56.000000 smplkit-0.0.3/smplkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-01 06:54:56.000000 smplkit-0.0.3/smplkit/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26537 2023-08-01 06:54:56.000000 smplkit-0.0.3/smplkit/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29389 2023-08-01 06:54:56.000000 smplkit-0.0.3/smplkit/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13836 2023-08-01 06:54:56.000000 smplkit-0.0.3/smplkit/lbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-08-01 06:54:56.000000 smplkit-0.0.3/smplkit/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20282 2023-08-01 06:54:56.000000 smplkit-0.0.3/smplkit/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10040 2023-08-01 06:54:56.000000 smplkit-0.0.3/smplkit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:55:06.888112 smplkit-0.0.3/smplkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6409 2023-08-01 06:55:06.000000 smplkit-0.0.3/smplkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-08-01 06:55:06.000000 smplkit-0.0.3/smplkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 06:55:06.000000 smplkit-0.0.3/smplkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-01 06:55:06.000000 smplkit-0.0.3/smplkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-01 06:55:06.000000 smplkit-0.0.3/smplkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:55:06.888112 smplkit-0.0.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-08-01 06:54:56.000000 smplkit-0.0.3/test/test.py
```

### Comparing `smplkit-0.0.2/LICENSE` & `smplkit-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `smplkit-0.0.2/setup.py` & `smplkit-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 REQUIRES_PYTHON = '>=3.6.0'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'numpy>=1.19.0',
     'einops>=0.3.0',
     'torch>=1.6.0',
+    'pytorch3d>=0.6.0',
+    'easydict>=1.9',
 ]
 
 # The rest you shouldn't have to touch too much :)
 # ------------------------------------------------
 # Except, perhaps the License and Trove Classifiers!
 # If you do change the License, remember to change the Trove Classifier for that!
```

### Comparing `smplkit-0.0.2/smplkit/layers.py` & `smplkit-0.0.3/smplkit/layers.py`

 * *Files identical despite different names*

### Comparing `smplkit-0.0.2/smplkit/lbs.py` & `smplkit-0.0.3/smplkit/lbs.py`

 * *Files identical despite different names*

### Comparing `smplkit-0.0.2/smplkit/misc.py` & `smplkit-0.0.3/smplkit/misc.py`

 * *Files identical despite different names*

### Comparing `smplkit-0.0.2/smplkit/params.py` & `smplkit-0.0.3/smplkit/params.py`

 * *Files identical despite different names*

