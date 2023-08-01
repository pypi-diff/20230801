# Comparing `tmp/jacktrade-0.1.1.tar.gz` & `tmp/jacktrade-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jacktrade-0.1.1.tar", last modified: Sun Apr  9 15:19:01 2023, max compression
+gzip compressed data, was "jacktrade-0.1.2.tar", last modified: Tue Aug  1 08:18:05 2023, max compression
```

## Comparing `jacktrade-0.1.1.tar` & `jacktrade-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 15:19:01.564228 jacktrade-0.1.1/
--rw-rw-rw-   0        0        0     1077 2023-02-11 18:38:48.000000 jacktrade-0.1.1/LICENSE.md
--rw-rw-rw-   0        0        0     5227 2023-04-09 15:19:01.563190 jacktrade-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     3455 2023-04-09 15:08:47.000000 jacktrade-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-09 15:19:01.544274 jacktrade-0.1.1/jacktrade/
--rw-rw-rw-   0        0        0        0 2023-02-12 13:53:20.000000 jacktrade-0.1.1/jacktrade/__init__.py
--rw-rw-rw-   0        0        0     2300 2023-04-09 15:05:56.000000 jacktrade-0.1.1/jacktrade/benchmark.py
--rw-rw-rw-   0        0        0     3665 2023-04-09 13:07:22.000000 jacktrade-0.1.1/jacktrade/collections.py
--rw-rw-rw-   0        0        0     2486 2023-04-08 15:30:12.000000 jacktrade-0.1.1/jacktrade/multicore.py
--rw-rw-rw-   0        0        0      662 2023-04-08 16:09:02.000000 jacktrade-0.1.1/jacktrade/pickler.py
-drwxrwxrwx   0        0        0        0 2023-04-09 15:19:01.552219 jacktrade-0.1.1/jacktrade.egg-info/
--rw-rw-rw-   0        0        0     5227 2023-04-09 15:19:01.000000 jacktrade-0.1.1/jacktrade.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      400 2023-04-09 15:19:01.000000 jacktrade-0.1.1/jacktrade.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 15:19:01.000000 jacktrade-0.1.1/jacktrade.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-04-09 15:19:01.000000 jacktrade-0.1.1/jacktrade.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      727 2023-04-09 14:59:59.000000 jacktrade-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-09 15:19:01.565183 jacktrade-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-09 15:19:01.561195 jacktrade-0.1.1/tests/
--rw-rw-rw-   0        0        0     1891 2023-04-08 14:04:02.000000 jacktrade-0.1.1/tests/test_benchmark.py
--rw-rw-rw-   0        0        0     4132 2023-04-09 13:07:18.000000 jacktrade-0.1.1/tests/test_collections.py
--rw-rw-rw-   0        0        0     3232 2023-04-09 12:49:59.000000 jacktrade-0.1.1/tests/test_multicore.py
--rw-rw-rw-   0        0        0      608 2023-04-08 16:08:21.000000 jacktrade-0.1.1/tests/test_pickler.py
--rw-rw-rw-   0        0        0      180 2023-04-08 14:13:05.000000 jacktrade-0.1.1/tests/test_template.py
+drwxrwxrwx   0        0        0        0 2023-08-01 08:18:05.206177 jacktrade-0.1.2/
+-rw-rw-rw-   0        0        0     1077 2023-02-11 18:38:48.000000 jacktrade-0.1.2/LICENSE.md
+-rw-rw-rw-   0        0        0     5258 2023-08-01 08:18:05.205180 jacktrade-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3486 2023-05-24 11:40:26.000000 jacktrade-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-08-01 08:18:05.181244 jacktrade-0.1.2/jacktrade/
+-rw-rw-rw-   0        0        0        0 2023-02-12 13:53:20.000000 jacktrade-0.1.2/jacktrade/__init__.py
+-rw-rw-rw-   0        0        0     2300 2023-04-09 15:05:56.000000 jacktrade-0.1.2/jacktrade/benchmark.py
+-rw-rw-rw-   0        0        0     3809 2023-08-01 08:16:47.000000 jacktrade-0.1.2/jacktrade/collections.py
+-rw-rw-rw-   0        0        0     2486 2023-04-08 15:30:12.000000 jacktrade-0.1.2/jacktrade/multicore.py
+-rw-rw-rw-   0        0        0      662 2023-04-08 16:09:02.000000 jacktrade-0.1.2/jacktrade/pickler.py
+drwxrwxrwx   0        0        0        0 2023-08-01 08:18:05.191217 jacktrade-0.1.2/jacktrade.egg-info/
+-rw-rw-rw-   0        0        0     5258 2023-08-01 08:18:05.000000 jacktrade-0.1.2/jacktrade.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      400 2023-08-01 08:18:05.000000 jacktrade-0.1.2/jacktrade.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 08:18:05.000000 jacktrade-0.1.2/jacktrade.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-08-01 08:18:05.000000 jacktrade-0.1.2/jacktrade.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      727 2023-08-01 08:14:05.000000 jacktrade-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-01 08:18:05.206177 jacktrade-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-01 08:18:05.203185 jacktrade-0.1.2/tests/
+-rw-rw-rw-   0        0        0     1891 2023-04-08 14:04:02.000000 jacktrade-0.1.2/tests/test_benchmark.py
+-rw-rw-rw-   0        0        0     4555 2023-08-01 08:17:05.000000 jacktrade-0.1.2/tests/test_collections.py
+-rw-rw-rw-   0        0        0     3232 2023-04-09 12:49:59.000000 jacktrade-0.1.2/tests/test_multicore.py
+-rw-rw-rw-   0        0        0      608 2023-04-08 16:08:21.000000 jacktrade-0.1.2/tests/test_pickler.py
+-rw-rw-rw-   0        0        0      180 2023-04-08 14:13:05.000000 jacktrade-0.1.2/tests/test_template.py
```

### Comparing `jacktrade-0.1.1/LICENSE.md` & `jacktrade-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `jacktrade-0.1.1/PKG-INFO` & `jacktrade-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jacktrade
-Version: 0.1.1
+Version: 0.1.2
 Summary: A collection of commonly used Python utilities.
 Author-email: Mario Zaja <mzaja0@gmail.com>
 License: MIT License
         
         Copyright (c) 2023, Mario Zaja
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -21,15 +21,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # jacktrade
-[![test](https://github.com/mzaja/jacktrade/actions/workflows/test.yml/badge.svg)](https://github.com/mzaja/jacktrade/actions/workflows/test.yml) [![Coverage Status](https://coveralls.io/repos/github/mzaja/jacktrade/badge.svg?branch=main)](https://coveralls.io/github/mzaja/jacktrade?branch=main) [![PyPI version](https://badge.fury.io/py/jacktrade.svg)](https://badge.fury.io/py/jacktrade) ![License](https://img.shields.io/github/license/mzaja/jacktrade)
+[![test](https://github.com/mzaja/jacktrade/actions/workflows/test.yml/badge.svg)](https://github.com/mzaja/jacktrade/actions/workflows/test.yml) [![Coverage Status](https://coveralls.io/repos/github/mzaja/jacktrade/badge.svg?branch=main)](https://coveralls.io/github/mzaja/jacktrade?branch=main) ![PyPI version](https://img.shields.io/pypi/v/jacktrade) ![Python version](https://img.shields.io/pypi/pyversions/jacktrade) ![License](https://img.shields.io/github/license/mzaja/jacktrade)
 
 **Jack of all trades, master of none** - a collection of commonly used Python utilities. Install using:
 ```
 pip install jacktrade
 ```
 
 The package consists of the following submodules:
```

### Comparing `jacktrade-0.1.1/README.md` & `jacktrade-0.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # jacktrade
-[![test](https://github.com/mzaja/jacktrade/actions/workflows/test.yml/badge.svg)](https://github.com/mzaja/jacktrade/actions/workflows/test.yml) [![Coverage Status](https://coveralls.io/repos/github/mzaja/jacktrade/badge.svg?branch=main)](https://coveralls.io/github/mzaja/jacktrade?branch=main) [![PyPI version](https://badge.fury.io/py/jacktrade.svg)](https://badge.fury.io/py/jacktrade) ![License](https://img.shields.io/github/license/mzaja/jacktrade)
+[![test](https://github.com/mzaja/jacktrade/actions/workflows/test.yml/badge.svg)](https://github.com/mzaja/jacktrade/actions/workflows/test.yml) [![Coverage Status](https://coveralls.io/repos/github/mzaja/jacktrade/badge.svg?branch=main)](https://coveralls.io/github/mzaja/jacktrade?branch=main) ![PyPI version](https://img.shields.io/pypi/v/jacktrade) ![Python version](https://img.shields.io/pypi/pyversions/jacktrade) ![License](https://img.shields.io/github/license/mzaja/jacktrade)
 
 **Jack of all trades, master of none** - a collection of commonly used Python utilities. Install using:
 ```
 pip install jacktrade
 ```
 
 The package consists of the following submodules:
```

### Comparing `jacktrade-0.1.1/jacktrade/benchmark.py` & `jacktrade-0.1.2/jacktrade/benchmark.py`

 * *Files identical despite different names*

### Comparing `jacktrade-0.1.1/jacktrade/collections.py` & `jacktrade-0.1.2/jacktrade/collections.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,35 +63,36 @@
     Recursion happens until a non-list item is encountered, or max_depth is reached.
     """
     output_data = []
     _flatten_list(input_data, output_data, max_depth)
     return output_data
 
 
-def chunkify(iterable: Iterable, chunk_size: int) -> Iterator[list]:
+def chunkify(iterable: Iterable, chunk_size: int = None) -> Iterator[list]:
     """
     Yields successive n-sized list chunks from an iterable.
     Supports generator expressions.
     """
-    iterator = iter(iterable)
+    iterator = iter(iterable)  # Must be assigned here, else infinite loop
     while chunk := list(islice(iterator, chunk_size)):
         yield chunk
 
 
-def ichunkify(iterable: Iterable, chunk_size: int) -> Iterator[Iterator]:
+def ichunkify(iterable: Iterable, chunk_size: int = None) -> Iterator[Iterator]:
     """
     Yields successive n-sized iterator chunks from an iterable.
     Supports generator expressions.
 
     WARNING!:   Chunks must be consumed as they are yielded, otherwise
                 the results will not be as expected!
     """
     iterator = iter(iterable)
+    chunk_size_minus_one = None if (chunk_size is None) else (chunk_size - 1)
     for first_chunk_elem in iterator:
-        yield chain([first_chunk_elem], islice(iterator, chunk_size - 1))
+        yield chain([first_chunk_elem], islice(iterator, chunk_size_minus_one))
 
 
 def limit_iterator(iterable: Iterable, limit: int = None) -> Iterator:
     """
     Returns an interator which yields successive elements of
     the iterable up to the limit, if the limit is specified.
     """
```

### Comparing `jacktrade-0.1.1/jacktrade/multicore.py` & `jacktrade-0.1.2/jacktrade/multicore.py`

 * *Files identical despite different names*

### Comparing `jacktrade-0.1.1/jacktrade/pickler.py` & `jacktrade-0.1.2/jacktrade/pickler.py`

 * *Files identical despite different names*

### Comparing `jacktrade-0.1.1/jacktrade.egg-info/PKG-INFO` & `jacktrade-0.1.2/jacktrade.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jacktrade
-Version: 0.1.1
+Version: 0.1.2
 Summary: A collection of commonly used Python utilities.
 Author-email: Mario Zaja <mzaja0@gmail.com>
 License: MIT License
         
         Copyright (c) 2023, Mario Zaja
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -21,15 +21,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # jacktrade
-[![test](https://github.com/mzaja/jacktrade/actions/workflows/test.yml/badge.svg)](https://github.com/mzaja/jacktrade/actions/workflows/test.yml) [![Coverage Status](https://coveralls.io/repos/github/mzaja/jacktrade/badge.svg?branch=main)](https://coveralls.io/github/mzaja/jacktrade?branch=main) [![PyPI version](https://badge.fury.io/py/jacktrade.svg)](https://badge.fury.io/py/jacktrade) ![License](https://img.shields.io/github/license/mzaja/jacktrade)
+[![test](https://github.com/mzaja/jacktrade/actions/workflows/test.yml/badge.svg)](https://github.com/mzaja/jacktrade/actions/workflows/test.yml) [![Coverage Status](https://coveralls.io/repos/github/mzaja/jacktrade/badge.svg?branch=main)](https://coveralls.io/github/mzaja/jacktrade?branch=main) ![PyPI version](https://img.shields.io/pypi/v/jacktrade) ![Python version](https://img.shields.io/pypi/pyversions/jacktrade) ![License](https://img.shields.io/github/license/mzaja/jacktrade)
 
 **Jack of all trades, master of none** - a collection of commonly used Python utilities. Install using:
 ```
 pip install jacktrade
 ```
 
 The package consists of the following submodules:
```

### Comparing `jacktrade-0.1.1/pyproject.toml` & `jacktrade-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jacktrade"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Mario Zaja", email="mzaja0@gmail.com" },
 ]
 description = "A collection of commonly used Python utilities."
 readme = "README.md"
 license = { file = "LICENSE.md" }
 requires-python = ">=3.10"
```

### Comparing `jacktrade-0.1.1/tests/test_benchmark.py` & `jacktrade-0.1.2/tests/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `jacktrade-0.1.1/tests/test_collections.py` & `jacktrade-0.1.2/tests/test_collections.py`

 * *Files 5% similar despite different names*

```diff
@@ -69,14 +69,18 @@
         for chunk_size, first_exp, last_exp, count_exp in CHUNKIFY_TEST_PARAMS:
             with self.subTest(chunk_size=chunk_size):
                 chunks = list(chunkify(LONG_LIST, chunk_size))
                 self.assertEqual(first_exp, chunks[0])
                 self.assertEqual(last_exp, chunks[-1])
                 self.assertEqual(count_exp, len(chunks))
 
+    def test_chunkify_infinite_chunk_size(self):
+        """Tests chunkify when chunk_size is not specified, making it infinite."""
+        self.assertEqual(list(chunkify(LONG_LIST, None)), [LONG_LIST])
+
     def test_ichunkify(self):
         """Tests ichunkify function."""
         for chunk_size, first_exp, last_exp, count_exp in CHUNKIFY_TEST_PARAMS:
             with self.subTest(chunk_size=chunk_size):
                 # Chunks must be consumed as they are yielded
                 for chunk_count, chunk in enumerate(
                     ichunkify(LONG_LIST, chunk_size), 1
@@ -86,14 +90,18 @@
                     if chunk_count == 1:
                         first_chunk = chunk
                 last_chunk = chunk
                 self.assertEqual(first_exp, first_chunk)
                 self.assertEqual(last_exp, last_chunk)
                 self.assertEqual(count_exp, chunk_count)
 
+    def test_ichunkify_infinite_chunk_size(self):
+        """Tests ichunkify when chunk_size is not specified, making it infinite."""
+        self.assertEqual(list(next(ichunkify(LONG_LIST, None))), LONG_LIST)
+
     def test_limited_iterator(self):
         """Tests limiting the iterator to max elements."""
         self.assertEqual(list(limit_iterator(LONG_LIST, 5)), [1, 2, 3, 4, 5])
         self.assertEqual(list(limit_iterator(iter(LONG_LIST), 5)), [1, 2, 3, 4, 5])
         self.assertEqual(list(limit_iterator(LONG_LIST, 99)), LONG_LIST)
         self.assertEqual(list(limit_iterator(iter(LONG_LIST), 99)), LONG_LIST)
```

### Comparing `jacktrade-0.1.1/tests/test_multicore.py` & `jacktrade-0.1.2/tests/test_multicore.py`

 * *Files identical despite different names*

### Comparing `jacktrade-0.1.1/tests/test_pickler.py` & `jacktrade-0.1.2/tests/test_pickler.py`

 * *Files identical despite different names*

