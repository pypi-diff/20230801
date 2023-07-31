# Comparing `tmp/kioss-0.2.1.tar.gz` & `tmp/kioss-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kioss-0.2.1.tar", last modified: Mon Jul 31 23:31:09 2023, max compression
+gzip compressed data, was "kioss-0.2.2.tar", last modified: Mon Jul 31 23:39:46 2023, max compression
```

## Comparing `kioss-0.2.1.tar` & `kioss-0.2.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 23:31:09.500140 kioss-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-31 23:30:53.000000 kioss-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-31 23:31:09.500140 kioss-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-07-31 23:30:53.000000 kioss-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 23:31:09.500140 kioss-0.2.1/kioss/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-31 23:30:53.000000 kioss-0.2.1/kioss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19401 2023-07-31 23:30:53.000000 kioss-0.2.1/kioss/pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-31 23:30:53.000000 kioss-0.2.1/kioss/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 23:31:09.500140 kioss-0.2.1/kioss.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-31 23:31:09.000000 kioss-0.2.1/kioss.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-31 23:31:09.000000 kioss-0.2.1/kioss.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 23:31:09.000000 kioss-0.2.1/kioss.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-31 23:31:09.000000 kioss-0.2.1/kioss.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 23:31:09.500140 kioss-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-31 23:30:53.000000 kioss-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 23:31:09.500140 kioss-0.2.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)    11211 2023-07-31 23:30:53.000000 kioss-0.2.1/test/test_pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-31 23:30:53.000000 kioss-0.2.1/test/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 23:39:46.481510 kioss-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-31 23:39:34.000000 kioss-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-31 23:39:46.481510 kioss-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-07-31 23:39:34.000000 kioss-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 23:39:46.481510 kioss-0.2.2/kioss/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-31 23:39:34.000000 kioss-0.2.2/kioss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19423 2023-07-31 23:39:34.000000 kioss-0.2.2/kioss/pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-31 23:39:34.000000 kioss-0.2.2/kioss/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 23:39:46.481510 kioss-0.2.2/kioss.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-31 23:39:46.000000 kioss-0.2.2/kioss.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-31 23:39:46.000000 kioss-0.2.2/kioss.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 23:39:46.000000 kioss-0.2.2/kioss.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-31 23:39:46.000000 kioss-0.2.2/kioss.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 23:39:46.481510 kioss-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-31 23:39:34.000000 kioss-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 23:39:46.481510 kioss-0.2.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    11211 2023-07-31 23:39:34.000000 kioss-0.2.2/test/test_pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-31 23:39:34.000000 kioss-0.2.2/test/test_util.py
```

### Comparing `kioss-0.2.1/LICENSE` & `kioss-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kioss-0.2.1/README.md` & `kioss-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `kioss-0.2.1/kioss/pipe.py` & `kioss-0.2.2/kioss/pipe.py`

 * *Files 0% similar despite different names*

```diff
@@ -359,22 +359,23 @@
             self.errors_count,
         )
 
     def __next__(self) -> T:
         try:
             elem = super().__next__()
         except StopIteration:
-            self._log()
+            if self.yields_count % 2:
+                self._log()
             raise
 
         self.yields_count += 1
         if isinstance(elem, Exception):
             self.errors_count += 1
 
-        if self.yields_count + self.errors_count >= 2 * self.last_log_at_yields_count:
+        if self.yields_count >= 2 * self.last_log_at_yields_count:
             self._log()
             self.last_log_at_yields_count = self.yields_count + self.errors_count
 
         return elem
 
 
 class _SlowingPipe(Pipe[T]):
```

### Comparing `kioss-0.2.1/kioss/util.py` & `kioss-0.2.2/kioss/util.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-import time
-import uuid
 from queue import Empty, Queue
-from typing import Any, Callable, Iterable, Iterator, Optional, TypeVar, Union
+from typing import Any, Callable, Iterable, Iterator, TypeVar, Union
 
 T = TypeVar("T")
 
 
 def sidify(func: Callable[[T], Any]) -> Callable[[T], T]:
     def wrap(arg):
         func(arg)
@@ -19,37 +17,29 @@
         pass
 
 
 def identity(obj: T) -> T:
     return obj
 
 
-_SENTINEL = (
-    "kioss.util.QueueIterator's Sentinel String -> "
-    + str(uuid.uuid4())
-    + "-"
-    + str(time.time())
-)
-
-
 class QueueIterator(Iterator[T]):
-    SENTINEL = _SENTINEL
     INITIAL_BACKOFF_SECS = 0.005
 
-    def __init__(self, queue: Queue) -> None:
+    def __init__(self, queue: Queue, sentinel: Any) -> None:
         self.queue = queue
+        self.sentinel = sentinel
         self.backoff = QueueIterator.INITIAL_BACKOFF_SECS
 
     def __iter__(self) -> Iterator[T]:
         return self
 
     def __next__(self) -> T:
         try:
             elem = self.queue.get(timeout=self.backoff)
             self.backoff = self.INITIAL_BACKOFF_SECS
         except Empty:
             self.backoff *= 2
             return next(self)
-        if elem == self.SENTINEL:
-            self.queue.put(self.SENTINEL)
+        if elem == self.sentinel:
+            self.queue.put(self.sentinel)
             raise StopIteration()
         return elem
```

### Comparing `kioss-0.2.1/test/test_pipe.py` & `kioss-0.2.2/test/test_pipe.py`

 * *Files identical despite different names*

### Comparing `kioss-0.2.1/test/test_util.py` & `kioss-0.2.2/test/test_util.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,12 +14,12 @@
         def f(x):
             return x**2
 
         self.assertEqual(f(2), 2)
 
     def test_queue_iterator(self):
         queue = Queue()
-        it = QueueIterator(queue)
+        it = QueueIterator(queue, None)
         for i in range(8):
             queue.put(i)
-        queue.put(QueueIterator.SENTINEL)
+        queue.put(None)
         self.assertListEqual(list(it), list(range(8)))
```

