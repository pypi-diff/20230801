# Comparing `tmp/kioss-0.1.2.tar.gz` & `tmp/kioss-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kioss-0.1.2.tar", last modified: Fri Jul 28 08:04:24 2023, max compression
+gzip compressed data, was "kioss-0.2.0.tar", last modified: Mon Jul 31 23:25:17 2023, max compression
```

## Comparing `kioss-0.1.2.tar` & `kioss-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:04:24.840126 kioss-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-28 08:04:14.000000 kioss-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-28 08:04:24.840126 kioss-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-07-28 08:04:14.000000 kioss-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:04:24.840126 kioss-0.1.2/kioss/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-28 08:04:14.000000 kioss-0.1.2/kioss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15118 2023-07-28 08:04:14.000000 kioss-0.1.2/kioss/pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-28 08:04:14.000000 kioss-0.1.2/kioss/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:04:24.840126 kioss-0.1.2/kioss.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-28 08:04:24.000000 kioss-0.1.2/kioss.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-28 08:04:24.000000 kioss-0.1.2/kioss.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 08:04:24.000000 kioss-0.1.2/kioss.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-28 08:04:24.000000 kioss-0.1.2/kioss.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 08:04:24.840126 kioss-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-28 08:04:14.000000 kioss-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:04:24.840126 kioss-0.1.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)     8574 2023-07-28 08:04:14.000000 kioss-0.1.2/test/test_pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-28 08:04:14.000000 kioss-0.1.2/test/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 23:25:17.564279 kioss-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-31 23:25:07.000000 kioss-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-31 23:25:17.564279 kioss-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-07-31 23:25:07.000000 kioss-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 23:25:17.564279 kioss-0.2.0/kioss/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-31 23:25:07.000000 kioss-0.2.0/kioss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19401 2023-07-31 23:25:07.000000 kioss-0.2.0/kioss/pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-31 23:25:07.000000 kioss-0.2.0/kioss/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 23:25:17.564279 kioss-0.2.0/kioss.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-31 23:25:17.000000 kioss-0.2.0/kioss.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-31 23:25:17.000000 kioss-0.2.0/kioss.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 23:25:17.000000 kioss-0.2.0/kioss.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-31 23:25:17.000000 kioss-0.2.0/kioss.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 23:25:17.564279 kioss-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-31 23:25:07.000000 kioss-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 23:25:17.564279 kioss-0.2.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    12002 2023-07-31 23:25:07.000000 kioss-0.2.0/test/test_pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-31 23:25:07.000000 kioss-0.2.0/test/test_util.py
```

### Comparing `kioss-0.1.2/LICENSE` & `kioss-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kioss-0.1.2/README.md` & `kioss-0.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -49,41 +49,42 @@
         .flatten()
         # log the advancement of this step
         .log(objects_description="parsed email domains deduplicated by batch")
 
         # construct url from email domain
         .map(lambda email_domain: f"https://{email_domain}")
         # sent GET requests to urls, using 2 threads for better I/O
-        .map(requests.get, n_threads=2)
+        .map(requests.get, n_workers=2)
         # limit requests to roughly 20 requests sent by second to avoid spam
         .slow(freq=20)
         # catch request errors without ignoring them this time:
         # it means that the pipeline will yield the exception object encountered instead of raising it
         .catch(requests.RequestException, ignore=False)
         # log the advancement of this step
         .log(objects_description="domain responses")
 
         # get only errors, i.e. non-200 status codes or request exceptions (yielded by upstream because ignore=False)
         .filter(lambda reponse: isinstance(reponse, requests.RequestException) or reponse.status_code != 200)
         # iterate over the entire pipe but only store the 32 first errors
-        .collect(limit=32) 
+        .collect(n_samples=32) 
     ):
         raise RuntimeError(f"Encountered unreachable domains, samples: {unreachable_domain_samples}")
 ```
 
 ## Features
-- mutate
-    - `.mix` several pipes to form a new one that yields elements concurrently as they arrive, using multiple threads.
-    - `.chain` several pipes to form a new one that yields elements of one pipe after the previous one is exhausted.
-    - `.map` over pipe's elements and yield the results as they arrive, using multiple threads.
+- define:
+    - `Pipe`'s constructor takes an `Iterator[T]` or `Iterable[T]` object as data source, and the constructed pipe object is itself an `Iterator[T]` on which you can call any function working with iterators: `set`, `functools.reduce`, etc...
+    - `.map` over pipe's elements and yield the results as they arrive, optionally using multiple threads.
     - `.flatten` a pipe, whose elements are assumed to be iterators, creating a new pipe with individual elements.
     - `.filter` a pipe.
+    - `.do` side effects on a pipe, optionally using multiple threads or processes.
+    - `.chain` several pipes to form a new one that yields elements of one pipe after the previous one is exhausted.
+    - `.mix` several pipes to form a new one that yields elements concurrently as they arrive, using multiple threads.
     - `.batch` pipe's elements and yield them as lists of a given max size or spanning over a given max period.
-- control
+- control:
+    - `.slow` a pipe to limit the iteration's speed over it.
     - `.log` a pipe's iteration status.
     - `.catch` a pipe's exceptions of a specific class and return them instead of raising.
-    - `.slow` a pipe to limit the iteration's speed over it.
-- consume
+- consume:
     - `.collect` a pipe into a list having an optional max size.
-    - `.reduce` a pipe to a result using a binary function.
     - `.superintend` a pipe: iterate over it entirely while catching exceptions + logging the iteration process + collecting and raising error samples.
```

### Comparing `kioss-0.1.2/kioss/pipe.py` & `kioss-0.2.0/kioss/pipe.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,47 +1,145 @@
-import atexit
 import itertools
 import logging
+import multiprocessing
+import pickle
 import time
 import timeit
-from concurrent.futures import ThreadPoolExecutor
+from concurrent.futures import (Executor, ProcessPoolExecutor,
+                                ThreadPoolExecutor)
 from datetime import datetime
-from functools import reduce
-from queue import Empty, Queue
-from typing import Callable, Iterable, Iterator, List, Tuple, Type, TypeVar, Union
+from multiprocessing.synchronize import Event
+from queue import Empty, Full, Queue
+from typing import (Any, Callable, Generic, Iterable, Iterator, List, Optional,
+                    Tuple, Type, TypeVar, Union)
 
 import kioss.util as util
 
 T = TypeVar("T")
 R = TypeVar("R")
 
 
+class PipeDefinitionError(Exception):
+    pass
+
+
 class Pipe(Iterator[T]):
     """
     Pipe class that represents a data processing pipeline.
 
     Args:
         source (Union[Iterable[T], Iterator[T]]): The iterator or iterable containing elements for the pipeline.
 
     Attributes:
         iterator (Iterator[T]): The iterator containing elements for the pipeline.
     """
 
-    def __init__(self, source: Union[Iterable[T], Iterator[T]] = []) -> None:
+    def __init__(self, source: Union[Iterable[T], Iterator[T]] = []) -> None:  # timeout
         self.iterator: Iterator[T] = iter(source)
+        self._exit_asked: Event = self._MANAGER.Event()
 
     def __next__(self) -> T:
         return next(self.iterator)
 
     def __iter__(self) -> T:
         return self
 
     def __add__(self, other: "Pipe[T]") -> "Pipe[T]":
         return self.chain(other)
 
+    def __enter__(self) -> "Pipe[T]":
+        return self
+
+    def __exit__(self, exc_type, exc_value, traceback) -> bool:
+        self._exit_asked.set()
+        if isinstance(self.iterator, Pipe):
+            return self.iterator.__exit__(exc_type, exc_value, traceback)
+        return False
+
+    THREAD_WORKER_TYPE = "thread"
+    PROCESS_WORKER_TYPE = "process"
+
+    SUPPORTED_WORKER_TYPES = [THREAD_WORKER_TYPE, PROCESS_WORKER_TYPE]
+
+    _MAX_NUM_WAITING_ELEMS_PER_THREAD = 16
+
+    _MANAGER = multiprocessing.Manager()
+
+    def _map_or_do(
+        self,
+        func: Callable[[T], R],
+        n_workers: Optional[int],
+        worker_type: str,
+        sidify: bool,
+    ) -> "Pipe[Union[R, T]]":
+        if worker_type not in self.SUPPORTED_WORKER_TYPES:
+            raise ValueError(
+                f"'{worker_type}' worker_type is not supported, must be one of: {self.SUPPORTED_WORKER_TYPES}"
+            )
+        if n_workers is None or n_workers <= 0:
+            if sidify:
+                func = util.sidify(func)
+            return Pipe[T](map(func, self))
+        if worker_type == Pipe.PROCESS_WORKER_TYPE:
+            pickle.dumps(func)
+        return _RasingPipe[T](
+            iter(
+                _multi_yielding_iterable(
+                    func,
+                    self,
+                    executor_class=ThreadPoolExecutor
+                    if worker_type == self.THREAD_WORKER_TYPE
+                    else ProcessPoolExecutor,
+                    queue_class=Queue
+                    if worker_type == self.THREAD_WORKER_TYPE
+                    else self._MANAGER.Queue,
+                    n_workers=n_workers,
+                    max_queue_size=self._MAX_NUM_WAITING_ELEMS_PER_THREAD * n_workers,
+                    sidify=sidify,
+                    exit_asked=self._exit_asked,
+                )
+            )
+        )
+
+    def map(
+        self,
+        func: Callable[[T], R],
+        n_workers: Optional[int] = None,
+        worker_type: str = THREAD_WORKER_TYPE,
+    ) -> "Pipe[R]":
+        """
+        Apply a function to each element of the Pipe, creating a new Pipe with the mapped elements.
+
+        Args:
+            func (Callable[[T], R]): The function to be applied to each element.
+            n_workers (int, optional): The number of threads (or processes is worker_type='process') for concurrent func execution (default is 0, meaning single-threaded).
+            worker_type (str, optional): Must be Pipe.THREAD_WORKER_TYPE (default) or Pipe.PROCESS_WORKER_TYPE.
+        Returns:
+            Pipe[R]: A new Pipe instance with elements resulting from applying the function to each element.
+        """
+        return self._map_or_do(func, n_workers, worker_type, sidify=False)
+
+    def do(
+        self,
+        func: Callable[[T], Any],
+        n_workers: Optional[int] = None,
+        worker_type: str = THREAD_WORKER_TYPE,
+    ) -> "Pipe[T]":
+        """
+        Run the func as side effect: the resulting Pipe forwards the upstream elements after func execution's end.
+
+        Args:
+            func (Callable[[T], R]): The function to be applied to each element.
+            n_workers (int, optional): The number of threads (or processes is worker_type='process') for concurrent func execution (default is 0, meaning single-threaded).
+            worker_type (str, optional): Must be Pipe.THREAD_WORKER_TYPE (default) or Pipe.PROCESS_WORKER_TYPE.
+        Returns:
+            Pipe[T]: A new Pipe instance with elements resulting from applying the function to each element.
+        """
+        return self._map_or_do(func, n_workers, worker_type, sidify=True)
+
     def chain(self, *others: Tuple["Pipe[T]"]) -> "Pipe[T]":
         """
         Create a new Pipe by chaining the elements of this Pipe with the elements from other Pipes. The elements of a given Pipe are yielded after its predecessor Pipe is exhausted.
 
         Args:
             *others ([Pipe[T]]): One or more additional Pipe instances to chain with this Pipe.
 
@@ -58,36 +156,14 @@
             *others ([Pipe[T]]): One or more additional Pipe instances to mix with this Pipe.
 
         Returns:
             Pipe[T]: A new Pipe instance concurrently yielding elements from self and others in any order.
         """
         return _RasingPipe[R](_ConcurrentlyMergingPipe[T]([self, *others]))
 
-    def map(
-        self, func: Callable[[T], R], n_threads: int = 0, sidify: bool = False
-    ) -> "Pipe[R]":
-        """
-        Apply a function to each element of the Pipe, creating a new Pipe with the mapped elements.
-
-        Args:
-            func (Callable[[T], R]): The function to be applied to each element.
-            n_threads (int, optional): The number of threads for concurrent mapping (default is 0, meaning single-threaded).
-            sidify (bool, optional): If True, apply function with side effect wrapping (default is False).
-
-        Returns:
-            Pipe[R]: A new Pipe instance with elements resulting from applying the function to each element.
-        """
-        if sidify:
-            func = util.sidify(func)
-
-        if n_threads <= 0:
-            return Pipe[R](map(func, self))
-        else:
-            return _RasingPipe[R](_ConcurrentlyMappingPipe[R](func, self, n_threads))
-
     def flatten(self: "Pipe[Iterator[R]]") -> "Pipe[R]":
         """
         Flatten the elements of the Pipe, which are assumed to be iterators, creating a new Pipe with individual elements.
 
         Returns:
             Pipe[R]: A new Pipe instance with individual elements obtained by flattening the original elements.
         """
@@ -126,27 +202,27 @@
 
         Args:
             freq (float): The frequency (in milliseconds) at which elements are iterated.
 
         Returns:
             Pipe[T]: A new Pipe instance with elements iterated at the specified frequency.
         """
-        return Pipe[T](_SlowingIterator(self, freq))
+        return Pipe[T](_SlowingPipe(self, freq))
 
     def head(self, n: int) -> "Pipe[T]":
         """
         Limit the number of elements in the Pipe, creating a new Pipe with the first `n` elements.
 
         Args:
             n (int): The number of elements to include in the new Pipe.
 
         Returns:
             Pipe[T]: A new Pipe instance with the first `n` elements.
         """
-        return Pipe[T](itertools.islice(self, n))
+        return _HeadPipe[T](self, n)
 
     def catch(self, *classes: Type[Exception], ignore=False) -> "Pipe[T]":
         """
         Any error whose class is exception_class or a subclass of it will be catched and yielded.
 
         Args:
             exception_class (Type[Exception]): The class of exceptions to catch
@@ -162,38 +238,25 @@
         Log the elements of the Pipe as they are iterated.
 
         Returns:
             Pipe[T]: A new Pipe instance with logging capability.
         """
         return _LoggingPipe[T](self, objects_description)
 
-    def reduce(self, func: Callable[[R, T], R], initial: R) -> R:
-        """
-        Reduce the elements of the Pipe using a binary function, starting from the given initial value.
-
-        Args:
-            func (Callable[[R, T], R]): The binary function used for reduction.
-            initial (R): The initial value for the reduction.
-
-        Returns:
-            R: The result of the reduction.
-        """
-        return reduce(func, self, initial)
-
-    def collect(self, limit: int = float("inf")) -> List[T]:
+    def collect(self, n_samples: int = float("inf")) -> List[T]:
         """
-        Convert the elements of the Pipe into a list. The entire pipe will be iterated, even after reaching the optional limit.
+        Convert the elements of the Pipe into a list. The entire pipe will be iterated, but only n_samples elements will be saved in the returned list.
 
         Args:
-            limit (int, optional): The maximum number of elements to include in the list (default is infinity).
+            n_samples (int, optional): The maximum number of elements to collect in the list (default is infinity).
 
         Returns:
             List[T]: A list containing the elements of the Pipe.
         """
-        return [elem for i, elem in enumerate(self) if i < limit]
+        return [elem for i, elem in enumerate(self) if i < n_samples]
 
     def time(self) -> float:
         """
         Measure the time taken to iterate through all the elements in the Pipe.
 
         Returns:
             float: The time taken in seconds.
@@ -215,19 +278,34 @@
             RuntimeError: If any exception is catched during iteration.
         """
         if errors := (
             self.catch(Exception, ignore=False)
             .log(objects_description="ultimate elements")
             .filter(lambda elem: isinstance(elem, Exception))
             .map(repr)
-            .collect(limit=n_error_samples)
+            .collect(n_samples=n_error_samples)
         ):
             raise RuntimeError(errors)
 
 
+class _HeadPipe(Pipe[T]):
+    def __init__(self, iterator: Iterator[T], n: int) -> None:
+        super().__init__(iterator)
+        self.n = n
+        self.yields_count = 0
+
+    def __next__(self) -> T:
+        if self.yields_count == self.n:
+            self.__exit__(None, None, None)
+            raise StopIteration
+        elem = super().__next__()
+        self.yields_count += 1
+        return elem
+
+
 class _FlatteningPipe(Pipe[R]):
     def __init__(self, iterator: Iterator[Iterator[R]]) -> None:
         super().__init__(iterator)
         self.current_iterator_elem = iter(super().__next__())
 
     def __next__(self) -> R:
         try:
@@ -246,14 +324,16 @@
         self.ignore = ignore
 
     def __next__(self) -> T:
         try:
             return super().__next__()
         except StopIteration:
             raise
+        except PipeDefinitionError:
+            raise
         except self.classes as e:
             if self.ignore:
                 return next(self)
             else:
                 return e
 
 
@@ -293,15 +373,15 @@
         if self.yields_count + self.errors_count >= 2 * self.last_log_at_yields_count:
             self._log()
             self.last_log_at_yields_count = self.yields_count + self.errors_count
 
         return elem
 
 
-class _SlowingIterator(Pipe[T]):
+class _SlowingPipe(Pipe[T]):
     def __init__(self, iterator: Iterator[T], freq: float) -> None:
         super().__init__(iterator)
         self.freq = freq
         self.start = None
         self.yields_count = 0
 
     def __next__(self) -> T:
@@ -311,14 +391,35 @@
             next_elem = super().__next__()
             while self.yields_count > (time.time() - self.start) * self.freq:
                 time.sleep(0.001)
             self.yields_count += 1
             return next_elem
 
 
+E = TypeVar("E", bound=Exception)
+
+
+class _CatchedError(Generic[E]):
+    def __init__(self, exception: E) -> None:
+        super().__init__()
+        self.exception: E = exception
+
+
+class _RasingPipe(Pipe[T]):
+    def __init__(self, iterator: Iterator[T]) -> None:
+        super().__init__(iterator)
+
+    def __next__(self) -> T:
+        next_elem = super().__next__()
+        if isinstance(next_elem, _CatchedError):
+            raise next_elem.exception
+        else:
+            return next_elem
+
+
 class _BatchingPipe(Pipe[List[T]]):
     def __init__(
         self, iterator: Iterator[T], max_size: int, max_window_seconds: float
     ) -> None:
         super().__init__(iterator)
         self.max_size = max_size
         self.max_window_seconds = max_window_seconds
@@ -363,79 +464,110 @@
                         queue.put(next(iterator))
                     except StopIteration:
                         break
                     except Exception as e:
                         queue.put(_CatchedError(e))
 
             futures = [executor.submit(pull_job, iterator) for iterator in iterators]
+            backoff_secs = 0.005
             while not queue.empty() or not all((future.done() for future in futures)):
                 try:
-                    yield queue.get(timeout=0.01)
+                    yield queue.get(timeout=backoff_secs)
+                    backoff_secs = 0.005
                 except Empty:
-                    pass
+                    backoff_secs *= 2
 
 
-class _ConcurrentlyMappingPipe(Pipe[R]):
-    MAX_NUM_WAITING_ELEMS_PER_THREAD = 16
+def _mapper(
+    func: Callable[[Any], Any],
+    input_queue: Queue,
+    output_queue: Queue,
+    sidify: bool,
+    exit_asked: Event,
+    sentinel: Any,
+) -> None:
+    while not exit_asked.is_set():
+        try:
+            elem = input_queue.get(timeout=0.1)
+            if elem == sentinel:
+                input_queue.put(sentinel)
+                break
+        except Empty:
+            continue
+        try:
+            res = func(elem)
+            to_output = elem if sidify else res
+        except Exception as e:
+            to_output = _CatchedError(e)
+        while not exit_asked.is_set():
+            try:
+                output_queue.put(to_output, timeout=0.1)
+                break
+            except Empty:
+                pass
 
-    def __init__(
-        self, func: Callable[[T], R], iterator: Iterator[T], n_threads: int
-    ) -> None:
-        super().__init__(
-            iter(
-                self._concurrently_mapping_iterable(
-                    func,
-                    iterator,
-                    n_threads=n_threads,
-                    max_queue_size=self.MAX_NUM_WAITING_ELEMS_PER_THREAD * n_threads,
-                )
-            )
-        )
 
-    @staticmethod
-    def _concurrently_mapping_iterable(
-        func: Callable[[T], R], iterator: Iterator[T], n_threads, max_queue_size: int
-    ) -> Iterator[T]:
-        input_queue: Queue = Queue(maxsize=max_queue_size)
-        output_queue: Queue = Queue(maxsize=max_queue_size)
+def _feeder(
+    input_queue: Queue, iterator: Iterator[T], exit_asked: Event, sentinel: Any
+):
+    while not exit_asked.is_set():
+        try:
+            elem = next(iterator)
+        except StopIteration:
+            while not exit_asked.is_set():
+                try:
+                    input_queue.put(sentinel, timeout=0.1)
+                    break
+                except Full:
+                    pass
+            break
+        except Exception as e:
+            elem = _CatchedError(e)
+        while not exit_asked.is_set():
+            try:
+                input_queue.put(elem, timeout=0.1)
+                break
+            except Full:
+                pass
 
-        with ThreadPoolExecutor(max_workers=n_threads + 1) as executor:
-            input_feeder_future = executor.submit(
-                lambda: util.iterate(map(input_queue.put, iterator))
-            )
 
-            def mapper_job():
-                while not input_feeder_future.done() or not input_queue.empty():
-                    try:
-                        output_queue.put(func(input_queue.get(timeout=0.01)))
-                    except Empty:
-                        pass
-                    except Exception as e:
-                        output_queue.put(_CatchedError(e))
-
-            futures = [executor.submit(mapper_job) for _ in range(n_threads)]
-            while (
+def _multi_yielding_iterable(
+    func: Callable[[T], R],
+    iterator: Iterator[T],
+    executor_class: Type[Executor],
+    queue_class: Type[Queue],
+    n_workers: int,
+    max_queue_size: int,
+    sidify: bool,
+    exit_asked: Event,
+) -> Iterator[Union[T, R]]:
+    input_queue: Queue = queue_class(maxsize=max_queue_size)
+    output_queue: Queue = queue_class(maxsize=max_queue_size)
+
+    with executor_class(max_workers=n_workers) as executor:
+        sentinel = f"__kioss__{time.time()}"
+        futures = [
+            executor.submit(
+                _mapper, func, input_queue, output_queue, sidify, exit_asked, sentinel
+            )
+            for _ in range(n_workers)
+        ]
+        with ThreadPoolExecutor(max_workers=1) as executor:
+            futures.append(
+                executor.submit(_feeder, input_queue, iterator, exit_asked, sentinel)
+            )
+            backoff_secs = 0.005
+            while not exit_asked.is_set() and (
                 not all((future.done() for future in futures))
                 or not output_queue.empty()
             ):
                 try:
-                    yield output_queue.get(timeout=0.01)
+                    yield output_queue.get(timeout=backoff_secs)
+                    backoff_secs = 0.005
                 except Empty:
-                    pass
-
-
-class _CatchedError:
-    def __init__(self, exception: Exception) -> None:
-        super().__init__()
-        self.exception: E = exception
-
-
-class _RasingPipe(Pipe[T]):
-    def __init__(self, iterator: Iterator[T]) -> None:
-        super().__init__(iterator)
-
-    def __next__(self) -> T:
-        next_elem = super().__next__()
-        if isinstance(next_elem, _CatchedError):
-            raise next_elem.exception
-        else:
-            return next_elem
+                    backoff_secs *= 2
+    # yield worker errors not linked to an element processing
+    for future in futures:
+        try:
+            future.result()
+        except Exception as e:
+            yield _CatchedError(e)
```

