# Comparing `tmp/evenity-0.0.8.tar.gz` & `tmp/evenity-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evenity-0.0.8.tar", last modified: Mon Jul 31 21:39:24 2023, max compression
+gzip compressed data, was "evenity-0.0.9.tar", last modified: Mon Jul 31 22:11:33 2023, max compression
```

## Comparing `evenity-0.0.8.tar` & `evenity-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 localghost  (1000) localghost  (1000)        0 2023-07-31 21:39:24.672329 evenity-0.0.8/
--rw-r--r--   0 localghost  (1000) localghost  (1000)        0 2023-07-28 21:02:20.000000 evenity-0.0.8/LICENSE
--rw-r--r--   0 localghost  (1000) localghost  (1000)     7703 2023-07-31 21:39:24.672329 evenity-0.0.8/PKG-INFO
--rw-r--r--   0 localghost  (1000) localghost  (1000)     7248 2023-07-31 21:11:07.000000 evenity-0.0.8/README.md
--rw-r--r--   0 localghost  (1000) localghost  (1000)      532 2023-07-31 21:38:27.000000 evenity-0.0.8/pyproject.toml
--rw-r--r--   0 localghost  (1000) localghost  (1000)       38 2023-07-31 21:39:24.672329 evenity-0.0.8/setup.cfg
-drwxr-xr-x   0 localghost  (1000) localghost  (1000)        0 2023-07-31 21:39:24.672329 evenity-0.0.8/src/
-drwxr-xr-x   0 localghost  (1000) localghost  (1000)        0 2023-07-31 21:39:24.672329 evenity-0.0.8/src/evenity/
--rw-r--r--   0 localghost  (1000) localghost  (1000)        0 2023-07-28 23:22:35.000000 evenity-0.0.8/src/evenity/__init__.py
--rw-r--r--   0 localghost  (1000) localghost  (1000)      404 2023-07-30 16:47:07.000000 evenity-0.0.8/src/evenity/observable.py
--rw-r--r--   0 localghost  (1000) localghost  (1000)      845 2023-07-31 21:38:27.000000 evenity-0.0.8/src/evenity/observer.py
-drwxr-xr-x   0 localghost  (1000) localghost  (1000)        0 2023-07-31 21:39:24.672329 evenity-0.0.8/src/evenity/plugins/
--rw-r--r--   0 localghost  (1000) localghost  (1000)        0 2023-07-28 23:22:35.000000 evenity-0.0.8/src/evenity/plugins/__init__.py
--rw-r--r--   0 localghost  (1000) localghost  (1000)     1451 2023-07-31 21:11:07.000000 evenity-0.0.8/src/evenity/plugins/ftp.py
--rw-r--r--   0 localghost  (1000) localghost  (1000)      714 2023-07-28 23:22:35.000000 evenity-0.0.8/src/evenity/plugins/kafka.py
--rw-r--r--   0 localghost  (1000) localghost  (1000)      632 2023-07-28 23:22:35.000000 evenity-0.0.8/src/evenity/plugins/shell.py
--rw-r--r--   0 localghost  (1000) localghost  (1000)      742 2023-07-31 21:11:07.000000 evenity-0.0.8/src/evenity/plugins/telegram.py
--rw-r--r--   0 localghost  (1000) localghost  (1000)     1741 2023-07-30 17:27:26.000000 evenity-0.0.8/src/evenity/plugins/websocket.py
-drwxr-xr-x   0 localghost  (1000) localghost  (1000)        0 2023-07-31 21:39:24.672329 evenity-0.0.8/src/evenity.egg-info/
--rw-r--r--   0 localghost  (1000) localghost  (1000)     7703 2023-07-31 21:39:24.000000 evenity-0.0.8/src/evenity.egg-info/PKG-INFO
--rw-r--r--   0 localghost  (1000) localghost  (1000)      449 2023-07-31 21:39:24.000000 evenity-0.0.8/src/evenity.egg-info/SOURCES.txt
--rw-r--r--   0 localghost  (1000) localghost  (1000)        1 2023-07-31 21:39:24.000000 evenity-0.0.8/src/evenity.egg-info/dependency_links.txt
--rw-r--r--   0 localghost  (1000) localghost  (1000)        8 2023-07-31 21:39:24.000000 evenity-0.0.8/src/evenity.egg-info/top_level.txt
-drwxr-xr-x   0 localghost  (1000) localghost  (1000)        0 2023-07-31 21:39:24.672329 evenity-0.0.8/tests/
--rw-r--r--   0 localghost  (1000) localghost  (1000)     1105 2023-07-31 21:38:27.000000 evenity-0.0.8/tests/test_simple.py
+drwxr-xr-x   0 localghost  (1000) localghost  (1000)        0 2023-07-31 22:11:33.722782 evenity-0.0.9/
+-rw-r--r--   0 localghost  (1000) localghost  (1000)        0 2023-07-28 21:02:20.000000 evenity-0.0.9/LICENSE
+-rw-r--r--   0 localghost  (1000) localghost  (1000)     7703 2023-07-31 22:11:33.722782 evenity-0.0.9/PKG-INFO
+-rw-r--r--   0 localghost  (1000) localghost  (1000)     7248 2023-07-31 21:11:07.000000 evenity-0.0.9/README.md
+-rw-r--r--   0 localghost  (1000) localghost  (1000)      532 2023-07-31 22:11:24.000000 evenity-0.0.9/pyproject.toml
+-rw-r--r--   0 localghost  (1000) localghost  (1000)       38 2023-07-31 22:11:33.722782 evenity-0.0.9/setup.cfg
+drwxr-xr-x   0 localghost  (1000) localghost  (1000)        0 2023-07-31 22:11:33.719449 evenity-0.0.9/src/
+drwxr-xr-x   0 localghost  (1000) localghost  (1000)        0 2023-07-31 22:11:33.719449 evenity-0.0.9/src/evenity/
+-rw-r--r--   0 localghost  (1000) localghost  (1000)        0 2023-07-28 23:22:35.000000 evenity-0.0.9/src/evenity/__init__.py
+-rw-r--r--   0 localghost  (1000) localghost  (1000)      528 2023-07-31 22:09:35.000000 evenity-0.0.9/src/evenity/observable.py
+-rw-r--r--   0 localghost  (1000) localghost  (1000)      919 2023-07-31 22:09:35.000000 evenity-0.0.9/src/evenity/observer.py
+drwxr-xr-x   0 localghost  (1000) localghost  (1000)        0 2023-07-31 22:11:33.722782 evenity-0.0.9/src/evenity/plugins/
+-rw-r--r--   0 localghost  (1000) localghost  (1000)        0 2023-07-28 23:22:35.000000 evenity-0.0.9/src/evenity/plugins/__init__.py
+-rw-r--r--   0 localghost  (1000) localghost  (1000)     1451 2023-07-31 21:11:07.000000 evenity-0.0.9/src/evenity/plugins/ftp.py
+-rw-r--r--   0 localghost  (1000) localghost  (1000)      714 2023-07-28 23:22:35.000000 evenity-0.0.9/src/evenity/plugins/kafka.py
+-rw-r--r--   0 localghost  (1000) localghost  (1000)      632 2023-07-28 23:22:35.000000 evenity-0.0.9/src/evenity/plugins/shell.py
+-rw-r--r--   0 localghost  (1000) localghost  (1000)      742 2023-07-31 21:11:07.000000 evenity-0.0.9/src/evenity/plugins/telegram.py
+-rw-r--r--   0 localghost  (1000) localghost  (1000)     1741 2023-07-30 17:27:26.000000 evenity-0.0.9/src/evenity/plugins/websocket.py
+drwxr-xr-x   0 localghost  (1000) localghost  (1000)        0 2023-07-31 22:11:33.719449 evenity-0.0.9/src/evenity.egg-info/
+-rw-r--r--   0 localghost  (1000) localghost  (1000)     7703 2023-07-31 22:11:33.000000 evenity-0.0.9/src/evenity.egg-info/PKG-INFO
+-rw-r--r--   0 localghost  (1000) localghost  (1000)      449 2023-07-31 22:11:33.000000 evenity-0.0.9/src/evenity.egg-info/SOURCES.txt
+-rw-r--r--   0 localghost  (1000) localghost  (1000)        1 2023-07-31 22:11:33.000000 evenity-0.0.9/src/evenity.egg-info/dependency_links.txt
+-rw-r--r--   0 localghost  (1000) localghost  (1000)        8 2023-07-31 22:11:33.000000 evenity-0.0.9/src/evenity.egg-info/top_level.txt
+drwxr-xr-x   0 localghost  (1000) localghost  (1000)        0 2023-07-31 22:11:33.722782 evenity-0.0.9/tests/
+-rw-r--r--   0 localghost  (1000) localghost  (1000)     1105 2023-07-31 21:38:27.000000 evenity-0.0.9/tests/test_simple.py
```

### Comparing `evenity-0.0.8/PKG-INFO` & `evenity-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evenity
-Version: 0.0.8
+Version: 0.0.9
 Summary: Pluggable event hooks library
 Author-email: Mario Baldi <mariobaldi.py@gmail.com>
 Project-URL: Homepage, https://github.com/baldimario/evenity
 Project-URL: Bug Tracker, https://github.com/baldimario/evenity/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
```

### Comparing `evenity-0.0.8/README.md` & `evenity-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `evenity-0.0.8/pyproject.toml` & `evenity-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["setuptools>=42"]
 
 [project]
 name = "evenity"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Mario Baldi", email="mariobaldi.py@gmail.com" },
 ]
 description = "Pluggable event hooks library"
 readme = "README.md"
 requires-python = ">=3.5"
 classifiers = [
```

### Comparing `evenity-0.0.8/src/evenity/observer.py` & `evenity-0.0.9/src/evenity/observable.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,20 @@
-"""Observer class"""
+"""Ovservable class"""
 
-class Observer:
-    """Observer class"""
+class Observable:
+    """Observable class"""
 
-    def __init__(self, observable):
-        self._listeners = {}
-        self.observable = observable
-        self.register(observable)
+    def __init__(self):
+        self._observers = []
 
-    def register(self, observable):
-        """Register to an observable"""
-        observable.register_observer(self)
-
-    def notify(self, listener, event):
-        """Notify the observer"""
-        if listener in self._listeners:
-            self._listeners[listener](event)
-
-    def listen(self, event, callback):
-        """Listen to an event"""
-        self._listeners[event] = callback
-
-class SimpleObserver(Observer):
-    """SimpleObserver class"""
-
-    def __init__(self, observable, callback_lookup):
-        super().__init__(observable)
-        for event, callback in callback_lookup.items():
-            self.listen(event, callback)
+    def register_observer(self, observer):
+        """Register an observer"""
+        self._observers.append(observer)
+
+    def unregister_observer(self, observer):
+        """Unregister an observer"""
+        self._observers.remove(observer)
+
+    def notify_observers(self, listener, event):
+        """Notify all observers"""
+        for obs in self._observers:
+            obs.notify(listener, event)
```

### Comparing `evenity-0.0.8/src/evenity/plugins/ftp.py` & `evenity-0.0.9/src/evenity/plugins/ftp.py`

 * *Files identical despite different names*

### Comparing `evenity-0.0.8/src/evenity/plugins/kafka.py` & `evenity-0.0.9/src/evenity/plugins/kafka.py`

 * *Files identical despite different names*

### Comparing `evenity-0.0.8/src/evenity/plugins/shell.py` & `evenity-0.0.9/src/evenity/plugins/shell.py`

 * *Files identical despite different names*

### Comparing `evenity-0.0.8/src/evenity/plugins/telegram.py` & `evenity-0.0.9/src/evenity/plugins/telegram.py`

 * *Files identical despite different names*

### Comparing `evenity-0.0.8/src/evenity/plugins/websocket.py` & `evenity-0.0.9/src/evenity/plugins/websocket.py`

 * *Files identical despite different names*

### Comparing `evenity-0.0.8/src/evenity.egg-info/PKG-INFO` & `evenity-0.0.9/src/evenity.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evenity
-Version: 0.0.8
+Version: 0.0.9
 Summary: Pluggable event hooks library
 Author-email: Mario Baldi <mariobaldi.py@gmail.com>
 Project-URL: Homepage, https://github.com/baldimario/evenity
 Project-URL: Bug Tracker, https://github.com/baldimario/evenity/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
```

### Comparing `evenity-0.0.8/tests/test_simple.py` & `evenity-0.0.9/tests/test_simple.py`

 * *Files identical despite different names*

