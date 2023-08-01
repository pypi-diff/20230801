# Comparing `tmp/log10_io-0.2.3.tar.gz` & `tmp/log10_io-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "log10_io-0.2.4.tar", max compression
```

## Comparing `log10_io-0.2.3.tar` & `log10_io-0.2.4.tar`

### file list

```diff
@@ -1,47 +1,17 @@
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 log10_io-0.2.3/requirements.txt
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 log10_io-0.2.3/setup.py
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 log10_io-0.2.3/.github/workflows/release.yml
--rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 log10_io-0.2.3/examples/README.md
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 log10_io-0.2.3/examples/agents/biochemist.py
--rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 log10_io-0.2.3/examples/agents/code_optimizer.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 log10_io-0.2.3/examples/agents/coder.py
--rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 log10_io-0.2.3/examples/agents/cybersecurity_expert.py
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 log10_io-0.2.3/examples/agents/email_generator.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 log10_io-0.2.3/examples/agents/scrape_summarizer.py
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 log10_io-0.2.3/examples/agents/translator.py
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 log10_io-0.2.3/examples/evals/basic_eval.py
--rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 log10_io-0.2.3/examples/evals/compile.py
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 log10_io-0.2.3/examples/evals/fuzzy.py
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 log10_io-0.2.3/examples/evals/fuzzy_data.csv
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 log10_io-0.2.3/examples/evals/match_data.csv
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 log10_io-0.2.3/examples/logging/anthropic_completion.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 log10_io-0.2.3/examples/logging/chatcompletion.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 log10_io-0.2.3/examples/logging/chatcompletion_async_vs_sync.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 log10_io-0.2.3/examples/logging/completion.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 log10_io-0.2.3/examples/logging/completion_ada.py
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 log10_io-0.2.3/examples/logging/get_url.py
--rw-r--r--   0        0        0    10777 2020-02-02 00:00:00.000000 log10_io-0.2.3/examples/logging/langchain_babyagi.py
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 log10_io-0.2.3/examples/logging/langchain_model_logger.py
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 log10_io-0.2.3/examples/logging/langchain_multiple_tools.py
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 log10_io-0.2.3/examples/logging/langchain_qa.py
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 log10_io-0.2.3/examples/logging/langchain_simple_sequential.py
--rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 log10_io-0.2.3/examples/logging/langchain_sqlagent.py
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 log10_io-0.2.3/examples/logging/multiple_sessions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 log10_io-0.2.3/log10/__init__.py
--rw-r--r--   0        0        0     4755 2020-02-02 00:00:00.000000 log10_io-0.2.3/log10/anthropic.py
--rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 log10_io-0.2.3/log10/bigquery.py
--rw-r--r--   0        0        0     2684 2020-02-02 00:00:00.000000 log10_io-0.2.3/log10/evals.py
--rw-r--r--   0        0        0     9316 2020-02-02 00:00:00.000000 log10_io-0.2.3/log10/langchain.py
--rw-r--r--   0        0        0     7142 2020-02-02 00:00:00.000000 log10_io-0.2.3/log10/llm.py
--rw-r--r--   0        0        0    13081 2020-02-02 00:00:00.000000 log10_io-0.2.3/log10/load.py
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 log10_io-0.2.3/log10/openai.py
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 log10_io-0.2.3/log10/tools.py
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 log10_io-0.2.3/log10/utils.py
--rw-r--r--   0        0        0     9271 2020-02-02 00:00:00.000000 log10_io-0.2.3/log10/agents/camel.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 log10_io-0.2.3/log10/agents/scrape_summarizer.py
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 log10_io-0.2.3/log10/schemas/bigquery.json
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 log10_io-0.2.3/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 log10_io-0.2.3/LICENSE
--rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 log10_io-0.2.3/README.md
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 log10_io-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     3184 2020-02-02 00:00:00.000000 log10_io-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-08-01 01:35:01.673205 log10_io-0.2.4/LICENSE
+-rw-r--r--   0        0        0     2715 2023-08-01 01:35:01.673205 log10_io-0.2.4/README.md
+-rw-r--r--   0        0        0        0 2023-08-01 01:35:01.673205 log10_io-0.2.4/log10/__init__.py
+-rw-r--r--   0        0        0     9271 2023-08-01 01:35:01.673205 log10_io-0.2.4/log10/agents/camel.py
+-rw-r--r--   0        0        0      765 2023-08-01 01:35:01.673205 log10_io-0.2.4/log10/agents/scrape_summarizer.py
+-rw-r--r--   0        0        0     4755 2023-08-01 01:35:01.673205 log10_io-0.2.4/log10/anthropic.py
+-rw-r--r--   0        0        0     2594 2023-08-01 01:35:01.673205 log10_io-0.2.4/log10/bigquery.py
+-rw-r--r--   0        0        0     2684 2023-08-01 01:35:01.673205 log10_io-0.2.4/log10/evals.py
+-rw-r--r--   0        0        0     9316 2023-08-01 01:35:01.677205 log10_io-0.2.4/log10/langchain.py
+-rw-r--r--   0        0        0     7142 2023-08-01 01:35:01.677205 log10_io-0.2.4/log10/llm.py
+-rw-r--r--   0        0        0    13442 2023-08-01 01:35:01.677205 log10_io-0.2.4/log10/load.py
+-rw-r--r--   0        0        0     1909 2023-08-01 01:35:01.677205 log10_io-0.2.4/log10/openai.py
+-rw-r--r--   0        0        0     1020 2023-08-01 01:35:01.677205 log10_io-0.2.4/log10/schemas/bigquery.json
+-rw-r--r--   0        0        0     2101 2023-08-01 01:35:01.677205 log10_io-0.2.4/log10/tools.py
+-rw-r--r--   0        0        0     1051 2023-08-01 01:35:01.677205 log10_io-0.2.4/log10/utils.py
+-rw-r--r--   0        0        0      965 2023-08-01 01:35:01.677205 log10_io-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     3725 1970-01-01 00:00:00.000000 log10_io-0.2.4/PKG-INFO
```

### Comparing `log10_io-0.2.3/log10/anthropic.py` & `log10_io-0.2.4/log10/anthropic.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.2.3/log10/bigquery.py` & `log10_io-0.2.4/log10/bigquery.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.2.3/log10/evals.py` & `log10_io-0.2.4/log10/evals.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.2.3/log10/langchain.py` & `log10_io-0.2.4/log10/langchain.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.2.3/log10/llm.py` & `log10_io-0.2.4/log10/llm.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.2.3/log10/load.py` & `log10_io-0.2.4/log10/load.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 load_dotenv()
 
 url = os.environ.get("LOG10_URL")
 token = os.environ.get("LOG10_TOKEN")
 org_id = os.environ.get("LOG10_ORG_ID")
 
 # log10, bigquery
-target_service = os.environ.get("LOG10_DATA_STORE")
+target_service = os.environ.get("LOG10_DATA_STORE", "log10")
 
 if target_service == "bigquery":
     from log10.bigquery import initialize_bigquery
     bigquery_client, bigquery_table = initialize_bigquery()
     import uuid
     from datetime import datetime, timezone
 elif target_service is None:
@@ -55,31 +55,41 @@
         raise Exception("Failed to create LOG10 session: " + str(e) + "\nLikely cause: LOG10 env vars missing or not picked up correctly!" +
                         "\nSee https://github.com/log10-io/log10#%EF%B8%8F-setup for details")
 
 
 # Global variable to store the current sessionID.
 sessionID = get_session_id()
 last_completion_response = None
-
+global_tags = []
 
 class log10_session:
+    def __init__(self, tags=None):
+         self.tags = tags
+
+         if tags is not None:
+            global global_tags
+            global_tags = tags
+
     def __enter__(self):
         global sessionID
         global last_completion_response
         sessionID = get_session_id()
         last_completion_response = None
         return self
 
     def last_completion_url(self):
         if last_completion_response is None:
             return None
 
         return url + '/app/' + last_completion_response['organizationSlug'] + '/completions/' + last_completion_response['completionID']
 
     def __exit__(self, exc_type, exc_value, traceback):
+        if self.tags is not None:
+            global global_tags
+            global_tags = None
         return
 
 
 @contextmanager
 def timed_block(block_name):
     if DEBUG:
         start_time = time.perf_counter()
@@ -117,15 +127,16 @@
         log_row = {
             # do we want to also store args?
             "status": "started",
             "orig_module": func.__module__,
             "orig_qualname": func.__qualname__,
             "request": json.dumps(kwargs),
             "session_id": sessionID,
-            "organization_id": org_id
+            "organization_id": org_id,
+            "tags": global_tags
         }
         if target_service == "log10":
             res = requests.request("POST",
                                    completion_url + "/" + completionID,
                                    headers={"x-log10-token": token,
                                             "Content-Type": "application/json"},
                                    json=log_row)
@@ -160,15 +171,16 @@
                            json={
                                # do we want to also store args?
                                "status": "started",
                                "orig_module": func.__module__,
                                "orig_qualname": func.__qualname__,
                                "request": json.dumps(kwargs),
                                "session_id": sessionID,
-                               "organization_id": org_id
+                               "organization_id": org_id,
+                               "tags": global_tags
                            })
     return completionID
 
 
 def intercepting_decorator(func):
     @functools.wraps(func)
     def wrapper(*args, **kwargs):
```

### Comparing `log10_io-0.2.3/log10/openai.py` & `log10_io-0.2.4/log10/openai.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.2.3/log10/tools.py` & `log10_io-0.2.4/log10/tools.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.2.3/log10/utils.py` & `log10_io-0.2.4/log10/utils.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.2.3/log10/agents/camel.py` & `log10_io-0.2.4/log10/agents/camel.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.2.3/log10/agents/scrape_summarizer.py` & `log10_io-0.2.4/log10/agents/scrape_summarizer.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.2.3/log10/schemas/bigquery.json` & `log10_io-0.2.4/log10/schemas/bigquery.json`

 * *Files identical despite different names*

### Comparing `log10_io-0.2.3/LICENSE` & `log10_io-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `log10_io-0.2.3/README.md` & `log10_io-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `log10_io-0.2.3/PKG-INFO` & `log10_io-0.2.4/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,32 @@
 Metadata-Version: 2.1
 Name: log10-io
-Version: 0.2.3
+Version: 0.2.4
 Summary: Unified LLM data management
-Project-URL: Homepage, https://github.com/log10-io/log10
-Project-URL: Bug Tracker, https://github.com/log10-io/log10/issues
-License-Expression: MIT
-License-File: LICENSE
+License: MIT
+Author: log10 team
+Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Dist: anthropic (>=0.3.6,<0.4.0)
+Requires-Dist: backoff (>=2.2.1,<3.0.0)
+Requires-Dist: faiss-cpu (>=1.7.4,<2.0.0)
+Requires-Dist: faker (>=19.2.0,<20.0.0)
+Requires-Dist: google-cloud-bigquery (>=3.11.4,<4.0.0)
+Requires-Dist: google-search-results (>=2.4.2,<3.0.0)
+Requires-Dist: langchain (>=0.0.242,<0.0.243)
+Requires-Dist: openai (>=0.27.8,<0.28.0)
+Requires-Dist: pexpect (>=4.8.0,<5.0.0)
+Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: tiktoken (>=0.4.0,<0.5.0)
+Requires-Dist: wikipedia (>=1.4.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # log10
 
 ⚡ Unified LLM data management ⚡
 
 [![pypi](https://github.com/log10-io/log10/actions/workflows/release.yml/badge.svg)](https://github.com/log10-io/log10/actions/workflows/release.yml)
@@ -83,7 +96,8 @@
 - `LOG10_TOKEN`: From the Settings tab in log10.io
 - `LOG10_ORG_ID`: From the Organization tab in log10.io
 - `OPENAI_API_KEY`: OpenAI API key
 
 ## 💬 Community
 
 We welcome community participation and feedback. Please leave an issue, submit a PR or join our [Discord](https://discord.gg/CZQvnuRV94).
+
```

