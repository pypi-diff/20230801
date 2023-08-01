# Comparing `tmp/kioss-0.2.5.tar.gz` & `tmp/kioss-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kioss-0.2.5.tar", last modified: Tue Aug  1 01:45:17 2023, max compression
+gzip compressed data, was "kioss-0.2.6.tar", last modified: Tue Aug  1 05:31:55 2023, max compression
```

## Comparing `kioss-0.2.5.tar` & `kioss-0.2.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 bonnal-enzo   (501) staff       (20)        0 2023-08-01 01:45:17.773019 kioss-0.2.5/
--rw-r--r--   0 bonnal-enzo   (501) staff       (20)    11357 2023-07-25 20:06:24.000000 kioss-0.2.5/LICENSE
--rw-r--r--   0 bonnal-enzo   (501) staff       (20)      339 2023-08-01 01:45:17.772840 kioss-0.2.5/PKG-INFO
--rw-r--r--   0 bonnal-enzo   (501) staff       (20)     4331 2023-07-31 23:49:05.000000 kioss-0.2.5/README.md
-drwxr-xr-x   0 bonnal-enzo   (501) staff       (20)        0 2023-08-01 01:45:17.771363 kioss-0.2.5/kioss/
--rw-r--r--   0 bonnal-enzo   (501) staff       (20)       28 2023-07-25 20:06:24.000000 kioss-0.2.5/kioss/__init__.py
--rw-r--r--   0 bonnal-enzo   (501) staff       (20)    18408 2023-08-01 01:40:58.000000 kioss-0.2.5/kioss/pipe.py
--rw-r--r--   0 bonnal-enzo   (501) staff       (20)     1058 2023-07-31 23:38:59.000000 kioss-0.2.5/kioss/util.py
-drwxr-xr-x   0 bonnal-enzo   (501) staff       (20)        0 2023-08-01 01:45:17.772086 kioss-0.2.5/kioss.egg-info/
--rw-r--r--   0 bonnal-enzo   (501) staff       (20)      339 2023-08-01 01:45:17.000000 kioss-0.2.5/kioss.egg-info/PKG-INFO
--rw-r--r--   0 bonnal-enzo   (501) staff       (20)      224 2023-08-01 01:45:17.000000 kioss-0.2.5/kioss.egg-info/SOURCES.txt
--rw-r--r--   0 bonnal-enzo   (501) staff       (20)        1 2023-08-01 01:45:17.000000 kioss-0.2.5/kioss.egg-info/dependency_links.txt
--rw-r--r--   0 bonnal-enzo   (501) staff       (20)        6 2023-08-01 01:45:17.000000 kioss-0.2.5/kioss.egg-info/top_level.txt
--rw-r--r--   0 bonnal-enzo   (501) staff       (20)       38 2023-08-01 01:45:17.773062 kioss-0.2.5/setup.cfg
--rw-r--r--   0 bonnal-enzo   (501) staff       (20)      369 2023-08-01 01:41:59.000000 kioss-0.2.5/setup.py
-drwxr-xr-x   0 bonnal-enzo   (501) staff       (20)        0 2023-08-01 01:45:17.772454 kioss-0.2.5/test/
--rw-r--r--   0 bonnal-enzo   (501) staff       (20)    11274 2023-08-01 01:42:22.000000 kioss-0.2.5/test/test_pipe.py
--rw-r--r--   0 bonnal-enzo   (501) staff       (20)      578 2023-07-31 23:33:35.000000 kioss-0.2.5/test/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 05:31:55.160259 kioss-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-01 05:31:46.000000 kioss-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-08-01 05:31:55.160259 kioss-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-08-01 05:31:46.000000 kioss-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 05:31:55.160259 kioss-0.2.6/kioss/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-01 05:31:46.000000 kioss-0.2.6/kioss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18761 2023-08-01 05:31:46.000000 kioss-0.2.6/kioss/pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-08-01 05:31:46.000000 kioss-0.2.6/kioss/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 05:31:55.160259 kioss-0.2.6/kioss.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-08-01 05:31:55.000000 kioss-0.2.6/kioss.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-08-01 05:31:55.000000 kioss-0.2.6/kioss.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 05:31:55.000000 kioss-0.2.6/kioss.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-01 05:31:55.000000 kioss-0.2.6/kioss.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 05:31:55.160259 kioss-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-08-01 05:31:46.000000 kioss-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 05:31:55.160259 kioss-0.2.6/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    11258 2023-08-01 05:31:46.000000 kioss-0.2.6/test/test_pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-08-01 05:31:46.000000 kioss-0.2.6/test/test_util.py
```

### Comparing `kioss-0.2.5/LICENSE` & `kioss-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `kioss-0.2.5/README.md` & `kioss-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `kioss-0.2.5/kioss/pipe.py` & `kioss-0.2.6/kioss/pipe.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,69 +41,80 @@
 
     Attributes:
         iterator (Iterator[T]): The iterator containing elements for the pipeline.
     """
 
     def __init__(self, source: Union[Iterable[T], Iterator[T]] = []) -> None:  # timeout
         self.iterator: Iterator[T] = iter(source)
-        self._exit_asked: Event = multiprocessing.Event()
+        self._exit_asked: Optional[Event] = None
 
     def __next__(self) -> T:
         return next(self.iterator)
 
     def __iter__(self) -> T:
         return self
 
     def __add__(self, other: "Pipe[T]") -> "Pipe[T]":
         return self.chain(other)
 
     def __enter__(self) -> "Pipe[T]":
         return self
 
     def __exit__(self, exc_type, exc_value, traceback) -> bool:
-        self._exit_asked.set()
+        if self._exit_asked is not None:
+            self._exit_asked.set()
         if isinstance(self.iterator, Pipe):
             return self.iterator.__exit__(exc_type, exc_value, traceback)
         return False
 
     THREAD_WORKER_TYPE = "thread"
     PROCESS_WORKER_TYPE = "process"
 
-    SUPPORTED_WORKER_TYPES = [THREAD_WORKER_TYPE]
+    SUPPORTED_WORKER_TYPES = [THREAD_WORKER_TYPE, PROCESS_WORKER_TYPE]
 
     _MAX_NUM_WAITING_ELEMS_PER_THREAD = 16
 
+    _MANAGER: Optional[multiprocessing.Manager] = None
+
     def _map_or_do(
         self,
         func: Callable[[T], R],
         n_workers: Optional[int],
         worker_type: str,
         sidify: bool,
     ) -> "Pipe[Union[R, T]]":
         if worker_type not in self.SUPPORTED_WORKER_TYPES:
             raise ValueError(
                 f"'{worker_type}' worker_type is not supported, must be one of: {self.SUPPORTED_WORKER_TYPES}"
             )
+
         if n_workers is None or n_workers <= 0:
             if sidify:
                 func = util.sidify(func)
             return Pipe[T](map(func, self))
+
         if worker_type == Pipe.PROCESS_WORKER_TYPE:
             pickle.dumps(func)
+            if Pipe._MANAGER is None:
+                Pipe._MANAGER = multiprocessing.Manager()
+            self._exit_asked = Pipe._MANAGER.Event()
+            queue_class: Type[Queue] = Pipe._MANAGER.Queue
+            executor_class: Type[Executor] = ProcessPoolExecutor
+        else:
+            self._exit_asked = multiprocessing.Event()
+            queue_class: Type[Queue] = Queue
+            executor_class: Type[Executor] = ThreadPoolExecutor
+
         return _RasingPipe[T](
             iter(
                 _multi_yielding_iterable(
                     func,
                     self,
-                    executor_class=ThreadPoolExecutor
-                    if worker_type == self.THREAD_WORKER_TYPE
-                    else ProcessPoolExecutor,
-                    queue_class=Queue
-                    if worker_type == self.THREAD_WORKER_TYPE
-                    else multiprocessing.Queue,
+                    executor_class=executor_class,
+                    queue_class=queue_class,
                     n_workers=n_workers,
                     max_queue_size=self._MAX_NUM_WAITING_ELEMS_PER_THREAD * n_workers,
                     sidify=sidify,
                     exit_asked=self._exit_asked,
                 )
             )
         )
```

### Comparing `kioss-0.2.5/kioss/util.py` & `kioss-0.2.6/kioss/util.py`

 * *Files identical despite different names*

### Comparing `kioss-0.2.5/test/test_pipe.py` & `kioss-0.2.6/test/test_pipe.py`

 * *Files 4% similar despite different names*

```diff
@@ -134,22 +134,22 @@
         pipe = Pipe(range(N)).map(ten_millis_identity, n_workers=n_workers)
         self.assertAlmostEqual(
             pipe.time(),
             TEN_MS * N / n_workers,
             delta=0.3 * (TEN_MS * N) / n_workers,
         )
 
-    # def test_map_or_do(self):
-    #     self.assertRaisesRegex(
-    #         AttributeError,
-    #         r"Can't pickle local object 'TestPipe\.test__apply\.<locals>\.<lambda>\.<locals>\.<lambda>'",
-    #         lambda: Pipe([]).map(
-    #             lambda x: x, n_workers=1, worker_type=Pipe.THREAD_WORKER_TYPE
-    #         ),
-    #     )
+    def test__apply(self):
+        self.assertRaisesRegex(
+            AttributeError,
+            r"Can't pickle local object 'TestPipe\.test__apply\.<locals>\.<lambda>\.<locals>\.<lambda>'",
+            lambda: Pipe([]).map(
+                lambda x: x, n_workers=1, worker_type=Pipe.PROCESS_WORKER_TYPE
+            ),
+        )
 
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
-                    worker_type=Pipe.THREAD_WORKER_TYPE,
+                    worker_type=Pipe.PROCESS_WORKER_TYPE,
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
-                    worker_type=Pipe.THREAD_WORKER_TYPE,
+                    worker_type=Pipe.PROCESS_WORKER_TYPE,
                 )
             ),
             set(range(N)),
         )
         self.assertSetEqual(set(l), set(map(func, args)))
 
     def test_flatten(self):
```

### Comparing `kioss-0.2.5/test/test_util.py` & `kioss-0.2.6/test/test_util.py`

 * *Files identical despite different names*

