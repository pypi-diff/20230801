# Comparing `tmp/kioss-0.2.4.tar.gz` & `tmp/kioss-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kioss-0.2.4.tar", last modified: Tue Aug  1 00:06:56 2023, max compression
+gzip compressed data, was "kioss-0.2.5.tar", last modified: Tue Aug  1 01:45:17 2023, max compression
```

## Comparing `kioss-0.2.4.tar` & `kioss-0.2.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:06:56.626949 kioss-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-01 00:06:44.000000 kioss-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-08-01 00:06:56.626949 kioss-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-08-01 00:06:44.000000 kioss-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:06:56.622949 kioss-0.2.4/kioss/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-01 00:06:44.000000 kioss-0.2.4/kioss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18474 2023-08-01 00:06:44.000000 kioss-0.2.4/kioss/pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-08-01 00:06:44.000000 kioss-0.2.4/kioss/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:06:56.622949 kioss-0.2.4/kioss.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-08-01 00:06:56.000000 kioss-0.2.4/kioss.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-08-01 00:06:56.000000 kioss-0.2.4/kioss.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 00:06:56.000000 kioss-0.2.4/kioss.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-01 00:06:56.000000 kioss-0.2.4/kioss.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 00:06:56.626949 kioss-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-08-01 00:06:44.000000 kioss-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:06:56.622949 kioss-0.2.4/test/
--rw-r--r--   0 runner    (1001) docker     (123)    11258 2023-08-01 00:06:44.000000 kioss-0.2.4/test/test_pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-08-01 00:06:44.000000 kioss-0.2.4/test/test_util.py
+drwxr-xr-x   0 bonnal-enzo   (501) staff       (20)        0 2023-08-01 01:45:17.773019 kioss-0.2.5/
+-rw-r--r--   0 bonnal-enzo   (501) staff       (20)    11357 2023-07-25 20:06:24.000000 kioss-0.2.5/LICENSE
+-rw-r--r--   0 bonnal-enzo   (501) staff       (20)      339 2023-08-01 01:45:17.772840 kioss-0.2.5/PKG-INFO
+-rw-r--r--   0 bonnal-enzo   (501) staff       (20)     4331 2023-07-31 23:49:05.000000 kioss-0.2.5/README.md
+drwxr-xr-x   0 bonnal-enzo   (501) staff       (20)        0 2023-08-01 01:45:17.771363 kioss-0.2.5/kioss/
+-rw-r--r--   0 bonnal-enzo   (501) staff       (20)       28 2023-07-25 20:06:24.000000 kioss-0.2.5/kioss/__init__.py
+-rw-r--r--   0 bonnal-enzo   (501) staff       (20)    18408 2023-08-01 01:40:58.000000 kioss-0.2.5/kioss/pipe.py
+-rw-r--r--   0 bonnal-enzo   (501) staff       (20)     1058 2023-07-31 23:38:59.000000 kioss-0.2.5/kioss/util.py
+drwxr-xr-x   0 bonnal-enzo   (501) staff       (20)        0 2023-08-01 01:45:17.772086 kioss-0.2.5/kioss.egg-info/
+-rw-r--r--   0 bonnal-enzo   (501) staff       (20)      339 2023-08-01 01:45:17.000000 kioss-0.2.5/kioss.egg-info/PKG-INFO
+-rw-r--r--   0 bonnal-enzo   (501) staff       (20)      224 2023-08-01 01:45:17.000000 kioss-0.2.5/kioss.egg-info/SOURCES.txt
+-rw-r--r--   0 bonnal-enzo   (501) staff       (20)        1 2023-08-01 01:45:17.000000 kioss-0.2.5/kioss.egg-info/dependency_links.txt
+-rw-r--r--   0 bonnal-enzo   (501) staff       (20)        6 2023-08-01 01:45:17.000000 kioss-0.2.5/kioss.egg-info/top_level.txt
+-rw-r--r--   0 bonnal-enzo   (501) staff       (20)       38 2023-08-01 01:45:17.773062 kioss-0.2.5/setup.cfg
+-rw-r--r--   0 bonnal-enzo   (501) staff       (20)      369 2023-08-01 01:41:59.000000 kioss-0.2.5/setup.py
+drwxr-xr-x   0 bonnal-enzo   (501) staff       (20)        0 2023-08-01 01:45:17.772454 kioss-0.2.5/test/
+-rw-r--r--   0 bonnal-enzo   (501) staff       (20)    11274 2023-08-01 01:42:22.000000 kioss-0.2.5/test/test_pipe.py
+-rw-r--r--   0 bonnal-enzo   (501) staff       (20)      578 2023-07-31 23:33:35.000000 kioss-0.2.5/test/test_util.py
```

### Comparing `kioss-0.2.4/LICENSE` & `kioss-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `kioss-0.2.4/README.md` & `kioss-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `kioss-0.2.4/kioss/pipe.py` & `kioss-0.2.5/kioss/pipe.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,30 @@
 import itertools
 import logging
 import multiprocessing
 import pickle
 import time
 import timeit
-from concurrent.futures import (Executor, ProcessPoolExecutor,
-                                ThreadPoolExecutor)
+from concurrent.futures import Executor, ProcessPoolExecutor, ThreadPoolExecutor
 from datetime import datetime
 from multiprocessing.synchronize import Event
 from queue import Empty, Full, Queue
-from typing import (Any, Callable, Generic, Iterable, Iterator, List, Optional,
-                    Tuple, Type, TypeVar, Union)
+from typing import (
+    Any,
+    Callable,
+    Generic,
+    Iterable,
+    Iterator,
+    List,
+    Optional,
+    Tuple,
+    Type,
+    TypeVar,
+    Union,
+)
 
 import kioss.util as util
 
 T = TypeVar("T")
 R = TypeVar("R")
 
 
@@ -31,15 +41,15 @@
 
     Attributes:
         iterator (Iterator[T]): The iterator containing elements for the pipeline.
     """
 
     def __init__(self, source: Union[Iterable[T], Iterator[T]] = []) -> None:  # timeout
         self.iterator: Iterator[T] = iter(source)
-        self._exit_asked: Event = self._MANAGER.Event()
+        self._exit_asked: Event = multiprocessing.Event()
 
     def __next__(self) -> T:
         return next(self.iterator)
 
     def __iter__(self) -> T:
         return self
 
@@ -54,20 +64,18 @@
         if isinstance(self.iterator, Pipe):
             return self.iterator.__exit__(exc_type, exc_value, traceback)
         return False
 
     THREAD_WORKER_TYPE = "thread"
     PROCESS_WORKER_TYPE = "process"
 
-    SUPPORTED_WORKER_TYPES = [THREAD_WORKER_TYPE, PROCESS_WORKER_TYPE]
+    SUPPORTED_WORKER_TYPES = [THREAD_WORKER_TYPE]
 
     _MAX_NUM_WAITING_ELEMS_PER_THREAD = 16
 
-    _MANAGER = multiprocessing.Manager()
-
     def _map_or_do(
         self,
         func: Callable[[T], R],
         n_workers: Optional[int],
         worker_type: str,
         sidify: bool,
     ) -> "Pipe[Union[R, T]]":
@@ -87,15 +95,15 @@
                     func,
                     self,
                     executor_class=ThreadPoolExecutor
                     if worker_type == self.THREAD_WORKER_TYPE
                     else ProcessPoolExecutor,
                     queue_class=Queue
                     if worker_type == self.THREAD_WORKER_TYPE
-                    else self._MANAGER.Queue,
+                    else multiprocessing.Queue,
                     n_workers=n_workers,
                     max_queue_size=self._MAX_NUM_WAITING_ELEMS_PER_THREAD * n_workers,
                     sidify=sidify,
                     exit_asked=self._exit_asked,
                 )
             )
         )
```

### Comparing `kioss-0.2.4/kioss/util.py` & `kioss-0.2.5/kioss/util.py`

 * *Files identical despite different names*

### Comparing `kioss-0.2.4/test/test_pipe.py` & `kioss-0.2.5/test/test_pipe.py`

 * *Files 4% similar despite different names*

```diff
@@ -134,22 +134,22 @@
         pipe = Pipe(range(N)).map(ten_millis_identity, n_workers=n_workers)
         self.assertAlmostEqual(
             pipe.time(),
             TEN_MS * N / n_workers,
             delta=0.3 * (TEN_MS * N) / n_workers,
         )
 
-    def test__apply(self):
-        self.assertRaisesRegex(
-            AttributeError,
-            r"Can't pickle local object 'TestPipe\.test__apply\.<locals>\.<lambda>\.<locals>\.<lambda>'",
-            lambda: Pipe([]).map(
-                lambda x: x, n_workers=1, worker_type=Pipe.PROCESS_WORKER_TYPE
-            ),
-        )
+    # def test_map_or_do(self):
+    #     self.assertRaisesRegex(
+    #         AttributeError,
+    #         r"Can't pickle local object 'TestPipe\.test__apply\.<locals>\.<lambda>\.<locals>\.<lambda>'",
+    #         lambda: Pipe([]).map(
+    #             lambda x: x, n_workers=1, worker_type=Pipe.THREAD_WORKER_TYPE
+    #         ),
+    #     )
 
     def test_do(self):
         l: List[int] = []
 
         func = lambda x: x**2
 
         def func_with_side_effect(x):
@@ -172,15 +172,15 @@
         while len(non_local_l):
             non_local_l.pop()
         self.assertSetEqual(
             set(
                 Pipe(args).do(
                     non_local_func_with_side_effect,
                     n_workers=2,
-                    worker_type=Pipe.PROCESS_WORKER_TYPE,
+                    worker_type=Pipe.THREAD_WORKER_TYPE,
                 )
             ),
             set(args),
         )
         self.assertSetEqual(set(l), set(map(func, args)))
 
         # with_processes and with slow upstream
@@ -189,15 +189,15 @@
         self.assertSetEqual(
             set(
                 Pipe(range(N))
                 .map(ten_millis_identity)
                 .do(
                     non_local_func_with_side_effect,
                     n_workers=8,
-                    worker_type=Pipe.PROCESS_WORKER_TYPE,
+                    worker_type=Pipe.THREAD_WORKER_TYPE,
                 )
             ),
             set(range(N)),
         )
         self.assertSetEqual(set(l), set(map(func, args)))
 
     def test_flatten(self):
```

### Comparing `kioss-0.2.4/test/test_util.py` & `kioss-0.2.5/test/test_util.py`

 * *Files identical despite different names*

