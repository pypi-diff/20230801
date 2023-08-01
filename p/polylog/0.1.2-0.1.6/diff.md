# Comparing `tmp/polylog-0.1.2.tar.gz` & `tmp/polylog-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polylog-0.1.2.tar", last modified: Tue Aug  1 20:27:31 2023, max compression
+gzip compressed data, was "polylog-0.1.6.tar", last modified: Tue Aug  1 21:40:24 2023, max compression
```

## Comparing `polylog-0.1.2.tar` & `polylog-0.1.6.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:27:31.418644 polylog-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-08-01 20:27:31.418644 polylog-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-08-01 20:27:21.000000 polylog-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:27:31.414644 polylog-0.1.2/polylog/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-08-01 20:27:21.000000 polylog-0.1.2/polylog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-08-01 20:27:21.000000 polylog-0.1.2/polylog/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:27:31.418644 polylog-0.1.2/polylog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-08-01 20:27:31.000000 polylog-0.1.2/polylog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-08-01 20:27:31.000000 polylog-0.1.2/polylog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 20:27:31.000000 polylog-0.1.2/polylog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-01 20:27:31.000000 polylog-0.1.2/polylog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-01 20:27:31.000000 polylog-0.1.2/polylog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-08-01 20:27:24.000000 polylog-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 20:27:31.418644 polylog-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-08-01 20:27:21.000000 polylog-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:27:31.418644 polylog-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-08-01 20:27:21.000000 polylog-0.1.2/tests/logger_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:40:24.549482 polylog-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-08-01 21:40:24.549482 polylog-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-08-01 21:40:08.000000 polylog-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:40:24.545482 polylog-0.1.6/polylog/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-08-01 21:40:08.000000 polylog-0.1.6/polylog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-08-01 21:40:08.000000 polylog-0.1.6/polylog/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:40:24.549482 polylog-0.1.6/polylog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-08-01 21:40:24.000000 polylog-0.1.6/polylog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-08-01 21:40:24.000000 polylog-0.1.6/polylog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 21:40:24.000000 polylog-0.1.6/polylog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-01 21:40:24.000000 polylog-0.1.6/polylog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-01 21:40:24.000000 polylog-0.1.6/polylog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-08-01 21:40:14.000000 polylog-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 21:40:24.549482 polylog-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-08-01 21:40:08.000000 polylog-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:40:24.549482 polylog-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-08-01 21:40:08.000000 polylog-0.1.6/tests/logger_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-08-01 21:40:08.000000 polylog-0.1.6/tests/manual_logger_test.py
```

### Comparing `polylog-0.1.2/PKG-INFO` & `polylog-0.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polylog
-Version: 0.1.2
+Version: 0.1.6
 Summary: A custom python logging package
 Home-page: https://github.com/lvlcn-t/PolyLog
 Author: lvlcn-t
 Author-email: lvlcn-t <75443136+lvlcn-t@users.noreply.github.com>
 Maintainer-email: lvlcn-t <75443136+lvlcn-t@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/lvlcn-t/polylog
 Project-URL: Bug Reports, https://github.com/lvlcn-t/polylog/issues
```

### Comparing `polylog-0.1.2/README.md` & `polylog-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `polylog-0.1.2/polylog/logger.py` & `polylog-0.1.6/polylog/logger.py`

 * *Files 5% similar despite different names*

```diff
@@ -100,14 +100,15 @@
                     maxBytes=int(
                         os.getenv("LOG_MAX_BYTES", 32 * 1024 * 1024)
                     ),  # 32 MiB
                     backupCount=int(
                         os.getenv("LOG_BACKUP_COUNT", 2)
                     ),  # Rotate through 2 files
                 )
-                log_handler.setFormatter(CustomFormatter())
+                file_formatter = logging.Formatter("%(asctime)-s %(levelname)-8s %(name)s %(extra)s %(message)s", "%Y-%m-%d %H:%M:%S")
+                log_handler.setFormatter(file_formatter)
                 log_handler.setLevel(level)
                 logger.addHandler(log_handler)
             except Exception as e:
                 logger.error(f"Failed to create file handler: {e}")
 
         return logger
```

### Comparing `polylog-0.1.2/polylog.egg-info/PKG-INFO` & `polylog-0.1.6/polylog.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polylog
-Version: 0.1.2
+Version: 0.1.6
 Summary: A custom python logging package
 Home-page: https://github.com/lvlcn-t/PolyLog
 Author: lvlcn-t
 Author-email: lvlcn-t <75443136+lvlcn-t@users.noreply.github.com>
 Maintainer-email: lvlcn-t <75443136+lvlcn-t@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/lvlcn-t/polylog
 Project-URL: Bug Reports, https://github.com/lvlcn-t/polylog/issues
```

### Comparing `polylog-0.1.2/pyproject.toml` & `polylog-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "polylog"  # Required
-version = "0.1.2"
+version = "0.1.6"
 description = "A custom python logging package"  # Optional
 
 readme = "README.md" # Optional
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 
 keywords = []  # Optional
```

### Comparing `polylog-0.1.2/setup.py` & `polylog-0.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `polylog-0.1.2/tests/logger_test.py` & `polylog-0.1.6/tests/logger_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     def setUp(self):
         self.stream = StringIO()
         self.log = logging.getLogger('test_logger')
         self.log.setLevel(logging.DEBUG)
         handler = logging.StreamHandler(self.stream)
         handler.setFormatter(CustomFormatter())
         self.log.addHandler(handler)
+        os.environ["LOGGING"] = "True"
         os.environ["LOG_LEVEL"] = "DEBUG"
 
     def test_setup_logger(self):
         logger = setup_logger(self.log.name)
         self.assertIsInstance(logger, logging.Logger)
         self.assertEqual(logger.name, self.log.name)
```

