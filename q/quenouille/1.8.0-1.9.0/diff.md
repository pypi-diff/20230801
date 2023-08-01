# Comparing `tmp/quenouille-1.8.0.tar.gz` & `tmp/quenouille-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/quenouille-1.8.0.tar", last modified: Thu May  4 13:48:23 2023, max compression
+gzip compressed data, was "dist/quenouille-1.9.0.tar", last modified: Tue Aug  1 14:48:53 2023, max compression
```

## Comparing `quenouille-1.8.0.tar` & `quenouille-1.9.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2023-05-04 13:48:23.000000 quenouille-1.8.0/
--rw-r--r--   0 Yomgui     (501) staff       (20)    19392 2023-05-04 13:48:23.000000 quenouille-1.8.0/PKG-INFO
--rw-r--r--   0 Yomgui     (501) staff       (20)    16510 2023-05-04 13:34:27.000000 quenouille-1.8.0/README.md
-drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2023-05-04 13:48:23.000000 quenouille-1.8.0/quenouille/
--rw-r--r--   0 Yomgui     (501) staff       (20)      183 2023-02-22 19:41:55.000000 quenouille-1.8.0/quenouille/__init__.py
--rw-r--r--   0 Yomgui     (501) staff       (20)      469 2021-05-25 17:09:07.000000 quenouille-1.8.0/quenouille/constants.py
--rw-r--r--   0 Yomgui     (501) staff       (20)      548 2023-05-03 18:05:41.000000 quenouille-1.8.0/quenouille/exceptions.py
--rw-r--r--   0 Yomgui     (501) staff       (20)    42481 2023-05-04 12:24:18.000000 quenouille-1.8.0/quenouille/imap.py
--rw-r--r--   0 Yomgui     (501) staff       (20)     4128 2023-05-04 12:24:05.000000 quenouille-1.8.0/quenouille/utils.py
-drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2023-05-04 13:48:23.000000 quenouille-1.8.0/quenouille.egg-info/
--rw-r--r--   0 Yomgui     (501) staff       (20)    19392 2023-05-04 13:48:23.000000 quenouille-1.8.0/quenouille.egg-info/PKG-INFO
--rw-r--r--   0 Yomgui     (501) staff       (20)      327 2023-05-04 13:48:23.000000 quenouille-1.8.0/quenouille.egg-info/SOURCES.txt
--rw-r--r--   0 Yomgui     (501) staff       (20)        1 2023-05-04 13:48:23.000000 quenouille-1.8.0/quenouille.egg-info/dependency_links.txt
--rw-r--r--   0 Yomgui     (501) staff       (20)       43 2023-05-04 13:48:23.000000 quenouille-1.8.0/quenouille.egg-info/requires.txt
--rw-r--r--   0 Yomgui     (501) staff       (20)       11 2023-05-04 13:48:23.000000 quenouille-1.8.0/quenouille.egg-info/top_level.txt
--rw-r--r--   0 Yomgui     (501) staff       (20)        1 2023-05-04 13:48:23.000000 quenouille-1.8.0/quenouille.egg-info/zip-safe
--rw-r--r--   0 Yomgui     (501) staff       (20)       38 2023-05-04 13:48:23.000000 quenouille-1.8.0/setup.cfg
--rw-r--r--   0 Yomgui     (501) staff       (20)      708 2023-05-04 13:47:32.000000 quenouille-1.8.0/setup.py
+drwxrwxr-x   0 yomguithereal  (1000) yomguithereal  (1000)        0 2023-08-01 14:48:53.000000 quenouille-1.9.0/
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)       38 2023-08-01 14:48:53.000000 quenouille-1.9.0/setup.cfg
+drwxrwxr-x   0 yomguithereal  (1000) yomguithereal  (1000)        0 2023-08-01 14:48:53.000000 quenouille-1.9.0/quenouille.egg-info/
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)       43 2023-08-01 14:48:53.000000 quenouille-1.9.0/quenouille.egg-info/requires.txt
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)       11 2023-08-01 14:48:53.000000 quenouille-1.9.0/quenouille.egg-info/top_level.txt
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      327 2023-08-01 14:48:53.000000 quenouille-1.9.0/quenouille.egg-info/SOURCES.txt
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)        1 2023-08-01 14:48:53.000000 quenouille-1.9.0/quenouille.egg-info/zip-safe
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)        1 2023-08-01 14:48:53.000000 quenouille-1.9.0/quenouille.egg-info/dependency_links.txt
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)    20184 2023-08-01 14:48:53.000000 quenouille-1.9.0/quenouille.egg-info/PKG-INFO
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)    17270 2023-08-01 14:47:25.000000 quenouille-1.9.0/README.md
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      708 2023-08-01 14:48:32.000000 quenouille-1.9.0/setup.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)    20184 2023-08-01 14:48:53.000000 quenouille-1.9.0/PKG-INFO
+drwxrwxr-x   0 yomguithereal  (1000) yomguithereal  (1000)        0 2023-08-01 14:48:53.000000 quenouille-1.9.0/quenouille/
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      183 2023-02-28 14:48:10.000000 quenouille-1.9.0/quenouille/__init__.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      548 2023-05-03 15:02:23.000000 quenouille-1.9.0/quenouille/exceptions.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     3929 2023-08-01 13:59:33.000000 quenouille-1.9.0/quenouille/utils.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)    44023 2023-08-01 14:29:49.000000 quenouille-1.9.0/quenouille/imap.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      469 2023-02-28 14:48:10.000000 quenouille-1.9.0/quenouille/constants.py
```

### Comparing `quenouille-1.8.0/PKG-INFO` & `quenouille-1.9.0/quenouille.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quenouille
-Version: 1.8.0
+Version: 1.9.0
 Summary: A library of multithreaded iterator workflows.
 Home-page: http://github.com/medialab/quenouille
 Author: Guillaume Plique
 Author-email: kropotkinepiotr@gmail.com
 License: MIT
 Description: [![Build Status](https://github.com/medialab/quenouille/workflows/Tests/badge.svg)](https://github.com/medialab/quenouille/actions)
         
@@ -22,27 +22,27 @@
         
         ```
         pip install quenouille
         ```
         
         ## Usage
         
-        * [imap, imap_unordered](#imap_unordered-imap)
-        * [ThreadPoolExecutor](#threadpoolexecutor)
-          * [#.imap, #.imap_unordered](#executor-imap)
-          * [#.shutdown](#shutdown)
-        * [NamedLocks](#namedlocks)
-        * [Miscellaneous notes](#miscellaneous-notes)
-          * [The None group](#the-none-group)
-          * [Parallelism > workers](#parallelism--workers)
-          * [Callable parallelism guarantees](#callable-parallelism-guarantees)
-          * [Parallelism vs. throttling](#parallelism-vs-throttling)
-          * [Adding entropy to throttle](#adding-entropy-to-throttle)
-          * [Caveats regarding exception raising](#caveats-regarding-exception-raising)
-          * [Caveats of using imap with queues](#caveats-of-using-imap-with-queues)
+        - [imap, imap_unordered](#imap_unordered-imap)
+        - [ThreadPoolExecutor](#threadpoolexecutor)
+          - [#.imap, #.imap_unordered](#executor-imap)
+          - [#.shutdown](#shutdown)
+        - [NamedLocks](#namedlocks)
+        - [Miscellaneous notes](#miscellaneous-notes)
+          - [The None group](#the-none-group)
+          - [Parallelism > workers](#parallelism--workers)
+          - [Callable parallelism guarantees](#callable-parallelism-guarantees)
+          - [Parallelism vs. throttling](#parallelism-vs-throttling)
+          - [Adding entropy to throttle](#adding-entropy-to-throttle)
+          - [Caveats regarding exception raising](#caveats-regarding-exception-raising)
+          - [Caveats of using imap with queues](#caveats-of-using-imap-with-queues)
         
         ### imap, imap_unordered
         
         Function lazily consuming an iterable and applying the desired function over the yielded items in a multithreaded fashion.
         
         This function is also able to respect group constraints regarding parallelism and throttling: for instance, if you need to download urls in a multithreaded fashion and need to ensure that you won't hit the same domain more than twice at the same time, this function can be given proper settings to ensure the desired behavior.
         
@@ -99,29 +99,31 @@
           print(html)
         
         # Only load 10 urls into memory when attempting to find next suitable job
         for html in imap(urls(), fetch, 10, key=get_domain_name, throttle=5, buffer_size=10):
           print(html)
         ```
         
-        *Arguments*
+        _Arguments_
         
-        * **iterable** *(iterable)*: Any python iterable.
-        * **func** *(callable)*: Function used to perform the desired tasks. The function takes an item yielded by the given iterable as single argument. Note that since this function will be dispatched in worker threads, so you should ensure it is thread-safe.
-        * **threads** *(int, optional)*: Maximum number of threads to use. Defaults to `min(32, os.cpu_count() + 1)`. Note that it can be `0`, in which case no threads will be used and everything will run synchronously (this can be useful for debugging or to avoid duplicating code sometimes).
-        * **key** *(callable, optional)*: Function returning to which "group" a given item is supposed to belong. This will be used to ensure maximum parallelism is respected.
-        * **parallelism** *(int or callable, optional)* [`1`]: Number of threads allowed to work on a same group at once. Can also be a function taking a group and returning its parallelism.
-        * **buffer_size** *(int, optional)* [`1024`]: Maximum number of items the function will buffer into memory while attempting to find an item that can be passed to a worker immediately, all while respecting throttling and group parallelism.
-        * **throttle** *(int or float or callable, optional)*: Optional throttle time, in seconds, to wait before processing the next item of a given group. Can also be a function taking last group, item and result and returning next throttle time for this group.
-        * **initializer** *(callable, optional)*: Function to run at the start of each thread worker. Can be useful to setup [thread-local data](https://docs.python.org/3/library/threading.html#thread-local-data), for instance. Remember this function must be threadsafe and should not block because the thread pool will wait for each thread to be correctly booted before being able to proceed. If one of the function calls fails, the thread pool will raise a `quenouille.exceptions.BrokenThreadPool` error and terminate immediately.
-        * **initargs** *(iterable, optional)*: Arguments to pass to the `initializer` function.
-        * **wait** *(bool, optional)* [`True`]: Whether to join worker threads, i.e. wait for them to end, when shutting down the executor. Set this to `False` if you need to go on quickly without waiting for your worker threads to end when cleaning up the executor's resources. Just note that if you spawn other thread-intensive tasks or other executors afterwards in rapid succession, you might start too many threads at once.
-        * **daemonic** *(bool, optional)* [`False`]: whether to spawn daemonic worker. If your worker are daemonic, the interpreter will not wait for them to end when exiting. This can be useful, combined to `wait=False`, for instance, if you want your program to exit as soon as hitting ctrl+C (you might want to avoid this if your threads need to cleanup things on exit as they will be abruptly shut down).
+        - **iterable** _(iterable)_: Any python iterable.
+        - **func** _(callable)_: Function used to perform the desired tasks. The function takes an item yielded by the given iterable as single argument. Note that since this function will be dispatched in worker threads, so you should ensure it is thread-safe.
+        - **threads** _(int, optional)_: Maximum number of threads to use. Defaults to `min(32, os.cpu_count() + 1)`. Note that it can be `0`, in which case no threads will be used and everything will run synchronously (this can be useful for debugging or to avoid duplicating code sometimes).
+        - **key** _(callable, optional)_: Function returning to which "group" a given item is supposed to belong. This will be used to ensure maximum parallelism is respected.
+        - **parallelism** _(int or callable, optional)_ [`1`]: Number of threads allowed to work on a same group at once. Can also be a function taking a group and returning its parallelism.
+        - **buffer_size** _(int, optional)_ [`1024`]: Maximum number of items the function will buffer into memory while attempting to find an item that can be passed to a worker immediately, all while respecting throttling and group parallelism.
+        - **throttle** _(int or float or callable, optional)_: Optional throttle time, in seconds, to wait before processing the next item of a given group. Can also be a function taking last group, item and result and returning next throttle time for this group.
+        - **block** _(bool, optional)_ [`False`]: Whether to block when using the `get` method of the given queue.
+        - **panic** _(callable, optional)_: Function that will be called when the process has errored. Useful to unblock some functions and avoid deadlock in specific situations. Note that this function will not be called when synchronous (i.e. when not using additional threads).
+        - **initializer** _(callable, optional)_: Function to run at the start of each thread worker. Can be useful to setup [thread-local data](https://docs.python.org/3/library/threading.html#thread-local-data), for instance. Remember this function must be threadsafe and should not block because the thread pool will wait for each thread to be correctly booted before being able to proceed. If one of the function calls fails, the thread pool will raise a `quenouille.exceptions.BrokenThreadPool` error and terminate immediately.
+        - **initargs** _(iterable, optional)_: Arguments to pass to the `initializer` function.
+        - **wait** _(bool, optional)_ [`True`]: Whether to join worker threads, i.e. wait for them to end, when shutting down the executor. Set this to `False` if you need to go on quickly without waiting for your worker threads to end when cleaning up the executor's resources. Just note that if you spawn other thread-intensive tasks or other executors afterwards in rapid succession, you might start too many threads at once.
+        - **daemonic** _(bool, optional)_ [`False`]: whether to spawn daemonic worker. If your worker are daemonic, the interpreter will not wait for them to end when exiting. This can be useful, combined to `wait=False`, for instance, if you want your program to exit as soon as hitting ctrl+C (you might want to avoid this if your threads need to cleanup things on exit as they will be abruptly shut down).
         
-        *Using a queue rather than an iterable*
+        _Using a queue rather than an iterable_
         
         If you need to add new items to process as a result of performing tasks (when designing a web crawler for instance, where each downloaded page will yield new pages to explore further down), know that the `imap` and `imap_unordered` function also accepts queues as input:
         
         ```python
         from queue import Queue
         from quenouille import imap
         
@@ -175,40 +177,42 @@
         executor = ThreadPoolExecutor()
         executor.imap(range(10), worker)
         executor.shutdown(wait=False)
         ```
         
         Note that your throttling state is kept between multiple `imap` and `imap_unordered` calls so you don't end up perform some tasks too soon. But keep in mind this state is tied to the `key` function you provide to remain consistent, so if you change the used `key`, the throttling state will be reset.
         
-        *Arguments*
+        _Arguments_
         
-        * **max_workers** *(int, optional)*: Maximum number of threads to use. Defaults to `min(32, os.cpu_count() + 1)`. Note that it can be `0`, in which case no threads will be used and everything will run synchronously (this can be useful for debugging or to avoid duplicating code sometimes).
-        * **initializer** *(callable, optional)*: Function to run at the start of each thread worker. Can be useful to setup [thread-local data](https://docs.python.org/3/library/threading.html#thread-local-data), for instance. Remember this function must be threadsafe and should not block because the thread pool will wait for each thread to be correctly booted before being able to proceed. If one of the function calls fails, the thread pool will raise a `quenouille.exceptions.BrokenThreadPool` error and terminate immediately.
-        * **initargs** *(iterable, optional)*: Arguments to pass to the `initializer` function.
-        * **wait** *(bool, optional)* [`True`]: Whether to join worker threads, i.e. wait for them to end, when closing the executor. Set this to `False` if you need to go on quickly without waiting for your worker threads to end when cleaning up the executor's resources. Just note that if you spawn other thread-intensive tasks or other executors afterwards in rapid succession, you might start too many threads at once.
-        * **daemonic** *(bool, optional)* [`False`]: whether to spawn daemonic worker. If your worker are daemonic, the interpreter will not wait for them to end when exiting. This can be useful, combined to `wait=False`, for instance, if you want your program to exit as soon as hitting ctrl+C (you might want to avoid this if your threads need to cleanup things on exit as they will be abruptly shut down).
+        - **max_workers** _(int, optional)_: Maximum number of threads to use. Defaults to `min(32, os.cpu_count() + 1)`. Note that it can be `0`, in which case no threads will be used and everything will run synchronously (this can be useful for debugging or to avoid duplicating code sometimes).
+        - **initializer** _(callable, optional)_: Function to run at the start of each thread worker. Can be useful to setup [thread-local data](https://docs.python.org/3/library/threading.html#thread-local-data), for instance. Remember this function must be threadsafe and should not block because the thread pool will wait for each thread to be correctly booted before being able to proceed. If one of the function calls fails, the thread pool will raise a `quenouille.exceptions.BrokenThreadPool` error and terminate immediately.
+        - **initargs** _(iterable, optional)_: Arguments to pass to the `initializer` function.
+        - **wait** _(bool, optional)_ [`True`]: Whether to join worker threads, i.e. wait for them to end, when closing the executor. Set this to `False` if you need to go on quickly without waiting for your worker threads to end when cleaning up the executor's resources. Just note that if you spawn other thread-intensive tasks or other executors afterwards in rapid succession, you might start too many threads at once.
+        - **daemonic** _(bool, optional)_ [`False`]: whether to spawn daemonic worker. If your worker are daemonic, the interpreter will not wait for them to end when exiting. This can be useful, combined to `wait=False`, for instance, if you want your program to exit as soon as hitting ctrl+C (you might want to avoid this if your threads need to cleanup things on exit as they will be abruptly shut down).
         
         <h4 id="executor-imap">#.imap, #.imap_unordered</h4>
         
         Basically the same as described [here](#imap_unordered-imap) with the following arguments:
         
-        * **iterable** *(iterable)*: Any python iterable.
-        * **func** *(callable)*: Function used to perform the desired tasks. The function takes an item yielded by the given iterable as single argument. Note that since this function will be dispatched in worker threads, so you should ensure it is thread-safe.
-        * **key** *(callable, optional)*: Function returning to which "group" a given item is supposed to belong. This will be used to ensure maximum parallelism is respected.
-        * **parallelism** *(int or callable, optional)* [`1`]: Number of threads allowed to work on a same group at once. Can also be a function taking a group and returning its parallelism.
-        * **buffer_size** *(int, optional)* [`1024`]: Maximum number of items the function will buffer into memory while attempting to find an item that can be passed to a worker immediately, all while respecting throttling and group parallelism.
-        * **throttle** *(int or float or callable, optional)*: Optional throttle time, in seconds, to wait before processing the next item of a given group. Can also be a function taking last group, item and result and returning next throttle time for this group.
+        - **iterable** _(iterable)_: Any python iterable.
+        - **func** _(callable)_: Function used to perform the desired tasks. The function takes an item yielded by the given iterable as single argument. Note that since this function will be dispatched in worker threads, so you should ensure it is thread-safe.
+        - **key** _(callable, optional)_: Function returning to which "group" a given item is supposed to belong. This will be used to ensure maximum parallelism is respected.
+        - **parallelism** _(int or callable, optional)_ [`1`]: Number of threads allowed to work on a same group at once. Can also be a function taking a group and returning its parallelism.
+        - **buffer_size** _(int, optional)_ [`1024`]: Maximum number of items the function will buffer into memory while attempting to find an item that can be passed to a worker immediately, all while respecting throttling and group parallelism.
+        - **throttle** _(int or float or callable, optional)_: Optional throttle time, in seconds, to wait before processing the next item of a given group. Can also be a function taking last group, item and result and returning next throttle time for this group.
+        - **block** _(bool, optional)_ [`False`]: Whether to block when using the `get` method of the given queue.
+        - **panic** _(callable, optional)_: Function that will be called when the process has errored. Useful to unblock some functions and avoid deadlock in specific situations. Note that this function will not be called when synchronous (i.e. when not using additional threads).
         
         #### #.shutdown
         
         Method used to explicitly shutdown the executor.
         
-        *Arguments*
+        _Arguments_
         
-        * **wait** *(bool, optional)* [`True`]: Whether to join worker threads, i.e. wait for them to end, when shutting down the executor. Set this to `False` if you need to go on quickly without waiting for your worker threads to end when cleaning up the executor's resources. Just note that if you spawn other thread-intensive tasks or other executors afterwards in rapid succession, you might start too many threads at once.
+        - **wait** _(bool, optional)_ [`True`]: Whether to join worker threads, i.e. wait for them to end, when shutting down the executor. Set this to `False` if you need to go on quickly without waiting for your worker threads to end when cleaning up the executor's resources. Just note that if you spawn other thread-intensive tasks or other executors afterwards in rapid succession, you might start too many threads at once.
         
         ### NamedLocks
         
         A weakref dictionary of locks useful to make some tasks based on keys threadsafe, e.g. if you need to ensure that two threads will not be writing to the same file at once.
         
         ```python
         from quenouille import NamedLocks
@@ -257,15 +261,15 @@
         # Waiting 5 + (between 0 and 2) seconds
         def throttle(group, item, result):
           return 5 + (2 * random())
         ```
         
         #### Caveats regarding exception raising
         
-        *Deferred generator usage exception deadlocks*
+        _Deferred generator usage exception deadlocks_
         
         If you consume a generator returned by `imap/imap_unordered` somewhere else than where you created it, you may end up in a deadlock if you raise an exception.
         
         This is not important when using `daemonic=True` but you might stumble upon segfaults on exit because of python reasons beyond my control.
         
         ```python
         # Safe
@@ -287,15 +291,15 @@
         
         for item in it:
           raise RuntimeError
         ```
         
         #### Caveats of using imap with queues
         
-        *Typical deadlocks*
+        _Typical deadlocks_
         
         Even if `imap` can process an input queue, you should avoid to find yourself in a situation where adding to the queue might block execution if you don't want to end in a deadlock. It can be easy to footgun yourself if your queue has a `maxsize`, for instance:
         
         ```python
         from queue import Queue
         from quenouille import imap
         
@@ -310,21 +314,21 @@
             # This will put you in a deadlock because this will block
             # because of the queue `maxsize` set to 2
             job_queue.put(4)
         
           print(i)
         ```
         
-        *Design choices*
+        _Design choices_
         
         To enable you to add items to the queue in the loop body and so it can safely detect when your queue is drained without race condition, `quenouille` acknowledges that a task is finished only after what you execute in the loop body is done.
         
         This means that sometimes it might be more performant to only add items to the queue from the worker functions rather than from the loop body.
         
-        *queue.task_done*
+        _queue.task_done_
         
         For now, `quenouille` does not call `queue.task_done` for you, so this remains your responsability, if you want to be able to call `queue.join` down the line.
         
 Keywords: url
 Platform: UNKNOWN
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
```

### Comparing `quenouille-1.8.0/README.md` & `quenouille-1.9.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -14,27 +14,27 @@
 
 ```
 pip install quenouille
 ```
 
 ## Usage
 
-* [imap, imap_unordered](#imap_unordered-imap)
-* [ThreadPoolExecutor](#threadpoolexecutor)
-  * [#.imap, #.imap_unordered](#executor-imap)
-  * [#.shutdown](#shutdown)
-* [NamedLocks](#namedlocks)
-* [Miscellaneous notes](#miscellaneous-notes)
-  * [The None group](#the-none-group)
-  * [Parallelism > workers](#parallelism--workers)
-  * [Callable parallelism guarantees](#callable-parallelism-guarantees)
-  * [Parallelism vs. throttling](#parallelism-vs-throttling)
-  * [Adding entropy to throttle](#adding-entropy-to-throttle)
-  * [Caveats regarding exception raising](#caveats-regarding-exception-raising)
-  * [Caveats of using imap with queues](#caveats-of-using-imap-with-queues)
+- [imap, imap_unordered](#imap_unordered-imap)
+- [ThreadPoolExecutor](#threadpoolexecutor)
+  - [#.imap, #.imap_unordered](#executor-imap)
+  - [#.shutdown](#shutdown)
+- [NamedLocks](#namedlocks)
+- [Miscellaneous notes](#miscellaneous-notes)
+  - [The None group](#the-none-group)
+  - [Parallelism > workers](#parallelism--workers)
+  - [Callable parallelism guarantees](#callable-parallelism-guarantees)
+  - [Parallelism vs. throttling](#parallelism-vs-throttling)
+  - [Adding entropy to throttle](#adding-entropy-to-throttle)
+  - [Caveats regarding exception raising](#caveats-regarding-exception-raising)
+  - [Caveats of using imap with queues](#caveats-of-using-imap-with-queues)
 
 ### imap, imap_unordered
 
 Function lazily consuming an iterable and applying the desired function over the yielded items in a multithreaded fashion.
 
 This function is also able to respect group constraints regarding parallelism and throttling: for instance, if you need to download urls in a multithreaded fashion and need to ensure that you won't hit the same domain more than twice at the same time, this function can be given proper settings to ensure the desired behavior.
 
@@ -91,29 +91,31 @@
   print(html)
 
 # Only load 10 urls into memory when attempting to find next suitable job
 for html in imap(urls(), fetch, 10, key=get_domain_name, throttle=5, buffer_size=10):
   print(html)
 ```
 
-*Arguments*
+_Arguments_
 
-* **iterable** *(iterable)*: Any python iterable.
-* **func** *(callable)*: Function used to perform the desired tasks. The function takes an item yielded by the given iterable as single argument. Note that since this function will be dispatched in worker threads, so you should ensure it is thread-safe.
-* **threads** *(int, optional)*: Maximum number of threads to use. Defaults to `min(32, os.cpu_count() + 1)`. Note that it can be `0`, in which case no threads will be used and everything will run synchronously (this can be useful for debugging or to avoid duplicating code sometimes).
-* **key** *(callable, optional)*: Function returning to which "group" a given item is supposed to belong. This will be used to ensure maximum parallelism is respected.
-* **parallelism** *(int or callable, optional)* [`1`]: Number of threads allowed to work on a same group at once. Can also be a function taking a group and returning its parallelism.
-* **buffer_size** *(int, optional)* [`1024`]: Maximum number of items the function will buffer into memory while attempting to find an item that can be passed to a worker immediately, all while respecting throttling and group parallelism.
-* **throttle** *(int or float or callable, optional)*: Optional throttle time, in seconds, to wait before processing the next item of a given group. Can also be a function taking last group, item and result and returning next throttle time for this group.
-* **initializer** *(callable, optional)*: Function to run at the start of each thread worker. Can be useful to setup [thread-local data](https://docs.python.org/3/library/threading.html#thread-local-data), for instance. Remember this function must be threadsafe and should not block because the thread pool will wait for each thread to be correctly booted before being able to proceed. If one of the function calls fails, the thread pool will raise a `quenouille.exceptions.BrokenThreadPool` error and terminate immediately.
-* **initargs** *(iterable, optional)*: Arguments to pass to the `initializer` function.
-* **wait** *(bool, optional)* [`True`]: Whether to join worker threads, i.e. wait for them to end, when shutting down the executor. Set this to `False` if you need to go on quickly without waiting for your worker threads to end when cleaning up the executor's resources. Just note that if you spawn other thread-intensive tasks or other executors afterwards in rapid succession, you might start too many threads at once.
-* **daemonic** *(bool, optional)* [`False`]: whether to spawn daemonic worker. If your worker are daemonic, the interpreter will not wait for them to end when exiting. This can be useful, combined to `wait=False`, for instance, if you want your program to exit as soon as hitting ctrl+C (you might want to avoid this if your threads need to cleanup things on exit as they will be abruptly shut down).
+- **iterable** _(iterable)_: Any python iterable.
+- **func** _(callable)_: Function used to perform the desired tasks. The function takes an item yielded by the given iterable as single argument. Note that since this function will be dispatched in worker threads, so you should ensure it is thread-safe.
+- **threads** _(int, optional)_: Maximum number of threads to use. Defaults to `min(32, os.cpu_count() + 1)`. Note that it can be `0`, in which case no threads will be used and everything will run synchronously (this can be useful for debugging or to avoid duplicating code sometimes).
+- **key** _(callable, optional)_: Function returning to which "group" a given item is supposed to belong. This will be used to ensure maximum parallelism is respected.
+- **parallelism** _(int or callable, optional)_ [`1`]: Number of threads allowed to work on a same group at once. Can also be a function taking a group and returning its parallelism.
+- **buffer_size** _(int, optional)_ [`1024`]: Maximum number of items the function will buffer into memory while attempting to find an item that can be passed to a worker immediately, all while respecting throttling and group parallelism.
+- **throttle** _(int or float or callable, optional)_: Optional throttle time, in seconds, to wait before processing the next item of a given group. Can also be a function taking last group, item and result and returning next throttle time for this group.
+- **block** _(bool, optional)_ [`False`]: Whether to block when using the `get` method of the given queue.
+- **panic** _(callable, optional)_: Function that will be called when the process has errored. Useful to unblock some functions and avoid deadlock in specific situations. Note that this function will not be called when synchronous (i.e. when not using additional threads).
+- **initializer** _(callable, optional)_: Function to run at the start of each thread worker. Can be useful to setup [thread-local data](https://docs.python.org/3/library/threading.html#thread-local-data), for instance. Remember this function must be threadsafe and should not block because the thread pool will wait for each thread to be correctly booted before being able to proceed. If one of the function calls fails, the thread pool will raise a `quenouille.exceptions.BrokenThreadPool` error and terminate immediately.
+- **initargs** _(iterable, optional)_: Arguments to pass to the `initializer` function.
+- **wait** _(bool, optional)_ [`True`]: Whether to join worker threads, i.e. wait for them to end, when shutting down the executor. Set this to `False` if you need to go on quickly without waiting for your worker threads to end when cleaning up the executor's resources. Just note that if you spawn other thread-intensive tasks or other executors afterwards in rapid succession, you might start too many threads at once.
+- **daemonic** _(bool, optional)_ [`False`]: whether to spawn daemonic worker. If your worker are daemonic, the interpreter will not wait for them to end when exiting. This can be useful, combined to `wait=False`, for instance, if you want your program to exit as soon as hitting ctrl+C (you might want to avoid this if your threads need to cleanup things on exit as they will be abruptly shut down).
 
-*Using a queue rather than an iterable*
+_Using a queue rather than an iterable_
 
 If you need to add new items to process as a result of performing tasks (when designing a web crawler for instance, where each downloaded page will yield new pages to explore further down), know that the `imap` and `imap_unordered` function also accepts queues as input:
 
 ```python
 from queue import Queue
 from quenouille import imap
 
@@ -167,40 +169,42 @@
 executor = ThreadPoolExecutor()
 executor.imap(range(10), worker)
 executor.shutdown(wait=False)
 ```
 
 Note that your throttling state is kept between multiple `imap` and `imap_unordered` calls so you don't end up perform some tasks too soon. But keep in mind this state is tied to the `key` function you provide to remain consistent, so if you change the used `key`, the throttling state will be reset.
 
-*Arguments*
+_Arguments_
 
-* **max_workers** *(int, optional)*: Maximum number of threads to use. Defaults to `min(32, os.cpu_count() + 1)`. Note that it can be `0`, in which case no threads will be used and everything will run synchronously (this can be useful for debugging or to avoid duplicating code sometimes).
-* **initializer** *(callable, optional)*: Function to run at the start of each thread worker. Can be useful to setup [thread-local data](https://docs.python.org/3/library/threading.html#thread-local-data), for instance. Remember this function must be threadsafe and should not block because the thread pool will wait for each thread to be correctly booted before being able to proceed. If one of the function calls fails, the thread pool will raise a `quenouille.exceptions.BrokenThreadPool` error and terminate immediately.
-* **initargs** *(iterable, optional)*: Arguments to pass to the `initializer` function.
-* **wait** *(bool, optional)* [`True`]: Whether to join worker threads, i.e. wait for them to end, when closing the executor. Set this to `False` if you need to go on quickly without waiting for your worker threads to end when cleaning up the executor's resources. Just note that if you spawn other thread-intensive tasks or other executors afterwards in rapid succession, you might start too many threads at once.
-* **daemonic** *(bool, optional)* [`False`]: whether to spawn daemonic worker. If your worker are daemonic, the interpreter will not wait for them to end when exiting. This can be useful, combined to `wait=False`, for instance, if you want your program to exit as soon as hitting ctrl+C (you might want to avoid this if your threads need to cleanup things on exit as they will be abruptly shut down).
+- **max_workers** _(int, optional)_: Maximum number of threads to use. Defaults to `min(32, os.cpu_count() + 1)`. Note that it can be `0`, in which case no threads will be used and everything will run synchronously (this can be useful for debugging or to avoid duplicating code sometimes).
+- **initializer** _(callable, optional)_: Function to run at the start of each thread worker. Can be useful to setup [thread-local data](https://docs.python.org/3/library/threading.html#thread-local-data), for instance. Remember this function must be threadsafe and should not block because the thread pool will wait for each thread to be correctly booted before being able to proceed. If one of the function calls fails, the thread pool will raise a `quenouille.exceptions.BrokenThreadPool` error and terminate immediately.
+- **initargs** _(iterable, optional)_: Arguments to pass to the `initializer` function.
+- **wait** _(bool, optional)_ [`True`]: Whether to join worker threads, i.e. wait for them to end, when closing the executor. Set this to `False` if you need to go on quickly without waiting for your worker threads to end when cleaning up the executor's resources. Just note that if you spawn other thread-intensive tasks or other executors afterwards in rapid succession, you might start too many threads at once.
+- **daemonic** _(bool, optional)_ [`False`]: whether to spawn daemonic worker. If your worker are daemonic, the interpreter will not wait for them to end when exiting. This can be useful, combined to `wait=False`, for instance, if you want your program to exit as soon as hitting ctrl+C (you might want to avoid this if your threads need to cleanup things on exit as they will be abruptly shut down).
 
 <h4 id="executor-imap">#.imap, #.imap_unordered</h4>
 
 Basically the same as described [here](#imap_unordered-imap) with the following arguments:
 
-* **iterable** *(iterable)*: Any python iterable.
-* **func** *(callable)*: Function used to perform the desired tasks. The function takes an item yielded by the given iterable as single argument. Note that since this function will be dispatched in worker threads, so you should ensure it is thread-safe.
-* **key** *(callable, optional)*: Function returning to which "group" a given item is supposed to belong. This will be used to ensure maximum parallelism is respected.
-* **parallelism** *(int or callable, optional)* [`1`]: Number of threads allowed to work on a same group at once. Can also be a function taking a group and returning its parallelism.
-* **buffer_size** *(int, optional)* [`1024`]: Maximum number of items the function will buffer into memory while attempting to find an item that can be passed to a worker immediately, all while respecting throttling and group parallelism.
-* **throttle** *(int or float or callable, optional)*: Optional throttle time, in seconds, to wait before processing the next item of a given group. Can also be a function taking last group, item and result and returning next throttle time for this group.
+- **iterable** _(iterable)_: Any python iterable.
+- **func** _(callable)_: Function used to perform the desired tasks. The function takes an item yielded by the given iterable as single argument. Note that since this function will be dispatched in worker threads, so you should ensure it is thread-safe.
+- **key** _(callable, optional)_: Function returning to which "group" a given item is supposed to belong. This will be used to ensure maximum parallelism is respected.
+- **parallelism** _(int or callable, optional)_ [`1`]: Number of threads allowed to work on a same group at once. Can also be a function taking a group and returning its parallelism.
+- **buffer_size** _(int, optional)_ [`1024`]: Maximum number of items the function will buffer into memory while attempting to find an item that can be passed to a worker immediately, all while respecting throttling and group parallelism.
+- **throttle** _(int or float or callable, optional)_: Optional throttle time, in seconds, to wait before processing the next item of a given group. Can also be a function taking last group, item and result and returning next throttle time for this group.
+- **block** _(bool, optional)_ [`False`]: Whether to block when using the `get` method of the given queue.
+- **panic** _(callable, optional)_: Function that will be called when the process has errored. Useful to unblock some functions and avoid deadlock in specific situations. Note that this function will not be called when synchronous (i.e. when not using additional threads).
 
 #### #.shutdown
 
 Method used to explicitly shutdown the executor.
 
-*Arguments*
+_Arguments_
 
-* **wait** *(bool, optional)* [`True`]: Whether to join worker threads, i.e. wait for them to end, when shutting down the executor. Set this to `False` if you need to go on quickly without waiting for your worker threads to end when cleaning up the executor's resources. Just note that if you spawn other thread-intensive tasks or other executors afterwards in rapid succession, you might start too many threads at once.
+- **wait** _(bool, optional)_ [`True`]: Whether to join worker threads, i.e. wait for them to end, when shutting down the executor. Set this to `False` if you need to go on quickly without waiting for your worker threads to end when cleaning up the executor's resources. Just note that if you spawn other thread-intensive tasks or other executors afterwards in rapid succession, you might start too many threads at once.
 
 ### NamedLocks
 
 A weakref dictionary of locks useful to make some tasks based on keys threadsafe, e.g. if you need to ensure that two threads will not be writing to the same file at once.
 
 ```python
 from quenouille import NamedLocks
@@ -249,15 +253,15 @@
 # Waiting 5 + (between 0 and 2) seconds
 def throttle(group, item, result):
   return 5 + (2 * random())
 ```
 
 #### Caveats regarding exception raising
 
-*Deferred generator usage exception deadlocks*
+_Deferred generator usage exception deadlocks_
 
 If you consume a generator returned by `imap/imap_unordered` somewhere else than where you created it, you may end up in a deadlock if you raise an exception.
 
 This is not important when using `daemonic=True` but you might stumble upon segfaults on exit because of python reasons beyond my control.
 
 ```python
 # Safe
@@ -279,15 +283,15 @@
 
 for item in it:
   raise RuntimeError
 ```
 
 #### Caveats of using imap with queues
 
-*Typical deadlocks*
+_Typical deadlocks_
 
 Even if `imap` can process an input queue, you should avoid to find yourself in a situation where adding to the queue might block execution if you don't want to end in a deadlock. It can be easy to footgun yourself if your queue has a `maxsize`, for instance:
 
 ```python
 from queue import Queue
 from quenouille import imap
 
@@ -302,16 +306,16 @@
     # This will put you in a deadlock because this will block
     # because of the queue `maxsize` set to 2
     job_queue.put(4)
 
   print(i)
 ```
 
-*Design choices*
+_Design choices_
 
 To enable you to add items to the queue in the loop body and so it can safely detect when your queue is drained without race condition, `quenouille` acknowledges that a task is finished only after what you execute in the loop body is done.
 
 This means that sometimes it might be more performant to only add items to the queue from the worker functions rather than from the loop body.
 
-*queue.task_done*
+_queue.task_done_
 
 For now, `quenouille` does not call `queue.task_done` for you, so this remains your responsability, if you want to be able to call `queue.join` down the line.
```

### Comparing `quenouille-1.8.0/quenouille/exceptions.py` & `quenouille-1.9.0/quenouille/exceptions.py`

 * *Files identical despite different names*

### Comparing `quenouille-1.8.0/quenouille/imap.py` & `quenouille-1.9.0/quenouille/imap.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,17 +18,17 @@
     Iterable,
     Union,
 )
 
 import sys
 
 if sys.version_info >= (3, 8):
-    from typing import Protocol
+    from typing import Protocol, runtime_checkable
 else:
-    from typing_extensions import Protocol
+    from typing_extensions import Protocol, runtime_checkable
 
 import time
 from queue import Queue, Empty
 from threading import Thread, Event, Lock, Condition, Barrier, BrokenBarrierError
 from collections import OrderedDict
 from collections.abc import Sized
 from itertools import count
@@ -38,25 +38,28 @@
     InvalidThrottleParallelismCombination,
 )
 from quenouille.utils import (
     clear,
     flush,
     smash,
     queue_iter,
-    is_usable_queue,
     get_default_maxworkers,
     SmartTimer,
     TimedHeapSet,
 )
 from quenouille.constants import THE_END_IS_NIGH, DEFAULT_BUFFER_SIZE, TIMER_EPSILON
 
 ItemType = TypeVar("ItemType", covariant=True)
 
 
+@runtime_checkable
 class QuenouilleQueueProtocol(Protocol[ItemType]):
+    def get(self, block: bool = ...) -> ItemType:
+        ...
+
     def get_nowait(self) -> ItemType:
         ...
 
 
 GroupType = TypeVar("GroupType", bound=Hashable)
 ResultType = TypeVar("ResultType")
 ImapTarget = Union[QuenouilleQueueProtocol[ItemType], Iterable[ItemType]]
@@ -566,17 +569,19 @@
         raise TypeError('"daemonic" should be boolean')
 
     if not isinstance(excepthook, bool):
         raise TypeError('"excepthook" should be boolean')
 
 
 def validate_imap_kwargs(
-    iterable, func, *, key, parallelism, buffer_size, throttle
+    iterable, func, *, key, parallelism, buffer_size, throttle, block, panic
 ) -> None:
-    if not isinstance(iterable, Iterable) and not is_usable_queue(iterable):
+    if not isinstance(iterable, Iterable) and not isinstance(
+        iterable, QuenouilleQueueProtocol
+    ):
         raise TypeError("target is not iterable nor a queue")
 
     if not callable(func):
         raise TypeError("worker function is not callable")
 
     if key is not None and not callable(key):
         raise TypeError('"key" is not callable')
@@ -592,14 +597,20 @@
 
     if not isinstance(throttle, (int, float)) and not callable(throttle):
         raise TypeError('"throttle" is not a number nor callable')
 
     if isinstance(throttle, (int, float)) and throttle < 0:
         raise TypeError('"throttle" cannot be negative')
 
+    if not isinstance(block, bool):
+        raise TypeError('"block" should be boolean')
+
+    if panic is not None and not callable(panic):
+        raise TypeError('"panic" should be callable')
+
 
 class ThreadPoolExecutor(object):
     """
     Quenouille custom ThreadPoolExecutor able to lazily pull items to process
     from iterated streams, all while bounding used memory and respecting
     group parallelism and throttling.
 
@@ -830,18 +841,19 @@
 
     def __imap_sync(
         self,
         iterable: ImapTarget[ItemType],
         func: Callable[[ItemType], ResultType],
         *,
         key: Optional[Callable[[ItemType], GroupType]] = None,
-        throttle: ThrottleType[GroupType, ItemType, ResultType] = 0
+        throttle: ThrottleType[GroupType, ItemType, ResultType] = 0,
+        block: bool = False
     ) -> Iterator[ResultType]:
-        if is_usable_queue(iterable):
-            items = queue_iter(iterable)  # type: ignore
+        if isinstance(iterable, QuenouilleQueueProtocol):
+            items = queue_iter(iterable, block)  # type: ignore
         else:
             items = iterable
 
         items = cast(Iterator[ItemType], items)
 
         # TODO: make throttling work per group
         timers = TimedHeapSet()  # type: TimedHeapSet[GroupType]
@@ -871,15 +883,17 @@
         iterable: ImapTarget[ItemType],
         func: Callable[[ItemType], ResultType],
         *,
         ordered: bool = False,
         key: Optional[Callable[[ItemType], GroupType]] = None,
         parallelism: ParallelismType[GroupType] = 1,
         buffer_size: int = DEFAULT_BUFFER_SIZE,
-        throttle: ThrottleType[GroupType, ItemType, ResultType] = 0
+        throttle: ThrottleType[GroupType, ItemType, ResultType] = 0,
+        block: bool = False,
+        panic: Optional[Callable[[], None]] = None
     ) -> Iterator[ResultType]:
         if self.dummy:
             return self.__imap_sync(iterable, func, key=key, throttle=throttle)
 
         # Cannot run in multiple threads
         if self.imap_lock.locked():
             raise RuntimeError(
@@ -891,15 +905,15 @@
             raise RuntimeError("cannot use thread pool after teardown")
 
         assert not self.boot_barrier.broken
 
         self.imap_lock.acquire()
 
         iterator = None
-        iterable_is_queue = is_usable_queue(iterable)
+        iterable_is_queue = isinstance(iterable, QuenouilleQueueProtocol)
 
         if not iterable_is_queue:
             iterator = iter(iterable)  # type: ignore
 
         # State
         self.throttled_groups.update(key, throttle)
         job_counter = count()
@@ -931,15 +945,15 @@
                     if job is None:
                         # Else we consume the iterator to find one
                         try:
                             if not iterable_is_queue:
                                 item = next(iterator)  # type: ignore
                             else:
                                 try:
-                                    item = iterable.get_nowait()  # type: ignore
+                                    item = iterable.get(block)  # type: ignore
                                 except Empty:
                                     if state.has_running_tasks():
                                         state.wait_for_any_task_to_finish()
                                         continue
                                     else:
                                         raise StopIteration
                         except StopIteration:
@@ -968,17 +982,24 @@
 
                     # Registering the job
                     buffer.register_job(job)
                     state.start_task()
                     self.job_queue.put(job)
 
             except BaseException as e:
+                # NOTE: this can happen multiple times, with nested
+                # exception or when cleaning up as we panic and
+                # unblock the user's queue or iterator for instance.
+                # This said, this is probably alright...
                 smash(self.output_queue, e)
 
         def cleanup(normal_exit: bool = True) -> None:
+            if not normal_exit and panic is not None:
+                panic()
+
             # NOTE: this is somewhat of a lock to avoid double firing of the
             # cleanup function in some race conditions with sys.excepthook
             self.cleanup = None
 
             end_event.set()
 
             # Clearing the job queue to cancel next jobs
@@ -1075,62 +1096,74 @@
         self,
         iterable: ImapTarget[ItemType],
         func: Callable[[ItemType], ResultType],
         *,
         key: Optional[Callable[[ItemType], GroupType]] = None,
         parallelism: ParallelismType[GroupType] = 1,
         buffer_size: int = DEFAULT_BUFFER_SIZE,
-        throttle: ThrottleType[GroupType, ItemType, ResultType] = 0
+        throttle: ThrottleType[GroupType, ItemType, ResultType] = 0,
+        block: bool = False,
+        panic: Optional[Callable[[], None]] = None
     ) -> Iterator[ResultType]:
         validate_imap_kwargs(
             iterable=iterable,
             func=func,
             key=key,
             parallelism=parallelism,
             buffer_size=buffer_size,
             throttle=throttle,
+            block=block,
+            panic=panic,
         )
 
         return self.__imap(
             iterable,
             func,
             ordered=False,
             key=key,
             parallelism=parallelism,
             buffer_size=buffer_size,
             throttle=throttle,
+            block=block,
+            panic=panic,
         )
 
     def imap(
         self,
         iterable: ImapTarget[ItemType],
         func: Callable[[ItemType], ResultType],
         *,
         key: Optional[Callable[[ItemType], GroupType]] = None,
         parallelism: ParallelismType[GroupType] = 1,
         buffer_size: int = DEFAULT_BUFFER_SIZE,
-        throttle: ThrottleType[GroupType, ItemType, ResultType] = 0
+        throttle: ThrottleType[GroupType, ItemType, ResultType] = 0,
+        block: bool = False,
+        panic: Optional[Callable[[], None]] = None
     ) -> Iterator[ResultType]:
         validate_imap_kwargs(
             iterable=iterable,
             func=func,
             key=key,
             parallelism=parallelism,
             buffer_size=buffer_size,
             throttle=throttle,
+            block=block,
+            panic=panic,
         )
 
         return self.__imap(
             iterable,
             func,
             ordered=True,
             key=key,
             parallelism=parallelism,
             buffer_size=buffer_size,
             throttle=throttle,
+            block=block,
+            panic=panic,
         )
 
 
 def imap_unordered(
     iterable: ImapTarget[ItemType],
     func: Callable[[ItemType], ResultType],
     threads: Optional[int] = None,
@@ -1139,15 +1172,17 @@
     parallelism: ParallelismType[GroupType] = 1,
     buffer_size: int = DEFAULT_BUFFER_SIZE,
     throttle: ThrottleType[GroupType, ItemType, ResultType] = 0,
     initializer: Optional[Callable[..., None]] = None,
     initargs: Iterable[Any] = tuple(),
     wait: bool = True,
     daemonic: bool = False,
-    excepthook: bool = False
+    excepthook: bool = False,
+    block: bool = False,
+    panic: Optional[Callable[[], None]] = None
 ) -> Iterator[ResultType]:
     validate_threadpool_kwargs(
         "threads",
         threads,
         initializer=initializer,
         initargs=initargs,
         wait=wait,
@@ -1157,14 +1192,16 @@
     validate_imap_kwargs(
         iterable=iterable,
         func=func,
         key=key,
         parallelism=parallelism,
         buffer_size=buffer_size,
         throttle=throttle,
+        block=block,
+        panic=panic,
     )
 
     # If we know the size of the iterable, and this size is less than the
     # number of desired threads, we adjust the number of threads accordingly
     if threads is not None and isinstance(iterable, Sized):
         threads = min(len(iterable), threads)
 
@@ -1180,14 +1217,16 @@
             yield from executor.imap_unordered(
                 iterable,
                 func,
                 key=key,
                 parallelism=parallelism,
                 buffer_size=buffer_size,
                 throttle=throttle,
+                block=block,
+                panic=panic,
             )
 
     return generator()
 
 
 def imap(
     iterable: ImapTarget[ItemType],
@@ -1198,15 +1237,17 @@
     parallelism: ParallelismType[GroupType] = 1,
     buffer_size: int = DEFAULT_BUFFER_SIZE,
     throttle: ThrottleType[GroupType, ItemType, ResultType] = 0,
     initializer: Optional[Callable[..., None]] = None,
     initargs: Iterable[Any] = tuple(),
     wait: bool = True,
     daemonic: bool = False,
-    excepthook: bool = False
+    excepthook: bool = False,
+    block: bool = False,
+    panic: Optional[Callable[[], None]] = None
 ) -> Iterator[ResultType]:
     validate_threadpool_kwargs(
         "threads",
         threads,
         initializer=initializer,
         initargs=initargs,
         wait=wait,
@@ -1216,14 +1257,16 @@
     validate_imap_kwargs(
         iterable=iterable,
         func=func,
         key=key,
         parallelism=parallelism,
         buffer_size=buffer_size,
         throttle=throttle,
+        block=block,
+        panic=panic,
     )
 
     # If we know the size of the iterable, and this size is less than the
     # number of desired threads, we adjust the number of threads accordingly
     if threads is not None and isinstance(iterable, Sized):
         threads = min(len(iterable), threads)
 
@@ -1239,14 +1282,16 @@
             yield from executor.imap(
                 iterable,
                 func,
                 key=key,
                 parallelism=parallelism,
                 buffer_size=buffer_size,
                 throttle=throttle,
+                block=block,
+                panic=panic,
             )
 
     return generator()
 
 
 def generate_function_doc(ordered: bool = False) -> str:
     disclaimer = "Note that results will be yielded in an arbitrary order."
```

### Comparing `quenouille-1.8.0/quenouille/utils.py` & `quenouille-1.9.0/quenouille/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,28 +35,22 @@
 
 
 def smash(q: "Queue[ItemType]", v: ItemType) -> None:
     clear(q)
     q.put_nowait(v)
 
 
-def queue_iter(q: "Queue[ItemType]") -> Iterator[ItemType]:
+def queue_iter(q: "Queue[ItemType]", block: bool = False) -> Iterator[ItemType]:
     while True:
         try:
-            yield q.get_nowait()
+            yield q.get(block)
         except Empty:
             break
 
 
-def is_usable_queue(v) -> bool:
-    # NOTE: get_nowait is the only method used by quenouille when working
-    # on a queue given by the user, as of now.
-    return hasattr(v, "get_nowait") and callable(v.get_nowait)
-
-
 # As per: https://docs.python.org/3/library/concurrent.futures.html#concurrent.futures.ThreadPoolExecutor
 def get_default_maxworkers() -> int:
     return min(32, (os.cpu_count() or 1) + 4)
 
 
 class SmartTimer(Timer):
     """
```

### Comparing `quenouille-1.8.0/quenouille.egg-info/PKG-INFO` & `quenouille-1.9.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quenouille
-Version: 1.8.0
+Version: 1.9.0
 Summary: A library of multithreaded iterator workflows.
 Home-page: http://github.com/medialab/quenouille
 Author: Guillaume Plique
 Author-email: kropotkinepiotr@gmail.com
 License: MIT
 Description: [![Build Status](https://github.com/medialab/quenouille/workflows/Tests/badge.svg)](https://github.com/medialab/quenouille/actions)
         
@@ -22,27 +22,27 @@
         
         ```
         pip install quenouille
         ```
         
         ## Usage
         
-        * [imap, imap_unordered](#imap_unordered-imap)
-        * [ThreadPoolExecutor](#threadpoolexecutor)
-          * [#.imap, #.imap_unordered](#executor-imap)
-          * [#.shutdown](#shutdown)
-        * [NamedLocks](#namedlocks)
-        * [Miscellaneous notes](#miscellaneous-notes)
-          * [The None group](#the-none-group)
-          * [Parallelism > workers](#parallelism--workers)
-          * [Callable parallelism guarantees](#callable-parallelism-guarantees)
-          * [Parallelism vs. throttling](#parallelism-vs-throttling)
-          * [Adding entropy to throttle](#adding-entropy-to-throttle)
-          * [Caveats regarding exception raising](#caveats-regarding-exception-raising)
-          * [Caveats of using imap with queues](#caveats-of-using-imap-with-queues)
+        - [imap, imap_unordered](#imap_unordered-imap)
+        - [ThreadPoolExecutor](#threadpoolexecutor)
+          - [#.imap, #.imap_unordered](#executor-imap)
+          - [#.shutdown](#shutdown)
+        - [NamedLocks](#namedlocks)
+        - [Miscellaneous notes](#miscellaneous-notes)
+          - [The None group](#the-none-group)
+          - [Parallelism > workers](#parallelism--workers)
+          - [Callable parallelism guarantees](#callable-parallelism-guarantees)
+          - [Parallelism vs. throttling](#parallelism-vs-throttling)
+          - [Adding entropy to throttle](#adding-entropy-to-throttle)
+          - [Caveats regarding exception raising](#caveats-regarding-exception-raising)
+          - [Caveats of using imap with queues](#caveats-of-using-imap-with-queues)
         
         ### imap, imap_unordered
         
         Function lazily consuming an iterable and applying the desired function over the yielded items in a multithreaded fashion.
         
         This function is also able to respect group constraints regarding parallelism and throttling: for instance, if you need to download urls in a multithreaded fashion and need to ensure that you won't hit the same domain more than twice at the same time, this function can be given proper settings to ensure the desired behavior.
         
@@ -99,29 +99,31 @@
           print(html)
         
         # Only load 10 urls into memory when attempting to find next suitable job
         for html in imap(urls(), fetch, 10, key=get_domain_name, throttle=5, buffer_size=10):
           print(html)
         ```
         
-        *Arguments*
+        _Arguments_
         
-        * **iterable** *(iterable)*: Any python iterable.
-        * **func** *(callable)*: Function used to perform the desired tasks. The function takes an item yielded by the given iterable as single argument. Note that since this function will be dispatched in worker threads, so you should ensure it is thread-safe.
-        * **threads** *(int, optional)*: Maximum number of threads to use. Defaults to `min(32, os.cpu_count() + 1)`. Note that it can be `0`, in which case no threads will be used and everything will run synchronously (this can be useful for debugging or to avoid duplicating code sometimes).
-        * **key** *(callable, optional)*: Function returning to which "group" a given item is supposed to belong. This will be used to ensure maximum parallelism is respected.
-        * **parallelism** *(int or callable, optional)* [`1`]: Number of threads allowed to work on a same group at once. Can also be a function taking a group and returning its parallelism.
-        * **buffer_size** *(int, optional)* [`1024`]: Maximum number of items the function will buffer into memory while attempting to find an item that can be passed to a worker immediately, all while respecting throttling and group parallelism.
-        * **throttle** *(int or float or callable, optional)*: Optional throttle time, in seconds, to wait before processing the next item of a given group. Can also be a function taking last group, item and result and returning next throttle time for this group.
-        * **initializer** *(callable, optional)*: Function to run at the start of each thread worker. Can be useful to setup [thread-local data](https://docs.python.org/3/library/threading.html#thread-local-data), for instance. Remember this function must be threadsafe and should not block because the thread pool will wait for each thread to be correctly booted before being able to proceed. If one of the function calls fails, the thread pool will raise a `quenouille.exceptions.BrokenThreadPool` error and terminate immediately.
-        * **initargs** *(iterable, optional)*: Arguments to pass to the `initializer` function.
-        * **wait** *(bool, optional)* [`True`]: Whether to join worker threads, i.e. wait for them to end, when shutting down the executor. Set this to `False` if you need to go on quickly without waiting for your worker threads to end when cleaning up the executor's resources. Just note that if you spawn other thread-intensive tasks or other executors afterwards in rapid succession, you might start too many threads at once.
-        * **daemonic** *(bool, optional)* [`False`]: whether to spawn daemonic worker. If your worker are daemonic, the interpreter will not wait for them to end when exiting. This can be useful, combined to `wait=False`, for instance, if you want your program to exit as soon as hitting ctrl+C (you might want to avoid this if your threads need to cleanup things on exit as they will be abruptly shut down).
+        - **iterable** _(iterable)_: Any python iterable.
+        - **func** _(callable)_: Function used to perform the desired tasks. The function takes an item yielded by the given iterable as single argument. Note that since this function will be dispatched in worker threads, so you should ensure it is thread-safe.
+        - **threads** _(int, optional)_: Maximum number of threads to use. Defaults to `min(32, os.cpu_count() + 1)`. Note that it can be `0`, in which case no threads will be used and everything will run synchronously (this can be useful for debugging or to avoid duplicating code sometimes).
+        - **key** _(callable, optional)_: Function returning to which "group" a given item is supposed to belong. This will be used to ensure maximum parallelism is respected.
+        - **parallelism** _(int or callable, optional)_ [`1`]: Number of threads allowed to work on a same group at once. Can also be a function taking a group and returning its parallelism.
+        - **buffer_size** _(int, optional)_ [`1024`]: Maximum number of items the function will buffer into memory while attempting to find an item that can be passed to a worker immediately, all while respecting throttling and group parallelism.
+        - **throttle** _(int or float or callable, optional)_: Optional throttle time, in seconds, to wait before processing the next item of a given group. Can also be a function taking last group, item and result and returning next throttle time for this group.
+        - **block** _(bool, optional)_ [`False`]: Whether to block when using the `get` method of the given queue.
+        - **panic** _(callable, optional)_: Function that will be called when the process has errored. Useful to unblock some functions and avoid deadlock in specific situations. Note that this function will not be called when synchronous (i.e. when not using additional threads).
+        - **initializer** _(callable, optional)_: Function to run at the start of each thread worker. Can be useful to setup [thread-local data](https://docs.python.org/3/library/threading.html#thread-local-data), for instance. Remember this function must be threadsafe and should not block because the thread pool will wait for each thread to be correctly booted before being able to proceed. If one of the function calls fails, the thread pool will raise a `quenouille.exceptions.BrokenThreadPool` error and terminate immediately.
+        - **initargs** _(iterable, optional)_: Arguments to pass to the `initializer` function.
+        - **wait** _(bool, optional)_ [`True`]: Whether to join worker threads, i.e. wait for them to end, when shutting down the executor. Set this to `False` if you need to go on quickly without waiting for your worker threads to end when cleaning up the executor's resources. Just note that if you spawn other thread-intensive tasks or other executors afterwards in rapid succession, you might start too many threads at once.
+        - **daemonic** _(bool, optional)_ [`False`]: whether to spawn daemonic worker. If your worker are daemonic, the interpreter will not wait for them to end when exiting. This can be useful, combined to `wait=False`, for instance, if you want your program to exit as soon as hitting ctrl+C (you might want to avoid this if your threads need to cleanup things on exit as they will be abruptly shut down).
         
-        *Using a queue rather than an iterable*
+        _Using a queue rather than an iterable_
         
         If you need to add new items to process as a result of performing tasks (when designing a web crawler for instance, where each downloaded page will yield new pages to explore further down), know that the `imap` and `imap_unordered` function also accepts queues as input:
         
         ```python
         from queue import Queue
         from quenouille import imap
         
@@ -175,40 +177,42 @@
         executor = ThreadPoolExecutor()
         executor.imap(range(10), worker)
         executor.shutdown(wait=False)
         ```
         
         Note that your throttling state is kept between multiple `imap` and `imap_unordered` calls so you don't end up perform some tasks too soon. But keep in mind this state is tied to the `key` function you provide to remain consistent, so if you change the used `key`, the throttling state will be reset.
         
-        *Arguments*
+        _Arguments_
         
-        * **max_workers** *(int, optional)*: Maximum number of threads to use. Defaults to `min(32, os.cpu_count() + 1)`. Note that it can be `0`, in which case no threads will be used and everything will run synchronously (this can be useful for debugging or to avoid duplicating code sometimes).
-        * **initializer** *(callable, optional)*: Function to run at the start of each thread worker. Can be useful to setup [thread-local data](https://docs.python.org/3/library/threading.html#thread-local-data), for instance. Remember this function must be threadsafe and should not block because the thread pool will wait for each thread to be correctly booted before being able to proceed. If one of the function calls fails, the thread pool will raise a `quenouille.exceptions.BrokenThreadPool` error and terminate immediately.
-        * **initargs** *(iterable, optional)*: Arguments to pass to the `initializer` function.
-        * **wait** *(bool, optional)* [`True`]: Whether to join worker threads, i.e. wait for them to end, when closing the executor. Set this to `False` if you need to go on quickly without waiting for your worker threads to end when cleaning up the executor's resources. Just note that if you spawn other thread-intensive tasks or other executors afterwards in rapid succession, you might start too many threads at once.
-        * **daemonic** *(bool, optional)* [`False`]: whether to spawn daemonic worker. If your worker are daemonic, the interpreter will not wait for them to end when exiting. This can be useful, combined to `wait=False`, for instance, if you want your program to exit as soon as hitting ctrl+C (you might want to avoid this if your threads need to cleanup things on exit as they will be abruptly shut down).
+        - **max_workers** _(int, optional)_: Maximum number of threads to use. Defaults to `min(32, os.cpu_count() + 1)`. Note that it can be `0`, in which case no threads will be used and everything will run synchronously (this can be useful for debugging or to avoid duplicating code sometimes).
+        - **initializer** _(callable, optional)_: Function to run at the start of each thread worker. Can be useful to setup [thread-local data](https://docs.python.org/3/library/threading.html#thread-local-data), for instance. Remember this function must be threadsafe and should not block because the thread pool will wait for each thread to be correctly booted before being able to proceed. If one of the function calls fails, the thread pool will raise a `quenouille.exceptions.BrokenThreadPool` error and terminate immediately.
+        - **initargs** _(iterable, optional)_: Arguments to pass to the `initializer` function.
+        - **wait** _(bool, optional)_ [`True`]: Whether to join worker threads, i.e. wait for them to end, when closing the executor. Set this to `False` if you need to go on quickly without waiting for your worker threads to end when cleaning up the executor's resources. Just note that if you spawn other thread-intensive tasks or other executors afterwards in rapid succession, you might start too many threads at once.
+        - **daemonic** _(bool, optional)_ [`False`]: whether to spawn daemonic worker. If your worker are daemonic, the interpreter will not wait for them to end when exiting. This can be useful, combined to `wait=False`, for instance, if you want your program to exit as soon as hitting ctrl+C (you might want to avoid this if your threads need to cleanup things on exit as they will be abruptly shut down).
         
         <h4 id="executor-imap">#.imap, #.imap_unordered</h4>
         
         Basically the same as described [here](#imap_unordered-imap) with the following arguments:
         
-        * **iterable** *(iterable)*: Any python iterable.
-        * **func** *(callable)*: Function used to perform the desired tasks. The function takes an item yielded by the given iterable as single argument. Note that since this function will be dispatched in worker threads, so you should ensure it is thread-safe.
-        * **key** *(callable, optional)*: Function returning to which "group" a given item is supposed to belong. This will be used to ensure maximum parallelism is respected.
-        * **parallelism** *(int or callable, optional)* [`1`]: Number of threads allowed to work on a same group at once. Can also be a function taking a group and returning its parallelism.
-        * **buffer_size** *(int, optional)* [`1024`]: Maximum number of items the function will buffer into memory while attempting to find an item that can be passed to a worker immediately, all while respecting throttling and group parallelism.
-        * **throttle** *(int or float or callable, optional)*: Optional throttle time, in seconds, to wait before processing the next item of a given group. Can also be a function taking last group, item and result and returning next throttle time for this group.
+        - **iterable** _(iterable)_: Any python iterable.
+        - **func** _(callable)_: Function used to perform the desired tasks. The function takes an item yielded by the given iterable as single argument. Note that since this function will be dispatched in worker threads, so you should ensure it is thread-safe.
+        - **key** _(callable, optional)_: Function returning to which "group" a given item is supposed to belong. This will be used to ensure maximum parallelism is respected.
+        - **parallelism** _(int or callable, optional)_ [`1`]: Number of threads allowed to work on a same group at once. Can also be a function taking a group and returning its parallelism.
+        - **buffer_size** _(int, optional)_ [`1024`]: Maximum number of items the function will buffer into memory while attempting to find an item that can be passed to a worker immediately, all while respecting throttling and group parallelism.
+        - **throttle** _(int or float or callable, optional)_: Optional throttle time, in seconds, to wait before processing the next item of a given group. Can also be a function taking last group, item and result and returning next throttle time for this group.
+        - **block** _(bool, optional)_ [`False`]: Whether to block when using the `get` method of the given queue.
+        - **panic** _(callable, optional)_: Function that will be called when the process has errored. Useful to unblock some functions and avoid deadlock in specific situations. Note that this function will not be called when synchronous (i.e. when not using additional threads).
         
         #### #.shutdown
         
         Method used to explicitly shutdown the executor.
         
-        *Arguments*
+        _Arguments_
         
-        * **wait** *(bool, optional)* [`True`]: Whether to join worker threads, i.e. wait for them to end, when shutting down the executor. Set this to `False` if you need to go on quickly without waiting for your worker threads to end when cleaning up the executor's resources. Just note that if you spawn other thread-intensive tasks or other executors afterwards in rapid succession, you might start too many threads at once.
+        - **wait** _(bool, optional)_ [`True`]: Whether to join worker threads, i.e. wait for them to end, when shutting down the executor. Set this to `False` if you need to go on quickly without waiting for your worker threads to end when cleaning up the executor's resources. Just note that if you spawn other thread-intensive tasks or other executors afterwards in rapid succession, you might start too many threads at once.
         
         ### NamedLocks
         
         A weakref dictionary of locks useful to make some tasks based on keys threadsafe, e.g. if you need to ensure that two threads will not be writing to the same file at once.
         
         ```python
         from quenouille import NamedLocks
@@ -257,15 +261,15 @@
         # Waiting 5 + (between 0 and 2) seconds
         def throttle(group, item, result):
           return 5 + (2 * random())
         ```
         
         #### Caveats regarding exception raising
         
-        *Deferred generator usage exception deadlocks*
+        _Deferred generator usage exception deadlocks_
         
         If you consume a generator returned by `imap/imap_unordered` somewhere else than where you created it, you may end up in a deadlock if you raise an exception.
         
         This is not important when using `daemonic=True` but you might stumble upon segfaults on exit because of python reasons beyond my control.
         
         ```python
         # Safe
@@ -287,15 +291,15 @@
         
         for item in it:
           raise RuntimeError
         ```
         
         #### Caveats of using imap with queues
         
-        *Typical deadlocks*
+        _Typical deadlocks_
         
         Even if `imap` can process an input queue, you should avoid to find yourself in a situation where adding to the queue might block execution if you don't want to end in a deadlock. It can be easy to footgun yourself if your queue has a `maxsize`, for instance:
         
         ```python
         from queue import Queue
         from quenouille import imap
         
@@ -310,21 +314,21 @@
             # This will put you in a deadlock because this will block
             # because of the queue `maxsize` set to 2
             job_queue.put(4)
         
           print(i)
         ```
         
-        *Design choices*
+        _Design choices_
         
         To enable you to add items to the queue in the loop body and so it can safely detect when your queue is drained without race condition, `quenouille` acknowledges that a task is finished only after what you execute in the loop body is done.
         
         This means that sometimes it might be more performant to only add items to the queue from the worker functions rather than from the loop body.
         
-        *queue.task_done*
+        _queue.task_done_
         
         For now, `quenouille` does not call `queue.task_done` for you, so this remains your responsability, if you want to be able to call `queue.join` down the line.
         
 Keywords: url
 Platform: UNKNOWN
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
```

### Comparing `quenouille-1.8.0/setup.py` & `quenouille-1.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("./README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="quenouille",
-    version="1.8.0",
+    version="1.9.0",
     description="A library of multithreaded iterator workflows.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="http://github.com/medialab/quenouille",
     license="MIT",
     author="Guillaume Plique",
     author_email="kropotkinepiotr@gmail.com",
```

