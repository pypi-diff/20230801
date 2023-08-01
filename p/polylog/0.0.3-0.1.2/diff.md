# Comparing `tmp/polylog-0.0.3.tar.gz` & `tmp/polylog-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polylog-0.0.3.tar", last modified: Wed Jul 26 19:59:32 2023, max compression
+gzip compressed data, was "polylog-0.1.2.tar", last modified: Tue Aug  1 20:27:31 2023, max compression
```

## Comparing `polylog-0.0.3.tar` & `polylog-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:59:32.091702 polylog-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-07-26 19:59:32.087702 polylog-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-26 19:59:18.000000 polylog-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:59:32.087702 polylog-0.0.3/polylog/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-26 19:59:18.000000 polylog-0.0.3/polylog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-07-26 19:59:18.000000 polylog-0.0.3/polylog/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:59:32.087702 polylog-0.0.3/polylog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-07-26 19:59:32.000000 polylog-0.0.3/polylog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-26 19:59:32.000000 polylog-0.0.3/polylog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 19:59:32.000000 polylog-0.0.3/polylog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-26 19:59:32.000000 polylog-0.0.3/polylog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-26 19:59:32.000000 polylog-0.0.3/polylog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-26 19:59:24.000000 polylog-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 19:59:32.091702 polylog-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-26 19:59:18.000000 polylog-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:59:32.087702 polylog-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-07-26 19:59:18.000000 polylog-0.0.3/tests/logger_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:27:31.418644 polylog-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-08-01 20:27:31.418644 polylog-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-08-01 20:27:21.000000 polylog-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:27:31.414644 polylog-0.1.2/polylog/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-08-01 20:27:21.000000 polylog-0.1.2/polylog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-08-01 20:27:21.000000 polylog-0.1.2/polylog/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:27:31.418644 polylog-0.1.2/polylog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-08-01 20:27:31.000000 polylog-0.1.2/polylog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-08-01 20:27:31.000000 polylog-0.1.2/polylog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 20:27:31.000000 polylog-0.1.2/polylog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-01 20:27:31.000000 polylog-0.1.2/polylog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-01 20:27:31.000000 polylog-0.1.2/polylog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-08-01 20:27:24.000000 polylog-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 20:27:31.418644 polylog-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-08-01 20:27:21.000000 polylog-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:27:31.418644 polylog-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-08-01 20:27:21.000000 polylog-0.1.2/tests/logger_test.py
```

### Comparing `polylog-0.0.3/PKG-INFO` & `polylog-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polylog
-Version: 0.0.3
+Version: 0.1.2
 Summary: A custom python logging package
 Home-page: https://github.com/lvlcn-t/PolyLog
 Author: lvlcn-t
 Author-email: lvlcn-t <75443136+lvlcn-t@users.noreply.github.com>
 Maintainer-email: lvlcn-t <75443136+lvlcn-t@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/lvlcn-t/polylog
 Project-URL: Bug Reports, https://github.com/lvlcn-t/polylog/issues
```

### Comparing `polylog-0.0.3/README.md` & `polylog-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `polylog-0.0.3/polylog.egg-info/PKG-INFO` & `polylog-0.1.2/polylog.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polylog
-Version: 0.0.3
+Version: 0.1.2
 Summary: A custom python logging package
 Home-page: https://github.com/lvlcn-t/PolyLog
 Author: lvlcn-t
 Author-email: lvlcn-t <75443136+lvlcn-t@users.noreply.github.com>
 Maintainer-email: lvlcn-t <75443136+lvlcn-t@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/lvlcn-t/polylog
 Project-URL: Bug Reports, https://github.com/lvlcn-t/polylog/issues
```

### Comparing `polylog-0.0.3/pyproject.toml` & `polylog-0.1.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "polylog"  # Required
-version = "0.0.3"
+version = "0.1.2"
 description = "A custom python logging package"  # Optional
 
 readme = "README.md" # Optional
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 
 keywords = []  # Optional
```

### Comparing `polylog-0.0.3/setup.py` & `polylog-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `polylog-0.0.3/tests/logger_test.py` & `polylog-0.1.2/tests/logger_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-import unittest
-from io import StringIO
-from contextlib import redirect_stdout
 import logging
 import os
 import sys
+import unittest
+from contextlib import redirect_stdout
+from io import StringIO
+
 sys.path.append(os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
 
-from polylog import setup_logger, TRACE_ID, SPAN_ID     # noqa: E402
-from polylog.logger import CustomFormatter              # noqa: E402
+from polylog import SPAN_ID, TRACE_ID, setup_logger
+from polylog.logger import CustomFormatter
 
 
 class LoggerTests(unittest.TestCase):
     def setUp(self):
         self.stream = StringIO()
         self.log = logging.getLogger('test_logger')
         self.log.setLevel(logging.DEBUG)
```

