# Comparing `tmp/kioss-0.2.6.tar.gz` & `tmp/kioss-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kioss-0.2.6.tar", last modified: Tue Aug  1 05:31:55 2023, max compression
+gzip compressed data, was "kioss-0.2.7.tar", last modified: Tue Aug  1 13:15:46 2023, max compression
```

## Comparing `kioss-0.2.6.tar` & `kioss-0.2.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 05:31:55.160259 kioss-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-01 05:31:46.000000 kioss-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-08-01 05:31:55.160259 kioss-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-08-01 05:31:46.000000 kioss-0.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 05:31:55.160259 kioss-0.2.6/kioss/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-01 05:31:46.000000 kioss-0.2.6/kioss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18761 2023-08-01 05:31:46.000000 kioss-0.2.6/kioss/pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-08-01 05:31:46.000000 kioss-0.2.6/kioss/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 05:31:55.160259 kioss-0.2.6/kioss.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-08-01 05:31:55.000000 kioss-0.2.6/kioss.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-08-01 05:31:55.000000 kioss-0.2.6/kioss.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 05:31:55.000000 kioss-0.2.6/kioss.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-01 05:31:55.000000 kioss-0.2.6/kioss.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 05:31:55.160259 kioss-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-08-01 05:31:46.000000 kioss-0.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 05:31:55.160259 kioss-0.2.6/test/
--rw-r--r--   0 runner    (1001) docker     (123)    11258 2023-08-01 05:31:46.000000 kioss-0.2.6/test/test_pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-08-01 05:31:46.000000 kioss-0.2.6/test/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:15:46.827067 kioss-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-01 13:15:36.000000 kioss-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-08-01 13:15:46.827067 kioss-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-08-01 13:15:36.000000 kioss-0.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:15:46.823066 kioss-0.2.7/kioss/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-01 13:15:36.000000 kioss-0.2.7/kioss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19453 2023-08-01 13:15:36.000000 kioss-0.2.7/kioss/pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-08-01 13:15:36.000000 kioss-0.2.7/kioss/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:15:46.827067 kioss-0.2.7/kioss.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-08-01 13:15:46.000000 kioss-0.2.7/kioss.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-08-01 13:15:46.000000 kioss-0.2.7/kioss.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 13:15:46.000000 kioss-0.2.7/kioss.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-01 13:15:46.000000 kioss-0.2.7/kioss.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 13:15:46.827067 kioss-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-08-01 13:15:36.000000 kioss-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:15:46.827067 kioss-0.2.7/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    12028 2023-08-01 13:15:36.000000 kioss-0.2.7/test/test_pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-08-01 13:15:36.000000 kioss-0.2.7/test/test_util.py
```

### Comparing `kioss-0.2.6/LICENSE` & `kioss-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `kioss-0.2.6/README.md` & `kioss-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `kioss-0.2.6/kioss/pipe.py` & `kioss-0.2.7/kioss/pipe.py`

 * *Files 2% similar despite different names*

```diff
@@ -407,32 +407,49 @@
         if isinstance(next_elem, _CatchedError):
             raise next_elem.exception
         else:
             return next_elem
 
 
 class _BatchingPipe(Pipe[List[T]]):
+    """
+    Batch an input iterator and yields its elements packed in a list when one of the following is True:
+    - len(batch) == size
+    - the time elapsed between the first next() call on input iterator and last received elements is grater than secs
+    - the next element reception thrown an exception (it is stored in self.to_be_raised and will be raised during the next call to self.__next__)
+    """
     def __init__(self, iterator: Iterator[T], size: int, secs: float) -> None:
         super().__init__(iterator)
         self.size = size
         self.secs = secs
+        self.to_be_raised: Exception = None
 
     def __next__(self) -> List[T]:
+        if self.to_be_raised:
+            e = self.to_be_raised
+            self.to_be_raised = None
+            raise e
         start_time = time.time()
         batch = None
         try:
             batch = [super().__next__()]
             while len(batch) < self.size and (time.time() - start_time) < self.secs:
                 batch.append(super().__next__())
             return batch
         except StopIteration:
             if batch:
                 return batch
-            else:
-                raise
+            raise
+        except Exception as e:
+            if batch:
+                self.to_be_raised = e
+                return batch
+            raise
+
+
 
 
 class _ConcurrentlyMergingPipe(Pipe[T]):
     MAX_NUM_WAITING_ELEMS_PER_THREAD = 16
 
     def __init__(self, iterators: List[Iterator[T]]) -> None:
         super().__init__(
```

### Comparing `kioss-0.2.6/kioss/util.py` & `kioss-0.2.7/kioss/util.py`

 * *Files identical despite different names*

### Comparing `kioss-0.2.6/test/test_pipe.py` & `kioss-0.2.7/test/test_pipe.py`

 * *Files 3% similar despite different names*

```diff
@@ -230,14 +230,27 @@
         )
         self.assertListEqual(
             Pipe(range(8)).batch(size=1).collect(),
             list(map(lambda x: [x], range(8))),
         )
         self.assertListEqual(Pipe(range(8)).batch(size=8).collect(), [list(range(8))])
         self.assertEqual(len(Pipe(range(8)).slow(10).batch(secs=0.09).collect()), 7)
+        # assert batch gracefully yields if next elem throw exception
+        self.assertListEqual(
+            Pipe("01234-56789").map(int).batch(2).catch(ValueError, ignore=True).collect(),
+            [[0, 1], [2, 3], [4], [5, 6], [7, 8], [9]]
+        )
+        self.assertListEqual(
+            Pipe("0123-56789").map(int).batch(2).catch(ValueError, ignore=True).collect(),
+            [[0, 1], [2, 3], [5, 6], [7, 8], [9]]
+        )
+        self.assertListEqual(
+            Pipe("0123-56789").map(int).batch(2).catch(ValueError, ignore=False).map(lambda potential_error: [potential_error] if isinstance(potential_error, Exception) else potential_error).flatten().map(type).collect(),
+            [int, int, int, int, ValueError, int, int, int, int, int]
+        )
 
     @parameterized.expand(
         [
             [n_workers, worker_type]
             for n_workers in [None, 1]
             for worker_type in Pipe.SUPPORTED_WORKER_TYPES
         ]
```

### Comparing `kioss-0.2.6/test/test_util.py` & `kioss-0.2.7/test/test_util.py`

 * *Files identical despite different names*

