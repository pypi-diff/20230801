# Comparing `tmp/xe-admix-1.0.10.tar.gz` & `tmp/xe-admix-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xe-admix-1.0.10.tar", last modified: Tue Aug  1 08:19:39 2023, max compression
+gzip compressed data, was "xe-admix-1.0.9.tar", last modified: Sun May 21 18:04:49 2023, max compression
```

## Comparing `xe-admix-1.0.10.tar` & `xe-admix-1.0.9.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:19:39.652194 xe-admix-1.0.10/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-08-01 08:19:32.000000 xe-admix-1.0.10/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-08-01 08:19:32.000000 xe-admix-1.0.10/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-08-01 08:19:32.000000 xe-admix-1.0.10/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-08-01 08:19:32.000000 xe-admix-1.0.10/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-08-01 08:19:32.000000 xe-admix-1.0.10/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-08-01 08:19:39.652194 xe-admix-1.0.10/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-08-01 08:19:32.000000 xe-admix-1.0.10/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:19:39.648194 xe-admix-1.0.10/admix/
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-08-01 08:19:32.000000 xe-admix-1.0.10/admix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-08-01 08:19:32.000000 xe-admix-1.0.10/admix/admix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-08-01 08:19:32.000000 xe-admix-1.0.10/admix/clients.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:19:39.648194 xe-admix-1.0.10/admix/daemons/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 08:19:32.000000 xe-admix-1.0.10/admix/daemons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-08-01 08:19:32.000000 xe-admix-1.0.10/admix/daemons/daemon.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-08-01 08:19:32.000000 xe-admix-1.0.10/admix/daemons/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-08-01 08:19:32.000000 xe-admix-1.0.10/admix/daemons/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-08-01 08:19:32.000000 xe-admix-1.0.10/admix/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    15707 2023-08-01 08:19:32.000000 xe-admix-1.0.10/admix/fix.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:19:39.648194 xe-admix-1.0.10/admix/helper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 08:19:32.000000 xe-admix-1.0.10/admix/helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-01 08:19:32.000000 xe-admix-1.0.10/admix/helper/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10103 2023-08-01 08:19:32.000000 xe-admix-1.0.10/admix/helper/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:19:39.648194 xe-admix-1.0.10/admix/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 08:19:32.000000 xe-admix-1.0.10/admix/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22176 2023-08-01 08:19:32.000000 xe-admix-1.0.10/admix/interfaces/rucio_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    36718 2023-08-01 08:19:32.000000 xe-admix-1.0.10/admix/interfaces/rucio_summoner.py
--rw-r--r--   0 runner    (1001) docker     (123)    15506 2023-08-01 08:19:32.000000 xe-admix-1.0.10/admix/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-08-01 08:19:32.000000 xe-admix-1.0.10/admix/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    11892 2023-08-01 08:19:32.000000 xe-admix-1.0.10/admix/rucio.py
--rw-r--r--   0 runner    (1001) docker     (123)    12886 2023-08-01 08:19:32.000000 xe-admix-1.0.10/admix/showrun.py
--rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-08-01 08:19:32.000000 xe-admix-1.0.10/admix/uploader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-08-01 08:19:32.000000 xe-admix-1.0.10/admix/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-08-01 08:19:32.000000 xe-admix-1.0.10/admix/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:19:39.648194 xe-admix-1.0.10/bin/
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-08-01 08:19:32.000000 xe-admix-1.0.10/bin/admix-download
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:19:39.652194 xe-admix-1.0.10/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6758 2023-08-01 08:19:32.000000 xe-admix-1.0.10/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-01 08:19:32.000000 xe-admix-1.0.10/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     8661 2023-08-01 08:19:32.000000 xe-admix-1.0.10/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-08-01 08:19:32.000000 xe-admix-1.0.10/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-01 08:19:32.000000 xe-admix-1.0.10/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-01 08:19:32.000000 xe-admix-1.0.10/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-08-01 08:19:32.000000 xe-admix-1.0.10/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-08-01 08:19:32.000000 xe-admix-1.0.10/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6457 2023-08-01 08:19:32.000000 xe-admix-1.0.10/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-01 08:19:32.000000 xe-admix-1.0.10/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)    28723 2023-08-01 08:19:32.000000 xe-admix-1.0.10/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-01 08:19:32.000000 xe-admix-1.0.10/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 08:19:39.652194 xe-admix-1.0.10/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-08-01 08:19:32.000000 xe-admix-1.0.10/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:19:39.652194 xe-admix-1.0.10/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-01 08:19:32.000000 xe-admix-1.0.10/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-08-01 08:19:32.000000 xe-admix-1.0.10/tests/test_admix.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:19:39.652194 xe-admix-1.0.10/xe_admix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-08-01 08:19:39.000000 xe-admix-1.0.10/xe_admix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-08-01 08:19:39.000000 xe-admix-1.0.10/xe_admix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 08:19:39.000000 xe-admix-1.0.10/xe_admix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 08:19:39.000000 xe-admix-1.0.10/xe_admix.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-01 08:19:39.000000 xe-admix-1.0.10/xe_admix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-01 08:19:39.000000 xe-admix-1.0.10/xe_admix.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:04:49.279588 xe-admix-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-21 18:04:44.000000 xe-admix-1.0.9/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-05-21 18:04:44.000000 xe-admix-1.0.9/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-21 18:04:44.000000 xe-admix-1.0.9/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-21 18:04:44.000000 xe-admix-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-21 18:04:44.000000 xe-admix-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-05-21 18:04:49.279588 xe-admix-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-21 18:04:44.000000 xe-admix-1.0.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:04:49.275588 xe-admix-1.0.9/admix/
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-21 18:04:44.000000 xe-admix-1.0.9/admix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-21 18:04:44.000000 xe-admix-1.0.9/admix/admix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-21 18:04:44.000000 xe-admix-1.0.9/admix/clients.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:04:49.275588 xe-admix-1.0.9/admix/daemons/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 18:04:44.000000 xe-admix-1.0.9/admix/daemons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-05-21 18:04:44.000000 xe-admix-1.0.9/admix/daemons/daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-21 18:04:44.000000 xe-admix-1.0.9/admix/daemons/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-05-21 18:04:44.000000 xe-admix-1.0.9/admix/daemons/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-05-21 18:04:44.000000 xe-admix-1.0.9/admix/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15707 2023-05-21 18:04:44.000000 xe-admix-1.0.9/admix/fix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:04:49.275588 xe-admix-1.0.9/admix/helper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 18:04:44.000000 xe-admix-1.0.9/admix/helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-21 18:04:44.000000 xe-admix-1.0.9/admix/helper/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10103 2023-05-21 18:04:44.000000 xe-admix-1.0.9/admix/helper/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:04:49.275588 xe-admix-1.0.9/admix/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 18:04:44.000000 xe-admix-1.0.9/admix/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22176 2023-05-21 18:04:44.000000 xe-admix-1.0.9/admix/interfaces/rucio_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36718 2023-05-21 18:04:44.000000 xe-admix-1.0.9/admix/interfaces/rucio_summoner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15506 2023-05-21 18:04:44.000000 xe-admix-1.0.9/admix/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-05-21 18:04:44.000000 xe-admix-1.0.9/admix/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11892 2023-05-21 18:04:44.000000 xe-admix-1.0.9/admix/rucio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12886 2023-05-21 18:04:44.000000 xe-admix-1.0.9/admix/showrun.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-05-21 18:04:44.000000 xe-admix-1.0.9/admix/uploader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-05-21 18:04:44.000000 xe-admix-1.0.9/admix/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-05-21 18:04:44.000000 xe-admix-1.0.9/admix/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:04:49.275588 xe-admix-1.0.9/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-05-21 18:04:44.000000 xe-admix-1.0.9/bin/admix-download
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:04:49.279588 xe-admix-1.0.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6758 2023-05-21 18:04:44.000000 xe-admix-1.0.9/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-21 18:04:44.000000 xe-admix-1.0.9/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8661 2023-05-21 18:04:44.000000 xe-admix-1.0.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-21 18:04:44.000000 xe-admix-1.0.9/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-21 18:04:44.000000 xe-admix-1.0.9/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-21 18:04:44.000000 xe-admix-1.0.9/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-21 18:04:44.000000 xe-admix-1.0.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-05-21 18:04:44.000000 xe-admix-1.0.9/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6457 2023-05-21 18:04:44.000000 xe-admix-1.0.9/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-21 18:04:44.000000 xe-admix-1.0.9/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    28723 2023-05-21 18:04:44.000000 xe-admix-1.0.9/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-21 18:04:44.000000 xe-admix-1.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 18:04:49.279588 xe-admix-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-21 18:04:44.000000 xe-admix-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:04:49.279588 xe-admix-1.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-21 18:04:44.000000 xe-admix-1.0.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-21 18:04:44.000000 xe-admix-1.0.9/tests/test_admix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:04:49.279588 xe-admix-1.0.9/xe_admix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-05-21 18:04:49.000000 xe-admix-1.0.9/xe_admix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-21 18:04:49.000000 xe-admix-1.0.9/xe_admix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 18:04:49.000000 xe-admix-1.0.9/xe_admix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 18:04:49.000000 xe-admix-1.0.9/xe_admix.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-21 18:04:49.000000 xe-admix-1.0.9/xe_admix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-21 18:04:49.000000 xe-admix-1.0.9/xe_admix.egg-info/top_level.txt
```

### Comparing `xe-admix-1.0.10/CONTRIBUTING.rst` & `xe-admix-1.0.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `xe-admix-1.0.10/LICENSE` & `xe-admix-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `xe-admix-1.0.10/PKG-INFO` & `xe-admix-1.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: xe-admix
-Version: 1.0.10
+Version: 1.0.9
 Summary: advanced Data Management In Xenon (aDMIX)
 Home-page: https://github.com/XENON1T/admix
 Author: UNKNOWN
 Author-email: UNKNOWN
 License: BSD license
 Description: =====
         aDMIX
```

### Comparing `xe-admix-1.0.10/README.rst` & `xe-admix-1.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `xe-admix-1.0.10/admix/__init__.py` & `xe-admix-1.0.9/admix/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 """Top-level package for aDMIX."""
-__version__ = '1.0.10'
+__version__ = '1.0.9'
 
 import os
 import logging
 from utilix import uconfig
 
 def get_logger():
     logger = logging.getLogger("admix")
```

### Comparing `xe-admix-1.0.10/admix/admix.py` & `xe-admix-1.0.9/admix/admix.py`

 * *Files identical despite different names*

### Comparing `xe-admix-1.0.10/admix/clients.py` & `xe-admix-1.0.9/admix/clients.py`

 * *Files identical despite different names*

### Comparing `xe-admix-1.0.10/admix/daemons/daemon.py` & `xe-admix-1.0.9/admix/daemons/daemon.py`

 * *Files identical despite different names*

### Comparing `xe-admix-1.0.10/admix/daemons/upload.py` & `xe-admix-1.0.9/admix/daemons/upload.py`

 * *Files identical despite different names*

### Comparing `xe-admix-1.0.10/admix/downloader.py` & `xe-admix-1.0.9/admix/downloader.py`

 * *Files identical despite different names*

### Comparing `xe-admix-1.0.10/admix/fix.py` & `xe-admix-1.0.9/admix/fix.py`

 * *Files identical despite different names*

### Comparing `xe-admix-1.0.10/admix/helper/helper.py` & `xe-admix-1.0.9/admix/helper/helper.py`

 * *Files identical despite different names*

### Comparing `xe-admix-1.0.10/admix/interfaces/rucio_api.py` & `xe-admix-1.0.9/admix/interfaces/rucio_api.py`

 * *Files identical despite different names*

### Comparing `xe-admix-1.0.10/admix/interfaces/rucio_summoner.py` & `xe-admix-1.0.9/admix/interfaces/rucio_summoner.py`

 * *Files identical despite different names*

### Comparing `xe-admix-1.0.10/admix/manager.py` & `xe-admix-1.0.9/admix/manager.py`

 * *Files identical despite different names*

### Comparing `xe-admix-1.0.10/admix/monitor.py` & `xe-admix-1.0.9/admix/monitor.py`

 * *Files identical despite different names*

### Comparing `xe-admix-1.0.10/admix/rucio.py` & `xe-admix-1.0.9/admix/rucio.py`

 * *Files identical despite different names*

### Comparing `xe-admix-1.0.10/admix/showrun.py` & `xe-admix-1.0.9/admix/showrun.py`

 * *Files identical despite different names*

### Comparing `xe-admix-1.0.10/admix/uploader.py` & `xe-admix-1.0.9/admix/uploader.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,16 +6,15 @@
 
 
 def get_default_scope():
     return 'user.' + clients.upload_client.client.account
 
 
 # TODO could we make this use multithreading or multiprocessing to speed things up?
-def upload(path, rse, 
-           register_after_upload=False, verbose=True, did=None, lifetime=None, update_db=False):
+def upload(path, rse, did=None, lifetime=None, update_db=False):
 
     # set scope initially to default one. will overwrite it below if did passed
     scope = get_default_scope()
 
     if did:
         if ':' in did:
             scope, name = did.split(':')
@@ -37,38 +36,33 @@
         try:
             existing_files = list_files(did)
         except DataIdentifierNotFound:
             pass
 
         to_upload = []
 
-        missing_files = set(local_files) - set(existing_files)
-        if verbose:
-            print(f"Found {len(missing_files)} files to upload:")
-            print(missing_files)
-            print("------")
-        for missing_file in missing_files:
+        for missing_file in set(local_files) - set(existing_files):
             _path = os.path.join(path, missing_file)
             to_upload.append(dict(path=_path,
                                   rse=rse,
                                   did_scope=scope,
                                   did_name=missing_file,
                                   dataset_scope=scope,
                                   dataset_name=name,
-                                  register_after_upload=register_after_upload,
+                                  register_after_upload=True,
                                   lifetime=lifetime
                                   )
                              )
     else:
         upload_dict = dict(path=path,
                            rse=rse,
                            did_scope=scope,
                            dataset_scope=scope,
                            dataset_name=name,
-                           register_after_upload=register_after_upload,
+                           register_after_upload=True,
                            lifetime=lifetime
                            )
         to_upload = [upload_dict]
 
     # get data dict to add to database
     number, dtype, lineage_hash = parse_did(did)
     data_dict = dict(did=did,
@@ -79,21 +73,15 @@
                      meta=dict(),
                      protocol='rucio',
                     )
 
     if len(to_upload):
         if update_db:
             db.update_data(number, data_dict)
-        try:
-            clients.upload_client.upload(to_upload)
-        except Exception as e:
-            if verbose:
-                print(f"Upload failed for {path}")
-                print(e)
-            return did
+        clients.upload_client.upload(to_upload)
         # then update db again when complete
         if update_db:
             data_dict['status'] = 'transferred'
             # get files, size etc
             files = list_files(did, verbose=True)
             size = sum([f['bytes'] for f in files]) / 1e6
             data_dict['meta'] = dict(lineage_hash=lineage_hash,
```

### Comparing `xe-admix-1.0.10/admix/utils.py` & `xe-admix-1.0.9/admix/utils.py`

 * *Files identical despite different names*

### Comparing `xe-admix-1.0.10/admix/validator.py` & `xe-admix-1.0.9/admix/validator.py`

 * *Files identical despite different names*

### Comparing `xe-admix-1.0.10/bin/admix-download` & `xe-admix-1.0.9/bin/admix-download`

 * *Files identical despite different names*

### Comparing `xe-admix-1.0.10/docs/Makefile` & `xe-admix-1.0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `xe-admix-1.0.10/docs/conf.py` & `xe-admix-1.0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `xe-admix-1.0.10/docs/configuration.rst` & `xe-admix-1.0.9/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `xe-admix-1.0.10/docs/installation.rst` & `xe-admix-1.0.9/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `xe-admix-1.0.10/docs/make.bat` & `xe-admix-1.0.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `xe-admix-1.0.10/docs/usage.rst` & `xe-admix-1.0.9/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `xe-admix-1.0.10/setup.py` & `xe-admix-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Get requirements from requirements.txt, stripping the version tags
 with open('requirements.txt') as f:
     requirements = [r.split('/')[-1] if r.startswith('git+') else r for r in f.read().splitlines()]
 
 
 setup(
     name='xe-admix',
-    version='1.0.10',
+    version='1.0.9',
     description="advanced Data Management In Xenon (aDMIX)",
     long_description=readme + '\n\n' + history,
     url='https://github.com/XENON1T/admix',
     install_requires=requirements,
     scripts=['bin/admix-download'],
     packages=find_packages(),
     license="BSD license",
```

### Comparing `xe-admix-1.0.10/xe_admix.egg-info/PKG-INFO` & `xe-admix-1.0.9/xe_admix.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: xe-admix
-Version: 1.0.10
+Version: 1.0.9
 Summary: advanced Data Management In Xenon (aDMIX)
 Home-page: https://github.com/XENON1T/admix
 Author: UNKNOWN
 Author-email: UNKNOWN
 License: BSD license
 Description: =====
         aDMIX
```

### Comparing `xe-admix-1.0.10/xe_admix.egg-info/SOURCES.txt` & `xe-admix-1.0.9/xe_admix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

