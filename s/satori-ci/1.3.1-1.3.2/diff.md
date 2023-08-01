# Comparing `tmp/satori_ci-1.3.1.tar.gz` & `tmp/satori_ci-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satori_ci-1.3.1.tar", last modified: Tue Aug  1 14:45:56 2023, max compression
+gzip compressed data, was "satori_ci-1.3.2.tar", last modified: Tue Aug  1 14:58:54 2023, max compression
```

## Comparing `satori_ci-1.3.1.tar` & `satori_ci-1.3.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    35149 2023-08-01 14:45:33.791812 satori_ci-1.3.1/LICENSE
--rw-r--r--   0        0        0     7140 2023-08-01 14:45:33.791812 satori_ci-1.3.1/README.md
--rw-r--r--   0        0        0      755 2023-08-01 14:45:56.007913 satori_ci-1.3.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-08-01 14:45:33.795812 satori_ci-1.3.1/src/satoricli/__init__.py
--rw-r--r--   0        0        0       37 2023-08-01 14:45:33.795812 satori_ci-1.3.1/src/satoricli/__main__.py
--rw-r--r--   0        0        0     4558 2023-08-01 14:45:33.795812 satori_ci-1.3.1/src/satoricli/classes/api.py
--rw-r--r--   0        0        0     1633 2023-08-01 14:45:33.795812 satori_ci-1.3.1/src/satoricli/classes/bundler.py
--rw-r--r--   0        0        0      468 2023-08-01 14:45:33.795812 satori_ci-1.3.1/src/satoricli/classes/models.py
--rw-r--r--   0        0        0     3345 2023-08-01 14:45:33.795812 satori_ci-1.3.1/src/satoricli/classes/playbooks.py
--rw-r--r--   0        0        0    28020 2023-08-01 14:45:33.795812 satori_ci-1.3.1/src/satoricli/classes/satori.py
--rw-r--r--   0        0        0    12442 2023-08-01 14:45:33.795812 satori_ci-1.3.1/src/satoricli/classes/utils.py
--rw-r--r--   0        0        0     1194 2023-08-01 14:45:33.795812 satori_ci-1.3.1/src/satoricli/classes/validations.py
--rwxr-xr-x   0        0        0     8966 2023-08-01 14:45:33.795812 satori_ci-1.3.1/src/satoricli/cli/parser.py
--rw-r--r--   0        0        0    48305 1970-01-01 00:00:00.000000 satori_ci-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-08-01 14:58:39.148381 satori_ci-1.3.2/LICENSE
+-rw-r--r--   0        0        0     7140 2023-08-01 14:58:39.148381 satori_ci-1.3.2/README.md
+-rw-r--r--   0        0        0      755 2023-08-01 14:58:54.964747 satori_ci-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-01 14:58:39.148381 satori_ci-1.3.2/src/satoricli/__init__.py
+-rw-r--r--   0        0        0       37 2023-08-01 14:58:39.148381 satori_ci-1.3.2/src/satoricli/__main__.py
+-rw-r--r--   0        0        0     4558 2023-08-01 14:58:39.148381 satori_ci-1.3.2/src/satoricli/classes/api.py
+-rw-r--r--   0        0        0     1633 2023-08-01 14:58:39.148381 satori_ci-1.3.2/src/satoricli/classes/bundler.py
+-rw-r--r--   0        0        0      468 2023-08-01 14:58:39.148381 satori_ci-1.3.2/src/satoricli/classes/models.py
+-rw-r--r--   0        0        0     3345 2023-08-01 14:58:39.148381 satori_ci-1.3.2/src/satoricli/classes/playbooks.py
+-rw-r--r--   0        0        0    28020 2023-08-01 14:58:39.148381 satori_ci-1.3.2/src/satoricli/classes/satori.py
+-rw-r--r--   0        0        0    12442 2023-08-01 14:58:39.148381 satori_ci-1.3.2/src/satoricli/classes/utils.py
+-rw-r--r--   0        0        0     1194 2023-08-01 14:58:39.148381 satori_ci-1.3.2/src/satoricli/classes/validations.py
+-rwxr-xr-x   0        0        0     8991 2023-08-01 14:58:39.148381 satori_ci-1.3.2/src/satoricli/cli/parser.py
+-rw-r--r--   0        0        0    48305 1970-01-01 00:00:00.000000 satori_ci-1.3.2/PKG-INFO
```

### Comparing `satori_ci-1.3.1/LICENSE` & `satori_ci-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `satori_ci-1.3.1/README.md` & `satori_ci-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `satori_ci-1.3.1/pyproject.toml` & `satori_ci-1.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "satori-ci"
-version = "1.3.1"
+version = "1.3.2"
 description = "Satori CI - Automated Software Testing Platform"
 authors = [
     { name = "Satori CI CLI", email = "info@satori-ci.com" },
 ]
 dependencies = [
     "requests>=2.27.1",
     "pyyaml>=6.0",
```

### Comparing `satori_ci-1.3.1/src/satoricli/classes/api.py` & `satori_ci-1.3.2/src/satoricli/classes/api.py`

 * *Files identical despite different names*

### Comparing `satori_ci-1.3.1/src/satoricli/classes/bundler.py` & `satori_ci-1.3.2/src/satoricli/classes/bundler.py`

 * *Files identical despite different names*

### Comparing `satori_ci-1.3.1/src/satoricli/classes/playbooks.py` & `satori_ci-1.3.2/src/satoricli/classes/playbooks.py`

 * *Files identical despite different names*

### Comparing `satori_ci-1.3.1/src/satoricli/classes/satori.py` & `satori_ci-1.3.2/src/satoricli/classes/satori.py`

 * *Files identical despite different names*

### Comparing `satori_ci-1.3.1/src/satoricli/classes/utils.py` & `satori_ci-1.3.2/src/satoricli/classes/utils.py`

 * *Files identical despite different names*

### Comparing `satori_ci-1.3.1/src/satoricli/classes/validations.py` & `satori_ci-1.3.2/src/satoricli/classes/validations.py`

 * *Files identical despite different names*

### Comparing `satori_ci-1.3.1/src/satoricli/cli/parser.py` & `satori_ci-1.3.2/src/satoricli/cli/parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 from argparse import ArgumentParser
-import os
+import subprocess
 import sys
 import requests  # autoupgrade
 from importlib import metadata
 from colorama import just_fix_windows_console
 from rich import print
 from pkg_resources import get_distribution, DistributionNotFound  # autoupgrade
 from packaging import version  # autoupgrade
@@ -215,13 +215,13 @@
             instance.team(args)
         elif args.subcommand == "user":
             instance.user(args)
         elif args.subcommand in (None, "dashboard"):
             instance.dashboard(args)
         elif args.subcommand == "help":
             if args.web:
-                os.system("satori-docs")
+                subprocess.run(["satori-docs", "--web"])
             else:
-                os.system("satori-docs --web")
+                subprocess.run(["satori-docs"])
     except KeyboardInterrupt:
         console.print("[critical]Interrupted by user")
         sys.exit(1)
```

### Comparing `satori_ci-1.3.1/PKG-INFO` & `satori_ci-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satori-ci
-Version: 1.3.1
+Version: 1.3.2
 Summary: Satori CI - Automated Software Testing Platform
 Author-Email: Satori CI CLI <info@satori-ci.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

