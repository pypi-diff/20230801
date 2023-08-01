# Comparing `tmp/grouped_query_attention_pytorch-0.1.0.tar.gz` & `tmp/grouped_query_attention_pytorch-0.1.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grouped_query_attention_pytorch-0.1.0.tar", last modified: Tue Aug  1 02:05:46 2023, max compression
+gzip compressed data, was "grouped_query_attention_pytorch-0.1.0rc2.tar", last modified: Tue Aug  1 01:57:57 2023, max compression
```

## Comparing `grouped_query_attention_pytorch-0.1.0.tar` & `grouped_query_attention_pytorch-0.1.0rc2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:05:46.053319 grouped_query_attention_pytorch-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-08-01 02:05:32.000000 grouped_query_attention_pytorch-0.1.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:05:46.045319 grouped_query_attention_pytorch-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:05:46.049319 grouped_query_attention_pytorch-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-08-01 02:05:32.000000 grouped_query_attention_pytorch-0.1.0/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-08-01 02:05:32.000000 grouped_query_attention_pytorch-0.1.0/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-08-01 02:05:32.000000 grouped_query_attention_pytorch-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-08-01 02:05:32.000000 grouped_query_attention_pytorch-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-08-01 02:05:32.000000 grouped_query_attention_pytorch-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8115 2023-08-01 02:05:46.053319 grouped_query_attention_pytorch-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-08-01 02:05:32.000000 grouped_query_attention_pytorch-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:05:46.049319 grouped_query_attention_pytorch-0.1.0/doc/
--rw-r--r--   0 runner    (1001) docker     (123)   335190 2023-08-01 02:05:32.000000 grouped_query_attention_pytorch-0.1.0/doc/attention.png
--rw-r--r--   0 runner    (1001) docker     (123)    37835 2023-08-01 02:05:32.000000 grouped_query_attention_pytorch-0.1.0/doc/benchmark_attention.png
--rw-r--r--   0 runner    (1001) docker     (123)    37657 2023-08-01 02:05:32.000000 grouped_query_attention_pytorch-0.1.0/doc/benchmark_t5.png
--rw-r--r--   0 runner    (1001) docker     (123)   118342 2023-08-01 02:05:32.000000 grouped_query_attention_pytorch-0.1.0/doc/benchmark_t5_original.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:05:46.049319 grouped_query_attention_pytorch-0.1.0/grouped_query_attention_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-08-01 02:05:32.000000 grouped_query_attention_pytorch-0.1.0/grouped_query_attention_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12512 2023-08-01 02:05:32.000000 grouped_query_attention_pytorch-0.1.0/grouped_query_attention_pytorch/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)    13858 2023-08-01 02:05:32.000000 grouped_query_attention_pytorch-0.1.0/grouped_query_attention_pytorch/t5.py
--rw-r--r--   0 runner    (1001) docker     (123)    12319 2023-08-01 02:05:32.000000 grouped_query_attention_pytorch-0.1.0/grouped_query_attention_pytorch/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:05:46.049319 grouped_query_attention_pytorch-0.1.0/grouped_query_attention_pytorch/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 02:05:32.000000 grouped_query_attention_pytorch-0.1.0/grouped_query_attention_pytorch/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-08-01 02:05:32.000000 grouped_query_attention_pytorch-0.1.0/grouped_query_attention_pytorch/utils/benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:05:46.049319 grouped_query_attention_pytorch-0.1.0/grouped_query_attention_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8115 2023-08-01 02:05:46.000000 grouped_query_attention_pytorch-0.1.0/grouped_query_attention_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-08-01 02:05:46.000000 grouped_query_attention_pytorch-0.1.0/grouped_query_attention_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 02:05:46.000000 grouped_query_attention_pytorch-0.1.0/grouped_query_attention_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-08-01 02:05:46.000000 grouped_query_attention_pytorch-0.1.0/grouped_query_attention_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-01 02:05:46.000000 grouped_query_attention_pytorch-0.1.0/grouped_query_attention_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-08-01 02:05:32.000000 grouped_query_attention_pytorch-0.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:05:46.053319 grouped_query_attention_pytorch-0.1.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-08-01 02:05:32.000000 grouped_query_attention_pytorch-0.1.0/scripts/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-08-01 02:05:32.000000 grouped_query_attention_pytorch-0.1.0/scripts/benchmark_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     9082 2023-08-01 02:05:32.000000 grouped_query_attention_pytorch-0.1.0/scripts/benchmark_t5.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 02:05:46.053319 grouped_query_attention_pytorch-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:05:46.053319 grouped_query_attention_pytorch-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 02:05:32.000000 grouped_query_attention_pytorch-0.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-08-01 02:05:32.000000 grouped_query_attention_pytorch-0.1.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-08-01 02:05:32.000000 grouped_query_attention_pytorch-0.1.0/tests/test_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-08-01 02:05:32.000000 grouped_query_attention_pytorch-0.1.0/tests/test_t5.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-08-01 02:05:32.000000 grouped_query_attention_pytorch-0.1.0/tests/test_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:57:57.172505 grouped_query_attention_pytorch-0.1.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-08-01 01:57:42.000000 grouped_query_attention_pytorch-0.1.0rc2/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:57:57.164504 grouped_query_attention_pytorch-0.1.0rc2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:57:57.168505 grouped_query_attention_pytorch-0.1.0rc2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-08-01 01:57:42.000000 grouped_query_attention_pytorch-0.1.0rc2/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-08-01 01:57:42.000000 grouped_query_attention_pytorch-0.1.0rc2/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-08-01 01:57:42.000000 grouped_query_attention_pytorch-0.1.0rc2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-08-01 01:57:42.000000 grouped_query_attention_pytorch-0.1.0rc2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-08-01 01:57:42.000000 grouped_query_attention_pytorch-0.1.0rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8118 2023-08-01 01:57:57.172505 grouped_query_attention_pytorch-0.1.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-08-01 01:57:42.000000 grouped_query_attention_pytorch-0.1.0rc2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:57:57.168505 grouped_query_attention_pytorch-0.1.0rc2/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)   335190 2023-08-01 01:57:42.000000 grouped_query_attention_pytorch-0.1.0rc2/doc/attention.png
+-rw-r--r--   0 runner    (1001) docker     (123)    37835 2023-08-01 01:57:42.000000 grouped_query_attention_pytorch-0.1.0rc2/doc/benchmark_attention.png
+-rw-r--r--   0 runner    (1001) docker     (123)    37657 2023-08-01 01:57:42.000000 grouped_query_attention_pytorch-0.1.0rc2/doc/benchmark_t5.png
+-rw-r--r--   0 runner    (1001) docker     (123)   118342 2023-08-01 01:57:42.000000 grouped_query_attention_pytorch-0.1.0rc2/doc/benchmark_t5_original.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:57:57.168505 grouped_query_attention_pytorch-0.1.0rc2/grouped_query_attention_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-08-01 01:57:42.000000 grouped_query_attention_pytorch-0.1.0rc2/grouped_query_attention_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12512 2023-08-01 01:57:42.000000 grouped_query_attention_pytorch-0.1.0rc2/grouped_query_attention_pytorch/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13858 2023-08-01 01:57:42.000000 grouped_query_attention_pytorch-0.1.0rc2/grouped_query_attention_pytorch/t5.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12319 2023-08-01 01:57:42.000000 grouped_query_attention_pytorch-0.1.0rc2/grouped_query_attention_pytorch/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:57:57.168505 grouped_query_attention_pytorch-0.1.0rc2/grouped_query_attention_pytorch/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 01:57:42.000000 grouped_query_attention_pytorch-0.1.0rc2/grouped_query_attention_pytorch/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-08-01 01:57:42.000000 grouped_query_attention_pytorch-0.1.0rc2/grouped_query_attention_pytorch/utils/benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:57:57.168505 grouped_query_attention_pytorch-0.1.0rc2/grouped_query_attention_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8118 2023-08-01 01:57:57.000000 grouped_query_attention_pytorch-0.1.0rc2/grouped_query_attention_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-08-01 01:57:57.000000 grouped_query_attention_pytorch-0.1.0rc2/grouped_query_attention_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 01:57:57.000000 grouped_query_attention_pytorch-0.1.0rc2/grouped_query_attention_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-08-01 01:57:57.000000 grouped_query_attention_pytorch-0.1.0rc2/grouped_query_attention_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-01 01:57:57.000000 grouped_query_attention_pytorch-0.1.0rc2/grouped_query_attention_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-08-01 01:57:42.000000 grouped_query_attention_pytorch-0.1.0rc2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:57:57.168505 grouped_query_attention_pytorch-0.1.0rc2/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-08-01 01:57:42.000000 grouped_query_attention_pytorch-0.1.0rc2/scripts/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-08-01 01:57:42.000000 grouped_query_attention_pytorch-0.1.0rc2/scripts/benchmark_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9082 2023-08-01 01:57:42.000000 grouped_query_attention_pytorch-0.1.0rc2/scripts/benchmark_t5.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 01:57:57.172505 grouped_query_attention_pytorch-0.1.0rc2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:57:57.172505 grouped_query_attention_pytorch-0.1.0rc2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 01:57:42.000000 grouped_query_attention_pytorch-0.1.0rc2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-08-01 01:57:42.000000 grouped_query_attention_pytorch-0.1.0rc2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-08-01 01:57:42.000000 grouped_query_attention_pytorch-0.1.0rc2/tests/test_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-08-01 01:57:42.000000 grouped_query_attention_pytorch-0.1.0rc2/tests/test_t5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-08-01 01:57:42.000000 grouped_query_attention_pytorch-0.1.0rc2/tests/test_transformer.py
```

### Comparing `grouped_query_attention_pytorch-0.1.0/.github/workflows/publish.yaml` & `grouped_query_attention_pytorch-0.1.0rc2/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `grouped_query_attention_pytorch-0.1.0/.github/workflows/test.yaml` & `grouped_query_attention_pytorch-0.1.0rc2/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `grouped_query_attention_pytorch-0.1.0/.gitignore` & `grouped_query_attention_pytorch-0.1.0rc2/.gitignore`

 * *Files identical despite different names*

### Comparing `grouped_query_attention_pytorch-0.1.0/LICENSE` & `grouped_query_attention_pytorch-0.1.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `grouped_query_attention_pytorch-0.1.0/PKG-INFO` & `grouped_query_attention_pytorch-0.1.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grouped_query_attention_pytorch
-Version: 0.1.0
+Version: 0.1.0rc2
 Summary: grouped-query-attention-pytorch
 Author-email: Frank Odom <frank.odom.iii@gmail.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `grouped_query_attention_pytorch-0.1.0/README.md` & `grouped_query_attention_pytorch-0.1.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `grouped_query_attention_pytorch-0.1.0/doc/attention.png` & `grouped_query_attention_pytorch-0.1.0rc2/doc/attention.png`

 * *Files identical despite different names*

### Comparing `grouped_query_attention_pytorch-0.1.0/doc/benchmark_attention.png` & `grouped_query_attention_pytorch-0.1.0rc2/doc/benchmark_attention.png`

 * *Files identical despite different names*

### Comparing `grouped_query_attention_pytorch-0.1.0/doc/benchmark_t5.png` & `grouped_query_attention_pytorch-0.1.0rc2/doc/benchmark_t5.png`

 * *Files identical despite different names*

### Comparing `grouped_query_attention_pytorch-0.1.0/doc/benchmark_t5_original.png` & `grouped_query_attention_pytorch-0.1.0rc2/doc/benchmark_t5_original.png`

 * *Files identical despite different names*

### Comparing `grouped_query_attention_pytorch-0.1.0/grouped_query_attention_pytorch/attention.py` & `grouped_query_attention_pytorch-0.1.0rc2/grouped_query_attention_pytorch/attention.py`

 * *Files identical despite different names*

### Comparing `grouped_query_attention_pytorch-0.1.0/grouped_query_attention_pytorch/t5.py` & `grouped_query_attention_pytorch-0.1.0rc2/grouped_query_attention_pytorch/t5.py`

 * *Files identical despite different names*

### Comparing `grouped_query_attention_pytorch-0.1.0/grouped_query_attention_pytorch/transformer.py` & `grouped_query_attention_pytorch-0.1.0rc2/grouped_query_attention_pytorch/transformer.py`

 * *Files identical despite different names*

### Comparing `grouped_query_attention_pytorch-0.1.0/grouped_query_attention_pytorch/utils/benchmark.py` & `grouped_query_attention_pytorch-0.1.0rc2/grouped_query_attention_pytorch/utils/benchmark.py`

 * *Files identical despite different names*

### Comparing `grouped_query_attention_pytorch-0.1.0/grouped_query_attention_pytorch.egg-info/PKG-INFO` & `grouped_query_attention_pytorch-0.1.0rc2/grouped_query_attention_pytorch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grouped-query-attention-pytorch
-Version: 0.1.0
+Version: 0.1.0rc2
 Summary: grouped-query-attention-pytorch
 Author-email: Frank Odom <frank.odom.iii@gmail.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `grouped_query_attention_pytorch-0.1.0/grouped_query_attention_pytorch.egg-info/SOURCES.txt` & `grouped_query_attention_pytorch-0.1.0rc2/grouped_query_attention_pytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `grouped_query_attention_pytorch-0.1.0/pyproject.toml` & `grouped_query_attention_pytorch-0.1.0rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `grouped_query_attention_pytorch-0.1.0/scripts/README.md` & `grouped_query_attention_pytorch-0.1.0rc2/scripts/README.md`

 * *Files identical despite different names*

### Comparing `grouped_query_attention_pytorch-0.1.0/scripts/benchmark_attention.py` & `grouped_query_attention_pytorch-0.1.0rc2/scripts/benchmark_attention.py`

 * *Files identical despite different names*

### Comparing `grouped_query_attention_pytorch-0.1.0/scripts/benchmark_t5.py` & `grouped_query_attention_pytorch-0.1.0rc2/scripts/benchmark_t5.py`

 * *Files identical despite different names*

### Comparing `grouped_query_attention_pytorch-0.1.0/tests/conftest.py` & `grouped_query_attention_pytorch-0.1.0rc2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `grouped_query_attention_pytorch-0.1.0/tests/test_attention.py` & `grouped_query_attention_pytorch-0.1.0rc2/tests/test_attention.py`

 * *Files identical despite different names*

### Comparing `grouped_query_attention_pytorch-0.1.0/tests/test_t5.py` & `grouped_query_attention_pytorch-0.1.0rc2/tests/test_t5.py`

 * *Files identical despite different names*

### Comparing `grouped_query_attention_pytorch-0.1.0/tests/test_transformer.py` & `grouped_query_attention_pytorch-0.1.0rc2/tests/test_transformer.py`

 * *Files identical despite different names*

