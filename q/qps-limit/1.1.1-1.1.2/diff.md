# Comparing `tmp/qps_limit-1.1.1-py3-none-any.whl.zip` & `tmp/qps_limit-1.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 5719 bytes, number of entries: 8
--rw-rw-r--  2.0 unx      165 b- defN 23-Jul-23 06:28 qps_limit/__init__.py
--rw-rw-r--  2.0 unx     6926 b- defN 23-Jul-23 06:28 qps_limit/limiter.py
+Zip file size: 5742 bytes, number of entries: 8
+-rw-rw-r--  2.0 unx      165 b- defN 23-Aug-01 15:37 qps_limit/__init__.py
+-rw-rw-r--  2.0 unx     7116 b- defN 23-Aug-01 15:36 qps_limit/limiter.py
 -rw-rw-r--  2.0 unx     5474 b- defN 23-Jul-07 07:33 qps_limit/run.py
--rw-rw-r--  2.0 unx     2803 b- defN 23-Jul-23 06:29 qps_limit-1.1.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-23 06:29 qps_limit-1.1.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       10 b- defN 23-Jul-23 06:29 qps_limit-1.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx        1 b- defN 23-Jul-23 06:29 qps_limit-1.1.1.dist-info/zip-safe
-?rw-rw-r--  2.0 unx      621 b- defN 23-Jul-23 06:29 qps_limit-1.1.1.dist-info/RECORD
-8 files, 16092 bytes uncompressed, 4635 bytes compressed:  71.2%
+-rw-rw-r--  2.0 unx     2783 b- defN 23-Aug-01 15:38 qps_limit-1.1.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Aug-01 15:38 qps_limit-1.1.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       10 b- defN 23-Aug-01 15:38 qps_limit-1.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-Aug-01 15:38 qps_limit-1.1.2.dist-info/zip-safe
+?rw-rw-r--  2.0 unx      621 b- defN 23-Aug-01 15:38 qps_limit-1.1.2.dist-info/RECORD
+8 files, 16262 bytes uncompressed, 4658 bytes compressed:  71.4%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: qps_limit/limiter.py
 Comment: 
 
 Filename: qps_limit/run.py
 Comment: 
 
-Filename: qps_limit-1.1.1.dist-info/METADATA
+Filename: qps_limit-1.1.2.dist-info/METADATA
 Comment: 
 
-Filename: qps_limit-1.1.1.dist-info/WHEEL
+Filename: qps_limit-1.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: qps_limit-1.1.1.dist-info/top_level.txt
+Filename: qps_limit-1.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: qps_limit-1.1.1.dist-info/zip-safe
+Filename: qps_limit-1.1.2.dist-info/zip-safe
 Comment: 
 
-Filename: qps_limit-1.1.1.dist-info/RECORD
+Filename: qps_limit-1.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## qps_limit/__init__.py

```diff
@@ -1,8 +1,8 @@
-__version__ = '1.1.1'
+__version__ = '1.1.2'
 
 from .limiter import Limiter
 from .run import async_batch_run, batch_run
 
 __all__ = [
     'batch_run',
     'async_batch_run',
```

## qps_limit/limiter.py

```diff
@@ -19,25 +19,27 @@
         params: Callable,
         callback: Optional[Callable] = None,
         num_workers: int = 1,
         worker_max_qps: Optional[float] = None,
         streaming: bool = False,
         ordered: bool = True,
         verbose: bool = False,
+        debug_steps: int = 0,
         warmup_steps: int = 1,
         max_coroutines: int = 128
     ) -> Callable:
         self.func = func
         self.params = params
         self.callback = callback
         self.num_workers = num_workers
         self.worker_max_qps = worker_max_qps
         self.streaming = streaming
         self.ordered = ordered
         self.verbose = verbose
+        self.debug_steps = debug_steps
         self.warmup_steps = warmup_steps
         self.max_coroutines = max_coroutines
 
         self.logger = logging.getLogger(__name__)
         self.logger.setLevel(logging.INFO)
         handler = logging.StreamHandler()
         handler.setLevel(logging.INFO)
@@ -98,15 +100,16 @@
             progress_cnt += 1
         progress_bar.close()
         with self.worker_time.get_lock():
             self.worker_time.value = progress_bar.last_print_t - progress_bar.start_t
 
     def _worker(self, mod: int):
         def make_worker_iterator():
-            for idx, (args, kwargs) in enumerate(self.params()):
+            worker_params = itertools.islice(self.params(), self.debug_steps) if self.debug_steps > 0 else self.params()
+            for idx, (args, kwargs) in enumerate(worker_params):
                 if idx % self.num_workers == mod:
                     yield args, kwargs
 
         batch_run_func = batch_run if not self.streaming else streaming_batch_run
         for idx, res in batch_run_func(
             func=self.func,
             params=make_worker_iterator(),
```

## Comparing `qps_limit-1.1.1.dist-info/METADATA` & `qps_limit-1.1.2.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: qps-limit
-Version: 1.1.1
+Version: 1.1.2
 Summary: Run functions under any limited rate
 Home-page: https://github.com/antct/qps-limit
 Author: tt
 Author-email: 527892245@qq.com
 License: GPLv2
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -105,9 +104,7 @@
 resource = None
 
 async def func(n):
     global resource
     if resource is None:
         resource = {}
 ```
-
-
```

