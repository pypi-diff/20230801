# Comparing `tmp/plemmy-0.3.3.tar.gz` & `tmp/plemmy-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plemmy-0.3.3.tar", last modified: Sat Jul 22 19:39:57 2023, max compression
+gzip compressed data, was "plemmy-0.3.4.tar", last modified: Tue Aug  1 03:32:53 2023, max compression
```

## Comparing `plemmy-0.3.3.tar` & `plemmy-0.3.4.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 tjkessler   (501) staff       (20)        0 2023-07-22 19:39:57.227370 plemmy-0.3.3/
--rw-r--r--   0 tjkessler   (501) staff       (20)    11367 2023-07-20 23:46:22.000000 plemmy-0.3.3/LICENSE
--rw-r--r--   0 tjkessler   (501) staff       (20)     2704 2023-07-22 19:39:57.227148 plemmy-0.3.3/PKG-INFO
--rw-r--r--   0 tjkessler   (501) staff       (20)     2418 2023-07-22 19:39:18.000000 plemmy-0.3.3/README.md
-drwxr-xr-x   0 tjkessler   (501) staff       (20)        0 2023-07-22 19:39:57.225731 plemmy-0.3.3/plemmy/
--rw-r--r--   0 tjkessler   (501) staff       (20)      209 2023-07-20 23:46:22.000000 plemmy-0.3.3/plemmy/__init__.py
--rw-r--r--   0 tjkessler   (501) staff       (20)    71480 2023-07-20 23:46:22.000000 plemmy-0.3.3/plemmy/lemmyhttp.py
--rw-r--r--   0 tjkessler   (501) staff       (20)    13987 2023-07-20 23:46:22.000000 plemmy-0.3.3/plemmy/objects.py
--rw-r--r--   0 tjkessler   (501) staff       (20)    19231 2023-07-20 23:46:22.000000 plemmy-0.3.3/plemmy/responses.py
--rw-r--r--   0 tjkessler   (501) staff       (20)     2907 2023-07-22 19:36:24.000000 plemmy-0.3.3/plemmy/utils.py
--rw-r--r--   0 tjkessler   (501) staff       (20)      120 2023-07-22 19:38:24.000000 plemmy-0.3.3/plemmy/version.py
--rw-r--r--   0 tjkessler   (501) staff       (20)    16980 2023-07-20 23:46:22.000000 plemmy-0.3.3/plemmy/views.py
-drwxr-xr-x   0 tjkessler   (501) staff       (20)        0 2023-07-22 19:39:57.226833 plemmy-0.3.3/plemmy.egg-info/
--rw-r--r--   0 tjkessler   (501) staff       (20)     2704 2023-07-22 19:39:57.000000 plemmy-0.3.3/plemmy.egg-info/PKG-INFO
--rw-r--r--   0 tjkessler   (501) staff       (20)      331 2023-07-22 19:39:57.000000 plemmy-0.3.3/plemmy.egg-info/SOURCES.txt
--rw-r--r--   0 tjkessler   (501) staff       (20)        1 2023-07-22 19:39:57.000000 plemmy-0.3.3/plemmy.egg-info/dependency_links.txt
--rw-r--r--   0 tjkessler   (501) staff       (20)        1 2023-07-22 19:39:57.000000 plemmy-0.3.3/plemmy.egg-info/not-zip-safe
--rw-r--r--   0 tjkessler   (501) staff       (20)       17 2023-07-22 19:39:57.000000 plemmy-0.3.3/plemmy.egg-info/requires.txt
--rw-r--r--   0 tjkessler   (501) staff       (20)        7 2023-07-22 19:39:57.000000 plemmy-0.3.3/plemmy.egg-info/top_level.txt
--rw-r--r--   0 tjkessler   (501) staff       (20)       38 2023-07-22 19:39:57.227424 plemmy-0.3.3/setup.cfg
--rw-r--r--   0 tjkessler   (501) staff       (20)      878 2023-07-20 23:46:22.000000 plemmy-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 03:32:53.234934 plemmy-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11367 2023-08-01 03:32:43.000000 plemmy-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-08-01 03:32:53.234934 plemmy-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-08-01 03:32:43.000000 plemmy-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 03:32:53.230934 plemmy-0.3.4/plemmy/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-08-01 03:32:43.000000 plemmy-0.3.4/plemmy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71480 2023-08-01 03:32:43.000000 plemmy-0.3.4/plemmy/lemmyhttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13987 2023-08-01 03:32:43.000000 plemmy-0.3.4/plemmy/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19231 2023-08-01 03:32:43.000000 plemmy-0.3.4/plemmy/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-08-01 03:32:43.000000 plemmy-0.3.4/plemmy/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-08-01 03:32:43.000000 plemmy-0.3.4/plemmy/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16980 2023-08-01 03:32:43.000000 plemmy-0.3.4/plemmy/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 03:32:53.234934 plemmy-0.3.4/plemmy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-08-01 03:32:53.000000 plemmy-0.3.4/plemmy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-08-01 03:32:53.000000 plemmy-0.3.4/plemmy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 03:32:53.000000 plemmy-0.3.4/plemmy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-01 03:32:53.000000 plemmy-0.3.4/plemmy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-01 03:32:53.000000 plemmy-0.3.4/plemmy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-08-01 03:32:43.000000 plemmy-0.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 03:32:53.234934 plemmy-0.3.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 03:32:53.234934 plemmy-0.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-08-01 03:32:43.000000 plemmy-0.3.4/tests/test_import.py
```

### Comparing `plemmy-0.3.3/LICENSE` & `plemmy-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `plemmy-0.3.3/PKG-INFO` & `plemmy-0.3.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 Metadata-Version: 2.1
 Name: plemmy
-Version: 0.3.3
-Summary: Python API for LemmyHttp
-Home-page: https://github.com/tjkessler/plemmy
-Author: Travis Kessler
-Author-email: travis.j.kessler@gmail.com
-License: Apache License 2.0
+Version: 0.3.4
+Summary: A Python package for accessing the LemmyHttp API
+Author-email: Travis Kessler <travis.j.kessler@gmail.com>
+Project-URL: Homepage, https://github.com/tjkessler/plemmy
+Project-URL: Bug Tracker, https://github.com/tjkessler/plemmy/issues
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Plemmy: a Python package for accessing the Lemmy API
 
 <img src="https://github.com/tjkessler/plemmy/blob/main/img/plemmy.png" alt="drawing" width="325"/>
 
@@ -24,21 +27,21 @@
 ## Installation ##
 
 For the most up-to-date version of Plemmy, clone and install from the repository:
 
 ```
 git clone https://github.com/tjkessler/plemmy
 cd plemmy
-python setup.py install
+python -m pip install .
 ```
 
-A PyPI repository is periodically updated:
+A PyPI repository is updated whenever a new version is available:
 
 ```
-pip install plemmy
+python -m pip install plemmy
 ```
 
 ## Basic usage ##
 
 Interact with a Lemmy instance using the _LemmyHttp_ object:
 
 ```python
```

### Comparing `plemmy-0.3.3/README.md` & `plemmy-0.3.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -13,21 +13,21 @@
 ## Installation ##
 
 For the most up-to-date version of Plemmy, clone and install from the repository:
 
 ```
 git clone https://github.com/tjkessler/plemmy
 cd plemmy
-python setup.py install
+python -m pip install .
 ```
 
-A PyPI repository is periodically updated:
+A PyPI repository is updated whenever a new version is available:
 
 ```
-pip install plemmy
+python -m pip install plemmy
 ```
 
 ## Basic usage ##
 
 Interact with a Lemmy instance using the _LemmyHttp_ object:
 
 ```python
```

### Comparing `plemmy-0.3.3/plemmy/lemmyhttp.py` & `plemmy-0.3.4/plemmy/lemmyhttp.py`

 * *Files identical despite different names*

### Comparing `plemmy-0.3.3/plemmy/objects.py` & `plemmy-0.3.4/plemmy/objects.py`

 * *Files identical despite different names*

### Comparing `plemmy-0.3.3/plemmy/responses.py` & `plemmy-0.3.4/plemmy/responses.py`

 * *Files identical despite different names*

### Comparing `plemmy-0.3.3/plemmy/utils.py` & `plemmy-0.3.4/plemmy/utils.py`

 * *Files identical despite different names*

### Comparing `plemmy-0.3.3/plemmy/views.py` & `plemmy-0.3.4/plemmy/views.py`

 * *Files identical despite different names*

### Comparing `plemmy-0.3.3/plemmy.egg-info/PKG-INFO` & `plemmy-0.3.4/plemmy.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 Metadata-Version: 2.1
 Name: plemmy
-Version: 0.3.3
-Summary: Python API for LemmyHttp
-Home-page: https://github.com/tjkessler/plemmy
-Author: Travis Kessler
-Author-email: travis.j.kessler@gmail.com
-License: Apache License 2.0
+Version: 0.3.4
+Summary: A Python package for accessing the LemmyHttp API
+Author-email: Travis Kessler <travis.j.kessler@gmail.com>
+Project-URL: Homepage, https://github.com/tjkessler/plemmy
+Project-URL: Bug Tracker, https://github.com/tjkessler/plemmy/issues
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Plemmy: a Python package for accessing the Lemmy API
 
 <img src="https://github.com/tjkessler/plemmy/blob/main/img/plemmy.png" alt="drawing" width="325"/>
 
@@ -24,21 +27,21 @@
 ## Installation ##
 
 For the most up-to-date version of Plemmy, clone and install from the repository:
 
 ```
 git clone https://github.com/tjkessler/plemmy
 cd plemmy
-python setup.py install
+python -m pip install .
 ```
 
-A PyPI repository is periodically updated:
+A PyPI repository is updated whenever a new version is available:
 
 ```
-pip install plemmy
+python -m pip install plemmy
 ```
 
 ## Basic usage ##
 
 Interact with a Lemmy instance using the _LemmyHttp_ object:
 
 ```python
```

