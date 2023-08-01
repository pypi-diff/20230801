# Comparing `tmp/pypomes_scheduling-0.2.1.tar.gz` & `tmp/pypomes_scheduling-0.2.2.tar.gz`

## Comparing `pypomes_scheduling-0.2.1.tar` & `pypomes_scheduling-0.2.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.1/src/pypomes_scheduling/__init__.py
--rw-r--r--   0        0        0     4714 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.1/src/pypomes_scheduling/__threaded_scheduler.py
--rw-r--r--   0        0        0     9739 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.1/src/pypomes_scheduling/scheduling_pomes.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.1/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.1/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.1/README.md
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.2/src/pypomes_scheduling/__init__.py
+-rw-r--r--   0        0        0     4736 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.2/src/pypomes_scheduling/__threaded_scheduler.py
+-rw-r--r--   0        0        0     9739 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.2/src/pypomes_scheduling/scheduling_pomes.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.2/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.2/README.md
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.2/PKG-INFO
```

### Comparing `pypomes_scheduling-0.2.1/src/pypomes_scheduling/__threaded_scheduler.py` & `pypomes_scheduling-0.2.2/src/pypomes_scheduling/__threaded_scheduler.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 import logging
 import pytz
 import threading
 
 
 class __ThreadedScheduler(threading.Thread):
     """
-    A scalable implementation of *APScheduler*'s *BlockingScheduler*, running as single or multiple instances,
-    each on its own thread.
+    A scalable implementation of *APScheduler*'s *BlockingScheduler*.
+
+    This implementation may run as single or multiple instances, each on its own thread.
     """
     _scheduler: BlockingScheduler
     _logger: logging.Logger
     _stopped: bool
 
     def __init__(self, timezone: pytz.timezone, retry_interval: int, logger: logging.Logger = None):
```

### Comparing `pypomes_scheduling-0.2.1/src/pypomes_scheduling/scheduling_pomes.py` & `pypomes_scheduling-0.2.2/src/pypomes_scheduling/scheduling_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_scheduling-0.2.1/LICENSE` & `pypomes_scheduling-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_scheduling-0.2.1/pyproject.toml` & `pypomes_scheduling-0.2.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 requires = [
     "hatchling"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_scheduling"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (scheduling module)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
 dependencies = [
-    "pip>=23.1.2",
-    "pypomes_core>=0.1.4",
+    "pip>=23.2.1",
+    "pypomes_core>=0.2.1",
     "APScheduler>=3.10.1",
     "setuptools>=68.0.0",
-    "wheel>=0.40.0"
+    "wheel>=0.41.0"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/TheWiseCoder/PyPomes-Scheduling"
 "Bug Tracker" = "https://github.com/TheWiseCoder/PyPomes-Scheduling/issues"
```

### Comparing `pypomes_scheduling-0.2.1/PKG-INFO` & `pypomes_scheduling-0.2.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pypomes_scheduling
-Version: 0.2.1
+Version: 0.2.2
 Summary: A collection of Python pomes, pennyeach (scheduling module)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-Scheduling
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-Scheduling/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: apscheduler>=3.10.1
-Requires-Dist: pip>=23.1.2
-Requires-Dist: pypomes-core>=0.1.4
+Requires-Dist: pip>=23.2.1
+Requires-Dist: pypomes-core>=0.2.1
 Requires-Dist: setuptools>=68.0.0
-Requires-Dist: wheel>=0.40.0
+Requires-Dist: wheel>=0.41.0
```

