# Comparing `tmp/PenPen-AI-0.0.2.tar.gz` & `tmp/PenPen-AI-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PenPen-AI-0.0.2.tar", last modified: Tue Aug  1 18:13:38 2023, max compression
+gzip compressed data, was "PenPen-AI-0.0.3.tar", last modified: Tue Aug  1 18:15:14 2023, max compression
```

## Comparing `PenPen-AI-0.0.2.tar` & `PenPen-AI-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 mush       (501) staff       (20)        0 2023-08-01 18:13:38.392367 PenPen-AI-0.0.2/
--rw-r--r--   0 mush       (501) staff       (20)     1063 2023-07-31 13:37:35.000000 PenPen-AI-0.0.2/LICENSE
--rw-r--r--   0 mush       (501) staff       (20)     4625 2023-08-01 18:13:38.392217 PenPen-AI-0.0.2/PKG-INFO
-drwxr-xr-x   0 mush       (501) staff       (20)        0 2023-08-01 18:13:38.390603 PenPen-AI-0.0.2/PenPen_AI.egg-info/
--rw-r--r--   0 mush       (501) staff       (20)     4625 2023-08-01 18:13:38.000000 PenPen-AI-0.0.2/PenPen_AI.egg-info/PKG-INFO
--rw-r--r--   0 mush       (501) staff       (20)      456 2023-08-01 18:13:38.000000 PenPen-AI-0.0.2/PenPen_AI.egg-info/SOURCES.txt
--rw-r--r--   0 mush       (501) staff       (20)        1 2023-08-01 18:13:38.000000 PenPen-AI-0.0.2/PenPen_AI.egg-info/dependency_links.txt
--rw-r--r--   0 mush       (501) staff       (20)       61 2023-08-01 18:13:38.000000 PenPen-AI-0.0.2/PenPen_AI.egg-info/entry_points.txt
--rw-r--r--   0 mush       (501) staff       (20)       31 2023-08-01 18:13:38.000000 PenPen-AI-0.0.2/PenPen_AI.egg-info/requires.txt
--rw-r--r--   0 mush       (501) staff       (20)        7 2023-08-01 18:13:38.000000 PenPen-AI-0.0.2/PenPen_AI.egg-info/top_level.txt
--rw-r--r--   0 mush       (501) staff       (20)     4313 2023-08-01 18:13:20.000000 PenPen-AI-0.0.2/README.md
-drwxr-xr-x   0 mush       (501) staff       (20)        0 2023-08-01 18:13:38.391063 PenPen-AI-0.0.2/penpen/
--rw-r--r--   0 mush       (501) staff       (20)       71 2023-08-01 18:13:20.000000 PenPen-AI-0.0.2/penpen/__init__.py
-drwxr-xr-x   0 mush       (501) staff       (20)        0 2023-08-01 18:13:38.391965 PenPen-AI-0.0.2/penpen/openai_client/
--rw-r--r--   0 mush       (501) staff       (20)      228 2023-08-01 18:13:20.000000 PenPen-AI-0.0.2/penpen/openai_client/__init__.py
--rw-r--r--   0 mush       (501) staff       (20)     6586 2023-08-01 18:13:20.000000 PenPen-AI-0.0.2/penpen/openai_client/function_handling.py
--rw-r--r--   0 mush       (501) staff       (20)    18078 2023-08-01 18:13:20.000000 PenPen-AI-0.0.2/penpen/openai_client/openai_client.py
--rw-r--r--   0 mush       (501) staff       (20)      822 2023-08-01 18:13:20.000000 PenPen-AI-0.0.2/penpen/openai_client/openai_client_exceptions.py
--rw-r--r--   0 mush       (501) staff       (20)     1922 2023-08-01 18:13:20.000000 PenPen-AI-0.0.2/penpen/prompt_builder.py
--rw-r--r--   0 mush       (501) staff       (20)     9117 2023-08-01 18:13:20.000000 PenPen-AI-0.0.2/penpen/prompt_runner.py
--rw-r--r--   0 mush       (501) staff       (20)       38 2023-08-01 18:13:38.392423 PenPen-AI-0.0.2/setup.cfg
--rw-r--r--   0 mush       (501) staff       (20)      690 2023-08-01 18:13:20.000000 PenPen-AI-0.0.2/setup.py
+drwxr-xr-x   0 mush       (501) staff       (20)        0 2023-08-01 18:15:14.193596 PenPen-AI-0.0.3/
+-rw-r--r--   0 mush       (501) staff       (20)     1063 2023-07-31 13:37:35.000000 PenPen-AI-0.0.3/LICENSE
+-rw-r--r--   0 mush       (501) staff       (20)     4625 2023-08-01 18:15:14.193480 PenPen-AI-0.0.3/PKG-INFO
+drwxr-xr-x   0 mush       (501) staff       (20)        0 2023-08-01 18:15:14.192054 PenPen-AI-0.0.3/PenPen_AI.egg-info/
+-rw-r--r--   0 mush       (501) staff       (20)     4625 2023-08-01 18:15:14.000000 PenPen-AI-0.0.3/PenPen_AI.egg-info/PKG-INFO
+-rw-r--r--   0 mush       (501) staff       (20)      456 2023-08-01 18:15:14.000000 PenPen-AI-0.0.3/PenPen_AI.egg-info/SOURCES.txt
+-rw-r--r--   0 mush       (501) staff       (20)        1 2023-08-01 18:15:14.000000 PenPen-AI-0.0.3/PenPen_AI.egg-info/dependency_links.txt
+-rw-r--r--   0 mush       (501) staff       (20)       61 2023-08-01 18:15:14.000000 PenPen-AI-0.0.3/PenPen_AI.egg-info/entry_points.txt
+-rw-r--r--   0 mush       (501) staff       (20)       31 2023-08-01 18:15:14.000000 PenPen-AI-0.0.3/PenPen_AI.egg-info/requires.txt
+-rw-r--r--   0 mush       (501) staff       (20)        7 2023-08-01 18:15:14.000000 PenPen-AI-0.0.3/PenPen_AI.egg-info/top_level.txt
+-rw-r--r--   0 mush       (501) staff       (20)     4313 2023-08-01 18:13:20.000000 PenPen-AI-0.0.3/README.md
+drwxr-xr-x   0 mush       (501) staff       (20)        0 2023-08-01 18:15:14.192439 PenPen-AI-0.0.3/penpen/
+-rw-r--r--   0 mush       (501) staff       (20)       71 2023-08-01 18:13:20.000000 PenPen-AI-0.0.3/penpen/__init__.py
+drwxr-xr-x   0 mush       (501) staff       (20)        0 2023-08-01 18:15:14.193284 PenPen-AI-0.0.3/penpen/openai_client/
+-rw-r--r--   0 mush       (501) staff       (20)      228 2023-08-01 18:13:20.000000 PenPen-AI-0.0.3/penpen/openai_client/__init__.py
+-rw-r--r--   0 mush       (501) staff       (20)     6586 2023-08-01 18:13:20.000000 PenPen-AI-0.0.3/penpen/openai_client/function_handling.py
+-rw-r--r--   0 mush       (501) staff       (20)    18078 2023-08-01 18:13:20.000000 PenPen-AI-0.0.3/penpen/openai_client/openai_client.py
+-rw-r--r--   0 mush       (501) staff       (20)      822 2023-08-01 18:13:20.000000 PenPen-AI-0.0.3/penpen/openai_client/openai_client_exceptions.py
+-rw-r--r--   0 mush       (501) staff       (20)     1922 2023-08-01 18:13:20.000000 PenPen-AI-0.0.3/penpen/prompt_builder.py
+-rw-r--r--   0 mush       (501) staff       (20)     9117 2023-08-01 18:13:20.000000 PenPen-AI-0.0.3/penpen/prompt_runner.py
+-rw-r--r--   0 mush       (501) staff       (20)       38 2023-08-01 18:15:14.193647 PenPen-AI-0.0.3/setup.cfg
+-rw-r--r--   0 mush       (501) staff       (20)      690 2023-08-01 18:14:43.000000 PenPen-AI-0.0.3/setup.py
```

### Comparing `PenPen-AI-0.0.2/LICENSE` & `PenPen-AI-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `PenPen-AI-0.0.2/PKG-INFO` & `PenPen-AI-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PenPen-AI
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python package for standardizing prompts for LLMs.
 Home-page: https://github.com/qurami/PenPen
 Author: Ufirst S.r.l.
 License: MIT
 Keywords: LLM,GPT,prompting,ufirst
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `PenPen-AI-0.0.2/PenPen_AI.egg-info/PKG-INFO` & `PenPen-AI-0.0.3/PenPen_AI.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PenPen-AI
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python package for standardizing prompts for LLMs.
 Home-page: https://github.com/qurami/PenPen
 Author: Ufirst S.r.l.
 License: MIT
 Keywords: LLM,GPT,prompting,ufirst
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `PenPen-AI-0.0.2/README.md` & `PenPen-AI-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `PenPen-AI-0.0.2/penpen/openai_client/function_handling.py` & `PenPen-AI-0.0.3/penpen/openai_client/function_handling.py`

 * *Files identical despite different names*

### Comparing `PenPen-AI-0.0.2/penpen/openai_client/openai_client.py` & `PenPen-AI-0.0.3/penpen/openai_client/openai_client.py`

 * *Files identical despite different names*

### Comparing `PenPen-AI-0.0.2/penpen/openai_client/openai_client_exceptions.py` & `PenPen-AI-0.0.3/penpen/openai_client/openai_client_exceptions.py`

 * *Files identical despite different names*

### Comparing `PenPen-AI-0.0.2/penpen/prompt_builder.py` & `PenPen-AI-0.0.3/penpen/prompt_builder.py`

 * *Files identical despite different names*

### Comparing `PenPen-AI-0.0.2/penpen/prompt_runner.py` & `PenPen-AI-0.0.3/penpen/prompt_runner.py`

 * *Files identical despite different names*

### Comparing `PenPen-AI-0.0.2/setup.py` & `PenPen-AI-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read requirements.txt
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
 setup(
     name="PenPen-AI",
-    version="0.0.2",
+    version="0.0.3",
     packages=find_packages(),
     description="A Python package for standardizing prompts for LLMs.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Ufirst S.r.l.",
     url="https://github.com/qurami/PenPen",
     license="MIT",
```

