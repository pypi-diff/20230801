# Comparing `tmp/log10_io-0.2.4.tar.gz` & `tmp/log10_io-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "log10_io-0.2.4.tar", max compression
+gzip compressed data, was "log10_io-0.2.7.tar", max compression
```

## Comparing `log10_io-0.2.4.tar` & `log10_io-0.2.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1083 2023-08-01 01:35:01.673205 log10_io-0.2.4/LICENSE
--rw-r--r--   0        0        0     2715 2023-08-01 01:35:01.673205 log10_io-0.2.4/README.md
--rw-r--r--   0        0        0        0 2023-08-01 01:35:01.673205 log10_io-0.2.4/log10/__init__.py
--rw-r--r--   0        0        0     9271 2023-08-01 01:35:01.673205 log10_io-0.2.4/log10/agents/camel.py
--rw-r--r--   0        0        0      765 2023-08-01 01:35:01.673205 log10_io-0.2.4/log10/agents/scrape_summarizer.py
--rw-r--r--   0        0        0     4755 2023-08-01 01:35:01.673205 log10_io-0.2.4/log10/anthropic.py
--rw-r--r--   0        0        0     2594 2023-08-01 01:35:01.673205 log10_io-0.2.4/log10/bigquery.py
--rw-r--r--   0        0        0     2684 2023-08-01 01:35:01.673205 log10_io-0.2.4/log10/evals.py
--rw-r--r--   0        0        0     9316 2023-08-01 01:35:01.677205 log10_io-0.2.4/log10/langchain.py
--rw-r--r--   0        0        0     7142 2023-08-01 01:35:01.677205 log10_io-0.2.4/log10/llm.py
--rw-r--r--   0        0        0    13442 2023-08-01 01:35:01.677205 log10_io-0.2.4/log10/load.py
--rw-r--r--   0        0        0     1909 2023-08-01 01:35:01.677205 log10_io-0.2.4/log10/openai.py
--rw-r--r--   0        0        0     1020 2023-08-01 01:35:01.677205 log10_io-0.2.4/log10/schemas/bigquery.json
--rw-r--r--   0        0        0     2101 2023-08-01 01:35:01.677205 log10_io-0.2.4/log10/tools.py
--rw-r--r--   0        0        0     1051 2023-08-01 01:35:01.677205 log10_io-0.2.4/log10/utils.py
--rw-r--r--   0        0        0      965 2023-08-01 01:35:01.677205 log10_io-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     3725 1970-01-01 00:00:00.000000 log10_io-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-08-01 01:39:16.080544 log10_io-0.2.7/LICENSE
+-rw-r--r--   0        0        0     2715 2023-08-01 01:39:16.080544 log10_io-0.2.7/README.md
+-rw-r--r--   0        0        0        0 2023-08-01 01:39:16.084544 log10_io-0.2.7/log10/__init__.py
+-rw-r--r--   0        0        0     9271 2023-08-01 01:39:16.084544 log10_io-0.2.7/log10/agents/camel.py
+-rw-r--r--   0        0        0      765 2023-08-01 01:39:16.084544 log10_io-0.2.7/log10/agents/scrape_summarizer.py
+-rw-r--r--   0        0        0     4755 2023-08-01 01:39:16.084544 log10_io-0.2.7/log10/anthropic.py
+-rw-r--r--   0        0        0     2594 2023-08-01 01:39:16.084544 log10_io-0.2.7/log10/bigquery.py
+-rw-r--r--   0        0        0     2684 2023-08-01 01:39:16.084544 log10_io-0.2.7/log10/evals.py
+-rw-r--r--   0        0        0     9316 2023-08-01 01:39:16.084544 log10_io-0.2.7/log10/langchain.py
+-rw-r--r--   0        0        0     7142 2023-08-01 01:39:16.084544 log10_io-0.2.7/log10/llm.py
+-rw-r--r--   0        0        0    13442 2023-08-01 01:39:16.084544 log10_io-0.2.7/log10/load.py
+-rw-r--r--   0        0        0     1909 2023-08-01 01:39:16.084544 log10_io-0.2.7/log10/openai.py
+-rw-r--r--   0        0        0     1020 2023-08-01 01:39:16.088544 log10_io-0.2.7/log10/schemas/bigquery.json
+-rw-r--r--   0        0        0     2101 2023-08-01 01:39:16.088544 log10_io-0.2.7/log10/tools.py
+-rw-r--r--   0        0        0     1051 2023-08-01 01:39:16.088544 log10_io-0.2.7/log10/utils.py
+-rw-r--r--   0        0        0      965 2023-08-01 01:39:16.088544 log10_io-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     3725 1970-01-01 00:00:00.000000 log10_io-0.2.7/PKG-INFO
```

### Comparing `log10_io-0.2.4/LICENSE` & `log10_io-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `log10_io-0.2.4/README.md` & `log10_io-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `log10_io-0.2.4/log10/agents/camel.py` & `log10_io-0.2.7/log10/agents/camel.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.2.4/log10/agents/scrape_summarizer.py` & `log10_io-0.2.7/log10/agents/scrape_summarizer.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.2.4/log10/anthropic.py` & `log10_io-0.2.7/log10/anthropic.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.2.4/log10/bigquery.py` & `log10_io-0.2.7/log10/bigquery.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.2.4/log10/evals.py` & `log10_io-0.2.7/log10/evals.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.2.4/log10/langchain.py` & `log10_io-0.2.7/log10/langchain.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.2.4/log10/llm.py` & `log10_io-0.2.7/log10/llm.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.2.4/log10/load.py` & `log10_io-0.2.7/log10/load.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.2.4/log10/openai.py` & `log10_io-0.2.7/log10/openai.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.2.4/log10/schemas/bigquery.json` & `log10_io-0.2.7/log10/schemas/bigquery.json`

 * *Files identical despite different names*

### Comparing `log10_io-0.2.4/log10/tools.py` & `log10_io-0.2.7/log10/tools.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.2.4/log10/utils.py` & `log10_io-0.2.7/log10/utils.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.2.4/pyproject.toml` & `log10_io-0.2.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "log10-io"
 
-version = "0.2.4"
+version = "0.2.7"
 authors = ["log10 team"]
 license = "MIT"
 description = "Unified LLM data management"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `log10_io-0.2.4/PKG-INFO` & `log10_io-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: log10-io
-Version: 0.2.4
+Version: 0.2.7
 Summary: Unified LLM data management
 License: MIT
 Author: log10 team
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

