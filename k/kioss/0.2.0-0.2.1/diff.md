# Comparing `tmp/kioss-0.2.0.tar.gz` & `tmp/kioss-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kioss-0.2.0.tar", last modified: Mon Jul 31 23:25:17 2023, max compression
+gzip compressed data, was "kioss-0.2.1.tar", last modified: Mon Jul 31 23:31:09 2023, max compression
```

## Comparing `kioss-0.2.0.tar` & `kioss-0.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 23:25:17.564279 kioss-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-31 23:25:07.000000 kioss-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-31 23:25:17.564279 kioss-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-07-31 23:25:07.000000 kioss-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 23:25:17.564279 kioss-0.2.0/kioss/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-31 23:25:07.000000 kioss-0.2.0/kioss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19401 2023-07-31 23:25:07.000000 kioss-0.2.0/kioss/pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-31 23:25:07.000000 kioss-0.2.0/kioss/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 23:25:17.564279 kioss-0.2.0/kioss.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-31 23:25:17.000000 kioss-0.2.0/kioss.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-31 23:25:17.000000 kioss-0.2.0/kioss.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 23:25:17.000000 kioss-0.2.0/kioss.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-31 23:25:17.000000 kioss-0.2.0/kioss.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 23:25:17.564279 kioss-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-31 23:25:07.000000 kioss-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 23:25:17.564279 kioss-0.2.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)    12002 2023-07-31 23:25:07.000000 kioss-0.2.0/test/test_pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-31 23:25:07.000000 kioss-0.2.0/test/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 23:31:09.500140 kioss-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-31 23:30:53.000000 kioss-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-31 23:31:09.500140 kioss-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-07-31 23:30:53.000000 kioss-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 23:31:09.500140 kioss-0.2.1/kioss/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-31 23:30:53.000000 kioss-0.2.1/kioss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19401 2023-07-31 23:30:53.000000 kioss-0.2.1/kioss/pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-31 23:30:53.000000 kioss-0.2.1/kioss/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 23:31:09.500140 kioss-0.2.1/kioss.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-31 23:31:09.000000 kioss-0.2.1/kioss.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-31 23:31:09.000000 kioss-0.2.1/kioss.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 23:31:09.000000 kioss-0.2.1/kioss.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-31 23:31:09.000000 kioss-0.2.1/kioss.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 23:31:09.500140 kioss-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-31 23:30:53.000000 kioss-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 23:31:09.500140 kioss-0.2.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    11211 2023-07-31 23:30:53.000000 kioss-0.2.1/test/test_pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-31 23:30:53.000000 kioss-0.2.1/test/test_util.py
```

### Comparing `kioss-0.2.0/LICENSE` & `kioss-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kioss-0.2.0/README.md` & `kioss-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `kioss-0.2.0/kioss/pipe.py` & `kioss-0.2.1/kioss/pipe.py`

 * *Files identical despite different names*

### Comparing `kioss-0.2.0/kioss/util.py` & `kioss-0.2.1/kioss/util.py`

 * *Files identical despite different names*

### Comparing `kioss-0.2.0/test/test_pipe.py` & `kioss-0.2.1/test/test_pipe.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,15 +51,14 @@
                 .chain(Pipe(range(2, 4)), Pipe(range(4, 6)))
                 .chain(Pipe(range(6, 8)))
             ),
             list(range(8)),
         )
 
     def test_mix(self):
-        N = 32
         single_pipe_iteration_duration = 0.5
         new_pipes = lambda: [
             Pipe(range(0, N, 3)).slow((N / 3) / single_pipe_iteration_duration),
             Pipe(range(1, N, 3)).slow((N / 3) / single_pipe_iteration_duration),
             Pipe(range(2, N, 3)).slow((N / 3) / single_pipe_iteration_duration),
         ]
         self.assertAlmostEqual(
@@ -241,43 +240,26 @@
         [
             [n_workers, worker_type]
             for n_workers in [None, 1]
             for worker_type in Pipe.SUPPORTED_WORKER_TYPES
         ]
     )
     def test_slow(self, n_workers: Optional[int], worker_type: str):
-        N = 100
         freq = 64
         pipe = (
             Pipe(range(N))
             .map(ten_millis_identity, n_workers=n_workers, worker_type=worker_type)
             .slow(freq)
         )
         self.assertAlmostEqual(
             pipe.time(),
             1 / freq * N,
             delta=0.3 * (1 / freq * N),
         )
 
-    # @parameterized.expand(
-    #         [
-    #             [n_workers, worker_type]
-    #             for n_workers in [None, 1]
-    #             for worker_type in Pipe.SUPPORTED_WORKER_TYPES
-    #         ]
-    # )
-    # def test_head(self, n_workers: Optional[int], worker_type: str):
-    #     self.assertListEqual(Pipe(range(8)).map(ten_millis_identity, n_workers=n_workers, worker_type=worker_type).head(3).collect(), [0, 1, 2])
-
-    #     self.assertAlmostEqual(
-    #         Pipe(range(N)).map(ten_millis_identity, n_workers=n_workers, worker_type=worker_type).head(N//2).time(),
-    #         Pipe(range(N)).map(ten_millis_identity, n_workers=n_workers, worker_type=worker_type).time()/2,
-    #         delta=0.3 * TEN_MS * (N//2),
-    #     )
-
     def test_collect(self):
         self.assertListEqual(Pipe(range(8)).collect(n_samples=6), list(range(6)))
         self.assertListEqual(Pipe(range(8)).collect(), list(range(8)))
         self.assertAlmostEqual(
             timeit.timeit(
                 lambda: Pipe(range(8)).map(ten_millis_identity).collect(0),
                 number=1,
```

### Comparing `kioss-0.2.0/test/test_util.py` & `kioss-0.2.1/test/test_util.py`

 * *Files identical despite different names*

